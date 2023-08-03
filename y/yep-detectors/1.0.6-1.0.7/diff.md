# Comparing `tmp/yep_detectors-1.0.6.tar.gz` & `tmp/yep_detectors-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yep_detectors-1.0.6.tar", last modified: Thu Aug  3 10:49:05 2023, max compression
+gzip compressed data, was "yep_detectors-1.0.7.tar", last modified: Thu Aug  3 10:51:18 2023, max compression
```

## Comparing `yep_detectors-1.0.6.tar` & `yep_detectors-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:49:05.449400 yep_detectors-1.0.6/
--rwxrwxrwx   0 a         (1000) a         (1000)      187 2023-08-03 10:49:05.447403 yep_detectors-1.0.6/PKG-INFO
--rwxrwxrwx   0 a         (1000) a         (1000)  2162315 2023-08-03 10:01:06.000000 yep_detectors-1.0.6/decomp.jar
-drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:49:05.362152 yep_detectors-1.0.6/decompiler/
--rwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 09:20:13.000000 yep_detectors-1.0.6/decompiler/__init__.py
--rwxrwxrwx   0 a         (1000) a         (1000)      249 2023-08-03 10:23:15.000000 yep_detectors-1.0.6/decompiler/decompiler.py
--rwxrwxrwx   0 a         (1000) a         (1000)     1070 2023-08-03 10:12:47.000000 yep_detectors-1.0.6/decompiler/inspector.py
--rwxrwxrwx   0 a         (1000) a         (1000)       38 2023-08-03 10:49:05.450402 yep_detectors-1.0.6/setup.cfg
--rwxrwxrwx   0 a         (1000) a         (1000)      367 2023-08-03 10:49:02.000000 yep_detectors-1.0.6/setup.py
-drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:49:05.381125 yep_detectors-1.0.6/yep_detector/
--rwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:37:51.000000 yep_detectors-1.0.6/yep_detector/__init__.py
--rwxrwxrwx   0 a         (1000) a         (1000)      494 2023-08-03 10:47:51.000000 yep_detectors-1.0.6/yep_detector/main.py
-drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:49:05.435763 yep_detectors-1.0.6/yep_detectors.egg-info/
--rwxrwxrwx   0 a         (1000) a         (1000)      187 2023-08-03 10:49:05.000000 yep_detectors-1.0.6/yep_detectors.egg-info/PKG-INFO
--rwxrwxrwx   0 a         (1000) a         (1000)      325 2023-08-03 10:49:05.000000 yep_detectors-1.0.6/yep_detectors.egg-info/SOURCES.txt
--rwxrwxrwx   0 a         (1000) a         (1000)        1 2023-08-03 10:49:05.000000 yep_detectors-1.0.6/yep_detectors.egg-info/dependency_links.txt
--rwxrwxrwx   0 a         (1000) a         (1000)       52 2023-08-03 10:49:05.000000 yep_detectors-1.0.6/yep_detectors.egg-info/entry_points.txt
--rwxrwxrwx   0 a         (1000) a         (1000)       24 2023-08-03 10:49:05.000000 yep_detectors-1.0.6/yep_detectors.egg-info/top_level.txt
+drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:51:18.121296 yep_detectors-1.0.7/
+-rwxrwxrwx   0 a         (1000) a         (1000)      187 2023-08-03 10:51:18.118080 yep_detectors-1.0.7/PKG-INFO
+-rwxrwxrwx   0 a         (1000) a         (1000)  2162315 2023-08-03 10:01:06.000000 yep_detectors-1.0.7/decomp.jar
+drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:51:18.025330 yep_detectors-1.0.7/decompiler/
+-rwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 09:20:13.000000 yep_detectors-1.0.7/decompiler/__init__.py
+-rwxrwxrwx   0 a         (1000) a         (1000)      249 2023-08-03 10:23:15.000000 yep_detectors-1.0.7/decompiler/decompiler.py
+-rwxrwxrwx   0 a         (1000) a         (1000)     1070 2023-08-03 10:12:47.000000 yep_detectors-1.0.7/decompiler/inspector.py
+-rwxrwxrwx   0 a         (1000) a         (1000)       38 2023-08-03 10:51:18.122465 yep_detectors-1.0.7/setup.cfg
+-rwxrwxrwx   0 a         (1000) a         (1000)      367 2023-08-03 10:51:11.000000 yep_detectors-1.0.7/setup.py
+drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:51:18.048144 yep_detectors-1.0.7/yep_detector/
+-rwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:37:51.000000 yep_detectors-1.0.7/yep_detector/__init__.py
+-rwxrwxrwx   0 a         (1000) a         (1000)      494 2023-08-03 10:50:43.000000 yep_detectors-1.0.7/yep_detector/yep_detector.py
+drwxrwxrwx   0 a         (1000) a         (1000)        0 2023-08-03 10:51:18.104551 yep_detectors-1.0.7/yep_detectors.egg-info/
+-rwxrwxrwx   0 a         (1000) a         (1000)      187 2023-08-03 10:51:17.000000 yep_detectors-1.0.7/yep_detectors.egg-info/PKG-INFO
+-rwxrwxrwx   0 a         (1000) a         (1000)      333 2023-08-03 10:51:17.000000 yep_detectors-1.0.7/yep_detectors.egg-info/SOURCES.txt
+-rwxrwxrwx   0 a         (1000) a         (1000)        1 2023-08-03 10:51:17.000000 yep_detectors-1.0.7/yep_detectors.egg-info/dependency_links.txt
+-rwxrwxrwx   0 a         (1000) a         (1000)       52 2023-08-03 10:51:17.000000 yep_detectors-1.0.7/yep_detectors.egg-info/entry_points.txt
+-rwxrwxrwx   0 a         (1000) a         (1000)       24 2023-08-03 10:51:17.000000 yep_detectors-1.0.7/yep_detectors.egg-info/top_level.txt
```

### Comparing `yep_detectors-1.0.6/decomp.jar` & `yep_detectors-1.0.7/decomp.jar`

 * *Files identical despite different names*

### Comparing `yep_detectors-1.0.6/decompiler/inspector.py` & `yep_detectors-1.0.7/decompiler/inspector.py`

 * *Files identical despite different names*

