# Comparing `tmp/dcentrapi-0.3.2.tar.gz` & `tmp/dcentrapi-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.3.2.tar", last modified: Wed Jul 26 11:06:45 2023, max compression
+gzip compressed data, was "dcentrapi-0.3.3.tar", last modified: Thu Aug  3 12:41:59 2023, max compression
```

## Comparing `dcentrapi-0.3.2.tar` & `dcentrapi-0.3.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 davidryan   (501) staff       (20)        0 2023-07-26 11:06:45.191721 dcentrapi-0.3.2/
--rw-r--r--   0 davidryan   (501) staff       (20)     1073 2023-03-07 11:18:55.000000 dcentrapi-0.3.2/LICENSE.rst
--rw-r--r--   0 davidryan   (501) staff       (20)     6780 2023-07-26 11:06:45.191576 dcentrapi-0.3.2/PKG-INFO
--rw-r--r--   0 davidryan   (501) staff       (20)     6211 2023-03-07 11:18:55.000000 dcentrapi-0.3.2/README.md
-drwxr-xr-x   0 davidryan   (501) staff       (20)        0 2023-07-26 11:06:45.190305 dcentrapi-0.3.2/dcentrapi/
--rw-r--r--   0 davidryan   (501) staff       (20)      902 2023-07-26 10:59:22.000000 dcentrapi-0.3.2/dcentrapi/Base.py
--rw-r--r--   0 davidryan   (501) staff       (20)      482 2023-07-25 08:24:00.000000 dcentrapi-0.3.2/dcentrapi/__init__.py
--rw-r--r--   0 davidryan   (501) staff       (20)     8761 2023-07-13 07:44:02.000000 dcentrapi-0.3.2/dcentrapi/eventPolling.py
--rw-r--r--   0 davidryan   (501) staff       (20)      673 2023-07-13 07:44:02.000000 dcentrapi-0.3.2/dcentrapi/gasMonitor.py
--rw-r--r--   0 davidryan   (501) staff       (20)      633 2023-07-13 07:44:02.000000 dcentrapi-0.3.2/dcentrapi/hackMitigation.py
--rw-r--r--   0 davidryan   (501) staff       (20)     3078 2023-03-07 11:18:55.000000 dcentrapi-0.3.2/dcentrapi/merkleTree.py
--rw-r--r--   0 davidryan   (501) staff       (20)      226 2023-07-13 07:44:02.000000 dcentrapi-0.3.2/dcentrapi/requests_dappi.py
--rw-r--r--   0 davidryan   (501) staff       (20)     3107 2023-07-13 07:44:02.000000 dcentrapi-0.3.2/dcentrapi/rpcAggregation.py
--rw-r--r--   0 davidryan   (501) staff       (20)     1758 2023-07-26 11:03:07.000000 dcentrapi-0.3.2/dcentrapi/txSimulation.py
--rw-r--r--   0 davidryan   (501) staff       (20)      837 2023-07-13 07:44:02.000000 dcentrapi-0.3.2/dcentrapi/web3Index.py
-drwxr-xr-x   0 davidryan   (501) staff       (20)        0 2023-07-26 11:06:45.191325 dcentrapi-0.3.2/dcentrapi.egg-info/
--rw-r--r--   0 davidryan   (501) staff       (20)     6780 2023-07-26 11:06:45.000000 dcentrapi-0.3.2/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 davidryan   (501) staff       (20)      441 2023-07-26 11:06:45.000000 dcentrapi-0.3.2/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 davidryan   (501) staff       (20)        1 2023-07-26 11:06:45.000000 dcentrapi-0.3.2/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 davidryan   (501) staff       (20)        9 2023-07-26 11:06:45.000000 dcentrapi-0.3.2/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 davidryan   (501) staff       (20)       10 2023-07-26 11:06:45.000000 dcentrapi-0.3.2/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 davidryan   (501) staff       (20)       38 2023-07-26 11:06:45.191772 dcentrapi-0.3.2/setup.cfg
--rw-r--r--   0 davidryan   (501) staff       (20)     1109 2023-07-26 10:59:16.000000 dcentrapi-0.3.2/setup.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-03 12:41:59.035478 dcentrapi-0.3.3/
+-rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.3.3/LICENSE.rst
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-08-03 12:41:59.035343 dcentrapi-0.3.3/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.3.3/README.md
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-03 12:41:59.034450 dcentrapi-0.3.3/dcentrapi/
+-rw-r--r--   0 oded       (502) staff       (20)      902 2023-08-03 12:41:57.000000 dcentrapi-0.3.3/dcentrapi/Base.py
+-rw-r--r--   0 oded       (502) staff       (20)      482 2023-08-03 11:37:36.000000 dcentrapi-0.3.3/dcentrapi/__init__.py
+-rw-r--r--   0 oded       (502) staff       (20)     8761 2023-06-28 06:59:47.000000 dcentrapi-0.3.3/dcentrapi/eventPolling.py
+-rw-r--r--   0 oded       (502) staff       (20)      673 2023-07-03 08:17:20.000000 dcentrapi-0.3.3/dcentrapi/gasMonitor.py
+-rw-r--r--   0 oded       (502) staff       (20)     1548 2023-08-03 12:36:23.000000 dcentrapi-0.3.3/dcentrapi/hackMitigation.py
+-rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.3.3/dcentrapi/merkleTree.py
+-rw-r--r--   0 oded       (502) staff       (20)      226 2023-06-28 06:59:47.000000 dcentrapi-0.3.3/dcentrapi/requests_dappi.py
+-rw-r--r--   0 oded       (502) staff       (20)     3107 2023-06-28 06:59:47.000000 dcentrapi-0.3.3/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 oded       (502) staff       (20)     1484 2023-08-03 12:37:42.000000 dcentrapi-0.3.3/dcentrapi/test.py
+-rw-r--r--   0 oded       (502) staff       (20)     1758 2023-08-03 11:37:36.000000 dcentrapi-0.3.3/dcentrapi/txSimulation.py
+-rw-r--r--   0 oded       (502) staff       (20)      837 2023-06-28 06:59:47.000000 dcentrapi-0.3.3/dcentrapi/web3Index.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-03 12:41:59.035149 dcentrapi-0.3.3/dcentrapi.egg-info/
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-08-03 12:41:59.000000 dcentrapi-0.3.3/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)      459 2023-08-03 12:41:59.000000 dcentrapi-0.3.3/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 oded       (502) staff       (20)        1 2023-08-03 12:41:59.000000 dcentrapi-0.3.3/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 oded       (502) staff       (20)        9 2023-08-03 12:41:59.000000 dcentrapi-0.3.3/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 oded       (502) staff       (20)       10 2023-08-03 12:41:59.000000 dcentrapi-0.3.3/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 oded       (502) staff       (20)       38 2023-08-03 12:41:59.035524 dcentrapi-0.3.3/setup.cfg
+-rw-r--r--   0 oded       (502) staff       (20)     1109 2023-08-03 12:41:57.000000 dcentrapi-0.3.3/setup.py
```

### Comparing `dcentrapi-0.3.2/LICENSE.rst` & `dcentrapi-0.3.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.2/PKG-INFO` & `dcentrapi-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.3.2
+Version: 0.3.3
 Summary: Dcentralab Pypi packages
-Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -105,9 +103,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

### Comparing `dcentrapi-0.3.2/README.md` & `dcentrapi-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.2/dcentrapi/Base.py` & `dcentrapi-0.3.3/dcentrapi/Base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 class Base:
     def __init__(self, stage, username=None, key=None):
-        self.__version__ = "0.3.2"
+        self.__version__ = "0.3.3"
 
         if stage == "develop":
             self.headers = {"Authorization": username + "," + key}
             self.url = "https://test-api.dcentralab.com/"
             self.web3index_url = "https://test-api.web3index.info/"
         if stage == "staging":
             self.headers = {"Authorization": username + "," + key}
```

### Comparing `dcentrapi-0.3.2/dcentrapi/eventPolling.py` & `dcentrapi-0.3.3/dcentrapi/eventPolling.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.2/dcentrapi/gasMonitor.py` & `dcentrapi-0.3.3/dcentrapi/gasMonitor.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.2/dcentrapi/merkleTree.py` & `dcentrapi-0.3.3/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.2/dcentrapi/rpcAggregation.py` & `dcentrapi-0.3.3/dcentrapi/rpcAggregation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.2/dcentrapi/txSimulation.py` & `dcentrapi-0.3.3/dcentrapi/txSimulation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.2/dcentrapi/web3Index.py` & `dcentrapi-0.3.3/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.2/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.3.3/dcentrapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.3.2
+Version: 0.3.3
 Summary: Dcentralab Pypi packages
-Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -105,9 +103,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

### Comparing `dcentrapi-0.3.2/setup.py` & `dcentrapi-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     return result.group(1)
 
 
 DESCRIPTION = 'Dcentralab Pypi packages'
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 project_name = 'dcentrapi'
-VERSION = "0.3.2"
+VERSION = "0.3.3"
 
 
 # Setting up
 setup(
     name="dcentrapi",
     version=VERSION,
     author="Dcentralab (Niv Shitrit)",
```

