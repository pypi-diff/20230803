# Comparing `tmp/nmecpy-1.4.0.tar.gz` & `tmp/nmecpy-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmecpy-1.4.0.tar", last modified: Tue Aug  1 19:11:36 2023, max compression
+gzip compressed data, was "nmecpy-1.4.1.tar", last modified: Wed Aug  2 19:18:53 2023, max compression
```

## Comparing `nmecpy-1.4.0.tar` & `nmecpy-1.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 19:11:36.071037 nmecpy-1.4.0/
--rw-rw-rw-   0        0        0      313 2023-08-01 19:11:36.063036 nmecpy-1.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 19:11:36.011037 nmecpy-1.4.0/nmecpy/
--rw-rw-rw-   0        0        0    11476 2023-06-29 01:10:56.000000 nmecpy-1.4.0/nmecpy/ChangePointModel.py
--rw-rw-rw-   0        0        0    19996 2023-06-28 20:22:20.000000 nmecpy-1.4.0/nmecpy/Model.py
--rw-rw-rw-   0        0        0    15573 2023-06-29 01:52:24.000000 nmecpy-1.4.0/nmecpy/StowtModel.py
--rw-rw-rw-   0        0        0       54 2023-06-28 20:22:20.000000 nmecpy-1.4.0/nmecpy/example.py
--rw-rw-rw-   0        0        0     6322 2023-08-01 19:08:55.000000 nmecpy-1.4.0/nmecpy/hddCddModel.py
--rw-rw-rw-   0        0        0     4257 2023-06-29 02:18:41.000000 nmecpy-1.4.0/nmecpy/nmec.py
--rw-rw-rw-   0        0        0    19014 2023-07-07 22:37:43.000000 nmecpy-1.4.0/nmecpy/towtModel.py
-drwxrwxrwx   0        0        0        0 2023-08-01 19:11:36.057040 nmecpy-1.4.0/nmecpy.egg-info/
--rw-rw-rw-   0        0        0      313 2023-08-01 19:11:35.000000 nmecpy-1.4.0/nmecpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-08-01 19:11:35.000000 nmecpy-1.4.0/nmecpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 19:11:35.000000 nmecpy-1.4.0/nmecpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-08-01 19:11:35.000000 nmecpy-1.4.0/nmecpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-01 19:11:35.000000 nmecpy-1.4.0/nmecpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 19:11:36.071037 nmecpy-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      593 2023-08-01 19:11:29.000000 nmecpy-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:18:52.987712 nmecpy-1.4.1/
+-rw-rw-rw-   0        0        0      313 2023-08-02 19:18:52.983713 nmecpy-1.4.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 19:18:52.939713 nmecpy-1.4.1/nmecpy/
+-rw-rw-rw-   0        0        0    11476 2023-06-29 01:10:56.000000 nmecpy-1.4.1/nmecpy/ChangePointModel.py
+-rw-rw-rw-   0        0        0    19996 2023-06-28 20:22:20.000000 nmecpy-1.4.1/nmecpy/Model.py
+-rw-rw-rw-   0        0        0    15573 2023-06-29 01:52:24.000000 nmecpy-1.4.1/nmecpy/StowtModel.py
+-rw-rw-rw-   0        0        0       54 2023-06-28 20:22:20.000000 nmecpy-1.4.1/nmecpy/example.py
+-rw-rw-rw-   0        0        0     6457 2023-08-02 19:17:05.000000 nmecpy-1.4.1/nmecpy/hddCddModel.py
+-rw-rw-rw-   0        0        0     4257 2023-06-29 02:18:41.000000 nmecpy-1.4.1/nmecpy/nmec.py
+-rw-rw-rw-   0        0        0    19014 2023-07-07 22:37:43.000000 nmecpy-1.4.1/nmecpy/towtModel.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:18:52.977711 nmecpy-1.4.1/nmecpy.egg-info/
+-rw-rw-rw-   0        0        0      313 2023-08-02 19:18:52.000000 nmecpy-1.4.1/nmecpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-08-02 19:18:52.000000 nmecpy-1.4.1/nmecpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 19:18:52.000000 nmecpy-1.4.1/nmecpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-08-02 19:18:52.000000 nmecpy-1.4.1/nmecpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 19:18:52.000000 nmecpy-1.4.1/nmecpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 19:18:52.988711 nmecpy-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      593 2023-08-02 19:18:47.000000 nmecpy-1.4.1/setup.py
```

### Comparing `nmecpy-1.4.0/nmecpy/ChangePointModel.py` & `nmecpy-1.4.1/nmecpy/ChangePointModel.py`

 * *Files identical despite different names*

### Comparing `nmecpy-1.4.0/nmecpy/Model.py` & `nmecpy-1.4.1/nmecpy/Model.py`

 * *Files identical despite different names*

### Comparing `nmecpy-1.4.0/nmecpy/StowtModel.py` & `nmecpy-1.4.1/nmecpy/StowtModel.py`

 * *Files identical despite different names*

### Comparing `nmecpy-1.4.0/nmecpy/hddCddModel.py` & `nmecpy-1.4.1/nmecpy/hddCddModel.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         out = train[[self.timestamp_col, 'yhat']].merge(
             main, on=self.timestamp_col, how='outer')
 
         print("Model completed running. Check model attribute.")
 
         return(out)
 
-    def predict(self, df, timestamp_col='time'):
+    def predict(self, df, timestamp_col='time', allow_neg_values=False):
         """
         Predict method for heating degree and cooling degree methods.
 
         Parameters
         ----------
         df : Pandas DataFrame
             Dataframe with heating and/or cooling degree variables.
@@ -157,8 +157,12 @@
         pred = main[[timestamp_col] +
                     self.x_train_cols].dropna().copy()
 
         x_pred = pred[self.x_train_cols]
         pred['predict'] = self.model.predict(x_pred)
         out = pred[[temp_time_col, 'predict']].merge(
             main, on=temp_time_col, how='outer')
-        return(out)
+        
+        if allow_neg_values==False:
+            out.loc[out['predict'] < 0, 'predict'] = 0
+        
+        return(out)
```

### Comparing `nmecpy-1.4.0/nmecpy/nmec.py` & `nmecpy-1.4.1/nmecpy/nmec.py`

 * *Files identical despite different names*

### Comparing `nmecpy-1.4.0/nmecpy/towtModel.py` & `nmecpy-1.4.1/nmecpy/towtModel.py`

 * *Files identical despite different names*

### Comparing `nmecpy-1.4.0/setup.py` & `nmecpy-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='nmecpy',
-    version='1.4.0',    
+    version='1.4.1',    
     description='An implementation of peer-reviewed energy data analysis algorithms in Python for site-specific M&V',
     url='https://github.com/kW-Labs/nmecpy',
     author='Maggie Jacoby, Deter Luu, Devan Johnson',
     author_email='dbardin@kw-engineering.com',
     license='MIT',
     packages=['nmecpy'],
     install_requires=['scikit-learn',
```

