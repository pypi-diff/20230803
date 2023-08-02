# Comparing `tmp/nmecpy-1.4.3.tar.gz` & `tmp/nmecpy-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmecpy-1.4.3.tar", last modified: Wed Aug  2 22:29:31 2023, max compression
+gzip compressed data, was "nmecpy-1.4.4.tar", last modified: Wed Aug  2 23:31:34 2023, max compression
```

## Comparing `nmecpy-1.4.3.tar` & `nmecpy-1.4.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 22:29:31.503447 nmecpy-1.4.3/
--rw-rw-rw-   0        0        0      313 2023-08-02 22:29:31.499443 nmecpy-1.4.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 22:29:31.462442 nmecpy-1.4.3/nmecpy/
--rw-rw-rw-   0        0        0    11476 2023-06-29 01:10:56.000000 nmecpy-1.4.3/nmecpy/ChangePointModel.py
--rw-rw-rw-   0        0        0    19996 2023-06-28 20:22:20.000000 nmecpy-1.4.3/nmecpy/Model.py
--rw-rw-rw-   0        0        0    15573 2023-06-29 01:52:24.000000 nmecpy-1.4.3/nmecpy/StowtModel.py
--rw-rw-rw-   0        0        0       54 2023-06-28 20:22:20.000000 nmecpy-1.4.3/nmecpy/example.py
--rw-rw-rw-   0        0        0     6525 2023-08-02 22:29:06.000000 nmecpy-1.4.3/nmecpy/hddCddModel.py
--rw-rw-rw-   0        0        0     4257 2023-06-29 02:18:41.000000 nmecpy-1.4.3/nmecpy/nmec.py
--rw-rw-rw-   0        0        0    19014 2023-07-07 22:37:43.000000 nmecpy-1.4.3/nmecpy/towtModel.py
-drwxrwxrwx   0        0        0        0 2023-08-02 22:29:31.495443 nmecpy-1.4.3/nmecpy.egg-info/
--rw-rw-rw-   0        0        0      313 2023-08-02 22:29:30.000000 nmecpy-1.4.3/nmecpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-08-02 22:29:31.000000 nmecpy-1.4.3/nmecpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 22:29:30.000000 nmecpy-1.4.3/nmecpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-08-02 22:29:30.000000 nmecpy-1.4.3/nmecpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-02 22:29:30.000000 nmecpy-1.4.3/nmecpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 22:29:31.504443 nmecpy-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      593 2023-08-02 22:29:24.000000 nmecpy-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:31:34.737964 nmecpy-1.4.4/
+-rw-rw-rw-   0        0        0      313 2023-08-02 23:31:34.733961 nmecpy-1.4.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 23:31:34.686961 nmecpy-1.4.4/nmecpy/
+-rw-rw-rw-   0        0        0    11476 2023-06-29 01:10:56.000000 nmecpy-1.4.4/nmecpy/ChangePointModel.py
+-rw-rw-rw-   0        0        0    19996 2023-06-28 20:22:20.000000 nmecpy-1.4.4/nmecpy/Model.py
+-rw-rw-rw-   0        0        0    15573 2023-06-29 01:52:24.000000 nmecpy-1.4.4/nmecpy/StowtModel.py
+-rw-rw-rw-   0        0        0       54 2023-06-28 20:22:20.000000 nmecpy-1.4.4/nmecpy/example.py
+-rw-rw-rw-   0        0        0     6697 2023-08-02 23:31:04.000000 nmecpy-1.4.4/nmecpy/hddCddModel.py
+-rw-rw-rw-   0        0        0     4257 2023-06-29 02:18:41.000000 nmecpy-1.4.4/nmecpy/nmec.py
+-rw-rw-rw-   0        0        0    19014 2023-07-07 22:37:43.000000 nmecpy-1.4.4/nmecpy/towtModel.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:31:34.728961 nmecpy-1.4.4/nmecpy.egg-info/
+-rw-rw-rw-   0        0        0      313 2023-08-02 23:31:34.000000 nmecpy-1.4.4/nmecpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-08-02 23:31:34.000000 nmecpy-1.4.4/nmecpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 23:31:34.000000 nmecpy-1.4.4/nmecpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-08-02 23:31:34.000000 nmecpy-1.4.4/nmecpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 23:31:34.000000 nmecpy-1.4.4/nmecpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 23:31:34.738960 nmecpy-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      593 2023-08-02 23:31:29.000000 nmecpy-1.4.4/setup.py
```

### Comparing `nmecpy-1.4.3/nmecpy/ChangePointModel.py` & `nmecpy-1.4.4/nmecpy/ChangePointModel.py`

 * *Files identical despite different names*

### Comparing `nmecpy-1.4.3/nmecpy/Model.py` & `nmecpy-1.4.4/nmecpy/Model.py`

 * *Files identical despite different names*

### Comparing `nmecpy-1.4.3/nmecpy/StowtModel.py` & `nmecpy-1.4.4/nmecpy/StowtModel.py`

 * *Files identical despite different names*

### Comparing `nmecpy-1.4.3/nmecpy/hddCddModel.py` & `nmecpy-1.4.4/nmecpy/hddCddModel.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,32 +135,32 @@
             on.
 
         Returns
         -------
         Predictions attached to main dataframe.
 
         """
-
         # Checks
         if self.model is None:
             raise ValueError("Create a model using train method.")
-
-        check_cols = all(item in df.columns for item in
+        main = df.copy()
+        main['CD'] = main[self.temperature_col] - self.CD_balancepoint
+        main.loc[main['CD'] < 0, 'CD'] = 0
+        main['HD'] = self.HD_balancepoint - main[self.temperature_col]
+        main.loc[main['HD'] < 0, 'HD'] = 0
+        
+        check_cols = all(item in main.columns for item in
                          [timestamp_col]+self.x_train_cols)
-
-        return [df.columns, [timestamp_col]+self.x_train_cols]
-
         if not check_cols:
             raise ValueError("Missing either the timestamp col"
                              " or one of the explanatory variables.")
 
         temp_time_col = timestamp_col
 
         # Predict
-        main = df.copy()
         pred = main[[timestamp_col] +
                     self.x_train_cols].dropna().copy()
 
         x_pred = pred[self.x_train_cols]
         pred['predict'] = self.model.predict(x_pred)
         out = pred[[temp_time_col, 'predict']].merge(
             main, on=temp_time_col, how='outer')
```

### Comparing `nmecpy-1.4.3/nmecpy/nmec.py` & `nmecpy-1.4.4/nmecpy/nmec.py`

 * *Files identical despite different names*

### Comparing `nmecpy-1.4.3/nmecpy/towtModel.py` & `nmecpy-1.4.4/nmecpy/towtModel.py`

 * *Files identical despite different names*

### Comparing `nmecpy-1.4.3/setup.py` & `nmecpy-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='nmecpy',
-    version='1.4.3',    
+    version='1.4.4',    
     description='An implementation of peer-reviewed energy data analysis algorithms in Python for site-specific M&V',
     url='https://github.com/kW-Labs/nmecpy',
     author='Maggie Jacoby, Deter Luu, Devan Johnson',
     author_email='dbardin@kw-engineering.com',
     license='MIT',
     packages=['nmecpy'],
     install_requires=['scikit-learn',
```

