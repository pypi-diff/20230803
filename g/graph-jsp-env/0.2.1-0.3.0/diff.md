# Comparing `tmp/graph-jsp-env-0.2.1.tar.gz` & `tmp/graph-jsp-env-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph-jsp-env-0.2.1.tar", last modified: Wed Jul  5 14:17:31 2023, max compression
+gzip compressed data, was "graph-jsp-env-0.3.0.tar", last modified: Thu Aug  3 11:13:57 2023, max compression
```

## Comparing `graph-jsp-env-0.2.1.tar` & `graph-jsp-env-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-07-05 14:17:31.002413 graph-jsp-env-0.2.1/
--rw-r--r--   0 qwerty     (501) staff       (20)     1072 2022-04-21 09:38:44.000000 graph-jsp-env-0.2.1/LICENSE
--rw-r--r--   0 qwerty     (501) staff       (20)       50 2022-12-07 18:44:16.000000 graph-jsp-env-0.2.1/MANIFEST.in
--rw-r--r--   0 qwerty     (501) staff       (20)    11113 2023-07-05 14:17:31.002492 graph-jsp-env-0.2.1/PKG-INFO
--rw-r--r--   0 qwerty     (501) staff       (20)     9205 2022-12-14 09:08:30.000000 graph-jsp-env-0.2.1/README.md
--rw-r--r--   0 qwerty     (501) staff       (20)     2107 2023-07-05 14:15:52.000000 graph-jsp-env-0.2.1/pyproject.toml
--rw-r--r--   0 qwerty     (501) staff       (20)      598 2023-07-05 14:17:31.002816 graph-jsp-env-0.2.1/setup.cfg
--rw-r--r--   0 qwerty     (501) staff       (20)       69 2022-12-07 19:01:51.000000 graph-jsp-env-0.2.1/setup.py
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-07-05 14:17:30.999926 graph-jsp-env-0.2.1/src/
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-07-05 14:17:31.001160 graph-jsp-env-0.2.1/src/graph_jsp_env/
--rw-r--r--   0 qwerty     (501) staff       (20)        0 2022-12-07 20:04:28.000000 graph-jsp-env-0.2.1/src/graph_jsp_env/__init__.py
--rw-r--r--   0 qwerty     (501) staff       (20)    46294 2023-07-05 14:08:54.000000 graph-jsp-env-0.2.1/src/graph_jsp_env/disjunctive_graph_jsp_env.py
--rw-r--r--   0 qwerty     (501) staff       (20)    20971 2022-12-08 10:42:07.000000 graph-jsp-env-0.2.1/src/graph_jsp_env/disjunctive_graph_jsp_visualizer.py
--rw-r--r--   0 qwerty     (501) staff       (20)      592 2022-12-08 13:18:55.000000 graph-jsp-env-0.2.1/src/graph_jsp_env/disjunctive_graph_logger.py
--rw-r--r--   0 qwerty     (501) staff       (20)     6535 2022-12-08 09:00:18.000000 graph-jsp-env-0.2.1/src/graph_jsp_env/wzl_ima_banner.py
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-07-05 14:17:31.001779 graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/
--rw-r--r--   0 qwerty     (501) staff       (20)    11113 2023-07-05 14:17:30.000000 graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/PKG-INFO
--rw-r--r--   0 qwerty     (501) staff       (20)      606 2023-07-05 14:17:30.000000 graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/SOURCES.txt
--rw-r--r--   0 qwerty     (501) staff       (20)        1 2023-07-05 14:17:30.000000 graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/dependency_links.txt
--rw-r--r--   0 qwerty     (501) staff       (20)        1 2022-12-07 20:26:06.000000 graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/not-zip-safe
--rw-r--r--   0 qwerty     (501) staff       (20)      232 2023-07-05 14:17:30.000000 graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/requires.txt
--rw-r--r--   0 qwerty     (501) staff       (20)       14 2023-07-05 14:17:30.000000 graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/top_level.txt
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-07-05 14:17:31.002089 graph-jsp-env-0.2.1/tests/
--rw-r--r--   0 qwerty     (501) staff       (20)      210 2022-12-08 09:05:55.000000 graph-jsp-env-0.2.1/tests/test_banner.py
--rw-r--r--   0 qwerty     (501) staff       (20)     3001 2022-12-14 16:45:39.000000 graph-jsp-env-0.2.1/tests/test_disjunctive_graph_jsp_env.py
--rw-r--r--   0 qwerty     (501) staff       (20)     1357 2022-12-08 12:32:13.000000 graph-jsp-env-0.2.1/tests/test_visualizer.py
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-08-03 11:13:57.570565 graph-jsp-env-0.3.0/
+-rw-r--r--   0 qwerty     (501) staff       (20)     1072 2022-04-21 09:38:44.000000 graph-jsp-env-0.3.0/LICENSE
+-rw-r--r--   0 qwerty     (501) staff       (20)       50 2022-12-07 18:44:16.000000 graph-jsp-env-0.3.0/MANIFEST.in
+-rw-r--r--   0 qwerty     (501) staff       (20)    11113 2023-08-03 11:13:57.570653 graph-jsp-env-0.3.0/PKG-INFO
+-rw-r--r--   0 qwerty     (501) staff       (20)     9205 2022-12-14 09:08:30.000000 graph-jsp-env-0.3.0/README.md
+-rw-r--r--   0 qwerty     (501) staff       (20)     2115 2023-08-03 10:17:19.000000 graph-jsp-env-0.3.0/pyproject.toml
+-rw-r--r--   0 qwerty     (501) staff       (20)      598 2023-08-03 11:13:57.571112 graph-jsp-env-0.3.0/setup.cfg
+-rw-r--r--   0 qwerty     (501) staff       (20)       69 2022-12-07 19:01:51.000000 graph-jsp-env-0.3.0/setup.py
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-08-03 11:13:57.567805 graph-jsp-env-0.3.0/src/
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-08-03 11:13:57.569279 graph-jsp-env-0.3.0/src/graph_jsp_env/
+-rw-r--r--   0 qwerty     (501) staff       (20)        0 2022-12-07 20:04:28.000000 graph-jsp-env-0.3.0/src/graph_jsp_env/__init__.py
+-rw-r--r--   0 qwerty     (501) staff       (20)    48131 2023-08-03 10:06:50.000000 graph-jsp-env-0.3.0/src/graph_jsp_env/disjunctive_graph_jsp_env.py
+-rw-r--r--   0 qwerty     (501) staff       (20)    21045 2023-08-03 09:44:55.000000 graph-jsp-env-0.3.0/src/graph_jsp_env/disjunctive_graph_jsp_visualizer.py
+-rw-r--r--   0 qwerty     (501) staff       (20)      592 2022-12-08 13:18:55.000000 graph-jsp-env-0.3.0/src/graph_jsp_env/disjunctive_graph_logger.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     6535 2022-12-08 09:00:18.000000 graph-jsp-env-0.3.0/src/graph_jsp_env/wzl_ima_banner.py
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-08-03 11:13:57.570099 graph-jsp-env-0.3.0/src/graph_jsp_env.egg-info/
+-rw-r--r--   0 qwerty     (501) staff       (20)    11113 2023-08-03 11:13:57.000000 graph-jsp-env-0.3.0/src/graph_jsp_env.egg-info/PKG-INFO
+-rw-r--r--   0 qwerty     (501) staff       (20)      606 2023-08-03 11:13:57.000000 graph-jsp-env-0.3.0/src/graph_jsp_env.egg-info/SOURCES.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)        1 2023-08-03 11:13:57.000000 graph-jsp-env-0.3.0/src/graph_jsp_env.egg-info/dependency_links.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)        1 2022-12-07 20:26:06.000000 graph-jsp-env-0.3.0/src/graph_jsp_env.egg-info/not-zip-safe
+-rw-r--r--   0 qwerty     (501) staff       (20)      238 2023-08-03 11:13:57.000000 graph-jsp-env-0.3.0/src/graph_jsp_env.egg-info/requires.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)       14 2023-08-03 11:13:57.000000 graph-jsp-env-0.3.0/src/graph_jsp_env.egg-info/top_level.txt
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-08-03 11:13:57.570473 graph-jsp-env-0.3.0/tests/
+-rw-r--r--   0 qwerty     (501) staff       (20)      210 2022-12-08 09:05:55.000000 graph-jsp-env-0.3.0/tests/test_banner.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     3972 2023-08-03 09:32:26.000000 graph-jsp-env-0.3.0/tests/test_disjunctive_graph_jsp_env.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     1357 2023-08-03 08:52:01.000000 graph-jsp-env-0.3.0/tests/test_visualizer.py
```

### Comparing `graph-jsp-env-0.2.1/LICENSE` & `graph-jsp-env-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graph-jsp-env-0.2.1/PKG-INFO` & `graph-jsp-env-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-jsp-env
-Version: 0.2.1
+Version: 0.3.0
 Summary: A flexible enviorment for job shop scheduling using the disjunctive graph apporach.
 Author: Alexander Nasuta
 Author-email: Alexander Nasuta <alexander.nasuta@ima.rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2022 Alexander Nasuta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: graph-jsp-env Version: 0.2.1 Summary: A flexible
+Metadata-Version: 2.1 Name: graph-jsp-env Version: 0.3.0 Summary: A flexible
 enviorment for job shop scheduling using the disjunctive graph apporach.
 Author: Alexander Nasuta Author-email: Alexander Nasuta
 nasuta@ima.rwth-aachen.de> License: MIT License Copyright (c) 2022 Alexander
 Nasuta Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
```

### Comparing `graph-jsp-env-0.2.1/README.md` & `graph-jsp-env-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `graph-jsp-env-0.2.1/pyproject.toml` & `graph-jsp-env-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=42.0", "wheel"]
+requires = ["setuptools>=65.5.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "graph-jsp-env"
-version = "0.2.1"
+version = "0.3.0"
 description = "A flexible enviorment for job shop scheduling using the disjunctive graph apporach."
 readme = "README.md"
 authors = [{ name = "Alexander Nasuta", email = "alexander.nasuta@ima.rwth-aachen.de" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -20,15 +20,15 @@
     "opencv-python",
     "plotly",
     "networkx>=3",
     "matplotlib",
     "numpy",
     "pandas",
     "kaleido",
-    "gym"
+    "gymnasium"
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
     "black",
     "bumpver",
```

### Comparing `graph-jsp-env-0.2.1/setup.cfg` & `graph-jsp-env-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `graph-jsp-env-0.2.1/src/graph_jsp_env/disjunctive_graph_jsp_env.py` & `graph-jsp-env-0.3.0/src/graph_jsp_env/disjunctive_graph_jsp_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-import gym
+import gymnasium as gym
 import numpy as np
+import numpy.typing as npt
 import networkx as nx
 import pandas as pd
 
 import matplotlib.pyplot as plt
 
 from collections import OrderedDict
 from typing import List, Union, Dict, Callable
 
 from graph_jsp_env.disjunctive_graph_jsp_visualizer import DisjunctiveGraphJspVisualizer
 from graph_jsp_env.disjunctive_graph_logger import log
 
+from typing import Any, SupportsFloat, Set
+
 
 class DisjunctiveGraphJspEnv(gym.Env):
     """
     Custom Environment for the Job Shop Problem (jsp) that follows gym interface.
 
     This environment is inspired by the
 
@@ -49,15 +52,15 @@
 
     The DisjunctiveGraphJssEnv uses the `networkx` library for graph structure and graph visualization.
     It is highly configurable and offers a lot of rendering options.
     """
     metadata = {'render.modes': ['human', 'rgb_array', 'console']}
 
     def __init__(self,
-                 jps_instance: np.ndarray = None, *,
+                 jps_instance: npt.NDArray = None, *,
                  # parameters for reward
                  reward_function='nasuta',
                  custom_reward_function: Callable = None,
                  reward_function_parameters: Dict = None,
                  # parameters for observation
                  normalize_observation_space: bool = True,
                  flat_observation_space: bool = True,
@@ -66,15 +69,15 @@
                  action_mode: str = "task",
                  env_transform: str = None,
                  perform_left_shift_if_possible: bool = True,
                  # parameters for rendering
                  c_map: str = "rainbow",
                  dummy_task_color="tab:gray",
                  default_visualisations: List[str] = None,
-                 visualizer_kwargs: dict = None,
+                 visualizer_kwargs: Dict = None,
                  verbose: int = 0
                  ):
         """
 
         :param jps_instance:                    a jsp instance as numpy array
 
         :param scaling_divisor:                 lower-bound of the jsp or some other scaling number for the reward.
@@ -152,15 +155,15 @@
         self.makespan_previous_step = None
 
         # reward function settings
         if reward_function not in ['nasuta', 'zhang', 'graph-tassel', 'samsonov', 'zero', 'custom']:
             raise ValueError(f"only 'nasuta', 'zhang', 'graph-tassel', 'samsonov', 'zero', 'custom' "
                              f"are valid arguments for 'reward_function'. {reward_function} is not.")
         if reward_function == 'custom' and custom_reward_function is None:
-            raise ValueError(f"if 'reward_function' is 'custom', 'custom_reward_function' must be specified.")
+            raise ValueError("if 'reward_function' is 'custom', 'custom_reward_function' must be specified.")
 
         self.reward_function = reward_function
         self.custom_reward_function = custom_reward_function
 
         # default reward function params
         if reward_function_parameters is None:
             if reward_function == 'nasuta':
@@ -214,18 +217,22 @@
         # values for dummy tasks nedded for the graph structure
         self.dummy_task_machine = -1
         self.dummy_task_job = -1
         self.dummy_task_color = dummy_task_color
 
         self.verbose = verbose
 
+        # save all taken actions into a list
+        # this might be useful for reconstruction the state of the environment after a reset
+        self.action_history = []
+
         if jps_instance is not None:
             self.load_instance(jsp_instance=jps_instance)
 
-    def load_instance(self, jsp_instance: np.ndarray, *, reward_function_parameters: Dict = None) -> None:
+    def load_instance(self, jsp_instance: npt.NDArray, *, reward_function_parameters: Dict = None) -> None:
         """
         This loads a jsp instance, sets up the corresponding graph and sets the attributes accordingly.
 
         :param jsp_instance:                a jsp instance as numpy array
         :param reward_function_parameters:  if specified, the reward functions params will be updated.
 
         :return:                            None
@@ -371,15 +378,15 @@
 
         if reward_function_parameters is not None:
             if self.verbose > 1:
                 log.info(f"updating reward_function_parameters from '{self.reward_function_parameters}' "
                          f"to '{reward_function_parameters}'")
             self.reward_function_parameters = reward_function_parameters
 
-    def step(self, action: int) -> (np.ndarray, float, bool, dict):
+    def step(self, action: int) -> tuple[npt.NDArray, SupportsFloat, bool, bool, Dict[str, Any]]:
         """
         perform an action on the environment. Not valid actions will have no effect.
 
         :param action: an action
         :return: state, reward, done-flag, info-dict
         """
         info = {
@@ -390,15 +397,15 @@
         if self.action_mode == 'task':
             task_id = action + 1
 
             if self.verbose > 1:
                 log.info(f"handling action={action} (Task {task_id})")
             info = {
                 **info,
-                **self._schedule_task(task_id=task_id)
+                **self._schedule_task(task_id=task_id, action=action)
             }
         else:  # case for self.action_mode == 'job'
             task_mask = self.valid_action_mask(action_mode='task')
             job_mask = np.array_split(task_mask, self.n_jobs)[action]
 
             if True not in job_mask:
                 if self.verbose > 0:
@@ -406,15 +413,15 @@
                 info["valid_action"] = False
             else:
                 task_id = 1 + action * self.n_machines + np.argmax(job_mask)
                 if self.verbose > 1:
                     log.info(f"handling job={action} (Task {task_id})")
                 info = {
                     **info,
-                    **self._schedule_task(task_id=task_id)
+                    **self._schedule_task(task_id=task_id, action=action)
                 }
 
         # check if done
         min_length = min([len(route) for m_id, route in self.machine_routes.items()])
         done = min_length == self.n_jobs
 
         makespan = nx.dag_longest_path_length(self.G)
@@ -428,25 +435,36 @@
             except nx.exception.NetworkXNoCycle:
                 pass
             info["makespan"] = makespan
             info["gantt_df"] = self.network_as_dataframe()
             if self.verbose > 0:
                 log.info(f"makespan: {makespan}")
 
-        state = self._state_array()
+        state = self.get_state()
         reward = self.get_reward(
             state=state,
             done=done,
             info=info,
             makespan_this_step=makespan
         )
         self.makespan_previous_step = makespan
-        return state, reward, done, info
+        truncated = False  # by construction always false. might by changed by a wrapper
+        return state, reward, done, truncated, info
+
+    def is_terminal(self) -> bool:
+        """
+        checks if the current state is terminal.
+        :return: bool flag. Flase -> not terminal, True -> terminal
+        """
+        # check if done
+        min_length = min([len(route) for m_id, route in self.machine_routes.items()])
+        done = min_length == self.n_jobs
+        return done
 
-    def get_reward(self, state: np.ndarray, done: bool, info: Dict, makespan_this_step: float):
+    def get_reward(self, state: npt.NDArray, done: bool, info: Dict, makespan_this_step: float):
         info['reward_function'] = self.reward_function
         reward_function_parameters = self.reward_function_parameters
 
         if self.reward_function == 'nasuta':
             if not done:
                 return 0.0
             else:
@@ -481,16 +499,16 @@
 
         elif self.reward_function == 'samsonov':
             if not done:
                 return 0.0
             else:
                 gamma = reward_function_parameters['gamma']
                 if reward_function_parameters['t_opt'] is None:
-                    raise ValueError(f"'t_opt' must be provided inside 'reward_function_parameters' for the samsonov "
-                                     f"reward function.")
+                    raise ValueError("'t_opt' must be provided inside 'reward_function_parameters' for the samsonov "
+                                     "reward function.")
                 t_opt = reward_function_parameters['t_opt']
                 return 1000 * gamma ** t_opt / gamma ** makespan_this_step
 
         elif self.reward_function == 'zero':
             return 0.0
 
         elif self.reward_function == 'custom':
@@ -500,37 +518,51 @@
                 info,  # info dict
                 self.G,  # networkX directed graph
                 makespan_this_step,  # longest path in G before the current timestep action
                 self.makespan_previous_step,  # longest path in G before the current timestep action
                 **reward_function_parameters  # custom reward function parameters
             )
 
-    def reset(self):
+    def reset(self, **kwargs) -> tuple[npt.NDArray, Dict[str, Any]]:
         """
         resets the environment and returns the initial state.
-
-        :return: initial state as numpy array.
+        :param **kwargs:   additional keyword arguments for the generic gymnasium reset method.
+        :return:
         """
+        # reset seed
+        super().reset(**kwargs)
+        #
+        info = {
+            "action_history": self.action_history
+        }
+        self.action_history = []  # rest action history
         # remove machine edges/routes
         machine_edges = [(from_, to_) for from_, to_, data_dict in self.G.edges(data=True) if not data_dict["job_edge"]]
         self.G.remove_edges_from(machine_edges)
 
         # reset machine routes dict
         self.machine_routes = {m_id: np.array([]) for m_id in range(self.n_machines)}
 
         # remove scheduled flags, reset start_time and finish_time
         for i in range(1, self.total_tasks_without_dummies + 1):
             node = self.G.nodes[i]
             node["scheduled"] = False
             node["start_time"] = None,
             node["finish_time"] = None
 
-        return self._state_array()
+        return self.get_state(), info  # obs, info
+
+    def get_action_history(self) -> List[int]:
+        """
+        returns the action history of the current episode.
+        :return: list of actions
+        """
+        return self.action_history
 
-    def render(self, mode="human", show: List[str] = None, **render_kwargs) -> Union[None, np.ndarray]:
+    def render(self, mode="human", show: List[str] = None, **render_kwargs) -> Union[None, npt.NDArray]:
         """
         renders the enviorment.
 
         :param mode:            valid options: "human", "rgb_array", "console"
 
                                 "human" (default)
 
@@ -594,15 +626,15 @@
 
         elif "gantt_window" in show:
             if mode == "human":
                 self.visualizer.render_gantt_in_window(df=df, colors=colors, **render_kwargs)
             elif mode == "rgb_array":
                 return self.visualizer.gantt_chart_rgb_array(df=df, colors=colors)
 
-    def _schedule_task(self, task_id: int) -> dict:
+    def _schedule_task(self, task_id: int, action: int) -> Dict[str, Any]:
         """
         schedules a task/node in the graph representation if the task can be scheduled.
 
         This adding one or multiple corresponding edges (multiple when performing a left shift) and updating the
         information stored in the nodes.
 
         :param task_id:     the task or node that shall be scheduled.
@@ -613,15 +645,15 @@
         if node["scheduled"]:
             if self.verbose > 0:
                 log.info(f"task {task_id} is already scheduled. ignoring it.")
             return {
                 "valid_action": False,
                 "node_id": task_id,
             }
-
+        self.action_history.append(action)
         m_id = node["machine"]
 
         prev_task_in_job_id, _ = list(self.G.in_edges(task_id))[0]
         prev_job_node = self.G.nodes[prev_task_in_job_id]
 
         if not prev_job_node["scheduled"]:
             if self.verbose > 1:
@@ -716,15 +748,15 @@
 
             else:
                 return self._append_at_the_end(task_id=task_id, node=node, prev_job_node=prev_job_node, m_id=m_id)
 
         else:
             return self._insert_at_index_0(task_id=task_id, node=node, prev_job_node=prev_job_node, m_id=m_id)
 
-    def _append_at_the_end(self, task_id: int, node: dict, prev_job_node: dict, m_id: int) -> dict:
+    def _append_at_the_end(self, task_id: int, node: Dict, prev_job_node: Dict, m_id: int) -> Dict[str, Any]:
         """
         inserts a task at the end (last element) in the `DisjunctiveGraphJssEnv.machine_routes`-dictionary.
 
         :param task_id:             the id oth the task with in graph representation.
         :param node:                the corresponding node in the graph (self.G).
         :param prev_job_node:       the node the is connected to :param node: via a job_edge (job_edge=True).
         :param m_id:                the id of the machine that corresponds to :param task_id:.
@@ -749,15 +781,15 @@
             "finish_time": ft,
             "node_id": task_id,
             "valid_action": True,
             "scheduling_method": '_append_at_the_end',
             "left_shift": 0,
         }
 
-    def _insert_at_index_0(self, task_id: int, node: dict, prev_job_node: dict, m_id: int) -> dict:
+    def _insert_at_index_0(self, task_id: int, node: Dict, prev_job_node: Dict, m_id: int) -> Dict:
         """
         inserts a task at index 0 (first element) in the `DisjunctiveGraphJssEnv.machine_routes`-dictionary.
 
         :param task_id:             the id oth the task with in graph representation.
         :param node:                the corresponding node in the graph (self.G).
         :param prev_job_node:       the node the is connected to :param node: via a job_edge (job_edge=True).
         :param m_id:                the id of the machine that corresponds to :param task_id:.
@@ -775,15 +807,15 @@
             "finish_time": ft,
             "node_id": task_id,
             "valid_action": True,
             "scheduling_method": '_insert_at_index_0',
             "left_shift": 0,
         }
 
-    def _state_array(self) -> np.ndarray:
+    def get_state(self) -> npt.NDArray:
         """
         returns the state of the environment as numpy array.
 
         :return: the state of the environment as numpy array.
         """
         adj = nx.to_numpy_array(self.G)[1:-1, 1:-1].astype(dtype=int)  # remove dummy tasks
         task_to_machine_mapping = np.zeros(shape=(self.total_tasks_without_dummies, 1), dtype=int)
@@ -934,15 +966,15 @@
             }
             for task_id, data in self.G.nodes(data=True)
             if data["job"] != -1 and data["finish_time"] is not None
         ])
 
     def valid_action_mask(self, action_mode: str = None) -> List[bool]:
         """
-        returs that indicates which action in the action space is valid (or will have an effect on the environment) and
+        returns that indicates which action in the action space is valid (or will have an effect on the environment) and
         which one is not.
 
         :param action_mode:     Specifies weather the `action`-argument of the `DisjunctiveGraphJssEnv.step`-method
                                 corresponds to a job or a task (or node in the graph representation)
 
         :return:                list of boolean in the same shape as the action-space.
         """
@@ -974,7 +1006,18 @@
             return mask
         elif action_mode == 'job':
             task_mask = self.valid_action_mask(action_mode='task')
             masks_per_job = np.array_split(task_mask, self.n_jobs)
             return [True in job_mask for job_mask in masks_per_job]
         else:
             raise ValueError(f"only 'task' and 'job' are valid arguments for 'action_mode'. {action_mode} is not.")
+
+    def valid_actions(self) -> Set[int]:
+        """
+        Returns the set of valid actions that can be taken in the current state of the environment.
+        The set contains the values one can pass to the step-function.
+        The values depend on the action_mode and the current state of the environment.
+        The set is empty if there are no valid actions.
+
+        :return: set of valid actions
+        """
+        return set(np.where(self.valid_action_mask())[0])
```

### Comparing `graph-jsp-env-0.2.1/src/graph_jsp_env/disjunctive_graph_jsp_visualizer.py` & `graph-jsp-env-0.3.0/src/graph_jsp_env/disjunctive_graph_jsp_visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 import signal
 import shutil
 import itertools
 
 import networkx as nx
 import matplotlib as mpl
 import numpy as np
+import numpy.typing as npt
 import pandas as pd
 
 import matplotlib.pyplot as plt
 import plotly.figure_factory as ff
 
-from typing import Union
+from typing import Union, Dict
 
 from graph_jsp_env.disjunctive_graph_logger import log
 
 
 def handler_stop_signals(*_) -> None:
     """
     closes all `cv2`-windows when the process is killed
@@ -47,16 +48,17 @@
 
         :param r:               red value.
         :param g:               green value
         :param b:               blue value
 
         :param format_type:     specifies weather the foreground-color or the background-color shall be adjusted.
                                 valid options: 'foreground','background'
-        :return:
+        :return:                a string that contains the color-codes.
         """
+        # type: ignore # noqa: F401
         if format_type == 'foreground':
             f = '\033[38;2;{};{};{}m'.format  # font rgb format
         elif format_type == 'background':
             f = '\033[48;2;{};{};{}m'.format  # font background rgb format
         else:
             raise ValueError(f"format {format_type} is not defined. Use 'foreground' or 'background'.")
         rgb = [r, g, b]
@@ -87,15 +89,15 @@
         :return:
         """
         return f"{DisjunctiveGraphJspVisualizer.rgb_color_sequence(r, g, b, **kwargs)}" \
                f"{s}" \
                f"{DisjunctiveGraphJspVisualizer.COLOR_ESCAPE_SEQUENCE}"
 
     @staticmethod
-    def gantt_chart_console(df: pd.DataFrame, colors: dict) -> None:
+    def gantt_chart_console(df: pd.DataFrame, colors: Dict) -> None:
         """
         console version of the `gantt_chart_rgb_array`-method. prints a gant chart to the console.
         the parameters need to follow the plotly specification.
         see: https://plotly.com/python/gantt/ or `gantt_chart_rgb_array`
 
         :param df:      dataframe according to `plotly` specification (https://plotly.com/python/gantt/).
 
@@ -161,17 +163,15 @@
         if len(df) > 0:
             for j, m in itertools.zip_longest(jobs, machines):
                 matching_tasks = df.loc[df['Task'] == j].iterrows()
                 chart_str = [i * x_interval_increment1 for i in range(x_pixels)]
                 for _, (_, start, finish, resource) in matching_tasks:
                     chart_str = [
                         f"{DisjunctiveGraphJspVisualizer.rgb_color_sequence(*colors[resource])}█"
-                        if not isinstance(v, str)
-                           and start <= v <= finish
-                        else v for v in chart_str
+                        if not isinstance(v, str) and start <= v <= finish else v for v in chart_str
                     ]
                 prefix = f"{f'{j}':<{len_prefix - 1}}║" if j else f"{'':<{len_prefix - 1}}║"
                 colored_block = DisjunctiveGraphJspVisualizer.wrap_with_color_codes("█", *colors[m]) if m else None
                 suffix = f"{f'║ {m}':<{len_suffix - 1}}" + f"{colored_block}" if m else f"{f'║':<{len_suffix}}"
 
                 chart_str = [" " if not isinstance(v, str) else v for v in chart_str]
                 chart_str = "".join(chart_str)
@@ -184,15 +184,15 @@
             *rows,
             x_axis,
             x_axis_label
         ])
         print(gant_str)
 
     @staticmethod
-    def render_rgb_array(vis: np.ndarray, *,
+    def render_rgb_array(vis: npt.NDArray, *,
                          window_title: str = "Job Shop Scheduling", wait: int = 1) -> None:
         """
         renders a rgb-array in an `cv2` window.
         the window will remain open for `:param wait:` ms or till the user presses any key.
 
         :param vis:             the rgb-array to render.
         :param window_title:    the title of the `cv2`-window
@@ -254,15 +254,15 @@
         :return:    a plot of the provided graph as rgb array.
         """
 
         plt.figure(dpi=self.dpi)
         plt.axis("off")
         plt.tight_layout()
 
-        pos: dict = nx.get_node_attributes(G, 'pos')  # node positions
+        pos: Dict = nx.get_node_attributes(G, 'pos')  # node positions
         fig = mpl.pyplot.gcf()
         fig.set_size_inches(self.width, self.height)
 
         # draw nodes
         for task, data in G.nodes(data=True):
             nx.draw_networkx_nodes(G, pos,
                                    nodelist=[task],
```

### Comparing `graph-jsp-env-0.2.1/src/graph_jsp_env/disjunctive_graph_logger.py` & `graph-jsp-env-0.3.0/src/graph_jsp_env/disjunctive_graph_logger.py`

 * *Files identical despite different names*

### Comparing `graph-jsp-env-0.2.1/src/graph_jsp_env/wzl_ima_banner.py` & `graph-jsp-env-0.3.0/src/graph_jsp_env/wzl_ima_banner.py`

 * *Files identical despite different names*

### Comparing `graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/PKG-INFO` & `graph-jsp-env-0.3.0/src/graph_jsp_env.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-jsp-env
-Version: 0.2.1
+Version: 0.3.0
 Summary: A flexible enviorment for job shop scheduling using the disjunctive graph apporach.
 Author: Alexander Nasuta
 Author-email: Alexander Nasuta <alexander.nasuta@ima.rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2022 Alexander Nasuta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: graph-jsp-env Version: 0.2.1 Summary: A flexible
+Metadata-Version: 2.1 Name: graph-jsp-env Version: 0.3.0 Summary: A flexible
 enviorment for job shop scheduling using the disjunctive graph apporach.
 Author: Alexander Nasuta Author-email: Alexander Nasuta
 nasuta@ima.rwth-aachen.de> License: MIT License Copyright (c) 2022 Alexander
 Nasuta Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
```

### Comparing `graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/SOURCES.txt` & `graph-jsp-env-0.3.0/src/graph_jsp_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graph-jsp-env-0.2.1/tests/test_visualizer.py` & `graph-jsp-env-0.3.0/tests/test_visualizer.py`

 * *Files identical despite different names*

