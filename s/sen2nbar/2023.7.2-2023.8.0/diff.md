# Comparing `tmp/sen2nbar-2023.7.2.tar.gz` & `tmp/sen2nbar-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sen2nbar-2023.7.2.tar", last modified: Sun Jul 30 07:12:29 2023, max compression
+gzip compressed data, was "dist/sen2nbar-2023.8.0.tar", last modified: Thu Aug  3 11:50:57 2023, max compression
```

## Comparing `sen2nbar-2023.7.2.tar` & `sen2nbar-2023.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-30 07:12:29.776848 sen2nbar-2023.7.2/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2023-07-09 13:18:33.000000 sen2nbar-2023.7.2/LICENSE
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-07-30 07:12:29.773515 sen2nbar-2023.7.2/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7217 2023-07-09 13:18:33.000000 sen2nbar-2023.7.2/README.md
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-30 07:12:29.773515 sen2nbar-2023.7.2/sen2nbar/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      194 2023-07-30 07:06:33.000000 sen2nbar-2023.7.2/sen2nbar/__init__.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      604 2023-07-09 13:18:34.000000 sen2nbar-2023.7.2/sen2nbar/axioms.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1679 2023-07-09 13:18:34.000000 sen2nbar-2023.7.2/sen2nbar/brdf.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2936 2023-07-09 13:18:34.000000 sen2nbar-2023.7.2/sen2nbar/c_factor.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     3695 2023-07-09 13:18:34.000000 sen2nbar-2023.7.2/sen2nbar/kernels.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     4602 2023-07-29 19:40:59.000000 sen2nbar-2023.7.2/sen2nbar/metadata.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     8292 2023-07-30 06:44:07.000000 sen2nbar-2023.7.2/sen2nbar/nbar.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1558 2023-07-09 13:18:34.000000 sen2nbar-2023.7.2/sen2nbar/utils.py
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-30 07:12:29.773515 sen2nbar-2023.7.2/sen2nbar.egg-info/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-07-30 07:12:29.000000 sen2nbar-2023.7.2/sen2nbar.egg-info/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      339 2023-07-30 07:12:29.000000 sen2nbar-2023.7.2/sen2nbar.egg-info/SOURCES.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-07-30 07:12:29.000000 sen2nbar-2023.7.2/sen2nbar.egg-info/dependency_links.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)       94 2023-07-30 07:12:29.000000 sen2nbar-2023.7.2/sen2nbar.egg-info/requires.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        9 2023-07-30 07:12:29.000000 sen2nbar-2023.7.2/sen2nbar.egg-info/top_level.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-07-30 07:12:29.776848 sen2nbar-2023.7.2/setup.cfg
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1234 2023-07-30 07:06:48.000000 sen2nbar-2023.7.2/setup.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-08-03 11:50:57.295251 sen2nbar-2023.8.0/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2023-07-09 13:18:33.000000 sen2nbar-2023.8.0/LICENSE
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-08-03 11:50:57.291918 sen2nbar-2023.8.0/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7217 2023-07-09 13:18:33.000000 sen2nbar-2023.8.0/README.md
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-08-03 11:50:57.291918 sen2nbar-2023.8.0/sen2nbar/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      194 2023-08-03 11:42:26.000000 sen2nbar-2023.8.0/sen2nbar/__init__.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      604 2023-07-09 13:18:34.000000 sen2nbar-2023.8.0/sen2nbar/axioms.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1679 2023-07-09 13:18:34.000000 sen2nbar-2023.8.0/sen2nbar/brdf.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2956 2023-08-03 08:51:45.000000 sen2nbar-2023.8.0/sen2nbar/c_factor.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     3695 2023-07-09 13:18:34.000000 sen2nbar-2023.8.0/sen2nbar/kernels.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     4602 2023-07-29 19:40:59.000000 sen2nbar-2023.8.0/sen2nbar/metadata.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     8292 2023-07-30 06:44:07.000000 sen2nbar-2023.8.0/sen2nbar/nbar.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1558 2023-07-09 13:18:34.000000 sen2nbar-2023.8.0/sen2nbar/utils.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-08-03 11:50:57.291918 sen2nbar-2023.8.0/sen2nbar.egg-info/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-08-03 11:50:57.000000 sen2nbar-2023.8.0/sen2nbar.egg-info/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      339 2023-08-03 11:50:57.000000 sen2nbar-2023.8.0/sen2nbar.egg-info/SOURCES.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-08-03 11:50:57.000000 sen2nbar-2023.8.0/sen2nbar.egg-info/dependency_links.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)       94 2023-08-03 11:50:57.000000 sen2nbar-2023.8.0/sen2nbar.egg-info/requires.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        9 2023-08-03 11:50:57.000000 sen2nbar-2023.8.0/sen2nbar.egg-info/top_level.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-08-03 11:50:57.295251 sen2nbar-2023.8.0/setup.cfg
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1234 2023-08-03 11:42:17.000000 sen2nbar-2023.8.0/setup.py
```

### Comparing `sen2nbar-2023.7.2/LICENSE` & `sen2nbar-2023.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.2/PKG-INFO` & `sen2nbar-2023.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sen2nbar
-Version: 2023.7.2
+Version: 2023.8.0
 Summary: Nadir BRDF Adjusted Reflectance (NBAR) for Sentinel-2 in Python
 Home-page: https://github.com/ESDS-Leipzig/sen2nbar
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sen2nbar Version: 2023.7.2 Summary: Nadir BRDF
+Metadata-Version: 2.1 Name: sen2nbar Version: 2023.8.0 Summary: Nadir BRDF
 Adjusted Reflectance (NBAR) for Sentinel-2 in Python Home-page: https://
 github.com/ESDS-Leipzig/sen2nbar Author: David Montero Loaiza Author-email:
 dml.mont@gmail.com License: MIT Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
                                     [cubo]
```

### Comparing `sen2nbar-2023.7.2/README.md` & `sen2nbar-2023.8.0/README.md`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.2/sen2nbar/axioms.py` & `sen2nbar-2023.8.0/sen2nbar/axioms.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.2/sen2nbar/brdf.py` & `sen2nbar-2023.8.0/sen2nbar/brdf.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.2/sen2nbar/c_factor.py` & `sen2nbar-2023.8.0/sen2nbar/c_factor.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,10 +103,10 @@
     # Compute the c-factor and extrapolate
     c = c_factor_from_metadata(metadata)
     c = _extrapolate_c_factor(c)
 
     # If the CRSs are different: reproject
     if SOURCE_EPSG != TO_EPSG:
         c = c.rio.write_crs(f"epsg:{SOURCE_EPSG}")
-        c = c.rio.reproject(f"epsg:{TO_EPSG}")
+        c = c.rio.reproject(f"epsg:{TO_EPSG}").drop("spatial_ref")
 
     return c
```

### Comparing `sen2nbar-2023.7.2/sen2nbar/kernels.py` & `sen2nbar-2023.8.0/sen2nbar/kernels.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.2/sen2nbar/metadata.py` & `sen2nbar-2023.8.0/sen2nbar/metadata.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.2/sen2nbar/nbar.py` & `sen2nbar-2023.8.0/sen2nbar/nbar.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.2/sen2nbar/utils.py` & `sen2nbar-2023.8.0/sen2nbar/utils.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.2/sen2nbar.egg-info/PKG-INFO` & `sen2nbar-2023.8.0/sen2nbar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sen2nbar
-Version: 2023.7.2
+Version: 2023.8.0
 Summary: Nadir BRDF Adjusted Reflectance (NBAR) for Sentinel-2 in Python
 Home-page: https://github.com/ESDS-Leipzig/sen2nbar
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sen2nbar Version: 2023.7.2 Summary: Nadir BRDF
+Metadata-Version: 2.1 Name: sen2nbar Version: 2023.8.0 Summary: Nadir BRDF
 Adjusted Reflectance (NBAR) for Sentinel-2 in Python Home-page: https://
 github.com/ESDS-Leipzig/sen2nbar Author: David Montero Loaiza Author-email:
 dml.mont@gmail.com License: MIT Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
                                     [cubo]
```

### Comparing `sen2nbar-2023.7.2/setup.py` & `sen2nbar-2023.8.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     name="sen2nbar",
-    version="2023.7.2",
+    version="2023.8.0",
     url="https://github.com/ESDS-Leipzig/sen2nbar",
     license="MIT",
     author="David Montero Loaiza",
     author_email="dml.mont@gmail.com",
     description="Nadir BRDF Adjusted Reflectance (NBAR) for Sentinel-2 in Python",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
```

