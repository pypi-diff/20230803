# Comparing `tmp/findmyorder-1.7.1.tar.gz` & `tmp/findmyorder-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.7.1.tar", max compression
+gzip compressed data, was "findmyorder-1.7.2.tar", max compression
```

## Comparing `findmyorder-1.7.1.tar` & `findmyorder-1.7.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-25 19:53:10.390204 findmyorder-1.7.1/LICENSE
--rw-r--r--   0        0        0     3022 2023-07-25 19:53:10.390204 findmyorder-1.7.1/README.md
--rw-r--r--   0        0        0      113 2023-07-25 19:53:14.898631 findmyorder-1.7.1/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-07-25 19:53:10.390204 findmyorder-1.7.1/findmyorder/config.py
--rw-r--r--   0        0        0     3221 2023-07-25 19:53:10.390204 findmyorder-1.7.1/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5931 2023-07-25 19:53:10.390204 findmyorder-1.7.1/findmyorder/main.py
--rw-r--r--   0        0        0     3002 2023-07-25 19:53:14.890630 findmyorder-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 findmyorder-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-03 19:54:06.072248 findmyorder-1.7.2/LICENSE
+-rw-r--r--   0        0        0     3022 2023-08-03 19:54:06.072248 findmyorder-1.7.2/README.md
+-rw-r--r--   0        0        0      113 2023-08-03 19:54:11.976315 findmyorder-1.7.2/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-08-03 19:54:06.072248 findmyorder-1.7.2/findmyorder/config.py
+-rw-r--r--   0        0        0     3221 2023-08-03 19:54:06.072248 findmyorder-1.7.2/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5931 2023-08-03 19:54:06.072248 findmyorder-1.7.2/findmyorder/main.py
+-rw-r--r--   0        0        0     2868 2023-08-03 19:54:11.968315 findmyorder-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 findmyorder-1.7.2/PKG-INFO
```

### Comparing `findmyorder-1.7.1/LICENSE` & `findmyorder-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.1/README.md` & `findmyorder-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.1/findmyorder/config.py` & `findmyorder-1.7.2/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.1/findmyorder/default_settings.toml` & `findmyorder-1.7.2/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.1/findmyorder/main.py` & `findmyorder-1.7.2/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.1/pyproject.toml` & `findmyorder-1.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "findmyorder"
-version = "1.7.1"
+version = "1.7.2"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
@@ -63,22 +63,18 @@
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.2.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^7.0.0"
+sphinx = ">=5,<6"
 sphinx_bootstrap_theme = "^0.8.1"
-sphinx-autoapi = "^2.1.1"
-sphinx-copybutton= "^0.5.2"
-myst-parser = "^2.0.0"
-sphinx-notfound-page = "^0.8.3"
 sphinxext-remoteliteralinclude = "^0.4.0"
-sphinx-togglebutton = "*"
+
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
```

### Comparing `findmyorder-1.7.1/PKG-INFO` & `findmyorder-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.7.1
+Version: 1.7.2
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: findmyorder Version: 1.7.1 Summary: A python
+Metadata-Version: 2.1 Name: findmyorder Version: 1.7.2 Summary: A python
 package to identify and parse order for trade execution. License: MIT Keywords:
 trading,order,trade,buy,sell Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: emoji (>=2.5.1,<3.0.0) Requires-Dist: loguru
```

