# Comparing `tmp/yep_detectors-1.0.0.tar.gz` & `tmp/yep_detectors-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yep_detectors-1.0.0.tar", last modified: Thu Aug  3 10:23:14 2023, max compression
+gzip compressed data, was "yep_detectors-1.0.1.tar", last modified: Thu Aug  3 10:28:59 2023, max compression
```

## Comparing `yep_detectors-1.0.0.tar` & `yep_detectors-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:23:14.153712 yep_detectors-1.0.0/
--rwxrwxrwx   0 a         (1000) a         (1000)      187 2023-08-03 10:23:14.152207 yep_detectors-1.0.0/PKG-INFO
--rwxrwxrwx   0 a         (1000) a         (1000)  2162315 2023-08-03 10:01:06.000000 yep_detectors-1.0.0/decomp.jar
-drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:23:14.083949 yep_detectors-1.0.0/decompiler/
--rwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 09:20:13.000000 yep_detectors-1.0.0/decompiler/__init__.py
--rwxrwxrwx   0 a         (1000) a         (1000)      249 2023-08-03 10:23:07.000000 yep_detectors-1.0.0/decompiler/decompiler.py
--rwxrwxrwx   0 a         (1000) a         (1000)     1070 2023-08-03 10:12:47.000000 yep_detectors-1.0.0/decompiler/inspector.py
--rwxrwxrwx   0 a         (1000) a         (1000)       38 2023-08-03 10:23:14.155576 yep_detectors-1.0.0/setup.cfg
--rwxrwxrwx   0 a         (1000) a         (1000)      367 2023-08-03 10:22:56.000000 yep_detectors-1.0.0/setup.py
-drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:23:14.141778 yep_detectors-1.0.0/yep_detectors.egg-info/
--rwxrwxrwx   0 a         (1000) a         (1000)      187 2023-08-03 10:23:13.000000 yep_detectors-1.0.0/yep_detectors.egg-info/PKG-INFO
--rwxrwxrwx   0 a         (1000) a         (1000)      279 2023-08-03 10:23:13.000000 yep_detectors-1.0.0/yep_detectors.egg-info/SOURCES.txt
--rwxrwxrwx   0 a         (1000) a         (1000)        1 2023-08-03 10:23:13.000000 yep_detectors-1.0.0/yep_detectors.egg-info/dependency_links.txt
--rwxrwxrwx   0 a         (1000) a         (1000)       52 2023-08-03 10:23:13.000000 yep_detectors-1.0.0/yep_detectors.egg-info/entry_points.txt
--rwxrwxrwx   0 a         (1000) a         (1000)       11 2023-08-03 10:23:13.000000 yep_detectors-1.0.0/yep_detectors.egg-info/top_level.txt
+drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:28:59.317502 yep_detectors-1.0.1/
+-rwxrwxrwx   0 a         (1000) a         (1000)      187 2023-08-03 10:28:59.316451 yep_detectors-1.0.1/PKG-INFO
+-rwxrwxrwx   0 a         (1000) a         (1000)  2162315 2023-08-03 10:01:06.000000 yep_detectors-1.0.1/decomp.jar
+drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:28:59.228998 yep_detectors-1.0.1/decompiler/
+-rwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 09:20:13.000000 yep_detectors-1.0.1/decompiler/__init__.py
+-rwxrwxrwx   0 a         (1000) a         (1000)      249 2023-08-03 10:23:15.000000 yep_detectors-1.0.1/decompiler/decompiler.py
+-rwxrwxrwx   0 a         (1000) a         (1000)     1070 2023-08-03 10:12:47.000000 yep_detectors-1.0.1/decompiler/inspector.py
+-rwxrwxrwx   0 a         (1000) a         (1000)       38 2023-08-03 10:28:59.318702 yep_detectors-1.0.1/setup.cfg
+-rwxrwxrwx   0 a         (1000) a         (1000)      367 2023-08-03 10:28:54.000000 yep_detectors-1.0.1/setup.py
+drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:28:59.248158 yep_detectors-1.0.1/yep_detector/
+-rwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:27:31.000000 yep_detectors-1.0.1/yep_detector/__init__.py
+-rwxrwxrwx   0 a         (1000) a         (1000)      494 2023-08-03 10:27:46.000000 yep_detectors-1.0.1/yep_detector/yep_detector.py
+drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:28:59.303826 yep_detectors-1.0.1/yep_detectors.egg-info/
+-rwxrwxrwx   0 a         (1000) a         (1000)      187 2023-08-03 10:28:59.000000 yep_detectors-1.0.1/yep_detectors.egg-info/PKG-INFO
+-rwxrwxrwx   0 a         (1000) a         (1000)      333 2023-08-03 10:28:59.000000 yep_detectors-1.0.1/yep_detectors.egg-info/SOURCES.txt
+-rwxrwxrwx   0 a         (1000) a         (1000)        1 2023-08-03 10:28:59.000000 yep_detectors-1.0.1/yep_detectors.egg-info/dependency_links.txt
+-rwxrwxrwx   0 a         (1000) a         (1000)       52 2023-08-03 10:28:59.000000 yep_detectors-1.0.1/yep_detectors.egg-info/entry_points.txt
+-rwxrwxrwx   0 a         (1000) a         (1000)       24 2023-08-03 10:28:59.000000 yep_detectors-1.0.1/yep_detectors.egg-info/top_level.txt
```

### Comparing `yep_detectors-1.0.0/decomp.jar` & `yep_detectors-1.0.1/decomp.jar`

 * *Files identical despite different names*

### Comparing `yep_detectors-1.0.0/decompiler/inspector.py` & `yep_detectors-1.0.1/decompiler/inspector.py`

 * *Files identical despite different names*

