# Comparing `tmp/enmerkar-underscore-2.1.0.tar.gz` & `tmp/enmerkar-underscore-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enmerkar-underscore-2.1.0.tar", last modified: Mon Jul 12 08:57:32 2021, max compression
+gzip compressed data, was "enmerkar-underscore-2.2.0.tar", last modified: Thu Aug  3 11:04:02 2023, max compression
```

## Comparing `enmerkar-underscore-2.1.0.tar` & `enmerkar-underscore-2.2.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 08:57:32.922159 enmerkar-underscore-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3366 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      243 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3373 2021-07-12 08:57:32.922159 enmerkar-underscore-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      741 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 08:57:32.922159 enmerkar-underscore-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6777 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8609 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      529 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6466 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)      113 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-07-12 08:57:32.922159 enmerkar-underscore-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2746 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 08:57:32.918159 enmerkar-underscore-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 08:57:32.922159 enmerkar-underscore-2.1.0/src/enmerkar_underscore/
--rw-r--r--   0 runner    (1001) docker     (121)     3197 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/src/enmerkar_underscore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 08:57:32.922159 enmerkar-underscore-2.1.0/src/enmerkar_underscore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3373 2021-07-12 08:57:32.000000 enmerkar-underscore-2.1.0/src/enmerkar_underscore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      661 2021-07-12 08:57:32.000000 enmerkar-underscore-2.1.0/src/enmerkar_underscore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-12 08:57:32.000000 enmerkar-underscore-2.1.0/src/enmerkar_underscore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-07-12 08:57:32.000000 enmerkar-underscore-2.1.0/src/enmerkar_underscore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-12 08:57:32.000000 enmerkar-underscore-2.1.0/src/enmerkar_underscore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-07-12 08:57:32.000000 enmerkar-underscore-2.1.0/src/enmerkar_underscore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-07-12 08:57:32.000000 enmerkar-underscore-2.1.0/src/enmerkar_underscore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 08:57:32.922159 enmerkar-underscore-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1976 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2021-07-12 08:57:28.000000 enmerkar-underscore-2.1.0/tests/test_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:04:02.478622 enmerkar-underscore-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-08-03 11:04:02.478622 enmerkar-underscore-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:04:02.474622 enmerkar-underscore-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     6777 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8609 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6466 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:04:02.474622 enmerkar-underscore-2.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-08-03 11:04:02.478622 enmerkar-underscore-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5710 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:04:02.474622 enmerkar-underscore-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:04:02.474622 enmerkar-underscore-2.2.0/src/enmerkar_underscore/
+-rw-r--r--   0 runner    (1001) docker     (122)     3218 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:04:02.478622 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-08-03 11:04:02.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-08-03 11:04:02.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 11:04:02.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-08-03 11:04:02.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 11:04:02.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-08-03 11:04:02.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-08-03 11:04:02.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:04:02.478622 enmerkar-underscore-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2006 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/tests/test_extract.py
```

### Comparing `enmerkar-underscore-2.1.0/CONTRIBUTING.rst` & `enmerkar-underscore-2.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.1.0/HISTORY.rst` & `enmerkar-underscore-2.2.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.1.0/LICENSE` & `enmerkar-underscore-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.1.0/README.rst` & `enmerkar-underscore-2.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 =================================
 Django Babel Underscore Extractor
 =================================
 
 .. image:: https://badge.fury.io/py/django-babel-underscore.png
     :target: http://badge.fury.io/py/django-babel-underscore
 
-.. image:: https://github.com/edx/enmerkar-underscore/workflows/Python%20CI/badge.svg?branch=master
-        :target: https://github.com/edx/enmerkar-underscore/actions?query=workflow%3A%22Python+CI%22
+.. image:: https://github.com/openedx/enmerkar-underscore/workflows/Python%20CI/badge.svg?branch=master
+        :target: https://github.com/openedx/enmerkar-underscore/actions?query=workflow%3A%22Python+CI%22
 
 .. image:: https://pypip.in/d/django-babel-underscore/badge.png
         :target: https://pypi.python.org/pypi/django-babel-underscore
 
 
 Implements a underscore extractor for django-babel.
```

### Comparing `enmerkar-underscore-2.1.0/docs/Makefile` & `enmerkar-underscore-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.1.0/docs/conf.py` & `enmerkar-underscore-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.1.0/docs/index.rst` & `enmerkar-underscore-2.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.1.0/docs/make.bat` & `enmerkar-underscore-2.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.1.0/src/enmerkar_underscore/__init__.py` & `enmerkar-underscore-2.2.0/src/enmerkar_underscore/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 
 if django.VERSION[:2] >= (2, 1):
     from django.template.base import TokenType
     TOKEN_TEXT = TokenType.TEXT
 else:  # django < 2.1
     from django.template.base import TOKEN_TEXT
 
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from enmerkar.extract import extract_django
 from markey import underscore
 from markey.tools import TokenStream
 from markey.machine import tokenize, parse_arguments
 
 
+__version__ = '2.2.0'
+
 def extract(fileobj, keywords, comment_tags, options):
     """Extracts translation messages from underscore template files.
 
     This method does also extract django templates. If a template does not
     contain any django translation tags we always fallback to underscore extraction.
 
     This is a plugin to Babel, written according to
@@ -71,15 +73,15 @@
                     funcname = stream.expect('func_name').value
                     args, kwargs = parse_arguments(stream, 'gettext_end')
 
                     strings = []
 
                     for arg, argtype in args:
                         if argtype == 'func_string_arg':
-                            strings.append(force_text(arg))
+                            strings.append(force_str(arg))
                         else:
                             strings.append(None)
 
                     for arg in kwargs:
                         strings.append(None)
 
                     if len(strings) == 1:
```

### Comparing `enmerkar-underscore-2.1.0/src/enmerkar_underscore.egg-info/SOURCES.txt` & `enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
+requirements/constraints.txt
 src/enmerkar_underscore/__init__.py
 src/enmerkar_underscore.egg-info/PKG-INFO
 src/enmerkar_underscore.egg-info/SOURCES.txt
 src/enmerkar_underscore.egg-info/dependency_links.txt
 src/enmerkar_underscore.egg-info/entry_points.txt
 src/enmerkar_underscore.egg-info/not-zip-safe
 src/enmerkar_underscore.egg-info/requires.txt
```

### Comparing `enmerkar-underscore-2.1.0/tests/__init__.py` & `enmerkar-underscore-2.2.0/tests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from babel._compat import BytesIO
+from io import BytesIO
 
 from enmerkar_underscore import extract
 
 class TestMixedExtract:
 
     @pytest.fixture(autouse=True)
     def setup(self):
```

### Comparing `enmerkar-underscore-2.1.0/tests/test_extract.py` & `enmerkar-underscore-2.2.0/tests/test_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from babel._compat import BytesIO
+from io import BytesIO
 from babel.messages.extract import DEFAULT_KEYWORDS
 
 from enmerkar_underscore import extract
 
 
 class TestMixedExtract:
```

