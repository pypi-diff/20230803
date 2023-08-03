# Comparing `tmp/xeus-python-shell-0.6.0.tar.gz` & `tmp/xeus-python-shell-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeus-python-shell-0.6.0.tar", last modified: Mon Jul 10 14:44:54 2023, max compression
+gzip compressed data, was "xeus-python-shell-0.6.1.tar", last modified: Thu Aug  3 14:28:38 2023, max compression
```

## Comparing `xeus-python-shell-0.6.0.tar` & `xeus-python-shell-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-10 14:44:54.241876 xeus-python-shell-0.6.0/
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     1518 2021-08-13 10:02:56.000000 xeus-python-shell-0.6.0/LICENSE
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)       16 2021-08-19 09:11:29.000000 xeus-python-shell-0.6.0/MANIFEST.in
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      852 2023-07-10 14:44:54.240876 xeus-python-shell-0.6.0/PKG-INFO
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)      101 2021-08-19 08:49:07.000000 xeus-python-shell-0.6.0/README.md
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       38 2023-07-10 14:44:54.241876 xeus-python-shell-0.6.0/setup.cfg
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1144 2023-07-10 14:43:23.000000 xeus-python-shell-0.6.0/setup.py
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-10 14:44:54.239876 xeus-python-shell-0.6.0/xeus_python_shell/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        0 2022-08-05 13:17:28.000000 xeus-python-shell-0.6.0/xeus_python_shell/__init__.py
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)      587 2022-06-29 10:04:57.000000 xeus-python-shell-0.6.0/xeus_python_shell/compiler.py
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     3805 2022-08-09 09:38:41.000000 xeus-python-shell-0.6.0/xeus_python_shell/debugger.py
--rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     1383 2022-06-29 10:04:57.000000 xeus-python-shell-0.6.0/xeus_python_shell/display.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3481 2023-07-10 14:43:11.000000 xeus-python-shell-0.6.0/xeus_python_shell/shell.py
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-10 14:44:54.240876 xeus-python-shell-0.6.0/xeus_python_shell.egg-info/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      852 2023-07-10 14:44:54.000000 xeus-python-shell-0.6.0/xeus_python_shell.egg-info/PKG-INFO
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      388 2023-07-10 14:44:54.000000 xeus-python-shell-0.6.0/xeus_python_shell.egg-info/SOURCES.txt
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        1 2023-07-10 14:44:54.000000 xeus-python-shell-0.6.0/xeus_python_shell.egg-info/dependency_links.txt
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       73 2023-07-10 14:44:54.000000 xeus-python-shell-0.6.0/xeus_python_shell.egg-info/requires.txt
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       18 2023-07-10 14:44:54.000000 xeus-python-shell-0.6.0/xeus_python_shell.egg-info/top_level.txt
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-08-03 14:28:38.054923 xeus-python-shell-0.6.1/
+-rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     1518 2021-08-13 10:02:56.000000 xeus-python-shell-0.6.1/LICENSE
+-rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)       16 2021-08-19 09:11:29.000000 xeus-python-shell-0.6.1/MANIFEST.in
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      852 2023-08-03 14:28:38.053923 xeus-python-shell-0.6.1/PKG-INFO
+-rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)      101 2021-08-19 08:49:07.000000 xeus-python-shell-0.6.1/README.md
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       38 2023-08-03 14:28:38.054923 xeus-python-shell-0.6.1/setup.cfg
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1144 2023-08-03 14:27:22.000000 xeus-python-shell-0.6.1/setup.py
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-08-03 14:28:38.050923 xeus-python-shell-0.6.1/xeus_python_shell/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        0 2022-08-05 13:17:28.000000 xeus-python-shell-0.6.1/xeus_python_shell/__init__.py
+-rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)      587 2022-06-29 10:04:57.000000 xeus-python-shell-0.6.1/xeus_python_shell/compiler.py
+-rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     3805 2022-08-09 09:38:41.000000 xeus-python-shell-0.6.1/xeus_python_shell/debugger.py
+-rw-rw-r--   0 martinrenou  (1000) martinrenou  (1000)     1383 2022-06-29 10:04:57.000000 xeus-python-shell-0.6.1/xeus_python_shell/display.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3521 2023-08-03 14:27:05.000000 xeus-python-shell-0.6.1/xeus_python_shell/shell.py
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-08-03 14:28:38.053923 xeus-python-shell-0.6.1/xeus_python_shell.egg-info/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      852 2023-08-03 14:28:38.000000 xeus-python-shell-0.6.1/xeus_python_shell.egg-info/PKG-INFO
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      388 2023-08-03 14:28:38.000000 xeus-python-shell-0.6.1/xeus_python_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        1 2023-08-03 14:28:38.000000 xeus-python-shell-0.6.1/xeus_python_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       73 2023-08-03 14:28:38.000000 xeus-python-shell-0.6.1/xeus_python_shell.egg-info/requires.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       18 2023-08-03 14:28:38.000000 xeus-python-shell-0.6.1/xeus_python_shell.egg-info/top_level.txt
```

### Comparing `xeus-python-shell-0.6.0/LICENSE` & `xeus-python-shell-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xeus-python-shell-0.6.0/PKG-INFO` & `xeus-python-shell-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeus-python-shell
-Version: 0.6.0
+Version: 0.6.1
 Summary: The xeus-python core python logic.
 Home-page: https://github.com/jupyter-xeus/xeus-python-shell
 Author: QuantStack dev team
 Maintainer: QuantStack dev team
 License: BSD 3-Clause
 Keywords: python ipython xeus-python
 Platform: any
```

### Comparing `xeus-python-shell-0.6.0/setup.py` & `xeus-python-shell-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 __AUTHOR__ = 'QuantStack dev team'
 
 setup(
     name='xeus-python-shell',
-    version='0.6.0',
+    version='0.6.1',
     description='The xeus-python core python logic.',
     author=__AUTHOR__,
     maintainer=__AUTHOR__,
     url='https://github.com/jupyter-xeus/xeus-python-shell',
     license='BSD 3-Clause',
     keywords='python ipython xeus-python',
     packages=find_packages(exclude=['test']),
```

### Comparing `xeus-python-shell-0.6.0/xeus_python_shell/compiler.py` & `xeus-python-shell-0.6.1/xeus_python_shell/compiler.py`

 * *Files identical despite different names*

### Comparing `xeus-python-shell-0.6.0/xeus_python_shell/debugger.py` & `xeus-python-shell-0.6.1/xeus_python_shell/debugger.py`

 * *Files identical despite different names*

### Comparing `xeus-python-shell-0.6.0/xeus_python_shell/display.py` & `xeus-python-shell-0.6.1/xeus_python_shell/display.py`

 * *Files identical despite different names*

### Comparing `xeus-python-shell-0.6.0/xeus_python_shell/shell.py` & `xeus-python-shell-0.6.1/xeus_python_shell/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 
 class XPythonShell(InteractiveShell):
     def __init__(self, *args, **kwargs):
         super(XPythonShell, self).__init__(*args, **kwargs)
 
         self.kernel = None
+        self.Completer.use_jedi = False
 
     def enable_gui(self, gui=None):
         """Not implemented yet."""
         pass
 
     def init_hooks(self):
         super(XPythonShell, self).init_hooks()
```

### Comparing `xeus-python-shell-0.6.0/xeus_python_shell.egg-info/PKG-INFO` & `xeus-python-shell-0.6.1/xeus_python_shell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeus-python-shell
-Version: 0.6.0
+Version: 0.6.1
 Summary: The xeus-python core python logic.
 Home-page: https://github.com/jupyter-xeus/xeus-python-shell
 Author: QuantStack dev team
 Maintainer: QuantStack dev team
 License: BSD 3-Clause
 Keywords: python ipython xeus-python
 Platform: any
```

