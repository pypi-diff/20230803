# Comparing `tmp/pyabf-2.3.7.tar.gz` & `tmp/pyabf-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyabf-2.3.7.tar", last modified: Tue Sep 27 00:25:46 2022, max compression
+gzip compressed data, was "pyabf-2.3.8.tar", last modified: Wed Aug  2 23:21:43 2023, max compression
```

## Comparing `pyabf-2.3.7.tar` & `pyabf-2.3.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:25:46.089851 pyabf-2.3.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-27 00:25:27.000000 pyabf-2.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-27 00:25:27.000000 pyabf-2.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2022-09-27 00:25:46.089851 pyabf-2.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-09-27 00:25:27.000000 pyabf-2.3.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:25:46.085851 pyabf-2.3.7/pyabf/
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33410 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:25:46.089851 pyabf-2.3.7/pyabf/abf1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11786 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf1/headerV1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:25:46.089851 pyabf-2.3.7/pyabf/abf2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3871 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf2/adcSection.py
--rw-r--r--   0 runner    (1001) docker     (121)     5241 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf2/dacSection.py
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf2/dataSection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf2/epochPerDacSection.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf2/epochSection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3278 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf2/headerV2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4477 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf2/protocolSection.py
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf2/section.py
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf2/stringsSection.py
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf2/synchArraySection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf2/tagSection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abf2/userListSection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3044 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abfReader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3946 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/abfWriter.py
--rw-r--r--   0 runner    (1001) docker     (121)     5718 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/atf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2698 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/names.py
--rw-r--r--   0 runner    (1001) docker     (121)     5722 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     5935 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/stimulus.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:25:46.089851 pyabf-2.3.7/pyabf/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9160 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/tools/abfHeaderDisplay.py
--rw-r--r--   0 runner    (1001) docker     (121)     3774 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/tools/ap.py
--rw-r--r--   0 runner    (1001) docker     (121)     7579 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/tools/generate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2906 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/tools/memtest.py
--rw-r--r--   0 runner    (1001) docker     (121)    10070 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/tools/memtestMath.py
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/tools/sweep.py
--rw-r--r--   0 runner    (1001) docker     (121)    21677 2022-09-27 00:25:27.000000 pyabf-2.3.7/pyabf/waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:25:46.089851 pyabf-2.3.7/pyabf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2022-09-27 00:25:46.000000 pyabf-2.3.7/pyabf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-09-27 00:25:46.000000 pyabf-2.3.7/pyabf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 00:25:46.000000 pyabf-2.3.7/pyabf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-27 00:25:46.000000 pyabf-2.3.7/pyabf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-27 00:25:46.000000 pyabf-2.3.7/pyabf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 00:25:46.089851 pyabf-2.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-09-27 00:25:27.000000 pyabf-2.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:21:43.335317 pyabf-2.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 23:21:33.000000 pyabf-2.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 23:21:33.000000 pyabf-2.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-02 23:21:43.335317 pyabf-2.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-02 23:21:33.000000 pyabf-2.3.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:21:43.331317 pyabf-2.3.8/pyabf/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33411 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:21:43.331317 pyabf-2.3.8/pyabf/abf1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf1/headerV1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:21:43.335317 pyabf-2.3.8/pyabf/abf2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf2/adcSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf2/dacSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf2/dataSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf2/epochPerDacSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf2/epochSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf2/headerV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf2/protocolSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf2/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf2/stringsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf2/synchArraySection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf2/tagSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abf2/userListSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abfReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/abfWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/atf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/stimulus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:21:43.335317 pyabf-2.3.8/pyabf/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/tools/abfHeaderDisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/tools/ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/tools/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/tools/memtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/tools/memtestMath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/tools/sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-08-02 23:21:33.000000 pyabf-2.3.8/pyabf/waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:21:43.331317 pyabf-2.3.8/pyabf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-02 23:21:43.000000 pyabf-2.3.8/pyabf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-02 23:21:43.000000 pyabf-2.3.8/pyabf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:21:43.000000 pyabf-2.3.8/pyabf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 23:21:43.000000 pyabf-2.3.8/pyabf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 23:21:43.000000 pyabf-2.3.8/pyabf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 23:21:43.335317 pyabf-2.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-08-02 23:21:33.000000 pyabf-2.3.8/setup.py
```

### Comparing `pyabf-2.3.7/LICENSE` & `pyabf-2.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/PKG-INFO` & `pyabf-2.3.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyabf
-Version: 2.3.7
+Version: 2.3.8
 Summary: Python library for reading files in Axon Binary Format (ABF)
 Home-page: http://swharden.com/pyabf
 Author: Scott W Harden
 Author-email: SWHarden@gmail.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/swharden/pyABF/issues
 Project-URL: Source, https://github.com/swharden/pyABF
@@ -18,24 +18,23 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 
 pyABF: a pure-Python ABF file reader
 ====================================
 
 **pyABF** provides a Python interface to electrophysiology files in the Axon Binary Format (ABF).
-pyABF supports Python versions 3.6 and newer and does not use obscure libraries
-(just the standard libraries plus numpy and matplotlib). pyABF supports reading
-of ABF1 and ABF2 files, and can write ABF1 files.
+pyABF supports Python 3 and does not use obscure libraries (just numpy and matplotlib). 
+pyABF supports reading ABF1 and ABF2 files and can write ABF1 files.
 
 .. class:: no-web
 
     .. image:: http://swharden.com/pyabf/graphics/action-potentials-small.png
         :alt: pyABF electrophysiology data analysis with Python and Matplotlib
         :align: center
```

### Comparing `pyabf-2.3.7/README.rst` & `pyabf-2.3.8/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 pyABF: a pure-Python ABF file reader
 ====================================
 
 **pyABF** provides a Python interface to electrophysiology files in the Axon Binary Format (ABF).
-pyABF supports Python versions 3.6 and newer and does not use obscure libraries
-(just the standard libraries plus numpy and matplotlib). pyABF supports reading
-of ABF1 and ABF2 files, and can write ABF1 files.
+pyABF supports Python 3 and does not use obscure libraries (just numpy and matplotlib). 
+pyABF supports reading ABF1 and ABF2 files and can write ABF1 files.
 
 .. class:: no-web
 
     .. image:: http://swharden.com/pyabf/graphics/action-potentials-small.png
         :alt: pyABF electrophysiology data analysis with Python and Matplotlib
         :align: center
```

### Comparing `pyabf-2.3.7/pyabf/__init__.py` & `pyabf-2.3.8/pyabf/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """
 pyABF - A Python interface to files in the Axon Binary Format (ABF)
     by Scott Harden
 
 Documentation and code examples, and more can be found at:
     https://github.com/swharden/pyABF
 """
-__version__ = '2.3.7'
+__version__ = '2.3.8'
 
 import sys
 import os
 
-if sys.version_info < (3, 6):
-    sys.stdout.write("ERROR: pyabf "+__version__+" requires Python 3.6 or newer.\n")
-    sys.stdout.write("pyabf 2.1.10 was the last version to support Python 2.7 and Python 3.5\n")
-    sys.exit(1)
-
 from pyabf.abf import ABF
 from pyabf.atf import ATF
 
 def info():
     """display information about the pyabf package."""
     import platform
     import numpy
```

### Comparing `pyabf-2.3.7/pyabf/abf.py` & `pyabf-2.3.8/pyabf/abf.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                  cacheStimulusFiles: bool = True,
                  stimulusFileFolder: bool = None):
         """
         Load header and sweep data from an ABF file.
 
         ### Parameters
 
-        1. abfFilePath -- path to the ABF file
+        1. abfFilePath -- path to the ABF file.
 
         2. loadData -- whether or not to load sweep data values from the file immediately on instantiation.
         Set this to False if you intent to iterate many ABF files rapidly and only inspect their headers.
 
         3. cacheStimulusFiles -- Some ABF files use a source ABF as a stimulus file to control its DAC.
         This module automatically loads the stimulus waveform from disk if it is available.
         This parameter controls whether stimulus files should be stored in memory at the module level.
```

### Comparing `pyabf-2.3.7/pyabf/abf1/headerV1.py` & `pyabf-2.3.8/pyabf/abf1/headerV1.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/abf2/adcSection.py` & `pyabf-2.3.8/pyabf/abf2/adcSection.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/abf2/dacSection.py` & `pyabf-2.3.8/pyabf/abf2/dacSection.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/abf2/epochPerDacSection.py` & `pyabf-2.3.8/pyabf/abf2/epochPerDacSection.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/abf2/epochSection.py` & `pyabf-2.3.8/pyabf/abf2/epochSection.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/abf2/headerV2.py` & `pyabf-2.3.8/pyabf/abf2/headerV2.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/abf2/protocolSection.py` & `pyabf-2.3.8/pyabf/abf2/protocolSection.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/abf2/stringsSection.py` & `pyabf-2.3.8/pyabf/abf2/stringsSection.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/abf2/synchArraySection.py` & `pyabf-2.3.8/pyabf/abf2/synchArraySection.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/abf2/tagSection.py` & `pyabf-2.3.8/pyabf/abf2/tagSection.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/abf2/userListSection.py` & `pyabf-2.3.8/pyabf/abf2/userListSection.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/abfReader.py` & `pyabf-2.3.8/pyabf/abfReader.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/abfWriter.py` & `pyabf-2.3.8/pyabf/abfWriter.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/atf.py` & `pyabf-2.3.8/pyabf/atf.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/filter.py` & `pyabf-2.3.8/pyabf/filter.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/names.py` & `pyabf-2.3.8/pyabf/names.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/plot.py` & `pyabf-2.3.8/pyabf/plot.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/stimulus.py` & `pyabf-2.3.8/pyabf/stimulus.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/tools/abfHeaderDisplay.py` & `pyabf-2.3.8/pyabf/tools/abfHeaderDisplay.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,18 +74,21 @@
 
     def showText(self):
         print(self.getText())
 
     def getText(self):
         """Return information about all objects as markdown-formatted text."""
         text = ""
-        for item in self.things:
-            name, value = item
-            if value == "~SECTION~":
-                text += "\n### %s ###\n" % name
+        for name, value in self.things:
+            if value is None:
+                text += "%s" % (name)+"\n"
+            elif not isinstance(value, str):
+                text += "%s = %s\n" % (name, value)
+            elif value == "~SECTION~":
+                text += "\n %s \n" % name
             elif value == "~DOCS~":
                 text += "\n~~~ %s ~~~\n" % name
             elif str(name) == "~CODE~":
                 text += value+"\n"
             else:
                 if value is None:
                     text += "%s" % (name)+"\n"
```

### Comparing `pyabf-2.3.7/pyabf/tools/ap.py` & `pyabf-2.3.8/pyabf/tools/ap.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/tools/generate.py` & `pyabf-2.3.8/pyabf/tools/generate.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/tools/memtest.py` & `pyabf-2.3.8/pyabf/tools/memtest.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,14 @@
 https://swharden.com/blog/2020-10-11-model-neuron-ltspice
 """
 
 import pyabf
 import pyabf.tools.sweep
 import pyabf.tools.memtestMath
 import numpy as np
-import warnings
-
-warnings.warn("The pyabf package is designed for reading ABF files (not analyzing them). " +
-              "This module is experimental, provided only for backwards compatibility, and its API may change in future releases. " +
-              "Users are encouraged to write their own ABF analysis code.")
 
 
 class Memtest:
     def __init__(self, abf: pyabf.ABF, channel: int = 0):
         """
         This object contains passive cell membrane properties calculated from 
         each sweep an episodic protocol containing a voltage-clamp step.
```

### Comparing `pyabf-2.3.7/pyabf/tools/memtestMath.py` & `pyabf-2.3.8/pyabf/tools/memtestMath.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/tools/sweep.py` & `pyabf-2.3.8/pyabf/tools/sweep.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf/waveform.py` & `pyabf-2.3.8/pyabf/waveform.py`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/pyabf.egg-info/PKG-INFO` & `pyabf-2.3.8/pyabf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyabf
-Version: 2.3.7
+Version: 2.3.8
 Summary: Python library for reading files in Axon Binary Format (ABF)
 Home-page: http://swharden.com/pyabf
 Author: Scott W Harden
 Author-email: SWHarden@gmail.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/swharden/pyABF/issues
 Project-URL: Source, https://github.com/swharden/pyABF
@@ -18,24 +18,23 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 
 pyABF: a pure-Python ABF file reader
 ====================================
 
 **pyABF** provides a Python interface to electrophysiology files in the Axon Binary Format (ABF).
-pyABF supports Python versions 3.6 and newer and does not use obscure libraries
-(just the standard libraries plus numpy and matplotlib). pyABF supports reading
-of ABF1 and ABF2 files, and can write ABF1 files.
+pyABF supports Python 3 and does not use obscure libraries (just numpy and matplotlib). 
+pyABF supports reading ABF1 and ABF2 files and can write ABF1 files.
 
 .. class:: no-web
 
     .. image:: http://swharden.com/pyabf/graphics/action-potentials-small.png
         :alt: pyABF electrophysiology data analysis with Python and Matplotlib
         :align: center
```

### Comparing `pyabf-2.3.7/pyabf.egg-info/SOURCES.txt` & `pyabf-2.3.8/pyabf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyabf-2.3.7/setup.py` & `pyabf-2.3.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import os
 from setuptools import setup
 from setuptools import find_packages
 import sys
 
-if sys.version_info[:2] < (3, 6):
-    raise RuntimeError("Python version >= 3.6 required.")
+if sys.version_info[:2] < (3, 8):
+    raise RuntimeError("Python version >= 3.8 required.")
 
 # load the description
 PATH_HERE = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.abspath(PATH_HERE+"/README.rst")) as f:
     long_description = f.read()
 
 # standard pypi stuff
 setup(
     name='pyabf',
-    version='2.3.7',
+    version='2.3.8',
     author='Scott W Harden',
     author_email='SWHarden@gmail.com',
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     packages=find_packages(),
     include_package_data=True,
     url='http://swharden.com/pyabf',
     license='MIT License',
     platforms='any',
     description='Python library for reading files in Axon Binary Format (ABF)',
     long_description=long_description,
```

