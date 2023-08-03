# Comparing `tmp/yvesCMD-0.0.5.3.tar.gz` & `tmp/yvesCMD-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvesCMD-0.0.5.3.tar", last modified: Wed Aug  2 16:23:50 2023, max compression
+gzip compressed data, was "yvesCMD-0.0.6.tar", last modified: Thu Aug  3 18:54:41 2023, max compression
```

## Comparing `yvesCMD-0.0.5.3.tar` & `yvesCMD-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:50.250730 yvesCMD-0.0.5.3/
--rw-rw-rw-   0        0        0     1730 2023-08-02 16:23:50.246739 yvesCMD-0.0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     1412 2023-08-02 16:18:12.000000 yvesCMD-0.0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:50.156981 yvesCMD-0.0.5.3/YvesCMD/
--rw-rw-rw-   0        0        0       25 2023-08-01 09:12:31.000000 yvesCMD-0.0.5.3/YvesCMD/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:50.166956 yvesCMD-0.0.5.3/YvesCMD/src/
--rw-rw-rw-   0        0        0       53 2023-08-02 14:29:12.000000 yvesCMD-0.0.5.3/YvesCMD/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:50.222804 yvesCMD-0.0.5.3/YvesCMD/src/extensions/
--rw-rw-rw-   0        0        0       37 2023-08-02 14:29:07.000000 yvesCMD-0.0.5.3/YvesCMD/src/extensions/__init__.py
--rw-rw-rw-   0        0        0     1351 2023-08-02 15:30:13.000000 yvesCMD-0.0.5.3/YvesCMD/src/extensions/select.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:50.242755 yvesCMD-0.0.5.3/YvesCMD/src/utils/
--rw-rw-rw-   0        0        0      104 2023-08-02 13:11:36.000000 yvesCMD-0.0.5.3/YvesCMD/src/utils/__init__.py
--rw-rw-rw-   0        0        0      527 2023-08-02 13:07:53.000000 yvesCMD-0.0.5.3/YvesCMD/src/utils/detector.py
--rw-rw-rw-   0        0        0      898 2023-08-02 12:19:00.000000 yvesCMD-0.0.5.3/YvesCMD/src/utils/hooks.py
--rw-rw-rw-   0        0        0     1427 2023-08-02 12:09:51.000000 yvesCMD-0.0.5.3/YvesCMD/src/utils/register.py
--rw-rw-rw-   0        0        0     2518 2023-08-02 15:11:19.000000 yvesCMD-0.0.5.3/YvesCMD/src/yvescmd.py
--rw-rw-rw-   0        0        0       42 2023-08-02 16:23:50.250730 yvesCMD-0.0.5.3/setup.cfg
--rw-rw-rw-   0        0        0      613 2023-08-02 16:23:00.000000 yvesCMD-0.0.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:50.205850 yvesCMD-0.0.5.3/yvesCMD.egg-info/
--rw-rw-rw-   0        0        0     1730 2023-08-02 16:23:49.000000 yvesCMD-0.0.5.3/yvesCMD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-08-02 16:23:49.000000 yvesCMD-0.0.5.3/yvesCMD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 16:23:49.000000 yvesCMD-0.0.5.3/yvesCMD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 16:23:49.000000 yvesCMD-0.0.5.3/yvesCMD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 18:54:41.739488 yvesCMD-0.0.6/
+-rw-rw-rw-   0        0        0     1728 2023-08-03 18:54:41.736496 yvesCMD-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1412 2023-08-02 16:18:12.000000 yvesCMD-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 18:54:41.653718 yvesCMD-0.0.6/YvesCMD/
+-rw-rw-rw-   0        0        0       25 2023-08-01 09:12:31.000000 yvesCMD-0.0.6/YvesCMD/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 18:54:41.659702 yvesCMD-0.0.6/YvesCMD/src/
+-rw-rw-rw-   0        0        0       53 2023-08-02 14:29:12.000000 yvesCMD-0.0.6/YvesCMD/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 18:54:41.722545 yvesCMD-0.0.6/YvesCMD/src/extensions/
+-rw-rw-rw-   0        0        0       67 2023-08-03 18:53:01.000000 yvesCMD-0.0.6/YvesCMD/src/extensions/__init__.py
+-rw-rw-rw-   0        0        0      606 2023-08-03 18:53:10.000000 yvesCMD-0.0.6/YvesCMD/src/extensions/anwser.py
+-rw-rw-rw-   0        0        0     1351 2023-08-02 15:30:13.000000 yvesCMD-0.0.6/YvesCMD/src/extensions/select.py
+-rw-rw-rw-   0        0        0      669 2023-08-02 17:24:57.000000 yvesCMD-0.0.6/YvesCMD/src/extensions/state.py
+drwxrwxrwx   0        0        0        0 2023-08-03 18:54:41.733503 yvesCMD-0.0.6/YvesCMD/src/utils/
+-rw-rw-rw-   0        0        0      104 2023-08-02 13:11:36.000000 yvesCMD-0.0.6/YvesCMD/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      527 2023-08-02 13:07:53.000000 yvesCMD-0.0.6/YvesCMD/src/utils/detector.py
+-rw-rw-rw-   0        0        0      898 2023-08-02 12:19:00.000000 yvesCMD-0.0.6/YvesCMD/src/utils/hooks.py
+-rw-rw-rw-   0        0        0     1427 2023-08-02 12:09:51.000000 yvesCMD-0.0.6/YvesCMD/src/utils/register.py
+-rw-rw-rw-   0        0        0     2518 2023-08-02 15:11:19.000000 yvesCMD-0.0.6/YvesCMD/src/yvescmd.py
+-rw-rw-rw-   0        0        0       42 2023-08-03 18:54:41.739488 yvesCMD-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      615 2023-08-03 18:53:40.000000 yvesCMD-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 18:54:41.707574 yvesCMD-0.0.6/yvesCMD.egg-info/
+-rw-rw-rw-   0        0        0     1728 2023-08-03 18:54:41.000000 yvesCMD-0.0.6/yvesCMD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-08-03 18:54:41.000000 yvesCMD-0.0.6/yvesCMD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 18:54:41.000000 yvesCMD-0.0.6/yvesCMD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-03 18:54:41.000000 yvesCMD-0.0.6/yvesCMD.egg-info/top_level.txt
```

### Comparing `yvesCMD-0.0.5.3/PKG-INFO` & `yvesCMD-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yvesCMD
-Version: 0.0.5.3
+Version: 0.0.6
 Home-page: https://github.com/Yveradvir/Yvescmd
 Author: YveRadvir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yvesCMD Version: 0.0.5.3 Home-page: https://
+Metadata-Version: 2.1 Name: yvesCMD Version: 0.0.6 Home-page: https://
 github.com/Yveradvir/Yvescmd Author: YveRadvir Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown #
 ``| -> YvesCMD <- |``
                               pip install yvesCMD
 This microframework is created for cmd applications based on the cmd module in
                      Python, which is built-in by default.
```

### Comparing `yvesCMD-0.0.5.3/README.md` & `yvesCMD-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.5.3/YvesCMD/src/extensions/select.py` & `yvesCMD-0.0.6/YvesCMD/src/extensions/select.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.5.3/YvesCMD/src/utils/detector.py` & `yvesCMD-0.0.6/YvesCMD/src/utils/detector.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.5.3/YvesCMD/src/utils/hooks.py` & `yvesCMD-0.0.6/YvesCMD/src/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.5.3/YvesCMD/src/utils/register.py` & `yvesCMD-0.0.6/YvesCMD/src/utils/register.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.5.3/YvesCMD/src/yvescmd.py` & `yvesCMD-0.0.6/YvesCMD/src/yvescmd.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.5.3/setup.py` & `yvesCMD-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 import os
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
-
+    
 setup(
     name='yvesCMD',
-    version='0.0.5.3',
+    version='0.0.6',
     author='YveRadvir',
     url='https://github.com/Yveradvir/Yvescmd',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

### Comparing `yvesCMD-0.0.5.3/yvesCMD.egg-info/PKG-INFO` & `yvesCMD-0.0.6/yvesCMD.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yvesCMD
-Version: 0.0.5.3
+Version: 0.0.6
 Home-page: https://github.com/Yveradvir/Yvescmd
 Author: YveRadvir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yvesCMD Version: 0.0.5.3 Home-page: https://
+Metadata-Version: 2.1 Name: yvesCMD Version: 0.0.6 Home-page: https://
 github.com/Yveradvir/Yvescmd Author: YveRadvir Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown #
 ``| -> YvesCMD <- |``
                               pip install yvesCMD
 This microframework is created for cmd applications based on the cmd module in
                      Python, which is built-in by default.
```

