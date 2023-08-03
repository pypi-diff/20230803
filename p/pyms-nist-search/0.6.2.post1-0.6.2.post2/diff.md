# Comparing `tmp/pyms-nist-search-0.6.2.post1.tar.gz` & `tmp/pyms-nist-search-0.6.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyms-nist-search-0.6.2.post1.tar", last modified: Tue Jul 25 19:30:35 2023, max compression
+gzip compressed data, was "pyms-nist-search-0.6.2.post2.tar", last modified: Thu Aug  3 17:17:33 2023, max compression
```

## Comparing `pyms-nist-search-0.6.2.post1.tar` & `pyms-nist-search-0.6.2.post2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 19:30:35.300146 pyms-nist-search-0.6.2.post1/
--rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      611 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8092 2023-07-25 19:30:35.300146 pyms-nist-search-0.6.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6212 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/THIRD_PARTY_COPYRIGHT
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 19:30:35.296146 pyms-nist-search-0.6.2.post1/pyms_nist_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8092 2023-07-25 19:30:34.000000 pyms-nist-search-0.6.2.post1/pyms_nist_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1343 2023-07-25 19:30:35.000000 pyms-nist-search-0.6.2.post1/pyms_nist_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 19:30:34.000000 pyms-nist-search-0.6.2.post1/pyms_nist_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 19:30:34.000000 pyms-nist-search-0.6.2.post1/pyms_nist_search.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-25 19:30:35.000000 pyms-nist-search-0.6.2.post1/pyms_nist_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-25 19:30:35.000000 pyms-nist-search-0.6.2.post1/pyms_nist_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5861 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-07-25 19:30:35.304146 pyms-nist-search-0.6.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2370 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 19:30:35.292146 pyms-nist-search-0.6.2.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 19:30:35.296146 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/
--rw-r--r--   0 runner    (1001) docker     (122)     3162 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/NISTERR.H
--rw-r--r--   0 runner    (1001) docker     (122)    36562 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/NISTMS.H
--rw-r--r--   0 runner    (1001) docker     (122)    20892 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/NISTMS_min.H
--rw-r--r--   0 runner    (1001) docker     (122)     2822 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3788 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     4172 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    10408 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/docker_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)     6226 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/mona_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    63776 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/pyms_nist_search.c
--rw-r--r--   0 runner    (1001) docker     (122)    20454 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/pyms_nist_search_min.c
--rw-r--r--   0 runner    (1001) docker     (122)     9819 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/reference_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4642 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/search_result.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 19:30:35.296146 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     1252 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/templates/msp_template
--rw-r--r--   0 runner    (1001) docker     (122)     3359 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5805 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/win_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 19:30:35.300146 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x64/
--rw-r--r--   0 runner    (1001) docker     (122)   226304 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x64/ctnt66_64.dll
--rw-r--r--   0 runner    (1001) docker     (122)   761344 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x64/nistdl64.dll
--rw-r--r--   0 runner    (1001) docker     (122)     5250 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x64/nistdl64.lib
--rw-r--r--   0 runner    (1001) docker     (122)   761856 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x64/nistdl64_2gb.dll
--rw-r--r--   0 runner    (1001) docker     (122)     5444 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x64/nistdl64_2gb.lib
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 19:30:35.300146 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x86/
--rw-r--r--   0 runner    (1001) docker     (122)   187904 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x86/ctnt66.dll
--rw-r--r--   0 runner    (1001) docker     (122)   634368 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x86/nistdl32.dll
--rw-r--r--   0 runner    (1001) docker     (122)     5422 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x86/nistdl32.lib
--rw-r--r--   0 runner    (1001) docker     (122)   634880 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x86/nistdl32_2gb.dll
--rw-r--r--   0 runner    (1001) docker     (122)     5616 2023-07-25 19:29:57.000000 pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x86/nistdl32_2gb.lib
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:17:33.881098 pyms-nist-search-0.6.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-08-03 17:16:50.000000 pyms-nist-search-0.6.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-08-03 17:16:50.000000 pyms-nist-search-0.6.2.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8092 2023-08-03 17:17:33.881098 pyms-nist-search-0.6.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6212 2023-08-03 17:16:50.000000 pyms-nist-search-0.6.2.post2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-08-03 17:16:50.000000 pyms-nist-search-0.6.2.post2/THIRD_PARTY_COPYRIGHT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:17:33.873098 pyms-nist-search-0.6.2.post2/pyms_nist_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8092 2023-08-03 17:17:33.000000 pyms-nist-search-0.6.2.post2/pyms_nist_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1343 2023-08-03 17:17:33.000000 pyms-nist-search-0.6.2.post2/pyms_nist_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 17:17:33.000000 pyms-nist-search-0.6.2.post2/pyms_nist_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 17:17:33.000000 pyms-nist-search-0.6.2.post2/pyms_nist_search.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-08-03 17:17:33.000000 pyms-nist-search-0.6.2.post2/pyms_nist_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-08-03 17:17:33.000000 pyms-nist-search-0.6.2.post2/pyms_nist_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5861 2023-08-03 17:16:50.000000 pyms-nist-search-0.6.2.post2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-08-03 17:16:50.000000 pyms-nist-search-0.6.2.post2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-08-03 17:17:33.885098 pyms-nist-search-0.6.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2370 2023-08-03 17:16:50.000000 pyms-nist-search-0.6.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:17:33.869098 pyms-nist-search-0.6.2.post2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:17:33.877098 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/
+-rw-r--r--   0 runner    (1001) docker     (122)     3162 2023-08-03 17:16:50.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/NISTERR.H
+-rw-r--r--   0 runner    (1001) docker     (122)    36562 2023-08-03 17:16:50.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/NISTMS.H
+-rw-r--r--   0 runner    (1001) docker     (122)    20892 2023-08-03 17:16:50.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/NISTMS_min.H
+-rw-r--r--   0 runner    (1001) docker     (122)     2822 2023-08-03 17:16:50.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3788 2023-08-03 17:16:50.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     4172 2023-08-03 17:16:50.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10408 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/docker_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6226 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/mona_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    63776 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/pyms_nist_search.c
+-rw-r--r--   0 runner    (1001) docker     (122)    20454 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/pyms_nist_search_min.c
+-rw-r--r--   0 runner    (1001) docker     (122)     9819 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/reference_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4642 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/search_result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:17:33.877098 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     1252 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/templates/msp_template
+-rw-r--r--   0 runner    (1001) docker     (122)     3359 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5805 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/win_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:17:33.877098 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x64/
+-rw-r--r--   0 runner    (1001) docker     (122)   226304 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x64/ctnt66_64.dll
+-rw-r--r--   0 runner    (1001) docker     (122)   761344 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x64/nistdl64.dll
+-rw-r--r--   0 runner    (1001) docker     (122)     5250 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x64/nistdl64.lib
+-rw-r--r--   0 runner    (1001) docker     (122)   761856 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x64/nistdl64_2gb.dll
+-rw-r--r--   0 runner    (1001) docker     (122)     5444 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x64/nistdl64_2gb.lib
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:17:33.881098 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x86/
+-rw-r--r--   0 runner    (1001) docker     (122)   187904 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x86/ctnt66.dll
+-rw-r--r--   0 runner    (1001) docker     (122)   634368 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x86/nistdl32.dll
+-rw-r--r--   0 runner    (1001) docker     (122)     5422 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x86/nistdl32.lib
+-rw-r--r--   0 runner    (1001) docker     (122)   634880 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x86/nistdl32_2gb.dll
+-rw-r--r--   0 runner    (1001) docker     (122)     5616 2023-08-03 17:16:51.000000 pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x86/nistdl32_2gb.lib
```

### Comparing `pyms-nist-search-0.6.2.post1/LICENSE` & `pyms-nist-search-0.6.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/MANIFEST.in` & `pyms-nist-search-0.6.2.post2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/PKG-INFO` & `pyms-nist-search-0.6.2.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyms-nist-search
-Version: 0.6.2.post1
+Version: 0.6.2.post2
 Summary: PyMassSpec extension for searching mass spectra using NIST's Mass Spectrum Search Engine.
 Home-page: https://github.com/domdfcoding/pynist
 Author: Dominic Davis-Foster
 Author-email: dominic@davis-foster.co.uk
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Project-URL: Documentation, https://pynist.readthedocs.io/en/latest
 Project-URL: Issue Tracker, https://github.com/domdfcoding/pynist/issues
@@ -125,15 +125,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/pynist
 	:target: https://github.com/domdfcoding/pynist/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/pynist
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/pynist/v0.6.2.post1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/pynist/v0.6.2.post2
 	:target: https://github.com/domdfcoding/pynist/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/pynist
 	:target: https://github.com/domdfcoding/pynist/commit/master
 	:alt: GitHub last commit
```

### Comparing `pyms-nist-search-0.6.2.post1/README.rst` & `pyms-nist-search-0.6.2.post2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/pynist
 	:target: https://github.com/domdfcoding/pynist/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/pynist
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/pynist/v0.6.2.post1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/pynist/v0.6.2.post2
 	:target: https://github.com/domdfcoding/pynist/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/pynist
 	:target: https://github.com/domdfcoding/pynist/commit/master
 	:alt: GitHub last commit
```

### Comparing `pyms-nist-search-0.6.2.post1/pyms_nist_search.egg-info/PKG-INFO` & `pyms-nist-search-0.6.2.post2/pyms_nist_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyms-nist-search
-Version: 0.6.2.post1
+Version: 0.6.2.post2
 Summary: PyMassSpec extension for searching mass spectra using NIST's Mass Spectrum Search Engine.
 Home-page: https://github.com/domdfcoding/pynist
 Author: Dominic Davis-Foster
 Author-email: dominic@davis-foster.co.uk
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Project-URL: Documentation, https://pynist.readthedocs.io/en/latest
 Project-URL: Issue Tracker, https://github.com/domdfcoding/pynist/issues
@@ -125,15 +125,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/pynist
 	:target: https://github.com/domdfcoding/pynist/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/pynist
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/pynist/v0.6.2.post1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/pynist/v0.6.2.post2
 	:target: https://github.com/domdfcoding/pynist/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/pynist
 	:target: https://github.com/domdfcoding/pynist/commit/master
 	:alt: GitHub last commit
```

### Comparing `pyms-nist-search-0.6.2.post1/pyms_nist_search.egg-info/SOURCES.txt` & `pyms-nist-search-0.6.2.post2/pyms_nist_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/pyproject.toml` & `pyms-nist-search-0.6.2.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools!=61.*,<61,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyms-nist-search"
-version = "0.6.2.post1"
+version = "0.6.2.post2"
 description = "PyMassSpec extension for searching mass spectra using NIST's Mass Spectrum Search Engine."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `pyms-nist-search-0.6.2.post1/requirements.txt` & `pyms-nist-search-0.6.2.post2/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/setup.cfg` & `pyms-nist-search-0.6.2.post2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyms-nist-search
-version = 0.6.2.post1
+version = 0.6.2.post2
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = GNU Lesser General Public License v3 or later (LGPLv3+)
 keywords = 
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, Linux
```

### Comparing `pyms-nist-search-0.6.2.post1/setup.py` & `pyms-nist-search-0.6.2.post2/setup.py`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/NISTERR.H` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/NISTERR.H`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/NISTMS.H` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/NISTMS.H`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/NISTMS_min.H` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/NISTMS_min.H`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/__init__.py` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,11 +69,11 @@
 	# this package
 	from pyms_nist_search.docker_engine import Engine  # noqa: F401
 
 name: str = "PyMassSpec NIST Search"
 __author__: str = "Dominic Davis-Foster"
 __license__: str = "LGPLv3+"
 __maintainer_email__: str = "dominic@davis-foster.co.uk"
-__version__: str = "0.6.2.post1"
+__version__: str = "0.6.2.post2"
 
 __copyright__: str = "2020 Dominic Davis-Foster"
 __email__: str = "dominic@davis-foster.co.uk"
```

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/__init__.pyi` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/base.py` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/base.py`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/docker_engine.py` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/docker_engine.py`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/mona_tools.py` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/mona_tools.py`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/pyms_nist_search.c` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/pyms_nist_search.c`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/pyms_nist_search_min.c` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/pyms_nist_search_min.c`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/reference_data.py` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/reference_data.py`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/search_result.py` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/search_result.py`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/templates/__init__.py` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/utils.py` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/utils.py`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/win_engine.py` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/win_engine.py`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x64/ctnt66_64.dll` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x64/ctnt66_64.dll`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x64/nistdl64.dll` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x64/nistdl64.dll`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x64/nistdl64.lib` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x64/nistdl64.lib`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x64/nistdl64_2gb.dll` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x64/nistdl64_2gb.dll`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x64/nistdl64_2gb.lib` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x64/nistdl64_2gb.lib`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x86/ctnt66.dll` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x86/ctnt66.dll`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x86/nistdl32.dll` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x86/nistdl32.dll`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x86/nistdl32.lib` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x86/nistdl32.lib`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x86/nistdl32_2gb.dll` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x86/nistdl32_2gb.dll`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.6.2.post1/src/pyms_nist_search/x86/nistdl32_2gb.lib` & `pyms-nist-search-0.6.2.post2/src/pyms_nist_search/x86/nistdl32_2gb.lib`

 * *Files identical despite different names*

