# Comparing `tmp/yep_detectors-1.0.3.tar.gz` & `tmp/yep_detectors-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yep_detectors-1.0.3.tar", last modified: Thu Aug  3 10:41:11 2023, max compression
+gzip compressed data, was "yep_detectors-1.0.4.tar", last modified: Thu Aug  3 10:45:31 2023, max compression
```

## Comparing `yep_detectors-1.0.3.tar` & `yep_detectors-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:41:11.622763 yep_detectors-1.0.3/
--rwxrwxrwx   0 a         (1000) a         (1000)      187 2023-08-03 10:41:11.621022 yep_detectors-1.0.3/PKG-INFO
--rwxrwxrwx   0 a         (1000) a         (1000)  2162315 2023-08-03 10:01:06.000000 yep_detectors-1.0.3/decomp.jar
-drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:41:11.553971 yep_detectors-1.0.3/decompiler/
--rwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 09:20:13.000000 yep_detectors-1.0.3/decompiler/__init__.py
--rwxrwxrwx   0 a         (1000) a         (1000)      249 2023-08-03 10:23:15.000000 yep_detectors-1.0.3/decompiler/decompiler.py
--rwxrwxrwx   0 a         (1000) a         (1000)     1070 2023-08-03 10:12:47.000000 yep_detectors-1.0.3/decompiler/inspector.py
--rwxrwxrwx   0 a         (1000) a         (1000)       38 2023-08-03 10:41:11.623824 yep_detectors-1.0.3/setup.cfg
--rwxrwxrwx   0 a         (1000) a         (1000)      367 2023-08-03 10:41:04.000000 yep_detectors-1.0.3/setup.py
-drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:41:11.608114 yep_detectors-1.0.3/yep_detectors.egg-info/
--rwxrwxrwx   0 a         (1000) a         (1000)      187 2023-08-03 10:41:11.000000 yep_detectors-1.0.3/yep_detectors.egg-info/PKG-INFO
--rwxrwxrwx   0 a         (1000) a         (1000)      279 2023-08-03 10:41:11.000000 yep_detectors-1.0.3/yep_detectors.egg-info/SOURCES.txt
--rwxrwxrwx   0 a         (1000) a         (1000)        1 2023-08-03 10:41:11.000000 yep_detectors-1.0.3/yep_detectors.egg-info/dependency_links.txt
--rwxrwxrwx   0 a         (1000) a         (1000)       52 2023-08-03 10:41:11.000000 yep_detectors-1.0.3/yep_detectors.egg-info/entry_points.txt
--rwxrwxrwx   0 a         (1000) a         (1000)       11 2023-08-03 10:41:11.000000 yep_detectors-1.0.3/yep_detectors.egg-info/top_level.txt
+drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:45:31.211350 yep_detectors-1.0.4/
+-rwxrwxrwx   0 a         (1000) a         (1000)      187 2023-08-03 10:45:31.209217 yep_detectors-1.0.4/PKG-INFO
+-rwxrwxrwx   0 a         (1000) a         (1000)  2162315 2023-08-03 10:01:06.000000 yep_detectors-1.0.4/decomp.jar
+-rwxrwxrwx   0 a         (1000) a         (1000)       38 2023-08-03 10:45:31.212352 yep_detectors-1.0.4/setup.cfg
+-rwxrwxrwx   0 a         (1000) a         (1000)      367 2023-08-03 10:45:20.000000 yep_detectors-1.0.4/setup.py
+drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:45:31.075726 yep_detectors-1.0.4/yep_detector/
+-rwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:37:51.000000 yep_detectors-1.0.4/yep_detector/__init__.py
+drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:45:31.125032 yep_detectors-1.0.4/yep_detector/decompiler/
+-rwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 09:20:13.000000 yep_detectors-1.0.4/yep_detector/decompiler/__init__.py
+-rwxrwxrwx   0 a         (1000) a         (1000)      249 2023-08-03 10:23:15.000000 yep_detectors-1.0.4/yep_detector/decompiler/decompiler.py
+-rwxrwxrwx   0 a         (1000) a         (1000)     1070 2023-08-03 10:12:47.000000 yep_detectors-1.0.4/yep_detector/decompiler/inspector.py
+-rwxrwxrwx   0 a         (1000) a         (1000)      494 2023-08-03 10:36:59.000000 yep_detectors-1.0.4/yep_detector/yep_detector.py
+drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:45:31.192168 yep_detectors-1.0.4/yep_detectors.egg-info/
+-rwxrwxrwx   0 a         (1000) a         (1000)      187 2023-08-03 10:45:30.000000 yep_detectors-1.0.4/yep_detectors.egg-info/PKG-INFO
+-rwxrwxrwx   0 a         (1000) a         (1000)      372 2023-08-03 10:45:30.000000 yep_detectors-1.0.4/yep_detectors.egg-info/SOURCES.txt
+-rwxrwxrwx   0 a         (1000) a         (1000)        1 2023-08-03 10:45:30.000000 yep_detectors-1.0.4/yep_detectors.egg-info/dependency_links.txt
+-rwxrwxrwx   0 a         (1000) a         (1000)       52 2023-08-03 10:45:30.000000 yep_detectors-1.0.4/yep_detectors.egg-info/entry_points.txt
+-rwxrwxrwx   0 a         (1000) a         (1000)       13 2023-08-03 10:45:30.000000 yep_detectors-1.0.4/yep_detectors.egg-info/top_level.txt
```

### Comparing `yep_detectors-1.0.3/decomp.jar` & `yep_detectors-1.0.4/decomp.jar`

 * *Files identical despite different names*

### Comparing `yep_detectors-1.0.3/decompiler/inspector.py` & `yep_detectors-1.0.4/yep_detector/decompiler/inspector.py`

 * *Files identical despite different names*

