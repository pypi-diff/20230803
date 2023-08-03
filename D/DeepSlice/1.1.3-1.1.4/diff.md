# Comparing `tmp/DeepSlice-1.1.3.tar.gz` & `tmp/DeepSlice-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepSlice-1.1.3.tar", last modified: Fri Jul 28 11:35:57 2023, max compression
+gzip compressed data, was "DeepSlice-1.1.4.tar", last modified: Thu Aug  3 11:05:25 2023, max compression
```

## Comparing `DeepSlice-1.1.3.tar` & `DeepSlice-1.1.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.272343 DeepSlice-1.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice/coord_post_processing/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/coord_post_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/coord_post_processing/angle_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/coord_post_processing/depth_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice/coord_post_processing/plane_alignment_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/coord_post_processing/spacing_and_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/metadata/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/metadata/metadata_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice/metadata/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/metadata/volumes/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice/metadata/weights/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/metadata/weights/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice/neural_network/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/neural_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/neural_network/network_architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/neural_network/neural_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.272343 DeepSlice-1.1.3/DeepSlice/read_and_write/
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/read_and_write/QuickNII_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/read_and_write/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-07-28 11:35:57.000000 DeepSlice-1.1.3/DeepSlice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-28 11:35:57.000000 DeepSlice-1.1.3/DeepSlice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:35:57.000000 DeepSlice-1.1.3/DeepSlice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-28 11:35:57.000000 DeepSlice-1.1.3/DeepSlice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 11:35:57.000000 DeepSlice-1.1.3/DeepSlice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-07-28 11:35:57.272343 DeepSlice-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 11:35:57.272343 DeepSlice-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.189206 DeepSlice-1.1.4/DeepSlice/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.189206 DeepSlice-1.1.4/DeepSlice/coord_post_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/coord_post_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/coord_post_processing/angle_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/coord_post_processing/depth_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.189206 DeepSlice-1.1.4/DeepSlice/coord_post_processing/plane_alignment_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/coord_post_processing/spacing_and_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/DeepSlice/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/metadata/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/metadata/metadata_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/DeepSlice/metadata/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/metadata/volumes/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/DeepSlice/metadata/weights/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/metadata/weights/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/DeepSlice/neural_network/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/neural_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/neural_network/network_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/neural_network/neural_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/DeepSlice/read_and_write/
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/read_and_write/QuickNII_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/read_and_write/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.189206 DeepSlice-1.1.4/DeepSlice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-08-03 11:05:25.000000 DeepSlice-1.1.4/DeepSlice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-03 11:05:25.000000 DeepSlice-1.1.4/DeepSlice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:05:25.000000 DeepSlice-1.1.4/DeepSlice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 11:05:25.000000 DeepSlice-1.1.4/DeepSlice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 11:05:25.000000 DeepSlice-1.1.4/DeepSlice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-03 11:05:10.000000 DeepSlice-1.1.4/setup.py
```

### Comparing `DeepSlice-1.1.3/DeepSlice/coord_post_processing/angle_methods.py` & `DeepSlice-1.1.4/DeepSlice/coord_post_processing/angle_methods.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.3/DeepSlice/coord_post_processing/depth_estimation.py` & `DeepSlice-1.1.4/DeepSlice/coord_post_processing/depth_estimation.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.3/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py` & `DeepSlice-1.1.4/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.3/DeepSlice/coord_post_processing/spacing_and_indexing.py` & `DeepSlice-1.1.4/DeepSlice/coord_post_processing/spacing_and_indexing.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.3/DeepSlice/main.py` & `DeepSlice-1.1.4/DeepSlice/main.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.3/DeepSlice/metadata/config.json` & `DeepSlice-1.1.4/DeepSlice/metadata/config.json`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.3/DeepSlice/metadata/metadata_loader.py` & `DeepSlice-1.1.4/DeepSlice/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.3/DeepSlice/neural_network/neural_network.py` & `DeepSlice-1.1.4/DeepSlice/neural_network/neural_network.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.3/DeepSlice/read_and_write/QuickNII_functions.py` & `DeepSlice-1.1.4/DeepSlice/read_and_write/QuickNII_functions.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.3/DeepSlice.egg-info/PKG-INFO` & `DeepSlice-1.1.4/DeepSlice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.1.3
+Version: 1.1.4
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.3.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.4.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.3 Summary: A package to
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.4 Summary: A package to
 align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
 DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
-tags/1.1.3.tar.gz Author: DeepSlice Team Author-email:
+tags/1.1.4.tar.gz Author: DeepSlice Team Author-email:
 harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
 histology,brain,atlas,alignment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python :: 3.7 Description-Content-Type: text/markdown License-File:
 LICENSE ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
```

### Comparing `DeepSlice-1.1.3/DeepSlice.egg-info/SOURCES.txt` & `DeepSlice-1.1.4/DeepSlice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.3/LICENSE` & `DeepSlice-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.3/PKG-INFO` & `DeepSlice-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.1.3
+Version: 1.1.4
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.3.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.4.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.3 Summary: A package to
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.4 Summary: A package to
 align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
 DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
-tags/1.1.3.tar.gz Author: DeepSlice Team Author-email:
+tags/1.1.4.tar.gz Author: DeepSlice Team Author-email:
 harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
 histology,brain,atlas,alignment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python :: 3.7 Description-Content-Type: text/markdown License-File:
 LICENSE ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
```

### Comparing `DeepSlice-1.1.3/README.md` & `DeepSlice-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.3/setup.py` & `DeepSlice-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='DeepSlice',
     packages=find_packages(),
-    version='1.1.3',
+    version='1.1.4',
     license='GPL-3.0',
     description='A package to align histology to 3D brain atlases',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='DeepSlice Team',
     package_data={'DeepSlice': ['metadata/volumes/placeholder.txt', 'metadata/config.json','metadata/weights/*.txt']},
     include_package_data=True,
     author_email='harry.carey@medisin.uio.no',
     url='https://github.com/PolarBean/DeepSlice',
-    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.3.tar.gz',
+    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.4.tar.gz',
     keywords=['histology', 'brain', 'atlas', 'alignment'],
     install_requires=[
         'numpy',
         'scikit-learn',
         'scikit-image',
         'tensorflow==1.15.0',
         'h5py==2.10.0',
```

