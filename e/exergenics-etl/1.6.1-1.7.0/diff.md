# Comparing `tmp/exergenics-etl-1.6.1.tar.gz` & `tmp/exergenics-etl-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-1.6.1.tar", last modified: Fri Jul 28 03:37:34 2023, max compression
+gzip compressed data, was "exergenics-etl-1.7.0.tar", last modified: Thu Aug  3 03:12:36 2023, max compression
```

## Comparing `exergenics-etl-1.6.1.tar` & `exergenics-etl-1.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:34.265580 exergenics-etl-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-28 03:37:34.261580 exergenics-etl-1.6.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:34.261580 exergenics-etl-1.6.1/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:34.261580 exergenics-etl-1.6.1/app/exergenics_etl/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:34.261580 exergenics-etl-1.6.1/app/exergenics_etl/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58210 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/src/exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/src/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:34.261580 exergenics-etl-1.6.1/app/exergenics_etl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    43240 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/test/test_exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-28 03:37:27.000000 exergenics-etl-1.6.1/app/exergenics_etl/test/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:34.261580 exergenics-etl-1.6.1/app/exergenics_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-28 03:37:34.000000 exergenics-etl-1.6.1/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-28 03:37:34.000000 exergenics-etl-1.6.1/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 03:37:34.000000 exergenics-etl-1.6.1/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-28 03:37:34.000000 exergenics-etl-1.6.1/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 03:37:34.000000 exergenics-etl-1.6.1/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 03:37:34.265580 exergenics-etl-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-28 03:37:32.000000 exergenics-etl-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:12:36.977429 exergenics-etl-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 03:12:32.000000 exergenics-etl-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-03 03:12:36.977429 exergenics-etl-1.7.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:12:36.973429 exergenics-etl-1.7.0/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:12:36.973429 exergenics-etl-1.7.0/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-03 03:12:32.000000 exergenics-etl-1.7.0/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:12:36.973429 exergenics-etl-1.7.0/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 03:12:32.000000 exergenics-etl-1.7.0/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58727 2023-08-03 03:12:32.000000 exergenics-etl-1.7.0/app/exergenics_etl/src/exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-08-03 03:12:32.000000 exergenics-etl-1.7.0/app/exergenics_etl/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:12:36.973429 exergenics-etl-1.7.0/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 03:12:32.000000 exergenics-etl-1.7.0/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-03 03:12:32.000000 exergenics-etl-1.7.0/app/exergenics_etl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43253 2023-08-03 03:12:32.000000 exergenics-etl-1.7.0/app/exergenics_etl/test/test_exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-03 03:12:32.000000 exergenics-etl-1.7.0/app/exergenics_etl/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:12:36.973429 exergenics-etl-1.7.0/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-03 03:12:36.000000 exergenics-etl-1.7.0/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-03 03:12:36.000000 exergenics-etl-1.7.0/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 03:12:36.000000 exergenics-etl-1.7.0/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-03 03:12:36.000000 exergenics-etl-1.7.0/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 03:12:36.000000 exergenics-etl-1.7.0/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 03:12:36.977429 exergenics-etl-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-03 03:12:34.000000 exergenics-etl-1.7.0/setup.py
```

### Comparing `exergenics-etl-1.6.1/LICENSE` & `exergenics-etl-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.6.1/app/exergenics_etl/__init__.py` & `exergenics-etl-1.7.0/app/exergenics_etl/__init__.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.6.1/app/exergenics_etl/src/exergenics_etl.py` & `exergenics-etl-1.7.0/app/exergenics_etl/src/exergenics_etl.py`

 * *Files 1% similar despite different names*

```diff
@@ -753,14 +753,16 @@
 
     isUnixTimestamp = False
 
     firstRowInStrings = df.iloc[0].astype(str)
     timestampColumnNames = []
     for index, possibleTimestamp in firstRowInStrings.items():
         try:
+            # FIXME: AEST and AEDT tz names raise error in pandas 2.0, fix them after error removed in pandas
+            possibleTimestamp = possibleTimestamp.replace("AEST", "AET").replace("AEDT", "AET")
             # Raise exception if possibleTimestamp is not in any timestamp format
             # or is a string of numbers (unix timestamps)
             pd.to_datetime(possibleTimestamp)
 
             # Store the column name if to_datetime passes
             timestampColumnNames.append(index)
             logger.info(f'This is a timestamp column. Column name = "{index}". Tested value = {possibleTimestamp}')
@@ -1217,20 +1219,24 @@
 
         self.logger.info(
             f'Showing the first and the last 2 of the timestamps BEFORE parsing: \n{pd.concat([dtSeries.head(2), dtSeries.tail(2)])}')
 
         # PARSE unix timestamps automatically without finding timestamp format
         if isUnixTimestamp:
             try:
+                # Convert unix timestamps need numeric type
+                if dtSeries.dtype == "O":
+                    dtSeries = dtSeries.astype(int)
                 dtObjects = pd.to_datetime(dtSeries, unit='s')
             except Exception as e:
                 errorMessage = f'Parsing unix timestamps failed: {e}'
                 self.logger.error(errorMessage)
                 raise EtlError(f'Parsing timestamps failed.')
             else:
+                self.logger.info(f'Showing the first and the last 2 of the timestamps AFTER parsing: \n{pd.concat([dtObjects.head(2), dtObjects.tail(2)])}')
                 return dtObjects
             
         # FIND the timestamp format
         if self.dtFinalFormat is None:
             self._find_final_format(dtSeries)
         else:
             self.logger.info(
```

### Comparing `exergenics-etl-1.6.1/app/exergenics_etl/src/logger.py` & `exergenics-etl-1.7.0/app/exergenics_etl/src/logger.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.6.1/app/exergenics_etl/test/conftest.py` & `exergenics-etl-1.7.0/app/exergenics_etl/test/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 @pytest.fixture(scope='session')
 def my_summary_statistics_table_test_case2():
     myTestPoint2 = 'Test data point2'
     myTestDf = pd.DataFrame({'timepretty': [Timestamp('2023-05-19 15:08:00'), Timestamp('2023-05-19 15:09:00'), Timestamp('2023-05-19 15:10:00')],
                              'observation': [myTestPoint2, myTestPoint2, myTestPoint2],
                              'datapoint': [True, True, False]})
-    expectedPointSummary = pd.DataFrame({'count': {myTestPoint2: 3}})
+    expectedPointSummary = pd.DataFrame({'count': {myTestPoint2: 3}}, dtype="object")
     return myTestPoint2, myTestDf, expectedPointSummary
 
 
 @pytest.fixture(scope='session')
 def my_summary_statistics_table_test_case3():
     myTestPoint3 = 'Test data point3'
     myTestDf = pd.DataFrame({'timepretty': [Timestamp('2023-05-19 15:08:00'), Timestamp('2023-05-19 15:09:00'), Timestamp('2023-05-19 15:10:00')],
```

### Comparing `exergenics-etl-1.6.1/app/exergenics_etl/test/test_exergenics_etl.py` & `exergenics-etl-1.7.0/app/exergenics_etl/test/test_exergenics_etl.py`

 * *Files 1% similar despite different names*

```diff
@@ -779,22 +779,21 @@
     @pytest.mark.parametrize("my_get_point_summary_test_case", ['my_summary_statistics_table_test_case1', 'my_summary_statistics_table_test_case2', 'my_summary_statistics_table_test_case3'])
     def test_get_point_summary(self, my_get_point_summary_test_case, request):
         myTestPoint, myTestDf, expectedPointSummary = request.getfixturevalue(
             my_get_point_summary_test_case)
         assert get_point_summary(
             myTestPoint, myTestDf).equals(expectedPointSummary)
 
-
 class TestGetStatisticalSummary:
     def test_get_statistical_summary(self, my_summary_statistics_table_test_case1, my_summary_statistics_table_test_case2, my_summary_statistics_table_test_case3):
         myTestPoint1, myTestDf1, expectedPointSummary = my_summary_statistics_table_test_case1
         myTestPoint2, myTestDf2, expectedPointSummary = my_summary_statistics_table_test_case2
         myTestPoint3, myTestDf3, expectedPointSummary = my_summary_statistics_table_test_case3
         expectedStatisticalSummaryTable = pd.DataFrame({'count': {'Test data point1': 2.0,
-                                                                  'Test data point2': 3.0,
+                                                                  'Test data point2': 3,
                                                                   'Test data point3': 0.0},
                                                         'mean': {'Test data point1': 1.0,
                                                                  'Test data point2': '',
                                                                  'Test data point3': ''},
                                                         'std': {'Test data point1': 1.414,
                                                                 'Test data point2': '',
                                                                 'Test data point3': ''},
@@ -808,15 +807,15 @@
                                                                 'Test data point2': '',
                                                                 'Test data point3': ''},
                                                         '75%': {'Test data point1': 1.5,
                                                                 'Test data point2': '',
                                                                 'Test data point3': ''},
                                                         'max': {'Test data point1': 2.0,
                                                                 'Test data point2': '',
-                                                                'Test data point3': ''}})
+                                                                'Test data point3': ''}}, dtype="object")
 
         assert get_statistical_summary(
             {myTestPoint1: myTestDf1, myTestPoint2: myTestDf2, myTestPoint3: myTestDf3}).equals(expectedStatisticalSummaryTable)
 
 
 class TestMergeLongDataframesClass:
```

### Comparing `exergenics-etl-1.6.1/app/exergenics_etl.egg-info/SOURCES.txt` & `exergenics-etl-1.7.0/app/exergenics_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.6.1/setup.py` & `exergenics-etl-1.7.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 # with open("app/Readme.md", "r") as f:
 #     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="v1.6.1",
+    version="v1.7.0",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
@@ -18,15 +18,15 @@
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent"
     ],
     install_requires=["exergenics >= 2.0.0",
                       "DateTime == 5.1",
-                      "pandas == 1.4.0",
+                      "pandas >= 1.4.0",
                       "PyMySQL == 1.0.2",
                       "pytz == 2022.7.1",
                       "SQLAlchemy == 1.4.46",
                       "python-dotenv == 1.0.0",
                       "openpyxl == 3.0.10",
                       "Levenshtein == 0.21.0",
                       "regex == 2022.10.31",
```

