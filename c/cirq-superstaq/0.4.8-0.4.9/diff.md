# Comparing `tmp/cirq-superstaq-0.4.8.tar.gz` & `tmp/cirq-superstaq-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirq-superstaq-0.4.8.tar", last modified: Fri Jul 28 17:44:46 2023, max compression
+gzip compressed data, was "cirq-superstaq-0.4.9.tar", last modified: Fri Jul 28 21:48:46 2023, max compression
```

## Comparing `cirq-superstaq-0.4.8.tar` & `cirq-superstaq-0.4.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:46.920900 cirq-superstaq-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-28 17:44:46.920900 cirq-superstaq-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:46.916900 cirq-superstaq-0.4.8/cirq_superstaq/
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/_version_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/compiler_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/compiler_output_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/daily_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/job_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:46.920900 cirq-superstaq-0.4.8/cirq_superstaq/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35310 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/ops/qubit_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)    38578 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/ops/qubit_gates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/ops/qudit_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16989 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/ops/qudit_gates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    33059 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    24505 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/validation_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:46.916900 cirq-superstaq-0.4.8/cirq_superstaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-28 17:44:46.000000 cirq-superstaq-0.4.8/cirq_superstaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 17:44:46.000000 cirq-superstaq-0.4.8/cirq_superstaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:44:46.000000 cirq-superstaq-0.4.8/cirq_superstaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-28 17:44:46.000000 cirq-superstaq-0.4.8/cirq_superstaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 17:44:46.000000 cirq-superstaq-0.4.8/cirq_superstaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/example-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:44:46.920900 cirq-superstaq-0.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:48:46.847288 cirq-superstaq-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-28 21:48:46.847288 cirq-superstaq-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:48:46.847288 cirq-superstaq-0.4.9/cirq_superstaq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/_version_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/compiler_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/compiler_output_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/daily_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/job_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:48:46.847288 cirq-superstaq-0.4.9/cirq_superstaq/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35310 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/ops/qubit_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38578 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/ops/qubit_gates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/ops/qudit_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16989 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/ops/qudit_gates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33059 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24505 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/cirq_superstaq/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:48:46.847288 cirq-superstaq-0.4.9/cirq_superstaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-28 21:48:46.000000 cirq-superstaq-0.4.9/cirq_superstaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 21:48:46.000000 cirq-superstaq-0.4.9/cirq_superstaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 21:48:46.000000 cirq-superstaq-0.4.9/cirq_superstaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-28 21:48:46.000000 cirq-superstaq-0.4.9/cirq_superstaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 21:48:46.000000 cirq-superstaq-0.4.9/cirq_superstaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/example-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 21:47:42.000000 cirq-superstaq-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 21:48:46.847288 cirq-superstaq-0.4.9/setup.cfg
```

### Comparing `cirq-superstaq-0.4.8/PKG-INFO` & `cirq-superstaq-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirq-superstaq
-Version: 0.4.8
+Version: 0.4.9
 Summary: The Cirq module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache 2
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `cirq-superstaq-0.4.8/README.md` & `cirq-superstaq-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/__init__.py` & `cirq-superstaq-0.4.9/cirq_superstaq/__init__.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/compiler_output.py` & `cirq-superstaq-0.4.9/cirq_superstaq/compiler_output.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/compiler_output_test.py` & `cirq-superstaq-0.4.9/cirq_superstaq/compiler_output_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/daily_integration_test.py` & `cirq-superstaq-0.4.9/cirq_superstaq/daily_integration_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,27 +153,25 @@
     assert "ibmq_qasm_simulator" in result["compile-and-run"]
     assert "aqt_keysight_qpu" in result["compile-only"]
 
 
 def test_qscout_compile(service: css.Service) -> None:
     q0, q1 = cirq.LineQubit.range(2)
     circuit = cirq.Circuit(cirq.H(q0), cirq.measure(q0))
-    compiled_circuit = cirq.Circuit(
-        cirq.PhasedXPowGate(phase_exponent=-0.5, exponent=0.5).on(q0),
-        cirq.Z(q0) ** -1.0,
-        cirq.measure(q0),
-    )
 
     out = service.qscout_compile(circuit)
     cirq.testing.assert_circuits_with_terminal_measurements_are_equivalent(
-        out.circuit, compiled_circuit, atol=1e-08
+        out.circuit, circuit, atol=1e-08
     )
     assert isinstance(out.jaqal_program, str)
     assert "measure_all" in out.jaqal_program
 
+    assert service.qscout_compile([circuit]).circuits == [out.circuit]
+    assert service.qscout_compile([circuit, circuit]).circuits == [out.circuit, out.circuit]
+
     cx_circuit = cirq.Circuit(cirq.H(q0), cirq.CX(q0, q1), cirq.measure(q0, q1))
     out = service.qscout_compile([cx_circuit])
     assert isinstance(out.circuits[0], cirq.Circuit)
     cirq.testing.assert_circuits_with_terminal_measurements_are_equivalent(
         out.circuits[0], cx_circuit, atol=1e-08
     )
     assert isinstance(out.jaqal_programs, list)
```

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/job.py` & `cirq-superstaq-0.4.9/cirq_superstaq/job.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/job_test.py` & `cirq-superstaq-0.4.9/cirq_superstaq/job_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/ops/__init__.py` & `cirq-superstaq-0.4.9/cirq_superstaq/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/ops/qubit_gates.py` & `cirq-superstaq-0.4.9/cirq_superstaq/ops/qubit_gates.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/ops/qubit_gates_test.py` & `cirq-superstaq-0.4.9/cirq_superstaq/ops/qubit_gates_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/ops/qudit_gates.py` & `cirq-superstaq-0.4.9/cirq_superstaq/ops/qudit_gates.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/ops/qudit_gates_test.py` & `cirq-superstaq-0.4.9/cirq_superstaq/ops/qudit_gates_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/sampler.py` & `cirq-superstaq-0.4.9/cirq_superstaq/sampler.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/serialization.py` & `cirq-superstaq-0.4.9/cirq_superstaq/serialization.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/serialization_test.py` & `cirq-superstaq-0.4.9/cirq_superstaq/serialization_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/service.py` & `cirq-superstaq-0.4.9/cirq_superstaq/service.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/service_test.py` & `cirq-superstaq-0.4.9/cirq_superstaq/service_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/validation.py` & `cirq-superstaq-0.4.9/cirq_superstaq/validation.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq/validation_test.py` & `cirq-superstaq-0.4.9/cirq_superstaq/validation_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq.egg-info/PKG-INFO` & `cirq-superstaq-0.4.9/cirq_superstaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirq-superstaq
-Version: 0.4.8
+Version: 0.4.9
 Summary: The Cirq module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache 2
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `cirq-superstaq-0.4.8/cirq_superstaq.egg-info/SOURCES.txt` & `cirq-superstaq-0.4.9/cirq_superstaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.8/pyproject.toml` & `cirq-superstaq-0.4.9/pyproject.toml`

 * *Files identical despite different names*

