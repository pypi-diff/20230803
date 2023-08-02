# Comparing `tmp/robotframework_asyncio_utils-0.1.1.tar.gz` & `tmp/robotframework_asyncio_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_asyncio_utils-0.1.1.tar", max compression
+gzip compressed data, was "robotframework_asyncio_utils-0.1.2.tar", max compression
```

## Comparing `robotframework_asyncio_utils-0.1.1.tar` & `robotframework_asyncio_utils-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       41 2023-08-02 20:34:16.257913 robotframework_asyncio_utils-0.1.1/asyncio_utils/__init__.py
--rw-r--r--   0        0        0     5804 2023-08-02 22:26:30.894935 robotframework_asyncio_utils-0.1.1/asyncio_utils/asyncio_utils.py
--rw-r--r--   0        0        0     1090 2023-08-02 22:42:06.375801 robotframework_asyncio_utils-0.1.1/LICENSE
--rw-r--r--   0        0        0      486 2023-08-02 23:10:13.456113 robotframework_asyncio_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      283 2023-08-02 22:54:32.449869 robotframework_asyncio_utils-0.1.1/README.md
--rw-r--r--   0        0        0      837 1970-01-01 00:00:00.000000 robotframework_asyncio_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-08-02 20:34:16.257913 robotframework_asyncio_utils-0.1.2/asyncio_utils/__init__.py
+-rw-r--r--   0        0        0     5804 2023-08-02 22:26:30.894935 robotframework_asyncio_utils-0.1.2/asyncio_utils/asyncio_utils.py
+-rw-r--r--   0        0        0     1090 2023-08-02 22:42:06.375801 robotframework_asyncio_utils-0.1.2/LICENSE
+-rw-r--r--   0        0        0      551 2023-08-02 23:15:22.527513 robotframework_asyncio_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      283 2023-08-02 22:54:32.449869 robotframework_asyncio_utils-0.1.2/README.md
+-rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 robotframework_asyncio_utils-0.1.2/PKG-INFO
```

### Comparing `robotframework_asyncio_utils-0.1.1/asyncio_utils/asyncio_utils.py` & `robotframework_asyncio_utils-0.1.2/asyncio_utils/asyncio_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_asyncio_utils-0.1.1/LICENSE` & `robotframework_asyncio_utils-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_asyncio_utils-0.1.1/PKG-INFO` & `robotframework_asyncio_utils-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: robotframework-asyncio-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
+Home-page: https://github.com/ygorpontelo/robot-asyncio-utils
 License: MIT
 Author: Ygor Pontelo
 Author-email: ygorpontelo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

