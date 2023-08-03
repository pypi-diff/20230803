# Comparing `tmp/pyclean-2.7.3.tar.gz` & `tmp/pyclean-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclean-2.7.3.tar", last modified: Sun May 21 21:02:45 2023, max compression
+gzip compressed data, was "pyclean-2.7.4.tar", last modified: Thu Aug  3 11:44:38 2023, max compression
```

## Comparing `pyclean-2.7.3.tar` & `pyclean-2.7.4.tar`

### file list

```diff
@@ -1,30 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:02:45.665949 pyclean-2.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 21:02:31.000000 pyclean-2.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-21 21:02:31.000000 pyclean-2.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-05-21 21:02:45.665949 pyclean-2.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-21 21:02:31.000000 pyclean-2.7.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:02:45.665949 pyclean-2.7.3/pyclean/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/modern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/py2clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/py3clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyclean/pypyclean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:02:45.665949 pyclean-2.7.3/pyclean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-05-21 21:02:45.000000 pyclean-2.7.3/pyclean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-21 21:02:45.000000 pyclean-2.7.3/pyclean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:02:45.000000 pyclean-2.7.3/pyclean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-21 21:02:45.000000 pyclean-2.7.3/pyclean.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 21:02:45.000000 pyclean-2.7.3/pyclean.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-21 21:02:31.000000 pyclean-2.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 21:02:45.665949 pyclean-2.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-21 21:02:31.000000 pyclean-2.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:02:45.665949 pyclean-2.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-21 21:02:31.000000 pyclean-2.7.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-21 21:02:31.000000 pyclean-2.7.3/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-21 21:02:31.000000 pyclean-2.7.3/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-05-21 21:02:31.000000 pyclean-2.7.3/tests/test_modern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-21 21:02:31.000000 pyclean-2.7.3/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-21 21:02:31.000000 pyclean-2.7.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:38.404256 pyclean-2.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 11:44:05.000000 pyclean-2.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    49715 2023-08-03 11:44:38.404256 pyclean-2.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-08-03 11:44:05.000000 pyclean-2.7.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:38.400256 pyclean-2.7.4/pyclean/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-03 11:44:05.000000 pyclean-2.7.4/pyclean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-03 11:44:05.000000 pyclean-2.7.4/pyclean/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-08-03 11:44:05.000000 pyclean-2.7.4/pyclean/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-03 11:44:05.000000 pyclean-2.7.4/pyclean/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-08-03 11:44:05.000000 pyclean-2.7.4/pyclean/modern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-08-03 11:44:05.000000 pyclean-2.7.4/pyclean/py2clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-08-03 11:44:05.000000 pyclean-2.7.4/pyclean/py3clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-03 11:44:05.000000 pyclean-2.7.4/pyclean/pypyclean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:38.404256 pyclean-2.7.4/pyclean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49715 2023-08-03 11:44:38.000000 pyclean-2.7.4/pyclean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-03 11:44:38.000000 pyclean-2.7.4/pyclean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:44:38.000000 pyclean-2.7.4/pyclean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-03 11:44:38.000000 pyclean-2.7.4/pyclean.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 11:44:38.000000 pyclean-2.7.4/pyclean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-08-03 11:44:05.000000 pyclean-2.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:44:38.404256 pyclean-2.7.4/setup.cfg
```

### Comparing `pyclean-2.7.3/LICENSE` & `pyclean-2.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.3/PKG-INFO` & `pyclean-2.7.4/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: pyclean
-Version: 2.7.3
-Summary: Pure Python cross-platform pyclean. Clean up your Python bytecode.
-Home-page: https://github.com/bittner/pyclean
-Author: Peter Bittner
-Author-email: django@bittner.it
-License: GPL-3.0-or-later
-Keywords: python,bytecode,cli,tools
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Utilities
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 pyclean |latest-version|
 ========================
 
 |checks-status| |tests-status| |publish-status| |scrutinizer| |codacy| |python-versions| |python-impl| |license|
 
 Worried about ``.pyc`` files and ``__pycache__`` directories? Fear not!
 PyClean is here to help. Finally the single-command clean up for Python
@@ -217,15 +188,15 @@
 
 You'll then be able to run it with `Tox`_ like this:
 
 .. code:: console
 
     $ tox -e clean
 
-.. _Tox: https://tox.readthedocs.io/
+.. _Tox: https://tox.wiki/
 
 Development
 ===========
 
 If you want to help out please see our `contribution guide`_.
 
 .. _contribution guide: https://github.com/bittner/pyclean/blob/main/CONTRIBUTING.md
```

### Comparing `pyclean-2.7.3/pyclean/cli.py` & `pyclean-2.7.4/pyclean/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,17 +102,22 @@
 def main(override=None):
     """
     Entry point for all scripts
     """
     args = parse_arguments()
     if override or args.legacy:
         impl = compat.get_implementation(override=override)
-        impl.main(args)
+        pyclean_main = impl.main
     else:
-        modern.pyclean(args)
+        pyclean_main = modern.pyclean
+
+    try:
+        pyclean_main(args)
+    except Exception as err:
+        raise SystemExit(err)
 
 
 def py2clean():
     """
     Forces the use of the implementation for Python 2
     """
     main('CPython2')
```

### Comparing `pyclean-2.7.3/pyclean/compat.py` & `pyclean-2.7.4/pyclean/compat.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         CPython3='pyclean.py3clean',
         PyPy2='pyclean.pypyclean',
         PyPy3='pyclean.pypyclean',
     )
 
     detected_version = '%s%s' % (
         platform.python_implementation(),
-        sys.version[0],
+        sys.version_info.major,
     )
 
     module_name = implementation[override if override else detected_version]
     return import_module(module_name)
 
 
 class ExtendAction(AppendAction):
```

### Comparing `pyclean-2.7.3/pyclean/modern.py` & `pyclean-2.7.4/pyclean/modern.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,8 +228,9 @@
 
 def confirm(message):
     """An interactive confirmation prompt."""
     try:
         answer = input("%s? " % message)
         return answer.strip().lower() in ['y', 'yes']
     except KeyboardInterrupt:
-        raise SystemExit('Aborted by user.')
+        msg = 'Aborted by user.'
+        raise SystemExit(msg)
```

### Comparing `pyclean-2.7.3/pyclean/py2clean.py` & `pyclean-2.7.4/pyclean/py2clean.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.3/pyclean/py3clean.py` & `pyclean-2.7.4/pyclean/py3clean.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.3/pyclean/pypyclean.py` & `pyclean-2.7.4/pyclean/pypyclean.py`

 * *Files identical despite different names*

