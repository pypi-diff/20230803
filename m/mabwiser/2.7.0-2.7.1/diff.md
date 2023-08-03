# Comparing `tmp/mabwiser-2.7.0.tar.gz` & `tmp/mabwiser-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mabwiser-2.7.0.tar", last modified: Wed Feb  8 14:37:16 2023, max compression
+gzip compressed data, was "mabwiser-2.7.1.tar", last modified: Thu Aug  3 01:06:41 2023, max compression
```

## Comparing `mabwiser-2.7.0.tar` & `mabwiser-2.7.1.tar`

### file list

```diff
@@ -1,30 +1,52 @@
-drwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2023-02-08 14:37:16.755000 mabwiser-2.7.0/
--rw-r--r--   0 a640920  (1141242692) staff       (20)    11356 2021-03-03 02:14:01.000000 mabwiser-2.7.0/LICENSE
--rw-r--r--   0 a640920  (1141242692) staff       (20)     6319 2023-02-08 14:37:16.754412 mabwiser-2.7.0/PKG-INFO
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)     5747 2022-11-23 14:31:52.000000 mabwiser-2.7.0/README.md
-drwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2023-02-08 14:37:16.745722 mabwiser-2.7.0/mabwiser/
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2021-03-03 02:14:01.000000 mabwiser-2.7.0/mabwiser/__init__.py
--rw-r--r--   0 a640920  (1141242692) staff       (20)      208 2023-02-08 14:36:49.000000 mabwiser-2.7.0/mabwiser/_version.py
--rw-r--r--   0 a640920  (1141242692) staff       (20)     6203 2022-03-01 18:26:24.000000 mabwiser-2.7.0/mabwiser/approximate.py
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)    17290 2023-02-01 16:43:19.000000 mabwiser-2.7.0/mabwiser/base_mab.py
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)     5985 2023-02-01 16:43:19.000000 mabwiser-2.7.0/mabwiser/clusters.py
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)     4359 2023-02-01 16:43:19.000000 mabwiser-2.7.0/mabwiser/greedy.py
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)     9648 2023-02-08 14:36:49.000000 mabwiser-2.7.0/mabwiser/linear.py
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)    71036 2023-02-01 16:43:19.000000 mabwiser-2.7.0/mabwiser/mab.py
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)     8417 2023-02-01 16:43:19.000000 mabwiser-2.7.0/mabwiser/neighbors.py
--rw-r--r--   0 a640920  (1141242692) staff       (20)     3076 2022-03-18 16:47:18.000000 mabwiser-2.7.0/mabwiser/popularity.py
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)     2464 2022-03-18 16:47:18.000000 mabwiser-2.7.0/mabwiser/rand.py
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)    69093 2021-03-03 02:14:01.000000 mabwiser-2.7.0/mabwiser/simulator.py
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)     5460 2023-02-01 16:43:19.000000 mabwiser-2.7.0/mabwiser/softmax.py
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)     5292 2023-02-01 16:43:19.000000 mabwiser-2.7.0/mabwiser/thompson.py
--rw-r--r--   0 a640920  (1141242692) staff       (20)     8290 2023-02-01 16:43:19.000000 mabwiser-2.7.0/mabwiser/treebandit.py
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)     4590 2023-02-01 16:43:19.000000 mabwiser-2.7.0/mabwiser/ucb.py
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)     9919 2022-03-28 14:43:49.000000 mabwiser-2.7.0/mabwiser/utils.py
-drwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2023-02-08 14:37:16.753658 mabwiser-2.7.0/mabwiser.egg-info/
--rw-r--r--   0 a640920  (1141242692) staff       (20)     6319 2023-02-08 14:37:16.000000 mabwiser-2.7.0/mabwiser.egg-info/PKG-INFO
--rw-r--r--   0 a640920  (1141242692) staff       (20)      529 2023-02-08 14:37:16.000000 mabwiser-2.7.0/mabwiser.egg-info/SOURCES.txt
--rw-r--r--   0 a640920  (1141242692) staff       (20)        1 2023-02-08 14:37:16.000000 mabwiser-2.7.0/mabwiser.egg-info/dependency_links.txt
--rw-r--r--   0 a640920  (1141242692) staff       (20)       70 2023-02-08 14:37:16.000000 mabwiser-2.7.0/mabwiser.egg-info/requires.txt
--rw-r--r--   0 a640920  (1141242692) staff       (20)        9 2023-02-08 14:37:16.000000 mabwiser-2.7.0/mabwiser.egg-info/top_level.txt
--rw-r--r--   0 a640920  (1141242692) staff       (20)       38 2023-02-08 14:37:16.755145 mabwiser-2.7.0/setup.cfg
--rwxr-xr-x   0 a640920  (1141242692) staff       (20)     1016 2021-03-03 02:14:01.000000 mabwiser-2.7.0/setup.py
+drwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2023-08-03 01:06:41.284093 mabwiser-2.7.1/
+-rw-r--r--   0 a640920  (1141242692) staff       (20)    11356 2021-03-03 02:14:01.000000 mabwiser-2.7.1/LICENSE
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     7784 2023-08-03 01:06:41.283200 mabwiser-2.7.1/PKG-INFO
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)     6278 2023-08-02 16:12:34.000000 mabwiser-2.7.1/README.md
+drwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2023-08-03 01:06:41.225376 mabwiser-2.7.1/mabwiser/
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2021-03-03 02:14:01.000000 mabwiser-2.7.1/mabwiser/__init__.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)      208 2023-08-03 01:03:18.000000 mabwiser-2.7.1/mabwiser/_version.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     6203 2022-03-01 18:26:24.000000 mabwiser-2.7.1/mabwiser/approximate.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    17290 2023-02-01 16:43:19.000000 mabwiser-2.7.1/mabwiser/base_mab.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)     5985 2023-02-01 16:43:19.000000 mabwiser-2.7.1/mabwiser/clusters.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)     4359 2023-02-01 16:43:19.000000 mabwiser-2.7.1/mabwiser/greedy.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)     9648 2023-02-08 14:36:49.000000 mabwiser-2.7.1/mabwiser/linear.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    71599 2023-08-03 01:03:18.000000 mabwiser-2.7.1/mabwiser/mab.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)     8417 2023-02-01 16:43:19.000000 mabwiser-2.7.1/mabwiser/neighbors.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     3076 2022-03-18 16:47:18.000000 mabwiser-2.7.1/mabwiser/popularity.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)     2464 2022-03-18 16:47:18.000000 mabwiser-2.7.1/mabwiser/rand.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    69093 2021-03-03 02:14:01.000000 mabwiser-2.7.1/mabwiser/simulator.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)     5460 2023-02-01 16:43:19.000000 mabwiser-2.7.1/mabwiser/softmax.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)     5292 2023-02-01 16:43:19.000000 mabwiser-2.7.1/mabwiser/thompson.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     8290 2023-02-01 16:43:19.000000 mabwiser-2.7.1/mabwiser/treebandit.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)     4590 2023-02-01 16:43:19.000000 mabwiser-2.7.1/mabwiser/ucb.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)     9919 2023-08-03 01:03:15.000000 mabwiser-2.7.1/mabwiser/utils.py
+drwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2023-08-03 01:06:41.230892 mabwiser-2.7.1/mabwiser.egg-info/
+-rw-r--r--   0 a640920  (1141242692) staff       (20)     7784 2023-08-03 01:06:40.000000 mabwiser-2.7.1/mabwiser.egg-info/PKG-INFO
+-rw-r--r--   0 a640920  (1141242692) staff       (20)      989 2023-08-03 01:06:40.000000 mabwiser-2.7.1/mabwiser.egg-info/SOURCES.txt
+-rw-r--r--   0 a640920  (1141242692) staff       (20)        1 2023-08-03 01:06:40.000000 mabwiser-2.7.1/mabwiser.egg-info/dependency_links.txt
+-rw-r--r--   0 a640920  (1141242692) staff       (20)       70 2023-08-03 01:06:40.000000 mabwiser-2.7.1/mabwiser.egg-info/requires.txt
+-rw-r--r--   0 a640920  (1141242692) staff       (20)        9 2023-08-03 01:06:40.000000 mabwiser-2.7.1/mabwiser.egg-info/top_level.txt
+-rw-r--r--   0 a640920  (1141242692) staff       (20)       38 2023-08-03 01:06:41.284548 mabwiser-2.7.1/setup.cfg
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)     1009 2023-08-03 01:06:14.000000 mabwiser-2.7.1/setup.py
+drwxr-xr-x   0 a640920  (1141242692) staff       (20)        0 2023-08-03 01:06:41.281340 mabwiser-2.7.1/tests/
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)     5830 2023-08-03 01:03:18.000000 mabwiser-2.7.1/tests/test_base.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    22608 2023-08-02 16:12:34.000000 mabwiser-2.7.1/tests/test_clusters.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    29980 2022-03-08 18:18:24.000000 mabwiser-2.7.1/tests/test_examples.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    18949 2023-01-26 21:36:46.000000 mabwiser-2.7.1/tests/test_greedy.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    39265 2023-08-01 14:29:34.000000 mabwiser-2.7.1/tests/test_invalid.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)    51717 2023-02-08 14:36:49.000000 mabwiser-2.7.1/tests/test_lingreedy.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)    33764 2023-02-08 14:36:49.000000 mabwiser-2.7.1/tests/test_lints.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    37839 2023-02-08 14:36:49.000000 mabwiser-2.7.1/tests/test_linucb.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)    33618 2023-02-01 16:43:19.000000 mabwiser-2.7.1/tests/test_lshnearest.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    93994 2023-02-01 16:43:19.000000 mabwiser-2.7.1/tests/test_mab.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    20571 2023-02-01 16:43:19.000000 mabwiser-2.7.1/tests/test_nearest.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    60360 2023-08-02 16:12:34.000000 mabwiser-2.7.1/tests/test_parallel.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)    16056 2023-01-26 21:36:46.000000 mabwiser-2.7.1/tests/test_popularity.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    27824 2023-02-01 16:43:19.000000 mabwiser-2.7.1/tests/test_radius.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)     5093 2022-03-18 16:47:18.000000 mabwiser-2.7.1/tests/test_random.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    31906 2023-02-08 14:36:49.000000 mabwiser-2.7.1/tests/test_ridge.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    62961 2022-03-28 14:44:10.000000 mabwiser-2.7.1/tests/test_simulator.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    18449 2023-01-26 21:36:46.000000 mabwiser-2.7.1/tests/test_softmax.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    22712 2023-01-26 21:36:46.000000 mabwiser-2.7.1/tests/test_thompson.py
+-rw-r--r--   0 a640920  (1141242692) staff       (20)    21840 2023-02-01 16:43:19.000000 mabwiser-2.7.1/tests/test_treebandit.py
+-rwxr-xr-x   0 a640920  (1141242692) staff       (20)    18329 2023-01-26 21:36:46.000000 mabwiser-2.7.1/tests/test_ucb.py
```

### Comparing `mabwiser-2.7.0/LICENSE` & `mabwiser-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/PKG-INFO` & `mabwiser-2.7.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,23 @@
-Metadata-Version: 2.1
-Name: mabwiser
-Version: 2.7.0
-Summary: MABWiser: Parallelizable Contextual Multi-Armed Bandits Library
-Home-page: https://github.com/fidelity/mabwiser
-Author: FMR LLC
-License: UNKNOWN
-Project-URL: Documentation, https://fidelity.github.io/mabwiser/
-Project-URL: Source, https://github.com/fidelity/mabwiser
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![ci](https://github.com/fidelity/mabwiser/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/fidelity/mabwiser/actions/workflows/ci.yml) [![PyPI version fury.io](https://badge.fury.io/py/mabwiser.svg)](https://pypi.python.org/pypi/mabwiser/) [![PyPI license](https://img.shields.io/pypi/l/mabwiser.svg)](https://pypi.python.org/pypi/mabwiser/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![Downloads](https://static.pepy.tech/personalized-badge/mabwiser?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/mabwiser)
 
 # MABWiser: Parallelizable Contextual Multi-Armed Bandits 
 
 MABWiser ([IJAIT 2021](https://www.worldscientific.com/doi/10.1142/S0218213021500214), [ICTAI 2019](https://ieeexplore.ieee.org/document/8995418)) is a research library written in Python for rapid prototyping of multi-armed bandit algorithms. It supports **context-free**, **parametric** and **non-parametric** **contextual** bandit models and provides built-in parallelization for both training and testing components. 
 
 The library also provides a simulation utility for comparing different policies and performing hyper-parameter tuning. MABWiser follows a scikit-learn style public interface, adheres to [PEP-8 standards](https://www.python.org/dev/peps/pep-0008/), and is tested heavily. 
 
-For Bandit-based Recommenders, see also our [Mab2Rec library](https://github.com/fidelity/mab2rec) built on top of MABWiser. 
-
 MABWiser is developed by the Artificial Intelligence Center of Excellence at Fidelity Investments. Documentation is available at [fidelity.github.io/mabwiser](https://fidelity.github.io/mabwiser).
 
+## Bandit-based Recommender Systems
+To solve personalized recommendation problems, MABWiser is integrated into our [Mab2Rec library](https://github.com/fidelity/mab2rec). Mab2Rec enables building content- and context-aware recommender systems, whereby MABWiser helps selecting the next best item (arm).
+
+## Bandit-based Large-Neighborhood Search
+To solve combinatorial optimization problems, MABWiser is integrated into [Adaptive Large Neighborhood Search](https://github.com/N-Wouda/ALNS). The ALNS library enables building metaheuristics for complex optimization problems, whereby MABWiser helps selecting the next best destroy, repair operation (arm).  
+
 ## Quick Start
 
 ```python
 # An example that shows how to use the UCB1 learning policy
 # to choose between two arms based on their expected rewards.
 
 # Import MABWiser Library
@@ -68,15 +56,15 @@
 * K-Nearest [7, 8]
 * LSH Nearest [9]
 * Radius [7, 8]
 * TreeBandit [10]
 
 ## Installation
 
-MABWiser requires **Python 3.6+** and can be installed from PyPI using ``pip install mabwiser`` or by building from source as shown in [installation instructions](https://fidelity.github.io/mabwiser/installation.html).
+MABWiser requires **Python 3.8+** and can be installed from PyPI using ``pip install mabwiser`` or by building from source as shown in [installation instructions](https://fidelity.github.io/mabwiser/installation.html).
 
 ## Support
 
 Please submit bug reports and feature requests as [Issues](https://github.com/fidelity/mabwiser/issues).
 
 ## Citation
 
@@ -125,9 +113,7 @@
 7. Melody Y. Guan and Heinrich Jiang, Nonparametric stochastic contextual bandits
 8. Philippe Rigollet and Assaf Zeevi. Nonparametric bandits with covariates 
 9. Indyk, Piotr, Motwani, Rajeev, Raghavan, Prabhakar, Vempala, Santosh. Locality-preserving hashing in multidimensional spaces
 10. Adam N. Elmachtoub, Ryan McNellis, Sechan Oh, Marek Petrik, A practical method for solving contextual bandit problems using decision trees
 11. Doruk Kilitcioglu, Serdar Kadioglu, Non-deterministic behavior of thompson sampling with linear payoffs and how to avoid it
 
 <br>
-
-
```

### Comparing `mabwiser-2.7.0/README.md` & `mabwiser-2.7.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,115 +1,134 @@
-[![ci](https://github.com/fidelity/mabwiser/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/fidelity/mabwiser/actions/workflows/ci.yml) [![PyPI version fury.io](https://badge.fury.io/py/mabwiser.svg)](https://pypi.python.org/pypi/mabwiser/) [![PyPI license](https://img.shields.io/pypi/l/mabwiser.svg)](https://pypi.python.org/pypi/mabwiser/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![Downloads](https://static.pepy.tech/personalized-badge/mabwiser?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/mabwiser)
-
-# MABWiser: Parallelizable Contextual Multi-Armed Bandits 
-
-MABWiser ([IJAIT 2021](https://www.worldscientific.com/doi/10.1142/S0218213021500214), [ICTAI 2019](https://ieeexplore.ieee.org/document/8995418)) is a research library written in Python for rapid prototyping of multi-armed bandit algorithms. It supports **context-free**, **parametric** and **non-parametric** **contextual** bandit models and provides built-in parallelization for both training and testing components. 
-
-The library also provides a simulation utility for comparing different policies and performing hyper-parameter tuning. MABWiser follows a scikit-learn style public interface, adheres to [PEP-8 standards](https://www.python.org/dev/peps/pep-0008/), and is tested heavily. 
-
-For Bandit-based Recommenders, see also our [Mab2Rec library](https://github.com/fidelity/mab2rec) built on top of MABWiser. 
-
-MABWiser is developed by the Artificial Intelligence Center of Excellence at Fidelity Investments. Documentation is available at [fidelity.github.io/mabwiser](https://fidelity.github.io/mabwiser).
-
-## Quick Start
-
-```python
-# An example that shows how to use the UCB1 learning policy
-# to choose between two arms based on their expected rewards.
-
-# Import MABWiser Library
-from mabwiser.mab import MAB, LearningPolicy, NeighborhoodPolicy
-
-# Data
-arms = ['Arm1', 'Arm2']
-decisions = ['Arm1', 'Arm1', 'Arm2', 'Arm1']
-rewards = [20, 17, 25, 9]
-
-# Model 
-mab = MAB(arms, LearningPolicy.UCB1(alpha=1.25))
-
-# Train
-mab.fit(decisions, rewards)
-
-# Test
-mab.predict()
-```
-
-## Available Bandit Policies
-
-Available Learning Policies:
-* Epsilon Greedy [1, 2]
-* LinGreedy [1, 2]
-* LinTS [3]. See [11] for a formal treatment of reproducibility in LinTS
-* LinUCB [4]
-* Popularity [2]
-* Random [2]
-* Softmax [2]
-* Thompson Sampling (TS) [5]
-* Upper Confidence Bound (UCB1) [2]
-
-Available Neighborhood Policies: 
-* Clusters [6]
-* K-Nearest [7, 8]
-* LSH Nearest [9]
-* Radius [7, 8]
-* TreeBandit [10]
-
-## Installation
-
-MABWiser requires **Python 3.6+** and can be installed from PyPI using ``pip install mabwiser`` or by building from source as shown in [installation instructions](https://fidelity.github.io/mabwiser/installation.html).
-
-## Support
-
-Please submit bug reports and feature requests as [Issues](https://github.com/fidelity/mabwiser/issues).
-
-## Citation
-
-If you use MABWiser in a publication, please cite it as:
-
-* **[IJAIT 2021]** [E. Strong,  B. Kleynhans, and S. Kadioglu, "MABWiser: Parallelizable Contextual Multi-Armed Bandits"](https://www.worldscientific.com/doi/abs/10.1142/S0218213021500214)
-* **[ICTAI 2019]** [E. Strong,  B. Kleynhans, and S. Kadioglu, "MABWiser: A Parallelizable Contextual Multi-Armed Bandit Library for Python"](https://ieeexplore.ieee.org/document/8995418)
-
-```bibtex
-    @article{DBLP:journals/ijait/StrongKK21,
-      author    = {Emily Strong and Bernard Kleynhans and Serdar Kadioglu},
-      title     = {{MABWiser:} Parallelizable Contextual Multi-armed Bandits},
-      journal   = {Int. J. Artif. Intell. Tools},
-      volume    = {30},
-      number    = {4},
-      pages     = {2150021:1--2150021:19},
-      year      = {2021},
-      url       = {https://doi.org/10.1142/S0218213021500214},
-      doi       = {10.1142/S0218213021500214},
-    }
-
-    @inproceedings{DBLP:conf/ictai/StrongKK19,
-    author    = {Emily Strong and Bernard Kleynhans and Serdar Kadioglu},
-    title     = {MABWiser: {A} Parallelizable Contextual Multi-Armed Bandit Library for Python},
-    booktitle = {31st {IEEE} International Conference on Tools with Artificial Intelligence, {ICTAI} 2019, Portland, OR, USA, November 4-6, 2019},
-    pages     = {909--914},
-    publisher = {{IEEE}},
-    year      = {2019},
-    url       = {https://doi.org/10.1109/ICTAI.2019.00129},
-    doi       = {10.1109/ICTAI.2019.00129},
-    }
-```
-
-## License
-
-MABWiser is licensed under the [Apache License 2.0](LICENSE).
-
-## References
-
-1. John Langford and Tong Zhang. The epoch-greedy algorithm for contextual multi-armed bandits
-2. Volodymyr Kuleshov and Doina Precup. Algorithms for multi-armed bandit problems
-3. Agrawal, Shipra and Navin Goyal. Thompson sampling for contextual bandits with linear payoffs
-4. Chu, Wei, Li, Lihong, Reyzin Lev, and Schapire Robert. Contextual bandits with linear payoff functions
-5. Osband, Ian, Daniel Russo, and Benjamin Van Roy. More efficient reinforcement learning via posterior sampling
-6. Nguyen, Trong T. and Hady W. Lauw. Dynamic clustering of contextual multi-armed bandits
-7. Melody Y. Guan and Heinrich Jiang, Nonparametric stochastic contextual bandits
-8. Philippe Rigollet and Assaf Zeevi. Nonparametric bandits with covariates 
-9. Indyk, Piotr, Motwani, Rajeev, Raghavan, Prabhakar, Vempala, Santosh. Locality-preserving hashing in multidimensional spaces
-10. Adam N. Elmachtoub, Ryan McNellis, Sechan Oh, Marek Petrik, A practical method for solving contextual bandit problems using decision trees
-11. Doruk Kilitcioglu, Serdar Kadioglu, Non-deterministic behavior of thompson sampling with linear payoffs and how to avoid it
-
-<br>
+Metadata-Version: 2.1
+Name: mabwiser
+Version: 2.7.1
+Summary: MABWiser: Parallelizable Contextual Multi-Armed Bandits Library
+Home-page: https://github.com/fidelity/mabwiser
+Author: FMR LLC
+License: UNKNOWN
+Project-URL: Documentation, https://fidelity.github.io/mabwiser/
+Project-URL: Source, https://github.com/fidelity/mabwiser
+Description: [![ci](https://github.com/fidelity/mabwiser/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/fidelity/mabwiser/actions/workflows/ci.yml) [![PyPI version fury.io](https://badge.fury.io/py/mabwiser.svg)](https://pypi.python.org/pypi/mabwiser/) [![PyPI license](https://img.shields.io/pypi/l/mabwiser.svg)](https://pypi.python.org/pypi/mabwiser/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![Downloads](https://static.pepy.tech/personalized-badge/mabwiser?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/mabwiser)
+        
+        # MABWiser: Parallelizable Contextual Multi-Armed Bandits 
+        
+        MABWiser ([IJAIT 2021](https://www.worldscientific.com/doi/10.1142/S0218213021500214), [ICTAI 2019](https://ieeexplore.ieee.org/document/8995418)) is a research library written in Python for rapid prototyping of multi-armed bandit algorithms. It supports **context-free**, **parametric** and **non-parametric** **contextual** bandit models and provides built-in parallelization for both training and testing components. 
+        
+        The library also provides a simulation utility for comparing different policies and performing hyper-parameter tuning. MABWiser follows a scikit-learn style public interface, adheres to [PEP-8 standards](https://www.python.org/dev/peps/pep-0008/), and is tested heavily. 
+        
+        MABWiser is developed by the Artificial Intelligence Center of Excellence at Fidelity Investments. Documentation is available at [fidelity.github.io/mabwiser](https://fidelity.github.io/mabwiser).
+        
+        ## Bandit-based Recommender Systems
+        To solve personalized recommendation problems, MABWiser is integrated into our [Mab2Rec library](https://github.com/fidelity/mab2rec). Mab2Rec enables building content- and context-aware recommender systems, whereby MABWiser helps selecting the next best item (arm).
+        
+        ## Bandit-based Large-Neighborhood Search
+        To solve combinatorial optimization problems, MABWiser is integrated into [Adaptive Large Neighborhood Search](https://github.com/N-Wouda/ALNS). The ALNS library enables building metaheuristics for complex optimization problems, whereby MABWiser helps selecting the next best destroy, repair operation (arm).  
+        
+        ## Quick Start
+        
+        ```python
+        # An example that shows how to use the UCB1 learning policy
+        # to choose between two arms based on their expected rewards.
+        
+        # Import MABWiser Library
+        from mabwiser.mab import MAB, LearningPolicy, NeighborhoodPolicy
+        
+        # Data
+        arms = ['Arm1', 'Arm2']
+        decisions = ['Arm1', 'Arm1', 'Arm2', 'Arm1']
+        rewards = [20, 17, 25, 9]
+        
+        # Model 
+        mab = MAB(arms, LearningPolicy.UCB1(alpha=1.25))
+        
+        # Train
+        mab.fit(decisions, rewards)
+        
+        # Test
+        mab.predict()
+        ```
+        
+        ## Available Bandit Policies
+        
+        Available Learning Policies:
+        * Epsilon Greedy [1, 2]
+        * LinGreedy [1, 2]
+        * LinTS [3]. See [11] for a formal treatment of reproducibility in LinTS
+        * LinUCB [4]
+        * Popularity [2]
+        * Random [2]
+        * Softmax [2]
+        * Thompson Sampling (TS) [5]
+        * Upper Confidence Bound (UCB1) [2]
+        
+        Available Neighborhood Policies: 
+        * Clusters [6]
+        * K-Nearest [7, 8]
+        * LSH Nearest [9]
+        * Radius [7, 8]
+        * TreeBandit [10]
+        
+        ## Installation
+        
+        MABWiser requires **Python 3.8+** and can be installed from PyPI using ``pip install mabwiser`` or by building from source as shown in [installation instructions](https://fidelity.github.io/mabwiser/installation.html).
+        
+        ## Support
+        
+        Please submit bug reports and feature requests as [Issues](https://github.com/fidelity/mabwiser/issues).
+        
+        ## Citation
+        
+        If you use MABWiser in a publication, please cite it as:
+        
+        * **[IJAIT 2021]** [E. Strong,  B. Kleynhans, and S. Kadioglu, "MABWiser: Parallelizable Contextual Multi-Armed Bandits"](https://www.worldscientific.com/doi/abs/10.1142/S0218213021500214)
+        * **[ICTAI 2019]** [E. Strong,  B. Kleynhans, and S. Kadioglu, "MABWiser: A Parallelizable Contextual Multi-Armed Bandit Library for Python"](https://ieeexplore.ieee.org/document/8995418)
+        
+        ```bibtex
+            @article{DBLP:journals/ijait/StrongKK21,
+              author    = {Emily Strong and Bernard Kleynhans and Serdar Kadioglu},
+              title     = {{MABWiser:} Parallelizable Contextual Multi-armed Bandits},
+              journal   = {Int. J. Artif. Intell. Tools},
+              volume    = {30},
+              number    = {4},
+              pages     = {2150021:1--2150021:19},
+              year      = {2021},
+              url       = {https://doi.org/10.1142/S0218213021500214},
+              doi       = {10.1142/S0218213021500214},
+            }
+        
+            @inproceedings{DBLP:conf/ictai/StrongKK19,
+            author    = {Emily Strong and Bernard Kleynhans and Serdar Kadioglu},
+            title     = {MABWiser: {A} Parallelizable Contextual Multi-Armed Bandit Library for Python},
+            booktitle = {31st {IEEE} International Conference on Tools with Artificial Intelligence, {ICTAI} 2019, Portland, OR, USA, November 4-6, 2019},
+            pages     = {909--914},
+            publisher = {{IEEE}},
+            year      = {2019},
+            url       = {https://doi.org/10.1109/ICTAI.2019.00129},
+            doi       = {10.1109/ICTAI.2019.00129},
+            }
+        ```
+        
+        ## License
+        
+        MABWiser is licensed under the [Apache License 2.0](LICENSE).
+        
+        ## References
+        
+        1. John Langford and Tong Zhang. The epoch-greedy algorithm for contextual multi-armed bandits
+        2. Volodymyr Kuleshov and Doina Precup. Algorithms for multi-armed bandit problems
+        3. Agrawal, Shipra and Navin Goyal. Thompson sampling for contextual bandits with linear payoffs
+        4. Chu, Wei, Li, Lihong, Reyzin Lev, and Schapire Robert. Contextual bandits with linear payoff functions
+        5. Osband, Ian, Daniel Russo, and Benjamin Van Roy. More efficient reinforcement learning via posterior sampling
+        6. Nguyen, Trong T. and Hady W. Lauw. Dynamic clustering of contextual multi-armed bandits
+        7. Melody Y. Guan and Heinrich Jiang, Nonparametric stochastic contextual bandits
+        8. Philippe Rigollet and Assaf Zeevi. Nonparametric bandits with covariates 
+        9. Indyk, Piotr, Motwani, Rajeev, Raghavan, Prabhakar, Vempala, Santosh. Locality-preserving hashing in multidimensional spaces
+        10. Adam N. Elmachtoub, Ryan McNellis, Sechan Oh, Marek Petrik, A practical method for solving contextual bandit problems using decision trees
+        11. Doruk Kilitcioglu, Serdar Kadioglu, Non-deterministic behavior of thompson sampling with linear payoffs and how to avoid it
+        
+        <br>
+        
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
```

### Comparing `mabwiser-2.7.0/mabwiser/approximate.py` & `mabwiser-2.7.1/mabwiser/approximate.py`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/mabwiser/base_mab.py` & `mabwiser-2.7.1/mabwiser/base_mab.py`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/mabwiser/clusters.py` & `mabwiser-2.7.1/mabwiser/clusters.py`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/mabwiser/greedy.py` & `mabwiser-2.7.1/mabwiser/greedy.py`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/mabwiser/linear.py` & `mabwiser-2.7.1/mabwiser/linear.py`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/mabwiser/mab.py` & `mabwiser-2.7.1/mabwiser/mab.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 This module defines the public interface of the **MABWiser Library** providing access to the following modules:
 
     - ``MAB``
     - ``LearningPolicy``
     - ``NeighborhoodPolicy``
 """
 
-from typing import List, Union, Dict, NamedTuple, NoReturn, Callable, Optional
+from typing import List, Union, Dict, NamedTuple, NoReturn, Callable, Optional, NewType
 
 import numpy as np
 import pandas as pd
 from sklearn.cluster import MiniBatchKMeans
 from sklearn.tree import DecisionTreeRegressor
 
 from mabwiser._version import __author__, __email__, __version__, __copyright__
@@ -663,27 +663,48 @@
         def _is_compatible(self, learning_policy: LearningPolicy):
             # TreeBandit is compatible with these learning policies
             return isinstance(learning_policy, (LearningPolicy.EpsilonGreedy,
                                                 LearningPolicy.UCB1,
                                                 LearningPolicy.ThompsonSampling))
 
 
+# LearningPolicyType is the Union of all possible learning policies
+LearningPolicyType = NewType('LearningPolicyType', Union[LearningPolicy.EpsilonGreedy,
+                                                         LearningPolicy.Popularity,
+                                                         LearningPolicy.Random,
+                                                         LearningPolicy.Softmax,
+                                                         LearningPolicy.ThompsonSampling,
+                                                         LearningPolicy.UCB1,
+                                                         LearningPolicy.LinGreedy,
+                                                         LearningPolicy.LinTS,
+                                                         LearningPolicy.LinUCB])
+
+
+# NeighborhoodPolicyType is the Union of all possible neighborhood policies
+NeighborhoodPolicyType = NewType('NeighborhoodPolicyType', Union[None,
+                                                                 NeighborhoodPolicy.LSHNearest,
+                                                                 NeighborhoodPolicy.Clusters,
+                                                                 NeighborhoodPolicy.KNearest,
+                                                                 NeighborhoodPolicy.Radius,
+                                                                 NeighborhoodPolicy.TreeBandit])
+
+
 class MAB:
     """**MABWiser: Contextual Multi-Armed Bandit Library**
 
     MABWiser is a research library for fast prototyping of multi-armed bandit algorithms.
     It supports **context-free**, **parametric** and **non-parametric** **contextual** bandit models.
 
     Attributes
     ----------
     arms : list
-        The list of all of the arms available for decisions. Arms can be integers, strings, etc.
-    learning_policy : LearningPolicy
+        The list of all the arms available for decisions. Arms can be integers, strings, etc.
+    learning_policy : LearningPolicyType
         The learning policy.
-    neighborhood_policy : NeighborhoodPolicy
+    neighborhood_policy : NeighborhoodPolicyType
         The neighborhood policy.
     is_contextual : bool
         True if contextual policy is given, false otherwise. This is a read-only data field.
     seed : numbers.Rational
         The random seed to initialize the internal random number generator. This is a read-only data field.
     n_jobs: int
         This is used to specify how many concurrent processes/threads should be used for parallelized routines.
@@ -691,15 +712,15 @@
         If set to -1, all CPUs are used.
         If set to -2, all CPUs but one are used, and so on.
     backend: str, optional
         Specify a parallelization backend implementation supported in the joblib library. Supported options are:
         - “loky” used by default, can induce some communication and memory overhead when exchanging input and
           output data with the worker Python processes.
         - “multiprocessing” previous process-based backend based on multiprocessing.Pool. Less robust than loky.
-        - “threading” is a very low-overhead backend but it suffers from the Python Global Interpreter Lock if the
+        - “threading” is a very low-overhead backend but, it suffers from the Python Global Interpreter Lock if the
           called function relies a lot on Python objects.
         Default value is None. In this case the default backend selected by joblib will be used.
 
     Examples
     --------
         >>> from mabwiser.mab import MAB, LearningPolicy
         >>> arms = ['Arm1', 'Arm2']
@@ -727,45 +748,32 @@
         >>> contextual_mab.partial_fit(['Arm3'], [30], [[1, 1, 1]])
         >>> contextual_mab.predict([[1, 1, 1]])
         'Arm3'
     """
 
     def __init__(self,
                  arms: List[Arm],  # The list of arms
-                 learning_policy: Union[LearningPolicy.EpsilonGreedy,
-                                        LearningPolicy.Popularity,
-                                        LearningPolicy.Random,
-                                        LearningPolicy.Softmax,
-                                        LearningPolicy.ThompsonSampling,
-                                        LearningPolicy.UCB1,
-                                        LearningPolicy.LinGreedy,
-                                        LearningPolicy.LinTS,
-                                        LearningPolicy.LinUCB],  # The learning policy
-                 neighborhood_policy: Union[None,
-                                            NeighborhoodPolicy.LSHNearest,
-                                            NeighborhoodPolicy.Clusters,
-                                            NeighborhoodPolicy.KNearest,
-                                            NeighborhoodPolicy.Radius,
-                                            NeighborhoodPolicy.TreeBandit] = None,  # The context policy, optional
+                 learning_policy: LearningPolicyType,  # The learning policy
+                 neighborhood_policy: NeighborhoodPolicyType = None,  # The context policy, optional
                  seed: int = Constants.default_seed,  # The random seed
                  n_jobs: int = 1,  # Number of parallel jobs
                  backend: str = None  # Parallel backend implementation
                  ):
         """Initializes a multi-armed bandit (MAB) with the given arguments.
 
         Validates the arguments and raises exception in case there are violations.
 
         Parameters
         ----------
         arms : List[Union[int, float, str]]
-            The list of all of the arms available for decisions.
+            The list of all the arms available for decisions.
             Arms can be integers, strings, etc.
-        learning_policy : LearningPolicy
+        learning_policy : LearningPolicyType
             The learning policy.
-        neighborhood_policy : NeighborhoodPolicy, optional
+        neighborhood_policy : NeighborhoodPolicyType, optional
             The context policy. Default value is None.
         seed : numbers.Rational, optional
             The random seed to initialize the random number generator.
             Default value is set to Constants.default_seed.value
         n_jobs: int, optional
             This is used to specify how many concurrent processes/threads should be used for parallelized routines.
             Default value is set to 1.
```

### Comparing `mabwiser-2.7.0/mabwiser/neighbors.py` & `mabwiser-2.7.1/mabwiser/neighbors.py`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/mabwiser/popularity.py` & `mabwiser-2.7.1/mabwiser/popularity.py`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/mabwiser/rand.py` & `mabwiser-2.7.1/mabwiser/rand.py`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/mabwiser/simulator.py` & `mabwiser-2.7.1/mabwiser/simulator.py`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/mabwiser/softmax.py` & `mabwiser-2.7.1/mabwiser/softmax.py`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/mabwiser/thompson.py` & `mabwiser-2.7.1/mabwiser/thompson.py`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/mabwiser/treebandit.py` & `mabwiser-2.7.1/mabwiser/treebandit.py`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/mabwiser/ucb.py` & `mabwiser-2.7.1/mabwiser/ucb.py`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/mabwiser/utils.py` & `mabwiser-2.7.1/mabwiser/utils.py`

 * *Files identical despite different names*

### Comparing `mabwiser-2.7.0/mabwiser.egg-info/PKG-INFO` & `mabwiser-2.7.1/mabwiser.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,133 +1,134 @@
 Metadata-Version: 2.1
 Name: mabwiser
-Version: 2.7.0
+Version: 2.7.1
 Summary: MABWiser: Parallelizable Contextual Multi-Armed Bandits Library
 Home-page: https://github.com/fidelity/mabwiser
 Author: FMR LLC
 License: UNKNOWN
 Project-URL: Documentation, https://fidelity.github.io/mabwiser/
 Project-URL: Source, https://github.com/fidelity/mabwiser
+Description: [![ci](https://github.com/fidelity/mabwiser/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/fidelity/mabwiser/actions/workflows/ci.yml) [![PyPI version fury.io](https://badge.fury.io/py/mabwiser.svg)](https://pypi.python.org/pypi/mabwiser/) [![PyPI license](https://img.shields.io/pypi/l/mabwiser.svg)](https://pypi.python.org/pypi/mabwiser/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![Downloads](https://static.pepy.tech/personalized-badge/mabwiser?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/mabwiser)
+        
+        # MABWiser: Parallelizable Contextual Multi-Armed Bandits 
+        
+        MABWiser ([IJAIT 2021](https://www.worldscientific.com/doi/10.1142/S0218213021500214), [ICTAI 2019](https://ieeexplore.ieee.org/document/8995418)) is a research library written in Python for rapid prototyping of multi-armed bandit algorithms. It supports **context-free**, **parametric** and **non-parametric** **contextual** bandit models and provides built-in parallelization for both training and testing components. 
+        
+        The library also provides a simulation utility for comparing different policies and performing hyper-parameter tuning. MABWiser follows a scikit-learn style public interface, adheres to [PEP-8 standards](https://www.python.org/dev/peps/pep-0008/), and is tested heavily. 
+        
+        MABWiser is developed by the Artificial Intelligence Center of Excellence at Fidelity Investments. Documentation is available at [fidelity.github.io/mabwiser](https://fidelity.github.io/mabwiser).
+        
+        ## Bandit-based Recommender Systems
+        To solve personalized recommendation problems, MABWiser is integrated into our [Mab2Rec library](https://github.com/fidelity/mab2rec). Mab2Rec enables building content- and context-aware recommender systems, whereby MABWiser helps selecting the next best item (arm).
+        
+        ## Bandit-based Large-Neighborhood Search
+        To solve combinatorial optimization problems, MABWiser is integrated into [Adaptive Large Neighborhood Search](https://github.com/N-Wouda/ALNS). The ALNS library enables building metaheuristics for complex optimization problems, whereby MABWiser helps selecting the next best destroy, repair operation (arm).  
+        
+        ## Quick Start
+        
+        ```python
+        # An example that shows how to use the UCB1 learning policy
+        # to choose between two arms based on their expected rewards.
+        
+        # Import MABWiser Library
+        from mabwiser.mab import MAB, LearningPolicy, NeighborhoodPolicy
+        
+        # Data
+        arms = ['Arm1', 'Arm2']
+        decisions = ['Arm1', 'Arm1', 'Arm2', 'Arm1']
+        rewards = [20, 17, 25, 9]
+        
+        # Model 
+        mab = MAB(arms, LearningPolicy.UCB1(alpha=1.25))
+        
+        # Train
+        mab.fit(decisions, rewards)
+        
+        # Test
+        mab.predict()
+        ```
+        
+        ## Available Bandit Policies
+        
+        Available Learning Policies:
+        * Epsilon Greedy [1, 2]
+        * LinGreedy [1, 2]
+        * LinTS [3]. See [11] for a formal treatment of reproducibility in LinTS
+        * LinUCB [4]
+        * Popularity [2]
+        * Random [2]
+        * Softmax [2]
+        * Thompson Sampling (TS) [5]
+        * Upper Confidence Bound (UCB1) [2]
+        
+        Available Neighborhood Policies: 
+        * Clusters [6]
+        * K-Nearest [7, 8]
+        * LSH Nearest [9]
+        * Radius [7, 8]
+        * TreeBandit [10]
+        
+        ## Installation
+        
+        MABWiser requires **Python 3.8+** and can be installed from PyPI using ``pip install mabwiser`` or by building from source as shown in [installation instructions](https://fidelity.github.io/mabwiser/installation.html).
+        
+        ## Support
+        
+        Please submit bug reports and feature requests as [Issues](https://github.com/fidelity/mabwiser/issues).
+        
+        ## Citation
+        
+        If you use MABWiser in a publication, please cite it as:
+        
+        * **[IJAIT 2021]** [E. Strong,  B. Kleynhans, and S. Kadioglu, "MABWiser: Parallelizable Contextual Multi-Armed Bandits"](https://www.worldscientific.com/doi/abs/10.1142/S0218213021500214)
+        * **[ICTAI 2019]** [E. Strong,  B. Kleynhans, and S. Kadioglu, "MABWiser: A Parallelizable Contextual Multi-Armed Bandit Library for Python"](https://ieeexplore.ieee.org/document/8995418)
+        
+        ```bibtex
+            @article{DBLP:journals/ijait/StrongKK21,
+              author    = {Emily Strong and Bernard Kleynhans and Serdar Kadioglu},
+              title     = {{MABWiser:} Parallelizable Contextual Multi-armed Bandits},
+              journal   = {Int. J. Artif. Intell. Tools},
+              volume    = {30},
+              number    = {4},
+              pages     = {2150021:1--2150021:19},
+              year      = {2021},
+              url       = {https://doi.org/10.1142/S0218213021500214},
+              doi       = {10.1142/S0218213021500214},
+            }
+        
+            @inproceedings{DBLP:conf/ictai/StrongKK19,
+            author    = {Emily Strong and Bernard Kleynhans and Serdar Kadioglu},
+            title     = {MABWiser: {A} Parallelizable Contextual Multi-Armed Bandit Library for Python},
+            booktitle = {31st {IEEE} International Conference on Tools with Artificial Intelligence, {ICTAI} 2019, Portland, OR, USA, November 4-6, 2019},
+            pages     = {909--914},
+            publisher = {{IEEE}},
+            year      = {2019},
+            url       = {https://doi.org/10.1109/ICTAI.2019.00129},
+            doi       = {10.1109/ICTAI.2019.00129},
+            }
+        ```
+        
+        ## License
+        
+        MABWiser is licensed under the [Apache License 2.0](LICENSE).
+        
+        ## References
+        
+        1. John Langford and Tong Zhang. The epoch-greedy algorithm for contextual multi-armed bandits
+        2. Volodymyr Kuleshov and Doina Precup. Algorithms for multi-armed bandit problems
+        3. Agrawal, Shipra and Navin Goyal. Thompson sampling for contextual bandits with linear payoffs
+        4. Chu, Wei, Li, Lihong, Reyzin Lev, and Schapire Robert. Contextual bandits with linear payoff functions
+        5. Osband, Ian, Daniel Russo, and Benjamin Van Roy. More efficient reinforcement learning via posterior sampling
+        6. Nguyen, Trong T. and Hady W. Lauw. Dynamic clustering of contextual multi-armed bandits
+        7. Melody Y. Guan and Heinrich Jiang, Nonparametric stochastic contextual bandits
+        8. Philippe Rigollet and Assaf Zeevi. Nonparametric bandits with covariates 
+        9. Indyk, Piotr, Motwani, Rajeev, Raghavan, Prabhakar, Vempala, Santosh. Locality-preserving hashing in multidimensional spaces
+        10. Adam N. Elmachtoub, Ryan McNellis, Sechan Oh, Marek Petrik, A practical method for solving contextual bandit problems using decision trees
+        11. Doruk Kilitcioglu, Serdar Kadioglu, Non-deterministic behavior of thompson sampling with linear payoffs and how to avoid it
+        
+        <br>
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![ci](https://github.com/fidelity/mabwiser/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/fidelity/mabwiser/actions/workflows/ci.yml) [![PyPI version fury.io](https://badge.fury.io/py/mabwiser.svg)](https://pypi.python.org/pypi/mabwiser/) [![PyPI license](https://img.shields.io/pypi/l/mabwiser.svg)](https://pypi.python.org/pypi/mabwiser/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![Downloads](https://static.pepy.tech/personalized-badge/mabwiser?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/mabwiser)
-
-# MABWiser: Parallelizable Contextual Multi-Armed Bandits 
-
-MABWiser ([IJAIT 2021](https://www.worldscientific.com/doi/10.1142/S0218213021500214), [ICTAI 2019](https://ieeexplore.ieee.org/document/8995418)) is a research library written in Python for rapid prototyping of multi-armed bandit algorithms. It supports **context-free**, **parametric** and **non-parametric** **contextual** bandit models and provides built-in parallelization for both training and testing components. 
-
-The library also provides a simulation utility for comparing different policies and performing hyper-parameter tuning. MABWiser follows a scikit-learn style public interface, adheres to [PEP-8 standards](https://www.python.org/dev/peps/pep-0008/), and is tested heavily. 
-
-For Bandit-based Recommenders, see also our [Mab2Rec library](https://github.com/fidelity/mab2rec) built on top of MABWiser. 
-
-MABWiser is developed by the Artificial Intelligence Center of Excellence at Fidelity Investments. Documentation is available at [fidelity.github.io/mabwiser](https://fidelity.github.io/mabwiser).
-
-## Quick Start
-
-```python
-# An example that shows how to use the UCB1 learning policy
-# to choose between two arms based on their expected rewards.
-
-# Import MABWiser Library
-from mabwiser.mab import MAB, LearningPolicy, NeighborhoodPolicy
-
-# Data
-arms = ['Arm1', 'Arm2']
-decisions = ['Arm1', 'Arm1', 'Arm2', 'Arm1']
-rewards = [20, 17, 25, 9]
-
-# Model 
-mab = MAB(arms, LearningPolicy.UCB1(alpha=1.25))
-
-# Train
-mab.fit(decisions, rewards)
-
-# Test
-mab.predict()
-```
-
-## Available Bandit Policies
-
-Available Learning Policies:
-* Epsilon Greedy [1, 2]
-* LinGreedy [1, 2]
-* LinTS [3]. See [11] for a formal treatment of reproducibility in LinTS
-* LinUCB [4]
-* Popularity [2]
-* Random [2]
-* Softmax [2]
-* Thompson Sampling (TS) [5]
-* Upper Confidence Bound (UCB1) [2]
-
-Available Neighborhood Policies: 
-* Clusters [6]
-* K-Nearest [7, 8]
-* LSH Nearest [9]
-* Radius [7, 8]
-* TreeBandit [10]
-
-## Installation
-
-MABWiser requires **Python 3.6+** and can be installed from PyPI using ``pip install mabwiser`` or by building from source as shown in [installation instructions](https://fidelity.github.io/mabwiser/installation.html).
-
-## Support
-
-Please submit bug reports and feature requests as [Issues](https://github.com/fidelity/mabwiser/issues).
-
-## Citation
-
-If you use MABWiser in a publication, please cite it as:
-
-* **[IJAIT 2021]** [E. Strong,  B. Kleynhans, and S. Kadioglu, "MABWiser: Parallelizable Contextual Multi-Armed Bandits"](https://www.worldscientific.com/doi/abs/10.1142/S0218213021500214)
-* **[ICTAI 2019]** [E. Strong,  B. Kleynhans, and S. Kadioglu, "MABWiser: A Parallelizable Contextual Multi-Armed Bandit Library for Python"](https://ieeexplore.ieee.org/document/8995418)
-
-```bibtex
-    @article{DBLP:journals/ijait/StrongKK21,
-      author    = {Emily Strong and Bernard Kleynhans and Serdar Kadioglu},
-      title     = {{MABWiser:} Parallelizable Contextual Multi-armed Bandits},
-      journal   = {Int. J. Artif. Intell. Tools},
-      volume    = {30},
-      number    = {4},
-      pages     = {2150021:1--2150021:19},
-      year      = {2021},
-      url       = {https://doi.org/10.1142/S0218213021500214},
-      doi       = {10.1142/S0218213021500214},
-    }
-
-    @inproceedings{DBLP:conf/ictai/StrongKK19,
-    author    = {Emily Strong and Bernard Kleynhans and Serdar Kadioglu},
-    title     = {MABWiser: {A} Parallelizable Contextual Multi-Armed Bandit Library for Python},
-    booktitle = {31st {IEEE} International Conference on Tools with Artificial Intelligence, {ICTAI} 2019, Portland, OR, USA, November 4-6, 2019},
-    pages     = {909--914},
-    publisher = {{IEEE}},
-    year      = {2019},
-    url       = {https://doi.org/10.1109/ICTAI.2019.00129},
-    doi       = {10.1109/ICTAI.2019.00129},
-    }
-```
-
-## License
-
-MABWiser is licensed under the [Apache License 2.0](LICENSE).
-
-## References
-
-1. John Langford and Tong Zhang. The epoch-greedy algorithm for contextual multi-armed bandits
-2. Volodymyr Kuleshov and Doina Precup. Algorithms for multi-armed bandit problems
-3. Agrawal, Shipra and Navin Goyal. Thompson sampling for contextual bandits with linear payoffs
-4. Chu, Wei, Li, Lihong, Reyzin Lev, and Schapire Robert. Contextual bandits with linear payoff functions
-5. Osband, Ian, Daniel Russo, and Benjamin Van Roy. More efficient reinforcement learning via posterior sampling
-6. Nguyen, Trong T. and Hady W. Lauw. Dynamic clustering of contextual multi-armed bandits
-7. Melody Y. Guan and Heinrich Jiang, Nonparametric stochastic contextual bandits
-8. Philippe Rigollet and Assaf Zeevi. Nonparametric bandits with covariates 
-9. Indyk, Piotr, Motwani, Rajeev, Raghavan, Prabhakar, Vempala, Santosh. Locality-preserving hashing in multidimensional spaces
-10. Adam N. Elmachtoub, Ryan McNellis, Sechan Oh, Marek Petrik, A practical method for solving contextual bandit problems using decision trees
-11. Doruk Kilitcioglu, Serdar Kadioglu, Non-deterministic behavior of thompson sampling with linear payoffs and how to avoid it
-
-<br>
-
-
```

### Comparing `mabwiser-2.7.0/setup.py` & `mabwiser-2.7.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     version=__version__,
     author=__author__,
     url="https://github.com/fidelity/mabwiser",
     packages=setuptools.find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     install_requires=required,
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python",
         "Operating System :: OS Independent",
     ],
     project_urls={
         "Documentation": "https://fidelity.github.io/mabwiser/",
         "Source": "https://github.com/fidelity/mabwiser"
     }
 )
```

