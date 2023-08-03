# Comparing `tmp/uvdiviner-2.1.0.tar.gz` & `tmp/uvdiviner-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uvdiviner-2.1.0.tar", last modified: Thu Aug  3 09:33:49 2023, max compression
+gzip compressed data, was "uvdiviner-2.1.1.tar", last modified: Thu Aug  3 10:56:31 2023, max compression
```

## Comparing `uvdiviner-2.1.0.tar` & `uvdiviner-2.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 09:33:49.994577 uvdiviner-2.1.0/
--rw-rw-rw-   0        0        0    11558 2023-08-03 07:38:11.000000 uvdiviner-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     1349 2023-08-03 09:33:49.994577 uvdiviner-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      761 2023-08-03 08:25:04.000000 uvdiviner-2.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-08-03 09:33:49.994577 uvdiviner-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      963 2023-08-03 09:33:25.000000 uvdiviner-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 09:33:49.964492 uvdiviner-2.1.0/uvdiviner/
--rw-rw-rw-   0        0        0       21 2023-08-03 09:32:08.000000 uvdiviner-2.1.0/uvdiviner/__init__.py
--rw-rw-rw-   0        0        0      713 2023-08-03 07:04:10.000000 uvdiviner-2.1.0/uvdiviner/colorize.py
--rw-rw-rw-   0        0        0     2818 2023-08-03 09:31:46.000000 uvdiviner-2.1.0/uvdiviner/divine.py
--rw-rw-rw-   0        0        0      902 2023-06-24 07:04:37.000000 uvdiviner-2.1.0/uvdiviner/errors.py
--rw-rw-rw-   0        0        0     2849 2023-07-31 12:34:56.000000 uvdiviner-2.1.0/uvdiviner/evolution.py
--rw-rw-rw-   0        0        0     6527 2023-08-03 09:12:09.000000 uvdiviner-2.1.0/uvdiviner/main.py
--rw-rw-rw-   0        0        0     1820 2023-08-03 06:31:01.000000 uvdiviner-2.1.0/uvdiviner/progressbar.py
--rw-rw-rw-   0        0        0       13 2023-08-03 09:32:16.000000 uvdiviner-2.1.0/uvdiviner/settings.py
--rw-rw-rw-   0        0        0    56165 2023-06-24 12:01:07.000000 uvdiviner-2.1.0/uvdiviner/trigrams.py
-drwxrwxrwx   0        0        0        0 2023-08-03 09:33:49.993212 uvdiviner-2.1.0/uvdiviner.egg-info/
--rw-rw-rw-   0        0        0     1349 2023-08-03 09:33:49.000000 uvdiviner-2.1.0/uvdiviner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-08-03 09:33:49.000000 uvdiviner-2.1.0/uvdiviner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 09:33:49.000000 uvdiviner-2.1.0/uvdiviner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-03 09:33:49.000000 uvdiviner-2.1.0/uvdiviner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-03 09:33:49.000000 uvdiviner-2.1.0/uvdiviner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 10:56:31.392118 uvdiviner-2.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-08-03 07:38:11.000000 uvdiviner-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1349 2023-08-03 10:56:31.391101 uvdiviner-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      761 2023-08-03 08:25:04.000000 uvdiviner-2.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 10:56:31.392118 uvdiviner-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      963 2023-08-03 09:33:25.000000 uvdiviner-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 10:56:31.363217 uvdiviner-2.1.1/uvdiviner/
+-rw-rw-rw-   0        0        0       21 2023-08-03 10:55:59.000000 uvdiviner-2.1.1/uvdiviner/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-08-03 07:04:10.000000 uvdiviner-2.1.1/uvdiviner/colorize.py
+-rw-rw-rw-   0        0        0     2818 2023-08-03 09:31:46.000000 uvdiviner-2.1.1/uvdiviner/divine.py
+-rw-rw-rw-   0        0        0      902 2023-08-03 10:54:13.000000 uvdiviner-2.1.1/uvdiviner/errors.py
+-rw-rw-rw-   0        0        0     3071 2023-08-03 10:55:25.000000 uvdiviner-2.1.1/uvdiviner/evolution.py
+-rw-rw-rw-   0        0        0     6527 2023-08-03 09:12:09.000000 uvdiviner-2.1.1/uvdiviner/main.py
+-rw-rw-rw-   0        0        0     1829 2023-08-03 10:55:47.000000 uvdiviner-2.1.1/uvdiviner/progressbar.py
+-rw-rw-rw-   0        0        0       13 2023-08-03 09:32:16.000000 uvdiviner-2.1.1/uvdiviner/settings.py
+-rw-rw-rw-   0        0        0    56165 2023-06-24 12:01:07.000000 uvdiviner-2.1.1/uvdiviner/trigrams.py
+drwxrwxrwx   0        0        0        0 2023-08-03 10:56:31.389678 uvdiviner-2.1.1/uvdiviner.egg-info/
+-rw-rw-rw-   0        0        0     1349 2023-08-03 10:56:31.000000 uvdiviner-2.1.1/uvdiviner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-08-03 10:56:31.000000 uvdiviner-2.1.1/uvdiviner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 10:56:31.000000 uvdiviner-2.1.1/uvdiviner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-03 10:56:31.000000 uvdiviner-2.1.1/uvdiviner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-03 10:56:31.000000 uvdiviner-2.1.1/uvdiviner.egg-info/top_level.txt
```

### Comparing `uvdiviner-2.1.0/LICENSE` & `uvdiviner-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.0/PKG-INFO` & `uvdiviner-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvdiviner
-Version: 2.1.0
+Version: 2.1.1
 Summary: 基于周易蓍草占卜原理实现的中国古占卜.
 Home-page: https://gitee.com/unvisitor/diviner
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/diviner/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `uvdiviner-2.1.0/README.md` & `uvdiviner-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.0/setup.py` & `uvdiviner-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.0/uvdiviner/colorize.py` & `uvdiviner-2.1.1/uvdiviner/colorize.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.0/uvdiviner/divine.py` & `uvdiviner-2.1.1/uvdiviner/divine.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.0/uvdiviner/errors.py` & `uvdiviner-2.1.1/uvdiviner/errors.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,22 +2,22 @@
     def __init__(self, message):
         super().__init__(self)
         self.message = "警告: 卜筮中所得到的爻数必须是 6 到 9 之间的正整数, 而传入的爻数为 %d, 这可能是算法错误或上层叙事者的一次叙事. 请优先检验算法问题." % message
     
     def __str__(self):
         return self.message
  
-class TiagramsValueError(ValueError):
+class TrigramsValueError(ValueError):
     def __init__(self, message):
         super().__init__(self)
         self.message = "卦爻数必须是 6 个, 但你传入了 %d 个数据." % message
 
     def __str__(self):
         return self.message
 
-class TiagramsTypeError(TypeError):
+class TrigramsTypeError(TypeError):
     def __init__(self, message):
         super().__init__(self)
         self.message = "卦爻必须是 List 或者 Tuple 数据, 但你传入的是 %s." % message
 
     def __str__(self):
         return self.message
```

### Comparing `uvdiviner-2.1.0/uvdiviner/evolution.py` & `uvdiviner-2.1.1/uvdiviner/evolution.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-from errors import *
-from trigrams import data
+try:
+    from errors import TrigramValueError, TrigramsValueError, TrigramsTypeError
+    from trigrams import data
+except ImportError:
+    from uvdiviner.errors import TrigramValueError, TrigramsValueError, TrigramsTypeError
+    from uvdiviner.trigrams import data
 
 class original:
     name = "无极"
 
 class ultimate:
     name = "太极"
 
 class diagram:
     trigrams = None
     status = "本卦"
     data = None
     variated = 0
     def __init__(self, trigrams):
         if not isinstance(trigrams, list) and not isinstance(trigrams, tuple):
-            raise TiagramsTypeError(type(trigrams))
+            raise TrigramsTypeError(type(trigrams))
         if len(trigrams) != 6:
-            raise TiagramsValueError(len(trigrams))
+            raise TrigramsValueError(len(trigrams))
         self.trigrams = trigrams
 
         position = 0
         for trigram in trigrams:
             trigram.position = position
             position += 1
```

### Comparing `uvdiviner-2.1.0/uvdiviner/main.py` & `uvdiviner-2.1.1/uvdiviner/main.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.0/uvdiviner/progressbar.py` & `uvdiviner-2.1.1/uvdiviner/progressbar.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import traceback
 import warnings
 from threading import Thread
 
 import colorama
 from colorama import Fore, Style, init
 
-init()
+colorama.init()
 
 def warning_show(message, category, filename, lineno, file=None, line=None):
     tb = traceback.extract_stack()[:-1]
     tb_message = ''.join(traceback.format_list(tb))
     warning_message = "Traceback (most recent call last):\n"
     warning_message += tb_message
     warning_message += f"{category.__name__}: {message}\n\n"
```

### Comparing `uvdiviner-2.1.0/uvdiviner/trigrams.py` & `uvdiviner-2.1.1/uvdiviner/trigrams.py`

 * *Files identical despite different names*

### Comparing `uvdiviner-2.1.0/uvdiviner.egg-info/PKG-INFO` & `uvdiviner-2.1.1/uvdiviner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvdiviner
-Version: 2.1.0
+Version: 2.1.1
 Summary: 基于周易蓍草占卜原理实现的中国古占卜.
 Home-page: https://gitee.com/unvisitor/diviner
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/diviner/issues
 Classifier: Programming Language :: Python :: 3
```

