# Comparing `tmp/kperm-0.1.1.tar.gz` & `tmp/kperm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kperm-0.1.1.tar", max compression
+gzip compressed data, was "kperm-0.2.0.tar", max compression
```

## Comparing `kperm-0.1.1.tar` & `kperm-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      857 2023-05-23 10:57:26.822094 kperm-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-04-25 08:52:42.315245 kperm-0.1.1/LICENSE
--rw-r--r--   0        0        0     1052 2023-05-22 16:38:34.625707 kperm-0.1.1/README.md
--rw-r--r--   0        0        0       55 2023-05-19 10:26:30.107079 kperm-0.1.1/kperm/__init__.py
--rw-r--r--   0        0        0    39967 2023-05-22 16:38:14.577682 kperm-0.1.1/kperm/channel.py
--rw-r--r--   0        0        0    27977 2023-05-22 16:38:34.625707 kperm-0.1.1/kperm/permeation.py
--rw-r--r--   0        0        0     1029 2023-05-19 10:26:30.119079 kperm-0.1.1/kperm/utils.py
--rw-r--r--   0        0        0      587 2023-05-23 12:11:38.094907 kperm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1937 1970-01-01 00:00:00.000000 kperm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1610 2023-07-28 11:06:57.919820 kperm-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-04-25 08:52:42.315245 kperm-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1712 2023-07-28 16:09:19.170156 kperm-0.2.0/README.md
+-rw-r--r--   0        0        0       34 2023-07-28 07:28:29.376187 kperm-0.2.0/kperm/__init__.py
+-rw-r--r--   0        0        0     2952 2023-07-28 16:26:07.251585 kperm-0.2.0/kperm/__main__.py
+-rw-r--r--   0        0        0    39277 2023-07-28 16:48:41.813506 kperm-0.2.0/kperm/channel.py
+-rw-r--r--   0        0        0      785 2023-05-25 06:49:41.603406 kperm-0.2.0/kperm/examples.py
+-rw-r--r--   0        0        0    28620 2023-05-26 07:57:46.602396 kperm-0.2.0/kperm/permeation.py
+-rw-r--r--   0        0        0     1029 2023-05-19 10:26:30.119079 kperm-0.2.0/kperm/utils.py
+-rw-r--r--   0        0        0      951 2023-07-28 16:31:03.983974 kperm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2641 1970-01-01 00:00:00.000000 kperm-0.2.0/PKG-INFO
```

### Comparing `kperm-0.1.1/LICENSE` & `kperm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kperm-0.1.1/kperm/channel.py` & `kperm-0.2.0/kperm/channel.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,30 +3,34 @@
 The module contains the class Channel and core functions for analysizing
 ion permeation events in MD simulations using the KPERM framework.
 
 """
 import os
 import re
 import warnings
+from pathlib import Path
 
 import numpy as np
 import MDAnalysis as mda
 import pandas as pd
 from scipy.stats import bootstrap
 
 from kperm.permeation import _find_cycles, _compute_trans_prob, _plot_cycle, \
     _compute_mfpt, _plot_netflux, _count_perm_cross
 from kperm.utils import _write_list_of_tuples, _count_time, _create_logger
 
 warnings.simplefilter('always', DeprecationWarning)
 
 
 class Channel:
-    def __init__(self, coor=None, trajs=None):
-        self.coor = coor
+    """TBA.
+
+    """
+    def __init__(self, coord=None, trajs=None):
+        self.coord = coord
         self.trajs = trajs
         self.results_loc = []
         self.occupancy_4_all = []
         self.occupancy_6_all = []
         self.jumps_all = []
         self.cycles_all = []
         self.n_water_events = []
@@ -37,26 +41,59 @@
         self.current = None
         self.total_times = None
         self.stats = None
         self.permeation_idx_all = None
         self.cycle_prob = None
         self.main_path = None
 
+    def set_coord(self, coord):
+        coord = Path(coord)
+        assert coord.is_file(), "Input coordinate file does not exist."
+        self.coord = coord
+
+        print("Coordinate is set to:")
+        print("\t", coord)
+
+    def set_trajs(self, trajs):
+        if isinstance(trajs, str):
+            trajs = [trajs]
+        elif isinstance(trajs, list) and isinstance(trajs[0], str):
+            pass
+        else:
+            raise TypeError("Neither a string of a list of strings is provided.")
+
+        trajs = [Path(traj) for traj in trajs]
+        for traj in trajs:
+            assert traj.is_file(), f"Input trajectory {traj} does not exist."
+
+        self.trajs = trajs
+
+        print("Trajectories are set to:")
+        for traj in trajs:
+            print("\t", traj)
+
+    def detect_sf(self):
+        detect_sf(self.coord)
+
     def run(self, perm_count=("cross"), output="kperm",
-            perm_details=False, sf_diag=False):
+            perm_details=False, sf_diag=False, bs_radius=4.0, check_flip=True,
+            check_water=True):
         self.results_loc = []
 
         for traj in self.trajs:
             run(
-                self.coor,
+                self.coord,
                 traj,
                 perm_count=perm_count,
                 perm_details=perm_details,
                 output=output,
                 sf_diag=sf_diag,
+                bs_radius=bs_radius,
+                check_flip=check_flip,
+                check_water=check_water
             )
 
             self.results_loc.append(os.path.dirname(traj))
 
     def load(self, results_loc=None, filename="kperm"):
         jumps_all = []
         occupancy_4_all = []
@@ -170,22 +207,15 @@
         self.total_times = np.array(total_times)
         self.dts = np.array(dts)
         self.currents = np.array(currents)
         self.n_water_events = n_water_events
         self.n_k_events = n_k_events
 
     def compute_stats(self):
-        """
-        Parameters
-        ----------
-        channel: object
-            info about the channel, defined by the class Channel
-
-        save: string
-            save stats to the location specified
+        """Compute statistics of trajectories regarding ion permeation
 
         Returns
         -------
         stats: Pandas dataframe
             store statistics of trajectories, such as total time, lag time,
             current and occupation state populations.
 
@@ -264,33 +294,25 @@
 
         print(f"current (pA): {self.currents}")
         print(f"number of k permeation events: {self.n_k_events}")
         print(f"number of water permeation events: {self.n_water_events}")
         print(f"total time (ns): {self.total_times}")
         print(f"dt (ns): {self.dts}")
         print("coordinate:")
-        print(f"\t{self.coor}")
+        print(f"\t{self.coord}")
         print("trajectories:")
         if self.trajs is None:
             print(f"\t{self.trajs}")
         else:
             for traj in self.trajs:
                 print(f"\t{traj}")
         print("==============================")
 
         self.stats = stats
 
-    def computeStats(self, *args, **kwargs):
-        warnings.warn(
-            "computeStats() is renamed to compute_stats(). " +
-            "You are recommended to call <Channel>.compute_stats() instead. " +
-            "computeStats() will be removed in the future.",
-            DeprecationWarning)
-        return self.compute_stats(*args, **kwargs)
-
     def find_cycle(self, cycle_state, n_jump_per_cycle=5):
         if len(cycle_state) == 4:
             cycles, perm_idx_all, cycle_count_perc = _find_cycles(
                 self.occupancy_4_all, self.jumps_all, cycle_state,
                 n_jump_per_cycle=n_jump_per_cycle
             )
 
@@ -308,30 +330,14 @@
             raise ValueError("Input invalid.")
 
         cycles_flattened = [c for cycle in self.cycles_all for c in cycle]
         self.cycle_prob = _compute_trans_prob(cycles_flattened, quiet=True)
 
         return cycle_count_perc
 
-    def findCycles(self, *args, **kwargs):
-        warnings.warn(
-            "findCycles() is renamed to find_cycle(). " +
-            "You are recommended to call <Channel>.find_cycle() instead. " +
-            "findCycles() will be removed in the future.",
-            DeprecationWarning)
-        return self.find_cycle(*args, **kwargs)
-
-    def plotCycles(self, *args, **kwargs):
-        warnings.warn(
-            "plotCycles() is renamed to plot_cycle(). " +
-            "You are recommended to call <Channel>.plot_cycle() instead. " +
-            "plotCycles() will be removed in the future.",
-            DeprecationWarning)
-        return self.plot_cycle(*args, **kwargs)
-
     def plot_cycle(
         self,
         state_threshold=0.01,
         label_threshold=0.15,
         offset=0.7,
         scale=0.4,
         figsize=(6, 6)
@@ -344,25 +350,16 @@
             offset=offset,
             scale=scale,
             figsize=figsize,
             cycle_prob=True,
             main_cycle=True,
         )
 
-    def permeationMFPT(self, *args, **kwargs):
-        warnings.warn(
-            "permeationMFPT() is renamed to mfpt(). " +
-            "You are recommended to call <Channel>.mfpt() instead. " +
-            "permeationMFPT() will be removed in the future.",
-            DeprecationWarning)
-        return self.mfpt(*args, **kwargs)
-
     def mfpt(
         self,
-        dt=0.02,
         paths=None,
         n_jump_per_cycle=5,
         backward=False,
         batch=10000,
         n_resamples=10000,
     ):
         if paths is None:
@@ -372,42 +369,34 @@
 
         if len(paths[0][0][0]) == 4:
             mfpt, fps = _compute_mfpt(
                 self.occupancy_4_all,
                 self.jumps_all,
                 paths,
                 n_jump_per_cycle=n_jump_per_cycle,
-                dt=dt,
+                dt=self.dts[0],
                 backward=backward,
                 batch=batch,
                 n_resamples=n_resamples,
             )
         elif len(paths[0][0][0]) == 6:
             mfpt, fps = _compute_mfpt(
                 self.occupancy_6_all,
                 self.jumps_all,
                 paths,
                 n_jump_per_cycle=n_jump_per_cycle,
-                dt=dt,
+                dt=self.dts[0],
                 backward=backward,
                 batch=batch,
                 n_resamples=n_resamples,
             )
         else:
             raise ValueError("paths invalid.")
         return mfpt, fps
 
-    def plotNetFlux(self, *args, **kwargs):
-        warnings.warn(
-            "plotNetFlux() is renamed to plot_netflux(). " +
-            "You are recommended to call <Channel>.plot_netflux() instead. " +
-            "plotNetFlux() will be removed in the future.",
-            DeprecationWarning)
-        return self.plot_netflux(*args, **kwargs)
-
     def plot_netflux(self, weight_threshold=0.1, save=None, data=False,
                      returnGraphData=False):
         if returnGraphData is True:
             warnings.warn(
                 "returnGraphData is renamed to Data. " +
                 "You are recommended to use data=true instead. " +
                 "returnGraphData will be removed in the future.",
@@ -419,24 +408,15 @@
             self.occupancy_6_all,
             weight_threshold,
             save=save,
             data=data,
         )
 
 
-def detectSF(*args, **kwargs):
-    warnings.warn(
-        "detectSF() is renamed to detect_sf(). " +
-        "You are recommended to call detect_sf() instead. " +
-        "detectSF() will be removed in the future.",
-        DeprecationWarning)
-    return detect_sf(*args, **kwargs)
-
-
-def detect_sf(coor, quiet=False, o_cutoff=5, og1_cutoff=7.0, all_res=False):
+def detect_sf(coord, quiet=False, o_cutoff=5, og1_cutoff=7.0, all_res=False):
     """read coordinate file and return zero-indexed atom indices defining SF
 
     Parameters
     ----------
     coor : str
         The path to the coordinate file containing the ion channel.
     quiet : bool, optional
@@ -456,15 +436,15 @@
     -------
     sf_layer: dict
         consisting of two dictionaries containing atom idx (zero-based) and
         residue id of SF's oxygen (backbone and hydroxyl) and CA atoms,
         respectively.
 
     """
-    u = mda.Universe(coor, in_memory=False)
+    u = mda.Universe(coord, in_memory=False)
 
     # Finding backbone oxygen atoms that meet the geometric requirements
     if all_res:
         protein_o = u.select_atoms("protein and name O", updating=False)
     else:
         protein_o = u.select_atoms(
             "protein and name O and (resname GLY VAL TYR THR PHE ILE)",
@@ -594,29 +574,29 @@
                 print(
                     f"{idx}\t{layer}\t{chain_id}\t{resid}\t{resname}\t{name}"
                 )
 
     return sf_layer
 
 
-def _get_non_protein_index(coor):
+def _get_non_protein_index(coord):
     """read coordinate file and return zero-indexed atom indices defining SF
 
     Parameters
     ----------
-    coor : str
+    coord : str
         The path to the coordinate file containing the system
 
     Returns
     -------
     indices: tuple
         arrays of zero-indexed indices of K, Cl and water respectively
 
     """
-    u = mda.Universe(coor, in_memory=False)
+    u = mda.Universe(coord, in_memory=False)
 
     indices = (
         u.select_atoms("resname K POT", updating=False).ix,
         u.select_atoms("resname CL CLA", updating=False).ix,
         u.select_atoms("(resname SOL TIP3) and (name OH2 OW)",
                        updating=False).ix,
     )
@@ -627,15 +607,15 @@
 def _find_bound(positions, sol_indices, sf_o_indices, additional_bs_cutoff=4.0,
                 bs_radius=4.0):
     """read solute (K) or solvent (water) positions and assign their
     (zero-based) indicies to binding sites
 
     Parameters
     ----------
-    coor : str
+    coord : str
         The path to the coordinate file containing the system.
     sol_idx : array of int
         containing zero-based indices of particles such as oxygen of water,
         K and Cl.
     bs_layer_idx : 2-dimensional array of int
         containing zero-based indices of atoms of layers (from SF) defining
         the binding sites.
@@ -942,42 +922,49 @@
                     old_pos_idx = 5
                 jump += old_pos_idx - bs_i_t1
     return jump
 
 
 @_count_time
 def run(
-    coor,
+    coord,
     traj,
     output="kperm",
     perm_count=("cross"),
     perm_details=False,
     sf_idx=None,
     sf_all_res=False,
     sf_diag=False,
+    check_flip=False,
+    check_water=True,
     bs_radius=4.0,
 ):
+    print("Compute diagonal distance of SF backbone atoms:", sf_diag)
+    print("Check SF oxygen flip:", check_flip)
+    print("Check water occupancy and jump:", check_water)
+    print()
+
     path = os.path.dirname(traj)
 
     log_loc = os.path.abspath(os.path.join(path, output + ".log"))
 
     logger = _create_logger(log_loc)
 
-    print(f"Reading coordinate {coor}\nReading trajectory {traj}")
-    u = mda.Universe(coor, traj, in_memory=False)
+    print(f"Reading coordinate {coord}\nReading trajectory {traj}")
+    u = mda.Universe(coord, traj, in_memory=False)
 
     if sf_idx is None:
-        sf_idx = detect_sf(coor, quiet=True, all_res=sf_all_res)
+        sf_idx = detect_sf(coord, quiet=True, all_res=sf_all_res)
 
     sf_o_idx = np.array([sf_idx["O"][i]["idx"]
                         for i in range(len(sf_idx["O"]))])
     sf_ca_idx = np.array([sf_idx["CA"][i]["idx"]
                          for i in range(len(sf_idx["CA"]))])
 
-    k_idx, _, water_idx = _get_non_protein_index(coor)
+    k_idx, _, water_idx = _get_non_protein_index(coord)
 
     k_occupancy = []
     w_occupancy = []
 
     if perm_details:
         k_in_sf = []
         w_in_sf = []
@@ -994,23 +981,29 @@
             (len(u.trajectory), 2 * len(sf_ca_idx)), dtype=float)
 
     for ts in u.trajectory:
         if sf_diag:
             o_d_diag[ts.frame] = _compute_sf_diagonal(ts.positions, sf_o_idx)
             ca_d_diag[ts.frame] = _compute_sf_diagonal(
                 ts.positions, sf_ca_idx)
-
-        flips[ts.frame] = _check_flip(ts.positions, sf_o_idx)
+            
+        if check_flip:
+            flips[ts.frame] = _check_flip(ts.positions, sf_o_idx)
 
         k_occ = _find_bound(
             ts.positions, k_idx, sf_o_idx, bs_radius=bs_radius
         )
-        w_occ = _find_bound(
-            ts.positions, water_idx, sf_o_idx, bs_radius=bs_radius
-        )
+
+        if check_water:
+            w_occ = _find_bound(
+                ts.positions, water_idx, sf_o_idx, bs_radius=bs_radius
+            )
+        
+        else:
+            w_occ = [[] for _ in range(6)]
 
         k_occupancy.append(k_occ)
         w_occupancy.append(w_occ)
 
         if perm_details:
             # unwrap k_occ and w_occ for sf_occ_k.dat and sf_occ_w.dat
             k_occ_unwrap = [
```

### Comparing `kperm-0.1.1/kperm/permeation.py` & `kperm-0.2.0/kperm/permeation.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,16 +142,17 @@
                         found = True
                     elif (
                         n_k_jump <= -n_jump_per_cycle
                         or n_k_jump >= 2 * n_jump_per_cycle
                     ):
                         found = True
                         print(
-                            f"Not returning to {cycle_state}, \
-no cycle is formed"
+                            f"At frame {t}, number of jumps exceeds "
+                            f"{n_jump_per_cycle} but no cycle is detected as "
+                            f"SF does not return to {cycle_state}."
                         )
             t = t + T - 1
         t = t + 1
 
     perm_indices = np.array(perm_indices)
 
     return perm_indices
@@ -273,15 +274,15 @@
 
 
 def _compute_trans_prob(trajs, return_matrix=False, quiet=False):
     """given trajectories, compute transition probabilities
 
     Parameters
     ----------
-    trajs: list of arrays of size N    or   list of lists of arrays
+    trajs: list of arrays of size N or list of lists of arrays
         trajectories, can be occupancy or cycles for all trajectories
 
     return_matrix: boolean
         if True, return also the transition matrix and mapping between indices
         and state names
 
     quiet: boolean
@@ -377,14 +378,15 @@
     label_threshold=0.05,
     offset=0.1,
     scale=0.1,
     figsize=(10, 10),
     save=None,
     cycle_prob=False,
     main_cycle=False,
+    show=True
 ):
     """given trajectories, compute transition probabilities
 
     Parameters
     ----------
     cycles: list of lists of arrays
         contain the cycles identified in each trajectory
@@ -529,15 +531,19 @@
                         ax=None,
                         rotate=True,
                     )
     _ = plt.tight_layout()
     if save is not None:
         _ = plt.savefig(save, dpi=400)
         print(f"saved as {save}")
-    _ = plt.show()
+
+    if show:
+        _ = plt.show()
+    else:
+        plt.close("all")
 
     if main_cycle:
         transition_pairs = [[k] for k in sidechain.keys()]
         transition_pairs_tmp = [
             [transition_pairs[i], transition_pairs[i + 1]]
             for i in range(len(transition_pairs) - 1)
         ]
@@ -557,15 +563,15 @@
         final_states, n_jump_per_cycle=5, backward=False):
     """compute hitting time for transition pairs within one permeation event,
         i.e. abs(k_netjumps) < n_bs_jump+1
 
     Parameters
     ----------
     occupancy: array of size N
-        tranjectory expressed in the form of SF occupancy
+        a tranjectory expressed in the form of SF occupancy
 
     jumps: arrays of size (N-1, 2)
         net jumps for ion and water for one trajectory
 
     initial_states: list of strings
         the SF occupation state that the transitions start in
 
@@ -577,20 +583,20 @@
         Example:
             n_jump_per_cycle = 5 if only jumps from or to S1, S2, S3, and S4
             are considered.
 
     backward: boolean, False by default
         whether the hitting times corresponding to transitions in which the
         ion movement is against the gradient. If True, then only
-        transitions with +ve k_netjump are taken into account
+        transitions with positive k_netjump are taken into account
 
     Returns
     -------
     fpts: list of int
-        First passage time
+        First passage time, unit of time = 1
 
     k_netjumps_count: list of int
         # net k jumps involved in the transitions
 
     w_netjumps_count: list of int
         # net water jumps involved in the transitions
     """
@@ -599,16 +605,17 @@
     fpts = []
 
     # count number of k and w jumps happening during the period for which
     # hitting times are computed
     k_netjumps_counts = []
     w_netjumps_counts = []
 
-    k_netjumps = jumps[:, 0]
-    w_netjumps = jumps[:, 1]
+    if jumps is not None:
+        k_netjumps = jumps[:, 0]
+        w_netjumps = jumps[:, 1]
 
     waiting = False
     passage_time = 0
 
     # count for each initial state to avoid overlooking some of the initial
     # states in scenario like
     #    initialState_1 -> xxx -> initialState_2 -> xxx -> finalState_2
@@ -618,14 +625,15 @@
             if s in int_states and waiting is False:
                 waiting = True
                 start_idx = i
             elif s in final_states and waiting is True:
                 end_idx = i
                 if jumps is None:
                     k_netjump = 0
+                    w_netjump = 0
                 else:
                     k_netjump = int(np.sum(k_netjumps[start_idx:end_idx]))
                     w_netjump = int(np.sum(w_netjumps[start_idx:end_idx]))
 
                 # restrict the scope to transitions within one permeation
                 # event, i.e. 0 <= abs(k_netjump) < n_jump_per_cycle
                 if (
@@ -654,15 +662,15 @@
 
 
 def _compute_mfpt(
     occupancy_all,
     jumps_all,
     pairs,
     n_jump_per_cycle=5,
-    dt=0.02,
+    dt=1,
     backward=False,
     batch=10000,
     n_resamples=10000,
 ):
     """compute mean first passage times (MFPTs) for all transition pairs
 
     Parameters
@@ -684,19 +692,26 @@
         Example:
             n_jump_per_cycle = 5 if only jumps from or to S1, S2, S3, and S4
             are considered.
 
     dt: float
         lag time in ns
 
+    backward: boolean, False by default
+        whether the hitting times corresponding to transitions in which the
+        ion movement is against the gradient. If True, then only
+        transitions with positive k_netjump are taken into account
+
     Returns
     -------
     df: Pandas dataframe
         all computed mean first passage times
     """
+    print(f"df = {dt} is used for the MFPT calculation.")
+
     data = []
     hts_output = {}
     for initial_states, final_states in pairs:
         fpts_all = []
         k_j_counts_all = []
         w_j_counts_all = []
         initial_states_label = ",".join(initial_states)
@@ -757,27 +772,27 @@
         data.append(row)
 
     df = pd.DataFrame(
         data,
         columns=[
             "initial",
             "final",
-            "mean (ns)",
-            "low (ns)",
-            "high (ns)",
+            "mfpt",
+            "mfpt_l",
+            "mfpt_h",
             "n",
             "k_f",
             "w_f",
         ],
     )
     return df, hts_output
 
 
 def _plot_netflux(occupancy_all, weight_threshold=0.1,
-                  save=None, data=False):
+                  save=None, data=False, show=True):
     """plot net fluxes
 
     Parameters
     ----------
     occupancy_all: list of arrays of size N
         all tranjectories expressed in the form of SF occupancy
 
@@ -863,11 +878,15 @@
         edgelist=list(edges_weights_trunc_norm),
         alpha=[e[-1] for e in edges_weights_trunc_norm],
     )
 
     if save is not None:
         _ = plt.savefig(save, dpi=300)
         print(f"saved as {save}")
-    _ = plt.show()
+
+    if show:
+        plt.show()
+    else:
+        plt.close("all")
 
     if data:
         return states_probs_full, edges_weights_full_positive
```

### Comparing `kperm-0.1.1/kperm/utils.py` & `kperm-0.2.0/kperm/utils.py`

 * *Files identical despite different names*

### Comparing `kperm-0.1.1/pyproject.toml` & `kperm-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,47 @@
 [tool.poetry]
 name = "kperm"
-version = "0.1.1"
+version = "0.2.0"
 description = "Toolkit for Analysis of Permeation Cycles in Potassium Channels"
 authors = ["Chun Kei (Tom) Lam <chun-kei.lam@mpinat.mpg.de>"]
 license = "GPL-3.0"
 readme = "README.md"
 include = ["CHANGELOG.md"]
 
-
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 numpy = "^1.24.3"
 MDAnalysis = "^2.4.3"
 matplotlib = "^3.7.1"
 pandas = "^2.0.1"
 networkx = "^3.1"
 scipy = "^1.10.1"
 jupyter = "^1.0.0"
+argcomplete = "^3.0.8"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
+sphinx = "^7.0.1"
+coverage = {extras = ["toml"], version = "^7.2.6"}
+pytest-cov = "^4.1.0"
+
+
+[tool.coverage.paths]
+source = ["kperm"]
 
+[tool.coverage.run]
+branch = true
+source = ["kperm"]
+
+[tool.coverage.report]
+show_missing = true
+
+[[tool.poetry.source]]
+name = "PyPI"
+priority = "primary"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+kperm = "kperm.__main__:main"
```

### Comparing `kperm-0.1.1/PKG-INFO` & `kperm-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,65 @@
 Metadata-Version: 2.1
 Name: kperm
-Version: 0.1.1
+Version: 0.2.0
 Summary: Toolkit for Analysis of Permeation Cycles in Potassium Channels
 License: GPL-3.0
 Author: Chun Kei (Tom) Lam
 Author-email: chun-kei.lam@mpinat.mpg.de
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: MDAnalysis (>=2.4.3,<3.0.0)
+Requires-Dist: argcomplete (>=3.0.8,<4.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # KPerm - Toolkit for Analysis of Permeation Cycles in Potassium Channels
 
+[![License](https://img.shields.io/github/license/deGrootLab/KPerm)](https://www.gnu.org/licenses/gpl-3.0.en.html) [![PyPI](https://img.shields.io/pypi/v/kperm?color=green)](https://pypi.org/project/kperm/) [![DOI](https://img.shields.io/badge/DOI-10.1021%2Facs.jctc.3c00061-purple)](https://dx.doi.org/10.1021/acs.jctc.3c00061)
 
-[![License](https://img.shields.io/github/license/deGrootLab/KPerm)](https://www.gnu.org/licenses/gpl-3.0.en.html) [![DOI](https://img.shields.io/badge/DOI-10.1021%2Facs.jctc.3c00061-purple)](https://pubs.acs.org/doi/10.1021/acs.jctc.3c00061)
+KPerm, released together with our [JCTC](https://dx.doi.org/10.1021/acs.jctc.3c00061) paper, is a Python package specifically for identifying selecivity filter occupancy in molecular dynamics (MD) simulations of potassium channels.
 
-This package allows you to identify permeation cycles in potassium channels from molecular dynamics (MD) simulation trajectories.
+## Installation
 
-## Conda
-You are recommended to install KPerm in a conda environment. If you have installed [Anaconda](https://www.anaconda.com/), create a new environment by running:
+You are recommended to install the latest release of KPerm via `pip` in a virtual environment with Python >=3.8.
 
 ```bash
-conda create -n kperm python=3.11
+pip install kperm
 ```
 
-Once the environment is set up, run:
-```bash
-conda activate kperm
-```
-## Installation
-Tested with Python 3.11, MDAnalysis 2.4.2, and Numpy 1.24.1.
+## Examples
+
+### Jupyter Notebook
+
+- [Permeation Cycle in MthK with charge-scaling](./docs/notebooks/charge-scaling.ipynb)
+
+### Command-line Interface
 ```bash
-git clone https://github.com/tomcklam/KPerm
-cd KPerm
-pip install .
-# you may need to add the kernel
-# ipython kernel install --name "kperm" --user
+# same as Channel.run(), computing SF occuapncy and identifying permeation events
+kperm run -s coord_file -f traj_1 traj_2 traj_3 ...
+
+# speed things up if you are not interested in SF oxygen flip and water occupancy
+kperm run -s coord_file -f traj_1 traj_2 traj_3 ... --noFlip --noW
+
+# compute summary of permeation events of all selected simulations 
+# use it after running "kperm run"
+kperm stats -s coord_file -f traj_1 traj_2 traj_3 ...
 ```
 
-You can now try our tutorial (tutorials/charge-scaling/charge-scaling.ipynb).
+## Documentation
+
+https://degrootlab.github.io/KPerm/
+
+## Citation
+
+- Lam, C. K., & de Groot, B. L. (2023). Ion Conduction Mechanisms in Potassium Channels Revealed by Permeation Cycles. Journal of Chemical Theory and Computation.doi:[10.1021/acs.jctc.3c00061](https://dx.doi.org/10.1021/acs.jctc.3c00061)
```

