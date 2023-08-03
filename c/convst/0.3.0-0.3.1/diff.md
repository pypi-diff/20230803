# Comparing `tmp/convst-0.3.0.tar.gz` & `tmp/convst-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convst-0.3.0.tar", last modified: Tue Jun 13 08:51:57 2023, max compression
+gzip compressed data, was "convst-0.3.1.tar", last modified: Thu Aug  3 07:34:02 2023, max compression
```

## Comparing `convst-0.3.0.tar` & `convst-0.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.359172 convst-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-06-13 08:51:44.000000 convst-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-06-13 08:51:57.359172 convst-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8316 2023-06-13 08:51:44.000000 convst-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.351172 convst-0.3.0/convst/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-06-13 08:51:44.000000 convst-0.3.0/convst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.351172 convst-0.3.0/convst/classifiers/
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-06-13 08:51:44.000000 convst-0.3.0/convst/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11754 2023-06-13 08:51:44.000000 convst-0.3.0/convst/classifiers/rdst_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     9636 2023-06-13 08:51:44.000000 convst-0.3.0/convst/classifiers/rdst_ridge.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.351172 convst-0.3.0/convst/interpreters/
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-06-13 08:51:44.000000 convst-0.3.0/convst/interpreters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18122 2023-06-13 08:51:44.000000 convst-0.3.0/convst/interpreters/rdst_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.355172 convst-0.3.0/convst/transformers/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19798 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/_commons.py
--rw-r--r--   0 runner    (1001) docker     (122)     4535 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/_input_transformers.py
--rw-r--r--   0 runner    (1001) docker     (122)    15510 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/_multivariate_same_length.py
--rw-r--r--   0 runner    (1001) docker     (122)    16916 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/_multivariate_variable_length.py
--rw-r--r--   0 runner    (1001) docker     (122)    12561 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/_univariate_same_length.py
--rw-r--r--   0 runner    (1001) docker     (122)    13600 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/_univariate_variable_length.py
--rw-r--r--   0 runner    (1001) docker     (122)    20936 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/rdst.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.359172 convst-0.3.0/convst/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      119 2023-06-13 08:51:44.000000 convst-0.3.0/convst/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-06-13 08:51:44.000000 convst-0.3.0/convst/utils/checks_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9241 2023-06-13 08:51:44.000000 convst-0.3.0/convst/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7270 2023-06-13 08:51:44.000000 convst-0.3.0/convst/utils/experiments_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3466 2023-06-13 08:51:44.000000 convst-0.3.0/convst/utils/numba_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    20896 2023-06-13 08:51:44.000000 convst-0.3.0/convst/utils/plot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.351172 convst-0.3.0/convst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-06-13 08:51:57.000000 convst-0.3.0/convst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-13 08:51:57.000000 convst-0.3.0/convst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 08:51:57.000000 convst-0.3.0/convst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 08:51:57.000000 convst-0.3.0/convst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      279 2023-06-13 08:51:57.000000 convst-0.3.0/convst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-13 08:51:57.000000 convst-0.3.0/convst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1890 2023-06-13 08:51:44.000000 convst-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-13 08:51:57.359172 convst-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-06-13 08:51:44.000000 convst-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.359172 convst-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-06-13 08:51:44.000000 convst-0.3.0/tests/test_checks_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-06-13 08:51:44.000000 convst-0.3.0/tests/test_commons_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-06-13 08:51:44.000000 convst-0.3.0/tests/test_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4484 2023-06-13 08:51:44.000000 convst-0.3.0/tests/test_rdst.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 07:34:02.041613 convst-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-08-03 07:33:49.000000 convst-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    10774 2023-08-03 07:34:02.041613 convst-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7903 2023-08-03 07:33:49.000000 convst-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 07:34:02.037613 convst-0.3.1/convst/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-08-03 07:33:49.000000 convst-0.3.1/convst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 07:34:02.037613 convst-0.3.1/convst/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-08-03 07:33:49.000000 convst-0.3.1/convst/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11540 2023-08-03 07:33:49.000000 convst-0.3.1/convst/classifiers/rdst_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9614 2023-08-03 07:33:49.000000 convst-0.3.1/convst/classifiers/rdst_ridge.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 07:34:02.037613 convst-0.3.1/convst/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-08-03 07:33:49.000000 convst-0.3.1/convst/interpreters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17523 2023-08-03 07:33:49.000000 convst-0.3.1/convst/interpreters/rdst_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 07:34:02.037613 convst-0.3.1/convst/transformers/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-08-03 07:33:49.000000 convst-0.3.1/convst/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19798 2023-08-03 07:33:49.000000 convst-0.3.1/convst/transformers/_commons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4786 2023-08-03 07:33:49.000000 convst-0.3.1/convst/transformers/_input_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15510 2023-08-03 07:33:49.000000 convst-0.3.1/convst/transformers/_multivariate_same_length.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16916 2023-08-03 07:33:49.000000 convst-0.3.1/convst/transformers/_multivariate_variable_length.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12561 2023-08-03 07:33:49.000000 convst-0.3.1/convst/transformers/_univariate_same_length.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13600 2023-08-03 07:33:49.000000 convst-0.3.1/convst/transformers/_univariate_variable_length.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20936 2023-08-03 07:33:49.000000 convst-0.3.1/convst/transformers/rdst.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 07:34:02.041613 convst-0.3.1/convst/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-08-03 07:33:49.000000 convst-0.3.1/convst/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-08-03 07:33:49.000000 convst-0.3.1/convst/utils/checks_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9613 2023-08-03 07:33:49.000000 convst-0.3.1/convst/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7270 2023-08-03 07:33:49.000000 convst-0.3.1/convst/utils/experiments_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3466 2023-08-03 07:33:49.000000 convst-0.3.1/convst/utils/numba_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20896 2023-08-03 07:33:49.000000 convst-0.3.1/convst/utils/plot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 07:34:02.037613 convst-0.3.1/convst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10774 2023-08-03 07:34:02.000000 convst-0.3.1/convst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-08-03 07:34:02.000000 convst-0.3.1/convst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 07:34:02.000000 convst-0.3.1/convst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 07:34:02.000000 convst-0.3.1/convst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-08-03 07:34:02.000000 convst-0.3.1/convst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-03 07:34:02.000000 convst-0.3.1/convst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1910 2023-08-03 07:33:49.000000 convst-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-08-03 07:34:02.041613 convst-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-08-03 07:33:49.000000 convst-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 07:34:02.041613 convst-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-08-03 07:33:49.000000 convst-0.3.1/tests/test_checks_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-08-03 07:33:49.000000 convst-0.3.1/tests/test_commons_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-08-03 07:33:49.000000 convst-0.3.1/tests/test_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4484 2023-08-03 07:33:49.000000 convst-0.3.1/tests/test_rdst.py
```

### Comparing `convst-0.3.0/LICENSE` & `convst-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/PKG-INFO` & `convst-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convst
-Version: 0.3.0
+Version: 0.3.1
 Summary: The Random Dilation Shapelet Transform algorithm and associated works
 Home-page: https://github.com/baraline/convst
 Download-URL: https://pypi.org/project/convst/#files
 Author: Antoine Guillaume
 Author-email: Antoine Guillaume <antoine.guillaume45@gmail.com>
 License: BSD 2-Clause License
         
@@ -45,21 +45,22 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # This package is moving to the aeon-toolkit.
 Starting from v0.3.0, this package will not be updated, bugfixes will still be included if issues are raised.
-You can already find an updated version of RDST in the Aeon package at https://github.com/aeon-toolkit/ . Further improvements are planned for further speeding up RDST, these improvement will only be implemented in aeon.
+You can already find RDST in the Aeon package at https://github.com/aeon-toolkit/ . Further improvements are planned for further speeding up RDST, these improvement will only be implemented in aeon.
 All the functionnalities of this package will be ported into Aeon when I got some time, for now, only the transformer for univariate and multivariate series of even length have been implemented.
 
 # Readme
 Welcome to the convst repository. It contains the implementation of the `Random Dilated Shapelet Transform (RDST)` along with other works in the same area.
 This work was supported by the following organisations:
 
 <p float="center">
@@ -87,17 +88,14 @@
 
 The recommended way to install the latest stable version is to use pip with `pip install convst`. To install the package from sources, you can download the latest version on GitHub and run `python setup.py install`. This should install the package and automatically look for the dependencies using `pip`. 
 
 We recommend doing this in a new virtual environment using anaconda to avoid any conflict with an existing installation. If you wish to install dependencies individually, you can see dependencies in the `setup.py` file.
 
 An optional dependency that can help speed up numba, which is used in our implementation, is the Intel vector math library (SVML). When using conda it can be installed by running `conda install -c numba icc_rt`. I didn't test the behavior with AMD processors, but I suspect it won't work.
 
-If you are using RDST in some specific settings such as an HPC cluster and are getting errors, take a loot at [issue #24](https://github.com/baraline/convst/issues/24), you may need to change the numba compilation settings to not using function caching (see [this example](https://github.com/baraline/convst/blob/main/examples/Changing_numba_options.py)). THIS SHOULD BE FIXED WITH v0.3.0
-
-
 ## Tutorial
 We give here a minimal example to run the `RDST` algorithm on any dataset of the UCR archive using the aeon API to get datasets:
 
 ```python
 
 from convst.classifiers import R_DST_Ridge
 from convst.utils.dataset_utils import load_UCR_UEA_dataset_split
```

### Comparing `convst-0.3.0/README.md` & `convst-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This package is moving to the aeon-toolkit.
 Starting from v0.3.0, this package will not be updated, bugfixes will still be included if issues are raised.
-You can already find an updated version of RDST in the Aeon package at https://github.com/aeon-toolkit/ . Further improvements are planned for further speeding up RDST, these improvement will only be implemented in aeon.
+You can already find RDST in the Aeon package at https://github.com/aeon-toolkit/ . Further improvements are planned for further speeding up RDST, these improvement will only be implemented in aeon.
 All the functionnalities of this package will be ported into Aeon when I got some time, for now, only the transformer for univariate and multivariate series of even length have been implemented.
 
 # Readme
 Welcome to the convst repository. It contains the implementation of the `Random Dilated Shapelet Transform (RDST)` along with other works in the same area.
 This work was supported by the following organisations:
 
 <p float="center">
@@ -32,17 +32,14 @@
 
 The recommended way to install the latest stable version is to use pip with `pip install convst`. To install the package from sources, you can download the latest version on GitHub and run `python setup.py install`. This should install the package and automatically look for the dependencies using `pip`. 
 
 We recommend doing this in a new virtual environment using anaconda to avoid any conflict with an existing installation. If you wish to install dependencies individually, you can see dependencies in the `setup.py` file.
 
 An optional dependency that can help speed up numba, which is used in our implementation, is the Intel vector math library (SVML). When using conda it can be installed by running `conda install -c numba icc_rt`. I didn't test the behavior with AMD processors, but I suspect it won't work.
 
-If you are using RDST in some specific settings such as an HPC cluster and are getting errors, take a loot at [issue #24](https://github.com/baraline/convst/issues/24), you may need to change the numba compilation settings to not using function caching (see [this example](https://github.com/baraline/convst/blob/main/examples/Changing_numba_options.py)). THIS SHOULD BE FIXED WITH v0.3.0
-
-
 ## Tutorial
 We give here a minimal example to run the `RDST` algorithm on any dataset of the UCR archive using the aeon API to get datasets:
 
 ```python
 
 from convst.classifiers import R_DST_Ridge
 from convst.utils.dataset_utils import load_UCR_UEA_dataset_split
```

### Comparing `convst-0.3.0/convst/classifiers/rdst_ensemble.py` & `convst-0.3.1/convst/classifiers/rdst_ensemble.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,283 +1,278 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 
 from joblib import Parallel
 
-from convst.utils.checks_utils import (check_n_jobs, check_array_1D,
-                                       check_is_boolean, check_is_numeric)
-from convst.transformers import R_DST
-from convst.transformers._input_transformers import (
-    Raw, Derivate, Periodigram
+from convst.utils.checks_utils import (
+    check_n_jobs,
+    check_array_1D,
+    check_is_boolean,
+    check_is_numeric,
 )
+from convst.transformers import R_DST
+from convst.transformers._input_transformers import Raw, Derivate, Periodigram
 from sklearn.utils.fixes import delayed
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.linear_model import RidgeClassifierCV
 from sklearn.utils.extmath import softmax
 from sklearn.metrics import accuracy_score, make_scorer
 from sklearn.preprocessing import StandardScaler
 from sklearn.pipeline import make_pipeline
 
 from sklearn.utils.validation import check_is_fitted, check_random_state
 
 from numba import set_num_threads
 
-class _internalRidgeCV(RidgeClassifierCV): 
+
+class _internalRidgeCV(RidgeClassifierCV):
     def __init__(self, **kwargs):
         super().__init__(
-            store_cv_values=True,
-            scoring=make_scorer(accuracy_score),
-            **kwargs
+            store_cv_values=True, scoring=make_scorer(accuracy_score), **kwargs
         )
-    
+
     def fit(self, X, y):
         self.scaler = StandardScaler().fit(X)
         return super().fit(self.scaler.transform(X), y)
-    
+
     def predict(self, X):
         return super().predict(self.scaler.transform(X))
-    
+
     def predict_proba(self, X):
         d = self.decision_function(self.scaler.transform(X))
         if len(d.shape) == 1:
             d = np.c_[-d, d]
         return softmax(d)
-    
+
     def get_loocv_train_acc(self, y_train):
         if self.store_cv_values:
             alpha_idx = np.where(self.alphas == self.alpha_)[0]
-            cv_vals = self.cv_values_[:,:,alpha_idx]
+            cv_vals = self.cv_values_[:, :, alpha_idx]
             if cv_vals.shape[1] == 1:
-                return accuracy_score((cv_vals[:,0]>0).astype(int), y_train)
+                return accuracy_score((cv_vals[:, 0] > 0).astype(int), y_train)
             else:
                 return accuracy_score(cv_vals.argmax(axis=1), y_train)
         else:
-            raise ValueError('LOOCV training accuracy is only available with store_cv_values to True')
+            raise ValueError(
+                "LOOCV training accuracy is only available with store_cv_values to True"
+            )
 
 
 def _parallel_fit(X, y, model):
     return model.fit(X, y)
 
+
 def _parallel_predict(X, model, w):
     return model.predict_proba(X) * w
 
+
 class R_DST_Ensemble(BaseEstimator, ClassifierMixin):
     """
-    
+
     Parameters
     ----------
     transform_type : str, optional
         Type of transformer to use. Based on the characteristics of the input
         time series, different class of transformer must be used, for example
         the tranformer for univariate series is not the same as for
         multivariate ones for run-time optimization reasons.
         The default is 'auto', which automatically select the transformer based
         on the data passed in the fit method.
     phase_invariance : bool, optional
-        Wheter to use phase invariance for shapelet sampling and distance 
+        Wheter to use phase invariance for shapelet sampling and distance
         computation. The default is False.
     alpha : float, optional
-        The alpha similarity parameter, the higher the value, the lower the 
-        allowed number of common indexes with previously sampled shapelets 
+        The alpha similarity parameter, the higher the value, the lower the
+        allowed number of common indexes with previously sampled shapelets
         when sampling a new one with similar parameters. It can cause the
         number of sampled shapelets to be lower than n_shapelets if the
         whole search space has been covered. The default is 0.5.
     normalize_output : boolean, optional
-        Wheter to normalize the argmin and shapelet occurrence feature by the 
+        Wheter to normalize the argmin and shapelet occurrence feature by the
         length of the series from which it was extracted. This is mostly useful
         for variable length time series. The default is False.
     n_samples : float, optional
         Proportion (in ]0,1]) of samples to consider for the shapelet
         extraction. The default is None, meaning that all samples are used.
     n_shapelets : int, optional
         The maximum number of shapelet to be sampled. The default is 10_000.
     shapelet_lengths : array, optional
         The set of possible length for shapelets. The values can be integers
-        to specify an absolute length, or a float, to specify a length relative 
+        to specify an absolute length, or a float, to specify a length relative
         to the input time series length. The default is [11].
     shapelet_lengths_bounds : array, optional
-        An 1D array with two elements containing the min and max possible 
+        An 1D array with two elements containing the min and max possible
         length for shapelet candidate, can be int or float. The default is
         None, meaning that shapelet_lengths parameter is used.
     lengths_bounds_reduction : float, optional
-        A float in ]0,1], quantifying the proportion of lengths to explore 
+        A float in ]0,1], quantifying the proportion of lengths to explore
         between the min and max bounds of shapelet_lengths_bounds. The default
         is 0.5. For example, with bounds as [4,10], and a reduction of 0.5,
         only [4,6,8,10] will be considered as possible lengths.
     prime_dilations : bool, optional
-        If True, only dilation with prime values will be considered for 
+        If True, only dilation with prime values will be considered for
         shapelet candidates. This will greatly speed-up the algorithm
         for long time series and/or short shapelet length, possibly at the cost
         of some accuracy.
     proba_norm : float, optional
-        The proportion of shapelets that will use a normalized distance 
+        The proportion of shapelets that will use a normalized distance
         function, which induce scale invariance. The default is 0.8.
     percentiles : array, optional
         The two perceniles used to select the lambda threshold used to compute
         the Shapelet Occurrence feature. The default is [5,10].
     n_jobs : int, optional
         The number of threads used to sample and compute the distance vectors.
         The default is 1, -1 means all available cores.
     random_state : object, optional
         The seed for the random state. The default is None.
     max_channels : int, optional
-        The maximum number of feature possibly considered by a multivariate 
+        The maximum number of feature possibly considered by a multivariate
         shapelet. The default is None, meaning max_chanels=n_features.
     min_len : int, optional
         The minimum length of an input time series for variable length input.
         The default is None, meaning min_len=min(n_timestamps) on the training data.
         This can cause error if a shorter serie sis present in the test set.
     class_weight : object, optional
          Class weight option of Ridge Classifier, either None, "balanced" or a
          custom dictionnary of weight for each class. The default is None.
     fit_intercept : bool, optional
          If True, the intercept term will be fitted during the ridge regression.
          The default is True.
     alphas : array, optional
-         Array of alpha values to try which influence regularization strength, 
+         Array of alpha values to try which influence regularization strength,
          must be a positive float. The default is np.logspace(-4,4,20).
     """
+
     def __init__(
         self,
         n_shapelets_per_estimator=10000,
         shapelet_lengths=[11],
         shapelet_lengths_bounds=None,
         lengths_bounds_reduction=0.5,
         prime_dilations=False,
         n_samples=None,
         n_jobs=1,
         prefer=None,
-        require='sharedmem',
+        require="sharedmem",
         random_state=None,
         shp_alpha=0.5,
         a_w=4,
         proba_norm=[0.8, 0.8, 0.8],
         phase_invariance=False,
         input_transformers=None,
-        transform_type='auto',
+        transform_type="auto",
         normalize_output=False,
-        percentiles=[5,10],
+        percentiles=[5, 10],
         max_channels=None,
         min_len=None,
         class_weight=None,
         fit_intercept=True,
-        alphas_ridge=list(np.logspace(-4,4,20))
+        alphas_ridge=list(np.logspace(-4, 4, 20)),
     ):
         self.transform_type = transform_type
         self.phase_invariance = check_is_boolean(phase_invariance)
         self.normalize_output = check_is_boolean(normalize_output)
-        self.n_samples = check_is_numeric(n_samples) if n_samples is not None else n_samples
+        self.n_samples = (
+            check_is_numeric(n_samples) if n_samples is not None else n_samples
+        )
         self.shapelet_lengths_bounds = shapelet_lengths_bounds
         self.prime_dilations = check_is_boolean(prime_dilations)
         self.percentiles = percentiles
         self.random_state = check_random_state(random_state)
-        self.max_channels=max_channels
-        self.min_len=min_len
+        self.max_channels = max_channels
+        self.min_len = min_len
         self.lengths_bounds_reduction = lengths_bounds_reduction
         self.n_shapelets_per_estimator = check_is_numeric(n_shapelets_per_estimator)
         self.shapelet_lengths = check_array_1D(shapelet_lengths)
         self.n_jobs = n_jobs
-        
+
         self.prefer = prefer
         self.require = require
         self.shp_alpha = check_is_numeric(shp_alpha)
         self.a_w = check_is_numeric(a_w)
         self.proba_norm = check_array_1D(proba_norm)
-        
+
         self.alphas_ridge = alphas_ridge
         self.class_weight = class_weight
         self.fit_intercept = fit_intercept
-      
+
         if input_transformers is None:
-            self.input_transformers = [
-                Raw(),
-                Derivate(),
-                Periodigram()
-            ]
+            self.input_transformers = [Raw(), Derivate(), Periodigram()]
         else:
             self.input_transformers = input_transformers
-        
+
         if len(self.input_transformers) != len(self.proba_norm):
             raise ValueError(
-                'The length of proba norm array should be equal to the'
-                ' length of the input transformers array, but found '
-                '{} for proba_norm and {} for input transformers'.format(
-                 len(self.proba_norm), len(self.input_transformers))
+                "The length of proba norm array should be equal to the"
+                " length of the input transformers array, but found "
+                "{} for proba_norm and {} for input transformers".format(
+                    len(self.proba_norm), len(self.input_transformers)
+                )
             )
-        
+
     def _more_tags(self):
         return {
             "capability:variable_length": True,
             "capability:univariate": True,
-            "capability:multivariate": True
+            "capability:multivariate": True,
         }
-        
+
     def _manage_n_jobs(self):
         total_jobs = check_n_jobs(self.n_jobs)
-        self.n_jobs = min(len(self.input_transformers),total_jobs)
-        self.n_jobs_rdst = max(1,total_jobs//self.n_jobs)
-        
+        self.n_jobs = min(len(self.input_transformers), total_jobs)
+        self.n_jobs_rdst = max(1, total_jobs // self.n_jobs)
+
     def fit(self, X, y):
         self._manage_n_jobs()
         set_num_threads(self.n_jobs_rdst)
-        models = Parallel(
-            n_jobs=self.n_jobs,
-            prefer=self.prefer,
-            require=self.require
-        )(
+        models = Parallel(n_jobs=self.n_jobs, prefer=self.prefer, require=self.require)(
             delayed(_parallel_fit)(
-                X, y, 
+                X,
+                y,
                 make_pipeline(
                     self.input_transformers[i],
                     R_DST(
                         n_shapelets=self.n_shapelets_per_estimator,
-                        alpha=self.shp_alpha, n_samples=self.n_samples, 
+                        alpha=self.shp_alpha,
+                        n_samples=self.n_samples,
                         proba_norm=self.proba_norm[i],
                         n_jobs=False,
                         shapelet_lengths=self.shapelet_lengths,
                         phase_invariance=self.phase_invariance,
                         prime_dilations=self.prime_dilations,
                         shapelet_lengths_bounds=self.shapelet_lengths_bounds,
                         lengths_bounds_reduction=self.lengths_bounds_reduction,
                         transform_type=self.transform_type,
                         percentiles=self.percentiles,
                         min_len=self.min_len,
                         max_channels=self.max_channels,
-                        random_state=self.random_state
+                        random_state=self.random_state,
                     ),
                     _internalRidgeCV(
                         alphas=self.alphas_ridge,
                         fit_intercept=self.fit_intercept,
-                        class_weight=self.class_weight
-                    )
-                )
+                        class_weight=self.class_weight,
+                    ),
+                ),
             )
             for i in range(len(self.input_transformers))
         )
-            
+
         self.models = models
-        self.model_weights = [model['_internalridgecv'].get_loocv_train_acc(y)**self.a_w
-                              for model in models]
+        self.model_weights = [
+            model["_internalridgecv"].get_loocv_train_acc(y) ** self.a_w
+            for model in models
+        ]
         return self
 
-
     def predict(self, X):
-        check_is_fitted(self, ['model_weights'])
+        check_is_fitted(self, ["model_weights"])
         preds_proba = Parallel(
-            n_jobs=self.n_jobs,
-            prefer=self.prefer,
-            require=self.require
+            n_jobs=self.n_jobs, prefer=self.prefer, require=self.require
         )(
-            delayed(_parallel_predict)(
-                X,
-                self.models[i],
-                self.model_weights[i]
-            )
+            delayed(_parallel_predict)(X, self.models[i], self.model_weights[i])
             for i in range(len(self.model_weights))
         )
-        #n_samples, n_models
+        # n_samples, n_models
         preds_proba = np.asarray(preds_proba).sum(axis=0)
         return preds_proba.argmax(axis=1)
-
-    
-
```

### Comparing `convst-0.3.0/convst/classifiers/rdst_ridge.py` & `convst-0.3.1/convst/classifiers/rdst_ridge.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 from convst.transformers import R_DST
 
 from convst.utils.checks_utils import check_n_jobs
 from sklearn.metrics import accuracy_score
 
 from numba import set_num_threads
 
+
 class R_DST_Ridge(BaseEstimator, ClassifierMixin):
     """
-    A wrapper class which use R_DST as a transformer, followed by a Ridge 
+    A wrapper class which use R_DST as a transformer, followed by a Ridge
     Classifier.
-    
+
     Attributes
     ----------
     classifier : object
         A sklearn pipeline for RidgeClassifierCV with L2 regularization.
     transformer : object
         An instance of R_DST.
 
@@ -32,138 +33,138 @@
         Type of transformer to use. Based on the characteristics of the input
         time series, different class of transformer must be used, for example
         the tranformer for univariate series is not the same as for
         multivariate ones for run-time optimization reasons.
         The default is 'auto', which automatically select the transformer based
         on the data passed in the fit method.
     phase_invariance : bool, optional
-        Wheter to use phase invariance for shapelet sampling and distance 
+        Wheter to use phase invariance for shapelet sampling and distance
         computation. The default is False.
     alpha : float, optional
-        The alpha similarity parameter, the higher the value, the lower the 
-        allowed number of common indexes with previously sampled shapelets 
+        The alpha similarity parameter, the higher the value, the lower the
+        allowed number of common indexes with previously sampled shapelets
         when sampling a new one with similar parameters. It can cause the
         number of sampled shapelets to be lower than n_shapelets if the
         whole search space has been covered. The default is 0.5.
     normalize_output : boolean, optional
-        Wheter to normalize the argmin and shapelet occurrence feature by the 
+        Wheter to normalize the argmin and shapelet occurrence feature by the
         length of the series from which it was extracted. This is mostly useful
         for variable length time series. The default is False.
     n_samples : float, optional
         Proportion (in ]0,1]) of samples to consider for the shapelet
         extraction. The default is None, meaning that all samples are used.
     n_shapelets : int, optional
         The maximum number of shapelet to be sampled. The default is 10_000.
     shapelet_lengths : array, optional
         The set of possible length for shapelets. The values can be integers
-        to specify an absolute length, or a float, to specify a length relative 
+        to specify an absolute length, or a float, to specify a length relative
         to the input time series length. The default is [11].
     shapelet_lengths_bounds : array, optional
-        An 1D array with two elements containing the min and max possible 
+        An 1D array with two elements containing the min and max possible
         length for shapelet candidate, can be int or float. The default is
         None, meaning that shapelet_lengths parameter is used.
     lengths_bounds_reduction : float, optional
-        A float in ]0,1], quantifying the proportion of lengths to explore 
+        A float in ]0,1], quantifying the proportion of lengths to explore
         between the min and max bounds of shapelet_lengths_bounds. The default
         is 0.5. For example, with bounds as [4,10], and a reduction of 0.5,
         only [4,6,8,10] will be considered as possible lengths.
     prime_dilations : bool, optional
-        If True, only dilation with prime values will be considered for 
+        If True, only dilation with prime values will be considered for
         shapelet candidates. This will greatly speed-up the algorithm
         for long time series and/or short shapelet length, possibly at the cost
         of some accuracy.
     proba_norm : float, optional
-        The proportion of shapelets that will use a normalized distance 
+        The proportion of shapelets that will use a normalized distance
         function, which induce scale invariance. The default is 0.8.
     percentiles : array, optional
         The two perceniles used to select the lambda threshold used to compute
         the Shapelet Occurrence feature. The default is [5,10].
     n_jobs : int, optional
         The number of threads used to sample and compute the distance vectors.
         The default is 1, -1 means all available cores.
     random_state : object, optional
         The seed for the random state. The default is None.
     max_channels : int, optional
-        The maximum number of feature possibly considered by a multivariate 
+        The maximum number of feature possibly considered by a multivariate
         shapelet. The default is None, meaning max_chanels=n_features.
     min_len : int, optional
         The minimum length of an input time series for variable length input.
         The default is None, meaning min_len=min(n_timestamps) on the training data.
         This can cause error if a shorter serie sis present in the test set.
     class_weight : object, optional
          Class weight option of Ridge Classifier, either None, "balanced" or a
          custom dictionnary of weight for each class. The default is None.
      fit_intercept : bool, optional
          If True, the intercept term will be fitted during the ridge regression.
          The default is True.
      alphas : array, optional
-         Array of alpha values to try which influence regularization strength, 
+         Array of alpha values to try which influence regularization strength,
          must be a positive float.
          The default is np.logspace(-4,4,20).
     """
-    
+
     def __init__(
-        self, 
-        transform_type='auto',
+        self,
+        transform_type="auto",
         phase_invariance=False,
         alpha=0.5,
         normalize_output=False,
         n_samples=None,
         n_shapelets=10_000,
         shapelet_lengths=[11],
         shapelet_lengths_bounds=None,
         lengths_bounds_reduction=0.5,
         prime_dilations=False,
         proba_norm=0.8,
-        percentiles=[5,10],
+        percentiles=[5, 10],
         n_jobs=1,
         random_state=None,
         min_len=None,
-        class_weight=None, 
+        class_weight=None,
         fit_intercept=True,
-        alphas_ridge=list(np.logspace(-4,4,20))
+        alphas_ridge=list(np.logspace(-4, 4, 20)),
     ):
-        self.alphas_ridge=alphas_ridge
-        self.class_weight=class_weight
-        self.fit_intercept=fit_intercept
-        self.transform_type=transform_type
-        self.phase_invariance=phase_invariance
-        self.prime_dilations=prime_dilations
-        self.alpha=alpha
-        self.normalize_output=normalize_output
-        self.n_samples=n_samples
-        self.shapelet_lengths_bounds=shapelet_lengths_bounds
-        self.lengths_bounds_reduction=lengths_bounds_reduction
-        self.n_shapelets=n_shapelets
-        self.shapelet_lengths=shapelet_lengths
-        self.proba_norm=proba_norm
-        self.percentiles=percentiles
+        self.alphas_ridge = alphas_ridge
+        self.class_weight = class_weight
+        self.fit_intercept = fit_intercept
+        self.transform_type = transform_type
+        self.phase_invariance = phase_invariance
+        self.prime_dilations = prime_dilations
+        self.alpha = alpha
+        self.normalize_output = normalize_output
+        self.n_samples = n_samples
+        self.shapelet_lengths_bounds = shapelet_lengths_bounds
+        self.lengths_bounds_reduction = lengths_bounds_reduction
+        self.n_shapelets = n_shapelets
+        self.shapelet_lengths = shapelet_lengths
+        self.proba_norm = proba_norm
+        self.percentiles = percentiles
         if isinstance(n_jobs, bool):
-            self.n_jobs=n_jobs
+            self.n_jobs = n_jobs
         else:
-            self.n_jobs=check_n_jobs(n_jobs)
+            self.n_jobs = check_n_jobs(n_jobs)
             set_num_threads(self.n_jobs)
-        self.random_state=random_state
-        self.min_len=min_len
-    
+        self.random_state = random_state
+        self.min_len = min_len
+
     def _more_tags(self):
         return {
             "capability:variable_length": True,
             "capability:univariate": True,
-            "capability:multivariate": True
+            "capability:multivariate": True,
         }
 
     def _init_components(self):
         self.classifier = make_pipeline(
             c_StandardScaler(with_mean=True),
             RidgeClassifierCV(
                 alphas=self.alphas_ridge,
-                class_weight=self.class_weight, 
-                fit_intercept=self.fit_intercept
-            )
+                class_weight=self.class_weight,
+                fit_intercept=self.fit_intercept,
+            ),
         )
         self.transformer = R_DST(
             transform_type=self.transform_type,
             phase_invariance=self.phase_invariance,
             alpha=self.alpha,
             prime_dilations=self.prime_dilations,
             shapelet_lengths_bounds=self.shapelet_lengths_bounds,
@@ -172,36 +173,36 @@
             n_samples=self.n_samples,
             n_shapelets=self.n_shapelets,
             n_jobs=False,
             shapelet_lengths=self.shapelet_lengths,
             proba_norm=self.proba_norm,
             percentiles=self.percentiles,
             random_state=self.random_state,
-            min_len=self.min_len 
+            min_len=self.min_len,
         )
-    
+
     def fit(self, X, y):
         """
         Fit method. Random shapelets are generated using the parameters
         supplied during initialisation. Then, input time series are transformed
         using R_DST before classification with a Ridge classifier.
 
         Parameters
         ----------
         X : array, shape=(n_samples, n_features, n_timestamps)
             Input time series.
-            
+
         y : array, shape=(n_samples)
             Class of the input time series.
         """
         self._init_components()
         self.transformer = self.transformer.fit(X, y)
         self.classifier = self.classifier.fit(self.transformer.transform(X), y)
         return self
-        
+
     def predict(self, X):
         """
         Transform the input time series with R_DST and predict their classes
         using the fitted Ridge Classifier.
 
         Parameters
         ----------
@@ -210,27 +211,27 @@
 
         Returns
         -------
         array, shape=(n_samples)
             Predicted class for each input time series
 
         """
-        check_is_fitted(self, ['classifier'])
+        check_is_fitted(self, ["classifier"])
         return self.classifier.predict(self.transformer.transform(X))
-    
+
     def score(self, X, y):
         """
-        Perform the prediction on input time series and return the accuracy 
+        Perform the prediction on input time series and return the accuracy
         score based on the class information.
 
         Parameters
         ----------
         X : array, shape=(n_samples, n_features, n_timestamps)
             Input time series.
-            
+
         y : array, shape=(n_samples)
             Class of the input time series.
 
         Returns
         -------
         float
             Accuracy score on the input time series
```

### Comparing `convst-0.3.0/convst/interpreters/rdst_interpreter.py` & `convst-0.3.1/convst/interpreters/rdst_interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 
 
 import seaborn as sns
 from matplotlib import pyplot as plt
 import numpy as np
 from sklearn.utils.validation import check_is_fitted
 
-from convst.transformers._commons import compute_shapelet_dist_vector, manhattan
+from convst.transformers._commons import compute_shapelet_dist_vector
 from convst.transformers import R_DST
 from convst.classifiers import R_DST_Ridge, R_DST_Ensemble
 
+
 class Shapelet:
     """
-    A Shapelet object to use for ploting operations
+    A Shapelet object to use for ploting operations.
 
     Parameters
     ----------
     values : array, shape=(n_channels * length)
         Values of the shapelet
     length : int
         Length of the shapelet
@@ -40,300 +41,296 @@
         Does the shapelet use phase invariance ?
 
     Returns
     -------
     None.
 
     """
+
     def __init__(self, values, length, dilation, norm, threshold, phase):
         self.values = np.asarray(values)
         self.length = length
         self.dilation = dilation
         self.norm = norm
         self.phase = phase
         self.threshold = threshold
-        
-    def plot(self, figsize=(10,5), seaborn_context='talk', ax=None):
+
+    def plot(self, figsize=(10, 5), seaborn_context='talk', ax=None):
         """
-        Plot the shapelet values
+        Plot the shapelet values.
 
         Parameters
         ----------
         figsize : tuple, optional
             2D size of the figure. The default is (10,5).
         seaborn_context : str, optional
             Seaborn module context. The default is 'talk'.
         ax : matplotlib axe, optional
-            A matplotlib axe on which to plot the figure. The default is None 
+            A matplotlib axe on which to plot the figure. The default is None
             and will create a new figure of size figsize.
 
         Returns
         -------
         fig : matplotlib figure
-            The resulting figure 
+            The resulting figure
         """
         if ax is None:
             sns.set()
             sns.set_context(seaborn_context)
             fig = plt.figure(figsize=(figsize))
             plt.plot(self.values)
             plt.title(
                 'd={},normalize={},threshold={}'.format(
-                    self.dilation, self.norm, np.round(self.threshold,decimals=2)
+                    self.dilation, self.norm, np.round(self.threshold, decimals=2)
                 )
             )
             return fig
         else:
             ax.plot(self.values)
             ax.set_title(
                 'd={},normalize={},threshold={}'.format(
-                    self.dilation, self.norm, np.round(self.threshold,decimals=2)
+                    self.dilation, self.norm, np.round(self.threshold, decimals=2)
                 )
             )
             return ax
-        
+
     def plot_on_X(
-        self, X, d_func=manhattan, figsize=(10,5), seaborn_context='talk', alpha=0.9,
+        self, X, figsize=(10, 5), seaborn_context='talk', alpha=0.9,
         shp_dot_size=40, shp_c='purple', ax=None, label=None, x_linewidth=2
     ):
         """
-        Plot the shapelet on its best match on the time series X
+        Plot the shapelet on its best match on the time series X.
 
         Parameters
         ----------
         X : array, shape=(n_timestamps) or shape=(n_features, n_timestamps)
             Input time series
-        d_func : object, optional
-            A distance function between two arrays. The default is manhattan.
+
         figsize : tuple, optional
             Size of the figure. The default is (10,5).
         seaborn_context : str, optional
             Seaborn context. The default is 'talk'.
         alpha : float, optional
             Alpha parameter for plotting X. The default is 0.9.
         shp_dot_size : float, optional
             Size of the scatter plot to represent the shapelet on X.
             The default is 40.
         shp_c : str, optional
             Color of the shapelet scatter plot. The default is 'purple'.
         ax : matplotlib axe, optional
-            A matplotlib axe on which to plot the figure. The default is None 
+            A matplotlib axe on which to plot the figure. The default is None
             and will create a new figure of size figsize.
         label : str, optional
             Custom label to plot as legend for X. The default is None.
         x_linewidth : float, optional
             The linewidth of X plot. The default is 2.
 
         Returns
         -------
         fig : matplotlib figure
             The resulting figure with S on its best match on X. A normalized
             shapelet will be scalled to macth the scale of X.
 
         """
         c = compute_shapelet_dist_vector(
-            X, self.values, self.length, self.dilation,
-            manhattan, self.norm, self.phase
+            X, self.values, self.length, self.dilation, self.norm, self.phase
         )
         _values = self.values
         idx_match = np.asarray(
-            [(c.argmin() + i*self.dilation)%X.shape[0] for i in range(self.length)]
+            [(c.argmin() + i*self.dilation) % X.shape[0] for i in range(self.length)]
         ).astype(int)
         if self.norm:
             _values = (_values * X[idx_match].std()) + X[idx_match].mean()
-            
+
         if ax is None:
             sns.set()
             sns.set_context(seaborn_context)
             fig = plt.figure(figsize=(figsize))
-            plt.plot(X,label=label, linewidth=x_linewidth, alpha=alpha)
-            plt.scatter(idx_match, _values, s=shp_dot_size, c=shp_c, zorder=3, alpha=alpha)
+            plt.plot(X, label=label, linewidth=x_linewidth, alpha=alpha)
+            plt.scatter(
+                idx_match, _values, s=shp_dot_size, c=shp_c, zorder=3, alpha=alpha
+            )
             return fig
         else:
-            ax.plot(X,label=label, linewidth=x_linewidth, alpha=alpha)
-            ax.scatter(idx_match, _values, s=shp_dot_size, c=shp_c, zorder=3, alpha=alpha)
-    
-    def plot_distance_vector(   
-        self, X, d_func=manhattan, figsize=(10,5), seaborn_context='talk',
+            ax.plot(X, label=label, linewidth=x_linewidth, alpha=alpha)
+            ax.scatter(
+                idx_match, _values, s=shp_dot_size, c=shp_c, zorder=3, alpha=alpha
+            )
+
+    def plot_distance_vector(
+        self, X, figsize=(10, 5), seaborn_context='talk',
         c_threshold='purple', ax=None, label=None
     ):
         """
         Plot the shapelet distance vector computed between itself and X.
 
         Parameters
         ----------
         X : array, shape=(n_timestamps) or shape=(n_features, n_timestamps)
             Input time series
-        d_func : object, optional
-            A distance function between two arrays. The default is manhattan.
         figsize : tuple, optional
             Size of the figure. The default is (10,5).
         seaborn_context : str, optional
             Seaborn context. The default is 'talk'.
         c_threshold : float, optional
             Color used to represent a line on the y-axis to visualize the lambda
             threshold. The default is 'purple'.
         ax : matplotlib axe, optional
-            A matplotlib axe on which to plot the figure. The default is None 
+            A matplotlib axe on which to plot the figure. The default is None
             and will create a new figure of size figsize.
         label : str, optional
             Custom label to plot as legend. The default is None.
-        
+
         Returns
         -------
         fig : matplotlib figure
             The resulting figure with the distance vector obtained by d(S,X)
 
         """
         c = compute_shapelet_dist_vector(
-            X, self.values, self.length, self.dilation,
-            manhattan, self.norm, self.phase
+            X, self.values, self.length, self.dilation, self.norm, self.phase
         )
         if ax is None:
             sns.set()
             sns.set_context(seaborn_context)
             fig = plt.figure(figsize=(figsize))
-            plt.plot(c,label=label)
+            plt.plot(c, label=label)
             plt.hlines(self.threshold, 0, c.shape[0], color=c_threshold)
             return fig
         else:
-            ax.plot(c,label=label)
+            ax.plot(c, label=label)
             ax.hlines(self.threshold, 0, c.shape[0], color=c_threshold)
             return ax
 
-    
+
 class RDST_interpreter():
     """
-    A class to interpret the result from a fitted RDST instance.    
+    A class to interpret the result from a fitted RDST instance.
 
     Parameters
     ----------
     RDST : object
         A fitted RDST transformer.
 
     Returns
     -------
     None.
 
     """
-    
+
     def __init__(self, RDST):
         check_is_fitted(RDST, ['shapelets_'])
         if isinstance(RDST, R_DST):
             self.RDST = RDST
         else:
             raise TypeError(
                 'Object passed to RDST interpreter should be an R_DST instance'
             )
-        
+
     def _get_params(self, id_shapelet):
         values, lengths, dilations, threshold, normalize = self.RDST.shapelets_
         phase = self.RDST.phase_invariance
-        if self.RDST.transform_type in ['multivariate','multivariate_variable']:
-            raise NotImplementedError('Interpreter is not yet implemented for multivariate data')
+        if self.RDST.transform_type in ['multivariate', 'multivariate_variable']:
+            raise NotImplementedError(
+                'Interpreter is not yet implemented for multivariate data'
+            )
         else:
             length_ = lengths[id_shapelet]
             values_ = values[id_shapelet, :length_]
             dilation = dilations[id_shapelet]
             norm = normalize[id_shapelet]
             threshold_ = threshold[id_shapelet]
-        return values_, length_, dilation, norm, threshold_, phase 
-        
-        
+        return values_, length_, dilation, norm, threshold_, phase
+
     def plot_on_X(
-        self, id_shapelet, X, d_func=manhattan, figsize=(10,5),
+        self, id_shapelet, X, figsize=(10, 5),
         seaborn_context='talk', shp_dot_size=40, shp_c='purple', ax=None,
         label=None
     ):
         """
-        Plot the shapelet on its best match on the time series X
+        Plot the shapelet on its best match on the time series X.
 
         Parameters
         ----------
         id_shapelet : int
             ID of the shapelet to plot.
         X : array, shape=(n_timestamps) or shape=(n_features, n_timestamps)
             Input time series
-        d_func : object, optional
-            A distance function between two arrays. The default is manhattan.
         figsize : tuple, optional
             Size of the figure. The default is (10,5).
         seaborn_context : str, optional
             Seaborn context. The default is 'talk'.
         alpha : float, optional
             Alpha parameter for plotting X. The default is 0.9.
         shp_dot_size : float, optional
             Size of the scatter plot to represent the shapelet on X.
             The default is 40.
         shp_c : str, optional
             Color of the shapelet scatter plot. The default is 'purple'.
         ax : matplotlib axe, optional
-            A matplotlib axe on which to plot the figure. The default is None 
+            A matplotlib axe on which to plot the figure. The default is None
             and will create a new figure of size figsize.
         label : str, optional
             Custom label to plot as legend for X. The default is None.
         x_linewidth : float, optional
             The linewidth of X plot. The default is 2.
 
         Returns
         -------
         fig : matplotlib figure
             The resulting figure with S on its best match on X. A normalized
             shapelet will be scalled to macth the scale of X.
 
         """
         return Shapelet(*self._get_params(id_shapelet)).plot_on_X(
-            X, d_func=d_func, figsize=figsize,
+            X, figsize=figsize,
             seaborn_context=seaborn_context, shp_dot_size=shp_dot_size,
             shp_c=shp_c, ax=ax, label=label
         )
 
     def plot_distance_vector(
-        self, id_shapelet, X, d_func=manhattan, figsize=(10,5), 
+        self, id_shapelet, X, figsize=(10, 5),
         seaborn_context='talk', c_threshold='purple', ax=None, label=None
     ):
         """
         Plot the shapelet distance vector computed between itself and X.
 
         Parameters
         ----------
         id_shapelet : int
             ID of the shapelet to plot.
         X : array, shape=(n_timestamps) or shape=(n_features, n_timestamps)
             Input time series
-        d_func : object, optional
-            A distance function between two arrays. The default is manhattan.
         figsize : tuple, optional
             Size of the figure. The default is (10,5).
         seaborn_context : str, optional
             Seaborn context. The default is 'talk'.
         c_threshold : float, optional
             Color used to represent a line on the y-axis to visualize the lambda
             threshold. The default is 'purple'.
         ax : matplotlib axe, optional
-            A matplotlib axe on which to plot the figure. The default is None 
+            A matplotlib axe on which to plot the figure. The default is None
             and will create a new figure of size figsize.
         label : str, optional
             Custom label to plot as legend. The default is None.
-        
+
         Returns
         -------
         fig : matplotlib figure
             The resulting figure with the distance vector obtained by d(S,X)
 
         """
-
         return Shapelet(*self._get_params(id_shapelet)).plot_distance_vector(
-            X, d_func=d_func, figsize=figsize, seaborn_context=seaborn_context,
+            X, figsize=figsize, seaborn_context=seaborn_context,
             c_threshold=c_threshold, ax=ax, label=label
         )
-    
+
     def plot(self, id_shapelet, figsize=(10,5), seaborn_context='talk', ax=None):
         """
-        Plot the shapelet values
+        Plot the shapelet values.
 
         Parameters
         ----------
         id_shapelet : int
             ID of the shapelet to plot.
         figsize : tuple, optional
             2D size of the figure. The default is (10,5).
```

### Comparing `convst-0.3.0/convst/transformers/_commons.py` & `convst-0.3.1/convst/transformers/_commons.py`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/convst/transformers/_input_transformers.py` & `convst-0.3.1/convst/transformers/_input_transformers.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,138 +15,161 @@
 from scipy.signal import periodogram
 from scipy.fft import fht, fhtoffset
 
 from sklearn.preprocessing import StandardScaler, MinMaxScaler
 from sklearn.base import BaseEstimator, TransformerMixin
 
 
-from convst import (
-    __USE_NUMBA_CACHE__, __USE_NUMBA_PARALLEL__
-)
+from convst import __USE_NUMBA_CACHE__, __USE_NUMBA_PARALLEL__
 
 
 class c_StandardScaler(StandardScaler):
     def fit(self, X, y=None):
         self.usefull_atts = np.where(np.std(X, axis=0) != 0)[0]
         return super().fit(X[:, self.usefull_atts], y=y)
-    
+
     def transform(self, X):
         return super().transform(X[:, self.usefull_atts])
-    
+
+
 class c_MinMaxScaler(MinMaxScaler):
     def fit(self, X, y=None):
         self.usefull_atts = np.where(np.std(X, axis=0) != 0)[0]
         return super().fit(X[:, self.usefull_atts], y=y)
-    
+
     def transform(self, X):
         return super().transform(X[:, self.usefull_atts])
 
+
 @njit(cache=__USE_NUMBA_CACHE__)
 def z_norm_one_sample(x):
     n_features, n_timestamps = x.shape
     x_new = np.empty((n_features, n_timestamps))
     for i in prange(n_features):
         x_new[i] = (x[i] - x[i].mean()) / (x[i].std() + 1e-8)
     return x_new
 
+
 @njit(cache=__USE_NUMBA_CACHE__, parallel=__USE_NUMBA_PARALLEL__)
 def z_norm_all_samples(X):
     n_samples, n_features, n_timestamps = X.shape
     X_new = np.empty((n_samples, n_features, n_timestamps))
     for i in prange(n_samples):
         X_new[i] = z_norm_one_sample(X[i])
     return X_new
 
+
 class Z_normalizer(BaseEstimator, TransformerMixin):
     def __init__(self):
-        self.is_univariate=False
-        
+        self.is_univariate = False
+
     def fit(self, X, y=None):
         return self
-    
+
     def transform(self, X):
         X = check_array_3D(X, is_univariate=self.is_univariate)
         return z_norm_all_samples(X)
-    
+
+
 class Raw(BaseEstimator, TransformerMixin):
     def fit(self, X, y=None):
         return self
-    
+
     def transform(self, X):
         return X
 
+
 class Derivate(BaseEstimator, TransformerMixin):
     def __init__(self, order=1, random=False):
         self.order = order
         self.random = random
-        
+
     def fit(self, X, y=None):
         if self.random:
             self._random_init()
         return self
-    
+
     def transform(self, X):
         for i in range(self.order):
             X = np.diff(X)
         return X
 
     def _random_init(self):
-        self.set_params(**{"order":np.random.choice(np.arange(1,5))})
+        self.set_params(**{"order": np.random.choice(np.arange(1, 5))})
+
 
 class Periodigram(BaseEstimator, TransformerMixin):
     def __init__(self, window_type="boxcar", random=False):
         self.window_type = window_type
         self.random = random
-        self.is_univariate=False
-        
+        self.is_univariate = False
+
     def fit(self, X, y=None):
         if self.random:
             self._random_init()
         return self
-    
+
     def transform(self, X):
-        n_ts = periodogram(X[0,0,:], detrend=False, window=self.window_type)[1].shape[0]
+        n_ts = periodogram(X[0, 0, :], detrend=False, window=self.window_type)[1].shape[
+            0
+        ]
         X_new = np.empty((X.shape[0], X.shape[1], n_ts))
         for i in range(X.shape[0]):
             for j in range(X.shape[1]):
-                X_new[i,j] = periodogram(X[i,j], detrend=False, window=self.window_type)[1]
+                X_new[i, j] = periodogram(
+                    X[i, j], detrend=False, window=self.window_type
+                )[1]
         return X_new
-    
+
     def _random_init(self):
-        self.set_params(**{"window_type":np.random.choice(self._get_windows())})
-    
+        self.set_params(**{"window_type": np.random.choice(self._get_windows())})
+
     def _get_windows(self):
         return np.asarray(
-            ["boxcar","triang","blackman","hamming","hann",
-             "bartlett","flattop","parzen","bohman",
-             "blackmanharris","nuttall","barthann",
-             "cosine","exponential","tukey","taylor"]
+            [
+                "boxcar",
+                "triang",
+                "blackman",
+                "hamming",
+                "hann",
+                "bartlett",
+                "flattop",
+                "parzen",
+                "bohman",
+                "blackmanharris",
+                "nuttall",
+                "barthann",
+                "cosine",
+                "exponential",
+                "tukey",
+                "taylor",
+            ]
         )
 
+
 class FastHankelTransform(BaseEstimator, TransformerMixin):
-    def __init__(
-        self, dln=0.01, mu=1, offset=0.0, bias=0.0, use_optimal_offset=True
-    ):
+    def __init__(self, dln=0.01, mu=1, offset=0.0, bias=0.0, use_optimal_offset=True):
         self.dln = dln
         self.mu = mu
         self.offset = offset
         self.bias = bias
         self.use_optimal_offset = use_optimal_offset
-    
+
     def fit(self, X, y=None):
         return self
-    
+
     def transform(self, X):
         X_new = np.zeros(X.shape)
         for i in range(X.shape[0]):
             if self.use_optimal_offset:
                 X_new[i] = fht(
-                    X[i], self.dln, self.mu,
+                    X[i],
+                    self.dln,
+                    self.mu,
                     offset=fhtoffset(self.dln, self.dln, self.bias),
-                    bias=self.bias
+                    bias=self.bias,
                 )
             else:
                 X_new[i] = fht(
-                    X[i], self.dln, self.mu, offset=self.offset,
-                    bias=self.bias
+                    X[i], self.dln, self.mu, offset=self.offset, bias=self.bias
                 )
-        return X_new
+        return X_new
```

### Comparing `convst-0.3.0/convst/transformers/_multivariate_same_length.py` & `convst-0.3.1/convst/transformers/_multivariate_same_length.py`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/convst/transformers/_multivariate_variable_length.py` & `convst-0.3.1/convst/transformers/_multivariate_variable_length.py`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/convst/transformers/_univariate_same_length.py` & `convst-0.3.1/convst/transformers/_univariate_same_length.py`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/convst/transformers/_univariate_variable_length.py` & `convst-0.3.1/convst/transformers/_univariate_variable_length.py`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/convst/transformers/rdst.py` & `convst-0.3.1/convst/transformers/rdst.py`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/convst/utils/checks_utils.py` & `convst-0.3.1/convst/utils/checks_utils.py`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/convst/utils/dataset_utils.py` & `convst-0.3.1/convst/utils/dataset_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 
-from aeon.datasets._data_loaders import _load_dataset
+from aeon.datasets import load_classification
 
 from sklearn.preprocessing import LabelEncoder
 from numba import njit, prange
 
 from convst import __USE_NUMBA_CACHE__
 
+
 @njit(cache=__USE_NUMBA_CACHE__)
 def z_norm_3D(X):
     """
     Z normalise a time series dataset assumed to be of even length. A small value
     is added to the standard deviation for all samples and features to avoid
     0 division.
 
@@ -25,17 +26,20 @@
     -------
     X : array, shape=(n_samples, n_features, n_timestamps)
         Z-normalised array
 
     """
     for i_x in prange(X.shape[0]):
         for i_ft in prange(X.shape[1]):
-            X[i_x, i_ft] = (X[i_x, i_ft] - X[i_x, i_ft].mean())/(X[i_x, i_ft].std() + 1e-8)
+            X[i_x, i_ft] = (X[i_x, i_ft] - X[i_x, i_ft].mean()) / (
+                X[i_x, i_ft].std() + 1e-8
+            )
     return X
-    
+
+
 def z_norm_3D_list(X):
     """
     Z normalise a time series dataset assumed to be of even length. A small value
     is added to the standard deviation for all samples and features to avoid
     0 division.
 
     Parameters
@@ -47,21 +51,23 @@
     -------
     X : array, shape=(n_samples, n_features, n_timestamps)
         Z-normalised array
 
     """
     for i_x in range(len(X)):
         for i_ft in range(len(X[i_x])):
-            X[i_x][i_ft] = (X[i_x][i_ft] - X[i_x][i_ft].mean())/(X[i_x][i_ft].std() + 1e-8)
+            X[i_x][i_ft] = (X[i_x][i_ft] - X[i_x][i_ft].mean()) / (
+                X[i_x][i_ft].std() + 1e-8
+            )
     return X
-    
+
 
 def load_UCR_UEA_dataset_split(name, normalize=False):
     """
-    Load the original train and test splits of a dataset 
+    Load the original train and test splits of a dataset
     from the UCR/UEA archive by name using aeon API.
 
     Parameters
     ----------
     name : string
         Name of the dataset to download.
     normalize : boolean, optional
@@ -79,27 +85,27 @@
     y_test : array, shape=(n_samples_test)
         Class of the testing data.
     le : LabelEncoder
         LabelEncoder object used to uniformize the class labels
 
 
     """
-    #Load datasets
-    X_train, y_train = _load_dataset(name, return_X_y=True, split='train')
-    X_test, y_test = _load_dataset(name, return_X_y=True, split='test')
+    # Load datasets
+    X_train, y_train = load_classification(name, return_metadata=False, split="train")
+    X_test, y_test = load_classification(name, return_metadata=False, split="test")
 
-    #Convert class labels to make sure they are between 0,n_classes
+    # Convert class labels to make sure they are between 0,n_classes
     le = LabelEncoder().fit(y_train)
     y_train = le.transform(y_train)
     y_test = le.transform(y_test)
     min_len = min(
-        min([len(X_train[i][0])for i in range(len(X_train))]),
-        min([len(X_test[i][0])for i in range(len(X_test))]),
+        min([len(X_train[i][0]) for i in range(len(X_train))]),
+        min([len(X_test[i][0]) for i in range(len(X_test))]),
     )
-    #Z-Normalize the data
+    # Z-Normalize the data
     if normalize and not isinstance(X_train, list):
         X_train = z_norm_3D(X_train)
         X_test = z_norm_3D(X_test)
     if normalize and isinstance(X_train, list):
         X_train = z_norm_3D_list(X_train)
         X_test = z_norm_3D_list(X_test)
     return X_train, X_test, y_train, y_test, min_len
@@ -119,98 +125,111 @@
     Returns
     -------
     X : array, shape=(n_samples, n_features, n_timestamps)
         Time series data from the dataset specified by name.
     y : array, shape=(n_samples)
         Class of the time series
     """
-    #Load datasets
+    # Load datasets
     X_train, X_test, y_train, y_test, _ = load_UCR_UEA_dataset_split(
         name, normalize=normalize
     )
-    return np.concatenate((X_train, X_test),axis=0), np.concatenate((y_train, y_test),axis=0)
+    return np.concatenate((X_train, X_test), axis=0), np.concatenate(
+        (y_train, y_test), axis=0
+    )
+
 
 def return_all_dataset_names():
-    return np.concatenate((
-        return_all_univariate_dataset_names(),
-        return_all_multivariate_dataset_names(),
-        return_all_variable_univariate_dataset_names(),
-        return_all_variable_multivariate_dataset_names()
-    ))
+    return np.concatenate(
+        (
+            return_all_univariate_dataset_names(),
+            return_all_multivariate_dataset_names(),
+            return_all_variable_univariate_dataset_names(),
+            return_all_variable_multivariate_dataset_names(),
+        )
+    )
+
 
 def return_all_multivariate_dataset_names():
-    
-    return np.asarray([
-        "ArticularyWordRecognition",
-        "AtrialFibrillation",
-        "BasicMotions",
-        "Cricket",
-        "DuckDuckGeese",
-        "EigenWorms",
-        "Epilepsy",
-        "EthanolConcentration",
-        "ERing",
-        "FaceDetection",
-        "FingerMovements",
-        "HandMovementDirection",
-        "Handwriting",
-        "Heartbeat",
-        "Libras",
-        "LSST",
-        "MotorImagery",
-        "NATOPS",
-        "PenDigits",
-        "PEMS-SF",
-        "PhonemeSpectra",
-        "RacketSports",
-        "SelfRegulationSCP1",
-        "SelfRegulationSCP2",
-        "StandWalkJump",
-        "UWaveGestureLibrary"
-    ])
+    return np.asarray(
+        [
+            "ArticularyWordRecognition",
+            "AtrialFibrillation",
+            "BasicMotions",
+            "Cricket",
+            "DuckDuckGeese",
+            "EigenWorms",
+            "Epilepsy",
+            "EthanolConcentration",
+            "ERing",
+            "FaceDetection",
+            "FingerMovements",
+            "HandMovementDirection",
+            "Handwriting",
+            "Heartbeat",
+            "Libras",
+            "LSST",
+            "MotorImagery",
+            "NATOPS",
+            "PenDigits",
+            "PEMS-SF",
+            "PhonemeSpectra",
+            "RacketSports",
+            "SelfRegulationSCP1",
+            "SelfRegulationSCP2",
+            "StandWalkJump",
+            "UWaveGestureLibrary",
+        ]
+    )
+
 
 def return_all_variable_multivariate_dataset_names():
-    return np.asarray([
-        "AsphaltObstaclesCoordinates",
-        "AsphaltPavementTypeCoordinates",
-        "AsphaltRegularityCoordinates",
-        "CharacterTrajectories",
-        "InsectWingbeat",
-        "JapaneseVowels",
-        "SpokenArabicDigits"
-    ])
+    return np.asarray(
+        [
+            "AsphaltObstaclesCoordinates",
+            "AsphaltPavementTypeCoordinates",
+            "AsphaltRegularityCoordinates",
+            "CharacterTrajectories",
+            "InsectWingbeat",
+            "JapaneseVowels",
+            "SpokenArabicDigits",
+        ]
+    )
 
 
 def return_all_variable_univariate_dataset_names():
-    return np.asarray([
-        "AllGestureWiimoteX",
-        "AllGestureWiimoteY",
-        "AllGestureWiimoteZ",
-        "GestureMidAirD1",
-        "GestureMidAirD2",
-        "GestureMidAirD3",
-        "GesturePebbleZ1",
-        "GesturePebbleZ2",
-        "PickupGestureWiimoteZ",
-        "PLAID",
-        "ShakeGestureWiimoteZ"
-    ])
+    return np.asarray(
+        [
+            "AllGestureWiimoteX",
+            "AllGestureWiimoteY",
+            "AllGestureWiimoteZ",
+            "GestureMidAirD1",
+            "GestureMidAirD2",
+            "GestureMidAirD3",
+            "GesturePebbleZ1",
+            "GesturePebbleZ2",
+            "PickupGestureWiimoteZ",
+            "PLAID",
+            "ShakeGestureWiimoteZ",
+        ]
+    )
 
 
 def return_all_univariate_dataset_names():
     """
     Return the names of the 112 univariate datasets of the UCR archive.
 
     Returns
     -------
     array, shape=(112)
         Names of the univariate UCR datasets.
 
     """
-    return np.asarray([
+    return np.asarray(
+        [
             "ACSF1",
             "Adiac",
             "ArrowHead",
             "Beef",
             "BeetleFly",
             "BirdChicken",
             "BME",
@@ -314,9 +333,10 @@
             "PigArtPressure",
             "PigCVP",
             "Crop",
             "StarLightCurves",
             "Rock",
             "HandOutlines",
             "CinCECGTorso",
-            "EthanolLevel"
-            ])
+            "EthanolLevel",
+        ]
+    )
```

### Comparing `convst-0.3.0/convst/utils/experiments_utils.py` & `convst-0.3.1/convst/utils/experiments_utils.py`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/convst/utils/numba_utils.py` & `convst-0.3.1/convst/utils/numba_utils.py`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/convst/utils/plot_utils.py` & `convst-0.3.1/convst/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/convst.egg-info/PKG-INFO` & `convst-0.3.1/convst.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convst
-Version: 0.3.0
+Version: 0.3.1
 Summary: The Random Dilation Shapelet Transform algorithm and associated works
 Home-page: https://github.com/baraline/convst
 Download-URL: https://pypi.org/project/convst/#files
 Author: Antoine Guillaume
 Author-email: Antoine Guillaume <antoine.guillaume45@gmail.com>
 License: BSD 2-Clause License
         
@@ -45,21 +45,22 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # This package is moving to the aeon-toolkit.
 Starting from v0.3.0, this package will not be updated, bugfixes will still be included if issues are raised.
-You can already find an updated version of RDST in the Aeon package at https://github.com/aeon-toolkit/ . Further improvements are planned for further speeding up RDST, these improvement will only be implemented in aeon.
+You can already find RDST in the Aeon package at https://github.com/aeon-toolkit/ . Further improvements are planned for further speeding up RDST, these improvement will only be implemented in aeon.
 All the functionnalities of this package will be ported into Aeon when I got some time, for now, only the transformer for univariate and multivariate series of even length have been implemented.
 
 # Readme
 Welcome to the convst repository. It contains the implementation of the `Random Dilated Shapelet Transform (RDST)` along with other works in the same area.
 This work was supported by the following organisations:
 
 <p float="center">
@@ -87,17 +88,14 @@
 
 The recommended way to install the latest stable version is to use pip with `pip install convst`. To install the package from sources, you can download the latest version on GitHub and run `python setup.py install`. This should install the package and automatically look for the dependencies using `pip`. 
 
 We recommend doing this in a new virtual environment using anaconda to avoid any conflict with an existing installation. If you wish to install dependencies individually, you can see dependencies in the `setup.py` file.
 
 An optional dependency that can help speed up numba, which is used in our implementation, is the Intel vector math library (SVML). When using conda it can be installed by running `conda install -c numba icc_rt`. I didn't test the behavior with AMD processors, but I suspect it won't work.
 
-If you are using RDST in some specific settings such as an HPC cluster and are getting errors, take a loot at [issue #24](https://github.com/baraline/convst/issues/24), you may need to change the numba compilation settings to not using function caching (see [this example](https://github.com/baraline/convst/blob/main/examples/Changing_numba_options.py)). THIS SHOULD BE FIXED WITH v0.3.0
-
-
 ## Tutorial
 We give here a minimal example to run the `RDST` algorithm on any dataset of the UCR archive using the aeon API to get datasets:
 
 ```python
 
 from convst.classifiers import R_DST_Ridge
 from convst.utils.dataset_utils import load_UCR_UEA_dataset_split
```

### Comparing `convst-0.3.0/convst.egg-info/SOURCES.txt` & `convst-0.3.1/convst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/pyproject.toml` & `convst-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "convst"
 
-version = "0.3.0"
+version = "0.3.1"
 
 description = "The Random Dilation Shapelet Transform algorithm and associated works"
 readme = "README.md"
 authors = [
     {name = "Antoine Guillaume", email = "antoine.guillaume45@gmail.com"}
 ]
 keywords = [
@@ -26,35 +26,34 @@
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
-requires-python = ">=3.8,<3.11"
+requires-python = ">=3.8,<3.12"
 dependencies = [
-    "aeon>=0.3",
+    "aeon>=0.4",
     "numba>=0.55",
     "numpy>=1.21.0,<1.25",
     "scikit-learn>=1.0.0,<1.3.0",
-    "scipy<2.0.0,>=1.2.0",
+    "scipy>=1.2.0,<2.0.0",
     "pandas>=1.1.0,<1.6.0",
     "joblib>=1.1.1",
-    "statsmodels>=0.12.1",
     "scipy<2.0.0,>=1.2.0",
-    "matplotlib>=3.1",
-    "seaborn>=0.10.0",
+    "matplotlib>=3.3.2",
+    "seaborn>=0.11.0",
     "pytest>=7.0",
     "sphinx >= 4.2.0",
     "sphinx_gallery >= 0.10.1",
     "numpydoc >= 1.1.0",
     "alabaster >= 0.7.12"
 ]
-
 [project.urls]
 repository = "https://github.com/baraline/convst"
 documentation = "https://convst.readthedocs.io/"
 download = "https://pypi.org/project/convst/#files"
 
 [project.license]
 file = "LICENSE"
```

### Comparing `convst-0.3.0/setup.py` & `convst-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/tests/test_checks_utils.py` & `convst-0.3.1/tests/test_checks_utils.py`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/tests/test_commons_transform.py` & `convst-0.3.1/tests/test_commons_transform.py`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/tests/test_dataset_utils.py` & `convst-0.3.1/tests/test_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `convst-0.3.0/tests/test_rdst.py` & `convst-0.3.1/tests/test_rdst.py`

 * *Files identical despite different names*

