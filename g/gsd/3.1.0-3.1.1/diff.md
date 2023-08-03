# Comparing `tmp/gsd-3.1.0.tar.gz` & `tmp/gsd-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsd-3.1.0.tar", last modified: Fri Jul 28 17:21:51 2023, max compression
+gzip compressed data, was "gsd-3.1.1.tar", last modified: Thu Aug  3 19:07:31 2023, max compression
```

## Comparing `gsd-3.1.0.tar` & `gsd-3.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:21:51.723649 gsd-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-07-28 17:21:36.000000 gsd-3.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-28 17:21:36.000000 gsd-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-28 17:21:36.000000 gsd-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-28 17:21:51.723649 gsd-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-28 17:21:36.000000 gsd-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:21:51.723649 gsd-3.1.0/gsd/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   940948 2023-07-28 17:21:51.000000 gsd-3.1.0/gsd/fl.c
--rw-r--r--   0 runner    (1001) docker     (123)    37102 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/fl.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    73766 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/gsd.c
--rw-r--r--   0 runner    (1001) docker     (123)    22342 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/gsd.h
--rw-r--r--   0 runner    (1001) docker     (123)    45581 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/hoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/libgsd.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/pygsd.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/pytest_plugin_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:21:51.723649 gsd-3.1.0/gsd/test/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/test/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/test/test_fl.py
--rw-r--r--   0 runner    (1001) docker     (123)    72428 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/test/test_gsd_v1.gsd
--rw-r--r--   0 runner    (1001) docker     (123)    34722 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/test/test_hoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/test/test_largefile.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-28 17:21:36.000000 gsd-3.1.0/gsd/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:21:51.723649 gsd-3.1.0/gsd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-28 17:21:51.000000 gsd-3.1.0/gsd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-28 17:21:51.000000 gsd-3.1.0/gsd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:21:51.000000 gsd-3.1.0/gsd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 17:21:51.000000 gsd-3.1.0/gsd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 17:21:51.000000 gsd-3.1.0/gsd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-28 17:21:51.000000 gsd-3.1.0/gsd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-28 17:21:36.000000 gsd-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-28 17:21:51.723649 gsd-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-28 17:21:36.000000 gsd-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:07:31.743453 gsd-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10659 2023-08-03 19:07:16.000000 gsd-3.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-08-03 19:07:16.000000 gsd-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-03 19:07:16.000000 gsd-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-03 19:07:31.743453 gsd-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-08-03 19:07:16.000000 gsd-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:07:31.739454 gsd-3.1.1/gsd/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   940948 2023-08-03 19:07:31.000000 gsd-3.1.1/gsd/fl.c
+-rw-r--r--   0 runner    (1001) docker     (123)    37102 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/fl.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    73994 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/gsd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22342 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/gsd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45581 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/hoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/libgsd.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/pygsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/pytest_plugin_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:07:31.743453 gsd-3.1.1/gsd/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/test/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    38005 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/test/test_fl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72428 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/test/test_gsd_v1.gsd
+-rw-r--r--   0 runner    (1001) docker     (123)    34722 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/test/test_hoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/test/test_largefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-03 19:07:16.000000 gsd-3.1.1/gsd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:07:31.743453 gsd-3.1.1/gsd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-03 19:07:31.000000 gsd-3.1.1/gsd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-03 19:07:31.000000 gsd-3.1.1/gsd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:07:31.000000 gsd-3.1.1/gsd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 19:07:31.000000 gsd-3.1.1/gsd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 19:07:31.000000 gsd-3.1.1/gsd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-03 19:07:31.000000 gsd-3.1.1/gsd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-08-03 19:07:16.000000 gsd-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-03 19:07:31.743453 gsd-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-03 19:07:16.000000 gsd-3.1.1/setup.py
```

### Comparing `gsd-3.1.0/CHANGELOG.rst` & `gsd-3.1.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 
 `GSD <https://github.com/glotzerlab/gsd>`_ releases follow `semantic versioning
 <https://semver.org/>`_.
 
 3.x
 ---
 
+3.1.1 (2023-08-03)
+^^^^^^^^^^^^^^^^^^
+
+*Fixed:*
+
+* Raise a ``FileExistsError`` when opening a file that already exists with ``mode = 'x'``.
+
 3.1.0 (2023-07-28)
 ^^^^^^^^^^^^^^^^^^
 
 *Fixed:*
 
 * ``hoomd.read_log`` no longer triggers a numpy deprecation warning.
```

### Comparing `gsd-3.1.0/LICENSE` & `gsd-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/PKG-INFO` & `gsd-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: gsd
-Version: 3.1.0
+Version: 3.1.1
 Summary: General simulation data file format.
 Author-email: "Joshua A. Anderson" <joaander@umich.edu>
 License: BSD-2-Clause
 Project-URL: Homepage, https://gsd.readthedocs.io
 Project-URL: Documentation, https://gsd.readthedocs.io
-Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v3.1.0/gsd-3.1.0.tar.gz
+Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v3.1.1/gsd-3.1.1.tar.gz
 Project-URL: Source, https://github.com/glotzerlab/gsd
 Project-URL: Issues, https://github.com/glotzerlab/gsd/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
```

### Comparing `gsd-3.1.0/README.md` & `gsd-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/gsd/__init__.py` & `gsd-3.1.1/gsd/__init__.py`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/gsd/__main__.py` & `gsd-3.1.1/gsd/__main__.py`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/gsd/fl.c` & `gsd-3.1.1/gsd/fl.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "gsd/gsd.h"
         ],
         "include_dirs": [
             "gsd",
-            "/tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/core/include"
+            "/tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/core/include"
         ],
         "name": "gsd.fl",
         "sources": [
             "gsd/fl.pyx",
             "gsd/gsd.c"
         ]
     },
@@ -1454,195 +1454,195 @@
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":746
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":756
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":759
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":759
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":766
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":766
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1672,42 +1672,42 @@
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_3gsd_2fl_GSDFile;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":770
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":770
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3837,261 +3837,261 @@
 #define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
 #define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
 #define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
 #define __pyx_codeobj__31 __pyx_mstate_global->__pyx_codeobj__31
 #define __pyx_codeobj__32 __pyx_mstate_global->__pyx_codeobj__32
 /* #### Code section: module_code ### */
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4100,29 +4100,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4133,15 +4133,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4150,29 +4150,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4183,15 +4183,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4200,29 +4200,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4233,15 +4233,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4250,29 +4250,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4283,15 +4283,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4300,29 +4300,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4333,212 +4333,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":793
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+    /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":795
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":795
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":977
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+    /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":978
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":978
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4554,15 +4554,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4570,68 +4570,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 984, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+    /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 985, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 986, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 986, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4639,15 +4639,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4662,15 +4662,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4686,15 +4686,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4702,68 +4702,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 990, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+    /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 991, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 992, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 992, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4771,15 +4771,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4794,15 +4794,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4818,15 +4818,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4834,68 +4834,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 996, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":997
+    /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":997
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 997, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+      /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 998, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 998, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4903,15 +4903,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4926,176 +4926,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
+/* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1052
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1052
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -14736,26 +14736,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-neg5g78n/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-5tt8duq4/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 992, __pyx_L1_error)
```

### Comparing `gsd-3.1.0/gsd/fl.pyx` & `gsd-3.1.1/gsd/fl.pyx`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/gsd/gsd.c` & `gsd-3.1.1/gsd/gsd.c`

 * *Files 0% similar despite different names*

```diff
@@ -1619,15 +1619,18 @@
 #endif
 
     // create the file
     int fd = gsd_open_file(fname,
                            O_RDWR | O_CREAT | O_TRUNC | extra_flags,
                            S_IRUSR | S_IWUSR | S_IRGRP | S_IWGRP);
     int retval = gsd_initialize_file(fd, application, schema, schema_version);
-    close(fd);
+    if (fd != -1)
+        {
+        close(fd);
+        }
     return retval;
     }
 
 int gsd_create_and_open(struct gsd_handle* handle,
                         const char* fname,
                         const char* application,
                         const char* schema,
@@ -1666,22 +1669,28 @@
     // create the file
     handle->fd = gsd_open_file(fname,
                                O_RDWR | O_CREAT | O_TRUNC | extra_flags,
                                S_IRUSR | S_IWUSR | S_IRGRP | S_IWGRP);
     int retval = gsd_initialize_file(handle->fd, application, schema, schema_version);
     if (retval != 0)
         {
-        close(handle->fd);
+        if (handle->fd != -1)
+            {
+            close(handle->fd);
+            }
         return retval;
         }
 
     retval = gsd_initialize_handle(handle);
     if (retval != 0)
         {
-        close(handle->fd);
+        if (handle->fd != -1)
+            {
+            close(handle->fd);
+            }
         }
     return retval;
     }
 
 int gsd_open(struct gsd_handle* handle, const char* fname, const enum gsd_open_flag flags)
     {
     // zero the handle
@@ -1708,15 +1717,18 @@
         handle->fd = gsd_open_file(fname, O_RDWR | extra_flags, 0);
         handle->open_flags = GSD_OPEN_APPEND;
         }
 
     int retval = gsd_initialize_handle(handle);
     if (retval != 0)
         {
-        close(handle->fd);
+        if (handle->fd != -1)
+            {
+            close(handle->fd);
+            }
         }
     return retval;
     }
 
 int gsd_truncate(struct gsd_handle* handle)
     {
     if (handle == NULL)
```

### Comparing `gsd-3.1.0/gsd/gsd.h` & `gsd-3.1.1/gsd/gsd.h`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/gsd/hoomd.py` & `gsd-3.1.1/gsd/hoomd.py`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/gsd/libgsd.pxd` & `gsd-3.1.1/gsd/libgsd.pxd`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/gsd/pygsd.py` & `gsd-3.1.1/gsd/pygsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from __future__ import division
 import logging
 import numpy
 import struct
 from collections import namedtuple
 import sys
 
-version = "3.1.0"
+version = "3.1.1"
 
 logger = logging.getLogger('gsd.pygsd')
 
 gsd_header = namedtuple(
     'gsd_header',
     'magic index_location index_allocated_entries '
     'namelist_location namelist_allocated_entries '
```

### Comparing `gsd-3.1.0/gsd/pytest_plugin_validate.py` & `gsd-3.1.1/gsd/pytest_plugin_validate.py`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/gsd/test/conftest.py` & `gsd-3.1.1/gsd/test/conftest.py`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/gsd/test/test_fl.py` & `gsd-3.1.1/gsd/test/test_fl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1026,7 +1026,18 @@
 
         assert f.index_entries_to_buffer > 0
         f.index_entries_to_buffer = 1024
         assert f.index_entries_to_buffer == 1024
 
         with pytest.raises(RuntimeError):
             f.index_entries_to_buffer = 0
+
+
+def test_file_exists_error():
+    """Test that IO errors throw the correct Python Excetion."""
+    with pytest.raises(FileExistsError):
+        with gsd.fl.open(name=test_path / 'test_gsd_v1.gsd',
+                         mode='x',
+                         application='test_gsd_v1',
+                         schema='none',
+                         schema_version=[1, 2]):
+            pass
```

### Comparing `gsd-3.1.0/gsd/test/test_gsd_v1.gsd` & `gsd-3.1.1/gsd/test/test_gsd_v1.gsd`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/gsd/test/test_hoomd.py` & `gsd-3.1.1/gsd/test/test_hoomd.py`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/gsd/test/test_largefile.py` & `gsd-3.1.1/gsd/test/test_largefile.py`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/gsd.egg-info/PKG-INFO` & `gsd-3.1.1/gsd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: gsd
-Version: 3.1.0
+Version: 3.1.1
 Summary: General simulation data file format.
 Author-email: "Joshua A. Anderson" <joaander@umich.edu>
 License: BSD-2-Clause
 Project-URL: Homepage, https://gsd.readthedocs.io
 Project-URL: Documentation, https://gsd.readthedocs.io
-Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v3.1.0/gsd-3.1.0.tar.gz
+Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v3.1.1/gsd-3.1.1.tar.gz
 Project-URL: Source, https://github.com/glotzerlab/gsd
 Project-URL: Issues, https://github.com/glotzerlab/gsd/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
```

### Comparing `gsd-3.1.0/gsd.egg-info/SOURCES.txt` & `gsd-3.1.1/gsd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/pyproject.toml` & `gsd-3.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 requires-python = ">=3.6"
 name = "gsd"
-version = "3.1.0"
+version = "3.1.1"
 description = "General simulation data file format."
 readme = "README.md"
 license = {text = "BSD-2-Clause"}
 authors = [
     {name = "Joshua A. Anderson", email = "joaander@umich.edu"},
 ]
 classifiers=[
@@ -21,15 +21,15 @@
 
 [project.scripts]
 gsd = "gsd.__main__:main"
 
 [project.urls]
 Homepage = "https://gsd.readthedocs.io"
 Documentation = "https://gsd.readthedocs.io"
-Download = "https://github.com/glotzerlab/gsd/releases/download/v3.1.0/gsd-3.1.0.tar.gz"
+Download = "https://github.com/glotzerlab/gsd/releases/download/v3.1.1/gsd-3.1.1.tar.gz"
 Source = "https://github.com/glotzerlab/gsd"
 Issues = "https://github.com/glotzerlab/gsd/issues"
 
 [tool.setuptools]
 packages = ["gsd", "gsd.test"]
 
 [build-system]
```

### Comparing `gsd-3.1.0/setup.cfg` & `gsd-3.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `gsd-3.1.0/setup.py` & `gsd-3.1.1/setup.py`

 * *Files identical despite different names*

