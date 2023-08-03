# Comparing `tmp/SuperPang-1.1.0.post1.tar.gz` & `tmp/SuperPang-1.1.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SuperPang-1.1.0.post1.tar", last modified: Sat Jul 29 18:57:32 2023, max compression
+gzip compressed data, was "SuperPang-1.1.0.post2.tar", last modified: Thu Aug  3 11:00:48 2023, max compression
```

## Comparing `SuperPang-1.1.0.post1.tar` & `SuperPang-1.1.0.post2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-29 18:57:32.672153 SuperPang-1.1.0.post1/
--rw-r--r--   0 fer       (1000) fer       (1000)     1532 2022-07-05 08:49:46.000000 SuperPang-1.1.0.post1/LICENSE
--rw-rw-r--   0 fer       (1000) fer       (1000)       31 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/MANIFEST.in
--rw-rw-r--   0 fer       (1000) fer       (1000)     8257 2023-07-29 18:57:32.672153 SuperPang-1.1.0.post1/PKG-INFO
--rw-rw-r--   0 fer       (1000) fer       (1000)     5730 2023-07-28 09:11:39.000000 SuperPang-1.1.0.post1/README.md
--rw-rw-r--   0 fer       (1000) fer       (1000)     1759 2023-07-28 09:09:52.000000 SuperPang-1.1.0.post1/pyproject.toml
--rw-rw-r--   0 fer       (1000) fer       (1000)       38 2023-07-29 18:57:32.672153 SuperPang-1.1.0.post1/setup.cfg
--rw-rw-r--   0 fer       (1000) fer       (1000)      798 2023-07-28 10:51:10.000000 SuperPang-1.1.0.post1/setup.py
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-29 18:57:32.660153 SuperPang-1.1.0.post1/src/
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-29 18:57:32.660153 SuperPang-1.1.0.post1/src/SuperPang.egg-info/
--rw-rw-r--   0 fer       (1000) fer       (1000)     8257 2023-07-29 18:57:32.000000 SuperPang-1.1.0.post1/src/SuperPang.egg-info/PKG-INFO
--rw-rw-r--   0 fer       (1000) fer       (1000)     1080 2023-07-29 18:57:32.000000 SuperPang-1.1.0.post1/src/SuperPang.egg-info/SOURCES.txt
--rw-rw-r--   0 fer       (1000) fer       (1000)        1 2023-07-29 18:57:32.000000 SuperPang-1.1.0.post1/src/SuperPang.egg-info/dependency_links.txt
--rw-rw-r--   0 fer       (1000) fer       (1000)      172 2023-07-29 18:57:32.000000 SuperPang-1.1.0.post1/src/SuperPang.egg-info/entry_points.txt
--rw-rw-r--   0 fer       (1000) fer       (1000)       38 2023-07-29 18:57:32.000000 SuperPang-1.1.0.post1/src/SuperPang.egg-info/requires.txt
--rw-rw-r--   0 fer       (1000) fer       (1000)       10 2023-07-29 18:57:32.000000 SuperPang-1.1.0.post1/src/SuperPang.egg-info/top_level.txt
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-29 18:57:32.660153 SuperPang-1.1.0.post1/src/superpang/
--rw-rw-r--   0 fer       (1000) fer       (1000)       12 2023-07-27 16:14:09.000000 SuperPang-1.1.0.post1/src/superpang/VERSION
--rw-rw-r--   0 fer       (1000) fer       (1000)        0 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/__init__.py
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-29 18:57:32.660153 SuperPang-1.1.0.post1/src/superpang/lib/
--rw-rw-r--   0 fer       (1000) fer       (1000)    59803 2023-07-27 18:42:42.000000 SuperPang-1.1.0.post1/src/superpang/lib/Assembler.py
--rw-rw-r--   0 fer       (1000) fer       (1000)     3485 2023-07-27 17:26:50.000000 SuperPang-1.1.0.post1/src/superpang/lib/Compressor.pyx
--rw-rw-r--   0 fer       (1000) fer       (1000)        0 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/lib/__init__.py
--rw-rw-r--   0 fer       (1000) fer       (1000)     5630 2023-07-28 09:05:45.000000 SuperPang-1.1.0.post1/src/superpang/lib/cutils.pyx
--rw-rw-r--   0 fer       (1000) fer       (1000)     3038 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/lib/utils.py
--rw-rw-r--   0 fer       (1000) fer       (1000)     2920 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/lib/vtools.pyx
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-29 18:57:32.660153 SuperPang-1.1.0.post1/src/superpang/scripts/
--rwxrwxr-x   0 fer       (1000) fer       (1000)    17576 2023-07-26 09:25:32.000000 SuperPang-1.1.0.post1/src/superpang/scripts/SuperPang.py
--rw-rw-r--   0 fer       (1000) fer       (1000)        0 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/scripts/__init__.py
--rwxrwxr-x   0 fer       (1000) fer       (1000)    12655 2023-07-27 07:48:19.000000 SuperPang-1.1.0.post1/src/superpang/scripts/condense-edges.py
--rwxrwxr-x   0 fer       (1000) fer       (1000)    16722 2023-07-28 09:06:48.000000 SuperPang-1.1.0.post1/src/superpang/scripts/homogenize.py
--rwxrwxr-x   0 fer       (1000) fer       (1000)     1568 2023-07-28 09:34:05.000000 SuperPang-1.1.0.post1/src/superpang/scripts/test-SuperPang.py
--rwxrwxr-x   0 fer       (1000) fer       (1000)     1568 2023-07-28 09:34:05.000000 SuperPang-1.1.0.post1/src/superpang/scripts/test_SuperPang.py
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-29 18:57:32.672153 SuperPang-1.1.0.post1/src/superpang/test_data/
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2430301 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2636415981.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2266131 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2636416036.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2274047 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2636416061.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2402610 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2636416062.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2207567 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2639762512.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2184834 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2639762514.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2317227 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2639762515.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2202772 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2639762516.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2210266 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2844342787.fna
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-08-03 11:00:48.192125 SuperPang-1.1.0.post2/
+-rw-r--r--   0 fer       (1000) fer       (1000)     1532 2022-07-05 08:49:46.000000 SuperPang-1.1.0.post2/LICENSE
+-rw-rw-r--   0 fer       (1000) fer       (1000)       31 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/MANIFEST.in
+-rw-rw-r--   0 fer       (1000) fer       (1000)     8257 2023-08-03 11:00:48.192125 SuperPang-1.1.0.post2/PKG-INFO
+-rw-rw-r--   0 fer       (1000) fer       (1000)     5730 2023-07-28 09:11:39.000000 SuperPang-1.1.0.post2/README.md
+-rw-rw-r--   0 fer       (1000) fer       (1000)     1759 2023-07-28 09:09:52.000000 SuperPang-1.1.0.post2/pyproject.toml
+-rw-rw-r--   0 fer       (1000) fer       (1000)       38 2023-08-03 11:00:48.192125 SuperPang-1.1.0.post2/setup.cfg
+-rw-rw-r--   0 fer       (1000) fer       (1000)      798 2023-07-28 10:51:10.000000 SuperPang-1.1.0.post2/setup.py
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-08-03 11:00:48.184125 SuperPang-1.1.0.post2/src/
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-08-03 11:00:48.184125 SuperPang-1.1.0.post2/src/SuperPang.egg-info/
+-rw-rw-r--   0 fer       (1000) fer       (1000)     8257 2023-08-03 11:00:48.000000 SuperPang-1.1.0.post2/src/SuperPang.egg-info/PKG-INFO
+-rw-rw-r--   0 fer       (1000) fer       (1000)     1080 2023-08-03 11:00:48.000000 SuperPang-1.1.0.post2/src/SuperPang.egg-info/SOURCES.txt
+-rw-rw-r--   0 fer       (1000) fer       (1000)        1 2023-08-03 11:00:48.000000 SuperPang-1.1.0.post2/src/SuperPang.egg-info/dependency_links.txt
+-rw-rw-r--   0 fer       (1000) fer       (1000)      172 2023-08-03 11:00:48.000000 SuperPang-1.1.0.post2/src/SuperPang.egg-info/entry_points.txt
+-rw-rw-r--   0 fer       (1000) fer       (1000)       38 2023-08-03 11:00:48.000000 SuperPang-1.1.0.post2/src/SuperPang.egg-info/requires.txt
+-rw-rw-r--   0 fer       (1000) fer       (1000)       10 2023-08-03 11:00:48.000000 SuperPang-1.1.0.post2/src/SuperPang.egg-info/top_level.txt
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-08-03 11:00:48.184125 SuperPang-1.1.0.post2/src/superpang/
+-rw-rw-r--   0 fer       (1000) fer       (1000)       12 2023-08-03 11:00:12.000000 SuperPang-1.1.0.post2/src/superpang/VERSION
+-rw-rw-r--   0 fer       (1000) fer       (1000)        0 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/src/superpang/__init__.py
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-08-03 11:00:48.184125 SuperPang-1.1.0.post2/src/superpang/lib/
+-rw-rw-r--   0 fer       (1000) fer       (1000)    59803 2023-07-27 18:42:42.000000 SuperPang-1.1.0.post2/src/superpang/lib/Assembler.py
+-rw-rw-r--   0 fer       (1000) fer       (1000)     3485 2023-07-27 17:26:50.000000 SuperPang-1.1.0.post2/src/superpang/lib/Compressor.pyx
+-rw-rw-r--   0 fer       (1000) fer       (1000)        0 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/src/superpang/lib/__init__.py
+-rw-rw-r--   0 fer       (1000) fer       (1000)     5244 2023-08-03 10:53:22.000000 SuperPang-1.1.0.post2/src/superpang/lib/cutils.pyx
+-rw-rw-r--   0 fer       (1000) fer       (1000)     3038 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/src/superpang/lib/utils.py
+-rw-rw-r--   0 fer       (1000) fer       (1000)     2920 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/src/superpang/lib/vtools.pyx
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-08-03 11:00:48.188125 SuperPang-1.1.0.post2/src/superpang/scripts/
+-rwxrwxr-x   0 fer       (1000) fer       (1000)    17576 2023-07-26 09:25:32.000000 SuperPang-1.1.0.post2/src/superpang/scripts/SuperPang.py
+-rw-rw-r--   0 fer       (1000) fer       (1000)        0 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/src/superpang/scripts/__init__.py
+-rwxrwxr-x   0 fer       (1000) fer       (1000)    12655 2023-07-27 07:48:19.000000 SuperPang-1.1.0.post2/src/superpang/scripts/condense-edges.py
+-rwxrwxr-x   0 fer       (1000) fer       (1000)    16722 2023-07-28 09:06:48.000000 SuperPang-1.1.0.post2/src/superpang/scripts/homogenize.py
+-rwxrwxr-x   0 fer       (1000) fer       (1000)     1568 2023-07-28 09:34:05.000000 SuperPang-1.1.0.post2/src/superpang/scripts/test-SuperPang.py
+-rwxrwxr-x   0 fer       (1000) fer       (1000)     1568 2023-07-28 09:34:05.000000 SuperPang-1.1.0.post2/src/superpang/scripts/test_SuperPang.py
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-08-03 11:00:48.192125 SuperPang-1.1.0.post2/src/superpang/test_data/
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2430301 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/src/superpang/test_data/2636415981.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2266131 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/src/superpang/test_data/2636416036.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2274047 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/src/superpang/test_data/2636416061.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2402610 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/src/superpang/test_data/2636416062.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2207567 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/src/superpang/test_data/2639762512.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2184834 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/src/superpang/test_data/2639762514.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2317227 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/src/superpang/test_data/2639762515.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2202772 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/src/superpang/test_data/2639762516.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2210266 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post2/src/superpang/test_data/2844342787.fna
```

### Comparing `SuperPang-1.1.0.post1/LICENSE` & `SuperPang-1.1.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/PKG-INFO` & `SuperPang-1.1.0.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SuperPang
-Version: 1.1.0.post1
+Version: 1.1.0.post2
 Summary: Non-redundant pangenome assemblies from multiple genomes or bins
 Author-email: Fernando Puente-Sánchez <fernando.puente.sanchez@slu.se>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Fernando Puente-Sánchez
         All rights reserved.
```

### Comparing `SuperPang-1.1.0.post1/README.md` & `SuperPang-1.1.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/pyproject.toml` & `SuperPang-1.1.0.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/setup.py` & `SuperPang-1.1.0.post2/setup.py`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/SuperPang.egg-info/PKG-INFO` & `SuperPang-1.1.0.post2/src/SuperPang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SuperPang
-Version: 1.1.0.post1
+Version: 1.1.0.post2
 Summary: Non-redundant pangenome assemblies from multiple genomes or bins
 Author-email: Fernando Puente-Sánchez <fernando.puente.sanchez@slu.se>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Fernando Puente-Sánchez
         All rights reserved.
```

### Comparing `SuperPang-1.1.0.post1/src/SuperPang.egg-info/SOURCES.txt` & `SuperPang-1.1.0.post2/src/SuperPang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/lib/Assembler.py` & `SuperPang-1.1.0.post2/src/superpang/lib/Assembler.py`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/lib/Compressor.pyx` & `SuperPang-1.1.0.post2/src/superpang/lib/Compressor.pyx`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/lib/cutils.pyx` & `SuperPang-1.1.0.post2/src/superpang/lib/cutils.pyx`

 * *Files 9% similar despite different names*

```diff
@@ -30,18 +30,16 @@
 
 
 cpdef parse_cigar(str cigar):
     cdef bytes py_bytes = cigar.encode('UTF-8')
     cdef Py_ssize_t cLen = len(py_bytes)
     cdef char *cigar_src = py_bytes
     cdef char c
-    cdef char [10] buf = [0]*10 # Explicitly initialize to 0.
-                                # Using conda compilers (but not base ubuntu compilers, even when versions were equal)
-                                #  caused trailing characters being passed to strtol in some instances (buf seemed to have more than 10 elements)
-                                #  so if those characters could be parsed as a number, the result from strtol was wront. Initializing to 0 from the starts apparently fixes this
+    cdef char [11] buf
+    buf[10] = 0 # We want a 10-element buffer, set the 11th to 0 so strtol knows where to stop
     cdef Py_ssize_t i, j, bsize = 0, nOps = 0, idlen = 0
     cdef float mlen = 0
     cdef long [:] Larray
     cdef char [:] oparray
     cdef double iden
     Larray  = clone(array('l'), 100000, False)
     oparray = clone(array('b'), 100000, False)
```

### Comparing `SuperPang-1.1.0.post1/src/superpang/lib/utils.py` & `SuperPang-1.1.0.post2/src/superpang/lib/utils.py`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/lib/vtools.pyx` & `SuperPang-1.1.0.post2/src/superpang/lib/vtools.pyx`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/scripts/SuperPang.py` & `SuperPang-1.1.0.post2/src/superpang/scripts/SuperPang.py`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/scripts/condense-edges.py` & `SuperPang-1.1.0.post2/src/superpang/scripts/condense-edges.py`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/scripts/homogenize.py` & `SuperPang-1.1.0.post2/src/superpang/scripts/homogenize.py`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/scripts/test-SuperPang.py` & `SuperPang-1.1.0.post2/src/superpang/scripts/test-SuperPang.py`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/scripts/test_SuperPang.py` & `SuperPang-1.1.0.post2/src/superpang/scripts/test_SuperPang.py`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/test_data/2636415981.fna` & `SuperPang-1.1.0.post2/src/superpang/test_data/2636415981.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/test_data/2636416036.fna` & `SuperPang-1.1.0.post2/src/superpang/test_data/2636416036.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/test_data/2636416061.fna` & `SuperPang-1.1.0.post2/src/superpang/test_data/2636416061.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/test_data/2636416062.fna` & `SuperPang-1.1.0.post2/src/superpang/test_data/2636416062.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/test_data/2639762512.fna` & `SuperPang-1.1.0.post2/src/superpang/test_data/2639762512.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/test_data/2639762514.fna` & `SuperPang-1.1.0.post2/src/superpang/test_data/2639762514.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/test_data/2639762515.fna` & `SuperPang-1.1.0.post2/src/superpang/test_data/2639762515.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/test_data/2639762516.fna` & `SuperPang-1.1.0.post2/src/superpang/test_data/2639762516.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0.post1/src/superpang/test_data/2844342787.fna` & `SuperPang-1.1.0.post2/src/superpang/test_data/2844342787.fna`

 * *Files identical despite different names*

