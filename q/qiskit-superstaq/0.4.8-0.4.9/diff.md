# Comparing `tmp/qiskit-superstaq-0.4.8.tar.gz` & `tmp/qiskit-superstaq-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-superstaq-0.4.8.tar", last modified: Fri Jul 28 17:44:28 2023, max compression
+gzip compressed data, was "qiskit-superstaq-0.4.9.tar", last modified: Fri Jul 28 21:48:25 2023, max compression
```

## Comparing `qiskit-superstaq-0.4.8.tar` & `qiskit-superstaq-0.4.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:28.480668 qiskit-superstaq-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-28 17:44:28.480668 qiskit-superstaq-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/example-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:28.480668 qiskit-superstaq-0.4.8/qiskit_superstaq/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/_version_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/compiler_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/compiler_output_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/custom_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/custom_gates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/daily_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_job_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20716 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    16465 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_provider_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/validation_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:28.480668 qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-28 17:44:28.000000 qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-28 17:44:28.000000 qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:44:28.000000 qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-28 17:44:28.000000 qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 17:44:28.000000 qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:44:28.480668 qiskit-superstaq-0.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:48:25.995102 qiskit-superstaq-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-28 21:48:25.995102 qiskit-superstaq-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/example-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:48:25.995102 qiskit-superstaq-0.4.9/qiskit_superstaq/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/_version_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/compiler_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/compiler_output_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/custom_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/custom_gates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/daily_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/superstaq_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/superstaq_backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/superstaq_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/superstaq_job_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20716 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/superstaq_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16465 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/superstaq_provider_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/qiskit_superstaq/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:48:25.995102 qiskit-superstaq-0.4.9/qiskit_superstaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-28 21:48:25.000000 qiskit-superstaq-0.4.9/qiskit_superstaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-28 21:48:25.000000 qiskit-superstaq-0.4.9/qiskit_superstaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 21:48:25.000000 qiskit-superstaq-0.4.9/qiskit_superstaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-28 21:48:25.000000 qiskit-superstaq-0.4.9/qiskit_superstaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 21:48:25.000000 qiskit-superstaq-0.4.9/qiskit_superstaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-28 21:47:42.000000 qiskit-superstaq-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 21:48:25.995102 qiskit-superstaq-0.4.9/setup.cfg
```

### Comparing `qiskit-superstaq-0.4.8/PKG-INFO` & `qiskit-superstaq-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-superstaq
-Version: 0.4.8
+Version: 0.4.9
 Summary: The Qiskit module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache 2
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `qiskit-superstaq-0.4.8/README.md` & `qiskit-superstaq-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/pyproject.toml` & `qiskit-superstaq-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/__init__.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/compiler_output.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/compiler_output.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/compiler_output_test.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/compiler_output_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/custom_gates.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/custom_gates.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/custom_gates_test.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/custom_gates_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/daily_integration_test.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/daily_integration_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,20 +142,21 @@
 
     assert resource_estimates == [resource_estimate, ResourceEstimate(1, 2, 3)]
 
 
 def test_qscout_compile(provider: qss.SuperstaqProvider) -> None:
     circuit = qiskit.QuantumCircuit(1)
     circuit.h(0)
-    expected = qiskit.QuantumCircuit(2)
-    expected.r(np.pi / 2, -np.pi / 2, 0)
-    expected.z(0)
-    assert provider.qscout_compile(circuit).circuit == expected
-    assert provider.qscout_compile([circuit]).circuits == [expected]
-    assert provider.qscout_compile([circuit, circuit]).circuits == [expected, expected]
+
+    compiled_circuit = provider.qscout_compile(circuit).circuit
+    assert isinstance(compiled_circuit, qiskit.QuantumCircuit)
+    assert qiskit.quantum_info.Operator(compiled_circuit) == qiskit.quantum_info.Operator(circuit)
+
+    assert provider.qscout_compile([circuit]).circuits == [compiled_circuit]
+    assert provider.qscout_compile([circuit, circuit]).circuits == 2 * [compiled_circuit]
 
 
 def test_qscout_compile_swap_mirror(provider: qss.SuperstaqProvider) -> None:
     qc = qiskit.QuantumCircuit(2)
     qc.swap(0, 1)
 
     out_qc_swap = qiskit.QuantumCircuit(2)
```

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/serialization.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/serialization_test.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/serialization_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_backend.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/superstaq_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_backend_test.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/superstaq_backend_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_job.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/superstaq_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_job_test.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/superstaq_job_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_provider.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/superstaq_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_provider_test.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/superstaq_provider_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/validation.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/validation.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq/validation_test.py` & `qiskit-superstaq-0.4.9/qiskit_superstaq/validation_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/PKG-INFO` & `qiskit-superstaq-0.4.9/qiskit_superstaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-superstaq
-Version: 0.4.8
+Version: 0.4.9
 Summary: The Qiskit module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache 2
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/SOURCES.txt` & `qiskit-superstaq-0.4.9/qiskit_superstaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

