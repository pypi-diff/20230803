# Comparing `tmp/magic_decorator-0.0.7.tar.gz` & `tmp/magic_decorator-0.0.8.tar.gz`

## Comparing `magic_decorator-0.0.7.tar` & `magic_decorator-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 magic_decorator-0.0.7/magic_decorator.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 magic_decorator-0.0.7/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 magic_decorator-0.0.7/LICENSE
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 magic_decorator-0.0.7/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 magic_decorator-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 magic_decorator-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 magic_decorator-0.0.8/magic_decorator.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 magic_decorator-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 magic_decorator-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 magic_decorator-0.0.8/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 magic_decorator-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 magic_decorator-0.0.8/PKG-INFO
```

### Comparing `magic_decorator-0.0.7/.gitignore` & `magic_decorator-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.7/LICENSE` & `magic_decorator-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.7/README.md` & `magic_decorator-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.7/pyproject.toml` & `magic_decorator-0.0.8/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "magic-decorator"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     {name="Kim Minjong", email="make.dirty.code@gmail.com"},
 ]
 description = "A magic function decorator using OpenAI ChatCompletion"
 readme = "README.md"
 requires-python = ">=3.7.1"
-dependencies = ["openai>0.27", "sick-json"]
+dependencies = ["openai>0.27", "sick-json", "langchain"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `magic_decorator-0.0.7/PKG-INFO` & `magic_decorator-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: magic-decorator
-Version: 0.0.7
+Version: 0.0.8
 Summary: A magic function decorator using OpenAI ChatCompletion
 Author-email: Kim Minjong <make.dirty.code@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.1
+Requires-Dist: langchain
 Requires-Dist: openai>0.27
 Requires-Dist: sick-json
 Description-Content-Type: text/markdown
 
 # Simple demo function using OpenAI's ChatComplete
 
 The only function implemented in this module is magic.
```

