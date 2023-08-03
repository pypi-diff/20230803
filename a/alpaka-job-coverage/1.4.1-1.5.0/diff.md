# Comparing `tmp/alpaka-job-coverage-1.4.1.tar.gz` & `tmp/alpaka-job-coverage-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaka-job-coverage-1.4.1.tar", last modified: Wed Aug  2 11:12:32 2023, max compression
+gzip compressed data, was "alpaka-job-coverage-1.5.0.tar", last modified: Thu Aug  3 12:16:01 2023, max compression
```

## Comparing `alpaka-job-coverage-1.4.1.tar` & `alpaka-job-coverage-1.5.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:12:32.565951 alpaka-job-coverage-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-02 11:12:32.565951 alpaka-job-coverage-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 11:12:32.565951 alpaka-job-coverage-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:12:32.557951 alpaka-job-coverage-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:12:32.561951 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_backend_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_compiler_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_compiler_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_software_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/main_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12111 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:12:32.561951 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-02 11:12:32.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-02 11:12:32.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:12:32.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-02 11:12:32.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-02 11:12:32.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 11:12:32.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:12:32.565951 alpaka-job-coverage-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/tests/test_compiler_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    42016 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/tests/test_cuda_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/tests/test_hipcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/tests/test_single_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:16:01.181329 alpaka-job-coverage-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-03 12:16:01.181329 alpaka-job-coverage-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:16:01.181329 alpaka-job-coverage-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:16:01.177329 alpaka-job-coverage-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:16:01.181329 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_backend_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_compiler_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_compiler_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_software_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/main_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12117 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:16:01.181329 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-03 12:16:01.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-03 12:16:01.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:16:01.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 12:16:01.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-03 12:16:01.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-03 12:16:01.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:16:01.181329 alpaka-job-coverage-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/tests/test_compiler_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42016 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/tests/test_cuda_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/tests/test_hipcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/tests/test_icpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/tests/test_single_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/version.txt
```

### Comparing `alpaka-job-coverage-1.4.1/LICENSE` & `alpaka-job-coverage-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.1/PKG-INFO` & `alpaka-job-coverage-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.4.1
+Version: 1.5.0
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.4.1/README.md` & `alpaka-job-coverage-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.1/setup.py` & `alpaka-job-coverage-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_backend_version.py` & `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_backend_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -196,9 +196,30 @@
         if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER):
             reason(
                 output,
                 "if hipcc is the device compiler and the HIP back-end is enabled, "
                 "it is not allowed to enable the CUDA back-end",
             )
             return False
+        
+    ###########################
+    ## icpx device compiler
+    ###########################
 
+    # Don't use icpx for the CUDA and HIP back-ends
+    if row_check_name(row, DEVICE_COMPILER, "==", ICPX):
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER):
+            reason(
+                output,
+                "if icpx is the device compiler it is not allowed to enable the CUDA "
+                "back-end",
+            )
+            return False
+        
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER):
+            reason(
+                output,
+                "if icpx is the device compiler it is not allowed to enable the HIP "
+                "back-end",
+            )
+            return False
     return True
```

### Comparing `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_compiler_name.py` & `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_compiler_name.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_compiler_version.py` & `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_compiler_version.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_software_dependency.py` & `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_software_dependency.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/globals.py` & `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/globals.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,35 +14,38 @@
 
 # name of the used compilers
 GCC: str = "gcc"
 CLANG: str = "clang"
 NVCC: str = "nvcc"
 CLANG_CUDA: str = "clang-cuda"
 HIPCC: str = "hipcc"
+ICPX: str = "icpx"
 
 # alpaka backend names
 ALPAKA_ACC_CPU_B_SEQ_T_SEQ_ENABLE: str = "alpaka_ACC_CPU_B_SEQ_T_SEQ_ENABLE"
 ALPAKA_ACC_CPU_B_SEQ_T_THREADS_ENABLE: str = "alpaka_ACC_CPU_B_SEQ_T_THREADS_ENABLE"
 ALPAKA_ACC_CPU_B_SEQ_T_FIBERS_ENABLE: str = "alpaka_ACC_CPU_B_SEQ_T_FIBERS_ENABLE"
 ALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLE: str = "alpaka_ACC_CPU_B_TBB_T_SEQ_ENABLE"
 ALPAKA_ACC_CPU_B_OMP2_T_SEQ_ENABLE: str = "alpaka_ACC_CPU_B_OMP2_T_SEQ_ENABLE"
 ALPAKA_ACC_CPU_B_SEQ_T_OMP2_ENABLE: str = "alpaka_ACC_CPU_B_SEQ_T_OMP2_ENABLE"
 ALPAKA_ACC_ANY_BT_OMP5_ENABLE: str = "alpaka_ACC_ANY_BT_OMP5_ENABLE"
 ALPAKA_ACC_GPU_CUDA_ENABLE: str = "alpaka_ACC_GPU_CUDA_ENABLE"
 ALPAKA_ACC_GPU_HIP_ENABLE: str = "alpaka_ACC_GPU_HIP_ENABLE"
+ALPAKA_ACC_SYCL_ENABLE: str = "alpaka_ACC_SYCL_ENABLE"
 BACKENDS_LIST: List[str] = [
     ALPAKA_ACC_CPU_B_SEQ_T_SEQ_ENABLE,
     ALPAKA_ACC_CPU_B_SEQ_T_THREADS_ENABLE,
     ALPAKA_ACC_CPU_B_SEQ_T_FIBERS_ENABLE,
     ALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLE,
     ALPAKA_ACC_CPU_B_OMP2_T_SEQ_ENABLE,
     ALPAKA_ACC_CPU_B_SEQ_T_OMP2_ENABLE,
     ALPAKA_ACC_ANY_BT_OMP5_ENABLE,
     ALPAKA_ACC_GPU_CUDA_ENABLE,
     ALPAKA_ACC_GPU_HIP_ENABLE,
+    ALPAKA_ACC_SYCL_ENABLE,
 ]
 
 # if want to use version comparison functions from util.py, you need to use ON_VER and OFF_VER
 ON: str = "on"
 OFF: str = "off"
 
 # backend states
```

### Comparing `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/main_functions.py` & `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/main_functions.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/util.py` & `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/util.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/validate.py` & `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         arguments (Dict[str, str]): Key needs to be HOST_COMPILER or
         DEVICE_COMPILER and values describes the compiler name and version.
 
     Returns:
         Dict[str, Tuple[str, str]]: Returns parsed compiler name and version
     """
     validated_args = {}
-    known_compiler = [GCC, CLANG, NVCC, CLANG_CUDA, HIPCC]
+    known_compiler = [GCC, CLANG, NVCC, CLANG_CUDA, HIPCC, ICPX]
 
     for parameter_name, parameter in arguments.items():
         if "@" not in parameter:
             exit_error(f"@ is missing in {parameter_name}={parameter}")
 
         splitted_name_version = parameter.split("@", 1)
         name = splitted_name_version[0]
```

### Comparing `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/versions.py` & `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/versions.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         "11.7",
         "11.8",
         "12.0",
         "12.1",
         "12.2",
     ],
     HIPCC: ["5.0", "5.1", "5.2", "5.3", "5.4", "5.5"],
+    ICPX: ["2023.1", "2023.2"],
     UBUNTU: ["18.04", "20.04"],
     CMAKE: ["3.18", "3.19", "3.20", "3.21", "3.22", "3.23", "3.24", "3.25", "3.26"],
     BOOST: [
         "1.74.0",
         "1.75.0",
         "1.76.0",
         "1.77.0",
```

### Comparing `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/PKG-INFO` & `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.4.1
+Version: 1.5.0
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/SOURCES.txt` & `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,10 +19,11 @@
 src/alpaka_job_coverage.egg-info/dependency_links.txt
 src/alpaka_job_coverage.egg-info/entry_points.txt
 src/alpaka_job_coverage.egg-info/requires.txt
 src/alpaka_job_coverage.egg-info/top_level.txt
 tests/test_compiler_names.py
 tests/test_cuda_sdk.py
 tests/test_hipcc.py
+tests/test_icpx.py
 tests/test_single_rules.py
 tests/test_util.py
 tests/test_versions.py
```

### Comparing `alpaka-job-coverage-1.4.1/tests/test_compiler_names.py` & `alpaka-job-coverage-1.5.0/tests/test_compiler_names.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,21 +20,25 @@
         param_map = {}
 
     def test_same_host_device_compiler(self):
         valid_combs = [
             [(GCC, "0"), (GCC, "0")],
             [(CLANG, "0"), (CLANG, "0")],
             [(HIPCC, "0"), (HIPCC, "0")],
+            [(ICPX, "0"), (ICPX, "0")],
         ]
 
         for comb in valid_combs:
             self.assertTrue(general_compiler_filter_typed(comb))
 
         invalid_combs = [
             [(GCC, "0"), (CLANG, "0")],
             [(GCC, "0"), (CLANG, "0")],
             [(GCC, "0"), (HIPCC, "0")],
             [(HIPCC, "0"), (CLANG, "0")],
+            [(GCC, "0"), (ICPX, "0")],
+            [(CLANG, "0"), (ICPX, "0")],
+            [(ICPX, "0"), (CLANG, "0")]
         ]
 
         for comb in invalid_combs:
             self.assertFalse(general_compiler_filter_typed(comb))
```

### Comparing `alpaka-job-coverage-1.4.1/tests/test_cuda_sdk.py` & `alpaka-job-coverage-1.5.0/tests/test_cuda_sdk.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.1/tests/test_hipcc.py` & `alpaka-job-coverage-1.5.0/tests/test_hipcc.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.1/tests/test_single_rules.py` & `alpaka-job-coverage-1.5.0/tests/test_single_rules.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.1/tests/test_util.py` & `alpaka-job-coverage-1.5.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.1/tests/test_versions.py` & `alpaka-job-coverage-1.5.0/tests/test_versions.py`

 * *Files identical despite different names*

