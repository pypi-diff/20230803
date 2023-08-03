# Comparing `tmp/pgzip-0.3.4.tar.gz` & `tmp/pgzip-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgzip-0.3.4.tar", last modified: Wed Nov  9 19:32:54 2022, max compression
+gzip compressed data, was "pgzip-0.3.5.tar", last modified: Thu Aug  3 21:44:56 2023, max compression
```

## Comparing `pgzip-0.3.4.tar` & `pgzip-0.3.5.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 19:32:54.595524 pgzip-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-11-09 19:32:39.000000 pgzip-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4614 2022-11-09 19:32:54.595524 pgzip-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3821 2022-11-09 19:32:39.000000 pgzip-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 19:32:54.595524 pgzip-0.3.4/pgzip/
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-11-09 19:32:39.000000 pgzip-0.3.4/pgzip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-11-09 19:32:39.000000 pgzip-0.3.4/pgzip/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26918 2022-11-09 19:32:39.000000 pgzip-0.3.4/pgzip/pgzip.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 19:32:54.595524 pgzip-0.3.4/pgzip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4614 2022-11-09 19:32:54.000000 pgzip-0.3.4/pgzip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-11-09 19:32:54.000000 pgzip-0.3.4/pgzip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 19:32:54.000000 pgzip-0.3.4/pgzip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-09 19:32:54.000000 pgzip-0.3.4/pgzip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-09 19:32:54.595524 pgzip-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-11-09 19:32:39.000000 pgzip-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:44:56.729747 pgzip-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-03 21:44:44.000000 pgzip-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-08-03 21:44:56.729747 pgzip-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-08-03 21:44:44.000000 pgzip-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:44:56.729747 pgzip-0.3.5/pgzip/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-03 21:44:44.000000 pgzip-0.3.5/pgzip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-08-03 21:44:44.000000 pgzip-0.3.5/pgzip/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-08-03 21:44:44.000000 pgzip-0.3.5/pgzip/pgzip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:44:56.729747 pgzip-0.3.5/pgzip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-08-03 21:44:56.000000 pgzip-0.3.5/pgzip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-03 21:44:56.000000 pgzip-0.3.5/pgzip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 21:44:56.000000 pgzip-0.3.5/pgzip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 21:44:56.000000 pgzip-0.3.5/pgzip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 21:44:56.729747 pgzip-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-03 21:44:44.000000 pgzip-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:44:56.729747 pgzip-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-03 21:44:44.000000 pgzip-0.3.5/tests/test_pgzip.py
```

### Comparing `pgzip-0.3.4/LICENSE` & `pgzip-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pgzip-0.3.4/PKG-INFO` & `pgzip-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pgzip
-Version: 0.3.4
+Version: 0.3.5
 Summary: A multi-threading implementation of Python gzip module
 Home-page: https://github.com/pgzip/pgzip
 Author: pgzip team
 Author-email: pgzip@thegoldfish.org
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pgzip
 
 [![Run tests](https://github.com/pgzip/pgzip/actions/workflows/python-tests.yml/badge.svg)](https://github.com/pgzip/pgzip/actions/workflows/python-tests.yml)
 [![CodeQL](https://github.com/pgzip/pgzip/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/pgzip/pgzip/actions/workflows/codeql-analysis.yml)
```

### Comparing `pgzip-0.3.4/README.md` & `pgzip-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pgzip-0.3.4/pgzip/__main__.py` & `pgzip-0.3.5/pgzip/__main__.py`

 * *Files identical despite different names*

### Comparing `pgzip-0.3.4/pgzip/pgzip.py` & `pgzip-0.3.5/pgzip/pgzip.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     FEXTRA,
     FNAME,
     FCOMMENT,
     FHCRC,
 )
 from concurrent.futures import ThreadPoolExecutor
 
-__version__ = "0.3.4"
+__version__ = "0.3.5"
 
 SID = b"IG"  # Subfield ID of indexed gzip file
 
 
 def open(
     filename,
     mode="rb",
@@ -568,14 +568,29 @@
         return (body_bytes, rsize, crc, rcrc)
 
     def _decompress_async(self, data, rcrc, rsize):
         self._read_pool.append(
             self._pool.submit(self._decompress_func, data, rcrc, rsize)
         )
 
+        
+    def _read_exact(self, n):
+        '''Read exactly *n* bytes from `fp`
+        This method is required because fp may be unbuffered,
+        i.e. return short reads.
+        '''
+        data = self._fp.read(n)
+        while len(data) < n:
+            b = self._fp.read(n - len(data))
+            if not b:
+                raise EOFError("Compressed file ended before the "
+                           "end-of-stream marker was reached")
+            data += b
+        return data
+   
     def _read_gzip_header(self):
         magic = self._fp.read(2)
         if magic == b"":
             return False
 
         if magic != b"\037\213":
             raise OSError("Not a gzipped file (%r)" % magic)
```

### Comparing `pgzip-0.3.4/pgzip.egg-info/PKG-INFO` & `pgzip-0.3.5/pgzip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pgzip
-Version: 0.3.4
+Version: 0.3.5
 Summary: A multi-threading implementation of Python gzip module
 Home-page: https://github.com/pgzip/pgzip
 Author: pgzip team
 Author-email: pgzip@thegoldfish.org
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pgzip
 
 [![Run tests](https://github.com/pgzip/pgzip/actions/workflows/python-tests.yml/badge.svg)](https://github.com/pgzip/pgzip/actions/workflows/python-tests.yml)
 [![CodeQL](https://github.com/pgzip/pgzip/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/pgzip/pgzip/actions/workflows/codeql-analysis.yml)
```

### Comparing `pgzip-0.3.4/setup.py` & `pgzip-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,9 +21,9 @@
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Intended Audience :: Developers',
     ],
-    python_requires=">=3.6"
+    python_requires=">=3.7"
 )
```

