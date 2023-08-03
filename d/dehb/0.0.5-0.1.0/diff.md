# Comparing `tmp/dehb-0.0.5.tar.gz` & `tmp/dehb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dehb-0.0.5.tar", last modified: Sun Feb 19 22:49:24 2023, max compression
+gzip compressed data, was "dehb-0.1.0.tar", last modified: Thu Aug  3 15:53:38 2023, max compression
```

## Comparing `dehb-0.0.5.tar` & `dehb-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,15 @@
-drwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)        0 2023-02-19 22:49:24.948120 dehb-0.0.5/
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)    11355 2022-06-27 08:41:50.000000 dehb-0.0.5/LICENSE.txt
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)      327 2022-06-27 08:41:50.000000 dehb-0.0.5/MANIFEST.in
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)     7257 2023-02-19 22:49:24.905912 dehb-0.0.5/PKG-INFO
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)     6284 2022-08-17 12:34:11.000000 dehb-0.0.5/README.md
-drwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)        0 2023-02-19 22:49:24.737929 dehb-0.0.5/dehb/
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)      102 2022-08-17 12:34:11.000000 dehb-0.0.5/dehb/__init__.py
-drwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)        0 2023-02-19 22:49:24.876580 dehb-0.0.5/dehb/optimizers/
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)       61 2022-05-19 13:45:44.000000 dehb-0.0.5/dehb/optimizers/__init__.py
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)    35476 2023-02-19 22:47:57.000000 dehb-0.0.5/dehb/optimizers/de.py
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)    37448 2022-09-18 21:13:05.000000 dehb-0.0.5/dehb/optimizers/dehb.py
-drwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)        0 2023-02-19 22:49:24.901324 dehb-0.0.5/dehb/utils/
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)       45 2022-05-19 13:45:44.000000 dehb-0.0.5/dehb/utils/__init__.py
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)     6513 2022-05-19 13:45:44.000000 dehb-0.0.5/dehb/utils/bracket_manager.py
-drwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)        0 2023-02-19 22:49:24.830217 dehb-0.0.5/dehb.egg-info/
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)     7257 2023-02-19 22:49:24.000000 dehb-0.0.5/dehb.egg-info/PKG-INFO
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)      357 2023-02-19 22:49:24.000000 dehb-0.0.5/dehb.egg-info/SOURCES.txt
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)        1 2023-02-19 22:49:24.000000 dehb-0.0.5/dehb.egg-info/dependency_links.txt
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)      200 2023-02-19 22:49:24.000000 dehb-0.0.5/dehb.egg-info/requires.txt
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)        5 2023-02-19 22:49:24.000000 dehb-0.0.5/dehb.egg-info/top_level.txt
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)     2078 2022-06-27 08:41:50.000000 dehb-0.0.5/pyproject.toml
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)       80 2022-06-13 12:16:39.000000 dehb-0.0.5/requirements.txt
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)       38 2023-02-19 22:49:24.948873 dehb-0.0.5/setup.cfg
--rwxrwxrwx   0 neeratyoy  (1000) neeratyoy  (1000)     2266 2023-02-19 22:48:46.000000 dehb-0.0.5/setup.py
+drwxr-xr-x   0 fixja     (1000) fixja     (1000)        0 2023-08-03 15:53:38.301760 dehb-0.1.0/
+-rw-r--r--   0 fixja     (1000) fixja     (1000)    11355 2023-06-06 14:25:13.000000 dehb-0.1.0/LICENSE.txt
+-rw-r--r--   0 fixja     (1000) fixja     (1000)      327 2023-06-06 14:25:13.000000 dehb-0.1.0/MANIFEST.in
+-rw-r--r--   0 fixja     (1000) fixja     (1000)     8653 2023-08-03 15:53:38.301760 dehb-0.1.0/PKG-INFO
+-rw-r--r--   0 fixja     (1000) fixja     (1000)     7622 2023-08-03 15:50:48.000000 dehb-0.1.0/README.md
+drwxr-xr-x   0 fixja     (1000) fixja     (1000)        0 2023-08-03 15:53:38.299189 dehb-0.1.0/dehb.egg-info/
+-rw-r--r--   0 fixja     (1000) fixja     (1000)     8653 2023-08-03 15:53:37.000000 dehb-0.1.0/dehb.egg-info/PKG-INFO
+-rw-r--r--   0 fixja     (1000) fixja     (1000)      213 2023-08-03 15:53:37.000000 dehb-0.1.0/dehb.egg-info/SOURCES.txt
+-rw-r--r--   0 fixja     (1000) fixja     (1000)        1 2023-08-03 15:53:37.000000 dehb-0.1.0/dehb.egg-info/dependency_links.txt
+-rw-r--r--   0 fixja     (1000) fixja     (1000)      190 2023-08-03 15:53:37.000000 dehb-0.1.0/dehb.egg-info/requires.txt
+-rw-r--r--   0 fixja     (1000) fixja     (1000)        1 2023-08-03 15:53:37.000000 dehb-0.1.0/dehb.egg-info/top_level.txt
+-rw-r--r--   0 fixja     (1000) fixja     (1000)     4159 2023-08-03 15:50:48.000000 dehb-0.1.0/pyproject.toml
+-rw-r--r--   0 fixja     (1000) fixja     (1000)       80 2023-06-06 14:25:13.000000 dehb-0.1.0/requirements.txt
+-rw-r--r--   0 fixja     (1000) fixja     (1000)       38 2023-08-03 15:53:38.301760 dehb-0.1.0/setup.cfg
+-rw-r--r--   0 fixja     (1000) fixja     (1000)     2302 2023-08-03 15:50:48.000000 dehb-0.1.0/setup.py
```

### Comparing `dehb-0.0.5/LICENSE.txt` & `dehb-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dehb-0.0.5/PKG-INFO` & `dehb-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,14 @@
-Metadata-Version: 2.1
-Name: dehb
-Version: 0.0.5
-Summary: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization
-Home-page: https://github.com/automl/DEHB
-Author: Neeratyoy, Noor, Frank
-Author-email: mallik@cs.uni-freiburg.de
-License: Apache-2.0
-Project-URL: Documentation, https://automl.org.github.io/DEHB/main
-Project-URL: Source Code, https://github.com/automl.org/dehb
-Platform: Linux
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
 # DEHB: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization
-
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Tests](https://github.com/automl/DEHB/actions/workflows/pytest.yml/badge.svg)](https://github.com/automl/DEHB/actions/workflows/pytest.yml)
+[![docs](https://github.com/automl/DEHB/actions/workflows/docs.yml/badge.svg)](https://automl.github.io/DEHB/)
+[![Coverage Status](https://coveralls.io/repos/github/automl/DEHB/badge.svg)](https://coveralls.io/github/automl/DEHB)
+[![PyPI](https://img.shields.io/pypi/v/dehb)](https://pypi.org/project/dehb/)
+[![Static Badge](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue)](https://pypi.org/project/dehb/)
 ### Installation
 ```bash
 # from pypi
 pip install dehb
 
 # to run examples, install from github
 git clone https://github.com/automl/DEHB.git
@@ -37,40 +17,41 @@
 
 ### Tutorials/Example notebooks
 
 * [00 - A generic template to use DEHB for multi-fidelity Hyperparameter Optimization](examples/00_interfacing_DEHB.ipynb)
 * [01 - Using DEHB to optimize 4 hyperparameters of a Scikit-learn's Random Forest on a classification dataset](examples/01_Optimizing_RandomForest_using_DEHB.ipynb)
 * [02 - Optimizing Scikit-learn's Random Forest without using ConfigSpace to represent the hyperparameter space](examples/02_using%20DEHB_without_ConfigSpace.ipynb)
 * [03 - Hyperparameter Optimization for MNIST in PyTorch](examples/03_pytorch_mnist_hpo.py)
+* [04 - A generic template to use MODEHB for multi-objectives Hyperparameter Optimization](examples/04_mo_pytorch_mnist_hpo.py)
 
 To run PyTorch example: (*note additional requirements*) 
 ```bash
 python examples/03_pytorch_mnist_hpo.py \
      --min_budget 1 --max_budget 3 --verbose --runtime 60
 ```
 
 ### Running DEHB in a parallel setting
 
 DEHB has been designed to interface a [Dask client](https://distributed.dask.org/en/latest/api.html#distributed.Client).
-DEHB can either create a Dask client during instantiation and close/kill the client during garbage colleciton. 
+DEHB can either create a Dask client during instantiation and close/kill the client during garbage collection. 
 Or a client can be passed as an argument during instantiation.
 
 * Setting `n_workers` during instantiation \
     If set to `1` (default) then the entire process is a sequential run without invoking Dask. \
     If set to `>1` then a Dask Client is initialized with as many workers as `n_workers`. \
     This parameter is ignored if `client` is not None.
 * Setting `client` during instantiation \
-    When `None` (default), the a Dask client is created using `n_workers` specified. \
-    Else, any custom configured Dask Client can be created and passed as the `client` argument to DEHB.
+    When `None` (default), a Dask client is created using `n_workers` specified. \
+    Else, any custom-configured Dask Client can be created and passed as the `client` argument to DEHB.
   
 #### Using GPUs in a parallel run
 
-Certain target function evaluations (especially for Deep Learning) requires computations to be 
+Certain target function evaluations (especially for Deep Learning) require computations to be 
 carried out on GPUs. The GPU devices are often ordered by device ID and if not configured, all 
-spawned worker processes access these devices in the same order and can either run out of memory, or
+spawned worker processes access these devices in the same order and can either run out of memory or
 not exhibit parallelism.
 
 For `n_workers>1` and when running on a single node (or local), the `single_node_with_gpus` can be 
 passed to the `run()` call to DEHB. Setting it to `False` (default) has no effect on the default setup 
 of the machine. Setting it to `True` will reorder the GPU device IDs dynamically by setting the environment 
 variable `CUDA_VISIBLE_DEVICES` for each worker process executing a target function evaluation. The re-ordering 
 is done in a manner that the first priority device is the one with the least number of active jobs assigned 
@@ -83,34 +64,35 @@
 ```
 
 #### Multi-node runs
 
 Multi-node parallelism is often contingent on the cluster setup to be deployed on. Dask provides useful 
 frameworks to interface various cluster designs. As long as the `client` passed to DEHB during 
 instantiation is of type `dask.distributed.Client`, DEHB can interact with this client and 
-distribute its optimisation process in a parallel manner. 
+distribute its optimization process in a parallel manner. 
 
 For instance, `Dask-CLI` can be used to create a `dask-scheduler` which can dump its connection 
 details to a file on a cluster node accessible to all processes. Multiple `dask-worker` can then be
 created to interface the `dask-scheduler` by connecting to the details read from the file dumped. Each
 dask-worker can be triggered on any remote machine. Each worker can be configured as required, 
 including mapping to specific GPU devices. 
 
-Some helper scripts can be found [here](utils/), that can be used as reference to run DEHB in a multi-node 
+Some helper scripts can be found [here](utils/), that can be used as a reference to run DEHB in a multi-node 
 manner on clusters managed by SLURM. (*not expected to work off-the-shelf*)
 
 To run the PyTorch MNIST example on a multi-node setup using 4 workers:
 ```bash
 bash utils/run_dask_setup.sh -f dask_dump/scheduler.json -e env_name -n 4
 sleep 5
 python examples/03_pytorch_mnist_hpo.py --min_budget 1 --max_budget 3 \
   --verbose --runtime 60 --scheduler_file dask_dump/scheduler.json 
 ```
 
-
+### Running DEHB to optimize multiple objectives
+To run multi-objective optimization we require 1 extra parameter mo_strategy: we provide MO-optimization using Non-dominated sorted (NDS) with crowding distance (NSGA-II) and NDS with eps-net(EPSNET). Find 04_mo_pytorch_mnist_hpo.py example to help you to get started
 
 ### DEHB Hyperparameters
 
 *We recommend the default settings*.
 The default settings were chosen based on ablation studies over a collection of diverse problems 
 and were found to be *generally* useful across all cases tested. 
 However, the parameters are still available for tuning to a specific problem.
@@ -143,7 +125,14 @@
   pages     = {2147--2153},
   booktitle = {Proceedings of the Thirtieth International Joint Conference on
                Artificial Intelligence, {IJCAI-21}},
   publisher = {ijcai.org},
   editor    = {Z. Zhou},
   year      = {2021}
 }
+
+@online{Awad-arXiv-2023,
+title = {MO-DEHB: Evolutionary-based Hyperband for Multi-Objective Optimization},
+author = {Noor Awad and Ayushi Sharma and Frank Hutter},
+year = {2023},
+keywords = {}
+}
```

### Comparing `dehb-0.0.5/README.md` & `dehb-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,40 @@
-# DEHB: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization
+Metadata-Version: 2.1
+Name: dehb
+Version: 0.1.0
+Summary: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization
+Home-page: https://github.com/automl/DEHB
+Author: Neeratyoy, Noor, Janis, Frank
+Author-email: mallik@cs.uni-freiburg.de
+License: Apache-2.0
+Project-URL: Documentation, https://automl.org.github.io/DEHB/main
+Project-URL: Source Code, https://github.com/automl.org/dehb
+Platform: Linux
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.txt
 
+# DEHB: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Tests](https://github.com/automl/DEHB/actions/workflows/pytest.yml/badge.svg)](https://github.com/automl/DEHB/actions/workflows/pytest.yml)
+[![docs](https://github.com/automl/DEHB/actions/workflows/docs.yml/badge.svg)](https://automl.github.io/DEHB/)
+[![Coverage Status](https://coveralls.io/repos/github/automl/DEHB/badge.svg)](https://coveralls.io/github/automl/DEHB)
+[![PyPI](https://img.shields.io/pypi/v/dehb)](https://pypi.org/project/dehb/)
+[![Static Badge](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue)](https://pypi.org/project/dehb/)
 ### Installation
 ```bash
 # from pypi
 pip install dehb
 
 # to run examples, install from github
 git clone https://github.com/automl/DEHB.git
@@ -12,40 +43,41 @@
 
 ### Tutorials/Example notebooks
 
 * [00 - A generic template to use DEHB for multi-fidelity Hyperparameter Optimization](examples/00_interfacing_DEHB.ipynb)
 * [01 - Using DEHB to optimize 4 hyperparameters of a Scikit-learn's Random Forest on a classification dataset](examples/01_Optimizing_RandomForest_using_DEHB.ipynb)
 * [02 - Optimizing Scikit-learn's Random Forest without using ConfigSpace to represent the hyperparameter space](examples/02_using%20DEHB_without_ConfigSpace.ipynb)
 * [03 - Hyperparameter Optimization for MNIST in PyTorch](examples/03_pytorch_mnist_hpo.py)
+* [04 - A generic template to use MODEHB for multi-objectives Hyperparameter Optimization](examples/04_mo_pytorch_mnist_hpo.py)
 
 To run PyTorch example: (*note additional requirements*) 
 ```bash
 python examples/03_pytorch_mnist_hpo.py \
      --min_budget 1 --max_budget 3 --verbose --runtime 60
 ```
 
 ### Running DEHB in a parallel setting
 
 DEHB has been designed to interface a [Dask client](https://distributed.dask.org/en/latest/api.html#distributed.Client).
-DEHB can either create a Dask client during instantiation and close/kill the client during garbage colleciton. 
+DEHB can either create a Dask client during instantiation and close/kill the client during garbage collection. 
 Or a client can be passed as an argument during instantiation.
 
 * Setting `n_workers` during instantiation \
     If set to `1` (default) then the entire process is a sequential run without invoking Dask. \
     If set to `>1` then a Dask Client is initialized with as many workers as `n_workers`. \
     This parameter is ignored if `client` is not None.
 * Setting `client` during instantiation \
-    When `None` (default), the a Dask client is created using `n_workers` specified. \
-    Else, any custom configured Dask Client can be created and passed as the `client` argument to DEHB.
+    When `None` (default), a Dask client is created using `n_workers` specified. \
+    Else, any custom-configured Dask Client can be created and passed as the `client` argument to DEHB.
   
 #### Using GPUs in a parallel run
 
-Certain target function evaluations (especially for Deep Learning) requires computations to be 
+Certain target function evaluations (especially for Deep Learning) require computations to be 
 carried out on GPUs. The GPU devices are often ordered by device ID and if not configured, all 
-spawned worker processes access these devices in the same order and can either run out of memory, or
+spawned worker processes access these devices in the same order and can either run out of memory or
 not exhibit parallelism.
 
 For `n_workers>1` and when running on a single node (or local), the `single_node_with_gpus` can be 
 passed to the `run()` call to DEHB. Setting it to `False` (default) has no effect on the default setup 
 of the machine. Setting it to `True` will reorder the GPU device IDs dynamically by setting the environment 
 variable `CUDA_VISIBLE_DEVICES` for each worker process executing a target function evaluation. The re-ordering 
 is done in a manner that the first priority device is the one with the least number of active jobs assigned 
@@ -58,34 +90,35 @@
 ```
 
 #### Multi-node runs
 
 Multi-node parallelism is often contingent on the cluster setup to be deployed on. Dask provides useful 
 frameworks to interface various cluster designs. As long as the `client` passed to DEHB during 
 instantiation is of type `dask.distributed.Client`, DEHB can interact with this client and 
-distribute its optimisation process in a parallel manner. 
+distribute its optimization process in a parallel manner. 
 
 For instance, `Dask-CLI` can be used to create a `dask-scheduler` which can dump its connection 
 details to a file on a cluster node accessible to all processes. Multiple `dask-worker` can then be
 created to interface the `dask-scheduler` by connecting to the details read from the file dumped. Each
 dask-worker can be triggered on any remote machine. Each worker can be configured as required, 
 including mapping to specific GPU devices. 
 
-Some helper scripts can be found [here](utils/), that can be used as reference to run DEHB in a multi-node 
+Some helper scripts can be found [here](utils/), that can be used as a reference to run DEHB in a multi-node 
 manner on clusters managed by SLURM. (*not expected to work off-the-shelf*)
 
 To run the PyTorch MNIST example on a multi-node setup using 4 workers:
 ```bash
 bash utils/run_dask_setup.sh -f dask_dump/scheduler.json -e env_name -n 4
 sleep 5
 python examples/03_pytorch_mnist_hpo.py --min_budget 1 --max_budget 3 \
   --verbose --runtime 60 --scheduler_file dask_dump/scheduler.json 
 ```
 
-
+### Running DEHB to optimize multiple objectives
+To run multi-objective optimization we require 1 extra parameter mo_strategy: we provide MO-optimization using Non-dominated sorted (NDS) with crowding distance (NSGA-II) and NDS with eps-net(EPSNET). Find 04_mo_pytorch_mnist_hpo.py example to help you to get started
 
 ### DEHB Hyperparameters
 
 *We recommend the default settings*.
 The default settings were chosen based on ablation studies over a collection of diverse problems 
 and were found to be *generally* useful across all cases tested. 
 However, the parameters are still available for tuning to a specific problem.
@@ -118,7 +151,14 @@
   pages     = {2147--2153},
   booktitle = {Proceedings of the Thirtieth International Joint Conference on
                Artificial Intelligence, {IJCAI-21}},
   publisher = {ijcai.org},
   editor    = {Z. Zhou},
   year      = {2021}
 }
+
+@online{Awad-arXiv-2023,
+title = {MO-DEHB: Evolutionary-based Hyperband for Multi-Objective Optimization},
+author = {Noor Awad and Ayushi Sharma and Frank Hutter},
+year = {2023},
+keywords = {}
+}
```

### Comparing `dehb-0.0.5/dehb.egg-info/PKG-INFO` & `dehb-0.1.0/dehb.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 Metadata-Version: 2.1
 Name: dehb
-Version: 0.0.5
+Version: 0.1.0
 Summary: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization
 Home-page: https://github.com/automl/DEHB
-Author: Neeratyoy, Noor, Frank
+Author: Neeratyoy, Noor, Janis, Frank
 Author-email: mallik@cs.uni-freiburg.de
 License: Apache-2.0
 Project-URL: Documentation, https://automl.org.github.io/DEHB/main
 Project-URL: Source Code, https://github.com/automl.org/dehb
 Platform: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # DEHB: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization
-
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Tests](https://github.com/automl/DEHB/actions/workflows/pytest.yml/badge.svg)](https://github.com/automl/DEHB/actions/workflows/pytest.yml)
+[![docs](https://github.com/automl/DEHB/actions/workflows/docs.yml/badge.svg)](https://automl.github.io/DEHB/)
+[![Coverage Status](https://coveralls.io/repos/github/automl/DEHB/badge.svg)](https://coveralls.io/github/automl/DEHB)
+[![PyPI](https://img.shields.io/pypi/v/dehb)](https://pypi.org/project/dehb/)
+[![Static Badge](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue)](https://pypi.org/project/dehb/)
 ### Installation
 ```bash
 # from pypi
 pip install dehb
 
 # to run examples, install from github
 git clone https://github.com/automl/DEHB.git
@@ -37,40 +43,41 @@
 
 ### Tutorials/Example notebooks
 
 * [00 - A generic template to use DEHB for multi-fidelity Hyperparameter Optimization](examples/00_interfacing_DEHB.ipynb)
 * [01 - Using DEHB to optimize 4 hyperparameters of a Scikit-learn's Random Forest on a classification dataset](examples/01_Optimizing_RandomForest_using_DEHB.ipynb)
 * [02 - Optimizing Scikit-learn's Random Forest without using ConfigSpace to represent the hyperparameter space](examples/02_using%20DEHB_without_ConfigSpace.ipynb)
 * [03 - Hyperparameter Optimization for MNIST in PyTorch](examples/03_pytorch_mnist_hpo.py)
+* [04 - A generic template to use MODEHB for multi-objectives Hyperparameter Optimization](examples/04_mo_pytorch_mnist_hpo.py)
 
 To run PyTorch example: (*note additional requirements*) 
 ```bash
 python examples/03_pytorch_mnist_hpo.py \
      --min_budget 1 --max_budget 3 --verbose --runtime 60
 ```
 
 ### Running DEHB in a parallel setting
 
 DEHB has been designed to interface a [Dask client](https://distributed.dask.org/en/latest/api.html#distributed.Client).
-DEHB can either create a Dask client during instantiation and close/kill the client during garbage colleciton. 
+DEHB can either create a Dask client during instantiation and close/kill the client during garbage collection. 
 Or a client can be passed as an argument during instantiation.
 
 * Setting `n_workers` during instantiation \
     If set to `1` (default) then the entire process is a sequential run without invoking Dask. \
     If set to `>1` then a Dask Client is initialized with as many workers as `n_workers`. \
     This parameter is ignored if `client` is not None.
 * Setting `client` during instantiation \
-    When `None` (default), the a Dask client is created using `n_workers` specified. \
-    Else, any custom configured Dask Client can be created and passed as the `client` argument to DEHB.
+    When `None` (default), a Dask client is created using `n_workers` specified. \
+    Else, any custom-configured Dask Client can be created and passed as the `client` argument to DEHB.
   
 #### Using GPUs in a parallel run
 
-Certain target function evaluations (especially for Deep Learning) requires computations to be 
+Certain target function evaluations (especially for Deep Learning) require computations to be 
 carried out on GPUs. The GPU devices are often ordered by device ID and if not configured, all 
-spawned worker processes access these devices in the same order and can either run out of memory, or
+spawned worker processes access these devices in the same order and can either run out of memory or
 not exhibit parallelism.
 
 For `n_workers>1` and when running on a single node (or local), the `single_node_with_gpus` can be 
 passed to the `run()` call to DEHB. Setting it to `False` (default) has no effect on the default setup 
 of the machine. Setting it to `True` will reorder the GPU device IDs dynamically by setting the environment 
 variable `CUDA_VISIBLE_DEVICES` for each worker process executing a target function evaluation. The re-ordering 
 is done in a manner that the first priority device is the one with the least number of active jobs assigned 
@@ -83,34 +90,35 @@
 ```
 
 #### Multi-node runs
 
 Multi-node parallelism is often contingent on the cluster setup to be deployed on. Dask provides useful 
 frameworks to interface various cluster designs. As long as the `client` passed to DEHB during 
 instantiation is of type `dask.distributed.Client`, DEHB can interact with this client and 
-distribute its optimisation process in a parallel manner. 
+distribute its optimization process in a parallel manner. 
 
 For instance, `Dask-CLI` can be used to create a `dask-scheduler` which can dump its connection 
 details to a file on a cluster node accessible to all processes. Multiple `dask-worker` can then be
 created to interface the `dask-scheduler` by connecting to the details read from the file dumped. Each
 dask-worker can be triggered on any remote machine. Each worker can be configured as required, 
 including mapping to specific GPU devices. 
 
-Some helper scripts can be found [here](utils/), that can be used as reference to run DEHB in a multi-node 
+Some helper scripts can be found [here](utils/), that can be used as a reference to run DEHB in a multi-node 
 manner on clusters managed by SLURM. (*not expected to work off-the-shelf*)
 
 To run the PyTorch MNIST example on a multi-node setup using 4 workers:
 ```bash
 bash utils/run_dask_setup.sh -f dask_dump/scheduler.json -e env_name -n 4
 sleep 5
 python examples/03_pytorch_mnist_hpo.py --min_budget 1 --max_budget 3 \
   --verbose --runtime 60 --scheduler_file dask_dump/scheduler.json 
 ```
 
-
+### Running DEHB to optimize multiple objectives
+To run multi-objective optimization we require 1 extra parameter mo_strategy: we provide MO-optimization using Non-dominated sorted (NDS) with crowding distance (NSGA-II) and NDS with eps-net(EPSNET). Find 04_mo_pytorch_mnist_hpo.py example to help you to get started
 
 ### DEHB Hyperparameters
 
 *We recommend the default settings*.
 The default settings were chosen based on ablation studies over a collection of diverse problems 
 and were found to be *generally* useful across all cases tested. 
 However, the parameters are still available for tuning to a specific problem.
@@ -143,7 +151,14 @@
   pages     = {2147--2153},
   booktitle = {Proceedings of the Thirtieth International Joint Conference on
                Artificial Intelligence, {IJCAI-21}},
   publisher = {ijcai.org},
   editor    = {Z. Zhou},
   year      = {2021}
 }
+
+@online{Awad-arXiv-2023,
+title = {MO-DEHB: Evolutionary-based Hyperband for Multi-Objective Optimization},
+author = {Noor Awad and Ayushi Sharma and Frank Hutter},
+year = {2023},
+keywords = {}
+}
```

### Comparing `dehb-0.0.5/setup.py` & `dehb-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import setuptools
 
 import datetime
 
 
 name = "DEHB"
 package_name = "dehb"
-author = "Neeratyoy, Noor, Frank"
+author = "Neeratyoy, Noor, Janis, Frank"
 author_email = "mallik@cs.uni-freiburg.de"
 description = "Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization"
 url = "https://github.com/automl/DEHB"
 project_urls = {
     "Documentation": "https://automl.org.github.io/DEHB/main",
     "Source Code": "https://github.com/automl.org/dehb",
 }
 copyright = f"Copyright {datetime.date.today().strftime('%Y')}, Neeratyoy, Noor, Frank"
-version = "0.0.5"
+version = "0.1.0"
 
 HERE = os.path.dirname(os.path.realpath(__file__))
 
 
 def read_file(filepath: str) -> str:
     """
     Read in a files contents
@@ -44,20 +44,19 @@
     "dev": [
         # Test
         "pytest>=4.6",
         "pytest-cov",
         "pytest-xdist",
         "pytest-timeout",
         # Docs
-        "automl_sphinx_theme",
+        "mkdocs-material",
+        "mkdocstrings",
         # Others
-        "isort",
+        "ruff",
         "black",
-        "pydocstyle",
-        "flake8",
         "pre-commit",
     ]
 }
 
 setuptools.setup(
     name=package_name,
     author=author,
@@ -75,14 +74,15 @@
     extras_require=extras_require,
     test_suite="pytest",
     platforms=["Linux"],
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Natural Language :: English",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
```

