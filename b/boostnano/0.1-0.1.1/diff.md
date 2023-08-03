# Comparing `tmp/boostnano-0.1.tar.gz` & `tmp/boostnano-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boostnano-0.1.tar", last modified: Thu Aug  3 07:54:55 2023, max compression
+gzip compressed data, was "boostnano-0.1.1.tar", last modified: Thu Aug  3 08:13:22 2023, max compression
```

## Comparing `boostnano-0.1.tar` & `boostnano-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 07:54:55.716364 boostnano-0.1/
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    15504 2023-08-03 07:53:01.000000 boostnano-0.1/LICENSE.md
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)       76 2023-08-03 07:54:55.716364 boostnano-0.1/PKG-INFO
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     2172 2023-08-03 07:53:01.000000 boostnano-0.1/README.md
-drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 07:54:55.716364 boostnano-0.1/boostnano/
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      335 2023-08-03 07:53:01.000000 boostnano-0.1/boostnano/__init__.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      299 2023-08-03 07:53:01.000000 boostnano-0.1/boostnano/_version.py
--rwxrwxr-x   0 haotiant  (1001) haotiant  (1001)    10459 2023-08-03 07:53:01.000000 boostnano-0.1/boostnano/boostnano_eval.py
--rwxrwxr-x   0 haotiant  (1001) haotiant  (1001)    11323 2023-08-03 07:53:01.000000 boostnano-0.1/boostnano/boostnano_input.py
--rwxrwxr-x   0 haotiant  (1001) haotiant  (1001)     3876 2023-08-03 07:53:01.000000 boostnano-0.1/boostnano/boostnano_model.py
--rwxrwxr-x   0 haotiant  (1001) haotiant  (1001)    12875 2023-08-03 07:53:01.000000 boostnano-0.1/boostnano/boostnano_resquiggle.py
--rwxrwxr-x   0 haotiant  (1001) haotiant  (1001)     8262 2023-08-03 07:53:01.000000 boostnano-0.1/boostnano/boostnano_train.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    12527 2023-08-03 07:53:01.000000 boostnano-0.1/boostnano/hand_label.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     6204 2023-08-03 07:53:01.000000 boostnano-0.1/boostnano/hmm.cpp
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      676 2023-08-03 07:53:01.000000 boostnano-0.1/boostnano/hmm_test.py
-drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 07:54:55.716364 boostnano-0.1/boostnano/model/
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 07:53:01.000000 boostnano-0.1/boostnano/model/__init__.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     2147 2023-08-03 07:53:01.000000 boostnano-0.1/boostnano/test.py
-drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 07:54:55.716364 boostnano-0.1/boostnano.egg-info/
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)       76 2023-08-03 07:54:55.000000 boostnano-0.1/boostnano.egg-info/PKG-INFO
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      464 2023-08-03 07:54:55.000000 boostnano-0.1/boostnano.egg-info/SOURCES.txt
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)        1 2023-08-03 07:54:55.000000 boostnano-0.1/boostnano.egg-info/dependency_links.txt
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)       10 2023-08-03 07:54:55.000000 boostnano-0.1/boostnano.egg-info/top_level.txt
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)       38 2023-08-03 07:54:55.716364 boostnano-0.1/setup.cfg
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      570 2023-08-03 07:54:19.000000 boostnano-0.1/setup.py
+drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 08:13:22.179612 boostnano-0.1.1/
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    15504 2023-08-03 07:53:01.000000 boostnano-0.1.1/LICENSE.md
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)       78 2023-08-03 08:13:22.179612 boostnano-0.1.1/PKG-INFO
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     2172 2023-08-03 07:53:01.000000 boostnano-0.1.1/README.md
+drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 08:13:22.175612 boostnano-0.1.1/boostnano/
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      335 2023-08-03 07:53:01.000000 boostnano-0.1.1/boostnano/__init__.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      301 2023-08-03 08:13:00.000000 boostnano-0.1.1/boostnano/_version.py
+-rwxrwxr-x   0 haotiant  (1001) haotiant  (1001)    10459 2023-08-03 07:53:01.000000 boostnano-0.1.1/boostnano/boostnano_eval.py
+-rwxrwxr-x   0 haotiant  (1001) haotiant  (1001)    11323 2023-08-03 07:53:01.000000 boostnano-0.1.1/boostnano/boostnano_input.py
+-rwxrwxr-x   0 haotiant  (1001) haotiant  (1001)     3876 2023-08-03 07:53:01.000000 boostnano-0.1.1/boostnano/boostnano_model.py
+-rwxrwxr-x   0 haotiant  (1001) haotiant  (1001)    12875 2023-08-03 07:53:01.000000 boostnano-0.1.1/boostnano/boostnano_resquiggle.py
+-rwxrwxr-x   0 haotiant  (1001) haotiant  (1001)     8262 2023-08-03 07:53:01.000000 boostnano-0.1.1/boostnano/boostnano_train.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    12527 2023-08-03 07:53:01.000000 boostnano-0.1.1/boostnano/hand_label.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     6204 2023-08-03 07:53:01.000000 boostnano-0.1.1/boostnano/hmm.cpp
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      676 2023-08-03 07:53:01.000000 boostnano-0.1.1/boostnano/hmm_test.py
+drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 08:13:22.179612 boostnano-0.1.1/boostnano/model/
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 07:53:01.000000 boostnano-0.1.1/boostnano/model/__init__.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     2147 2023-08-03 07:53:01.000000 boostnano-0.1.1/boostnano/test.py
+drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 08:13:22.179612 boostnano-0.1.1/boostnano.egg-info/
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)       78 2023-08-03 08:13:22.000000 boostnano-0.1.1/boostnano.egg-info/PKG-INFO
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      464 2023-08-03 08:13:22.000000 boostnano-0.1.1/boostnano.egg-info/SOURCES.txt
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)        1 2023-08-03 08:13:22.000000 boostnano-0.1.1/boostnano.egg-info/dependency_links.txt
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)       10 2023-08-03 08:13:22.000000 boostnano-0.1.1/boostnano.egg-info/top_level.txt
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)       38 2023-08-03 08:13:22.179612 boostnano-0.1.1/setup.cfg
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      582 2023-08-03 08:11:46.000000 boostnano-0.1.1/setup.py
```

### Comparing `boostnano-0.1/LICENSE.md` & `boostnano-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `boostnano-0.1/README.md` & `boostnano-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `boostnano-0.1/boostnano/boostnano_eval.py` & `boostnano-0.1.1/boostnano/boostnano_eval.py`

 * *Files identical despite different names*

### Comparing `boostnano-0.1/boostnano/boostnano_input.py` & `boostnano-0.1.1/boostnano/boostnano_input.py`

 * *Files identical despite different names*

### Comparing `boostnano-0.1/boostnano/boostnano_model.py` & `boostnano-0.1.1/boostnano/boostnano_model.py`

 * *Files identical despite different names*

### Comparing `boostnano-0.1/boostnano/boostnano_resquiggle.py` & `boostnano-0.1.1/boostnano/boostnano_resquiggle.py`

 * *Files identical despite different names*

### Comparing `boostnano-0.1/boostnano/boostnano_train.py` & `boostnano-0.1.1/boostnano/boostnano_train.py`

 * *Files identical despite different names*

### Comparing `boostnano-0.1/boostnano/hand_label.py` & `boostnano-0.1.1/boostnano/hand_label.py`

 * *Files identical despite different names*

### Comparing `boostnano-0.1/boostnano/hmm.cpp` & `boostnano-0.1.1/boostnano/hmm.cpp`

 * *Files identical despite different names*

### Comparing `boostnano-0.1/boostnano/hmm_test.py` & `boostnano-0.1.1/boostnano/hmm_test.py`

 * *Files identical despite different names*

### Comparing `boostnano-0.1/boostnano/test.py` & `boostnano-0.1.1/boostnano/test.py`

 * *Files identical despite different names*

### Comparing `boostnano-0.1/setup.py` & `boostnano-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 
 ext_modules = [ Extension('boostnano.hmm', sources = ['boostnano/hmm.cpp'],language='c++')]
 exec(open('boostnano/_version.py').read()) #readount the __version__ variable
 setup(
 	name = 'boostnano',
 	version = __version__,
-	include_dirs = [np.get_include()],
+	include_dirs = [np.get_include(),'boostnano'],
 	ext_modules = ext_modules,
 	packages=find_packages(),
     package_data={
         'boostnano': ['boostnano/model/*'],  # Include all .txt files under the 'data' directory
     },
     include_package_data=True,
 )
```

