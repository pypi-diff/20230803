# Comparing `tmp/Supermarq-0.4.8.tar.gz` & `tmp/Supermarq-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Supermarq-0.4.8.tar", last modified: Fri Jul 28 17:45:06 2023, max compression
+gzip compressed data, was "Supermarq-0.4.9.tar", last modified: Fri Jul 28 21:49:07 2023, max compression
```

## Comparing `Supermarq-0.4.8.tar` & `Supermarq-0.4.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:45:06.641135 Supermarq-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 17:45:06.641135 Supermarq-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-28 17:43:49.000000 Supermarq-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:45:06.633135 Supermarq-0.4.8/Supermarq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 17:45:06.000000 Supermarq-0.4.8/Supermarq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-28 17:45:06.000000 Supermarq-0.4.8/Supermarq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:45:06.000000 Supermarq-0.4.8/Supermarq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-28 17:45:06.000000 Supermarq-0.4.8/Supermarq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 17:45:06.000000 Supermarq-0.4.8/Supermarq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 17:43:49.000000 Supermarq-0.4.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-28 17:43:49.000000 Supermarq-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 17:43:49.000000 Supermarq-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:45:06.641135 Supermarq-0.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:45:06.637135 Supermarq-0.4.8/supermarq/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/_version_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmark_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:45:06.641135 Supermarq-0.4.8/supermarq/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/bit_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/bit_code_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/ghz.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/ghz_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/hamiltonian_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/hamiltonian_simulation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/mermin_bell.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/mermin_bell_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/phase_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/phase_code_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/qaoa_fermionic_swap_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/qaoa_fermionic_swap_proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/qaoa_vanilla_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/qaoa_vanilla_proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/vqe_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/benchmarks/vqe_proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/converters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/features_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13156 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/plotting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/run_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-28 17:43:49.000000 Supermarq-0.4.8/supermarq/stabilizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:49:07.763472 Supermarq-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 21:49:07.763472 Supermarq-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-28 21:47:42.000000 Supermarq-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:49:07.759472 Supermarq-0.4.9/Supermarq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 21:49:07.000000 Supermarq-0.4.9/Supermarq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-28 21:49:07.000000 Supermarq-0.4.9/Supermarq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 21:49:07.000000 Supermarq-0.4.9/Supermarq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-28 21:49:07.000000 Supermarq-0.4.9/Supermarq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 21:49:07.000000 Supermarq-0.4.9/Supermarq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 21:47:42.000000 Supermarq-0.4.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-28 21:47:43.000000 Supermarq-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 21:47:43.000000 Supermarq-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 21:49:07.763472 Supermarq-0.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:49:07.759472 Supermarq-0.4.9/supermarq/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 21:47:42.000000 Supermarq-0.4.9/supermarq/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/_version_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmark_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:49:07.763472 Supermarq-0.4.9/supermarq/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/bit_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/bit_code_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/ghz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/ghz_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/hamiltonian_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/hamiltonian_simulation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/mermin_bell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/mermin_bell_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/phase_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/phase_code_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/qaoa_fermionic_swap_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/qaoa_fermionic_swap_proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/qaoa_vanilla_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/qaoa_vanilla_proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/vqe_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/benchmarks/vqe_proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/features_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13156 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/plotting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/run_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-28 21:47:43.000000 Supermarq-0.4.9/supermarq/stabilizers.py
```

### Comparing `Supermarq-0.4.8/PKG-INFO` & `Supermarq-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Supermarq
-Version: 0.4.8
+Version: 0.4.9
 Summary: Supermarq is a scalable, application-centric quantum benchmarking suite.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache 2
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `Supermarq-0.4.8/README.md` & `Supermarq-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/Supermarq.egg-info/PKG-INFO` & `Supermarq-0.4.9/Supermarq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Supermarq
-Version: 0.4.8
+Version: 0.4.9
 Summary: Supermarq is a scalable, application-centric quantum benchmarking suite.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache 2
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `Supermarq-0.4.8/Supermarq.egg-info/SOURCES.txt` & `Supermarq-0.4.9/Supermarq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/pyproject.toml` & `Supermarq-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/__init__.py` & `Supermarq-0.4.9/supermarq/__init__.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmark.py` & `Supermarq-0.4.9/supermarq/benchmark.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmark_test.py` & `Supermarq-0.4.9/supermarq/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmarks/bit_code.py` & `Supermarq-0.4.9/supermarq/benchmarks/bit_code.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmarks/bit_code_test.py` & `Supermarq-0.4.9/supermarq/benchmarks/bit_code_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmarks/ghz.py` & `Supermarq-0.4.9/supermarq/benchmarks/ghz.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmarks/hamiltonian_simulation.py` & `Supermarq-0.4.9/supermarq/benchmarks/hamiltonian_simulation.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmarks/hamiltonian_simulation_test.py` & `Supermarq-0.4.9/supermarq/benchmarks/hamiltonian_simulation_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmarks/mermin_bell.py` & `Supermarq-0.4.9/supermarq/benchmarks/mermin_bell.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmarks/mermin_bell_test.py` & `Supermarq-0.4.9/supermarq/benchmarks/mermin_bell_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmarks/phase_code.py` & `Supermarq-0.4.9/supermarq/benchmarks/phase_code.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmarks/phase_code_test.py` & `Supermarq-0.4.9/supermarq/benchmarks/phase_code_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmarks/qaoa_fermionic_swap_proxy.py` & `Supermarq-0.4.9/supermarq/benchmarks/qaoa_fermionic_swap_proxy.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmarks/qaoa_fermionic_swap_proxy_test.py` & `Supermarq-0.4.9/supermarq/benchmarks/qaoa_fermionic_swap_proxy_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmarks/qaoa_vanilla_proxy.py` & `Supermarq-0.4.9/supermarq/benchmarks/qaoa_vanilla_proxy.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmarks/qaoa_vanilla_proxy_test.py` & `Supermarq-0.4.9/supermarq/benchmarks/qaoa_vanilla_proxy_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/benchmarks/vqe_proxy.py` & `Supermarq-0.4.9/supermarq/benchmarks/vqe_proxy.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/converters.py` & `Supermarq-0.4.9/supermarq/converters.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/features.py` & `Supermarq-0.4.9/supermarq/features.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/features_test.py` & `Supermarq-0.4.9/supermarq/features_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/plotting.py` & `Supermarq-0.4.9/supermarq/plotting.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/plotting_test.py` & `Supermarq-0.4.9/supermarq/plotting_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/run_benchmarks.py` & `Supermarq-0.4.9/supermarq/run_benchmarks.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/simulation.py` & `Supermarq-0.4.9/supermarq/simulation.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.4.8/supermarq/stabilizers.py` & `Supermarq-0.4.9/supermarq/stabilizers.py`

 * *Files identical despite different names*

