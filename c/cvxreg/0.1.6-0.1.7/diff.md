# Comparing `tmp/cvxreg-0.1.6.tar.gz` & `tmp/cvxreg-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxreg-0.1.6.tar", last modified: Wed Jun 14 12:45:31 2023, max compression
+gzip compressed data, was "cvxreg-0.1.7.tar", last modified: Thu Aug  3 08:17:33 2023, max compression
```

## Comparing `cvxreg-0.1.6.tar` & `cvxreg-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:45:31.446835 cvxreg-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-14 12:45:21.000000 cvxreg-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-14 12:45:31.446835 cvxreg-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-14 12:45:21.000000 cvxreg-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:45:31.442835 cvxreg-0.1.6/cvxreg/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-14 12:45:21.000000 cvxreg-0.1.6/cvxreg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-14 12:45:21.000000 cvxreg-0.1.6/cvxreg/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-14 12:45:21.000000 cvxreg-0.1.6/cvxreg/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:45:31.446835 cvxreg-0.1.6/cvxreg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-14 12:45:21.000000 cvxreg-0.1.6/cvxreg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-14 12:45:21.000000 cvxreg-0.1.6/cvxreg/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 12:45:21.000000 cvxreg-0.1.6/cvxreg/models/_cvxpy_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-14 12:45:21.000000 cvxreg-0.1.6/cvxreg/models/_penalized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:45:31.446835 cvxreg-0.1.6/cvxreg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-14 12:45:21.000000 cvxreg-0.1.6/cvxreg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-06-14 12:45:21.000000 cvxreg-0.1.6/cvxreg/utils/_param_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-14 12:45:21.000000 cvxreg-0.1.6/cvxreg/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-14 12:45:21.000000 cvxreg-0.1.6/cvxreg/utils/extmath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:45:31.446835 cvxreg-0.1.6/cvxreg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-14 12:45:31.000000 cvxreg-0.1.6/cvxreg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-14 12:45:31.000000 cvxreg-0.1.6/cvxreg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:45:31.000000 cvxreg-0.1.6/cvxreg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:45:31.000000 cvxreg-0.1.6/cvxreg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-14 12:45:31.000000 cvxreg-0.1.6/cvxreg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 12:45:31.000000 cvxreg-0.1.6/cvxreg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:45:31.446835 cvxreg-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-14 12:45:21.000000 cvxreg-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:17:33.980303 cvxreg-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 08:17:20.000000 cvxreg-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-03 08:17:33.980303 cvxreg-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-03 08:17:20.000000 cvxreg-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:17:33.976303 cvxreg-0.1.7/cvxreg/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:17:33.976303 cvxreg-0.1.7/cvxreg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/models/_cvxpy_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/models/_penalized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:17:33.980303 cvxreg-0.1.7/cvxreg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/utils/_param_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-03 08:17:20.000000 cvxreg-0.1.7/cvxreg/utils/extmath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:17:33.976303 cvxreg-0.1.7/cvxreg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-03 08:17:33.000000 cvxreg-0.1.7/cvxreg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-03 08:17:33.000000 cvxreg-0.1.7/cvxreg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:17:33.000000 cvxreg-0.1.7/cvxreg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:17:33.000000 cvxreg-0.1.7/cvxreg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-03 08:17:33.000000 cvxreg-0.1.7/cvxreg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 08:17:33.000000 cvxreg-0.1.7/cvxreg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:17:33.980303 cvxreg-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-03 08:17:20.000000 cvxreg-0.1.7/setup.py
```

### Comparing `cvxreg-0.1.6/LICENSE` & `cvxreg-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.6/PKG-INFO` & `cvxreg-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python Package for Convex Regression
 Home-page: https://github.com/ConvexRegression/cvxreg
 Download-URL: https://pypi.org/project/cvxreg/
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
 Keywords: ML,Prediction,Regression
```

### Comparing `cvxreg-0.1.6/README.md` & `cvxreg-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.6/cvxreg/base.py` & `cvxreg-0.1.7/cvxreg/base.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.6/cvxreg/models/_base.py` & `cvxreg-0.1.7/cvxreg/models/_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,59 +3,68 @@
 """
 
 # Author: Zhiqiang Liao @ Aalto University <zhiqiang.liao@aalto.fi>
 # License: MIT
 
 from abc import ABCMeta, abstractmethod
 import numpy as np
+from scipy import sparse
 from cvxpy import Variable, sum_squares
 
 from ._cvxpy_opt import solve_model
 from ..base import BaseEstimator
 from ..constant import convex, concave
 from ..utils.extmath import yhat
 from ..utils._param_check import StrOptions
-from ..utils.check import check_ndarray
+
 
 def _calculate_matrix_A(n):
     res = np.zeros((n*(n-1), n))
     k = 0
     for i in range(n):
         for j in range(n):
             if i != j:
                 res[k, i] = -1
                 res[k, j] = 1
                 k += 1
     return res
 
 def _calculate_matrix_B(x, n, d):
-    res = np.zeros((n*(n-1), n*d))
+    num_rows = n * (n - 1)
+    num_cols = n * d
+
+    row_indices = []
+    col_indices = []
+    data = []
+
     k = 0
     for i in range(n):
         for j in range(n):
             if i != j:
-                res[k, i*d:(i+1)*d] = x[j,:] - x[i,:]
+                row_indices.extend([k] * d)
+                col_indices.extend(range(i * d, (i + 1) * d))
+                data.extend(x[j, :] - x[i, :])
                 k += 1
-    return -res
 
-def _shape_constraint(A, B, Xi, theta, n, d, shape=convex, positive=False):
-    check_ndarray(A, n*(n-1), n)
-    check_ndarray(B, n*(n-1), n*d)
+    sparse_matrix = sparse.coo_matrix((data, (row_indices, col_indices)), shape=(num_rows, num_cols))
+    return -sparse_matrix
+
+def _shape_constraint(A, B, Xi, theta, shape=convex, positive=False):
 
     if shape == convex:
         cons_shape = A @ theta + B @ Xi >= 0
     elif shape == concave:
         cons_shape = A @ theta + B @ Xi <= 0
 
     if positive:
         cons_positive = Xi >= 0.0
     else:
-        return cons_shape
+        return [cons_shape]
 
-    return cons_shape, cons_positive
+    return [cons_shape, cons_positive]
 
 class CRModel(BaseEstimator, metaclass=ABCMeta):
     """
     Base class for CR models
     """
     @abstractmethod
     def fit(self):
@@ -141,15 +150,15 @@
 
         # interface with cvxpy
         Xi = Variable(n*d)
         theta = Variable(n)
         objective = 0.5*sum_squares(y - theta)
 
         # add shape constraint
-        constraint = [_shape_constraint(A, B, Xi, theta, n, d, shape=self.shape, positive=self.positive)]
+        constraint = _shape_constraint(A, B, Xi, theta, shape=self.shape, positive=self.positive)
 
         # optimize the model with solver
         self.solution = solve_model(objective, constraint, self.solver)
         
         Xi_val = Xi.value.reshape(n,d)
         theta_val = theta.value
```

### Comparing `cvxreg-0.1.6/cvxreg/models/_penalized.py` & `cvxreg-0.1.7/cvxreg/models/_penalized.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
         # interface with cvxpy
         Xi = Variable(n*d)
         theta = Variable(n)
         objective = 0.5*sum_squares(y - theta) + self.c*sum_squares(Xi)
 
         # add shape constraint
-        constraint = [_shape_constraint(A, B, Xi, theta, n, d, shape=self.shape, positive=self.positive)]
+        constraint = _shape_constraint(A, B, Xi, theta, shape=self.shape, positive=self.positive)
 
         # optimize the model with solver
         self.solution = solve_model(objective, constraint, self.solver)
         
         Xi_val = Xi.value.reshape(n,d)
         theta_val = theta.value
```

### Comparing `cvxreg-0.1.6/cvxreg/utils/_param_check.py` & `cvxreg-0.1.7/cvxreg/utils/_param_check.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.6/cvxreg/utils/check.py` & `cvxreg-0.1.7/cvxreg/utils/check.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.6/cvxreg/utils/extmath.py` & `cvxreg-0.1.7/cvxreg/utils/extmath.py`

 * *Files identical despite different names*

### Comparing `cvxreg-0.1.6/cvxreg.egg-info/PKG-INFO` & `cvxreg-0.1.7/cvxreg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python Package for Convex Regression
 Home-page: https://github.com/ConvexRegression/cvxreg
 Download-URL: https://pypi.org/project/cvxreg/
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
 Keywords: ML,Prediction,Regression
```

### Comparing `cvxreg-0.1.6/setup.py` & `cvxreg-0.1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='cvxreg',
-    version='0.1.6',
+    version='0.1.7',
     description='A Python Package for Convex Regression',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Zhiqiang Liao',
     author_email='zhiqiang.liao@aalto.fi',
@@ -24,14 +24,15 @@
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
 
 install_requires = [
+    'python>=3.7',
     'numpy>=1.19.2',
     'pandas>=1.1.3',
     'scipy>=1.5.2',
     'cvxpy>=1.1.7'
 ]
 
 if __name__ == '__main__':
```

