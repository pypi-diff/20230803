# Comparing `tmp/uframe-0.0.8.tar.gz` & `tmp/uframe-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uframe-0.0.8.tar", last modified: Tue Aug  1 11:51:39 2023, max compression
+gzip compressed data, was "uframe-0.0.9.tar", last modified: Wed Aug  2 07:58:10 2023, max compression
```

## Comparing `uframe-0.0.8.tar` & `uframe-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 11:51:39.080892 uframe-0.0.8/
--rw-rw-rw-   0        0        0     1090 2023-07-11 11:16:34.000000 uframe-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     5081 2023-08-01 11:51:39.080892 uframe-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4479 2023-07-11 11:16:34.000000 uframe-0.0.8/README.md
--rw-rw-rw-   0        0        0     1055 2023-07-26 11:56:43.000000 uframe-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      462 2023-08-01 11:51:39.082891 uframe-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      223 2023-07-20 12:52:29.000000 uframe-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 11:51:39.011892 uframe-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 11:51:39.051893 uframe-0.0.8/src/uframe/
--rw-rw-rw-   0        0        0      583 2023-07-21 13:40:49.000000 uframe-0.0.8/src/uframe/__init__.py
--rw-rw-rw-   0        0        0    50775 2023-07-26 12:41:19.000000 uframe-0.0.8/src/uframe/uframe.py
--rw-rw-rw-   0        0        0     6880 2023-07-24 08:36:56.000000 uframe-0.0.8/src/uframe/uframe_from_mice.py
--rw-rw-rw-   0        0        0    12958 2023-07-24 06:43:12.000000 uframe-0.0.8/src/uframe/uframe_instance.py
--rw-rw-rw-   0        0        0      123 2023-07-21 13:40:05.000000 uframe-0.0.8/src/uframe/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-01 11:51:39.066892 uframe-0.0.8/src/uframe.egg-info/
--rw-rw-rw-   0        0        0     5081 2023-08-01 11:51:38.000000 uframe-0.0.8/src/uframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-08-01 11:51:38.000000 uframe-0.0.8/src/uframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 11:51:38.000000 uframe-0.0.8/src/uframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-20 07:40:14.000000 uframe-0.0.8/src/uframe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      142 2023-08-01 11:51:38.000000 uframe-0.0.8/src/uframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-01 11:51:38.000000 uframe-0.0.8/src/uframe.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 11:51:39.079893 uframe-0.0.8/tests/
--rw-rw-rw-   0        0        0      224 2023-07-11 11:16:34.000000 uframe-0.0.8/tests/test_uframe.py
--rw-rw-rw-   0        0        0     2703 2023-07-11 11:16:34.000000 uframe-0.0.8/tests/test_uframe_instance.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:58:10.631978 uframe-0.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-07-11 11:16:34.000000 uframe-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5081 2023-08-02 07:58:10.631978 uframe-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4479 2023-07-11 11:16:34.000000 uframe-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1055 2023-08-02 07:57:03.000000 uframe-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      462 2023-08-02 07:58:10.635906 uframe-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      223 2023-07-20 12:52:29.000000 uframe-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:58:10.588005 uframe-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 07:58:10.603969 uframe-0.0.9/src/uframe/
+-rw-rw-rw-   0        0        0      583 2023-08-02 07:56:29.000000 uframe-0.0.9/src/uframe/__init__.py
+-rw-rw-rw-   0        0        0    50791 2023-08-02 07:56:01.000000 uframe-0.0.9/src/uframe/uframe.py
+-rw-rw-rw-   0        0        0     6880 2023-07-24 08:36:56.000000 uframe-0.0.9/src/uframe/uframe_from_mice.py
+-rw-rw-rw-   0        0        0    12958 2023-07-24 06:43:12.000000 uframe-0.0.9/src/uframe/uframe_instance.py
+-rw-rw-rw-   0        0        0      123 2023-07-21 13:40:05.000000 uframe-0.0.9/src/uframe/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:58:10.619919 uframe-0.0.9/src/uframe.egg-info/
+-rw-rw-rw-   0        0        0     5081 2023-08-02 07:58:10.000000 uframe-0.0.9/src/uframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-08-02 07:58:10.000000 uframe-0.0.9/src/uframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 07:58:10.000000 uframe-0.0.9/src/uframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 07:40:14.000000 uframe-0.0.9/src/uframe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      142 2023-08-02 07:58:10.000000 uframe-0.0.9/src/uframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 07:58:10.000000 uframe-0.0.9/src/uframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 07:58:10.631978 uframe-0.0.9/tests/
+-rw-rw-rw-   0        0        0      224 2023-07-11 11:16:34.000000 uframe-0.0.9/tests/test_uframe.py
+-rw-rw-rw-   0        0        0     2703 2023-07-11 11:16:34.000000 uframe-0.0.9/tests/test_uframe_instance.py
```

### Comparing `uframe-0.0.8/LICENSE` & `uframe-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uframe-0.0.8/PKG-INFO` & `uframe-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uframe
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for handling uncertain data
 Author: Christian Amesoeder and Michael Hagn
 Author-email: Christian Amesoder <christian.amesoeder@informatik.uni-regensburg.de>, Michael Hagn <michael.hagn@stud.uni-regensburg.de>
 Project-URL: Homepage, https://github.com/URWI2/uframe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uframe-0.0.8/README.md` & `uframe-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `uframe-0.0.8/pyproject.toml` & `uframe-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 warn_unreachable = true
 warn_unused_configs = true
 no_implicit_reexport = true
 
 
 [project]
 name = "uframe"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Christian Amesoder", email="christian.amesoeder@informatik.uni-regensburg.de" },
   { name="Michael Hagn", email="michael.hagn@stud.uni-regensburg.de" }
 ]
 description = "Package for handling uncertain data"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `uframe-0.0.8/src/uframe/__init__.py` & `uframe-0.0.9/src/uframe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for uframe."""
 
 __author__ = """Christian Amesoeder and Michael Hagn"""
 __email__ = 'christian.amesoeder@informatik.uni-regensburg.de'
-__version__ = '0.0.1'
+__version__ = '0.0.9'
 
 
 from .uframe import uframe
 from .uframe_instance import uframe_instance
 from .utils import load_uframe
 from.uframe_from_mice import (uframe_from_array_mice_2,
             uframe_from_array_mice,
```

### Comparing `uframe-0.0.8/src/uframe/uframe.py` & `uframe-0.0.9/src/uframe/uframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1045,15 +1045,15 @@
         #if not, append new keys with them and give them the correct index 
         
         
         return 
             
     
     def __getitem__(self, index):
-        return uframe(new = self.data[index], colnames = self._columns, rownames = self._rows[index])
+        return uframe(new = [self.data[i] for i in index], colnames = self._columns, rownames = self._rows[index])
 
     # TO DO: function which takes i,j and returns element of uframe (need marginal distributions for that)
 
     def add_cat_values(self, cat_value_dict):
         
         if hasattr(self, 'cat_values'):
             self.cat_values.update(cat_value_dict)
@@ -1084,13 +1084,13 @@
             
 
 if __name__ == "__main__":
    
     
    
    import scipy.stats as ss  
-   a = uframe(new = [ss.norm(1), ss.norm(10), ss.norm(112)])
+   a = uf.uframe(new = [ss.norm(1), ss.norm(10), ss.norm(112)])
    a[0:1].sample()
```

### Comparing `uframe-0.0.8/src/uframe/uframe_from_mice.py` & `uframe-0.0.9/src/uframe/uframe_from_mice.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.8/src/uframe/uframe_instance.py` & `uframe-0.0.9/src/uframe/uframe_instance.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.8/src/uframe.egg-info/PKG-INFO` & `uframe-0.0.9/src/uframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uframe
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for handling uncertain data
 Author: Christian Amesoeder and Michael Hagn
 Author-email: Christian Amesoder <christian.amesoeder@informatik.uni-regensburg.de>, Michael Hagn <michael.hagn@stud.uni-regensburg.de>
 Project-URL: Homepage, https://github.com/URWI2/uframe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uframe-0.0.8/tests/test_uframe_instance.py` & `uframe-0.0.9/tests/test_uframe_instance.py`

 * *Files identical despite different names*

