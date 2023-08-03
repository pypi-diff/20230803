# Comparing `tmp/pygtop-2.1.4.tar.gz` & `tmp/pygtop-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pygtop-2.1.4.tar", last modified: Thu Jan 31 16:55:02 2019, max compression
+gzip compressed data, was "pygtop-2.1.5.tar", last modified: Thu Aug  3 16:07:45 2023, max compression
```

## Comparing `pygtop-2.1.4.tar` & `pygtop-2.1.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2019-01-31 16:55:02.000000 pygtop-2.1.4/
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2019-01-31 16:55:02.000000 pygtop-2.1.4/pygtop/
--rw-r--r--   0 sam       (1000) sam       (1000)     1261 2019-01-31 16:53:33.000000 pygtop-2.1.4/pygtop/gtop.py
--rw-r--r--   0 sam       (1000) sam       (1000)      150 2019-01-31 16:54:19.000000 pygtop-2.1.4/pygtop/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3822 2019-01-31 16:53:33.000000 pygtop-2.1.4/pygtop/shared.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6135 2019-01-31 16:53:33.000000 pygtop-2.1.4/pygtop/interactions.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2216 2019-01-31 16:53:33.000000 pygtop-2.1.4/pygtop/pdb.py
--rw-r--r--   0 sam       (1000) sam       (1000)      764 2019-01-31 16:53:33.000000 pygtop-2.1.4/pygtop/exceptions.py
--rw-r--r--   0 sam       (1000) sam       (1000)    23741 2019-01-31 16:53:33.000000 pygtop-2.1.4/pygtop/ligands.py
--rw-r--r--   0 sam       (1000) sam       (1000)    14667 2019-01-31 16:53:33.000000 pygtop-2.1.4/pygtop/targets.py
--rw-r--r--   0 sam       (1000) sam       (1000)       38 2019-01-31 16:55:02.000000 pygtop-2.1.4/setup.cfg
--rw-r--r--   0 sam       (1000) sam       (1000)     1028 2019-01-31 16:55:02.000000 pygtop-2.1.4/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)     1024 2019-01-31 16:54:07.000000 pygtop-2.1.4/setup.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2019-01-31 16:55:02.000000 pygtop-2.1.4/pygtop.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2019-01-31 16:55:02.000000 pygtop-2.1.4/pygtop.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)      313 2019-01-31 16:55:02.000000 pygtop-2.1.4/pygtop.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       18 2019-01-31 16:55:02.000000 pygtop-2.1.4/pygtop.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)     1028 2019-01-31 16:55:02.000000 pygtop-2.1.4/pygtop.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)        7 2019-01-31 16:55:02.000000 pygtop-2.1.4/pygtop.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)    13179 2019-01-31 16:53:33.000000 pygtop-2.1.4/README.rst
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-08-03 16:07:45.954981 pygtop-2.1.5/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1078 2016-03-15 20:52:22.000000 pygtop-2.1.5/LICENSE
+-rw-r--r--   0 simon     (1000) simon     (1000)      911 2023-08-03 16:07:45.954981 pygtop-2.1.5/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)    13179 2016-08-04 15:05:50.000000 pygtop-2.1.5/README.rst
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-08-03 16:07:45.953981 pygtop-2.1.5/pygtop/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      150 2018-02-15 17:03:29.000000 pygtop-2.1.5/pygtop/__init__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)      764 2016-07-09 12:22:11.000000 pygtop-2.1.5/pygtop/exceptions.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1262 2023-08-03 16:04:11.000000 pygtop-2.1.5/pygtop/gtop.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     6130 2017-08-23 17:15:09.000000 pygtop-2.1.5/pygtop/interactions.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)    23741 2018-02-15 17:02:59.000000 pygtop-2.1.5/pygtop/ligands.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2216 2016-05-18 19:41:48.000000 pygtop-2.1.5/pygtop/pdb.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3822 2016-08-04 15:01:21.000000 pygtop-2.1.5/pygtop/shared.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)    14667 2016-08-04 15:01:21.000000 pygtop-2.1.5/pygtop/targets.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-08-03 16:07:45.954981 pygtop-2.1.5/pygtop.egg-info/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      911 2023-08-03 16:07:45.000000 pygtop-2.1.5/pygtop.egg-info/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)      321 2023-08-03 16:07:45.000000 pygtop-2.1.5/pygtop.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-08-03 16:07:45.000000 pygtop-2.1.5/pygtop.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       18 2023-08-03 16:07:45.000000 pygtop-2.1.5/pygtop.egg-info/requires.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)        7 2023-08-03 16:07:45.000000 pygtop-2.1.5/pygtop.egg-info/top_level.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-08-03 16:07:45.954981 pygtop-2.1.5/setup.cfg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      937 2023-08-03 16:06:46.000000 pygtop-2.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pygtop-2.1.4/pygtop/gtop.py` & `pygtop-2.1.5/pygtop/gtop.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Functions for interacting with the Guide to PHARMACOLOGY web services."""
 
 import json
 import requests
 
-ROOT_URL = "http://www.guidetopharmacology.org/services/"
+ROOT_URL = "https://www.guidetopharmacology.org/services/"
 
 def get_json_from_gtop(query, attempts=5):
     """Issues a query to the GtoP web services, and returns the resulting JSON.
 
     If it does not get a valid response, it will try again, and if it still
     doesn't get JSON back, it will return None.
```

### Comparing `pygtop-2.1.4/pygtop/shared.py` & `pygtop-2.1.5/pygtop/shared.py`

 * *Files identical despite different names*

### Comparing `pygtop-2.1.4/pygtop/interactions.py` & `pygtop-2.1.5/pygtop/interactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self._action = json_data["action"]
         affinity_values = "".join(
          [char for char in json_data["affinity"] if char in "0123456789. "]
         ).split()
         affinity_values = tuple(sorted([float(val) for val in affinity_values]))
         self._affinity_low = affinity_values[0] if affinity_values else None
         self._affinity_high = affinity_values[-1] if affinity_values else None
-        self._affinity_type = json_data["affinityParameter"]
+        self._affinity_type = json_data["affinityType"]
 
 
     def __repr__(self):
         return "<Interaction (%i --> %s %i)>" % (
          self._ligand_id,
          self._species,
          self._target_id
```

### Comparing `pygtop-2.1.4/pygtop/pdb.py` & `pygtop-2.1.5/pygtop/pdb.py`

 * *Files identical despite different names*

### Comparing `pygtop-2.1.4/pygtop/exceptions.py` & `pygtop-2.1.5/pygtop/exceptions.py`

 * *Files identical despite different names*

### Comparing `pygtop-2.1.4/pygtop/ligands.py` & `pygtop-2.1.5/pygtop/ligands.py`

 * *Files identical despite different names*

### Comparing `pygtop-2.1.4/pygtop/targets.py` & `pygtop-2.1.5/pygtop/targets.py`

 * *Files identical despite different names*

### Comparing `pygtop-2.1.4/PKG-INFO` & `pygtop-2.1.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pygtop
-Version: 2.1.4
+Version: 2.1.5
 Summary: A Python wrapper for the Guide to PHARMACOLOGY API. It provides  a Python interface for access to the GtoP database.
 Home-page: https://pygtop.readthedocs.org
 Author: Sam Ireland
 Author-email: Sam.Ireland@ed.ac.uk
 License: MIT
-Description: UNKNOWN
 Keywords: pharmacology drugs chemistry bioinformatics
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.0
 Classifier: Programming Language :: Python :: 3.1
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
```

### Comparing `pygtop-2.1.4/setup.py` & `pygtop-2.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
  name="pygtop",
- version="2.1.4",
+ version="2.1.5",
  description="A Python wrapper for the Guide to PHARMACOLOGY API. It provides \
  a Python interface for access to the GtoP database.",
  url="https://pygtop.readthedocs.org",
  author="Sam Ireland",
  author_email="Sam.Ireland@ed.ac.uk",
  license="MIT",
  classifiers=[
@@ -17,15 +17,12 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.0",
   "Programming Language :: Python :: 3.1",
   "Programming Language :: Python :: 3.2",
   "Programming Language :: Python :: 3.3",
   "Programming Language :: Python :: 3.4",
   "Programming Language :: Python :: 3.5",
-  "Programming Language :: Python :: 3.6",
-  "Programming Language :: Python :: 3.7",
-
  ],
  keywords="pharmacology drugs chemistry bioinformatics",
  packages=["pygtop"],
  install_requires=["requests", "molecupy"]
 )
```

### Comparing `pygtop-2.1.4/pygtop.egg-info/PKG-INFO` & `pygtop-2.1.5/pygtop.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pygtop
-Version: 2.1.4
+Version: 2.1.5
 Summary: A Python wrapper for the Guide to PHARMACOLOGY API. It provides  a Python interface for access to the GtoP database.
 Home-page: https://pygtop.readthedocs.org
 Author: Sam Ireland
 Author-email: Sam.Ireland@ed.ac.uk
 License: MIT
-Description: UNKNOWN
 Keywords: pharmacology drugs chemistry bioinformatics
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.0
 Classifier: Programming Language :: Python :: 3.1
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
```

### Comparing `pygtop-2.1.4/README.rst` & `pygtop-2.1.5/README.rst`

 * *Files identical despite different names*

