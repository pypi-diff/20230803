# Comparing `tmp/gautodoc-0.0.0.tar.gz` & `tmp/gautodoc-0.0.1.tar.gz`

## Comparing `gautodoc-0.0.0.tar` & `gautodoc-0.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 gautodoc-0.0.0/flake.lock
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 gautodoc-0.0.0/flake.nix
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gautodoc-0.0.0/gautodoc/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 gautodoc-0.0.0/gautodoc/__main__.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 gautodoc-0.0.0/gautodoc/build.py
--rwxr-xr-x   0        0        0     1910 2020-02-02 00:00:00.000000 gautodoc-0.0.0/gautodoc/cli.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 gautodoc-0.0.0/gautodoc/common.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 gautodoc-0.0.0/gautodoc/config.py
--rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 gautodoc-0.0.0/gautodoc/registry.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 gautodoc-0.0.0/gautodoc/template/index.html
--rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 gautodoc-0.0.0/gautodoc/template/modules/gautodoc.mjs
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 gautodoc-0.0.0/gautodoc/template/styles/gautodoc.css
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 gautodoc-0.0.0/gautodoc/template/styles/index.css
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 gautodoc-0.0.0/.gitignore
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 gautodoc-0.0.0/LICENSE.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 gautodoc-0.0.0/README.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 gautodoc-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 gautodoc-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 gautodoc-0.0.1/flake.lock
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 gautodoc-0.0.1/flake.nix
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gautodoc-0.0.1/gautodoc/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 gautodoc-0.0.1/gautodoc/__main__.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 gautodoc-0.0.1/gautodoc/build.py
+-rwxr-xr-x   0        0        0     1910 2020-02-02 00:00:00.000000 gautodoc-0.0.1/gautodoc/cli.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 gautodoc-0.0.1/gautodoc/common.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 gautodoc-0.0.1/gautodoc/config.py
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 gautodoc-0.0.1/gautodoc/registry.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 gautodoc-0.0.1/gautodoc/template/index.html
+-rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 gautodoc-0.0.1/gautodoc/template/modules/gautodoc.mjs
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 gautodoc-0.0.1/gautodoc/template/styles/gautodoc.css
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 gautodoc-0.0.1/gautodoc/template/styles/index.css
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 gautodoc-0.0.1/.gitignore
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 gautodoc-0.0.1/LICENSE.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 gautodoc-0.0.1/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 gautodoc-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 gautodoc-0.0.1/PKG-INFO
```

### Comparing `gautodoc-0.0.0/flake.lock` & `gautodoc-0.0.1/flake.lock`

 * *Files identical despite different names*

### Comparing `gautodoc-0.0.0/flake.nix` & `gautodoc-0.0.1/flake.nix`

 * *Files identical despite different names*

### Comparing `gautodoc-0.0.0/gautodoc/build.py` & `gautodoc-0.0.1/gautodoc/build.py`

 * *Files identical despite different names*

### Comparing `gautodoc-0.0.0/gautodoc/cli.py` & `gautodoc-0.0.1/gautodoc/cli.py`

 * *Files identical despite different names*

### Comparing `gautodoc-0.0.0/gautodoc/config.py` & `gautodoc-0.0.1/gautodoc/config.py`

 * *Files identical despite different names*

### Comparing `gautodoc-0.0.0/gautodoc/registry.py` & `gautodoc-0.0.1/gautodoc/registry.py`

 * *Files identical despite different names*

### Comparing `gautodoc-0.0.0/gautodoc/template/index.html` & `gautodoc-0.0.1/gautodoc/template/index.html`

 * *Files identical despite different names*

### Comparing `gautodoc-0.0.0/gautodoc/template/modules/gautodoc.mjs` & `gautodoc-0.0.1/gautodoc/template/modules/gautodoc.mjs`

 * *Files identical despite different names*

### Comparing `gautodoc-0.0.0/gautodoc/template/styles/gautodoc.css` & `gautodoc-0.0.1/gautodoc/template/styles/gautodoc.css`

 * *Files identical despite different names*

### Comparing `gautodoc-0.0.0/LICENSE.md` & `gautodoc-0.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gautodoc-0.0.0/README.md` & `gautodoc-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gautodoc-0.0.0/pyproject.toml` & `gautodoc-0.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gautodoc"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
     { name = "Garrison Hinson-Hasty", email = "garrisonhh+dev@pm.me" },
 ]
 description = "stupid simple autodoc"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: Free To Use But Restricted",
     "Operating System :: POSIX :: Linux",
     "Topic :: Documentation",
 ]
 
 [project.entry_points.console_scripts]
```

### Comparing `gautodoc-0.0.0/PKG-INFO` & `gautodoc-0.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: gautodoc
-Version: 0.0.0
+Version: 0.0.1
 Summary: stupid simple autodoc
 Project-URL: Homepage, https://github.com/garrisonhh/gautodoc
 Project-URL: Bug Tracker, https://github.com/garrisonhh/gautodoc/issues
 Author-email: Garrison Hinson-Hasty <garrisonhh+dev@pm.me>
 License-File: LICENSE.md
 Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # gautodoc
 
 stupid simple autodoc.
 
 ## how do I use your stupid tool?
```

