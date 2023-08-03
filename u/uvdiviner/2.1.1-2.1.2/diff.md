# Comparing `tmp/uvdiviner-2.1.1.tar.gz` & `tmp/uvdiviner-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uvdiviner-2.1.1.tar", last modified: Thu Aug  3 10:56:31 2023, max compression
+gzip compressed data, was "uvdiviner-2.1.2.tar", last modified: Thu Aug  3 11:11:01 2023, max compression
```

## Comparing `uvdiviner-2.1.1.tar` & `uvdiviner-2.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 10:56:31.392118 uvdiviner-2.1.1/
--rw-rw-rw-   0        0        0    11558 2023-08-03 07:38:11.000000 uvdiviner-2.1.1/LICENSE
--rw-rw-rw-   0        0        0     1349 2023-08-03 10:56:31.391101 uvdiviner-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      761 2023-08-03 08:25:04.000000 uvdiviner-2.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-03 10:56:31.392118 uvdiviner-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      963 2023-08-03 09:33:25.000000 uvdiviner-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 10:56:31.363217 uvdiviner-2.1.1/uvdiviner/
--rw-rw-rw-   0        0        0       21 2023-08-03 10:55:59.000000 uvdiviner-2.1.1/uvdiviner/__init__.py
--rw-rw-rw-   0        0        0      713 2023-08-03 07:04:10.000000 uvdiviner-2.1.1/uvdiviner/colorize.py
--rw-rw-rw-   0        0        0     2818 2023-08-03 09:31:46.000000 uvdiviner-2.1.1/uvdiviner/divine.py
--rw-rw-rw-   0        0        0      902 2023-08-03 10:54:13.000000 uvdiviner-2.1.1/uvdiviner/errors.py
--rw-rw-rw-   0        0        0     3071 2023-08-03 10:55:25.000000 uvdiviner-2.1.1/uvdiviner/evolution.py
--rw-rw-rw-   0        0        0     6527 2023-08-03 09:12:09.000000 uvdiviner-2.1.1/uvdiviner/main.py
--rw-rw-rw-   0        0        0     1829 2023-08-03 10:55:47.000000 uvdiviner-2.1.1/uvdiviner/progressbar.py
--rw-rw-rw-   0        0        0       13 2023-08-03 09:32:16.000000 uvdiviner-2.1.1/uvdiviner/settings.py
--rw-rw-rw-   0        0        0    56165 2023-06-24 12:01:07.000000 uvdiviner-2.1.1/uvdiviner/trigrams.py
-drwxrwxrwx   0        0        0        0 2023-08-03 10:56:31.389678 uvdiviner-2.1.1/uvdiviner.egg-info/
--rw-rw-rw-   0        0        0     1349 2023-08-03 10:56:31.000000 uvdiviner-2.1.1/uvdiviner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-08-03 10:56:31.000000 uvdiviner-2.1.1/uvdiviner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 10:56:31.000000 uvdiviner-2.1.1/uvdiviner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-03 10:56:31.000000 uvdiviner-2.1.1/uvdiviner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-03 10:56:31.000000 uvdiviner-2.1.1/uvdiviner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 11:11:01.380105 uvdiviner-2.1.2/
+-rw-rw-rw-   0        0        0    11558 2023-08-03 07:38:11.000000 uvdiviner-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1349 2023-08-03 11:11:01.380105 uvdiviner-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      761 2023-08-03 08:25:04.000000 uvdiviner-2.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 11:11:01.380105 uvdiviner-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      963 2023-08-03 09:33:25.000000 uvdiviner-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:11:01.357384 uvdiviner-2.1.2/uvdiviner/
+-rw-rw-rw-   0        0        0       21 2023-08-03 11:10:55.000000 uvdiviner-2.1.2/uvdiviner/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-08-03 07:04:10.000000 uvdiviner-2.1.2/uvdiviner/colorize.py
+-rw-rw-rw-   0        0        0     2818 2023-08-03 09:31:46.000000 uvdiviner-2.1.2/uvdiviner/divine.py
+-rw-rw-rw-   0        0        0      902 2023-08-03 10:54:13.000000 uvdiviner-2.1.2/uvdiviner/errors.py
+-rw-rw-rw-   0        0        0     3071 2023-08-03 10:55:25.000000 uvdiviner-2.1.2/uvdiviner/evolution.py
+-rw-rw-rw-   0        0        0     6540 2023-08-03 11:10:39.000000 uvdiviner-2.1.2/uvdiviner/main.py
+-rw-rw-rw-   0        0        0     1829 2023-08-03 10:55:47.000000 uvdiviner-2.1.2/uvdiviner/progressbar.py
+-rw-rw-rw-   0        0        0       13 2023-08-03 09:32:16.000000 uvdiviner-2.1.2/uvdiviner/settings.py
+-rw-rw-rw-   0        0        0    56165 2023-06-24 12:01:07.000000 uvdiviner-2.1.2/uvdiviner/trigrams.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:11:01.380105 uvdiviner-2.1.2/uvdiviner.egg-info/
+-rw-rw-rw-   0        0        0     1349 2023-08-03 11:11:01.000000 uvdiviner-2.1.2/uvdiviner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-08-03 11:11:01.000000 uvdiviner-2.1.2/uvdiviner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 11:11:01.000000 uvdiviner-2.1.2/uvdiviner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-03 11:11:01.000000 uvdiviner-2.1.2/uvdiviner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-03 11:11:01.000000 uvdiviner-2.1.2/uvdiviner.egg-info/top_level.txt
```

### Comparing `uvdiviner-2.1.1/LICENSE` & `uvdiviner-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.1/PKG-INFO` & `uvdiviner-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvdiviner
-Version: 2.1.1
+Version: 2.1.2
 Summary: 基于周易蓍草占卜原理实现的中国古占卜.
 Home-page: https://gitee.com/unvisitor/diviner
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/diviner/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `uvdiviner-2.1.1/README.md` & `uvdiviner-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.1/setup.py` & `uvdiviner-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.1/uvdiviner/colorize.py` & `uvdiviner-2.1.2/uvdiviner/colorize.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.1/uvdiviner/divine.py` & `uvdiviner-2.1.2/uvdiviner/divine.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.1/uvdiviner/errors.py` & `uvdiviner-2.1.2/uvdiviner/errors.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.1/uvdiviner/evolution.py` & `uvdiviner-2.1.2/uvdiviner/evolution.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.1/uvdiviner/main.py` & `uvdiviner-2.1.2/uvdiviner/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 try:
     from uvdiviner.evolution import diagram, trigram
     from uvdiviner.trigrams import data
     from uvdiviner.progressbar import ProgressBar
-    from uvdiviner.divine import make_trigram
+    from uvdiviner.divine import make_trigram, update_data
     from uvdiviner.colorize import bright, light_white, cyan, light_green, light_red, light_magenta, light_yellow
     from uvdiviner.settings import DEBUG
 except ImportError:
     from evolution import diagram, trigram
     from trigrams import data
     from progressbar import ProgressBar
     from divine import make_trigram, update_data
```

### Comparing `uvdiviner-2.1.1/uvdiviner/progressbar.py` & `uvdiviner-2.1.2/uvdiviner/progressbar.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.1/uvdiviner/trigrams.py` & `uvdiviner-2.1.2/uvdiviner/trigrams.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.1/uvdiviner.egg-info/PKG-INFO` & `uvdiviner-2.1.2/uvdiviner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvdiviner
-Version: 2.1.1
+Version: 2.1.2
 Summary: 基于周易蓍草占卜原理实现的中国古占卜.
 Home-page: https://gitee.com/unvisitor/diviner
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/diviner/issues
 Classifier: Programming Language :: Python :: 3
```

