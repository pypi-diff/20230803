# Comparing `tmp/ansys-dpf-post-0.4.0.tar.gz` & `tmp/ansys_dpf_post-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-dpf-post-0.4.0.tar", last modified: Tue Apr  4 13:44:49 2023, max compression
+gzip compressed data, was "ansys_dpf_post-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys-dpf-post-0.4.0.tar` & `ansys_dpf_post-0.5.0.tar`

### file list

```diff
@@ -1,39 +1,49 @@
--rw-r--r--   0        0        0     1066 2023-04-04 13:44:39.165341 ansys-dpf-post-0.4.0/LICENSE
--rw-r--r--   0        0        0     3807 2023-04-04 13:44:39.165341 ansys-dpf-post-0.4.0/README.md
--rw-r--r--   0        0        0     1567 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1929 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/__init__.py
--rw-r--r--   0        0        0     4721 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/common.py
--rw-r--r--   0        0        0    42974 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/dataframe.py
--rw-r--r--   0        0        0     1042 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/displacement.py
--rw-r--r--   0        0        0     2706 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/dpf_path.py
--rwxr-xr-x   0        0        0    15830 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/dpf_solution.py
--rwxr-xr-x   0        0        0     1532 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/electric_results.py
--rwxr-xr-x   0        0        0     1519 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/errors.py
--rw-r--r--   0        0        0      433 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/examples/__init__.py
--rw-r--r--   0        0        0      287 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/harmonic_analysis.py
--rw-r--r--   0        0        0   137646 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/harmonic_mechanical_simulation.py
--rw-r--r--   0        0        0    11513 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/index.py
--rw-r--r--   0        0        0     1162 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/mesh.py
--rw-r--r--   0        0        0     2117 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/misc.py
--rwxr-xr-x   0        0        0    31320 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/misc_results.py
--rw-r--r--   0        0        0      276 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/modal_analysis.py
--rw-r--r--   0        0        0   174286 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/modal_mechanical_simulation.py
--rw-r--r--   0        0        0    10113 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/post_utility.py
--rwxr-xr-x   0        0        0    15062 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/result_data.py
--rw-r--r--   0        0        0    10026 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/result_definition.py
--rwxr-xr-x   0        0        0    14351 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/result_evaluation.py
--rwxr-xr-x   0        0        0     3491 2023-04-04 13:44:39.173341 ansys-dpf-post-0.4.0/src/ansys/dpf/post/result_object.py
--rw-r--r--   0        0        0     1357 2023-04-04 13:44:39.177342 ansys-dpf-post-0.4.0/src/ansys/dpf/post/scalar.py
--rw-r--r--   0        0        0    18920 2023-04-04 13:44:39.177342 ansys-dpf-post-0.4.0/src/ansys/dpf/post/selection.py
--rw-r--r--   0        0        0    29027 2023-04-04 13:44:39.177342 ansys-dpf-post-0.4.0/src/ansys/dpf/post/simulation.py
--rw-r--r--   0        0        0      429 2023-04-04 13:44:39.177342 ansys-dpf-post-0.4.0/src/ansys/dpf/post/static_analysis.py
--rw-r--r--   0        0        0   233095 2023-04-04 13:44:39.177342 ansys-dpf-post-0.4.0/src/ansys/dpf/post/static_mechanical_simulation.py
--rw-r--r--   0        0        0     1748 2023-04-04 13:44:39.177342 ansys-dpf-post-0.4.0/src/ansys/dpf/post/strain.py
--rw-r--r--   0        0        0     1847 2023-04-04 13:44:39.177342 ansys-dpf-post-0.4.0/src/ansys/dpf/post/stress.py
--rw-r--r--   0        0        0     2440 2023-04-04 13:44:39.177342 ansys-dpf-post-0.4.0/src/ansys/dpf/post/temperature.py
--rw-r--r--   0        0        0     9225 2023-04-04 13:44:39.177342 ansys-dpf-post-0.4.0/src/ansys/dpf/post/tensor.py
--rw-r--r--   0        0        0     1311 2023-04-04 13:44:39.177342 ansys-dpf-post-0.4.0/src/ansys/dpf/post/tools.py
--rw-r--r--   0        0        0      451 2023-04-04 13:44:39.177342 ansys-dpf-post-0.4.0/src/ansys/dpf/post/transient_analysis.py
--rw-r--r--   0        0        0   167539 2023-04-04 13:44:39.177342 ansys-dpf-post-0.4.0/src/ansys/dpf/post/transient_mechanical_simulation.py
--rw-r--r--   0        0        0     5785 2023-04-04 13:44:39.177342 ansys-dpf-post-0.4.0/src/ansys/dpf/post/vector.py
--rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 ansys-dpf-post-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-03 10:40:17.294318 ansys_dpf_post-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4299 2023-08-03 10:40:17.294318 ansys_dpf_post-0.5.0/README.md
+-rw-r--r--   0        0        0     1518 2023-08-03 10:40:17.298318 ansys_dpf_post-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2300 2023-08-03 10:40:17.298318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/__init__.py
+-rw-r--r--   0        0        0     5184 2023-08-03 10:40:17.298318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/common.py
+-rw-r--r--   0        0        0     4878 2023-08-03 10:40:17.298318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/connectivity.py
+-rw-r--r--   0        0        0    46448 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/dataframe.py
+-rw-r--r--   0        0        0     1042 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/displacement.py
+-rw-r--r--   0        0        0     2706 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/dpf_path.py
+-rwxr-xr-x   0        0        0    15841 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/dpf_solution.py
+-rwxr-xr-x   0        0        0     1532 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/electric_results.py
+-rw-r--r--   0        0        0     7761 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/elements.py
+-rwxr-xr-x   0        0        0     1519 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/errors.py
+-rw-r--r--   0        0        0      433 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/examples/__init__.py
+-rw-r--r--   0        0        0     5076 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/faces.py
+-rw-r--r--   0        0        0   386032 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/fluid_simulation.py
+-rw-r--r--   0        0        0      287 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/harmonic_analysis.py
+-rw-r--r--   0        0        0   165307 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/harmonic_mechanical_simulation.py
+-rw-r--r--   0        0        0    12316 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/index.py
+-rw-r--r--   0        0        0    20305 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/mesh.py
+-rw-r--r--   0        0        0     7123 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/mesh_info.py
+-rw-r--r--   0        0        0     6218 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/meshes.py
+-rw-r--r--   0        0        0     2117 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/misc.py
+-rwxr-xr-x   0        0        0    31334 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/misc_results.py
+-rw-r--r--   0        0        0      276 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/modal_analysis.py
+-rw-r--r--   0        0        0   212763 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/modal_mechanical_simulation.py
+-rw-r--r--   0        0        0     4735 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/named_selection.py
+-rw-r--r--   0        0        0     4177 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/nodes.py
+-rw-r--r--   0        0        0     3069 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/phase.py
+-rw-r--r--   0        0        0    10862 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/post_utility.py
+-rwxr-xr-x   0        0        0    15063 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/result_data.py
+-rw-r--r--   0        0        0    10026 2023-08-03 10:40:17.302318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/result_definition.py
+-rwxr-xr-x   0        0        0    14351 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/result_evaluation.py
+-rwxr-xr-x   0        0        0     3491 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/result_object.py
+-rw-r--r--   0        0        0     1357 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/scalar.py
+-rw-r--r--   0        0        0    37947 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/selection.py
+-rw-r--r--   0        0        0    39781 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/simulation.py
+-rw-r--r--   0        0        0     3091 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/species.py
+-rw-r--r--   0        0        0      429 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/static_analysis.py
+-rw-r--r--   0        0        0   283854 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/static_mechanical_simulation.py
+-rw-r--r--   0        0        0     1748 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/strain.py
+-rw-r--r--   0        0        0     1847 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/stress.py
+-rw-r--r--   0        0        0     2440 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/temperature.py
+-rw-r--r--   0        0        0     9225 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/tensor.py
+-rw-r--r--   0        0        0     1312 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/tools.py
+-rw-r--r--   0        0        0      451 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/transient_analysis.py
+-rw-r--r--   0        0        0   213701 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/transient_mechanical_simulation.py
+-rw-r--r--   0        0        0     5785 2023-08-03 10:40:17.306318 ansys_dpf_post-0.5.0/src/ansys/dpf/post/vector.py
+-rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 ansys_dpf_post-0.5.0/PKG-INFO
```

### Comparing `ansys-dpf-post-0.4.0/LICENSE` & `ansys_dpf_post-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/README.md` & `ansys_dpf_post-0.5.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,103 @@
-# PyDPF-Post - Ansys Data Post-Processing Framework
+# PyDPF-Post - Ansys Data PostProcessing Framework
 [![PyAnsys](https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC)](https://docs.pyansys.com/)
 [![Python](https://img.shields.io/pypi/pyversions/ansys-dpf-post?logo=pypi)](https://pypi.org/project/ansys-dpf-post/)
 [![pypi](https://badge.fury.io/py/ansys-dpf-post.svg?logo=python&logoColor=white)](https://pypi.org/project/ansys-dpf-post)
 [![MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-The Data Processing Framework (DPF) is designed to provide numerical
-simulation users/engineers with a toolbox for accessing and
+The Ansys Data Processing Framework (DPF) is designed to provide numerical
+simulation users and engineers with a toolbox for accessing and
 transforming simulation data.
 
-The Python `ansys-dpf-post` package provides a high level, physics oriented API for postprocessing.
+The Python `ansys-dpf-post` package provides a high-level, physics-oriented API for postprocessing.
 Loading a simulation (defined by its result files) allows you to extract simulation metadata as well
-as results and apply postprocessing operations on it.
+as results and then apply postprocessing operations on it.
 
-This module leverages the PyDPF-Core project's ``ansys-dpf-core`` package and can
-be found by visiting [PyDPF-Core
-GitHub](https://github.com/pyansys/pydpf-core).  Use ``ansys-dpf-core`` for
-building more advanced and customized workflows using Ansys DPF.
+The latest version of DPF supports Ansys solver result files for:
+
+  - MAPDL (`.rst`, `.mode`, `.rfrq`, `.rdsp`)
+  - LS-DYNA (`.d3plot`, `.binout`)
+  - Fluent (`.cas/dat.h5`, `.flprj`)
+  - CFX (`.cad/dat.cff`, `.flprj`)
+
+See the `PyDPF-Core main page <https://dpf.docs.pyansys.com/version/stable/index.html>`_
+for more information on compatibility.
+
+This module leverages the PyDPF-Core project's ``ansys-dpf-core`` package, which is
+available at [PyDPF-Core GitHub](https://github.com/ansys/pydpf-core).
+Use the ``ansys-dpf-core`` package for building more advanced and customized workflows
+using Ansys DPF.
 
 ## Documentation
 
-Visit the [PyDPF-Post Documentation](https://postdocs.pyansys.com) for a
-detailed description of the package, or see the [Examples
-Gallery](https://postdocs.pyansys.com/examples/index.html) for more
-detailed examples.
+For comprehensive information on this package, see the [PyDPF-Post Documentation](https://post.docs.pyansys.com),
+For detailed how-to information, see the [Examples](https://post.docs.pyansys.com/version/stable/examples/index.html)
+in the PyDPF-Post documentation.
 
 ## Installation
 
-Install this repository with:
+To install this package, use this command:
 
 ```
 pip install ansys-dpf-post
 ```
 
-You can also clone and install this repository with:
+You can also clone and install this package with this code:
 
 ```
-git clone https://github.com/pyansys/pydpf-post
+git clone https://github.com/ansys/pydpf-post
 cd pydpf-post
 pip install . --user
 ```
 
-## Brief Demo
+## Brief demo
 
-Provided you have ANSYS 2023 R1 installed, a DPF server starts
+Provided you have Ansys 2023 R1 or later installed, a DPF server starts
 automatically once you start using PyDPF-Post.
-Loading a simulation to extract and post-process results:
+
+To load a simulation to extract and post-process results, use this code:
 
 ```pycon
 >>> from ansys.dpf import post
 >>> from ansys.dpf.post import examples
 >>> simulation = post.load_simulation(examples.download_crankshaft())
 >>> displacement = simulation.displacement()
 >>> print(displacement)
 ```
 ```pycon
-             results         U
-              set_id         3
-      node      comp          
-      4872         X -3.41e-05
-                   Y  1.54e-03
-                   Z -2.64e-06
-      9005         X -5.56e-05
-                   Y  1.44e-03
-                   Z  5.31e-06
-       ...
+             results       U (m)
+             set_ids           3
+ node_ids components            
+     4872          X -3.4137e-05
+                   Y  1.5417e-03
+                   Z -2.6398e-06
+     9005          X -5.5625e-05
+                   Y  1.4448e-03
+                   Z  5.3134e-06
+      ...        ...         ...
 ```
 ```pycon
 >>> displacement.plot()
 ```
-![Example Displacement plot Crankshaft](https://github.com/pyansys/dpf-post/raw/master/docs/source/images/crankshaft_disp.png)
+![Example Displacement plot Crankshaft](https://github.com/ansys/pydpf-post/raw/master/docs/source/images/crankshaft_disp.png)
 ```pycon
 >>> stress_eqv = simulation.stress_eqv_von_mises_nodal()
 >>> stress_eqv.plot()
 ```
-![Example Stress plot Crankshaft](https://github.com/pyansys/dpf-post/raw/master/docs/source/images/crankshaft_stress.png)
+![Example Stress plot Crankshaft](https://github.com/ansys/pydpf-post/raw/master/docs/source/images/crankshaft_stress.png)
 
-To run PyDPF-Post with Ansys versions starting from 2021 R1 to 2022 R2, use the following legacy PyDPF-Post 
-tools:
+To run PyDPF-Post with Ansys versions 2021 R1 and 2022 R2, use this code to
+start the legacy PyDPF-Post tools::
 
 ```pycon
 >>> from ansys.dpf import post
 >>> from ansys.dpf.post import examples
 >>> solution = post.load_solution(examples.download_crankshaft())
 >>> stress = solution.stress()
 >>> stress.eqv.plot_contour(show_edges=False)
 ```
-![Example Stress plot Crankshaft](https://github.com/pyansys/dpf-post/raw/master/docs/source/images/crankshaft_stress.png)
+![Example Stress plot Crankshaft](https://github.com/ansys/pydpf-post/raw/master/docs/source/images/crankshaft_stress.png)
 
 ## License
 
-``PyDPF-Post`` is licensed under the MIT license.  For more information, see the
-[LICENSE](https://github.com/pyansys/dpf-post/raw/master/LICENSE).
+``PyDPF-Post`` is licensed under the MIT license. For more information, see the
+[LICENSE](https://github.com/ansys/pydpf-post/raw/master/LICENSE).
```

### Comparing `ansys-dpf-post-0.4.0/pyproject.toml` & `ansys_dpf_post-0.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-dpf-post"
-version = "0.4.0"
+version = "0.5.0"
 description = "PyDPF-Post Python library."
 readme = "README.md"
-requires-python = ">=3.7.*,<4.0"
+requires-python = ">=3.8,<4.0"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
 maintainers = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -23,26 +23,25 @@
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Information Analysis",
 ]
 
 [tool.flit.module]
 name = "ansys.dpf.post"
 
 [project.urls]
-Source = "https://github.com/pyansys/pydpf-post"
+Source = "https://github.com/ansys/pydpf-post"
 
 [project.optional-dependencies]
 plotting = [
     "pyvista>=0.24.0",
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/__init__.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,30 +21,35 @@
 from ansys.dpf.core.common import locations, shell_layers  # noqa: F401
 
 try:
     import importlib.metadata as importlib_metadata
 except ModuleNotFoundError:  # pragma: no cover
     import importlib_metadata
 
-from ansys.dpf.post import mesh, selection, tools
-from ansys.dpf.post.common import Grouping as grouping
+from ansys.dpf.post import mesh, selection, tools  # noqa: F401
+from ansys.dpf.post.common import Grouping as grouping  # noqa: F401
 from ansys.dpf.post.dataframe import DataFrame  # noqa: F401
-from ansys.dpf.post.dpf_path import create_path_on_coordinates
+from ansys.dpf.post.dpf_path import create_path_on_coordinates  # noqa: F401
+from ansys.dpf.post.fluid_simulation import FluidSimulation  # noqa: F401
 from ansys.dpf.post.harmonic_mechanical_simulation import (  # noqa: F401
     HarmonicMechanicalSimulation,
 )
+from ansys.dpf.post.mesh import Mesh  # noqa: F401
+from ansys.dpf.post.meshes import Meshes  # noqa: F401
 from ansys.dpf.post.misc import Report
 from ansys.dpf.post.modal_mechanical_simulation import (  # noqa: F401
     ModalMechanicalSimulation,
 )
-from ansys.dpf.post.post_utility import (
+from ansys.dpf.post.phase import Phase, PhasesDict  # noqa: F401
+from ansys.dpf.post.post_utility import (  # noqa: F401
     load_simulation,
     load_solution,
     print_available_keywords,
 )
+from ansys.dpf.post.species import Species, SpeciesDict  # noqa: F401
 from ansys.dpf.post.static_mechanical_simulation import (  # noqa: F401
     StaticMechanicalSimulation,
 )
 from ansys.dpf.post.transient_mechanical_simulation import (  # noqa: F401
     TransientMechanicalSimulation,
 )
```

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/common.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """Module containing the common tools for a better usage of the PyDPF-Post module.
 
 Common
 ------
 
 """
+from ansys.dpf.core.common import (  # noqa: F401  # pylint: disable=W0611
+    elemental_properties,
+)
 
+from ansys.dpf.post.fluid_simulation import FluidSimulation
 from ansys.dpf.post.harmonic_mechanical_simulation import HarmonicMechanicalSimulation
 from ansys.dpf.post.modal_mechanical_simulation import ModalMechanicalSimulation
 from ansys.dpf.post.static_mechanical_simulation import StaticMechanicalSimulation
 from ansys.dpf.post.transient_mechanical_simulation import TransientMechanicalSimulation
 
 # class ElShapes(Enum):
 #     """Class with Enum inheritance. This class must be used to
@@ -114,35 +118,42 @@
     """
 
     static = "static"
     modal = "modal"
     harmonic = "harmonic"
     transient = "transient"
     msup = "MSUP"
+    steady = "steady"
+    unsteady = "unsteady"
 
 
 class _PhysicsType:
     """Contains names of Python physics types.
 
     For developer usage.
     """
 
     mechanical = "mechanical"
     mecanic = "mecanic"  # Keep for retro-compatibility with ANSYS < 231
     thermal = "thermal"
+    fluid = "fluid"
 
 
 class AvailableSimulationTypes:
     """Contains available simulation types to give the :func:`load_simulation` function."""
 
     static_mechanical = "static mechanical"  # StaticMechanicalSimulation
     transient_mechanical = "transient mechanical"  # TransientMechanicalSimulation
     modal_mechanical = "modal mechanical"  # ModalMechanicalSimulation
     harmonic_mechanical = "harmonic mechanical"  # HarmonicMechanicalSimulation
+    steady_fluid = "steady fluid"  # FluidSimulation
+    unsteady_fluid = "unsteady fluid"  # FluidSimulation
 
 
 simulation_type_str_to_class = {
     AvailableSimulationTypes.static_mechanical: StaticMechanicalSimulation,
     AvailableSimulationTypes.transient_mechanical: TransientMechanicalSimulation,
     AvailableSimulationTypes.modal_mechanical: ModalMechanicalSimulation,
     AvailableSimulationTypes.harmonic_mechanical: HarmonicMechanicalSimulation,
+    AvailableSimulationTypes.steady_fluid: FluidSimulation,
+    AvailableSimulationTypes.unsteady_fluid: FluidSimulation,
 }
```

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/dataframe.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/dataframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,39 +10,43 @@
 from os import PathLike
 from typing import List, Union
 import warnings
 
 import ansys.dpf.core as dpf
 from ansys.dpf.core.dpf_array import DPFArray
 from ansys.dpf.core.plotter import DpfPlotter
+from ansys.dpf.core.property_fields_container import (
+    _MockPropertyFieldsContainer as PropertyFieldsContainer,
+)
+import ansys.dpf.gate.errors
 import numpy as np
 
 from ansys.dpf.post import locations, shell_layers
 from ansys.dpf.post.index import (
     CompIndex,
+    ElementNodeIndex,
     Index,
     LabelIndex,
     MeshIndex,
     MultiIndex,
     ResultsIndex,
     SetIndex,
     ref_labels,
 )
 
-display_width = 100
-display_max_colwidth = 12
-display_max_lines = 6
+default_display_max_columns = 6
+default_display_max_rows = 6
 
 
 class DataFrame:
     """A DataFrame style API to manipulate DPF data."""
 
     def __init__(
         self,
-        data: dpf.FieldsContainer,
+        data: Union[dpf.FieldsContainer, PropertyFieldsContainer],
         index: Union[MultiIndex, Index, List[int]],
         columns: Union[MultiIndex, Index, List[str], None] = None,
     ):
         """Creates a DPF DataFrame based on the given input data.
 
         Parameters
         ----------
@@ -50,15 +54,17 @@
             Data to use.
         index:
             Row indexing (labels) to use.
         columns:
             Column indexing (labels) to use.
         """
         self._index = index
-        if isinstance(data, dpf.FieldsContainer):
+        if isinstance(data, dpf.FieldsContainer) or isinstance(
+            data, PropertyFieldsContainer
+        ):
             self._fc = data
             # if index is None:
             #     raise NotImplementedError("Creation from FieldsContainer without index "
             #                               "is not yet supported")
             #     # self._index = Index(
             #     #     name=location_to_label[data[0].location], values=None
             #     # )
@@ -67,23 +73,52 @@
                 f"Input data type '{type(data)}' is not a valid data type for DataFrame creation."
             )
         if columns is not None:
             self._columns = columns
         else:
             self._columns = None
 
+        # If MeshIndex is elemental nodal, update columns
+        for i in self.index:
+            if isinstance(i, MeshIndex):
+                if i.location == locations.elemental_nodal:
+                    # Update columns with a dynamic node index
+                    self.columns.indexes.append(ElementNodeIndex())
+
         self._disp_wf = None
 
         self._str = None
-        self._last_display_width = display_width
-        self._last_display_max_colwidth = display_max_colwidth
+        self._display_max_columns = default_display_max_columns
+        self._display_max_rows = default_display_max_rows
+        self._last_display_max_columns = self._display_max_columns
+        self._last_display_max_rows = self._display_max_rows
 
         self._last_minmax: dict = {"axis": None, "min": None, "max": None}
 
     @property
+    def display_max_columns(self) -> int:
+        """Returns the current maximum number of columns to display for this Dataframe."""
+        return self._display_max_columns
+
+    @display_max_columns.setter
+    def display_max_columns(self, max_columns: int):
+        """Sets a new maximum number of value columns to display for this Dataframe."""
+        self._display_max_columns = max_columns
+
+    @property
+    def display_max_rows(self) -> int:
+        """Returns the current maximum number of rows to display for this Dataframe."""
+        return self._display_max_rows
+
+    @display_max_rows.setter
+    def display_max_rows(self, max_rows: int):
+        """Sets a new maximum number of value rows to display for this Dataframe."""
+        self._display_max_rows = max_rows
+
+    @property
     def columns(self) -> MultiIndex:
         """Returns the MultiIndex for the columns of the DataFrame."""
         if self._columns is None:
             indexes = [ResultsIndex(values=[self._fc[0].name.split("_")])]
             indexes.extend(
                 [
                     LabelIndex(name=label, values=self._fc.get_label_scoping(label).ids)
@@ -266,34 +301,39 @@
                 node_ids = axis_kwargs[mesh_index_name]
                 if not isinstance(node_ids, (DPFArray, list)):
                     node_ids = [node_ids]
                 mesh_scoping = dpf.mesh_scoping_factory.nodal_scoping(
                     node_ids=node_ids,
                     server=server,
                 )
-            elif ref_labels.element_ids in mesh_index_name:
+            elif ref_labels.element_ids or ref_labels.cell_ids in mesh_index_name:
+                if ref_labels.cell_ids in mesh_index_name:
+                    location = "cells"
                 element_ids = axis_kwargs[mesh_index_name]
                 if not isinstance(element_ids, list):
                     element_ids = [element_ids]
                 mesh_scoping = dpf.mesh_scoping_factory.elemental_scoping(
                     element_ids=element_ids,
                     server=server,
                 )
             else:
                 raise NotImplementedError(
                     f"Selection on a DataFrame with index "
                     f"'{mesh_index_name}' is not yet supported"
                 )
-            rescope_fc = dpf.operators.scoping.rescope_fc(
-                fields_container=input_fc,
-                mesh_scoping=mesh_scoping,
-                server=server,
-            )
-            out = rescope_fc.outputs.fields_container
-            mesh_index = MeshIndex(location=location, values=mesh_scoping.ids)
+            if isinstance(input_fc, PropertyFieldsContainer):
+                fc = input_fc.rescope(mesh_scoping)
+            else:
+                rescope_fc = dpf.operators.scoping.rescope_fc(
+                    fields_container=input_fc,
+                    mesh_scoping=mesh_scoping,
+                    server=server,
+                )
+                out = rescope_fc.outputs.fields_container
+                mesh_index = MeshIndex(location=location, values=mesh_scoping.ids)
         elif (
             mesh_index_name in axis_kwargs.keys()
             and mesh_index.location == locations.elemental_nodal
         ):
             raise NotImplementedError(
                 "Element selection on a DataFrame with elemental nodal results "
                 "is not yet supported"
@@ -315,20 +355,33 @@
         else:
             set_index = SetIndex(values=[])
 
         column_indexes = [
             results_index,
             set_index,
         ]
+        if isinstance(fc, PropertyFieldsContainer):
+            column_indexes = [results_index]
+
         label_indexes = []
         for label in fc.labels:
             if label not in ["time"]:
-                column_indexes.append(
-                    LabelIndex(name=label, values=fc.get_available_ids_for_label(label))
-                )
+                fc_values = fc.get_available_ids_for_label(label)
+                old_values = self.columns[self.columns.names.index(label)].values
+                if old_values is None:
+                    values = fc_values
+                else:
+                    fc_to_old_map = {}
+                    for v in old_values:
+                        if isinstance(v, str) and ("(" and ")" in v):
+                            fc_to_old_map[v.split("(")[1].split(")")[0]] = v
+                        else:
+                            fc_to_old_map[str(v)] = v
+                    values = [fc_to_old_map[str(f)] for f in fc_values]
+                column_indexes.append(LabelIndex(name=label, values=values))
         column_indexes.extend(label_indexes)
         column_index = MultiIndex(indexes=column_indexes)
 
         return DataFrame(
             data=fc,
             columns=column_index,
             index=row_index,
@@ -373,280 +426,284 @@
         """Return the length of the DataFrame."""
         return len(self.index)
 
     def __str__(self) -> str:
         """String representation of the DataFrame."""
         if (
             (self._str is None)
-            or (self._last_display_width != display_width)
-            or (self._last_display_max_colwidth != display_max_colwidth)
+            or (self._last_display_max_columns != self.display_max_columns)
+            or (self._last_display_max_rows != self.display_max_rows)
         ):
-            self._update_str(width=display_width, max_colwidth=display_max_colwidth)
-            self._last_display_width = display_width
-            self._last_display_max_colwidth = display_max_colwidth
+            self._update_str(
+                max_columns=self.display_max_columns, max_rows=self.display_max_rows
+            )
+            self._last_display_max_columns = self.display_max_columns
+            self._last_display_max_rows = self.display_max_rows
         return self._str
 
-    def _update_str(self, width: int, max_colwidth: int):
+    def _update_str(self, max_columns: int, max_rows: int):
         """Updates the DataFrame string representation using given display options.
 
         The string representation is limited to five lines, meaning any DataFrame with more than
         five rows will be truncated and only the five first rows are displayed.
 
         Parameters
         ----------
-        width:
-            Number of characters to use for the total width.
-        max_colwidth:
-            Maximum number of characters to use for each column.
+        max_columns:
+            Maximum number of value columns to show.
+        max_rows:
+            Maximum number of value rows to show.
         """
+        cells = []
         lines = []
-        empty = " " * max_colwidth
-        truncated_str = "...".rjust(max_colwidth)
-        max_n_col = width // max_colwidth
-        max_n_rows = display_max_lines
-        # Create lines with row labels and values
+        # Static
+        empty = ""
+        element_node_offset = 0
+
+        # Create cells with row labels and values
         num_column_indexes = len(self.columns)
         num_rows_indexes = len(self.index)
-        n_max_value_col = max_n_col - num_rows_indexes
-        column_headers = []
-        for column_index in self.columns:
-            column_headers.append(
-                empty * (num_rows_indexes - 1) + column_index.name.rjust(max_colwidth)
-            )
-        lines.extend(column_headers)
 
-        row_headers = "".join(
-            [row_index.name.rjust(max_colwidth) for row_index in self.index]
-        )
-        lines.append(row_headers)
-        entity_ids = []
-        truncated = False
+        # Add top-left empty space above row headers
+        cells.extend([[empty] * num_column_indexes] * (num_rows_indexes - 1))
+        # Add column headers cells
+        cells.append([c.name for c in self.columns])
+        # Add row headers
+        _ = [cells[i].append(row.name) for i, row in enumerate(self._index)]
+
+        # Find out whether rows will be truncated
+        truncate_row = 0
         if len(self._fc) > 0:
             num_mesh_entities_to_ask = self._fc[0].size
         else:
             num_mesh_entities_to_ask = 0
-        if num_mesh_entities_to_ask > max_n_rows:
-            num_mesh_entities_to_ask = max_n_rows
-            truncated = True
+        if num_mesh_entities_to_ask > max_rows:
+            num_mesh_entities_to_ask = max_rows
+            truncate_row = max_rows + num_column_indexes
+
+        comp_values = [1]
+        entity_ids = [1]
+
+        # Create row label values combinations
         lists = []
-        # Create combinations for rows
-        entity_ids = None
         for index in self.index:
             if isinstance(index, MeshIndex):
                 if index._values is not None:
                     values = index.values
                 else:
                     values = self._first_n_ids_first_field(num_mesh_entities_to_ask)
                 entity_ids = values
             elif isinstance(index, CompIndex):
                 values = index.values
+                comp_values = values
             else:
                 values = index.values
             lists.append(values)
-        row_combinations = [p for p in itertools.product(*lists)][:max_n_rows]
+        row_combinations = [p for p in itertools.product(*lists)][:max_rows]
 
-        # Add row headers for the first combinations (max_n_rows)
+        # Add row labels for the first max_rows combinations
         previous_combination = [None] * len(lists)
         for combination in row_combinations:
-            line = "".join(
-                [
-                    str(combination[i]).rjust(max_colwidth)
+            [
+                cells[i + element_node_offset].append(
+                    str(combination[i])
                     if combination[i] != previous_combination[i]
                     else empty
-                    for i in range(len(combination))
-                ]
-            )
+                )
+                for i in range(len(combination))
+            ]
             previous_combination = combination
-            lines.append(line)
 
-        # Create combinations for columns
-        entity_ids = None
+        # Create column label values combinations
         lists = []
         label_positions_in_combinations = {}
-        comp_values = [1]
         for position, index in enumerate(self.columns):
             if isinstance(index, MeshIndex):
                 if index._values is not None:
                     values = index.values
                     entity_ids = values
                 else:
                     values = self._first_n_ids_first_field(num_mesh_entities_to_ask)
                     entity_ids = values
             elif isinstance(index, CompIndex):
                 values = index.values
                 comp_values = values
             else:
                 values = index.values
+            if values is None:
+                values = [1]
             label_positions_in_combinations[index.name] = position
             lists.append(values)
-        combinations = [p for p in itertools.product(*lists)]
-        truncated_columns = False
-        if len(combinations) > n_max_value_col:
-            truncated_columns = True
-            combinations = combinations[:n_max_value_col]
-
-        def flatten(arr):
-            new_arr = []
-            for item in arr:
-                if isinstance(item, list):
-                    new_arr.extend(flatten(item))
-                else:
-                    new_arr.append(item)
-            return new_arr
+        column_combinations = [p for p in itertools.product(*lists)]
 
-        def treat_elemental_nodal(treat_lines, pos, n_comp, n_ent, n_lines):
-            # Update row headers
-            elem_headers = treat_lines[pos : pos + n_comp]
-            new_elem_headers = []
-            for i_ent in range(1, n_ent + 1):
-                for header in elem_headers:
-                    new_elem_header = [
-                        header[:max_colwidth]
-                        + header[max_colwidth + 4 :]
-                        + f" ({i_ent})"
-                    ]
-                    # elem_header_i.extend(elem_headers[1:])
-                    new_elem_headers.extend(new_elem_header)
-                treat_lines = treat_lines[:pos] + new_elem_headers + treat_lines[pos:]
-            return treat_lines[:n_lines]
+        # Find out whether columns will be truncated
+        truncate_col = 0
+        if len(column_combinations) > max_columns:
+            truncate_col = max_columns + num_rows_indexes
+            column_combinations = column_combinations[:max_columns]
 
-        # Add text for the first n_max_value_col columns
+        combination_index = num_rows_indexes
+        # For each column combination
         previous_combination = [None] * len(lists)
-        for i_c, combination in enumerate(combinations[:n_max_value_col]):
-            to_append = [
-                str(combination[i]).rjust(max_colwidth)
+        for combination in column_combinations[:max_columns]:
+            if combination_index > max_columns + num_rows_indexes:
+                truncate_col = max_columns + num_rows_indexes
+                break
+            max_n_col_per_entity = 1
+            # ## Fill the label values
+            labels = [
+                str(combination[i])
                 if combination[i] != previous_combination[i]
                 else empty
                 for i in range(len(combination))
             ]
-            to_append.append(empty)  # row where row index headers are
-            if len(self._fc) == 0:
-                for i, _ in enumerate(to_append):
-                    lines[i] = lines[i] + to_append[i]
-                break
-            # Get data in the FieldsContainer for those positions
+            previous_combination = combination
+            labels.append(empty)  # add empty cell on the row header line
+            cells.append(labels)
+
+            # ## Fill the data
             # Create label_space from combination
             label_space = {}
             for label_name in self.labels:
                 value = combination[label_positions_in_combinations[label_name]]
+                if value is None or value == "":
+                    raise ValueError(
+                        f"Could not find label value for label {label_name}"
+                    )
+                elif isinstance(value, str):
+                    if "(" in value:
+                        value = value.split("(")[1].split(")")[0]
                 if label_name == ref_labels.set_ids:
                     label_name = ref_labels.time
-                label_space[label_name] = value
+                label_space[label_name] = int(value)
             fields = self._fc.get_fields(label_space=label_space)
-            values = []
-            if entity_ids is None:
+
+            # Start counting values found
+            n_values = 0
+            # Loop over asked entities
+            for e, entity_id in enumerate(entity_ids):
+                values = []
+                # Look for data for this entity in each field
                 for field in fields:
-                    array_values = []
-                    position = len(column_headers) + 1
-                    for k in list(range(num_mesh_entities_to_ask)):
-                        try:
-                            values_list = field.get_entity_data(k).tolist()
-                        except Exception:
-                            values_list = [[None] * len(comp_values)]
-                        num_entities = len(values_list)
-                        if isinstance(values_list[0], list):
-                            num_components = len(values_list[0])
+                    try:
+                        # Try getting data for this entity ID in the current field
+                        data = field.get_entity_data_by_id(entity_id).tolist()
+                    except ansys.dpf.gate.errors.DPFServerException as e:
+                        # If entity data not found in this field, try next field
+                        if "Field_GetEntityDataById" in str(e):
+                            continue
                         else:
-                            num_components = 1
-                        current_number_lines = len(lines)
-                        # Detect number of nodes when elemental nodal and update headers to
-                        # repeat for each node (do not print their ID for now)
-                        if (
-                            i_c == 0
-                            and field.location == locations.elemental_nodal
-                            and len(values_list) != 0
-                        ):
-                            lines = treat_elemental_nodal(
-                                lines,
-                                position,
-                                num_components,
-                                num_entities,
-                                current_number_lines,
-                            )
-                        array_values.append(values_list)
-                        if (
-                            position + num_entities * num_components
-                            >= current_number_lines + len(column_headers) + 1
-                        ):
-                            if k < num_mesh_entities_to_ask:
-                                truncated = True
-                        if position >= current_number_lines:
-                            break
-                        position += num_entities * num_components
-                    if array_values:
-                        array_values = flatten(array_values)
-                        values.extend(array_values)
-            else:
-                array_values = []
-                position = len(column_headers) + 1
-                for entity_id in entity_ids:
-                    for field in fields:
-                        try:
-                            values_list = field.get_entity_data_by_id(
-                                entity_id
-                            ).tolist()
-                        except Exception:
-                            values_list = [[None] * len(comp_values)]
-                        num_entities = len(values_list)
-                        num_components = len(values_list[0])
-                        current_number_lines = len(lines)
-                        # Detect number of nodes when elemental nodal and update headers to
-                        # repeat for each node (do not print their ID for now)
-                        if (
-                            i_c == 0
-                            and field.location == locations.elemental_nodal
-                            and len(values_list) != 0
-                        ):
-                            lines = treat_elemental_nodal(
-                                lines,
-                                position,
-                                num_components,
-                                num_entities,
-                                current_number_lines,
-                            )
-                        array_values.append(values_list)
-                        if (
-                            position + num_entities * num_components
-                            >= current_number_lines + len(column_headers) + 1
-                        ):
-                            if k < num_mesh_entities_to_ask:
-                                truncated = True
-                        if position >= current_number_lines:
-                            break
-                        position += num_entities * num_components
-                        if array_values:
-                            array_values = flatten(array_values)
-                            values.extend(array_values)
-
-            # take_comp_map = [True] * len(values)
-            # if comp_values is not None:
-
-            value_strings = []
-            for value in values[: len(lines) - (num_column_indexes + 1)]:
-                if value is not None:
-                    value_string = f"{value:.{max_colwidth - 8}e}".rjust(max_colwidth)
-                else:
-                    value_string = empty
-                value_strings.append(value_string)
-            to_append.extend(value_strings)
-            previous_combination = combination
-            # print(to_append)
-            # print(len(to_append))
-            # print(len(lines))
-            for i, _ in enumerate(lines):
-                lines[i] = lines[i] + to_append[i]
-
-        if truncated_columns:
-            for i, _ in enumerate(lines):
-                lines[i] = lines[i] + truncated_str
-
-        if truncated:
-            lines.append(truncated_str)
-        txt = "\n" + "".join([line + "\n" for line in lines])
-        self._str = txt
+                            raise e
+                    except ValueError:
+                        continue
+                    n_col_per_entity = len(data)
+                    # Update max number of node per element in case of elemental nodal
+                    if field.location == locations.elemental_nodal:
+                        # Update the cells table if more nodes per element than previously
+                        if n_col_per_entity > max_n_col_per_entity:
+                            for i_n in range(max_n_col_per_entity, n_col_per_entity):
+                                to_append = [empty] * (num_column_indexes - 1)
+                                to_append.append(str(i_n))
+                                to_append.append(empty)
+                                to_append.extend(
+                                    [empty] * e
+                                )  # Pad previous entity lines
+                                cells.append(to_append)
+                        max_n_col_per_entity = max(
+                            max_n_col_per_entity, n_col_per_entity
+                        )
+                    if n_col_per_entity > max_columns:
+                        truncate_col = max_columns + num_rows_indexes
+                    # Update number of values found to add per column
+                    if isinstance(data[0], list):
+                        n_values += len(data[0])
+                    else:
+                        n_values += 1
+                    # # Flatten obtained data and format to string
+                    # values_list = [f"{x:.4e}" for y in data for x in y]
+                    break_loop = False
+                    # Loop over the number of node columns to fill
+                    for i_n in range(n_col_per_entity):
+                        # Build list of str values to append to current column
+                        if i_n < n_col_per_entity:
+                            values = data[i_n]
+                            if isinstance(values, list):
+                                values = [
+                                    f"{x}"
+                                    if np.issubdtype(type(x), np.integer)
+                                    else f"{x:.4e}"
+                                    for x in values
+                                ]
+                            else:
+                                values = [
+                                    f"{values}"
+                                    if np.issubdtype(type(values), np.integer)
+                                    else f"{values:.4e}"
+                                ]
+                        else:
+                            values = [empty] * max_rows
+                        cells[combination_index + i_n].extend(values)
+                        # If already found enough values to print
+                        if n_values >= max_rows:
+                            # Exit the loop on fields
+                            break_loop = True
+                    if break_loop:
+                        break
+                # If already found enough values to print
+                if n_values >= max_rows:
+                    # Exit the loop on entity IDs
+                    break
+                if not values:
+                    # If no data found for this entity ID, add empty cells
+                    values = [[empty] * len(comp_values)]
+                    n_values += len(values)
+                    cells[combination_index].extend(*values)
+
+            combination_index += max_n_col_per_entity
+
+        self._str = self._format_cells(
+            cells=cells, truncate_col=truncate_col, truncate_row=truncate_row
+        )
+
+    @staticmethod
+    def _format_cells(
+        cells: List[List[str]],
+        truncate_col: int = 0,
+        truncate_row: int = 0,
+    ) -> str:
+        """Format the data cells into one string.
+
+        Argument cells is a list of column data, each one itself a list of row data.
+        """
+        truncated_str = "..."
+
+        # Truncate columns
+        if truncate_col:
+            cells = cells[:truncate_col]
+            cells.append([truncated_str] * len(cells[0]))
+
+        # Truncate rows
+        if truncate_row:
+            for i, _ in enumerate(cells):
+                cells[i] = cells[i][: truncate_row + 1]
+                cells[i].append(truncated_str)
+        n_lines = len(cells[0])
+
+        lines = [""] * n_lines
+        for c, column in enumerate(cells):
+            if len(column) != n_lines:
+                print(cells)
+                raise ValueError(
+                    f"Column {c} has {len(column)} lines instead of {n_lines}!"
+                )
+            max_length = max(map(len, column))
+            for i in range(n_lines):
+                lines[i] += column[i].rjust(max_length + 1)
+        lines = [line + "\n" for line in lines]
+        return "\n" + "".join(lines)
 
     def _first_n_ids_first_field(self, n: int) -> List[int]:
         """Return the n first entity IDs of the first field in the underlying FieldsContainer."""
         if len(self._fc) > 0:
             return self._fc[0].scoping.ids[:n]
         else:
             return []
@@ -675,14 +732,16 @@
             arguments, see ``help(pyvista.plot)``.
 
         Returns
         -------
             The interactive plotter object used for plotting.
 
         """
+        if len(self.index.mesh_index) == 0:
+            raise ValueError("Cannot plot a Dataframe with an empty mesh index.")
         label_space = {}
         if kwargs != {}:
             axis_kwargs, kwargs = self._filter_arguments(arguments=kwargs)
             # Construct the associated label_space
             df_temp = self.select(**axis_kwargs)
             fc = df_temp._fc
             if len(fc) == 0:
@@ -711,14 +770,16 @@
                 label_space[label] = value
         else:
             axis_kwargs = {}
             # If no kwarg was given, construct a default label_space
             fc = self._fc
             label_space = fc.get_label_space(0)
 
+        if len(fc) == 0:
+            raise ValueError("No data to plot.")
         for field in fc:
             # Treat multi-layer field
             shell_layer_check = field.shell_layers
             if shell_layer_check in [
                 shell_layers.topbottom,
                 shell_layers.topbottommid,
             ]:
@@ -745,16 +806,30 @@
             merge_stages_op = dpf.operators.utility.merge_fields_by_label(
                 fields_container=fc, label="stage"
             )
             fc = merge_stages_op.outputs.fields_container()
             label_space.pop("stage")
 
         fields = fc.get_fields(label_space=label_space)
-        plotter = DpfPlotter(**kwargs)
-        plotter.add_field(field=fields[0], **kwargs)
+        # for field in fields:
+        if len(fields) > 1:
+            # try:
+            #     for field in fields[1:]:
+            #         plotter.add_field(field=field, **kwargs)
+            # except Exception as e:
+            raise ValueError(
+                f"Plotting failed with filter {axis_kwargs} due to incompatible data."
+            )
+            # warnings.warn(
+            #     UserWarning(
+            #         "Plotting criteria resulted in incompatible data. "
+            #         "Try narrowing down to specific values for each column."
+            #     )
+            # )
+            # return None
         # for field in fields:
         if len(fields) > 1:
             # try:
             #     for field in fields[1:]:
             #         plotter.add_field(field=field, **kwargs)
             # except Exception as e:
             raise ValueError(
@@ -764,14 +839,23 @@
             #     UserWarning(
             #         "Plotting criteria resulted in incompatible data. "
             #         "Try narrowing down to specific values for each column."
             #     )
             # )
             # return None
         # field.plot(text="debug")
+        field_to_plot = fields[0]
+        # If multi-component, take the norm
+        if field_to_plot.component_count > 1:
+            field_to_plot = dpf.operators.math.norm(
+                field_to_plot, server=field_to_plot._server
+            ).eval()
+        plotter = DpfPlotter(**kwargs)
+        plotter.add_field(field=field_to_plot, **kwargs)
+
         return plotter.show_figure(
             title=kwargs.pop("title", str(label_space)), **kwargs
         )
 
     def animate(
         self,
         save_as: Union[PathLike, str, None] = None,
@@ -901,23 +985,23 @@
         components
                  X -7.4732e-04 -1.5081e-03 -2.2755e-03
                  Y -4.0138e-04 -8.0316e-04 -1.2014e-03
                  Z -2.1555e-04 -4.3299e-04 -6.5101e-04
         >>> # Compute the maximum displacement for each node and component across time
         >>> minimum_over_time = displacement.min(axis="set_ids")
         >>> print(minimum_over_time)  # doctest: +NORMALIZE_WHITESPACE
-                   results       U (m)
-        node_ids  components
-          4872           X -3.4137e-05
-                         Y  5.1667e-04
-                         Z -4.1346e-06
-          9005           X -5.5625e-05
-                         Y  4.8445e-04
-                         Z -4.9795e-07
-                       ...
+                    results       U (m)
+         node_ids components
+             4872          X -3.4137e-05
+                           Y  5.1667e-04
+                           Z -4.1346e-06
+             9005          X -5.5625e-05
+                           Y  4.8445e-04
+                           Z -4.9795e-07
+              ...        ...         ...
         >>> # Compute the maximum displacement overall
         >>> minimum_overall = minimum_over_time.min()
         >>> print(minimum_overall)  # doctest: +NORMALIZE_WHITESPACE
            results       U (m)
         components
                  X -2.2755e-03
                  Y -1.2014e-03
@@ -957,23 +1041,23 @@
         components
                  X  7.3303e-04  1.4495e-03  2.1441e-03
                  Y  1.3962e-03  2.7884e-03  4.1656e-03
                  Z  2.1567e-04  4.3321e-04  6.5135e-04
         >>> # Compute the maximum displacement for each node and component across time
         >>> maximum_over_time = displacement.max(axis="set_ids")
         >>> print(maximum_over_time)  # doctest: +NORMALIZE_WHITESPACE
-                   results       U (m)
-        node_ids  components
-          4872           X  5.6781e-06
-                         Y  1.5417e-03
-                         Z -2.6398e-06
-          9005           X -2.6323e-06
-                         Y  1.4448e-03
-                         Z  5.3134e-06
-           ...
+                     results       U (m)
+         node_ids components
+             4872          X  5.6781e-06
+                           Y  1.5417e-03
+                           Z -2.6398e-06
+             9005          X -2.6323e-06
+                           Y  1.4448e-03
+                           Z  5.3134e-06
+              ...        ...         ...
         >>> # Compute the maximum displacement overall
         >>> maximum_overall = maximum_over_time.max()
         >>> print(maximum_overall)  # doctest: +NORMALIZE_WHITESPACE
            results       U (m)
         components
                  X  2.1441e-03
                  Y  4.1656e-03
```

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/displacement.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/displacement.py`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/dpf_path.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/dpf_path.py`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/dpf_solution.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/dpf_solution.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
              -  stiffness_matrix_energy: Elemental Energy-stiffness matrix
              -  artificial_hourglass_energy: Elemental Hourglass Energy
              -  thermal_dissipation_energy: Elemental thermal dissipation energy
              -  kinetic_energy: Elemental Kinetic Energy
              -  co_energy: Elemental co-energy
              -  incremental_energy: Elemental incremental energy
              -  elastic_strain: ElementalNodal Strain
-             -  structural_temperature: ElementalNodal Temperature
+             -  structural_temperature: ElementalNodal Structural temperature
         """
         return self._model.metadata.result_info
 
     @staticmethod
     def _check_nodal_location(**kwargs):
         if _AvailableKeywords.location in kwargs:
             location = kwargs.pop(_AvailableKeywords.location)
```

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/electric_results.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/electric_results.py`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/errors.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/errors.py`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/index.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,43 @@
     components = "components"
     results = "results"
     time = "time"
     modes = "modes"
     frequencies = "frequencies"
     set_ids = "set_ids"
     node_ids = "node_ids"
+    face_ids = "face_ids"
     element_ids = "element_ids"
+    cell_ids = "cell_ids"
     elemental_nodal = "element_ids"
     step = "step_ids"
     overall = "overall"
+    element_node = "node"
 
 
 location_to_label = {
     dpf.locations.nodal: ref_labels.node_ids,
+    "cells": ref_labels.cell_ids,
     dpf.locations.elemental: ref_labels.element_ids,
     dpf.locations.elemental_nodal: ref_labels.elemental_nodal,
     dpf.locations.overall: ref_labels.overall,
     dpf.locations.time_freq_step: ref_labels.step,
     dpf.locations.time_freq: ref_labels.set_ids,
+    None: "unknown",
 }
 
+# dpf.locations.faces is available only starting with ansys-dpg-gate 0.4.0
+try:  # pragma: no cover
+    location_to_label[dpf.locations.faces] = ref_labels.face_ids
+except AttributeError as e:
+    if "type object 'locations' has no attribute 'faces'" in str(e):
+        pass
+    else:
+        raise e
+
 
 class Index(ABC):
     """A Pandas style API to manipulate indexes."""
 
     def __init__(
         self,
         name: str,
@@ -70,20 +84,20 @@
             self._scoping_ref = weakref.ref(scoping)
         if values is not None and len(values) > 0:
             self._dtype = type(values[0])
         self._str = None
 
     def __repr__(self):
         """Representation of the Index."""
-        return f'Index<name="{self._name}", dtype={self._dtype}>'
+        return f'{type(self).__name__}<name="{self._name}", dtype={self._dtype}>'
 
     def __str__(self):
         """String representation of the Index."""
         return (
-            f'Index "{self._name}" with '
+            f'{type(self).__name__} "{self._name}" with '
             f"{len(self._values) if self._values is not None else 'uncounted'} "
             f"values of {self._dtype if self._dtype is not None else 'undetermined'} type"
         )
 
     def __len__(self):
         """Returns the length of the index."""
         if self._len is not None:
@@ -130,18 +144,15 @@
         if fc is None and values is None and scoping is None:
             raise ValueError(
                 "Arguments 'values', 'scoping' and 'fc' cannot all be None."
             )
         if fc is not None:
             self._fc = weakref.ref(fc)
         super().__init__(name=name, values=values, scoping=scoping)
-
-    def __repr__(self):
-        """Representation of the MeshIndex."""
-        return f'MeshIndex<name="{self._name}", dtype={int}>'
+        self._dtype = int
 
     def _evaluate_values(self):
         """Evaluates the values of the MeshIndex."""
         if self._scoping_ref is not None:
             self._values = self._scoping_ref().ids
         else:
             # Merge the fields container scoping
@@ -290,14 +301,25 @@
         self,
         values: Union[List, None] = None,
     ):
         """Initiate this class."""
         super().__init__(name=ref_labels.components, values=values)
 
 
+class ElementNodeIndex(Index):
+    """Index class specific to elemental nodal results."""
+
+    def __init__(
+        self,
+    ):
+        """Initiate this class."""
+        # We know there will be at least one node value per element.
+        super().__init__(name=ref_labels.element_node, values=[0])
+
+
 class MultiIndex:
     """A Pandas style API to manipulate multi-indexes."""
 
     def __init__(
         self,
         indexes: List[Index],
     ):
@@ -311,14 +333,19 @@
         self._indexes = indexes
         # self._labels = []
         # self._label_names = None
         # self._result_names = None
         for _, index in enumerate(self._indexes):
             setattr(self, index.name, index)
 
+    @property
+    def indexes(self) -> List[Index]:
+        """Returns the list of Index in the MultiIndex."""
+        return self._indexes
+
     # @property
     # def labels(self):
     #     """Returns the list of label Index objects."""
     #     return self._labels
     #
     # @property
     # def results(self):
```

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/misc.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/misc.py`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/misc_results.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/misc_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         self._check_elemental_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "S",
             self,
             self._data_sources,
             location="Elemental",
             b_elem_average=True,
-            **kwargs
+            **kwargs,
         )
 
     def elemental_nodal_stress(self, **kwargs):
         """Get result data for the elemental nodal stress."""
         self._check_elemnodal_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "S", self, self._data_sources, location="ElementalNodal", **kwargs
@@ -214,15 +214,15 @@
         self._check_elemental_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "EPEL",
             self,
             self._data_sources,
             location="Elemental",
             b_elem_average=True,
-            **kwargs
+            **kwargs,
         )
 
     def elemental_nodal_elastic_strain(self, **kwargs):
         """Get result data for the elemental nodal elastic strain."""
         self._check_elemnodal_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "EPEL", self, self._data_sources, location="ElementalNodal", **kwargs
@@ -240,15 +240,15 @@
         self._check_elemental_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "EPPL",
             self,
             self._data_sources,
             location="Elemental",
             b_elem_average=True,
-            **kwargs
+            **kwargs,
         )
 
     def elemental_nodal_plastic_strain(self, **kwargs):
         """Get result data for the elemental nodal plastic strain."""
         self._check_elemnodal_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "EPPL", self, self._data_sources, location="ElementalNodal", **kwargs
@@ -266,15 +266,15 @@
         self._check_elemental_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "BFE",
             self,
             self._data_sources,
             location="Elemental",
             b_elem_average=True,
-            **kwargs
+            **kwargs,
         )
 
     def elemental_nodal_structural_temperature(self, **kwargs):
         """Get result data for the elemental nodal structural temperature."""
         self._check_elemnodal_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "BFE", self, self._data_sources, location="ElementalNodal", **kwargs
@@ -292,15 +292,15 @@
         self._check_elemental_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ETH",
             self,
             self._data_sources,
             location="Elemental",
             b_elem_average=True,
-            **kwargs
+            **kwargs,
         )
 
     def elemental_nodal_thermal_strains(self, **kwargs):
         """Get result data for the elemental nodal thermal strains."""
         self._check_elemnodal_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ETH", self, self._data_sources, location="ElementalNodal", **kwargs
@@ -318,15 +318,15 @@
         self._check_elemental_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_SEPL",
             self,
             self._data_sources,
             location="Elemental",
             b_elem_average=True,
-            **kwargs
+            **kwargs,
         )
 
     def elemental_nodal_eqv_stress_parameter(self, **kwargs):
         """Get result data for the elemental nodal equivalent stress parameter."""
         self._check_elemnodal_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_SEPL", self, self._data_sources, location="ElementalNodal", **kwargs
@@ -344,15 +344,15 @@
         self._check_elemental_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_SRAT",
             self,
             self._data_sources,
             location="Elemental",
             b_elem_average=True,
-            **kwargs
+            **kwargs,
         )
 
     def elemental_nodal_stress_ratio(self, **kwargs):
         """Get result data for the elemental nodal stress ratio."""
         self._check_elemnodal_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_SRAT", self, self._data_sources, location="ElementalNodal", **kwargs
@@ -370,15 +370,15 @@
         self._check_elemental_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_HPRES",
             self,
             self._data_sources,
             location="Elemental",
             b_elem_average=True,
-            **kwargs
+            **kwargs,
         )
 
     def elemental_nodal_hydrostatic_pressure(self, **kwargs):
         """Get result data for the elemental nodal hydrostatic pressure."""
         self._check_elemnodal_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_HPRES", self, self._data_sources, location="ElementalNodal", **kwargs
@@ -396,15 +396,15 @@
         self._check_elemental_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_EPEQ",
             self,
             self._data_sources,
             location="Elemental",
             b_elem_average=True,
-            **kwargs
+            **kwargs,
         )
 
     def elemental_nodal_accu_eqv_plastic_strain(self, **kwargs):
         """Get result data for the elemental nodal accurate eqvivalent plastic strain."""
         self._check_elemnodal_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_EPEQ", self, self._data_sources, location="ElementalNodal", **kwargs
@@ -422,15 +422,15 @@
         self._check_elemental_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_PSV",
             self,
             self._data_sources,
             location="Elemental",
             b_elem_average=True,
-            **kwargs
+            **kwargs,
         )
 
     def elemental_nodal_plastic_state_variable(self, **kwargs):
         """Get result data for the elemental nodal plastic state variable."""
         self._check_elemnodal_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_PSV", self, self._data_sources, location="ElementalNodal", **kwargs
@@ -448,15 +448,15 @@
         self._check_elemental_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_CREQ",
             self,
             self._data_sources,
             location="Elemental",
             b_elem_average=True,
-            **kwargs
+            **kwargs,
         )
 
     def elemental_nodal_accu_eqv_creep_strain(self, **kwargs):
         """Get result data for the elemental nodal accurate equivalent creep strain."""
         self._check_elemnodal_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_CREQ", self, self._data_sources, location="ElementalNodal", **kwargs
@@ -474,15 +474,15 @@
         self._check_elemental_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_PLWK",
             self,
             self._data_sources,
             location="Elemental",
             b_elem_average=True,
-            **kwargs
+            **kwargs,
         )
 
     def elemental_nodal_plastic_strain_energy_density(self, **kwargs):
         """Get result data for the elemental nodal plastic strain energy density."""
         self._check_elemnodal_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_PLWK", self, self._data_sources, location="ElementalNodal", **kwargs
@@ -500,15 +500,15 @@
         self._check_elemental_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_CRWK",
             self,
             self._data_sources,
             location="Elemental",
             b_elem_average=True,
-            **kwargs
+            **kwargs,
         )
 
     def elemental_nodal_creep_strain_energy_density(self, **kwargs):
         """Get result data for the elemental nodal creep strain energy density."""
         self._check_elemnodal_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_CRWK", self, self._data_sources, location="ElementalNodal", **kwargs
@@ -526,15 +526,15 @@
         self._check_elemental_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_ELENG",
             self,
             self._data_sources,
             location="Elemental",
             b_elem_average=True,
-            **kwargs
+            **kwargs,
         )
 
     def elemental_nodal_elastic_strain_energy_density(self, **kwargs):
         """Get result data for the elemental nodal elastic strain energy density."""
         self._check_elemnodal_location(**kwargs)
         return self._get_result_data_function_of_operator(
             "ENL_ELENG", self, self._data_sources, location="ElementalNodal", **kwargs
```

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/modal_mechanical_simulation.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/modal_mechanical_simulation.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 """
 from typing import List, Union
 
 from ansys.dpf import core as dpf
 from ansys.dpf.post import locations
 from ansys.dpf.post.dataframe import DataFrame
-from ansys.dpf.post.selection import Selection
+from ansys.dpf.post.selection import Selection, _WfNames
 from ansys.dpf.post.simulation import MechanicalSimulation, ResultCategory
 
 
 class ModalMechanicalSimulation(MechanicalSimulation):
     """Provides methods for mechanical modal simulations."""
 
     def _get_result(
@@ -29,72 +29,85 @@
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            base_name:
-                Base name for the requested result.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            category:
-                Type of result requested. See the :class:`ResultCategory` class.
-            components:
-                Components to get results for.
-            norm:
-                Whether to return the norm of the results.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            set_ids:
-                List of sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets/modes.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        base_name:
+            Base name for the requested result.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        category:
+            Type of result requested. See the :class:`ResultCategory` class.
+        components:
+            Components to get results for.
+        norm:
+            Whether to return the norm of the results.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        set_ids:
+            List of sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets/modes.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         # Build the targeted spatial and time scoping
         tot = (
             (set_ids is not None)
             + (all_sets is True)
             + (frequencies is not None)
@@ -106,104 +119,142 @@
                 "Arguments all_sets, selection, set_ids, frequencies, "
                 "and modes are mutually exclusive."
             )
         elif tot == 0:
             set_ids = 1
 
         selection = self._build_selection(
+            base_name=base_name,
+            category=category,
             selection=selection,
             set_ids=set_ids if set_ids else modes,
             times=frequencies,
             load_steps=None,
             all_sets=all_sets,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             location=location,
+            external_layer=external_layer,
+            skin=skin,
         )
 
         comp, to_extract, columns = self._create_components(
             base_name, category, components
         )
 
         # Initialize a workflow
         wf = dpf.Workflow(server=self._model._server)
-        wf.progress_bar = False
 
-        if category == ResultCategory.equivalent and base_name[0] == "E":
-            force_elemental_nodal = True
-        else:
-            force_elemental_nodal = False
+        force_elemental_nodal = self._requires_manual_averaging(
+            base_name=base_name,
+            location=location,
+            category=category,
+            selection=selection,
+        )
 
         # Instantiate the main result operator
-        result_op = self._build_result_operator(
+        wf, result_op = self._build_result_workflow(
             name=base_name,
             location=location,
             force_elemental_nodal=force_elemental_nodal,
         )
 
-        # Treat cyclic cases
-        result_op = self._treat_cyclic(expand_cyclic, phase_angle_cyclic, result_op)
-
         # Its output is selected as future workflow output for now
         out = result_op.outputs.fields_container
         # Its inputs are selected as workflow inputs for merging with selection workflows
         wf.set_input_name("time_scoping", result_op.inputs.time_scoping)
         wf.set_input_name("mesh_scoping", result_op.inputs.mesh_scoping)
 
         wf.connect_with(
             selection.time_freq_selection._selection,
             output_input_names=("scoping", "time_scoping"),
         )
+        if selection.requires_mesh:
+            mesh_wf = dpf.Workflow(server=self._model._server)
+            mesh_wf.set_output_name(
+                _WfNames.initial_mesh, self._model.metadata.mesh_provider
+            )
+            selection.spatial_selection._selection.connect_with(
+                mesh_wf,
+                output_input_names={_WfNames.initial_mesh: _WfNames.initial_mesh},
+            )
+
         wf.connect_with(
             selection.spatial_selection._selection,
-            output_input_names=("scoping", "mesh_scoping"),
+            output_input_names={
+                "scoping": "mesh_scoping",
+            },
         )
 
+        # Treat cyclic cases
+        wf = self._treat_cyclic(expand_cyclic, phase_angle_cyclic, wf)
+
         # Connect data_sources and streams_container inputs of selection if necessary
         if "streams" in wf.input_names:
             wf.connect("streams", self._model.metadata.streams_provider)
         if "data_sources" in wf.input_names:
             wf.connect("data_sources", self._model.metadata.data_sources)
 
+        average_op = None
+        if force_elemental_nodal:
+            average_op = self._create_averaging_operator(
+                location=location, selection=selection
+            )
+
         # Add a step to compute principal invariants if result is principal
         if category == ResultCategory.principal:
             # Instantiate the required operator
             principal_op = self._model.operator(name="invariants_fc")
             # Corresponds to scripting name principal_invariants
-            principal_op.connect(0, out)
+            if average_op is not None:
+                average_op[0].connect(0, out)
+                principal_op.connect(0, average_op[1])
+                # Set as future output of the workflow
+                average_op = None
+            else:
+                principal_op.connect(0, out)
             wf.add_operator(operator=principal_op)
             # Set as future output of the workflow
             if len(to_extract) == 1:
                 out = getattr(principal_op.outputs, f"fields_eig_{to_extract[0]+1}")
             else:
                 raise NotImplementedError("Cannot combine principal results yet.")
                 # We need to define the behavior for storing different results in a DataFrame
 
         # Add a step to compute equivalent if result is equivalent
         elif category == ResultCategory.equivalent:
             equivalent_op = self._model.operator(name="eqv_fc")
-            equivalent_op.connect(0, out)
             wf.add_operator(operator=equivalent_op)
-            # Set as future output of the workflow
-            out = equivalent_op.outputs.fields_container
             # If a strain result, change the location now
-            if force_elemental_nodal:
-                average_op = None
-                if location == locations.nodal:
-                    average_op = self._model.operator(name="to_nodal_fc")
-                elif location == locations.elemental:
-                    average_op = self._model.operator(name="to_elemental_fc")
-                if average_op is not None:
-                    average_op.connect(0, out)
-                    wf.add_operator(operator=average_op)
-                    # Set as future output of the workflow
-                    out = average_op.outputs.fields_container
+            if (
+                average_op is not None
+                and category == ResultCategory.equivalent
+                and base_name[0] == "E"
+            ):
+                equivalent_op.connect(0, out)
+                average_op[0].connect(0, equivalent_op)
+                wf.add_operator(operator=average_op[1])
+                # Set as future output of the workflow
+                out = average_op[1].outputs.fields_container
+            elif average_op is not None:
+                average_op[0].connect(0, out)
+                equivalent_op.connect(0, average_op[1])
+                # Set as future output of the workflow
+                out = equivalent_op.outputs.fields_container
+            else:
+                equivalent_op.connect(0, out)
+                out = equivalent_op.outputs.fields_container
+            average_op = None
             base_name += "_VM"
 
+        if average_op is not None:
+            average_op[0].connect(0, out)
+            out = average_op[1].outputs.fields_container
+
         # Add an optional component selection step if result is vector, matrix, or principal
         if (category in [ResultCategory.vector, ResultCategory.matrix]) and (
             to_extract is not None
         ):
             # Instantiate a component selector operator
             extract_op = self._model.operator(name="component_selector_fc")
             # Feed it the current workflow output
@@ -224,20 +275,30 @@
             wf.add_operator(operator=norm_op)
             out = norm_op.outputs.fields_container
             comp = None
             base_name += "_N"
 
         # Set the workflow output
         wf.set_output_name("out", out)
+        wf.progress_bar = False
         # Evaluate  the workflow
         fc = wf.get_output("out", dpf.types.fields_container)
 
         disp_wf = self._generate_disp_workflow(fc, selection)
 
-        return self._create_dataframe(fc, location, columns, comp, base_name, disp_wf)
+        submesh = None
+        if selection.outputs_mesh:
+            selection.spatial_selection._selection.progress_bar = False
+            submesh = selection.spatial_selection._selection.get_output(
+                _WfNames.mesh, dpf.types.meshed_region
+            )
+
+        return self._create_dataframe(
+            fc, location, columns, comp, base_name, disp_wf, submesh
+        )
 
     def displacement(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
@@ -245,132 +306,145 @@
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract displacement results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements whose nodes to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z",
-                and their respective equivalents 1, 2, 3.
-            norm:
-                Whether to return the norm of the results.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements whose nodes to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         Examples
         --------
         >>> from ansys.dpf import post
         >>> from ansys.dpf.post import examples
         >>> simulation = post.ModalMechanicalSimulation(examples.download_modal_frame())
         >>> # Extract the displacement field for the first mode
         >>> displacement = simulation.displacement()
         >>> print(displacement)  # doctest: +NORMALIZE_WHITESPACE
                      results      U (mm)
                      set_ids           1
-        node_ids  components
-             367           X -2.9441e-01
+         node_ids components
+              367          X -2.9441e-01
                            Y  1.2397e+00
                            Z  5.1160e-01
-             509           X -3.4043e-01
+              509          X -3.4043e-01
                            Y  1.8414e+00
                            Z  3.4187e-01
-             ...
+              ...        ...         ...
         >>> # Extract the displacement field for the first two modes
         >>> displacement = simulation.displacement(modes=[1, 2])
         >>> print(displacement)  # doctest: +NORMALIZE_WHITESPACE
                      results      U (mm)
                      set_ids           1           2
-        node_ids  components
-             367           X -2.9441e-01  1.7382e+00
+         node_ids components
+              367          X -2.9441e-01  1.7382e+00
                            Y  1.2397e+00  5.4243e-01
                            Z  5.1160e-01 -4.2969e-01
-             509           X -3.4043e-01  2.4632e+00
+              509          X -3.4043e-01  2.4632e+00
                            Y  1.8414e+00  7.5043e-01
                            Z  3.4187e-01 -2.7130e-01
-             ...
+              ...        ...         ...         ...
         >>> # Extract the displacement field for all modes
         >>> displacement = simulation.displacement(all_sets=True)
         >>> print(displacement)  # doctest: +NORMALIZE_WHITESPACE
                      results      U (mm)
                      set_ids           1           2           3           4           5           6
-        node_ids  components
-             367           X -2.9441e-01  1.7382e+00 -1.0401e-01 -3.6455e-01  2.8577e+00 -6.7501e-01
+         node_ids components
+              367          X -2.9441e-01  1.7382e+00 -1.0401e-01 -3.6455e-01  2.8577e+00 -6.7501e-01
                            Y  1.2397e+00  5.4243e-01  1.9069e+00  2.1373e+00 -5.0887e-02 -1.0978e+00
                            Z  5.1160e-01 -4.2969e-01  6.5813e-01  6.7056e-01 -8.8191e-01 -1.4610e-01
-             509           X -3.4043e-01  2.4632e+00 -3.1666e-01 -3.1348e-01  3.9674e+00 -5.1783e-01
+              509          X -3.4043e-01  2.4632e+00 -3.1666e-01 -3.1348e-01  3.9674e+00 -5.1783e-01
                            Y  1.8414e+00  7.5043e-01  2.5367e+00  3.0538e+00 -6.2025e-02 -1.1483e+00
                            Z  3.4187e-01 -2.7130e-01  4.4146e-01  3.9606e-01 -5.0972e-01 -1.1397e-01
-             ...
+              ...        ...         ...         ...         ...         ...         ...         ...
         >>> # Extract the norm of the displacement field for the first mode
         >>> displacement = simulation.displacement(norm=True)
         >>> print(displacement)  # doctest: +NORMALIZE_WHITESPACE
-         results    U_N (mm)
-         set_ids           1
-        node_ids
-             367  1.3730e+00
-             509  1.9036e+00
-             428  1.0166e+00
-             510  1.0461e+00
-            3442  1.6226e+00
-            3755  1.4089e+00
-             ...
+          results   U_N (mm)
+          set_ids          1
+         node_ids
+              367 1.3730e+00
+              509 1.9036e+00
+              428 1.0166e+00
+              510 1.0461e+00
+             3442 1.6226e+00
+             3755 1.4089e+00
+              ...        ...
         >>> # Extract the displacement field along X for the first mode
         >>> displacement = simulation.displacement(components=["X"])
         >>> print(displacement)  # doctest: +NORMALIZE_WHITESPACE
-         results    U_X (mm)
-         set_ids           1
-        node_ids
-             367 -2.9441e-01
-             509 -3.4043e-01
-             428 -1.1434e-01
-             510 -2.0561e-01
-            3442 -3.1765e-01
-            3755 -2.2155e-01
-             ...
+          results    U_X (mm)
+          set_ids           1
+         node_ids
+              367 -2.9441e-01
+              509 -3.4043e-01
+              428 -1.1434e-01
+              510 -2.0561e-01
+             3442 -3.1765e-01
+             3755 -2.2155e-01
+              ...         ...
         >>> # Extract the displacement field at nodes 23 and 24 for the first mode
         >>> displacement = simulation.displacement(node_ids=[23, 24])
         >>> print(displacement)  # doctest: +NORMALIZE_WHITESPACE
                      results      U (mm)
                      set_ids           1
         node_ids  components
               23           X -0.0000e+00
@@ -380,96 +454,96 @@
                            Y  1.3243e-01
                            Z  1.4795e-01
         >>> # Extract the displacement field at nodes of element 40 for the first mode
         >>> displacement = simulation.displacement(element_ids=[40])
         >>> print(displacement)  # doctest: +NORMALIZE_WHITESPACE
                      results      U (mm)
                      set_ids           1
-        node_ids  components
-             344           X -2.0812e-01
+         node_ids components
+              344          X -2.0812e-01
                            Y  1.1289e+00
                            Z  3.5111e-01
-             510           X -2.0561e-01
+              510          X -2.0561e-01
                            Y  9.8847e-01
                            Z  2.7365e-01
-             ...
+              ...        ...         ...
         >>> # For cyclic results
         >>> simulation = post.ModalMechanicalSimulation(examples.find_simple_cyclic())
         >>> # Extract the displacement field with cyclic expansion on all sectors at first mode
         >>> displacement = simulation.displacement(expand_cyclic=True)
         >>> print(displacement)  # doctest: +NORMALIZE_WHITESPACE
-                     results       U (m)
-                     set_ids           1
-        node_ids  components
-               1           X  1.7611e-13
-                           Y  8.5207e+01
-                           Z  3.1717e-12
-              52           X  2.3620e-12
-                           Y  8.5207e+01
-                           Z  2.1160e-12
-             ...
+                     results      U (m)
+                     set_ids          1
+         node_ids components
+                1          X 1.7611e-13
+                           Y 8.5207e+01
+                           Z 3.1717e-12
+               52          X 2.3620e-12
+                           Y 8.5207e+01
+                           Z 2.1160e-12
+              ...        ...        ...
         >>> # Extract the displacement field without cyclic expansion at first mode
         >>> displacement = simulation.displacement(expand_cyclic=False)
         >>> print(displacement)  # doctest: +NORMALIZE_WHITESPACE
-                     results       U (m)
-                     set_ids           1
-                 base_sector           1
-        node_ids  components
-               1           X  4.9812e-13
-                           Y  2.4100e+02
-                           Z  8.9709e-12
-              14           X -1.9511e-12
-                           Y  1.9261e+02
-                           Z  5.0359e-12
-             ...
+                      results       U (m)
+                      set_ids           1
+                  base_sector           1
+         node_ids  components
+                1           X  4.9812e-13
+                            Y  2.4100e+02
+                            Z  8.9709e-12
+               14           X -1.9511e-12
+                            Y  1.9261e+02
+                            Z  5.0359e-12
+              ...         ...         ...
         >>> # Extract the displacement field with cyclic expansion on selected sectors at first mode
         >>> displacement = simulation.displacement(expand_cyclic=[1, 2, 3])
         >>> print(displacement)  # doctest: +NORMALIZE_WHITESPACE
-                     results       U (m)
-                     set_ids           1
-        node_ids  components
-               1           X  1.7611e-13
-                           Y  8.5207e+01
-                           Z  3.1717e-12
-              52           X  2.3620e-12
-                           Y  8.5207e+01
-                           Z  2.1160e-12
-             ...
+                     results      U (m)
+                     set_ids          1
+         node_ids components
+                1          X 1.7611e-13
+                           Y 8.5207e+01
+                           Z 3.1717e-12
+               52          X 2.3620e-12
+                           Y 8.5207e+01
+                           Z 2.1160e-12
+              ...        ...        ...
         >>> # For multi-stage cyclic results
         >>> simulation = post.ModalMechanicalSimulation(
         ...     examples.download_multi_stage_cyclic_result()
         ... )
         >>> # Extract the displacement field with cyclic expansion on the first four sectors of the
         >>> # first stage at first mode
         >>> displacement = simulation.displacement(expand_cyclic=[1, 2, 3, 4])
         >>> print(displacement)  # doctest: +NORMALIZE_WHITESPACE
                      results       U (m)
                      set_ids           1
-        node_ids  components
-            1376           X  4.3586e-02
+         node_ids components
+             1376          X  4.3586e-02
                            Y -3.0071e-02
                            Z -9.4850e-05
-            4971           X  4.7836e-02
+             4971          X  4.7836e-02
                            Y  2.2711e-02
                            Z -9.4850e-05
-             ...
+              ...        ...         ...
         >>> # Extract the displacement field with cyclic expansion on the first two sectors of both
         >>> # stages at first mode
         >>> displacement = simulation.displacement(expand_cyclic=[[1, 2], [1, 2]])
         >>> print(displacement)  # doctest: +NORMALIZE_WHITESPACE
                      results       U (m)
                      set_ids           1
-        node_ids  components
-            1376           X  4.3586e-02
+         node_ids components
+             1376          X  4.3586e-02
                            Y -3.0071e-02
                            Z -9.4850e-05
-            4971           X  4.7836e-02
+             4971          X  4.7836e-02
                            Y  2.2711e-02
                            Z -9.4850e-05
-             ...
+              ...        ...         ...
         """
         return self._get_result(
             base_name="U",
             location=locations.nodal,
             category=ResultCategory.vector,
             components=components,
             norm=norm,
@@ -479,14 +553,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -495,67 +571,80 @@
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="S",
             location=location,
             category=ResultCategory.matrix,
             components=components,
@@ -565,71 +654,86 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="S",
             location=locations.elemental,
             category=ResultCategory.matrix,
             components=components,
@@ -639,14 +743,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -654,59 +760,72 @@
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="S",
             location=locations.nodal,
             category=ResultCategory.matrix,
             components=components,
@@ -716,14 +835,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_principal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -732,66 +853,79 @@
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract principal stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="S",
             location=location,
             category=ResultCategory.principal,
             components=components,
@@ -801,70 +935,85 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_principal_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         components: Union[List[str], List[int], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental principal stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="S",
             location=locations.elemental,
             category=ResultCategory.principal,
             components=components,
@@ -874,14 +1023,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_principal_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -889,58 +1040,71 @@
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal principal stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="S",
             location=locations.nodal,
             category=ResultCategory.principal,
             components=components,
@@ -950,14 +1114,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_eqv_von_mises(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -965,64 +1131,77 @@
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract equivalent von Mises stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="S",
             location=location,
             category=ResultCategory.equivalent,
             components=None,
@@ -1032,67 +1211,82 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_eqv_von_mises_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental equivalent von Mises stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="S",
             location=locations.elemental,
             category=ResultCategory.equivalent,
             components=None,
@@ -1102,70 +1296,85 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_eqv_von_mises_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal equivalent von Mises stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="S",
             location=locations.nodal,
             category=ResultCategory.equivalent,
             components=None,
@@ -1175,14 +1384,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -1191,67 +1402,80 @@
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPEL",
             location=location,
             category=ResultCategory.matrix,
             components=components,
@@ -1261,14 +1485,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -1276,59 +1502,72 @@
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPEL",
             location=locations.nodal,
             category=ResultCategory.matrix,
             components=components,
@@ -1338,71 +1577,86 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPEL",
             location=locations.elemental,
             category=ResultCategory.matrix,
             components=components,
@@ -1412,14 +1666,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_principal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -1428,66 +1684,79 @@
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract principal elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPEL",
             location=location,
             category=ResultCategory.principal,
             components=components,
@@ -1497,14 +1766,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_principal_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -1512,58 +1783,71 @@
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal principal elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPEL",
             location=locations.nodal,
             category=ResultCategory.principal,
             components=components,
@@ -1573,70 +1857,85 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_principal_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental principal elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPEL",
             location=locations.elemental,
             category=ResultCategory.principal,
             components=components,
@@ -1646,14 +1945,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_eqv_von_mises(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -1661,64 +1962,77 @@
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract equivalent von Mises elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPEL",
             location=location,
             category=ResultCategory.equivalent,
             components=None,
@@ -1728,67 +2042,82 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_eqv_von_mises_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental equivalent von Mises elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPEL",
             location=locations.elemental,
             category=ResultCategory.equivalent,
             components=None,
@@ -1798,70 +2127,85 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_eqv_von_mises_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal equivalent von Mises elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPEL",
             location=locations.nodal,
             category=ResultCategory.equivalent,
             components=None,
@@ -1871,14 +2215,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_state_variable(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -1886,64 +2232,77 @@
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract plastic state variable results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="ENL_PSV",
             location=location,
             category=ResultCategory.scalar,
             components=None,
@@ -1953,67 +2312,82 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_state_variable_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental plastic state variable results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="ENL_PSV",
             location=locations.elemental,
             category=ResultCategory.scalar,
             components=None,
@@ -2023,70 +2397,85 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_state_variable_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal plastic state variable results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="ENL_PSV",
             location=locations.nodal,
             category=ResultCategory.scalar,
             components=None,
@@ -2096,14 +2485,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -2112,67 +2503,80 @@
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPPL",
             location=location,
             category=ResultCategory.matrix,
             components=components,
@@ -2182,14 +2586,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -2197,59 +2603,72 @@
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPPL",
             location=locations.nodal,
             category=ResultCategory.matrix,
             components=components,
@@ -2259,71 +2678,86 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPPL",
             location=locations.elemental,
             category=ResultCategory.matrix,
             components=components,
@@ -2333,14 +2767,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_principal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -2349,66 +2785,79 @@
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract principal plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPPL",
             location=location,
             category=ResultCategory.principal,
             components=components,
@@ -2418,14 +2867,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_principal_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -2433,58 +2884,71 @@
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal principal plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPPL",
             location=locations.nodal,
             category=ResultCategory.principal,
             components=components,
@@ -2494,70 +2958,85 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_principal_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental principal plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPPL",
             location=locations.elemental,
             category=ResultCategory.principal,
             components=components,
@@ -2567,14 +3046,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_eqv(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -2582,64 +3063,77 @@
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract equivalent plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPPL",
             location=location,
             category=ResultCategory.equivalent,
             components=None,
@@ -2649,70 +3143,85 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_eqv_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal equivalent plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPPL",
             location=locations.nodal,
             category=ResultCategory.equivalent,
             components=None,
@@ -2722,67 +3231,82 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_eqv_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental equivalent plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EPPL",
             location=locations.elemental,
             category=ResultCategory.equivalent,
             components=None,
@@ -2792,14 +3316,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def reaction_force(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -2808,61 +3334,74 @@
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract reaction force results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z",
-                and their respective equivalents 1, 2, 3.
-            norm:
-                Whether to return the norm of the results.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="RF",
             location=locations.nodal,
             category=ResultCategory.vector,
             components=components,
@@ -2873,67 +3412,82 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elemental_volume(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental volume results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="ENG_VOL",
             location=locations.elemental,
             category=ResultCategory.scalar,
             components=None,
@@ -2943,67 +3497,82 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elemental_mass(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental mass results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="ElementalMass",
             location=locations.elemental,
             category=ResultCategory.scalar,
             components=None,
@@ -3013,67 +3582,82 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def element_centroids(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract element centroids results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="centroids",
             location=locations.elemental,
             category=ResultCategory.scalar,
             components=None,
@@ -3083,67 +3667,82 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def thickness(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract element thickness results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="thickness",
             location=locations.elemental,
             category=ResultCategory.scalar,
             components=None,
@@ -3153,14 +3752,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def element_orientations(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -3168,64 +3769,77 @@
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental nodal element orientations results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EUL",
             location=location,
             category=ResultCategory.scalar,
             components=None,
@@ -3235,67 +3849,82 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def element_orientations_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental element orientations results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EUL",
             location=locations.elemental,
             category=ResultCategory.scalar,
             components=None,
@@ -3305,70 +3934,85 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def element_orientations_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal element orientations results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="EUL",
             location=locations.nodal,
             category=ResultCategory.scalar,
             components=None,
@@ -3378,14 +4022,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def hydrostatic_pressure(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -3393,64 +4039,77 @@
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract hydrostatic pressure element nodal results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="ENL_HPRES",
             location=location,
             category=ResultCategory.scalar,
             components=None,
@@ -3460,70 +4119,85 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def hydrostatic_pressure_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract hydrostatic pressure nodal results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="ENL_HPRES",
             location=locations.nodal,
             category=ResultCategory.scalar,
             components=None,
@@ -3533,67 +4207,82 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def hydrostatic_pressure_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract hydrostatic pressure elemental results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="ENL_HPRES",
             location=locations.elemental,
             category=ResultCategory.scalar,
             components=None,
@@ -3603,14 +4292,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def element_nodal_forces(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -3620,69 +4311,82 @@
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract element nodal forces results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z",
-                and their respective equivalents 1, 2, 3.
-            norm:
-                Whether to return the norm of the results.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="ENF",
             location=location,
             category=ResultCategory.vector,
             components=components,
@@ -3693,14 +4397,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def element_nodal_forces_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -3709,61 +4415,74 @@
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract element nodal forces nodal results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z",
-                and their respective equivalents 1, 2, 3.
-            norm:
-                Whether to return the norm of the results.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="ENF",
             location=locations.nodal,
             category=ResultCategory.vector,
             components=components,
@@ -3774,14 +4493,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def element_nodal_forces_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
@@ -3789,59 +4510,72 @@
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract element nodal forces elemental results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            elements:
-                List of elements to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z",
-                and their respective equivalents 1, 2, 3.
-            norm:
-                Whether to return the norm of the results.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selection:
-                Named selection to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="ENF",
             location=locations.elemental,
             category=ResultCategory.vector,
             components=components,
@@ -3852,14 +4586,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def nodal_force(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -3868,61 +4604,74 @@
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal force results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements whose nodes to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z",
-                and their respective equivalents 1, 2, 3.
-            norm:
-                Whether to return the norm of the results.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements whose nodes to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="F",
             location=locations.nodal,
             category=ResultCategory.vector,
             components=components,
@@ -3933,14 +4682,16 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def nodal_moment(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         frequencies: Union[float, List[float], None] = None,
@@ -3949,61 +4700,74 @@
         modes: Union[int, List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal moment results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
         exclusive.
         If none of the above is given, only the first mode will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-         Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements whose nodes to get results for.
-            frequencies:
-                Frequency value or list of frequency values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z",
-                and their respective equivalents 1, 2, 3.
-            norm:
-                Whether to return the norm of the results.
-            modes:
-                Mode number or list of mode numbers to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            set_ids:
-                Sets to get results for. Equivalent to modes.
-                Common to all simulation types for easier scripting.
-            all_sets:
-                Whether to get results for all sets/modes.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements whose nodes to get results for.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        set_ids:
+            Sets to get results for. Equivalent to modes.
+            Common to all simulation types for easier scripting.
+        all_sets:
+            Whether to get results for all sets/modes.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
             base_name="M",
             location=locations.nodal,
             category=ResultCategory.vector,
             components=components,
@@ -4014,8 +4778,10 @@
             all_sets=all_sets,
             modes=modes,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             expand_cyclic=expand_cyclic,
             phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
```

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/post_utility.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/post_utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This module is used for the initialization of PyDPF-Post objects.
 """
 from typing import TypeVar, Union
 import warnings
 
 from ansys.dpf.core.model import Model
+from ansys.dpf.core.server_types import BaseServer
 
 from ansys.dpf.post.common import (
     AvailableSimulationTypes,
     _AnalysisType,
     _AvailableKeywords,
     _PhysicsType,
     simulation_type_str_to_class,
@@ -29,14 +30,17 @@
     TransientAnalysisSolution,
 )
 
 
 def load_solution(data_sources, physics_type=None, analysis_type=None):
     """Loads a solution and returns a :class:`ansys.dpf.post.Result` object.
 
+    .. deprecated:: 3.0
+       Use :func:`load_simulation` instead.
+
     This class provides information on a given set on a given scoping.
 
     Parameters
     ----------
     data_sources: str, ansys.dpf.core.DataSources
          Path to the file to open or the :class:`ansys.dpf.core.DataSources` class.
     physics_type: common._PhysicsType, str, optional
@@ -45,17 +49,14 @@
         the data sources are read to determine the physics type.
     analysis_type: common._AnalysisType, str, optional
         Type of analysis described in the specified data sources. Options are
         ``"static"``, ``"modal"``, ``"harmonic"``, and ``"transient"``. The
         default is ``None``, in which case the data sources are read to determine
         the analysis type.
 
-    .. deprecated:: 3.0
-       Use :func:`load_simulation` instead.
-
     Examples
     --------
     Load the example static result.
 
     >>> from ansys.dpf import post
     >>> from ansys.dpf.post import examples
     >>> solution = post.load_solution(examples.static_rst)
@@ -113,14 +114,15 @@
 
 SimulationType = TypeVar("SimulationType", bound=Simulation)
 
 
 def load_simulation(
     data_sources,
     simulation_type: Union[AvailableSimulationTypes, str] = None,
+    server: Union[BaseServer, None] = None,
 ) -> SimulationType:
     """Loads a simulation and returns a :class:`ansys.dpf.post.simulation.Simulation` object.
 
     This class provides the main interface to explore and manipulate results, meshes, geometries,
     and other entities associated with the result files given in input.
     The interface exposed depends on the type of simulation selected with the argument
     `simulation_type`. Each one proposes a post-processing context with its specific vocabulary and
@@ -138,14 +140,16 @@
         expectations and vocabulary of each context.
         This defaults to the simulation type corresponding to the combination of physics type
         and analysis type detected automatically by DPF when reading the result files.
         If nothing is detected, this will default to a static mechanical type of simulation.
         The best practice is to define this parameter to select the right post-processing context.
         Options are given in
         :class:`<AvailableSimulationTypes> ansys.dpf.post.common.AvailableSimulationTypes`.
+    server:
+        DPF server connected to a remote or local instance.
 
     Returns
     -------
     An instance of one of the subclasses of the
     :class:`Simulation <ansys.dpf.post.simulation.Simulation>` class.
 
     .. versionadded:: 3.0
@@ -155,15 +159,15 @@
     --------
     Load the example static result.
 
     >>> from ansys.dpf import post
     >>> from ansys.dpf.post import examples
     >>> simulation = post.load_simulation(examples.static_rst)
     """
-    _model = Model(data_sources)
+    _model = Model(data_sources, server=server)
     data_sources = _model.metadata.data_sources
 
     if not simulation_type:
         try:
             physics_type = _model.metadata.result_info.physics_type
         except Exception as e:
             warnings.warn(
@@ -187,15 +191,15 @@
         if physics_type == _PhysicsType.thermal:
             if analysis_type == _AnalysisType.static:
                 raise NotImplementedError
             elif analysis_type == _AnalysisType.transient:
                 raise NotImplementedError
             else:
                 raise ValueError(
-                    f"Unknown analysis type '{analysis_type}' for thermal."
+                    f"Unknown analysis type '{analysis_type}' for {physics_type}."
                 )
         elif (
             physics_type == _PhysicsType.mecanic
             or physics_type == _PhysicsType.mechanical
         ):
             if analysis_type == _AnalysisType.static:
                 simulation_type = AvailableSimulationTypes.static_mechanical
@@ -206,23 +210,34 @@
                 or analysis_type == _AnalysisType.msup
             ):
                 simulation_type = AvailableSimulationTypes.harmonic_mechanical
             elif analysis_type == _AnalysisType.transient:
                 simulation_type = AvailableSimulationTypes.transient_mechanical
             else:
                 raise ValueError(
-                    f"Unknown analysis type '{analysis_type}' for mechanical."
+                    f"Unknown analysis type '{analysis_type}' for {physics_type}."
+                )
+        elif physics_type == _PhysicsType.fluid:
+            if analysis_type in [_AnalysisType.steady, _AnalysisType.static]:
+                simulation_type = AvailableSimulationTypes.steady_fluid
+            elif analysis_type in [_AnalysisType.unsteady, _AnalysisType.transient]:
+                simulation_type = AvailableSimulationTypes.unsteady_fluid
+            else:
+                raise ValueError(
+                    f"Unknown analysis type '{analysis_type}' for {physics_type}."
                 )
         else:
             raise ValueError(f"Unknown physics type '{physics_type}.")
 
     if simulation_type in [
         getattr(AvailableSimulationTypes, x) for x in vars(AvailableSimulationTypes)
     ]:
-        return simulation_type_str_to_class[simulation_type](data_sources)
+        return simulation_type_str_to_class[simulation_type](
+            data_sources, server=_model._server
+        )
     else:
         raise ValueError(
             f"Simulation type '{simulation_type}' is not a recognized simulation type."
             f" Please use ansys.dpf.post.common.AvailableSimulationTypes or instantiate one of the"
             f" available Simulation sub-classes directly."
         )
```

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/result_data.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/result_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,15 +389,15 @@
                 pl.add_field(field_m, mesh_m)
             # Add the mesh associated to the path
             pl.add_mesh(
                 self._evaluator._model.metadata.meshed_region,
                 style="surface",
                 show_edges=True,
                 opacity=0.3,
-                **kwargs
+                **kwargs,
             )
             # Show the plot
             pl.show_figure(**kwargs)
 
         # If not plotting on a path
         else:
             # Initialize a Plotter
```

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/result_definition.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/result_definition.py`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/result_evaluation.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/result_evaluation.py`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/result_object.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/result_object.py`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/scalar.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/scalar.py`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/static_mechanical_simulation.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/transient_mechanical_simulation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""Module containing the ``StaticMechanicalSimulation`` class.
+"""Module containing the ``TransientMechanicalSimulation`` class.
 
-StaticMechanicalSimulation
---------------------------
+TransientMechanicalSimulation
+-----------------------------
 
 """
 from typing import List, Tuple, Union
 
-from ansys.dpf import core
+from ansys.dpf import core as dpf
 from ansys.dpf.post import locations
 from ansys.dpf.post.dataframe import DataFrame
-from ansys.dpf.post.selection import Selection
+from ansys.dpf.post.selection import Selection, _WfNames
 from ansys.dpf.post.simulation import MechanicalSimulation, ResultCategory
 
 
-class StaticMechanicalSimulation(MechanicalSimulation):
-    """Provides methods for mechanical static simulations."""
+class TransientMechanicalSimulation(MechanicalSimulation):
+    """Provides methods for mechanical transient simulations."""
 
     def _get_result(
         self,
         base_name: str,
         location: str,
         category: ResultCategory,
         components: Union[str, List[str], int, List[int], None] = None,
@@ -29,72 +29,77 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         named_selections: Union[List[str], str, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            base_name:
-                Base name for the requested result.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            category:
-                Type of result requested. See the :class:`ResultCategory` class.
-            components:
-                Components to get results for.
-            norm:
-                Whether to return the norm of the results.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            times:
-                List of times to get results for.
-            set_ids:
-                List of sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            named_selections:
-                Named selection or list of named selections to get results for.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        base_name:
+            Base name for the requested result.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        category:
+            Type of result requested. See the :class:`ResultCategory` class.
+        components:
+            Components to get results for.
+        norm:
+            Whether to return the norm of the results.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+            It takes precedence over any other filter argument.
+        times:
+            List of times to get results for.
+        set_ids:
+            List of sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         # Build the targeted time scoping
@@ -108,108 +113,145 @@
         if tot > 1:
             raise ValueError(
                 "Arguments all_sets, selection, set_ids, times, "
                 "and load_steps are mutually exclusive."
             )
 
         selection = self._build_selection(
+            base_name=base_name,
+            category=category,
             selection=selection,
             set_ids=set_ids,
             times=times,
             load_steps=load_steps,
             all_sets=all_sets,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
             location=location,
+            external_layer=external_layer,
+            skin=skin,
         )
 
         comp, to_extract, columns = self._create_components(
             base_name, category, components
         )
 
         # Initialize a workflow
-        wf = core.Workflow(server=self._model._server)
-        wf.progress_bar = False
+        wf = dpf.Workflow(server=self._model._server)
 
-        if category == ResultCategory.equivalent and base_name[0] == "E":
-            force_elemental_nodal = True
-        else:
-            force_elemental_nodal = False
+        force_elemental_nodal = self._requires_manual_averaging(
+            base_name=base_name,
+            location=location,
+            category=category,
+            selection=selection,
+        )
 
         # Instantiate the main result operator
-        result_op = self._build_result_operator(
+        wf, result_op = self._build_result_workflow(
             name=base_name,
             location=location,
             force_elemental_nodal=force_elemental_nodal,
         )
-
-        # Treat cyclic cases
-        result_op = self._treat_cyclic(expand_cyclic, phase_angle_cyclic, result_op)
-
         # Its output is selected as future workflow output for now
         out = result_op.outputs.fields_container
         # Its inputs are selected as workflow inputs for merging with selection workflows
         wf.set_input_name("time_scoping", result_op.inputs.time_scoping)
         wf.set_input_name("mesh_scoping", result_op.inputs.mesh_scoping)
 
         wf.connect_with(
             selection.time_freq_selection._selection,
             output_input_names=("scoping", "time_scoping"),
         )
+        if selection.requires_mesh:
+            # wf.set_input_name(_WfNames.mesh, result_op.inputs.mesh)
+            mesh_wf = dpf.Workflow(server=self._model._server)
+            mesh_wf.set_output_name(
+                _WfNames.initial_mesh, self._model.metadata.mesh_provider
+            )
+            selection.spatial_selection._selection.connect_with(
+                mesh_wf,
+                output_input_names={_WfNames.initial_mesh: _WfNames.initial_mesh},
+            )
         wf.connect_with(
             selection.spatial_selection._selection,
-            output_input_names=("scoping", "mesh_scoping"),
+            output_input_names={
+                "scoping": "mesh_scoping",
+            },
         )
 
         # Connect data_sources and streams_container inputs of selection if necessary
         if "streams" in wf.input_names:
             wf.connect("streams", self._model.metadata.streams_provider)
         if "data_sources" in wf.input_names:
             wf.connect("data_sources", self._model.metadata.data_sources)
 
+        average_op = None
+        if force_elemental_nodal:
+            average_op = self._create_averaging_operator(
+                location=location, selection=selection
+            )
+
         # Add a step to compute principal invariants if result is principal
         if category == ResultCategory.principal:
             # Instantiate the required operator
             principal_op = self._model.operator(name="invariants_fc")
             # Corresponds to scripting name principal_invariants
-            principal_op.connect(0, out)
-            wf.add_operator(operator=principal_op)
+            if average_op is not None:
+                average_op[0].connect(0, out)
+                principal_op.connect(0, average_op[1])
+                # Set as future output of the workflow
+                average_op = None
+            else:
+                principal_op.connect(0, out)
             # Set as future output of the workflow
             if len(to_extract) == 1:
                 out = getattr(principal_op.outputs, f"fields_eig_{to_extract[0]+1}")
             else:
                 raise NotImplementedError("Cannot combine principal results yet.")
                 # We need to define the behavior for storing different results in a DataFrame
 
         # Add a step to compute equivalent if result is equivalent
         elif category == ResultCategory.equivalent:
             equivalent_op = self._model.operator(name="eqv_fc")
-            equivalent_op.connect(0, out)
             wf.add_operator(operator=equivalent_op)
-            # Set as future output of the workflow
-            out = equivalent_op.outputs.fields_container
             # If a strain result, change the location now
-            if force_elemental_nodal:
-                average_op = None
-                if location == locations.nodal:
-                    average_op = self._model.operator(name="to_nodal_fc")
-                elif location == locations.elemental:
-                    average_op = self._model.operator(name="to_elemental_fc")
-                if average_op is not None:
-                    average_op.connect(0, out)
-                    wf.add_operator(operator=average_op)
-                    # Set as future output of the workflow
-                    out = average_op.outputs.fields_container
+            if (
+                average_op is not None
+                and category == ResultCategory.equivalent
+                and base_name[0] == "E"
+            ):
+                equivalent_op.connect(0, out)
+                average_op[0].connect(0, equivalent_op)
+                wf.add_operator(operator=average_op[1])
+                # Set as future output of the workflow
+                out = average_op[1].outputs.fields_container
+            elif average_op is not None:
+                average_op[0].connect(0, out)
+                equivalent_op.connect(0, average_op[1])
+                # Set as future output of the workflow
+                out = equivalent_op.outputs.fields_container
+            else:
+                equivalent_op.connect(0, out)
+                out = equivalent_op.outputs.fields_container
+            average_op = None
             base_name += "_VM"
 
+        if average_op is not None:
+            average_op[0].connect(0, out)
+            out = average_op[1].outputs.fields_container
+
         # Add an optional component selection step if result is vector, matrix, or principal
-        if (category in [ResultCategory.vector, ResultCategory.matrix]) and (
-            to_extract is not None
-        ):
+        if (
+            category
+            in [
+                ResultCategory.vector,
+                ResultCategory.matrix,
+            ]
+        ) and (to_extract is not None):
             # Instantiate a component selector operator
             extract_op = self._model.operator(name="component_selector_fc")
             # Feed it the current workflow output
             extract_op.connect(0, out)
             # Feed it the requested components
             extract_op.connect(1, to_extract)
             wf.add_operator(operator=extract_op)
@@ -226,20 +268,30 @@
             wf.add_operator(operator=norm_op)
             out = norm_op.outputs.fields_container
             comp = None
             base_name += "_N"
 
         # Set the workflow output
         wf.set_output_name("out", out)
+        wf.progress_bar = False
         # Evaluate  the workflow
-        fc = wf.get_output("out", core.types.fields_container)
+        fc = wf.get_output("out", dpf.types.fields_container)
 
         disp_wf = self._generate_disp_workflow(fc, selection)
 
-        return self._create_dataframe(fc, location, columns, comp, base_name, disp_wf)
+        submesh = None
+        if selection.outputs_mesh:
+            selection.spatial_selection._selection.progress_bar = False
+            submesh = selection.spatial_selection._selection.get_output(
+                _WfNames.mesh, dpf.types.meshed_region
+            )
+
+        return self._create_dataframe(
+            fc, location, columns, comp, base_name, disp_wf=disp_wf, submesh=submesh
+        )
 
     def displacement(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
@@ -247,61 +299,64 @@
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract displacement results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements whose nodes to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z",
-                and their respective equivalents 1, 2, 3.
-            norm:
-                Whether to return the norm of the results.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements whose nodes to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -314,16 +369,192 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
+        )
+
+    def velocity(
+        self,
+        node_ids: Union[List[int], None] = None,
+        element_ids: Union[List[int], None] = None,
+        times: Union[float, List[float], None] = None,
+        components: Union[str, List[str], int, List[int], None] = None,
+        norm: bool = False,
+        set_ids: Union[int, List[int], None] = None,
+        all_sets: bool = False,
+        load_steps: Union[
+            int, List[int], Tuple[int, Union[int, List[int]]], None
+        ] = None,
+        named_selections: Union[List[str], str, None] = None,
+        selection: Union[Selection, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
+    ) -> DataFrame:
+        """Extract velocity results from the simulation.
+
+        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
+        exclusive.
+        If none of the above is given, only the last result will be returned.
+
+        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
+        exclusive.
+        If none of the above is given, results will be extracted for the whole mesh.
+
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements whose nodes to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
+
+        Returns
+        -------
+            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+
+        """
+        return self._get_result(
+            base_name="V",
+            location=locations.nodal,
+            category=ResultCategory.vector,
+            components=components,
+            norm=norm,
+            selection=selection,
+            times=times,
+            set_ids=set_ids,
+            all_sets=all_sets,
+            load_steps=load_steps,
+            node_ids=node_ids,
+            element_ids=element_ids,
+            named_selections=named_selections,
+            external_layer=external_layer,
+            skin=skin,
+        )
+
+    def acceleration(
+        self,
+        node_ids: Union[List[int], None] = None,
+        element_ids: Union[List[int], None] = None,
+        times: Union[float, List[float], None] = None,
+        components: Union[str, List[str], int, List[int], None] = None,
+        norm: bool = False,
+        set_ids: Union[int, List[int], None] = None,
+        all_sets: bool = False,
+        load_steps: Union[
+            int, List[int], Tuple[int, Union[int, List[int]]], None
+        ] = None,
+        named_selections: Union[List[str], str, None] = None,
+        selection: Union[Selection, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
+    ) -> DataFrame:
+        """Extract acceleration results from the simulation.
+
+        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
+        exclusive.
+        If none of the above is given, only the last result will be returned.
+
+        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
+        exclusive.
+        If none of the above is given, results will be extracted for the whole mesh.
+
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements whose nodes to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
+
+        Returns
+        -------
+            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+
+        """
+        return self._get_result(
+            base_name="A",
+            location=locations.nodal,
+            category=ResultCategory.vector,
+            components=components,
+            norm=norm,
+            selection=selection,
+            times=times,
+            set_ids=set_ids,
+            all_sets=all_sets,
+            load_steps=load_steps,
+            node_ids=node_ids,
+            element_ids=element_ids,
+            named_selections=named_selections,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -332,67 +563,70 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
-        Arguments `selection`, `named_selections`, and `element_ids` are mutually
+        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -404,73 +638,76 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -482,16 +719,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -499,59 +736,62 @@
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -563,16 +803,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_principal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[List[float], None] = None,
@@ -581,67 +821,69 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract principal stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
-
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -653,72 +895,75 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_principal_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[List[float], None] = None,
         components: Union[List[str], List[int], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental principal stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -730,16 +975,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_principal_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[List[float], None] = None,
@@ -747,58 +992,61 @@
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal principal stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs pf elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -810,16 +1058,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_eqv_von_mises(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[List[float], None] = None,
@@ -827,64 +1075,67 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract equivalent von Mises stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -896,69 +1147,72 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_eqv_von_mises_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental equivalent von Mises stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -970,72 +1224,75 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def stress_eqv_von_mises_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal equivalent von Mises stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -1047,16 +1304,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -1065,67 +1322,70 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -1137,16 +1397,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -1154,59 +1414,62 @@
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -1218,73 +1481,76 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract stress results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -1296,16 +1562,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_principal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -1314,66 +1580,69 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract principal elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -1385,16 +1654,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_principal_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -1402,58 +1671,61 @@
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal principal elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs pf elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -1465,72 +1737,75 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_principal_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental principal elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -1542,16 +1817,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_eqv_von_mises(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[List[float], None] = None,
@@ -1559,64 +1834,67 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract equivalent von Mises elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -1628,69 +1906,72 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_eqv_von_mises_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental equivalent von Mises elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -1702,72 +1983,75 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elastic_strain_eqv_von_mises_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal equivalent von Mises elastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -1779,16 +2063,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_state_variable(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -1796,64 +2080,67 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract plastic state variable results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -1865,69 +2152,72 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_state_variable_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental plastic state variable results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -1939,72 +2229,75 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_state_variable_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal plastic state variable results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -2016,16 +2309,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -2034,67 +2327,70 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -2106,16 +2402,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -2123,59 +2419,62 @@
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -2187,73 +2486,76 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
+            "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -2265,16 +2567,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_principal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -2283,66 +2585,69 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract principal plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -2354,16 +2659,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_principal_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -2371,58 +2676,61 @@
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal principal plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs pf elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -2434,72 +2742,75 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_principal_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental principal plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are: 1, 2, and 3.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -2511,16 +2822,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_eqv(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -2528,64 +2839,67 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract equivalent plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -2597,72 +2911,75 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_eqv_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal equivalent plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -2674,69 +2991,72 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def plastic_strain_eqv_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental equivalent plastic strain results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -2748,748 +3068,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
-        )
-
-    def creep_strain(
-        self,
-        node_ids: Union[List[int], None] = None,
-        element_ids: Union[List[int], None] = None,
-        times: Union[float, List[float], None] = None,
-        components: Union[str, List[str], int, List[int], None] = None,
-        set_ids: Union[int, List[int], None] = None,
-        all_sets: bool = False,
-        load_steps: Union[
-            int, List[int], Tuple[int, Union[int, List[int]]], None
-        ] = None,
-        named_selections: Union[List[str], str, None] = None,
-        selection: Union[Selection, None] = None,
-        location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
-    ) -> DataFrame:
-        """Extract creep strain results from the simulation.
-
-        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
-        exclusive.
-        If none of the above is given, only the last result will be returned.
-
-        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
-        exclusive.
-        If none of the above is given, results will be extracted for the whole mesh.
-
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
-
-        Returns
-        -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
-
-        """
-        return self._get_result(
-            base_name="ECR",
-            location=location,
-            category=ResultCategory.matrix,
-            components=components,
-            selection=selection,
-            times=times,
-            set_ids=set_ids,
-            all_sets=all_sets,
-            load_steps=load_steps,
-            node_ids=node_ids,
-            element_ids=element_ids,
-            named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
-        )
-
-    def creep_strain_nodal(
-        self,
-        node_ids: Union[List[int], None] = None,
-        element_ids: Union[List[int], None] = None,
-        times: Union[float, List[float], None] = None,
-        components: Union[str, List[str], int, List[int], None] = None,
-        set_ids: Union[int, List[int], None] = None,
-        all_sets: bool = False,
-        load_steps: Union[
-            int, List[int], Tuple[int, Union[int, List[int]]], None
-        ] = None,
-        named_selections: Union[List[str], str, None] = None,
-        selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
-    ) -> DataFrame:
-        """Extract nodal creep strain results from the simulation.
-
-        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
-        exclusive.
-        If none of the above is given, only the last result will be returned.
-
-        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
-        exclusive.
-        If none of the above is given, results will be extracted for the whole mesh.
-
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
-
-        Returns
-        -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
-
-        """
-        return self._get_result(
-            base_name="ECR",
-            location=locations.nodal,
-            category=ResultCategory.matrix,
-            components=components,
-            selection=selection,
-            times=times,
-            set_ids=set_ids,
-            all_sets=all_sets,
-            load_steps=load_steps,
-            node_ids=node_ids,
-            element_ids=element_ids,
-            named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
-        )
-
-    def creep_strain_elemental(
-        self,
-        element_ids: Union[List[int], None] = None,
-        times: Union[float, List[float], None] = None,
-        components: Union[str, List[str], int, List[int], None] = None,
-        set_ids: Union[int, List[int], None] = None,
-        all_sets: bool = False,
-        load_steps: Union[
-            int, List[int], Tuple[int, Union[int, List[int]]], None
-        ] = None,
-        named_selections: Union[List[str], str, None] = None,
-        selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
-    ) -> DataFrame:
-        """Extract elemental creep strain results from the simulation.
-
-        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
-        exclusive.
-        If none of the above is given, only the last result will be returned.
-
-        Arguments `selection`, `named_selections`, and `element_ids` are mutually
-        exclusive.
-        If none of the above is given, results will be extracted for the whole mesh.
-
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z", "XX", "XY",
-                "XZ", and their respective equivalents 1, 2, 3, 4, 5, 6.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
-
-        Returns
-        -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
-
-        """
-        return self._get_result(
-            base_name="ECR",
-            location=locations.elemental,
-            category=ResultCategory.matrix,
-            components=components,
-            selection=selection,
-            times=times,
-            set_ids=set_ids,
-            all_sets=all_sets,
-            load_steps=load_steps,
-            node_ids=None,
-            element_ids=element_ids,
-            named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
-        )
-
-    def creep_strain_principal(
-        self,
-        node_ids: Union[List[int], None] = None,
-        element_ids: Union[List[int], None] = None,
-        times: Union[float, List[float], None] = None,
-        components: Union[str, List[str], int, List[int], None] = None,
-        set_ids: Union[int, List[int], None] = None,
-        all_sets: bool = False,
-        load_steps: Union[
-            int, List[int], Tuple[int, Union[int, List[int]]], None
-        ] = None,
-        named_selections: Union[List[str], str, None] = None,
-        selection: Union[Selection, None] = None,
-        location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
-    ) -> DataFrame:
-        """Extract principal creep strain results from the simulation.
-
-        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
-        exclusive.
-        If none of the above is given, only the last result will be returned.
-
-        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
-        exclusive.
-        If none of the above is given, results will be extracted for the whole mesh.
-
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
-
-        Returns
-        -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
-
-        """
-        return self._get_result(
-            base_name="ECR",
-            location=location,
-            category=ResultCategory.principal,
-            components=components,
-            selection=selection,
-            times=times,
-            set_ids=set_ids,
-            all_sets=all_sets,
-            load_steps=load_steps,
-            node_ids=node_ids,
-            element_ids=element_ids,
-            named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
-        )
-
-    def creep_strain_principal_nodal(
-        self,
-        node_ids: Union[List[int], None] = None,
-        element_ids: Union[List[int], None] = None,
-        times: Union[float, List[float], None] = None,
-        components: Union[str, List[str], int, List[int], None] = None,
-        set_ids: Union[int, List[int], None] = None,
-        all_sets: bool = False,
-        load_steps: Union[
-            int, List[int], Tuple[int, Union[int, List[int]]], None
-        ] = None,
-        named_selections: Union[List[str], str, None] = None,
-        selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
-    ) -> DataFrame:
-        """Extract nodal principal creep strain results from the simulation.
-
-        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
-        exclusive.
-        If none of the above is given, only the last result will be returned.
-
-        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
-        exclusive.
-        If none of the above is given, results will be extracted for the whole mesh.
-
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
-
-        Returns
-        -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
-
-        """
-        return self._get_result(
-            base_name="ECR",
-            location=locations.nodal,
-            category=ResultCategory.principal,
-            components=components,
-            selection=selection,
-            times=times,
-            set_ids=set_ids,
-            all_sets=all_sets,
-            load_steps=load_steps,
-            node_ids=node_ids,
-            element_ids=element_ids,
-            named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
-        )
-
-    def creep_strain_principal_elemental(
-        self,
-        element_ids: Union[List[int], None] = None,
-        times: Union[float, List[float], None] = None,
-        components: Union[str, List[str], int, List[int], None] = None,
-        set_ids: Union[int, List[int], None] = None,
-        all_sets: bool = False,
-        load_steps: Union[
-            int, List[int], Tuple[int, Union[int, List[int]]], None
-        ] = None,
-        named_selections: Union[List[str], str, None] = None,
-        selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
-    ) -> DataFrame:
-        """Extract elemental principal creep strain results from the simulation.
-
-        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
-        exclusive.
-        If none of the above is given, only the last result will be returned.
-
-        Arguments `selection`, `named_selections`, and `element_ids` are mutually
-        exclusive.
-        If none of the above is given, results will be extracted for the whole mesh.
-
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are: 1, 2, and 3.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
-
-        Returns
-        -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
-
-        """
-        return self._get_result(
-            base_name="ECR",
-            location=locations.elemental,
-            category=ResultCategory.principal,
-            components=components,
-            selection=selection,
-            times=times,
-            set_ids=set_ids,
-            all_sets=all_sets,
-            load_steps=load_steps,
-            node_ids=None,
-            element_ids=element_ids,
-            named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
-        )
-
-    def creep_strain_eqv(
-        self,
-        node_ids: Union[List[int], None] = None,
-        element_ids: Union[List[int], None] = None,
-        times: Union[float, List[float], None] = None,
-        set_ids: Union[int, List[int], None] = None,
-        all_sets: bool = False,
-        load_steps: Union[
-            int, List[int], Tuple[int, Union[int, List[int]]], None
-        ] = None,
-        named_selections: Union[List[str], str, None] = None,
-        selection: Union[Selection, None] = None,
-        location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
-    ) -> DataFrame:
-        """Extract equivalent creep strain results from the simulation.
-
-        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
-        exclusive.
-        If none of the above is given, only the last result will be returned.
-
-        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
-        exclusive.
-        If none of the above is given, results will be extracted for the whole mesh.
-
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
-
-        Returns
-        -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
-
-        """
-        return self._get_result(
-            base_name="ECR",
-            location=location,
-            category=ResultCategory.equivalent,
-            components=None,
-            selection=selection,
-            times=times,
-            set_ids=set_ids,
-            all_sets=all_sets,
-            load_steps=load_steps,
-            node_ids=node_ids,
-            element_ids=element_ids,
-            named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
-        )
-
-    def creep_strain_equivalent_nodal(
-        self,
-        node_ids: Union[List[int], None] = None,
-        element_ids: Union[List[int], None] = None,
-        times: Union[float, List[float], None] = None,
-        set_ids: Union[int, List[int], None] = None,
-        all_sets: bool = False,
-        load_steps: Union[
-            int, List[int], Tuple[int, Union[int, List[int]]], None
-        ] = None,
-        named_selections: Union[List[str], str, None] = None,
-        selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
-    ) -> DataFrame:
-        """Extract nodal equivalent creep strain results from the simulation.
-
-        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
-        exclusive.
-        If none of the above is given, only the last result will be returned.
-
-        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
-        exclusive.
-        If none of the above is given, results will be extracted for the whole mesh.
-
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
-
-        Returns
-        -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
-
-        """
-        return self._get_result(
-            base_name="ECR",
-            location=locations.nodal,
-            category=ResultCategory.equivalent,
-            components=None,
-            selection=selection,
-            times=times,
-            set_ids=set_ids,
-            all_sets=all_sets,
-            load_steps=load_steps,
-            node_ids=node_ids,
-            element_ids=element_ids,
-            named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
-        )
-
-    def creep_strain_equivalent_elemental(
-        self,
-        element_ids: Union[List[int], None] = None,
-        times: Union[float, List[float], None] = None,
-        set_ids: Union[int, List[int], None] = None,
-        all_sets: bool = False,
-        load_steps: Union[
-            int, List[int], Tuple[int, Union[int, List[int]]], None
-        ] = None,
-        named_selections: Union[List[str], str, None] = None,
-        selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
-    ) -> DataFrame:
-        """Extract elemental equivalent creep strain results from the simulation.
-
-        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
-        exclusive.
-        If none of the above is given, only the last result will be returned.
-
-        Arguments `selection`, `named_selections`, and `element_ids` are mutually
-        exclusive.
-        If none of the above is given, results will be extracted for the whole mesh.
-
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
-
-        Returns
-        -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
-
-        """
-        return self._get_result(
-            base_name="ECR",
-            location=locations.elemental,
-            category=ResultCategory.equivalent,
-            components=None,
-            selection=selection,
-            times=times,
-            set_ids=set_ids,
-            all_sets=all_sets,
-            load_steps=load_steps,
-            node_ids=None,
-            element_ids=element_ids,
-            named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def reaction_force(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -3498,61 +3086,64 @@
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract reaction force results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z",
-                and their respective equivalents 1, 2, 3.
-            norm:
-                Whether to return the norm of the results.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -3565,72 +3156,72 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elemental_volume(
         self,
-        node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental volume results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -3639,72 +3230,75 @@
             category=ResultCategory.scalar,
             components=None,
             selection=selection,
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
-            node_ids=node_ids,
+            node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elemental_mass(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental mass results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -3716,69 +3310,72 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def elemental_heat_generation(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental heat generation results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -3790,69 +3387,72 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def element_centroids(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract element centroids results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -3864,69 +3464,72 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def thickness(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract element thickness results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -3938,16 +3541,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def element_orientations(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -3955,64 +3558,67 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract element orientations results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -4024,69 +3630,72 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def element_orientations_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract elemental element orientations results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -4098,72 +3707,75 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def element_orientations_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal element orientations results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -4175,143 +3787,72 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
-        )
-
-    def stiffness_matrix_energy(
-        self,
-        element_ids: Union[List[int], None] = None,
-        times: Union[float, List[float], None] = None,
-        set_ids: Union[int, List[int], None] = None,
-        all_sets: bool = False,
-        load_steps: Union[
-            int, List[int], Tuple[int, Union[int, List[int]]], None
-        ] = None,
-        named_selections: Union[List[str], str, None] = None,
-        selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
-    ) -> DataFrame:
-        """Extract stiffness matrix energy results from the simulation.
-
-        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
-        exclusive.
-        If none of the above is given, only the last result will be returned.
-
-        Arguments `selection`, `named_selections`, and `element_ids` are mutually
-        exclusive.
-        If none of the above is given, results will be extracted for the whole mesh.
-
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
-
-        Returns
-        -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
-
-        """
-        return self._get_result(
-            base_name="ENG_SE",
-            location=locations.elemental,
-            category=ResultCategory.scalar,
-            components="",
-            selection=selection,
-            times=times,
-            set_ids=set_ids,
-            all_sets=all_sets,
-            load_steps=load_steps,
-            node_ids=None,
-            element_ids=element_ids,
-            named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def artificial_hourglass_energy(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract artificial hourglass energy results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -4323,69 +3864,72 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def thermal_dissipation_energy(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract thermal dissipation energy results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -4397,69 +3941,72 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def kinetic_energy(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract kinetic energy results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -4471,16 +4018,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def hydrostatic_pressure(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -4488,56 +4035,67 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract hydrostatic pressure element nodal results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -4549,72 +4107,75 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def hydrostatic_pressure_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract hydrostatic pressure nodal results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -4626,69 +4187,72 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def hydrostatic_pressure_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract hydrostatic pressure elemental results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -4700,16 +4264,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def structural_temperature(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -4717,64 +4281,67 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract structural temperature element nodal results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -4786,72 +4353,75 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def structural_temperature_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract structural temperature nodal results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -4863,69 +4433,72 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def structural_temperature_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract structural temperature elemental results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of times to get results for.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -4937,16 +4510,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def element_nodal_forces(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -4956,69 +4529,72 @@
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         location: Union[locations, str] = locations.elemental_nodal,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract element nodal forces results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z",
-                and their respective equivalents 1, 2, 3.
-            norm:
-                Whether to return the norm of the results.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            location:
-                Location to extract results at. Available locations are listed in
-                class:`post.locations` and are: `post.locations.nodal`,
-                `post.locations.elemental`, and `post.locations.elemental_nodal`.
-                Using the default `post.locations.elemental_nodal` results in a value
-                for every node at each element. Similarly, using `post.locations.elemental`
-                gives results with one value for each element, while using `post.locations.nodal`
-                gives results with one value for each node.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -5031,16 +4607,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def element_nodal_forces_nodal(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -5049,61 +4625,64 @@
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract element nodal forces nodal results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z",
-                and their respective equivalents 1, 2, 3.
-            norm:
-                Whether to return the norm of the results.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -5116,16 +4695,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def element_nodal_forces_elemental(
         self,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
@@ -5133,59 +4712,62 @@
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract element nodal forces elemental results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, and `element_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            element_ids:
-                List of IDs of elements to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z",
-                and their respective equivalents 1, 2, 3.
-            norm:
-                Whether to return the norm of the results.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        element_ids:
+            List of IDs of elements to get results for.
+        times:
+            List of time values to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -5198,16 +4780,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=None,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def nodal_force(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -5216,61 +4798,64 @@
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal force results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements whose nodes to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z",
-                and their respective equivalents 1, 2, 3.
-            norm:
-                Whether to return the norm of the results.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        times:
+            List of time values to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -5283,16 +4868,16 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
 
     def nodal_moment(
         self,
         node_ids: Union[List[int], None] = None,
         element_ids: Union[List[int], None] = None,
         times: Union[float, List[float], None] = None,
@@ -5301,61 +4886,64 @@
         set_ids: Union[int, List[int], None] = None,
         all_sets: bool = False,
         load_steps: Union[
             int, List[int], Tuple[int, Union[int, List[int]]], None
         ] = None,
         named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
-        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
-        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
     ) -> DataFrame:
         """Extract nodal moment results from the simulation.
 
         Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
         exclusive.
         If none of the above is given, only the last result will be returned.
 
         Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
         exclusive.
         If none of the above is given, results will be extracted for the whole mesh.
 
-        Args:
-            node_ids:
-                List of IDs of nodes to get results for.
-            element_ids:
-                List of IDs of elements whose nodes to get results for.
-            times:
-                List of time values to get results for.
-            components:
-                Components to get results for. Available components are "X", "Y", "Z",
-                and their respective equivalents 1, 2, 3.
-            norm:
-                Whether to return the norm of the results.
-            set_ids:
-                Sets to get results for.
-                A set is defined as a unique combination of {time, load step, sub-step}.
-            all_sets:
-                Whether to get results for all sets.
-            load_steps:
-                Load step number or list of load step numbers to get results for.
-                One can specify sub-steps of a load step with a tuple of format:
-                (load-step, sub-step number or list of sub-step numbers).
-            named_selections:
-                Named selection or list of named selections to get results for.
-            selection:
-                Selection to get results for.
-                A Selection defines both spatial and time-like criteria for filtering.
-            expand_cyclic:
-                For cyclic problems, whether to expand the sectors.
-                Can take a list of sector numbers to select specific sectors to expand
-                (one-based indexing).
-                If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-                by stage.
-            phase_angle_cyclic:
-                 For cyclic problems, phase angle to apply (in degrees).
+        Parameters
+        ----------
+        node_ids:
+            List of IDs of nodes to get results for.
+        times:
+            List of time values to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        components:
+            Components to get results for. Available components are "X", "Y", "Z",
+            and their respective equivalents 1, 2, 3.
+        norm:
+            Whether to return the norm of the results.
+        set_ids:
+            Sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        named_selections:
+            Named selection or list of named selections to get results for.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
 
         Returns
         -------
             Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
 
         """
         return self._get_result(
@@ -5368,10 +4956,10 @@
             times=times,
             set_ids=set_ids,
             all_sets=all_sets,
             load_steps=load_steps,
             node_ids=node_ids,
             element_ids=element_ids,
             named_selections=named_selections,
-            expand_cyclic=expand_cyclic,
-            phase_angle_cyclic=phase_angle_cyclic,
+            external_layer=external_layer,
+            skin=skin,
         )
```

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/strain.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/strain.py`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/stress.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/stress.py`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/temperature.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/temperature.py`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/tensor.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/tensor.py`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/tools.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def select(
     time_freq_indexes=None,
     time_freq_sets=None,
     time_freq_values=None,
     named_selection_names=None,
-    **kwargs
+    **kwargs,
 ):
     """Creates a ``Selection`` instance allowing to choose the domain on which to evaluate results.
 
     The results domain defines the time frequency and the spatial selection.
 
     Parameters
     ----------
```

### Comparing `ansys-dpf-post-0.4.0/src/ansys/dpf/post/vector.py` & `ansys_dpf_post-0.5.0/src/ansys/dpf/post/vector.py`

 * *Files identical despite different names*

### Comparing `ansys-dpf-post-0.4.0/PKG-INFO` & `ansys_dpf_post-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,119 +1,128 @@
 Metadata-Version: 2.1
 Name: ansys-dpf-post
-Version: 0.4.0
+Version: 0.5.0
 Summary: PyDPF-Post Python library.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
-Requires-Python: >=3.7.*,<4.0
+Requires-Python: >=3.8,<4.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Dist: ansys-dpf-core
 Requires-Dist: scooby
 Requires-Dist: pyvista>=0.24.0 ; extra == "plotting"
-Project-URL: Source, https://github.com/pyansys/pydpf-post
+Project-URL: Source, https://github.com/ansys/pydpf-post
 Provides-Extra: plotting
 
-# PyDPF-Post - Ansys Data Post-Processing Framework
+# PyDPF-Post - Ansys Data PostProcessing Framework
 [![PyAnsys](https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC)](https://docs.pyansys.com/)
 [![Python](https://img.shields.io/pypi/pyversions/ansys-dpf-post?logo=pypi)](https://pypi.org/project/ansys-dpf-post/)
 [![pypi](https://badge.fury.io/py/ansys-dpf-post.svg?logo=python&logoColor=white)](https://pypi.org/project/ansys-dpf-post)
 [![MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-The Data Processing Framework (DPF) is designed to provide numerical
-simulation users/engineers with a toolbox for accessing and
+The Ansys Data Processing Framework (DPF) is designed to provide numerical
+simulation users and engineers with a toolbox for accessing and
 transforming simulation data.
 
-The Python `ansys-dpf-post` package provides a high level, physics oriented API for postprocessing.
+The Python `ansys-dpf-post` package provides a high-level, physics-oriented API for postprocessing.
 Loading a simulation (defined by its result files) allows you to extract simulation metadata as well
-as results and apply postprocessing operations on it.
+as results and then apply postprocessing operations on it.
 
-This module leverages the PyDPF-Core project's ``ansys-dpf-core`` package and can
-be found by visiting [PyDPF-Core
-GitHub](https://github.com/pyansys/pydpf-core).  Use ``ansys-dpf-core`` for
-building more advanced and customized workflows using Ansys DPF.
+The latest version of DPF supports Ansys solver result files for:
+
+  - MAPDL (`.rst`, `.mode`, `.rfrq`, `.rdsp`)
+  - LS-DYNA (`.d3plot`, `.binout`)
+  - Fluent (`.cas/dat.h5`, `.flprj`)
+  - CFX (`.cad/dat.cff`, `.flprj`)
+
+See the `PyDPF-Core main page <https://dpf.docs.pyansys.com/version/stable/index.html>`_
+for more information on compatibility.
+
+This module leverages the PyDPF-Core project's ``ansys-dpf-core`` package, which is
+available at [PyDPF-Core GitHub](https://github.com/ansys/pydpf-core).
+Use the ``ansys-dpf-core`` package for building more advanced and customized workflows
+using Ansys DPF.
 
 ## Documentation
 
-Visit the [PyDPF-Post Documentation](https://postdocs.pyansys.com) for a
-detailed description of the package, or see the [Examples
-Gallery](https://postdocs.pyansys.com/examples/index.html) for more
-detailed examples.
+For comprehensive information on this package, see the [PyDPF-Post Documentation](https://post.docs.pyansys.com),
+For detailed how-to information, see the [Examples](https://post.docs.pyansys.com/version/stable/examples/index.html)
+in the PyDPF-Post documentation.
 
 ## Installation
 
-Install this repository with:
+To install this package, use this command:
 
 ```
 pip install ansys-dpf-post
 ```
 
-You can also clone and install this repository with:
+You can also clone and install this package with this code:
 
 ```
-git clone https://github.com/pyansys/pydpf-post
+git clone https://github.com/ansys/pydpf-post
 cd pydpf-post
 pip install . --user
 ```
 
-## Brief Demo
+## Brief demo
 
-Provided you have ANSYS 2023 R1 installed, a DPF server starts
+Provided you have Ansys 2023 R1 or later installed, a DPF server starts
 automatically once you start using PyDPF-Post.
-Loading a simulation to extract and post-process results:
+
+To load a simulation to extract and post-process results, use this code:
 
 ```pycon
 >>> from ansys.dpf import post
 >>> from ansys.dpf.post import examples
 >>> simulation = post.load_simulation(examples.download_crankshaft())
 >>> displacement = simulation.displacement()
 >>> print(displacement)
 ```
 ```pycon
-             results         U
-              set_id         3
-      node      comp          
-      4872         X -3.41e-05
-                   Y  1.54e-03
-                   Z -2.64e-06
-      9005         X -5.56e-05
-                   Y  1.44e-03
-                   Z  5.31e-06
-       ...
+             results       U (m)
+             set_ids           3
+ node_ids components            
+     4872          X -3.4137e-05
+                   Y  1.5417e-03
+                   Z -2.6398e-06
+     9005          X -5.5625e-05
+                   Y  1.4448e-03
+                   Z  5.3134e-06
+      ...        ...         ...
 ```
 ```pycon
 >>> displacement.plot()
 ```
-![Example Displacement plot Crankshaft](https://github.com/pyansys/dpf-post/raw/master/docs/source/images/crankshaft_disp.png)
+![Example Displacement plot Crankshaft](https://github.com/ansys/pydpf-post/raw/master/docs/source/images/crankshaft_disp.png)
 ```pycon
 >>> stress_eqv = simulation.stress_eqv_von_mises_nodal()
 >>> stress_eqv.plot()
 ```
-![Example Stress plot Crankshaft](https://github.com/pyansys/dpf-post/raw/master/docs/source/images/crankshaft_stress.png)
+![Example Stress plot Crankshaft](https://github.com/ansys/pydpf-post/raw/master/docs/source/images/crankshaft_stress.png)
 
-To run PyDPF-Post with Ansys versions starting from 2021 R1 to 2022 R2, use the following legacy PyDPF-Post 
-tools:
+To run PyDPF-Post with Ansys versions 2021 R1 and 2022 R2, use this code to
+start the legacy PyDPF-Post tools::
 
 ```pycon
 >>> from ansys.dpf import post
 >>> from ansys.dpf.post import examples
 >>> solution = post.load_solution(examples.download_crankshaft())
 >>> stress = solution.stress()
 >>> stress.eqv.plot_contour(show_edges=False)
 ```
-![Example Stress plot Crankshaft](https://github.com/pyansys/dpf-post/raw/master/docs/source/images/crankshaft_stress.png)
+![Example Stress plot Crankshaft](https://github.com/ansys/pydpf-post/raw/master/docs/source/images/crankshaft_stress.png)
 
 ## License
 
-``PyDPF-Post`` is licensed under the MIT license.  For more information, see the
-[LICENSE](https://github.com/pyansys/dpf-post/raw/master/LICENSE).
+``PyDPF-Post`` is licensed under the MIT license. For more information, see the
+[LICENSE](https://github.com/ansys/pydpf-post/raw/master/LICENSE).
```

