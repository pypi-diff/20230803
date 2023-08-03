# Comparing `tmp/mypy-boto3-autoscaling-1.28.16.post1.tar.gz` & `tmp/mypy-boto3-autoscaling-1.28.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-autoscaling-1.28.16.post1.tar", last modified: Tue Aug  1 11:36:15 2023, max compression
+gzip compressed data, was "mypy-boto3-autoscaling-1.28.19.tar", last modified: Thu Aug  3 19:48:32 2023, max compression
```

## Comparing `mypy-boto3-autoscaling-1.28.16.post1.tar` & `mypy-boto3-autoscaling-1.28.19.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.300945 mypy-boto3-autoscaling-1.28.16.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24006 2023-08-01 11:36:15.296945 mypy-boto3-autoscaling-1.28.16.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22500 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.288945 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52911 2023-08-01 11:11:21.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52828 2023-08-01 11:11:21.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-08-01 11:11:21.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-08-01 11:11:21.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-08-01 11:11:21.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-08-01 11:11:21.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    87518 2023-08-01 11:11:25.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    87381 2023-08-01 11:11:23.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.296945 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24006 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 11:36:15.000000 mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:15.300945 mypy-boto3-autoscaling-1.28.16.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-01 11:11:20.000000 mypy-boto3-autoscaling-1.28.16.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:48:32.544403 mypy-boto3-autoscaling-1.28.19/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-03 19:46:51.000000 mypy-boto3-autoscaling-1.28.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24000 2023-08-03 19:48:32.544403 mypy-boto3-autoscaling-1.28.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22500 2023-08-03 19:46:51.000000 mypy-boto3-autoscaling-1.28.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:48:32.532403 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-03 19:46:51.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-03 19:46:51.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-03 19:46:51.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52911 2023-08-03 19:46:51.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52828 2023-08-03 19:46:51.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-08-03 19:46:52.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-08-03 19:46:52.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-08-03 19:46:51.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-08-03 19:46:51.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 19:46:51.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    87518 2023-08-03 19:46:54.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87381 2023-08-03 19:46:53.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-03 19:46:51.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:48:32.544403 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24000 2023-08-03 19:48:32.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-03 19:48:32.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:48:32.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:48:32.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-03 19:48:32.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 19:48:32.000000 mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 19:48:32.544403 mypy-boto3-autoscaling-1.28.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-03 19:46:51.000000 mypy-boto3-autoscaling-1.28.19/setup.py
```

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/LICENSE` & `mypy-boto3-autoscaling-1.28.19/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/PKG-INFO` & `mypy-boto3-autoscaling-1.28.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.28.16.post1
-Summary: Type annotations for boto3.AutoScaling 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.19
+Summary: Type annotations for boto3.AutoScaling 1.28.19 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/README.md` & `mypy-boto3-autoscaling-1.28.19/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/__init__.py` & `mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/__init__.pyi` & `mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/__main__.py` & `mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AutoScaling 1.28.16\nVersion:         1.28.16.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for boto3.AutoScaling 1.28.19\nVersion:         1.28.19\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16.post1")
+    print("1.28.19")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/client.py` & `mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/client.pyi` & `mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/literals.py` & `mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -565,14 +565,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/literals.pyi` & `mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -563,14 +563,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/paginator.py` & `mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/paginator.pyi` & `mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/type_defs.py` & `mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling/type_defs.pyi` & `mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/PKG-INFO` & `mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.28.16.post1
-Summary: Type annotations for boto3.AutoScaling 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.19
+Summary: Type annotations for boto3.AutoScaling 1.28.19 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/mypy_boto3_autoscaling.egg-info/SOURCES.txt` & `mypy-boto3-autoscaling-1.28.19/mypy_boto3_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.16.post1/setup.py` & `mypy-boto3-autoscaling-1.28.19/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-autoscaling",
-    version="1.28.16.post1",
+    version="1.28.19",
     packages=["mypy_boto3_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AutoScaling 1.28.16 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.AutoScaling 1.28.19 service generated with mypy-boto3-builder"
         " 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

