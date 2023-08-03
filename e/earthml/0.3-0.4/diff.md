# Comparing `tmp/earthml-0.3.tar.gz` & `tmp/earthml-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthml-0.3.tar", last modified: Tue Aug  1 19:45:55 2023, max compression
+gzip compressed data, was "earthml-0.4.tar", last modified: Thu Aug  3 19:26:50 2023, max compression
```

## Comparing `earthml-0.3.tar` & `earthml-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 19:45:55.147952 earthml-0.3/
--rw-r--r--   0 akhilchhibber   (501) staff       (20)     1070 2023-08-01 18:41:39.000000 earthml-0.3/LICENSE
--rw-r--r--   0 akhilchhibber   (501) staff       (20)     2019 2023-08-01 19:45:55.147839 earthml-0.3/PKG-INFO
--rw-r--r--   0 akhilchhibber   (501) staff       (20)     1379 2023-08-01 19:45:18.000000 earthml-0.3/README.md
-drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 19:45:55.147008 earthml-0.3/earthml/
--rw-r--r--   0 akhilchhibber   (501) staff       (20)       33 2023-08-01 18:30:59.000000 earthml-0.3/earthml/__init__.py
--rw-r--r--   0 akhilchhibber   (501) staff       (20)    13831 2023-08-01 18:57:08.000000 earthml-0.3/earthml/geodata_to_geohash.py
-drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 19:45:55.147678 earthml-0.3/earthml.egg-info/
--rw-r--r--   0 akhilchhibber   (501) staff       (20)     2019 2023-08-01 19:45:55.000000 earthml-0.3/earthml.egg-info/PKG-INFO
--rw-r--r--   0 akhilchhibber   (501) staff       (20)      230 2023-08-01 19:45:55.000000 earthml-0.3/earthml.egg-info/SOURCES.txt
--rw-r--r--   0 akhilchhibber   (501) staff       (20)        1 2023-08-01 19:45:55.000000 earthml-0.3/earthml.egg-info/dependency_links.txt
--rw-r--r--   0 akhilchhibber   (501) staff       (20)       38 2023-08-01 19:45:55.000000 earthml-0.3/earthml.egg-info/requires.txt
--rw-r--r--   0 akhilchhibber   (501) staff       (20)        8 2023-08-01 19:45:55.000000 earthml-0.3/earthml.egg-info/top_level.txt
--rw-r--r--   0 akhilchhibber   (501) staff       (20)       38 2023-08-01 19:45:55.147990 earthml-0.3/setup.cfg
--rw-r--r--   0 akhilchhibber   (501) staff       (20)     1030 2023-08-01 19:45:18.000000 earthml-0.3/setup.py
+drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-03 19:26:50.467686 earthml-0.4/
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     1070 2023-08-01 18:41:39.000000 earthml-0.4/LICENSE
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     2034 2023-08-03 19:26:50.467558 earthml-0.4/PKG-INFO
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     1394 2023-08-03 19:25:37.000000 earthml-0.4/README.md
+drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-03 19:26:50.466564 earthml-0.4/earthml/
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)       33 2023-08-01 18:30:59.000000 earthml-0.4/earthml/__init__.py
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)    13831 2023-08-01 18:57:08.000000 earthml-0.4/earthml/geodata_to_geohash.py
+drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-03 19:26:50.467374 earthml-0.4/earthml.egg-info/
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     2034 2023-08-03 19:26:50.000000 earthml-0.4/earthml.egg-info/PKG-INFO
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)      230 2023-08-03 19:26:50.000000 earthml-0.4/earthml.egg-info/SOURCES.txt
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)        1 2023-08-03 19:26:50.000000 earthml-0.4/earthml.egg-info/dependency_links.txt
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)       38 2023-08-03 19:26:50.000000 earthml-0.4/earthml.egg-info/requires.txt
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)        8 2023-08-03 19:26:50.000000 earthml-0.4/earthml.egg-info/top_level.txt
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)       38 2023-08-03 19:26:50.467730 earthml-0.4/setup.cfg
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     1030 2023-08-03 19:25:24.000000 earthml-0.4/setup.py
```

### Comparing `earthml-0.3/LICENSE` & `earthml-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `earthml-0.3/PKG-INFO` & `earthml-0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: earthml
-Version: 0.3
+Version: 0.4
 Summary: A library to Perform different possible operations on Geo-Spatial Dataset
 Home-page: https://github.com/akhilchibber
 Author: Akhil Chhibber
 Author-email: akhil.chibber@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# EarthML - Geodata to Geohash
+# EarthML: Geospatial Data Analysis Made Easy
 
 EarthML is a Python library designed to convert geospatial datasets into a single geohash representing the smallest possible area that covers the entire dataset. It supports various formats, including `.shp`, `.geojson`, `.tif`, `.las`, `.png`, `.jpg`, and `.jpeg`.
 
 ## Goal
 
 The goal of EarthML is to simplify the process of converting geospatial data into a geohash. It can handle different file formats and automatically calculate the geohash that fits the entire study area.
```

### Comparing `earthml-0.3/README.md` & `earthml-0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# EarthML - Geodata to Geohash
+# EarthML: Geospatial Data Analysis Made Easy
 
 EarthML is a Python library designed to convert geospatial datasets into a single geohash representing the smallest possible area that covers the entire dataset. It supports various formats, including `.shp`, `.geojson`, `.tif`, `.las`, `.png`, `.jpg`, and `.jpeg`.
 
 ## Goal
 
 The goal of EarthML is to simplify the process of converting geospatial data into a geohash. It can handle different file formats and automatically calculate the geohash that fits the entire study area.
```

### Comparing `earthml-0.3/earthml/geodata_to_geohash.py` & `earthml-0.4/earthml/geodata_to_geohash.py`

 * *Files identical despite different names*

### Comparing `earthml-0.3/earthml.egg-info/PKG-INFO` & `earthml-0.4/earthml.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: earthml
-Version: 0.3
+Version: 0.4
 Summary: A library to Perform different possible operations on Geo-Spatial Dataset
 Home-page: https://github.com/akhilchibber
 Author: Akhil Chhibber
 Author-email: akhil.chibber@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# EarthML - Geodata to Geohash
+# EarthML: Geospatial Data Analysis Made Easy
 
 EarthML is a Python library designed to convert geospatial datasets into a single geohash representing the smallest possible area that covers the entire dataset. It supports various formats, including `.shp`, `.geojson`, `.tif`, `.las`, `.png`, `.jpg`, and `.jpeg`.
 
 ## Goal
 
 The goal of EarthML is to simplify the process of converting geospatial data into a geohash. It can handle different file formats and automatically calculate the geohash that fits the entire study area.
```

### Comparing `earthml-0.3/setup.py` & `earthml-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the content of the README.md file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='earthml',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     install_requires=[
         'fiona',
         'rasterio',
         'pygeohash',
         'Pillow',
         'laspy',
```

