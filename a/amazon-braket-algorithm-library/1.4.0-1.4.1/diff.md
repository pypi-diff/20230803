# Comparing `tmp/amazon-braket-algorithm-library-1.4.0.tar.gz` & `tmp/amazon-braket-algorithm-library-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-braket-algorithm-library-1.4.0.tar", last modified: Mon Jun 26 16:05:29 2023, max compression
+gzip compressed data, was "amazon-braket-algorithm-library-1.4.1.tar", last modified: Thu Aug  3 16:04:42 2023, max compression
```

## Comparing `amazon-braket-algorithm-library-1.4.0.tar` & `amazon-braket-algorithm-library-1.4.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.205947 amazon-braket-algorithm-library-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-26 16:05:29.205947 amazon-braket-algorithm-library-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-26 16:05:29.205947 amazon-braket-algorithm-library-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.193948 amazon-braket-algorithm-library-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.197948 amazon-braket-algorithm-library-1.4.0/src/amazon_braket_algorithm_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-26 16:05:29.000000 amazon-braket-algorithm-library-1.4.0/src/amazon_braket_algorithm_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-26 16:05:29.000000 amazon-braket-algorithm-library-1.4.0/src/amazon_braket_algorithm_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:05:29.000000 amazon-braket-algorithm-library-1.4.0/src/amazon_braket_algorithm_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-26 16:05:29.000000 amazon-braket-algorithm-library-1.4.0/src/amazon_braket_algorithm_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 16:05:29.000000 amazon-braket-algorithm-library-1.4.0/src/amazon_braket_algorithm_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.193948 amazon-braket-algorithm-library-1.4.0/src/braket/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.197948 amazon-braket-algorithm-library-1.4.0/src/braket/_algos/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/_algos/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.197948 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.197948 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.201948 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/bells_inequality/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/bells_inequality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/bells_inequality/bells_inequality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.201948 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/bernstein_vazirani/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/bernstein_vazirani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/bernstein_vazirani/bernstein_vazirani.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.201948 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/chsh_inequality/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/chsh_inequality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/chsh_inequality/chsh_inequality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.201948 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/deutsch_jozsa/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/deutsch_jozsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/deutsch_jozsa/deutsch_jozsa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.201948 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/grovers_search/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/grovers_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/grovers_search/grovers_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.201948 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/qc_qmc/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/qc_qmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/qc_qmc/classical_qmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/qc_qmc/qc_qmc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.205947 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_approximate_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_approximate_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_approximate_optimization/quantum_approximate_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.205947 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_circuit_born_machine/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_circuit_born_machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_circuit_born_machine/qcbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.205947 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_fourier_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_fourier_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_fourier_transform/quantum_fourier_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.205947 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_phase_estimation/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_phase_estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_phase_estimation/quantum_phase_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.205947 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_walk/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_walk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_walk/quantum_walk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.205947 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/shors/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/shors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/shors/shors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:29.205947 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/simons/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/simons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-26 16:05:18.000000 amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/simons/simons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.921621 amazon-braket-algorithm-library-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-08-03 16:04:42.921621 amazon-braket-algorithm-library-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-03 16:04:42.921621 amazon-braket-algorithm-library-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.905621 amazon-braket-algorithm-library-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.913621 amazon-braket-algorithm-library-1.4.1/src/amazon_braket_algorithm_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-08-03 16:04:42.000000 amazon-braket-algorithm-library-1.4.1/src/amazon_braket_algorithm_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-03 16:04:42.000000 amazon-braket-algorithm-library-1.4.1/src/amazon_braket_algorithm_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:04:42.000000 amazon-braket-algorithm-library-1.4.1/src/amazon_braket_algorithm_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-03 16:04:42.000000 amazon-braket-algorithm-library-1.4.1/src/amazon_braket_algorithm_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 16:04:42.000000 amazon-braket-algorithm-library-1.4.1/src/amazon_braket_algorithm_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.909621 amazon-braket-algorithm-library-1.4.1/src/braket/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.913621 amazon-braket-algorithm-library-1.4.1/src/braket/_algos/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/_algos/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.913621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.913621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.917621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/bells_inequality/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/bells_inequality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/bells_inequality/bells_inequality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.917621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/bernstein_vazirani/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/bernstein_vazirani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/bernstein_vazirani/bernstein_vazirani.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.917621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/chsh_inequality/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/chsh_inequality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/chsh_inequality/chsh_inequality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.917621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/deutsch_jozsa/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/deutsch_jozsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/deutsch_jozsa/deutsch_jozsa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.917621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/grovers_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/grovers_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/grovers_search/grovers_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.917621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/qc_qmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/qc_qmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/qc_qmc/classical_qmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/qc_qmc/qc_qmc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.921621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_approximate_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_approximate_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_approximate_optimization/quantum_approximate_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.921621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_circuit_born_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_circuit_born_machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_circuit_born_machine/qcbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.921621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_fourier_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_fourier_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_fourier_transform/quantum_fourier_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.921621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_phase_estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_phase_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_phase_estimation/quantum_phase_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.921621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_walk/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_walk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_walk/quantum_walk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.921621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/shors/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/shors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/shors/shors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:42.921621 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/simons/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/simons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-08-03 16:04:32.000000 amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/simons/simons.py
```

### Comparing `amazon-braket-algorithm-library-1.4.0/LICENSE` & `amazon-braket-algorithm-library-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/PKG-INFO` & `amazon-braket-algorithm-library-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-algorithm-library
-Version: 1.4.0
+Version: 1.4.1
 Summary: An open source library of quantum computing algorithms implemented on Amazon Braket
 Home-page: https://github.com/aws-samples/amazon-braket-algorithm-library
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `amazon-braket-algorithm-library-1.4.0/README.md` & `amazon-braket-algorithm-library-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/setup.py` & `amazon-braket-algorithm-library-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/amazon_braket_algorithm_library.egg-info/PKG-INFO` & `amazon-braket-algorithm-library-1.4.1/src/amazon_braket_algorithm_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-algorithm-library
-Version: 1.4.0
+Version: 1.4.1
 Summary: An open source library of quantum computing algorithms implemented on Amazon Braket
 Home-page: https://github.com/aws-samples/amazon-braket-algorithm-library
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `amazon-braket-algorithm-library-1.4.0/src/amazon_braket_algorithm_library.egg-info/SOURCES.txt` & `amazon-braket-algorithm-library-1.4.1/src/amazon_braket_algorithm_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/_algos/_version.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/_algos/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # language governing permissions and limitations under the License.
 
 """Version information.
 
 Version number (major.minor.patch[-label])
 """
 
-__version__ = "1.4.0"
+__version__ = "1.4.1"
```

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/bells_inequality/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/bells_inequality/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/bells_inequality/bells_inequality.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/bells_inequality/bells_inequality.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/bernstein_vazirani/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/bernstein_vazirani/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/bernstein_vazirani/bernstein_vazirani.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/bernstein_vazirani/bernstein_vazirani.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/chsh_inequality/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/chsh_inequality/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/chsh_inequality/chsh_inequality.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/chsh_inequality/chsh_inequality.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/deutsch_jozsa/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/deutsch_jozsa/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/deutsch_jozsa/deutsch_jozsa.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/deutsch_jozsa/deutsch_jozsa.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/grovers_search/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/grovers_search/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/grovers_search/grovers_search.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/grovers_search/grovers_search.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/qc_qmc/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/qc_qmc/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/qc_qmc/classical_qmc.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/qc_qmc/classical_qmc.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/qc_qmc/qc_qmc.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/qc_qmc/qc_qmc.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_approximate_optimization/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_approximate_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_approximate_optimization/quantum_approximate_optimization.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_approximate_optimization/quantum_approximate_optimization.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_circuit_born_machine/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_circuit_born_machine/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_circuit_born_machine/qcbm.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_circuit_born_machine/qcbm.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_fourier_transform/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_fourier_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_fourier_transform/quantum_fourier_transform.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_fourier_transform/quantum_fourier_transform.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_phase_estimation/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_phase_estimation/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_phase_estimation/quantum_phase_estimation.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_phase_estimation/quantum_phase_estimation.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_walk/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_walk/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/quantum_walk/quantum_walk.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/quantum_walk/quantum_walk.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/shors/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/shors/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/shors/shors.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/shors/shors.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/simons/__init__.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/simons/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.0/src/braket/experimental/algorithms/simons/simons.py` & `amazon-braket-algorithm-library-1.4.1/src/braket/experimental/algorithms/simons/simons.py`

 * *Files identical despite different names*

