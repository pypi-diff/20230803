# Comparing `tmp/reata-1.1.5.tar.gz` & `tmp/reata-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reata-1.1.5.tar", last modified: Mon Jul 31 03:18:21 2023, max compression
+gzip compressed data, was "reata-1.1.6.tar", last modified: Thu Aug  3 04:31:33 2023, max compression
```

## Comparing `reata-1.1.5.tar` & `reata-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-31 03:18:21.000000 reata-1.1.5/
--rw-rw-r--   0 subvert   (1000) subvert   (1000)    35149 2022-12-27 12:35:32.000000 reata-1.1.5/LICENSE
--rw-rw-r--   0 subvert   (1000) subvert   (1000)    42542 2023-07-31 03:18:21.000000 reata-1.1.5/PKG-INFO
--rw-rw-r--   0 subvert   (1000) subvert   (1000)     1812 2023-01-08 05:17:25.000000 reata-1.1.5/README.rst
-drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-31 03:18:21.000000 reata-1.1.5/reata/
--rw-rw-r--   0 subvert   (1000) subvert   (1000)     6008 2023-07-30 07:06:23.000000 reata-1.1.5/reata/__futures__.py
--rw-rw-r--   0 subvert   (1000) subvert   (1000)       74 2023-01-08 04:34:06.000000 reata-1.1.5/reata/__init__.py
--rw-rw-r--   0 subvert   (1000) subvert   (1000)    22848 2023-04-13 02:09:12.000000 reata-1.1.5/reata/client.py
--rw-rw-r--   0 subvert   (1000) subvert   (1000)     2974 2023-07-15 21:59:03.000000 reata-1.1.5/reata/schema.py
-drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-31 03:18:21.000000 reata-1.1.5/reata.egg-info/
--rw-rw-r--   0 subvert   (1000) subvert   (1000)    42542 2023-07-31 03:18:21.000000 reata-1.1.5/reata.egg-info/PKG-INFO
--rw-rw-r--   0 subvert   (1000) subvert   (1000)      242 2023-07-31 03:18:21.000000 reata-1.1.5/reata.egg-info/SOURCES.txt
--rw-rw-r--   0 subvert   (1000) subvert   (1000)        1 2023-07-31 03:18:21.000000 reata-1.1.5/reata.egg-info/dependency_links.txt
--rw-rw-r--   0 subvert   (1000) subvert   (1000)       73 2023-07-31 03:18:21.000000 reata-1.1.5/reata.egg-info/requires.txt
--rw-rw-r--   0 subvert   (1000) subvert   (1000)        6 2023-07-31 03:18:21.000000 reata-1.1.5/reata.egg-info/top_level.txt
--rw-rw-r--   0 subvert   (1000) subvert   (1000)       38 2023-07-31 03:18:21.000000 reata-1.1.5/setup.cfg
--rw-rw-r--   0 subvert   (1000) subvert   (1000)      599 2023-07-31 03:17:42.000000 reata-1.1.5/setup.py
+drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-08-03 04:31:33.000000 reata-1.1.6/
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)    35149 2022-12-27 12:35:32.000000 reata-1.1.6/LICENSE
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)    42542 2023-08-03 04:31:33.000000 reata-1.1.6/PKG-INFO
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)     1812 2023-01-08 05:17:25.000000 reata-1.1.6/README.rst
+drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-08-03 04:31:33.000000 reata-1.1.6/reata/
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)     6239 2023-08-01 04:32:32.000000 reata-1.1.6/reata/__futures__.py
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)       74 2023-01-08 04:34:06.000000 reata-1.1.6/reata/__init__.py
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)    22848 2023-07-31 07:38:46.000000 reata-1.1.6/reata/client.py
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)     2974 2023-07-15 21:59:03.000000 reata-1.1.6/reata/schema.py
+drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-08-03 04:31:33.000000 reata-1.1.6/reata.egg-info/
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)    42542 2023-08-03 04:31:33.000000 reata-1.1.6/reata.egg-info/PKG-INFO
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)      242 2023-08-03 04:31:33.000000 reata-1.1.6/reata.egg-info/SOURCES.txt
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)        1 2023-08-03 04:31:33.000000 reata-1.1.6/reata.egg-info/dependency_links.txt
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)       73 2023-08-03 04:31:33.000000 reata-1.1.6/reata.egg-info/requires.txt
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)        6 2023-08-03 04:31:33.000000 reata-1.1.6/reata.egg-info/top_level.txt
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)       38 2023-08-03 04:31:33.000000 reata-1.1.6/setup.cfg
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)      599 2023-08-03 04:29:59.000000 reata-1.1.6/setup.py
```

### Comparing `reata-1.1.5/LICENSE` & `reata-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reata-1.1.5/PKG-INFO` & `reata-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reata
-Version: 1.1.5
+Version: 1.1.6
 Summary: A simple MySQL DBAPI wrapper for simplifying data processing pipelines.
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `reata-1.1.5/README.rst` & `reata-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `reata-1.1.5/reata/__futures__.py` & `reata-1.1.6/reata/__futures__.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,18 @@
         super().__init__(attrs)
         self.size = size
         self.attrs = attrs
 
     def __str__(self) -> str:
         return f"{self.dtype}({self.size}) {self.attrs}"
 
+    @property
+    def effective_size(self) -> int:
+        return self.size
+
 
 class StringType(BaseDataType):
     """Base class for all string types."""
 
     def __init__(self, size: Optional[int] = None, attrs: str = "") -> None:
         super().__init__(attrs)
         self.size = size
@@ -70,14 +74,18 @@
 
     def __str__(self) -> str:
         if self.size is None:
             return f"{self.dtype} {self.attrs}"
         else:
             return f"{self.dtype}({self.size}) {self.attrs}"
 
+    @property
+    def effective_size(self) -> int:
+        return self.size
+
 
 class DecimalType(BaseDataType):
     """Base class for all floating point types."""
 
     def __init__(self, size: int, precision: int, attrs: str = "") -> None:
         super().__init__(attrs)
         self.size = size
@@ -104,14 +112,18 @@
     def __init__(self, size: int, attrs: str = "") -> None:
         super().__init__(attrs)
         self.size = size
 
     def __str__(self) -> str:
         return f"{self.dtype}({self.size}) {self.attrs}"
 
+    @property
+    def effective_size(self) -> int:
+        return self.size
+
 
 class TimeType(BaseDataType):
     """Base class for all time types that take a precision argument."""
 
     def __init__(self, precision: int = None, attrs: str = "") -> None:
         super().__init__(attrs)
         self.precision = precision
```

### Comparing `reata-1.1.5/reata/client.py` & `reata-1.1.6/reata/client.py`

 * *Files identical despite different names*

### Comparing `reata-1.1.5/reata/schema.py` & `reata-1.1.6/reata/schema.py`

 * *Files identical despite different names*

### Comparing `reata-1.1.5/reata.egg-info/PKG-INFO` & `reata-1.1.6/reata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reata
-Version: 1.1.5
+Version: 1.1.6
 Summary: A simple MySQL DBAPI wrapper for simplifying data processing pipelines.
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `reata-1.1.5/setup.py` & `reata-1.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from setuptools import find_packages, setup
 
 src = Path(__file__).parent
 
 setup(
     name="reata",
-    version="1.1.5",
+    version="1.1.6",
     description=(
         "A simple MySQL DBAPI wrapper for simplifying "
         "data processing pipelines."
     ),
     long_description=(src/"README.rst").read_text(),
     packages=find_packages(),
     install_requires=[
```

