# Comparing `tmp/CurvPy-1.0.7.tar.gz` & `tmp/CurvPy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CurvPy-1.0.7.tar", last modified: Fri Jul 14 14:20:37 2023, max compression
+gzip compressed data, was "CurvPy-1.0.8.tar", last modified: Thu Aug  3 17:07:25 2023, max compression
```

## Comparing `CurvPy-1.0.7.tar` & `CurvPy-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:20:37.907738 CurvPy-1.0.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:20:37.897738 CurvPy-1.0.7/CurvPy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5464 2023-07-14 14:20:37.000000 CurvPy-1.0.7/CurvPy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-14 14:20:37.000000 CurvPy-1.0.7/CurvPy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 14:20:37.000000 CurvPy-1.0.7/CurvPy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-14 14:20:37.000000 CurvPy-1.0.7/CurvPy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-14 14:20:37.000000 CurvPy-1.0.7/CurvPy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5464 2023-07-14 14:20:37.907738 CurvPy-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5346 2023-07-14 14:19:02.000000 CurvPy-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:20:37.907738 CurvPy-1.0.7/curvpy/
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-05 19:13:20.000000 CurvPy-1.0.7/curvpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8078 2023-07-05 19:20:26.000000 CurvPy-1.0.7/curvpy/curvpy.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 14:20:37.907738 CurvPy-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      549 2023-07-14 14:20:04.000000 CurvPy-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 17:07:25.790628 CurvPy-1.0.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 17:07:25.790628 CurvPy-1.0.8/CurvPy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5464 2023-08-03 17:07:25.000000 CurvPy-1.0.8/CurvPy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2023-08-03 17:07:25.000000 CurvPy-1.0.8/CurvPy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 17:07:25.000000 CurvPy-1.0.8/CurvPy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-08-03 17:07:25.000000 CurvPy-1.0.8/CurvPy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-03 17:07:25.000000 CurvPy-1.0.8/CurvPy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5464 2023-08-03 17:07:25.790628 CurvPy-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5346 2023-07-14 14:19:02.000000 CurvPy-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 17:07:25.790628 CurvPy-1.0.8/curvpy/
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-05 19:13:20.000000 CurvPy-1.0.8/curvpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10052 2023-08-03 17:05:39.000000 CurvPy-1.0.8/curvpy/curvpy.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 17:07:25.790628 CurvPy-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      573 2023-08-03 17:05:37.000000 CurvPy-1.0.8/setup.py
```

### Comparing `CurvPy-1.0.7/CurvPy.egg-info/PKG-INFO` & `CurvPy-1.0.8/CurvPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CurvPy
-Version: 1.0.7
+Version: 1.0.8
 Summary: A regression analysis library
 Home-page: UNKNOWN
 Author: sidharth
 Author-email: sidharthss2690@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `CurvPy-1.0.7/PKG-INFO` & `CurvPy-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CurvPy
-Version: 1.0.7
+Version: 1.0.8
 Summary: A regression analysis library
 Home-page: UNKNOWN
 Author: sidharth
 Author-email: sidharthss2690@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `CurvPy-1.0.7/README.md` & `CurvPy-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `CurvPy-1.0.7/curvpy/curvpy.py` & `CurvPy-1.0.8/curvpy/curvpy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import numpy as np
 from scipy.optimize import curve_fit
 from sklearn.linear_model import LinearRegression
 from sklearn.preprocessing import PolynomialFeatures
 import scipy.optimize as optimize
 import matplotlib.pyplot as plt
 from scipy import stats
+from sklearn.model_selection import train_test_split, GridSearchCV
+from sklearn.linear_model import LinearRegression
+from sklearn.preprocessing import PolynomialFeatures
+from sklearn.pipeline import Pipeline
+from sklearn.metrics import mean_squared_error, r2_score
 
 
 # Function to calculate R-squared value
 def r_squared(y_true, y_pred):
     residuals = y_true - y_pred
     ss_residuals = np.sum(residuals ** 2)
     ss_total = np.sum((y_true - np.mean(y_true)) ** 2)
@@ -88,23 +93,56 @@
         equation += f' {coef:.2f}x{i+1} +'
     equation += f' {model.intercept_:.2f}'
     r2 = r_squared(y, y_pred)
     return equation, r2
 
 # Data sleuth function
 def datasleuth(x, y):
+    # Split data into training and testing sets
+    x_train, x_test, y_train, y_test = train_test_split(x, y, train_size=0.7)
+
+    # Reshape the data for PolynomialFeatures
+    x_train_reshaped = x_train.reshape(-1, 1)
+    x_test_reshaped = x_test.reshape(-1, 1)
+
+    # Set the range of degrees to search
+    param_grid = {'poly__degree': np.arange(1, 11)}
+
+    # Create a pipeline with PolynomialFeatures and LinearRegression
+    pipeline = Pipeline([
+        ('poly', PolynomialFeatures()),
+        ('model', LinearRegression())
+    ])
+
+    # Perform a grid search to find the best degree
+    grid_search = GridSearchCV(pipeline, param_grid, cv=5)
+    grid_search.fit(x_train_reshaped, y_train)
+
+    # Get the best degree and best model
+    best_degree = grid_search.best_params_['poly__degree']
+    best_model = grid_search.best_estimator_
+
+    # Predict using the best model
+    y_pred = best_model.predict(x_test_reshaped)
+
+    # Calculate and print the best polynomial regression equation
+    coefficients = best_model.named_steps['model'].coef_
+    equation = f"y = {coefficients[0]:.4f}"
+    for i in range(1, best_degree + 1):
+        equation += f" + {coefficients[i]:.4f}x^{i}"
+
     # Linear regression
     linear_equation, linear_r2 = linear_regression(x.reshape(-1, 1), y)
     print("Linear Regression")
     print("Equation:", linear_equation)
     print("R-squared value:", linear_r2)
     print()
 
     # Polynomial regression
-    poly_degree = 2
+    poly_degree = best_degree
     poly_equation, poly_r2 = polynomial_regression(x.reshape(-1, 1), y, poly_degree)
     print("Polynomial Regression (Degree", poly_degree, ")")
     print("Equation:", poly_equation)
     print("R-squared value:", poly_r2)
     print()
 
     # Logarithmic regression
@@ -130,14 +168,28 @@
 
     # Sinusoidal regression
     sinusoidal_equation, sinusoidal_r2 = sinusoidal_regression(x, y)
     print("Sinusoidal Regression")
     print("Equation:", sinusoidal_equation)
     print("R-squared value:", sinusoidal_r2)
     print()
+    print("Best Polynomial Regression Equation:", equation)
+
+    # Calculate and print the mean squared error
+    mse = mean_squared_error(y_test, y_pred)
+    print("Mean Squared Error:", mse)
+
+    # Calculate and print the R-squared score
+    r2 = r2_score(y_test, y_pred)
+    print("R2 Score:", r2)
+    plt.scatter(y_pred,y_test,c='g')
+    plt.xlabel("Predicted y")
+    plt.ylabel("Actual y")
+    plt.title("Predicted v/s Actual value of Y")
+    plt.show()
 
 def optifit(func, x_data, y_data, guess_params):
     # Perform curve fitting
     fitted_params, _ = optimize.curve_fit(func, x_data, y_data, guess_params)
     y_pred = func(x_data, *fitted_params)
 
     # Calculate metrics
@@ -222,8 +274,8 @@
     upper_bounds = upper_bounds_input if upper_bounds_input is not None else np.inf
     
     if maxfev is None:
         maxfev = 10000
     
     popt, pcov = curve_fit(func, x, y, p0=initial_parameters, bounds=(lower_bounds, upper_bounds), maxfev=maxfev)
     
-    return popt
+    return popt
```

### Comparing `CurvPy-1.0.7/setup.py` & `CurvPy-1.0.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='CurvPy',
-    version='1.0.7',
+    version='1.0.8',
     author='sidharth',
     author_email='sidharthss2690@gmail.com',
     description='A regression analysis library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
         'scikit-learn',
         'matplotlib',
+        'scikit-learn'
     ],
 )
```

