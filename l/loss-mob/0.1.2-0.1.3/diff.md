# Comparing `tmp/loss_mob-0.1.2.tar.gz` & `tmp/loss_mob-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loss_mob-0.1.2.tar", last modified: Sun Jul 30 17:48:43 2023, max compression
+gzip compressed data, was "loss_mob-0.1.3.tar", last modified: Thu Aug  3 00:12:56 2023, max compression
```

## Comparing `loss_mob-0.1.2.tar` & `loss_mob-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-30 17:48:43.311997 loss_mob-0.1.2/
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1073 2023-07-28 04:54:22.000000 loss_mob-0.1.2/LICENSE.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     2206 2023-07-30 17:48:43.311997 loss_mob-0.1.2/PKG-INFO
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1786 2023-07-30 17:39:40.000000 loss_mob-0.1.2/README.md
-drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-30 17:48:43.280782 loss_mob-0.1.2/loss_mob/
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)       71 2023-07-30 17:46:23.000000 loss_mob-0.1.2/loss_mob/__init__.py
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)    17238 2023-07-30 17:46:40.000000 loss_mob-0.1.2/loss_mob/loss_mob.py
-drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-30 17:48:43.311997 loss_mob-0.1.2/loss_mob.egg-info/
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     2206 2023-07-30 17:48:43.000000 loss_mob-0.1.2/loss_mob.egg-info/PKG-INFO
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)      231 2023-07-30 17:48:43.000000 loss_mob-0.1.2/loss_mob.egg-info/SOURCES.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        1 2023-07-30 17:48:43.000000 loss_mob-0.1.2/loss_mob.egg-info/dependency_links.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       46 2023-07-30 17:48:43.000000 loss_mob-0.1.2/loss_mob.egg-info/requires.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        9 2023-07-30 17:48:43.000000 loss_mob-0.1.2/loss_mob.egg-info/top_level.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       38 2023-07-30 17:48:43.311997 loss_mob-0.1.2/setup.cfg
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)      700 2023-07-30 17:46:08.000000 loss_mob-0.1.2/setup.py
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-08-03 00:12:56.847599 loss_mob-0.1.3/
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1073 2023-07-28 04:54:22.000000 loss_mob-0.1.3/LICENSE.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     2206 2023-08-03 00:12:56.847599 loss_mob-0.1.3/PKG-INFO
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1786 2023-07-30 17:39:40.000000 loss_mob-0.1.3/README.md
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-08-03 00:12:56.803501 loss_mob-0.1.3/loss_mob/
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)       71 2023-08-03 00:09:34.000000 loss_mob-0.1.3/loss_mob/__init__.py
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)    17238 2023-08-03 00:10:45.000000 loss_mob-0.1.3/loss_mob/loss_mob.py
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-08-03 00:12:56.847599 loss_mob-0.1.3/loss_mob.egg-info/
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     2206 2023-08-03 00:12:56.000000 loss_mob-0.1.3/loss_mob.egg-info/PKG-INFO
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)      231 2023-08-03 00:12:56.000000 loss_mob-0.1.3/loss_mob.egg-info/SOURCES.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        1 2023-08-03 00:12:56.000000 loss_mob-0.1.3/loss_mob.egg-info/dependency_links.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       51 2023-08-03 00:12:56.000000 loss_mob-0.1.3/loss_mob.egg-info/requires.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        9 2023-08-03 00:12:56.000000 loss_mob-0.1.3/loss_mob.egg-info/top_level.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       38 2023-08-03 00:12:56.847599 loss_mob-0.1.3/setup.cfg
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)      705 2023-08-03 00:01:02.000000 loss_mob-0.1.3/setup.py
```

### Comparing `loss_mob-0.1.2/LICENSE.txt` & `loss_mob-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `loss_mob-0.1.2/PKG-INFO` & `loss_mob-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loss_mob
-Version: 0.1.2
+Version: 0.1.3
 Summary: Monotonic Optimal Binning for Loss Models
 Home-page: https://github.com/statcompute/loss_mob
 Author: WenSui Liu
 Author-email: liuwensui@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `loss_mob-0.1.2/README.md` & `loss_mob-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `loss_mob-0.1.2/loss_mob/loss_mob.py` & `loss_mob-0.1.3/loss_mob/loss_mob.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # loss_mob/loss_mob.py
-# version 0.1.2, 07/29/2023
+# version 0.1.3, 08/02/2023
 
 import tabulate, numpy, cytoolz, operator
 from scipy.stats import spearmanr
 from sklearn.isotonic import IsotonicRegression as isoreg
 from sklearn.cluster import KMeans as kmeans
 from sklearn import metrics 
 from lightgbm import LGBMRegressor as gbmreg
```

### Comparing `loss_mob-0.1.2/loss_mob.egg-info/PKG-INFO` & `loss_mob-0.1.3/loss_mob.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loss-mob
-Version: 0.1.2
+Version: 0.1.3
 Summary: Monotonic Optimal Binning for Loss Models
 Home-page: https://github.com/statcompute/loss_mob
 Author: WenSui Liu
 Author-email: liuwensui@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `loss_mob-0.1.2/setup.py` & `loss_mob-0.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
  
 with open("README.md", "r") as fh:
   long_description = fh.read()
  
 setuptools.setup(
   name = "loss_mob",
-  version = "0.1.2",
+  version = "0.1.3",
   author = "WenSui Liu",
   author_email = "liuwensui@gmail.com",
   description = "Monotonic Optimal Binning for Loss Models",
   long_description = long_description,
   long_description_content_type = "text/markdown",
   url = "https://github.com/statcompute/loss_mob",
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

