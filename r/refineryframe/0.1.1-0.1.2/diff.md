# Comparing `tmp/refineryframe-0.1.1.tar.gz` & `tmp/refineryframe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineryframe-0.1.1.tar", last modified: Tue Aug  1 02:17:43 2023, max compression
+gzip compressed data, was "refineryframe-0.1.2.tar", last modified: Wed Aug  2 22:22:24 2023, max compression
```

## Comparing `refineryframe-0.1.1.tar` & `refineryframe-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:17:43.741247 refineryframe-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-01 02:17:28.000000 refineryframe-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30409 2023-08-01 02:17:43.741247 refineryframe-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    29623 2023-08-01 02:17:42.000000 refineryframe-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:17:43.737247 refineryframe-0.1.1/refineryframe/
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-08-01 02:17:28.000000 refineryframe-0.1.1/refineryframe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34997 2023-08-01 02:17:28.000000 refineryframe-0.1.1/refineryframe/detect_unexpected.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-01 02:17:28.000000 refineryframe-0.1.1/refineryframe/other.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17760 2023-08-01 02:17:28.000000 refineryframe-0.1.1/refineryframe/refiner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-01 02:17:28.000000 refineryframe-0.1.1/refineryframe/replace_unexpected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:17:43.741247 refineryframe-0.1.1/refineryframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30409 2023-08-01 02:17:43.000000 refineryframe-0.1.1/refineryframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 02:17:43.000000 refineryframe-0.1.1/refineryframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:17:43.000000 refineryframe-0.1.1/refineryframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 02:17:43.000000 refineryframe-0.1.1/refineryframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 02:17:43.000000 refineryframe-0.1.1/refineryframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 02:17:43.741247 refineryframe-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-01 02:17:42.000000 refineryframe-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:17:43.741247 refineryframe-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:17:28.000000 refineryframe-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-08-01 02:17:28.000000 refineryframe-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-08-01 02:17:28.000000 refineryframe-0.1.1/tests/test_refiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:22:24.111378 refineryframe-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-02 22:22:10.000000 refineryframe-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    31929 2023-08-02 22:22:24.111378 refineryframe-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31144 2023-08-02 22:22:23.000000 refineryframe-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:22:24.107378 refineryframe-0.1.2/refineryframe/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-08-02 22:22:10.000000 refineryframe-0.1.2/refineryframe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36408 2023-08-02 22:22:10.000000 refineryframe-0.1.2/refineryframe/detect_unexpected.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-02 22:22:10.000000 refineryframe-0.1.2/refineryframe/other.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19516 2023-08-02 22:22:10.000000 refineryframe-0.1.2/refineryframe/refiner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-02 22:22:10.000000 refineryframe-0.1.2/refineryframe/replace_unexpected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:22:24.107378 refineryframe-0.1.2/refineryframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31929 2023-08-02 22:22:24.000000 refineryframe-0.1.2/refineryframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-02 22:22:24.000000 refineryframe-0.1.2/refineryframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:22:24.000000 refineryframe-0.1.2/refineryframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 22:22:24.000000 refineryframe-0.1.2/refineryframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 22:22:24.000000 refineryframe-0.1.2/refineryframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 22:22:24.111378 refineryframe-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-02 22:22:23.000000 refineryframe-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:22:24.111378 refineryframe-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:22:10.000000 refineryframe-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-08-02 22:22:11.000000 refineryframe-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-08-02 22:22:11.000000 refineryframe-0.1.2/tests/test_refiner.py
```

### Comparing `refineryframe-0.1.1/LICENSE` & `refineryframe-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.1/PKG-INFO` & `refineryframe-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Home-page: UNKNOWN
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 License: UNKNOWN
 Keywords: python,data cleaning,safeguards
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -61,14 +61,15 @@
 and searches for any instances of these missing types in each column of the DataFrame.
 - `refineryframe.refiner.Refiner.check_missing_values` - counts the number of NaN, None, and NaT values in each column of a pandas DataFrame.
 - `refineryframe.refiner.Refiner.check_numeric_range` - checks if numeric values are in expected ranges.
 - `refineryframe.refiner.Refiner.detect_unexpected_values` - detects unexpected values in a pandas DataFrame.
 - `refineryframe.refiner.Refiner.get_refiner_settings` - extracts values of parameters from refiner and saves them in dictionary for later use.
 - `refineryframe.refiner.Refiner.get_type_dict_from_dataframe` - returns a dictionary or string representation of a dictionary containing the data types
 of each column in the given pandas DataFrame.
+- `refineryframe.refiner.Refiner.get_unexpected_exceptions_scaned` - returns unexpected_exceptions with appropriate settings to the values in the dataframe.
 - `refineryframe.refiner.Refiner.replace_unexpected_values` - replaces unexpected values in a pandas DataFrame with missing types.
 - `refineryframe.refiner.Refiner.set_refiner_settings` - updates input parameters with values from provided settings dict.
 - `refineryframe.refiner.Refiner.set_type_dict` - changes the data types of the columns in the given DataFrame
 based on a dictionary of intended data types.
 - `refineryframe.refiner.Refiner.set_types` - changes the data types of the columns in the given DataFrame
 based on a dictionary of intended data types.
 
@@ -85,14 +86,15 @@
     * [replacing unexpected values](#replace-unexpected)
     * [moulding types](#moulding-types)
 * [Use of complex targeted conditions](#use-complex-targeted-conditions)
     * [to detect unexpected](#detect_unexpected_with_conds)
     * [to replace unexpected](#replace-unexpected-with-conds)
 * [Refiner class settings](#refiner-class-settings)
     * [extracting settigns](#extracting-refiner-class-settings)
+    * [scanning unexpected conditions](#scanning-dataframe)
     * [recreating identical class with settings](#recreating-refiner-class-settings)
 * [Data quality scores](#scores)
     * [duv score](#duv_scores)
     * [ruv scores](#ruv_scores)
 
 ### Creating example data (exceptionally messy dataframe)
 
@@ -904,14 +906,48 @@
 ### Initializing new clean Refiner
 
 
 ```python
 tns2 = Refiner(dataframe = df)
 ```
 
+#### scanning dataframe for unexpected conditions <a name="scanning-dataframe"></a>
+
+
+```python
+scanned_unexpected_exceptions = tns2.get_unexpected_exceptions_scaned()
+scanned_unexpected_exceptions
+```
+
+    WARNING:Refiner:Column CharColumn: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column DateColumn2: (NA) : 4 : 80.00%
+    WARNING:Refiner:Column NumericColumn: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn_exepted: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn2: (NA) : 4 : 80.00%
+    WARNING:Refiner:Column DateColumn3: (1850-01-09) : 1 : 20.00%
+    WARNING:Refiner:Column DateColumn2 has non-date values or unexpected format.
+    WARNING:Refiner:Column NumericColumn: (INF) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn_exepted: (INF) : 1 : 20.00%
+    WARNING:Refiner:Percentage of passed tests: 71.43%
+
+
+
+
+
+    {'col_names_types': 'NONE',
+     'missing_values': 'ALL',
+     'missing_types': 'ALL',
+     'inf_values': 'ALL',
+     'date_format': 'ALL',
+     'duplicates': 'NONE',
+     'date_range': 'NONE',
+     'numeric_range': 'NONE'}
+
+
+
 #### detection before applying settings
 
 
 ```python
 tns2.detect_unexpected_values()
 ```
 
@@ -945,14 +981,29 @@
     DEBUG:Refiner:=== checking expected date range
     DEBUG:Refiner:=== checking for presense of inf values in numeric colums
     WARNING:Refiner:Column NumericColumn: (INF) : 2 : 40.00%
     WARNING:Refiner:Column NumericColumn_exepted: (INF) : 1 : 20.00%
     WARNING:Refiner:Percentage of passed tests: 66.67%
 
 
+
+```python
+tns3 = Refiner(dataframe = df, 
+               unexpected_exceptions_duv = scanned_unexpected_exceptions)
+```
+
+
+```python
+tns3.detect_unexpected_values()
+print(f'duv score: {tns3.duv_score}')
+```
+
+    duv score: 1.0
+
+
 ### Data quality scores <a class="anchor" id="scores"></a>
 
 ##### DUV score <a class="anchor" id="duv_scores"></a>
 
 The score is the result of checking general conditions with `.detect_unexpected_values()`.
 
 It is a percentange of checks that passed.
```

### Comparing `refineryframe-0.1.1/README.md` & `refineryframe-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 and searches for any instances of these missing types in each column of the DataFrame.
 - `refineryframe.refiner.Refiner.check_missing_values` - counts the number of NaN, None, and NaT values in each column of a pandas DataFrame.
 - `refineryframe.refiner.Refiner.check_numeric_range` - checks if numeric values are in expected ranges.
 - `refineryframe.refiner.Refiner.detect_unexpected_values` - detects unexpected values in a pandas DataFrame.
 - `refineryframe.refiner.Refiner.get_refiner_settings` - extracts values of parameters from refiner and saves them in dictionary for later use.
 - `refineryframe.refiner.Refiner.get_type_dict_from_dataframe` - returns a dictionary or string representation of a dictionary containing the data types
 of each column in the given pandas DataFrame.
+- `refineryframe.refiner.Refiner.get_unexpected_exceptions_scaned` - returns unexpected_exceptions with appropriate settings to the values in the dataframe.
 - `refineryframe.refiner.Refiner.replace_unexpected_values` - replaces unexpected values in a pandas DataFrame with missing types.
 - `refineryframe.refiner.Refiner.set_refiner_settings` - updates input parameters with values from provided settings dict.
 - `refineryframe.refiner.Refiner.set_type_dict` - changes the data types of the columns in the given DataFrame
 based on a dictionary of intended data types.
 - `refineryframe.refiner.Refiner.set_types` - changes the data types of the columns in the given DataFrame
 based on a dictionary of intended data types.
 
@@ -62,14 +63,15 @@
     * [replacing unexpected values](#replace-unexpected)
     * [moulding types](#moulding-types)
 * [Use of complex targeted conditions](#use-complex-targeted-conditions)
     * [to detect unexpected](#detect_unexpected_with_conds)
     * [to replace unexpected](#replace-unexpected-with-conds)
 * [Refiner class settings](#refiner-class-settings)
     * [extracting settigns](#extracting-refiner-class-settings)
+    * [scanning unexpected conditions](#scanning-dataframe)
     * [recreating identical class with settings](#recreating-refiner-class-settings)
 * [Data quality scores](#scores)
     * [duv score](#duv_scores)
     * [ruv scores](#ruv_scores)
 
 ### Creating example data (exceptionally messy dataframe)
 
@@ -881,14 +883,48 @@
 ### Initializing new clean Refiner
 
 
 ```python
 tns2 = Refiner(dataframe = df)
 ```
 
+#### scanning dataframe for unexpected conditions <a name="scanning-dataframe"></a>
+
+
+```python
+scanned_unexpected_exceptions = tns2.get_unexpected_exceptions_scaned()
+scanned_unexpected_exceptions
+```
+
+    WARNING:Refiner:Column CharColumn: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column DateColumn2: (NA) : 4 : 80.00%
+    WARNING:Refiner:Column NumericColumn: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn_exepted: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn2: (NA) : 4 : 80.00%
+    WARNING:Refiner:Column DateColumn3: (1850-01-09) : 1 : 20.00%
+    WARNING:Refiner:Column DateColumn2 has non-date values or unexpected format.
+    WARNING:Refiner:Column NumericColumn: (INF) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn_exepted: (INF) : 1 : 20.00%
+    WARNING:Refiner:Percentage of passed tests: 71.43%
+
+
+
+
+
+    {'col_names_types': 'NONE',
+     'missing_values': 'ALL',
+     'missing_types': 'ALL',
+     'inf_values': 'ALL',
+     'date_format': 'ALL',
+     'duplicates': 'NONE',
+     'date_range': 'NONE',
+     'numeric_range': 'NONE'}
+
+
+
 #### detection before applying settings
 
 
 ```python
 tns2.detect_unexpected_values()
 ```
 
@@ -922,14 +958,29 @@
     DEBUG:Refiner:=== checking expected date range
     DEBUG:Refiner:=== checking for presense of inf values in numeric colums
     WARNING:Refiner:Column NumericColumn: (INF) : 2 : 40.00%
     WARNING:Refiner:Column NumericColumn_exepted: (INF) : 1 : 20.00%
     WARNING:Refiner:Percentage of passed tests: 66.67%
 
 
+
+```python
+tns3 = Refiner(dataframe = df, 
+               unexpected_exceptions_duv = scanned_unexpected_exceptions)
+```
+
+
+```python
+tns3.detect_unexpected_values()
+print(f'duv score: {tns3.duv_score}')
+```
+
+    duv score: 1.0
+
+
 ### Data quality scores <a class="anchor" id="scores"></a>
 
 ##### DUV score <a class="anchor" id="duv_scores"></a>
 
 The score is the result of checking general conditions with `.detect_unexpected_values()`.
 
 It is a percentange of checks that passed.
```

### Comparing `refineryframe-0.1.1/refineryframe/detect_unexpected.py` & `refineryframe-0.1.2/refineryframe/detect_unexpected.py`

 * *Files 4% similar despite different names*

```diff
@@ -618,15 +618,15 @@
                              types_dict_str : dict = None,
                              expected_date_format : str = '%Y-%m-%d',
                              earliest_date : str = "1900-08-25",
                              latest_date : str = "2100-01-01",
                              numeric_lower_bound : float = 0,
                              numeric_upper_bound : float = float("inf"),
                              print_score : bool = True,
-                            logger : logging.Logger = logging) -> float:
+                            logger : logging.Logger = logging) -> dict:
 
     """
     Detect unexpected values in a pandas DataFrame.
 
     Parameters:
     -----------
 
@@ -643,15 +643,16 @@
     earliest_date (str): The earliest acceptable date (default is "1900-08-25").
     latest_date (str): The latest acceptable date (default is "2100-01-01").
     numeric_lower_bound (float): The lowest acceptable value for numeric columns (default is 0).
     numeric_upper_bound (float): The highest acceptable value for numeric columns
                                     (default is infinity).
 
     Returns:
-        duv_score - number between 0 and 1 that means what percentage of tests have passed
+        duv_score (float) - number between 0 and 1 that means what percentage of tests have passed
+        unexpected_exceptions_scaned - unexpected_exceptions based on detected unexpected values
     """
 
 
     try:
 
 
         # Separate column names by major types
@@ -708,96 +709,131 @@
             run_check_additional_cons = False
 
 
         if ids_for_dup is None:
             ids_for_dup = index_cols
 
 
-        # Run checks
+        # Checks scan
+        unexpected_exceptions_scaned = {
+            "col_names_types": "NONE",
+            "missing_values": "NONE",
+            "missing_types": "NONE",
+            "inf_values": "NONE",
+            "date_format": "NONE",
+            "duplicates": "NONE",
+            "date_range": "NONE",
+            "numeric_range": "NONE"
+        }
 
+        # Run checks
         checks_list = []
 
 
         if run_check_col_names_types:
 
             logger.debug(f"=== checking column names and types")
 
             checks_list.extend(check_col_names_types(dataframe = dataframe[cols_check_col_names_types],
                                                        types_dict_str = types_dict_str,
                                                        independent = False,
                                                        logger = logger))
 
+            if not checks_list[-1]:
+                unexpected_exceptions_scaned["col_names_types"] = "ALL"
+
         if run_check_missing_values:
 
             logger.debug("=== checking for presence of missing values")
 
             checks_list.extend([check_missing_values(dataframe = dataframe[cols_check_missing_values],
                                                      logger = logger)])
 
+            if not checks_list[-1]:
+                unexpected_exceptions_scaned["missing_values"] = "ALL"
+
         if run_check_missing_types:
 
             logger.debug("=== checking for presence of missing types")
 
             checks_list.extend(check_missing_types(dataframe = dataframe[cols_check_missing_types],
                                                     MISSING_TYPES = MISSING_TYPES,
                                                     independent = False,
                                                     logger = logger))
 
+            if not checks_list[-1]:
+                unexpected_exceptions_scaned["missing_types"] = "ALL"
+
         if run_check_date_format:
 
             logger.debug("=== checking propper date format")
 
             checks_list.extend([check_date_format(dataframe = dataframe[cols_check_date_format],
                                                   expected_date_format = expected_date_format,
                                                   independent = False,
                                                   logger = logger)])
 
+            if not checks_list[-1]:
+                unexpected_exceptions_scaned["date_format"] = "ALL"
+
 
         if run_check_date_range:
 
             logger.debug("=== checking expected date range")
 
             checks_list.extend(check_date_range(dataframe = dataframe[cols_check_date_range],
                                                  earliest_date = earliest_date,
                                                  latest_date = latest_date,
                                                  independent = False,
                                                  ignore_dates = [v for k, v in MISSING_TYPES.items()
                                                                  if k.startswith("date_")],
                                                  logger = logger))
 
+            if not checks_list[-1]:
+                unexpected_exceptions_scaned["date_range"] = "ALL"
+
         if run_check_duplicates:
 
             logger.debug("=== checking for duplicates")
 
             checks_list.extend(check_duplicates(dataframe = dataframe[cols_check_duplicates],
                              subset = ids_for_dup,
                              independent = False,
                              logger = logger))
 
+            if not checks_list[-1]:
+                unexpected_exceptions_scaned["duplicates"] = "ALL"
+
 
         if run_check_inf_values:
 
             logger.debug("=== checking for presense of inf values in numeric colums")
 
             checks_list.extend([check_inf_values(dataframe = dataframe[cols_check_inf_values],
                                                  independent = False,
                                                  logger = logger)])
 
+            if not checks_list[-1]:
+                unexpected_exceptions_scaned["inf_values"] = "ALL"
+
         if run_check_numeric_range:
 
             logger.debug("=== checking expected numeric range")
 
             checks_list.extend(check_numeric_range(dataframe = dataframe[cols_check_numeric_range],
                                                     lower_bound = numeric_lower_bound,
                                                     upper_bound = numeric_upper_bound,
                                                     independent = False,
                                                     ignore_values = [v for k, v in MISSING_TYPES.items()
                                                                      if k.startswith("numeric_")],
                                                     logger = logger))
 
+            if not checks_list[-1]:
+                unexpected_exceptions_scaned["numeric_range"] = "ALL"
+
 
         if run_check_additional_cons:
 
             logger.debug("=== checking additional cons")
 
             conds = [i for i in unexpected_conditions if unexpected_conditions[i]['warning']]
 
@@ -825,13 +861,14 @@
         if TEST_DUV_FLAGS_PATH is not None:
 
             with open(TEST_DUV_FLAGS_PATH, "w", encoding="utf8") as f:
                 f.write(str(duv_score))
 
         else:
 
-            return duv_score
+            return {'duv_score' : duv_score,
+                    'unexpected_exceptions_scaned' : unexpected_exceptions_scaned}
 
 
     except Exception as e:
         logger.error("Error occured during duv score calculation!")
         print("The error:", e)
```

### Comparing `refineryframe-0.1.1/refineryframe/other.py` & `refineryframe-0.1.2/refineryframe/other.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.1/refineryframe/refiner.py` & `refineryframe-0.1.2/refineryframe/refiner.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
     unexpected_conditions = attr.ib(default=None)
 
     ignore_values = attr.ib(default=[])
     ignore_dates = attr.ib(default=[])
 
     # outputs
+    unexpected_exceptions_scaned = attr.ib(default={},init = False, type=dict)
     type_dict = attr.ib(default={}, init = False, type=dict)
 
     MISSING_TYPES_TEST = attr.ib(default=None, init = False)
     MISSING_COUNT_TEST = attr.ib(default=None, init = False)
     NUM_INF_TEST = attr.ib(default=None, init = False)
     DATE_FORMAT_TEST = attr.ib(default=None, init = False)
     DATE_RANGE_TEST = attr.ib(default=None, init = False)
@@ -111,15 +112,15 @@
         shoutOUT(output_type=self.shout_type,
                  mess=mess,
                  dotline_length=self.dotline_length,
                  logger=self.logger)
 
     def get_type_dict_from_dataframe(self,
                       explicit=True,
-                      stringout=False):
+                      stringout=False) -> dict:
 
         """
         Returns a dictionary or string representation of a dictionary containing the data types
         of each column in the given pandas DataFrame.
 
         Numeric columns will have type 'numeric', date columns will have type 'date',
         character columns will have type 'category', and columns containing 'id' at
@@ -131,15 +132,15 @@
                                        stringout=stringout)
 
         return type_dict
 
     def set_type_dict(self,
                       type_dict=None,
                       explicit=True,
-                      stringout=False):
+                      stringout=False) -> None:
 
         """
         Changes the data types of the columns in the given DataFrame
         based on a dictionary of intended data types.
         """
 
         if type_dict is None:
@@ -188,14 +189,15 @@
                       'NUM_INF_TEST',
                       'DATE_FORMAT_TEST',
                       'DATE_RANGE_TEST',
                       'DUPLICATES_TEST',
                       'COL_NAMES_TYPES_TEST',
                       'NUMERIC_RANGE_TEST',
                       'logger',
+                      'unexpected_exceptions_scaned',
                       'duv_score',
                       'ruv_score0',
                       'ruv_score1',
                       'ruv_score2']
 
         # Getting the dictionary representation of the instance
         my_instance_dict = attr.asdict(self)
@@ -370,29 +372,61 @@
         if latest_date is None:
             latest_date = self.latest_date
         if numeric_lower_bound is None:
             numeric_lower_bound = self.lower_bound
         if numeric_upper_bound is None:
             numeric_upper_bound = self.upper_bound
 
-        self.duv_score = detect_unexpected_values(dataframe = self.dataframe,
+        duv_obj = detect_unexpected_values(dataframe = self.dataframe,
                                                  MISSING_TYPES = MISSING_TYPES,
                                                  unexpected_exceptions = unexpected_exceptions,
                                                  unexpected_conditions = unexpected_conditions,
                                                  ids_for_dup = ids_for_dup,
                                                  TEST_DUV_FLAGS_PATH = TEST_DUV_FLAGS_PATH,
                                                  types_dict_str = types_dict_str,
                                                  expected_date_format = expected_date_format,
                                                  earliest_date = earliest_date,
                                                  latest_date = latest_date,
                                                  numeric_lower_bound = numeric_lower_bound,
                                                  numeric_upper_bound = numeric_upper_bound,
                                                  print_score = print_score,
                                       logger = self.logger)
 
+        self.duv_score = duv_obj['duv_score']
+        self.unexpected_exceptions_scaned = duv_obj['unexpected_exceptions_scaned']
+
+    def get_unexpected_exceptions_scaned(self, dataframe = None) -> dict:
+
+        """
+        Returns unexpected_exceptions with appropriate settings to the values in the dataframe.
+        """
+
+        if dataframe is None:
+            dataframe = self.dataframe
+
+        duv_obj = detect_unexpected_values(dataframe = dataframe,
+                                                 MISSING_TYPES = self.MISSING_TYPES,
+                                                 unexpected_exceptions = self.unexpected_exceptions_duv,
+                                                 unexpected_conditions = self.unexpected_conditions,
+                                                 ids_for_dup = None,
+                                                 TEST_DUV_FLAGS_PATH = None,
+                                                 types_dict_str = self.type_dict,
+                                                 expected_date_format = self.expected_date_format,
+                                                 earliest_date = self.earliest_date,
+                                                 latest_date = self.latest_date,
+                                                 numeric_lower_bound = self.lower_bound,
+                                                 numeric_upper_bound = self.upper_bound,
+                                                 print_score = True,
+                                      logger = self.logger)
+
+        return duv_obj['unexpected_exceptions_scaned']
+
+
+
+
     def replace_unexpected_values(self,
                              MISSING_TYPES = None,
                              unexpected_exceptions = None,
                              unexpected_conditions = None,
                              TEST_RUV_FLAGS_PATH = None,
                              earliest_date = None,
                              latest_date = None,
```

### Comparing `refineryframe-0.1.1/refineryframe/replace_unexpected.py` & `refineryframe-0.1.2/refineryframe/replace_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.1/refineryframe.egg-info/PKG-INFO` & `refineryframe-0.1.2/refineryframe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Home-page: UNKNOWN
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 License: UNKNOWN
 Keywords: python,data cleaning,safeguards
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -61,14 +61,15 @@
 and searches for any instances of these missing types in each column of the DataFrame.
 - `refineryframe.refiner.Refiner.check_missing_values` - counts the number of NaN, None, and NaT values in each column of a pandas DataFrame.
 - `refineryframe.refiner.Refiner.check_numeric_range` - checks if numeric values are in expected ranges.
 - `refineryframe.refiner.Refiner.detect_unexpected_values` - detects unexpected values in a pandas DataFrame.
 - `refineryframe.refiner.Refiner.get_refiner_settings` - extracts values of parameters from refiner and saves them in dictionary for later use.
 - `refineryframe.refiner.Refiner.get_type_dict_from_dataframe` - returns a dictionary or string representation of a dictionary containing the data types
 of each column in the given pandas DataFrame.
+- `refineryframe.refiner.Refiner.get_unexpected_exceptions_scaned` - returns unexpected_exceptions with appropriate settings to the values in the dataframe.
 - `refineryframe.refiner.Refiner.replace_unexpected_values` - replaces unexpected values in a pandas DataFrame with missing types.
 - `refineryframe.refiner.Refiner.set_refiner_settings` - updates input parameters with values from provided settings dict.
 - `refineryframe.refiner.Refiner.set_type_dict` - changes the data types of the columns in the given DataFrame
 based on a dictionary of intended data types.
 - `refineryframe.refiner.Refiner.set_types` - changes the data types of the columns in the given DataFrame
 based on a dictionary of intended data types.
 
@@ -85,14 +86,15 @@
     * [replacing unexpected values](#replace-unexpected)
     * [moulding types](#moulding-types)
 * [Use of complex targeted conditions](#use-complex-targeted-conditions)
     * [to detect unexpected](#detect_unexpected_with_conds)
     * [to replace unexpected](#replace-unexpected-with-conds)
 * [Refiner class settings](#refiner-class-settings)
     * [extracting settigns](#extracting-refiner-class-settings)
+    * [scanning unexpected conditions](#scanning-dataframe)
     * [recreating identical class with settings](#recreating-refiner-class-settings)
 * [Data quality scores](#scores)
     * [duv score](#duv_scores)
     * [ruv scores](#ruv_scores)
 
 ### Creating example data (exceptionally messy dataframe)
 
@@ -904,14 +906,48 @@
 ### Initializing new clean Refiner
 
 
 ```python
 tns2 = Refiner(dataframe = df)
 ```
 
+#### scanning dataframe for unexpected conditions <a name="scanning-dataframe"></a>
+
+
+```python
+scanned_unexpected_exceptions = tns2.get_unexpected_exceptions_scaned()
+scanned_unexpected_exceptions
+```
+
+    WARNING:Refiner:Column CharColumn: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column DateColumn2: (NA) : 4 : 80.00%
+    WARNING:Refiner:Column NumericColumn: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn_exepted: (NA) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn2: (NA) : 4 : 80.00%
+    WARNING:Refiner:Column DateColumn3: (1850-01-09) : 1 : 20.00%
+    WARNING:Refiner:Column DateColumn2 has non-date values or unexpected format.
+    WARNING:Refiner:Column NumericColumn: (INF) : 2 : 40.00%
+    WARNING:Refiner:Column NumericColumn_exepted: (INF) : 1 : 20.00%
+    WARNING:Refiner:Percentage of passed tests: 71.43%
+
+
+
+
+
+    {'col_names_types': 'NONE',
+     'missing_values': 'ALL',
+     'missing_types': 'ALL',
+     'inf_values': 'ALL',
+     'date_format': 'ALL',
+     'duplicates': 'NONE',
+     'date_range': 'NONE',
+     'numeric_range': 'NONE'}
+
+
+
 #### detection before applying settings
 
 
 ```python
 tns2.detect_unexpected_values()
 ```
 
@@ -945,14 +981,29 @@
     DEBUG:Refiner:=== checking expected date range
     DEBUG:Refiner:=== checking for presense of inf values in numeric colums
     WARNING:Refiner:Column NumericColumn: (INF) : 2 : 40.00%
     WARNING:Refiner:Column NumericColumn_exepted: (INF) : 1 : 20.00%
     WARNING:Refiner:Percentage of passed tests: 66.67%
 
 
+
+```python
+tns3 = Refiner(dataframe = df, 
+               unexpected_exceptions_duv = scanned_unexpected_exceptions)
+```
+
+
+```python
+tns3.detect_unexpected_values()
+print(f'duv score: {tns3.duv_score}')
+```
+
+    duv score: 1.0
+
+
 ### Data quality scores <a class="anchor" id="scores"></a>
 
 ##### DUV score <a class="anchor" id="duv_scores"></a>
 
 The score is the result of checking general conditions with `.detect_unexpected_values()`.
 
 It is a percentange of checks that passed.
```

### Comparing `refineryframe-0.1.1/setup.py` & `refineryframe-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "attrs>=22.2.0",
     "datetime",
     "pandas",
     "numpy",
     "unidecode"
 ]
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'Cleans data, best to be used as a part of initial preprocessor'
 LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them according to set of predefined rules'
 
 # Setting up
 setup(
     name="refineryframe",
     #use_scm_version=True,
@@ -29,15 +29,15 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=base_packages,
     keywords=['python', 'data cleaning', 'safeguards'],
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
```

### Comparing `refineryframe-0.1.1/tests/conftest.py` & `refineryframe-0.1.2/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,14 +118,31 @@
     "numeric_range": "ALL"
 }
 
     yield unexpected_exceptions2
 
 
 @pytest.fixture(scope='session')
+def scanned_unexpected_exceptions():
+
+    scanned_unexpected_exceptions = {
+                "col_names_types": "NONE",
+                "missing_values": "ALL",
+                "missing_types": "NONE",
+                "inf_values": "ALL",
+                "date_format": "ALL",
+                "duplicates": "NONE",
+                "date_range": "ALL",
+                "numeric_range": "NONE"
+            }
+
+    yield scanned_unexpected_exceptions
+
+
+@pytest.fixture(scope='session')
 def refiner_settings():
 
     refiner_settings = {'replace_dict': {-996: -999, '1000-01-09': '1850-01-09'},
                         'MISSING_TYPES': {'date_not_delivered': '1850-01-09',
                         'numeric_not_delivered': -999,
                         'character_not_delivered': 'missing'},
                         'expected_date_format': '%Y-%m-%d',
```

### Comparing `refineryframe-0.1.1/tests/test_refiner.py` & `refineryframe-0.1.2/tests/test_refiner.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,14 +113,21 @@
     assert "checking expected date range" in caplog.text
     assert "Not all dates in DateColumn are later than DateColumn3" in caplog.text
     assert "checking for presense of inf values in numeric colums" in caplog.text
     assert "checking expected numeric range" in caplog.text
     assert "Percentage of passed tests: 50.00%" in caplog.text
 
 
+def test_get_unexpected_exceptions_scaned(tns, scanned_unexpected_exceptions):
+
+    scanned_unexpected_exceptions2 = tns.get_unexpected_exceptions_scaned()
+
+    assert scanned_unexpected_exceptions2 == scanned_unexpected_exceptions
+
+
 def test_duv_score1(tns):
 
     assert tns.duv_score == 0.5
 
 
 def test_replace_unexpected(tns,df1, caplog):
 
@@ -201,14 +208,15 @@
 
 def test_get_refiner_settings(tns2,refiner_settings):
 
     refiner_settings2 = tns2.get_refiner_settings()
 
     assert refiner_settings2 == refiner_settings
 
+
 def test_set_refiner_settings(tns2,df, refiner_settings):
 
     tns = Refiner(dataframe = df)
 
     tns.set_refiner_settings(refiner_settings)
 
     tns.shout(mess = "TNS1")
```

