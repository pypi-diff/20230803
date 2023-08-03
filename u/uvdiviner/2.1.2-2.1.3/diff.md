# Comparing `tmp/uvdiviner-2.1.2.tar.gz` & `tmp/uvdiviner-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uvdiviner-2.1.2.tar", last modified: Thu Aug  3 11:11:01 2023, max compression
+gzip compressed data, was "uvdiviner-2.1.3.tar", last modified: Thu Aug  3 11:20:27 2023, max compression
```

## Comparing `uvdiviner-2.1.2.tar` & `uvdiviner-2.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 11:11:01.380105 uvdiviner-2.1.2/
--rw-rw-rw-   0        0        0    11558 2023-08-03 07:38:11.000000 uvdiviner-2.1.2/LICENSE
--rw-rw-rw-   0        0        0     1349 2023-08-03 11:11:01.380105 uvdiviner-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      761 2023-08-03 08:25:04.000000 uvdiviner-2.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-08-03 11:11:01.380105 uvdiviner-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      963 2023-08-03 09:33:25.000000 uvdiviner-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 11:11:01.357384 uvdiviner-2.1.2/uvdiviner/
--rw-rw-rw-   0        0        0       21 2023-08-03 11:10:55.000000 uvdiviner-2.1.2/uvdiviner/__init__.py
--rw-rw-rw-   0        0        0      713 2023-08-03 07:04:10.000000 uvdiviner-2.1.2/uvdiviner/colorize.py
--rw-rw-rw-   0        0        0     2818 2023-08-03 09:31:46.000000 uvdiviner-2.1.2/uvdiviner/divine.py
--rw-rw-rw-   0        0        0      902 2023-08-03 10:54:13.000000 uvdiviner-2.1.2/uvdiviner/errors.py
--rw-rw-rw-   0        0        0     3071 2023-08-03 10:55:25.000000 uvdiviner-2.1.2/uvdiviner/evolution.py
--rw-rw-rw-   0        0        0     6540 2023-08-03 11:10:39.000000 uvdiviner-2.1.2/uvdiviner/main.py
--rw-rw-rw-   0        0        0     1829 2023-08-03 10:55:47.000000 uvdiviner-2.1.2/uvdiviner/progressbar.py
--rw-rw-rw-   0        0        0       13 2023-08-03 09:32:16.000000 uvdiviner-2.1.2/uvdiviner/settings.py
--rw-rw-rw-   0        0        0    56165 2023-06-24 12:01:07.000000 uvdiviner-2.1.2/uvdiviner/trigrams.py
-drwxrwxrwx   0        0        0        0 2023-08-03 11:11:01.380105 uvdiviner-2.1.2/uvdiviner.egg-info/
--rw-rw-rw-   0        0        0     1349 2023-08-03 11:11:01.000000 uvdiviner-2.1.2/uvdiviner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-08-03 11:11:01.000000 uvdiviner-2.1.2/uvdiviner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 11:11:01.000000 uvdiviner-2.1.2/uvdiviner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-03 11:11:01.000000 uvdiviner-2.1.2/uvdiviner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-03 11:11:01.000000 uvdiviner-2.1.2/uvdiviner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 11:20:27.355110 uvdiviner-2.1.3/
+-rw-rw-rw-   0        0        0    11558 2023-08-03 07:38:11.000000 uvdiviner-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1349 2023-08-03 11:20:27.354132 uvdiviner-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      761 2023-08-03 08:25:04.000000 uvdiviner-2.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 11:20:27.355110 uvdiviner-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      963 2023-08-03 09:33:25.000000 uvdiviner-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:20:27.345111 uvdiviner-2.1.3/uvdiviner/
+-rw-rw-rw-   0        0        0       21 2023-08-03 11:20:08.000000 uvdiviner-2.1.3/uvdiviner/__init__.py
+-rw-rw-rw-   0        0        0      972 2023-08-03 11:19:37.000000 uvdiviner-2.1.3/uvdiviner/colorize.py
+-rw-rw-rw-   0        0        0     2818 2023-08-03 09:31:46.000000 uvdiviner-2.1.3/uvdiviner/divine.py
+-rw-rw-rw-   0        0        0      902 2023-08-03 10:54:13.000000 uvdiviner-2.1.3/uvdiviner/errors.py
+-rw-rw-rw-   0        0        0     3071 2023-08-03 10:55:25.000000 uvdiviner-2.1.3/uvdiviner/evolution.py
+-rw-rw-rw-   0        0        0     6540 2023-08-03 11:10:39.000000 uvdiviner-2.1.3/uvdiviner/main.py
+-rw-rw-rw-   0        0        0     1829 2023-08-03 10:55:47.000000 uvdiviner-2.1.3/uvdiviner/progressbar.py
+-rw-rw-rw-   0        0        0       13 2023-08-03 09:32:16.000000 uvdiviner-2.1.3/uvdiviner/settings.py
+-rw-rw-rw-   0        0        0    56165 2023-06-24 12:01:07.000000 uvdiviner-2.1.3/uvdiviner/trigrams.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:20:27.354132 uvdiviner-2.1.3/uvdiviner.egg-info/
+-rw-rw-rw-   0        0        0     1349 2023-08-03 11:20:27.000000 uvdiviner-2.1.3/uvdiviner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-08-03 11:20:27.000000 uvdiviner-2.1.3/uvdiviner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 11:20:27.000000 uvdiviner-2.1.3/uvdiviner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-03 11:20:27.000000 uvdiviner-2.1.3/uvdiviner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-03 11:20:27.000000 uvdiviner-2.1.3/uvdiviner.egg-info/top_level.txt
```

### Comparing `uvdiviner-2.1.2/LICENSE` & `uvdiviner-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.2/PKG-INFO` & `uvdiviner-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvdiviner
-Version: 2.1.2
+Version: 2.1.3
 Summary: 基于周易蓍草占卜原理实现的中国古占卜.
 Home-page: https://gitee.com/unvisitor/diviner
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/diviner/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `uvdiviner-2.1.2/README.md` & `uvdiviner-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.2/setup.py` & `uvdiviner-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.2/uvdiviner/colorize.py` & `uvdiviner-2.1.3/uvdiviner/colorize.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from colorama import Fore, Style
 import colorama
 
 colorama.init()
+enabled = False
+
+def disable():
+    global enabled
+    enabled = True
 
 def bright(string):
-    return Style.BRIGHT + string + Style.RESET_ALL
+    return Style.BRIGHT + string + Style.RESET_ALL if enabled else string
 
 def light_white(string):
-    return Fore.WHITE + string + Style.RESET_ALL
+    return Fore.WHITE + string + Style.RESET_ALL if enabled else string
 
 def cyan(string):
-    return Fore.CYAN + string + Style.RESET_ALL
+    return Fore.CYAN + string + Style.RESET_ALL if enabled else string
 
 def green(string):
-    return Fore.GREEN + string + Style.RESET_ALL
+    return Fore.GREEN + string + Style.RESET_ALL if enabled else string
 
 def light_green(string):
-    return Fore.LIGHTGREEN_EX + string + Style.RESET_ALL
+    return Fore.LIGHTGREEN_EX + string + Style.RESET_ALL if enabled else string
 
 def light_red(string):
-    return Fore.LIGHTRED_EX + string + Style.RESET_ALL
+    return Fore.LIGHTRED_EX + string + Style.RESET_ALL if enabled else string
 
 def light_magenta(string):
-    return Fore.LIGHTMAGENTA_EX + string + Style.RESET_ALL
+    return Fore.LIGHTMAGENTA_EX + string + Style.RESET_ALL if enabled else string
 
 def light_yellow(string):
-    return Fore.LIGHTYELLOW_EX + string + Style.RESET_ALL
+    return Fore.LIGHTYELLOW_EX + string + Style.RESET_ALL if enabled else string
```

### Comparing `uvdiviner-2.1.2/uvdiviner/divine.py` & `uvdiviner-2.1.3/uvdiviner/divine.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.2/uvdiviner/errors.py` & `uvdiviner-2.1.3/uvdiviner/errors.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.2/uvdiviner/evolution.py` & `uvdiviner-2.1.3/uvdiviner/evolution.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.2/uvdiviner/main.py` & `uvdiviner-2.1.3/uvdiviner/main.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.2/uvdiviner/progressbar.py` & `uvdiviner-2.1.3/uvdiviner/progressbar.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.2/uvdiviner/trigrams.py` & `uvdiviner-2.1.3/uvdiviner/trigrams.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.2/uvdiviner.egg-info/PKG-INFO` & `uvdiviner-2.1.3/uvdiviner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvdiviner
-Version: 2.1.2
+Version: 2.1.3
 Summary: 基于周易蓍草占卜原理实现的中国古占卜.
 Home-page: https://gitee.com/unvisitor/diviner
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/diviner/issues
 Classifier: Programming Language :: Python :: 3
```

