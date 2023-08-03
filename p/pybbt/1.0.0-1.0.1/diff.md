# Comparing `tmp/pybbt-1.0.0.tar.gz` & `tmp/pybbt-1.0.1.tar.gz`

## Comparing `pybbt-1.0.0.tar` & `pybbt-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pybbt-1.0.0/.DS_Store
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/__init__.py
--rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/__main__.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/assertion.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/case.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/context.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/error_case.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/launcher.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/logger.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/safe_thread.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/subcase.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/pybbt/__init__.py
--rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/pybbt/__main__.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/pybbt/assertion.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/pybbt/case.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/pybbt/context.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/pybbt/error_case.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/pybbt/launcher.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/pybbt/logger.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/pybbt/safe_thread.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/pybbt/subcase.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/pybbt/utils/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/pybbt/utils/filesystem.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/pybbt/utils/timer.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/utils/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/utils/filesystem.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pybbt-1.0.0/pybbt/utils/timer.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pybbt-1.0.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pybbt-1.0.0/LICENSE
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 pybbt-1.0.0/README.md
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pybbt-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 pybbt-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pybbt-1.0.1/.DS_Store
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/__init__.py
+-rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/__main__.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/assertion.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/case.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/context.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/error_case.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/launcher.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/logger.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/safe_thread.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/subcase.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/pybbt/__init__.py
+-rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/pybbt/__main__.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/pybbt/assertion.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/pybbt/case.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/pybbt/context.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/pybbt/error_case.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/pybbt/launcher.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/pybbt/logger.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/pybbt/safe_thread.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/pybbt/subcase.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/pybbt/utils/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/pybbt/utils/filesystem.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/pybbt/utils/timer.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/utils/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/utils/filesystem.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pybbt-1.0.1/pybbt/utils/timer.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pybbt-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pybbt-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 pybbt-1.0.1/README.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pybbt-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 pybbt-1.0.1/PKG-INFO
```

### Comparing `pybbt-1.0.0/.DS_Store` & `pybbt-1.0.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/__init__.py` & `pybbt-1.0.1/pybbt/__init__.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/__main__.py` & `pybbt-1.0.1/pybbt/__main__.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/assertion.py` & `pybbt-1.0.1/pybbt/assertion.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/case.py` & `pybbt-1.0.1/pybbt/case.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/context.py` & `pybbt-1.0.1/pybbt/context.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/error_case.py` & `pybbt-1.0.1/pybbt/error_case.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/launcher.py` & `pybbt-1.0.1/pybbt/launcher.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/logger.py` & `pybbt-1.0.1/pybbt/logger.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/safe_thread.py` & `pybbt-1.0.1/pybbt/safe_thread.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/subcase.py` & `pybbt-1.0.1/pybbt/subcase.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/pybbt/__init__.py` & `pybbt-1.0.1/pybbt/pybbt/__init__.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/pybbt/__main__.py` & `pybbt-1.0.1/pybbt/pybbt/__main__.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/pybbt/assertion.py` & `pybbt-1.0.1/pybbt/pybbt/assertion.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/pybbt/case.py` & `pybbt-1.0.1/pybbt/pybbt/case.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/pybbt/context.py` & `pybbt-1.0.1/pybbt/pybbt/context.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/pybbt/error_case.py` & `pybbt-1.0.1/pybbt/pybbt/error_case.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/pybbt/launcher.py` & `pybbt-1.0.1/pybbt/pybbt/launcher.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/pybbt/logger.py` & `pybbt-1.0.1/pybbt/pybbt/logger.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/pybbt/safe_thread.py` & `pybbt-1.0.1/pybbt/pybbt/safe_thread.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pybbt/pybbt/subcase.py` & `pybbt-1.0.1/pybbt/pybbt/subcase.py`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/LICENSE` & `pybbt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/README.md` & `pybbt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pybbt-1.0.0/pyproject.toml` & `pybbt-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pybbt"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name = "Tair", email = "tair-opensource@alibabacloud.com" },
     { name = "suxb201", email = "suxb201@gmail.com" },
 ]
 description = "pybbt is a Python-based tool that simplifies black box testing of software. It provides a range of auxiliary functions and the ability to filter test cases, making your testing process more efficient and manageable."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = ["rich >= 13.5.2"]
 
 [project.scripts]
 pybbt = "pybbt.__main__:main"
 
 [project.urls]
 "Homepage" = "https://github.com/tair-opensource/pybbt"
 "Bug Tracker" = "https://github.com/tair-opensource/pybbt/issues"
-
```

### Comparing `pybbt-1.0.0/PKG-INFO` & `pybbt-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pybbt
-Version: 1.0.0
+Version: 1.0.1
 Summary: pybbt is a Python-based tool that simplifies black box testing of software. It provides a range of auxiliary functions and the ability to filter test cases, making your testing process more efficient and manageable.
 Project-URL: Homepage, https://github.com/tair-opensource/pybbt
 Project-URL: Bug Tracker, https://github.com/tair-opensource/pybbt/issues
 Author-email: Tair <tair-opensource@alibabacloud.com>, suxb201 <suxb201@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
+Requires-Dist: rich>=13.5.2
 Description-Content-Type: text/markdown
 
 # pybbt: Python Black Box Testing Tool
 
 pybbt is a Python-based tool that simplifies black box testing of software. It provides a range of auxiliary functions and the ability to filter test cases, making your testing
 process more efficient and manageable.
```

