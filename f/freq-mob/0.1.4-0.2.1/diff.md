# Comparing `tmp/freq_mob-0.1.4.tar.gz` & `tmp/freq_mob-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freq_mob-0.1.4.tar", last modified: Sat Jul 29 20:13:37 2023, max compression
+gzip compressed data, was "freq_mob-0.2.1.tar", last modified: Thu Aug  3 00:22:20 2023, max compression
```

## Comparing `freq_mob-0.1.4.tar` & `freq_mob-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-29 20:13:37.523550 freq_mob-0.1.4/
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1073 2023-07-28 04:54:22.000000 freq_mob-0.1.4/LICENSE.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     2235 2023-07-29 20:13:37.514076 freq_mob-0.1.4/PKG-INFO
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1810 2023-07-29 08:06:21.000000 freq_mob-0.1.4/README.md
-drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-29 20:13:37.480298 freq_mob-0.1.4/freq_mob/
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)       71 2023-07-29 20:11:04.000000 freq_mob-0.1.4/freq_mob/__init__.py
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)    17269 2023-07-29 20:12:35.000000 freq_mob-0.1.4/freq_mob/freq_mob.py
-drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-29 20:13:37.512151 freq_mob-0.1.4/freq_mob.egg-info/
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     2235 2023-07-29 20:13:37.000000 freq_mob-0.1.4/freq_mob.egg-info/PKG-INFO
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)      231 2023-07-29 20:13:37.000000 freq_mob-0.1.4/freq_mob.egg-info/SOURCES.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        1 2023-07-29 20:13:37.000000 freq_mob-0.1.4/freq_mob.egg-info/dependency_links.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       46 2023-07-29 20:13:37.000000 freq_mob-0.1.4/freq_mob.egg-info/requires.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        9 2023-07-29 20:13:37.000000 freq_mob-0.1.4/freq_mob.egg-info/top_level.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       38 2023-07-29 20:13:37.523550 freq_mob-0.1.4/setup.cfg
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)      705 2023-07-29 20:10:30.000000 freq_mob-0.1.4/setup.py
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-08-03 00:22:20.390001 freq_mob-0.2.1/
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1073 2023-07-28 04:54:22.000000 freq_mob-0.2.1/LICENSE.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     2235 2023-08-03 00:22:20.390001 freq_mob-0.2.1/PKG-INFO
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1810 2023-07-29 08:06:21.000000 freq_mob-0.2.1/README.md
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-08-03 00:22:20.358775 freq_mob-0.2.1/freq_mob/
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)       71 2023-08-03 00:18:30.000000 freq_mob-0.2.1/freq_mob/__init__.py
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)    17269 2023-08-03 00:19:42.000000 freq_mob-0.2.1/freq_mob/freq_mob.py
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-08-03 00:22:20.390001 freq_mob-0.2.1/freq_mob.egg-info/
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     2235 2023-08-03 00:22:20.000000 freq_mob-0.2.1/freq_mob.egg-info/PKG-INFO
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)      231 2023-08-03 00:22:20.000000 freq_mob-0.2.1/freq_mob.egg-info/SOURCES.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        1 2023-08-03 00:22:20.000000 freq_mob-0.2.1/freq_mob.egg-info/dependency_links.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       51 2023-08-03 00:22:20.000000 freq_mob-0.2.1/freq_mob.egg-info/requires.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        9 2023-08-03 00:22:20.000000 freq_mob-0.2.1/freq_mob.egg-info/top_level.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       38 2023-08-03 00:22:20.405622 freq_mob-0.2.1/setup.cfg
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)      710 2023-08-03 00:18:12.000000 freq_mob-0.2.1/setup.py
```

### Comparing `freq_mob-0.1.4/LICENSE.txt` & `freq_mob-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `freq_mob-0.1.4/PKG-INFO` & `freq_mob-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freq_mob
-Version: 0.1.4
+Version: 0.2.1
 Summary: Monotonic Optimal Binning for Frequency Models
 Home-page: https://github.com/statcompute/freq_mob
 Author: WenSui Liu
 Author-email: liuwensui@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `freq_mob-0.1.4/README.md` & `freq_mob-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `freq_mob-0.1.4/freq_mob/freq_mob.py` & `freq_mob-0.2.1/freq_mob/freq_mob.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # freq_mob/freq_mob.py
-# version 0.1.4, 07/29/2023
+# version 0.2.1, 08/02/2023
 
 import tabulate, numpy, cytoolz, operator
 from scipy.stats import spearmanr
 from sklearn.isotonic import IsotonicRegression as isoreg
 from sklearn.cluster import KMeans as kmeans
 from sklearn import metrics 
 from lightgbm import LGBMRegressor as gbmreg
```

### Comparing `freq_mob-0.1.4/freq_mob.egg-info/PKG-INFO` & `freq_mob-0.2.1/freq_mob.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freq-mob
-Version: 0.1.4
+Version: 0.2.1
 Summary: Monotonic Optimal Binning for Frequency Models
 Home-page: https://github.com/statcompute/freq_mob
 Author: WenSui Liu
 Author-email: liuwensui@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `freq_mob-0.1.4/setup.py` & `freq_mob-0.2.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
  
 with open("README.md", "r") as fh:
   long_description = fh.read()
  
 setuptools.setup(
   name = "freq_mob",
-  version = "0.1.4",
+  version = "0.2.1",
   author = "WenSui Liu",
   author_email = "liuwensui@gmail.com",
   description = "Monotonic Optimal Binning for Frequency Models",
   long_description = long_description,
   long_description_content_type = "text/markdown",
   url = "https://github.com/statcompute/freq_mob",
   packages = setuptools.find_packages(),
-  install_requires = ['numpy', 'scipy', 'sklearn', 'lightgbm', 'tabulate', 'cytoolz'], 
+  install_requires = ['numpy', 'scipy', 'scikit-learn', 'lightgbm', 'tabulate', 'cytoolz'], 
   classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
   ],
 )
```

