# Comparing `tmp/MOBPY-1.1.0.tar.gz` & `tmp/MOBPY-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MOBPY-1.1.0.tar", last modified: Tue Aug  1 12:55:00 2023, max compression
+gzip compressed data, was "MOBPY-1.1.1.tar", last modified: Thu Aug  3 08:54:02 2023, max compression
```

## Comparing `MOBPY-1.1.0.tar` & `MOBPY-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.704392 MOBPY-1.1.0/
--rw-r--r--   0 chentahung   (501) staff       (20)     1073 2023-07-04 10:05:44.000000 MOBPY-1.1.0/LICENSE
--rw-r--r--   0 chentahung   (501) staff       (20)    12304 2023-08-01 12:55:00.704179 MOBPY-1.1.0/PKG-INFO
--rw-r--r--   0 chentahung   (501) staff       (20)    11672 2023-07-30 14:03:25.000000 MOBPY-1.1.0/README.md
--rw-r--r--   0 chentahung   (501) staff       (20)      702 2023-08-01 12:53:56.000000 MOBPY-1.1.0/pyproject.toml
--rw-r--r--   0 chentahung   (501) staff       (20)       38 2023-08-01 12:55:00.704441 MOBPY-1.1.0/setup.cfg
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.700839 MOBPY-1.1.0/src/
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.702030 MOBPY-1.1.0/src/MOBPY/
--rw-r--r--   0 chentahung   (501) staff       (20)    13237 2023-07-27 09:47:44.000000 MOBPY-1.1.0/src/MOBPY/MOB.py
--rw-r--r--   0 chentahung   (501) staff       (20)    13410 2023-07-30 13:45:11.000000 MOBPY-1.1.0/src/MOBPY/PAVA.py
--rw-------   0 chentahung   (501) staff       (20)        0 2022-10-18 10:30:40.000000 MOBPY-1.1.0/src/MOBPY/__ init __.py
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.702720 MOBPY-1.1.0/src/MOBPY/categorical/
--rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:26.000000 MOBPY-1.1.0/src/MOBPY/categorical/__init__.py
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.703299 MOBPY-1.1.0/src/MOBPY/numeric/
--rw-r--r--   0 chentahung   (501) staff       (20)     5028 2023-07-22 19:06:58.000000 MOBPY-1.1.0/src/MOBPY/numeric/Monotone.py
--rw-r--r--   0 chentahung   (501) staff       (20)     3185 2023-06-11 15:50:05.000000 MOBPY-1.1.0/src/MOBPY/numeric/MonotoneNode.py
--rw-r--r--   0 chentahung   (501) staff       (20)    15005 2023-07-22 19:08:22.000000 MOBPY-1.1.0/src/MOBPY/numeric/OptimalBinning.py
--rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:33.000000 MOBPY-1.1.0/src/MOBPY/numeric/__init__.py
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.703719 MOBPY-1.1.0/src/MOBPY/pav/
--rw-r--r--   0 chentahung   (501) staff       (20)     7837 2023-07-27 09:47:36.000000 MOBPY-1.1.0/src/MOBPY/pav/PAV.py
--rw-r--r--   0 chentahung   (501) staff       (20)     3248 2023-07-24 15:46:45.000000 MOBPY-1.1.0/src/MOBPY/pav/PavMonoNode.py
--rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-16 12:44:20.000000 MOBPY-1.1.0/src/MOBPY/pav/__init__.py
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.703994 MOBPY-1.1.0/src/MOBPY/plot/
--rw-r--r--   0 chentahung   (501) staff       (20)     6524 2023-07-27 09:48:36.000000 MOBPY-1.1.0/src/MOBPY/plot/MOB_PLOT.py
--rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:39.000000 MOBPY-1.1.0/src/MOBPY/plot/__init__.py
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-01 12:55:00.702579 MOBPY-1.1.0/src/MOBPY.egg-info/
--rw-r--r--   0 chentahung   (501) staff       (20)    12304 2023-08-01 12:55:00.000000 MOBPY-1.1.0/src/MOBPY.egg-info/PKG-INFO
--rw-r--r--   0 chentahung   (501) staff       (20)      517 2023-08-01 12:55:00.000000 MOBPY-1.1.0/src/MOBPY.egg-info/SOURCES.txt
--rw-r--r--   0 chentahung   (501) staff       (20)        1 2023-08-01 12:55:00.000000 MOBPY-1.1.0/src/MOBPY.egg-info/dependency_links.txt
--rw-r--r--   0 chentahung   (501) staff       (20)        6 2023-08-01 12:55:00.000000 MOBPY-1.1.0/src/MOBPY.egg-info/top_level.txt
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-03 08:54:02.738160 MOBPY-1.1.1/
+-rw-r--r--   0 chentahung   (501) staff       (20)     1073 2023-07-04 10:05:44.000000 MOBPY-1.1.1/LICENSE
+-rw-r--r--   0 chentahung   (501) staff       (20)    12304 2023-08-03 08:54:02.737942 MOBPY-1.1.1/PKG-INFO
+-rw-r--r--   0 chentahung   (501) staff       (20)    11672 2023-07-30 14:03:25.000000 MOBPY-1.1.1/README.md
+-rw-r--r--   0 chentahung   (501) staff       (20)      702 2023-08-03 08:40:53.000000 MOBPY-1.1.1/pyproject.toml
+-rw-r--r--   0 chentahung   (501) staff       (20)       38 2023-08-03 08:54:02.738208 MOBPY-1.1.1/setup.cfg
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-03 08:54:02.731718 MOBPY-1.1.1/src/
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-03 08:54:02.734137 MOBPY-1.1.1/src/MOBPY/
+-rw-r--r--   0 chentahung   (501) staff       (20)    13237 2023-07-27 09:47:44.000000 MOBPY-1.1.1/src/MOBPY/MOB.py
+-rw-r--r--   0 chentahung   (501) staff       (20)    13456 2023-08-03 08:35:39.000000 MOBPY-1.1.1/src/MOBPY/PAVA.py
+-rw-------   0 chentahung   (501) staff       (20)        0 2022-10-18 10:30:40.000000 MOBPY-1.1.1/src/MOBPY/__ init __.py
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-03 08:54:02.735122 MOBPY-1.1.1/src/MOBPY/categorical/
+-rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:26.000000 MOBPY-1.1.1/src/MOBPY/categorical/__init__.py
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-03 08:54:02.736353 MOBPY-1.1.1/src/MOBPY/numeric/
+-rw-r--r--   0 chentahung   (501) staff       (20)     5028 2023-07-22 19:06:58.000000 MOBPY-1.1.1/src/MOBPY/numeric/Monotone.py
+-rw-r--r--   0 chentahung   (501) staff       (20)     3185 2023-06-11 15:50:05.000000 MOBPY-1.1.1/src/MOBPY/numeric/MonotoneNode.py
+-rw-r--r--   0 chentahung   (501) staff       (20)    15005 2023-07-22 19:08:22.000000 MOBPY-1.1.1/src/MOBPY/numeric/OptimalBinning.py
+-rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:33.000000 MOBPY-1.1.1/src/MOBPY/numeric/__init__.py
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-03 08:54:02.737262 MOBPY-1.1.1/src/MOBPY/pav/
+-rw-r--r--   0 chentahung   (501) staff       (20)     7837 2023-07-27 09:47:36.000000 MOBPY-1.1.1/src/MOBPY/pav/PAV.py
+-rw-r--r--   0 chentahung   (501) staff       (20)     3248 2023-07-24 15:46:45.000000 MOBPY-1.1.1/src/MOBPY/pav/PavMonoNode.py
+-rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-16 12:44:20.000000 MOBPY-1.1.1/src/MOBPY/pav/__init__.py
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-03 08:54:02.737709 MOBPY-1.1.1/src/MOBPY/plot/
+-rw-r--r--   0 chentahung   (501) staff       (20)     6689 2023-08-03 08:44:36.000000 MOBPY-1.1.1/src/MOBPY/plot/MOB_PLOT.py
+-rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:39.000000 MOBPY-1.1.1/src/MOBPY/plot/__init__.py
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-08-03 08:54:02.734916 MOBPY-1.1.1/src/MOBPY.egg-info/
+-rw-r--r--   0 chentahung   (501) staff       (20)    12304 2023-08-03 08:54:02.000000 MOBPY-1.1.1/src/MOBPY.egg-info/PKG-INFO
+-rw-r--r--   0 chentahung   (501) staff       (20)      517 2023-08-03 08:54:02.000000 MOBPY-1.1.1/src/MOBPY.egg-info/SOURCES.txt
+-rw-r--r--   0 chentahung   (501) staff       (20)        1 2023-08-03 08:54:02.000000 MOBPY-1.1.1/src/MOBPY.egg-info/dependency_links.txt
+-rw-r--r--   0 chentahung   (501) staff       (20)        6 2023-08-03 08:54:02.000000 MOBPY-1.1.1/src/MOBPY.egg-info/top_level.txt
```

### Comparing `MOBPY-1.1.0/LICENSE` & `MOBPY-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MOBPY-1.1.0/PKG-INFO` & `MOBPY-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MOBPY
-Version: 1.1.0
+Version: 1.1.1
 Summary: MOB is a statistical approach to transform continuous variables into optimal and monotonic categorical variables.
 Author-email: "Ta-Hung (Denny) Chen" <denny20700@gmail.com>
 Project-URL: Homepage, https://github.com/ChenTaHung/Monotonic-Optimal-Binning
 Project-URL: Bug Tracker, https://github.com/ChenTaHung/Monotonic-Optimal-Binning/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `MOBPY-1.1.0/README.md` & `MOBPY-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `MOBPY-1.1.0/pyproject.toml` & `MOBPY-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "MOBPY"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Ta-Hung (Denny) Chen", email="denny20700@gmail.com" }
 ]
 description = "MOB is a statistical approach to transform continuous variables into optimal and monotonic categorical variables."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `MOBPY-1.1.0/src/MOBPY/MOB.py` & `MOBPY-1.1.1/src/MOBPY/MOB.py`

 * *Files identical despite different names*

### Comparing `MOBPY-1.1.0/src/MOBPY/PAVA.py` & `MOBPY-1.1.1/src/MOBPY/PAVA.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,16 +221,16 @@
 
             PAVA_Final_Df = GCM.sort_values(by = 'intervalStart').rename(columns = {'intervalStart':self.var, self.metric : f'{self.response}_{self.metric}'})
             PAVA_Result = PAVA_Final_Df
         #Generate final PAVA result (include additional var aggregation functions)
         # create interval 
         PAVA_Result.insert(1, column='intervalEnd)', value=PAVA_Result[self.var].shift(-1))
         PAVA_Result.rename(columns = {self.var:'[intervalStart'}, inplace=True)
-        PAVA_Result.iloc[0, 0] = -np.inf
-        PAVA_Result.iloc[-1, 1] = np.inf
+        PAVA_Result.iloc[0, 0] = -np.inf #minimum interval start
+        PAVA_Result.iloc[-1, 1] = np.inf #maximum interval end
         PAVA_Result = PAVA_Result.drop('intervalEnd', axis = 1)
         '''
         OrgDataAssignment : original dataset but only select columns below 
         self.var | self.response | assignValue | assignMetric
         -----------------------------------------------------
         '''
         self._OrgDataAssignment = OrgDataAssignment
```

### Comparing `MOBPY-1.1.0/src/MOBPY/numeric/Monotone.py` & `MOBPY-1.1.1/src/MOBPY/numeric/Monotone.py`

 * *Files identical despite different names*

### Comparing `MOBPY-1.1.0/src/MOBPY/numeric/MonotoneNode.py` & `MOBPY-1.1.1/src/MOBPY/numeric/MonotoneNode.py`

 * *Files identical despite different names*

### Comparing `MOBPY-1.1.0/src/MOBPY/numeric/OptimalBinning.py` & `MOBPY-1.1.1/src/MOBPY/numeric/OptimalBinning.py`

 * *Files identical despite different names*

### Comparing `MOBPY-1.1.0/src/MOBPY/pav/PAV.py` & `MOBPY-1.1.1/src/MOBPY/pav/PAV.py`

 * *Files identical despite different names*

### Comparing `MOBPY-1.1.0/src/MOBPY/pav/PavMonoNode.py` & `MOBPY-1.1.1/src/MOBPY/pav/PavMonoNode.py`

 * *Files identical despite different names*

### Comparing `MOBPY-1.1.0/src/MOBPY/plot/MOB_PLOT.py` & `MOBPY-1.1.1/src/MOBPY/plot/MOB_PLOT.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                         line_color = 'orange', line_width = 3, dot_color = 'red', dot_size = 80, annotation_font_weight = 'bold', 
                         figsavePath: str = None , dpi:int = 300):
         
         fig, ax1 = plt.subplots(1,1,figsize = (12,8))
         binSummaryTable = monoOptBinTable.copy()
         var_name = binSummaryTable.index.name        
         binSummaryTable['interval'] = '[' + binSummaryTable['[intervalStart'].astype(str) + ' , ' + binSummaryTable['intervalEnd)'].astype(str) + ')'
-        
+        binSummaryTable.loc[0, 'interval'] = binSummaryTable.loc[0, 'interval'].replace('[', '(')
         # Plot bar chart for 'dist_obs'
         bars = ax1.bar(np.arange(len(binSummaryTable['interval'])), binSummaryTable['woe'], color = bar_fill, alpha = bar_alpha, width = bar_width)
         ax1.set_xticks(ticks = np.arange(len(binSummaryTable['interval'])), labels = binSummaryTable['interval'])
         ax1.axhline(0)
         ax1.set_xlabel('Interval End Value')
         ax1.set_ylabel('WoE', color = bar_text_color)
 
@@ -71,17 +71,18 @@
         var = CSD_Summary.columns[0]
         response = CSD_Summary.iloc[:,1].name.split('_')[0]
         metric = CSD_Summary.iloc[:,1].name.split('_')[1]
         
         _GCM = CSD_Summary[['intervalStart', 'intervalEnd', 'assignMetric']].drop_duplicates(['intervalStart', 'intervalEnd', 'assignMetric'])
         _GCM['[intervalStart'] = _GCM['intervalStart'].astype(str)
         _GCM['intervalEnd)'] = _GCM['intervalStart'].shift(-1).astype(str)
-        _GCM.iloc[0,3] = str(np.inf)
-        _GCM.iloc[-1,4] = str(-np.inf)
+        _GCM.iloc[0,3] = str(-np.inf)
+        _GCM.iloc[-1,4] = str(np.inf)
         _GCM['interval'] = '[' + _GCM['[intervalStart'] + ',' + _GCM['intervalEnd)'] + ')'
+        _GCM.loc[0, 'interval'] = _GCM.loc[0, 'interval'].replace('[', '(')
         '''
         GCM
         intervalStart | intervalEnd | assignMetric | [intervalStart | intervalEnd) | interval
         -------------------------------------------------------------------------------------
         '''
         
         _CSD = CSD_Summary.drop_duplicates(var, keep = 'last')
```

### Comparing `MOBPY-1.1.0/src/MOBPY.egg-info/PKG-INFO` & `MOBPY-1.1.1/src/MOBPY.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MOBPY
-Version: 1.1.0
+Version: 1.1.1
 Summary: MOB is a statistical approach to transform continuous variables into optimal and monotonic categorical variables.
 Author-email: "Ta-Hung (Denny) Chen" <denny20700@gmail.com>
 Project-URL: Homepage, https://github.com/ChenTaHung/Monotonic-Optimal-Binning
 Project-URL: Bug Tracker, https://github.com/ChenTaHung/Monotonic-Optimal-Binning/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `MOBPY-1.1.0/src/MOBPY.egg-info/SOURCES.txt` & `MOBPY-1.1.1/src/MOBPY.egg-info/SOURCES.txt`

 * *Files identical despite different names*

