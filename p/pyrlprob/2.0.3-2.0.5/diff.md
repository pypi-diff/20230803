# Comparing `tmp/pyrlprob-2.0.3.tar.gz` & `tmp/pyrlprob-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrlprob-2.0.3.tar", last modified: Tue Apr 25 19:26:18 2023, max compression
+gzip compressed data, was "pyrlprob-2.0.5.tar", last modified: Thu Aug  3 18:02:13 2023, max compression
```

## Comparing `pyrlprob-2.0.3.tar` & `pyrlprob-2.0.5.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.626211 pyrlprob-2.0.3/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1073 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/LICENSE.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      301 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/MANIFEST.in
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2322 2023-04-25 19:26:18.625215 pyrlprob-2.0.3/PKG-INFO
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1803 2023-03-08 19:07:40.000000 pyrlprob-2.0.3/README.md
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      103 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyproject.toml
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.343208 pyrlprob-2.0.3/pyrlprob/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      250 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1157 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/__main__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)    15337 2023-04-21 21:39:44.000000 pyrlprob-2.0.3/pyrlprob/base_funs.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      661 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/commands.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.277208 pyrlprob-2.0.3/pyrlprob/include/
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.370209 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2938 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/binding.cpp
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     5140 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/mdp.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     3818 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/mdp_vec.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     4114 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/py_mdp.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     7448 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/mdp.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)    12688 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/problem.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.447207 pyrlprob-2.0.3/pyrlprob/tests/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      477 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/__init__.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.527209 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      210 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      390 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/binding.cpp
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     6849 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.cpp
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2063 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1830 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.py
--rwx------   0 lorenzof (1001204911) domain users (1000000513)   463776 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      696 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d_dyn.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1405 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/rk4.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1282 2023-03-08 18:08:23.000000 pyrlprob-2.0.3/pyrlprob/tests/landing1d_cpp.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1574 2023-04-21 21:36:35.000000 pyrlprob-2.0.3/pyrlprob/tests/landing1d_load.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1266 2023-04-21 21:39:57.000000 pyrlprob-2.0.3/pyrlprob/tests/landing1d_py.yaml
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.539206 pyrlprob-2.0.3/pyrlprob/tests/py_tests/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      190 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     4713 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      974 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d_dyn.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     6161 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d_gym.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.611210 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      428 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      691 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      331 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      560 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1064 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      496 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      433 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_DQN.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      713 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      520 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      456 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      582 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      732 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      639 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      497 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      714 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      615 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     5273 2023-04-21 21:13:31.000000 pyrlprob-2.0.3/pyrlprob/tests/test_landing1d.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2813 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/test_multiple_gym.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.623205 pyrlprob-2.0.3/pyrlprob/utils/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      546 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/utils/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     3183 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/utils/auxiliary.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     4637 2023-04-25 19:25:53.000000 pyrlprob-2.0.3/pyrlprob/utils/callbacks.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     3036 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/utils/plots.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.357207 pyrlprob-2.0.3/pyrlprob.egg-info/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2322 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/PKG-INFO
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2454 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/SOURCES.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)        1 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/dependency_links.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      194 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/requires.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)        9 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/top_level.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)       38 2023-04-25 19:26:18.627209 pyrlprob-2.0.3/setup.cfg
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1242 2023-04-25 19:25:59.000000 pyrlprob-2.0.3/setup.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2023-08-03 18:02:13.690062 pyrlprob-2.0.5/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1073 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/LICENSE.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      301 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/MANIFEST.in
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2322 2023-08-03 18:02:13.687067 pyrlprob-2.0.5/PKG-INFO
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1803 2023-03-08 19:07:40.000000 pyrlprob-2.0.5/README.md
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      103 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyproject.toml
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2023-08-03 18:02:13.426059 pyrlprob-2.0.5/pyrlprob/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      250 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1157 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/__main__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)    15337 2023-04-21 21:39:44.000000 pyrlprob-2.0.5/pyrlprob/base_funs.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      661 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/commands.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2023-08-03 18:02:13.393060 pyrlprob-2.0.5/pyrlprob/include/
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2023-08-03 18:02:13.484061 pyrlprob-2.0.5/pyrlprob/include/pyrlprob/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2938 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/include/pyrlprob/binding.cpp
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     5140 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/include/pyrlprob/mdp.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     3818 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/include/pyrlprob/mdp_vec.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     4114 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/include/pyrlprob/py_mdp.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     7448 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/mdp.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)    12688 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/problem.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2023-08-03 18:02:13.525062 pyrlprob-2.0.5/pyrlprob/tests/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      477 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/__init__.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2023-08-03 18:02:13.568069 pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      210 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      390 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/binding.cpp
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     6849 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/landing1d.cpp
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2063 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/landing1d.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1830 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/landing1d.py
+-rwx------   0 lorenzof (332258323) domainusers (245600513)   463776 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      696 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/landing1d_dyn.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1405 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/rk4.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1282 2023-03-08 18:08:23.000000 pyrlprob-2.0.5/pyrlprob/tests/landing1d_cpp.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1574 2023-04-21 21:36:35.000000 pyrlprob-2.0.5/pyrlprob/tests/landing1d_load.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1266 2023-04-21 21:39:57.000000 pyrlprob-2.0.5/pyrlprob/tests/landing1d_py.yaml
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2023-08-03 18:02:13.577078 pyrlprob-2.0.5/pyrlprob/tests/py_tests/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      190 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     4713 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/landing1d.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      974 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/landing1d_dyn.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     6161 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/landing1d_gym.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2023-08-03 18:02:13.674063 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      428 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      691 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      331 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      560 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1064 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      496 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      433 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_DQN.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      713 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      520 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      456 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      582 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      732 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      639 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      497 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      714 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      615 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     5273 2023-04-21 21:13:31.000000 pyrlprob-2.0.5/pyrlprob/tests/test_landing1d.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2813 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/tests/test_multiple_gym.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2023-08-03 18:02:13.683069 pyrlprob-2.0.5/pyrlprob/utils/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      546 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/utils/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     3183 2022-11-23 23:28:53.000000 pyrlprob-2.0.5/pyrlprob/utils/auxiliary.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     4637 2023-04-25 19:25:53.000000 pyrlprob-2.0.5/pyrlprob/utils/callbacks.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     3154 2023-08-03 17:57:45.000000 pyrlprob-2.0.5/pyrlprob/utils/plots.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2023-08-03 18:02:13.472066 pyrlprob-2.0.5/pyrlprob.egg-info/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2322 2023-08-03 18:02:13.000000 pyrlprob-2.0.5/pyrlprob.egg-info/PKG-INFO
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2454 2023-08-03 18:02:13.000000 pyrlprob-2.0.5/pyrlprob.egg-info/SOURCES.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)        1 2023-08-03 18:02:13.000000 pyrlprob-2.0.5/pyrlprob.egg-info/dependency_links.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      194 2023-08-03 18:02:13.000000 pyrlprob-2.0.5/pyrlprob.egg-info/requires.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)        9 2023-08-03 18:02:13.000000 pyrlprob-2.0.5/pyrlprob.egg-info/top_level.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)       38 2023-08-03 18:02:13.691062 pyrlprob-2.0.5/setup.cfg
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1242 2023-08-03 18:01:52.000000 pyrlprob-2.0.5/setup.py
```

### Comparing `pyrlprob-2.0.3/LICENSE.txt` & `pyrlprob-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/PKG-INFO` & `pyrlprob-2.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrlprob
-Version: 2.0.3
+Version: 2.0.5
 Summary: Train Gym-derived environments in Python/C++ through Ray RLlib
 Home-page: https://github.com/LorenzoFederici/pyrlprob
 Author: Lorenzo Federici
 Author-email: federicilorenzo94@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrlprob-2.0.3/README.md` & `pyrlprob-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/__main__.py` & `pyrlprob-2.0.5/pyrlprob/__main__.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/base_funs.py` & `pyrlprob-2.0.5/pyrlprob/base_funs.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/commands.py` & `pyrlprob-2.0.5/pyrlprob/commands.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/include/pyrlprob/binding.cpp` & `pyrlprob-2.0.5/pyrlprob/include/pyrlprob/binding.cpp`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/include/pyrlprob/mdp.h` & `pyrlprob-2.0.5/pyrlprob/include/pyrlprob/mdp.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/include/pyrlprob/mdp_vec.h` & `pyrlprob-2.0.5/pyrlprob/include/pyrlprob/mdp_vec.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/include/pyrlprob/py_mdp.h` & `pyrlprob-2.0.5/pyrlprob/include/pyrlprob/py_mdp.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/mdp.py` & `pyrlprob-2.0.5/pyrlprob/mdp.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/problem.py` & `pyrlprob-2.0.5/pyrlprob/problem.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.cpp` & `pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/landing1d.cpp`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.h` & `pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/landing1d.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.py` & `pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so` & `pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d_dyn.h` & `pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/landing1d_dyn.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/rk4.h` & `pyrlprob-2.0.5/pyrlprob/tests/cpp_tests/rk4.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/landing1d_cpp.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/landing1d_cpp.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/landing1d_load.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/landing1d_load.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/landing1d_py.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/landing1d_py.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d.py` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d_dyn.py` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/landing1d_dyn.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d_gym.py` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/landing1d_gym.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml` & `pyrlprob-2.0.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/test_landing1d.py` & `pyrlprob-2.0.5/pyrlprob/tests/test_landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/test_multiple_gym.py` & `pyrlprob-2.0.5/pyrlprob/tests/test_multiple_gym.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/utils/__init__.py` & `pyrlprob-2.0.5/pyrlprob/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/utils/auxiliary.py` & `pyrlprob-2.0.5/pyrlprob/utils/auxiliary.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/utils/callbacks.py` & `pyrlprob-2.0.5/pyrlprob/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/utils/plots.py` & `pyrlprob-2.0.5/pyrlprob/utils/plots.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,26 +6,28 @@
 from pyrlprob.utils.auxiliary import moving_average, metric_training_trend
 
 def plot_metric(metric_name: str,
                 experiment_dirs: List[str],
                 last_checkpoints: List[int],
                 window: int = 1,
                 step: int = 1,
+                factor: float = 1.,
                 fig: Optional[Callable] = None,
                 label: Optional[str] = None,
                 color: Optional[str] = None) -> Callable:
     """
     plot the trend during training of a metric
 
     Args:
         metric_name (str): full name of the metric (with the path)
         experiment_dirs (list): list of the experiment directories
         last_checkpoints (list): list with the last checkpoints of the experiments
         window (int): window to evaluate the moving average
         step (int): plot points every step steps
+        factor (float): factor to multiply the metric values
         fig (callable): figure object
         label (str): the label of the plotted curve
         color (str): color of the curve (if None -> random color)
     
     Return:
         fig: figure object
     """
@@ -61,12 +63,12 @@
         metric_std_max_mov = np.array(metric_mean_mov) + abs(np.array(metric_mean_mov) - np.array(metric_max_mov))/4.
 
     #Plot
     if fig is None:
         fig = plt.figure()
         fig.set_size_inches(9.7,6.4)
     ax = fig.gca()
-    ax.plot(training_iter_mov[::step], metric_mean_mov[::step], '-', linewidth='2.5', color=color, label=label)
+    ax.plot(training_iter_mov[::step], metric_mean_mov[::step]*factor, '-', linewidth='2.5', color=color, label=label)
     if metric_min !=  None:
-        plt.fill_between(training_iter_mov[::step], metric_std_min_mov[::step], metric_std_max_mov[::step], alpha=0.3, color=color)
+        plt.fill_between(training_iter_mov[::step], metric_std_min_mov[::step]*factor, metric_std_max_mov[::step]*factor, alpha=0.3, color=color)
     
     return fig
```

### Comparing `pyrlprob-2.0.3/pyrlprob.egg-info/PKG-INFO` & `pyrlprob-2.0.5/pyrlprob.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrlprob
-Version: 2.0.3
+Version: 2.0.5
 Summary: Train Gym-derived environments in Python/C++ through Ray RLlib
 Home-page: https://github.com/LorenzoFederici/pyrlprob
 Author: Lorenzo Federici
 Author-email: federicilorenzo94@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrlprob-2.0.3/pyrlprob.egg-info/SOURCES.txt` & `pyrlprob-2.0.5/pyrlprob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/setup.py` & `pyrlprob-2.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='pyrlprob',
-    version='2.0.3',
+    version='2.0.5',
     author='Lorenzo Federici',
     author_email = 'federicilorenzo94@gmail.com',
     description = 'Train Gym-derived environments in Python/C++ through Ray RLlib',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/LorenzoFederici/pyrlprob',
     classifiers = [
```

