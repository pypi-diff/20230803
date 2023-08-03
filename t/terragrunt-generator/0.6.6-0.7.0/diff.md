# Comparing `tmp/terragrunt-generator-0.6.6.tar.gz` & `tmp/terragrunt-generator-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terragrunt-generator-0.6.6.tar", last modified: Wed Aug  2 16:25:35 2023, max compression
+gzip compressed data, was "terragrunt-generator-0.7.0.tar", last modified: Wed Aug  2 20:14:19 2023, max compression
```

## Comparing `terragrunt-generator-0.6.6.tar` & `terragrunt-generator-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:25:35.964164 terragrunt-generator-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    21492 2023-08-02 16:25:35.960163 terragrunt-generator-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21241 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:25:35.960163 terragrunt-generator-0.6.6/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 16:25:23.000000 terragrunt-generator-0.6.6/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/generator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/generator/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/generator/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/generator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/generator/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/generator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-02 16:25:23.000000 terragrunt-generator-0.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:25:35.964164 terragrunt-generator-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:25:35.960163 terragrunt-generator-0.6.6/terragrunt_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21492 2023-08-02 16:25:35.000000 terragrunt-generator-0.6.6/terragrunt_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-02 16:25:35.000000 terragrunt-generator-0.6.6/terragrunt_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:25:35.000000 terragrunt-generator-0.6.6/terragrunt_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 16:25:35.000000 terragrunt-generator-0.6.6/terragrunt_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-02 16:25:35.000000 terragrunt-generator-0.6.6/terragrunt_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 16:25:35.000000 terragrunt-generator-0.6.6/terragrunt_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:25:35.960163 terragrunt-generator-0.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:14:19.823458 terragrunt-generator-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    21492 2023-08-02 20:14:19.823458 terragrunt-generator-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21241 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:14:19.819458 terragrunt-generator-0.7.0/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 20:14:06.000000 terragrunt-generator-0.7.0/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/generator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/generator/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/generator/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/generator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/generator/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/generator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-02 20:14:06.000000 terragrunt-generator-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:14:19.823458 terragrunt-generator-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:14:19.819458 terragrunt-generator-0.7.0/terragrunt_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21492 2023-08-02 20:14:19.000000 terragrunt-generator-0.7.0/terragrunt_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-02 20:14:19.000000 terragrunt-generator-0.7.0/terragrunt_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:14:19.000000 terragrunt-generator-0.7.0/terragrunt_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 20:14:19.000000 terragrunt-generator-0.7.0/terragrunt_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-02 20:14:19.000000 terragrunt-generator-0.7.0/terragrunt_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 20:14:19.000000 terragrunt-generator-0.7.0/terragrunt_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:14:19.823458 terragrunt-generator-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 20:13:52.000000 terragrunt-generator-0.7.0/tests/test_utils.py
```

### Comparing `terragrunt-generator-0.6.6/COPYING` & `terragrunt-generator-0.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.6/PKG-INFO` & `terragrunt-generator-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terragrunt-generator
-Version: 0.6.6
+Version: 0.7.0
 Summary: generate terragrunt manifest from terraform module.
 Author: Chris
 Author-email: goabonga@pm.me
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: COPYING
```

### Comparing `terragrunt-generator-0.6.6/README.md` & `terragrunt-generator-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.6/generator/generate.py` & `terragrunt-generator-0.7.0/generator/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 
 def generate_header(
     name: str,
     url: str,
     path: str,
     version: str,
     lookup: str,
-    variables: list = [],
+    variables: map = {
+        'mandatories': {},
+        'optionals': {},
+        'nullables': {},
+    },
 ) -> str:
     text = ''
 
     for var_type in ('mandatories', 'optionals', 'nullables'):
         for variable in variables.get(var_type, []):
             default = variable.get('default')
             description = (
@@ -180,14 +184,15 @@
             if v.get('mandatory') is True:
                 mandatories.append(v)
             if v.get('nullable') is True:
                 nullables.append(v)
             if v.get('mandatory') is False and v.get('nullable') is False:
                 optionals.append(v)
             outputs.append(v)
+
     return outputs, {
         'mandatories': mandatories,
         'optionals': optionals,
         'nullables': nullables,
     }
```

### Comparing `terragrunt-generator-0.6.6/generator/main.py` & `terragrunt-generator-0.7.0/generator/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,50 +5,48 @@
 
 from generator import __version__
 from generator.generate import generate
 from generator.git import clone
 from generator.reader import read_directory
 from generator.utils import is_local
 
+parser = argparse.ArgumentParser(
+    prog='terragrunt-gernerator',
+    description='generate terragrunt.hcl confirugation' + ' from terraform module',
+)
+
+parser.add_argument(
+    '-V',
+    action='version',
+    version=f'%(prog)s {__version__}',
+)
+
+parser.add_argument('-u', '--url', required=True, help='the module repository url')
+
+parser.add_argument('-v', '--version', help='the module version to use', default='main')
+
+parser.add_argument('-p', '--path', help='define the module path if needed')
+
+parser.add_argument(
+    '--include',
+    help='do no rendering the include block',
+    action=argparse.BooleanOptionalAction,
+    default=True,
+)
+
+parser.add_argument(
+    '-l',
+    '--lookup',
+    help='define the lookup path'
+    # , default='["{name}"]'
+)
 
-def main():
-    parser = argparse.ArgumentParser(
-        prog='terragrunt-gernerator',
-        description='generate terragrunt.hcl confirugation' + ' from terraform module',
-    )
-
-    parser.add_argument(
-        '-V',
-        action='version',
-        version=f'%(prog)s {__version__}',
-    )
-
-    parser.add_argument('-u', '--url', required=True, help='the module repository url')
-
-    parser.add_argument(
-        '-v', '--version', help='the module version to use', default='main'
-    )
-
-    parser.add_argument('-p', '--path', help='define the module path if needed')
-
-    parser.add_argument(
-        '--include',
-        help='do no rendering the include block',
-        action=argparse.BooleanOptionalAction,
-        default=True,
-    )
-
-    parser.add_argument(
-        '-l',
-        '--lookup',
-        help='define the lookup path'
-        # , default='["{name}"]'
-    )
 
-    args = parser.parse_args()
+def main(args=None):
+    args = parser.parse_args(args)
 
     tempdir = f'{gettempdir()}/{uuid4()}'
 
     if is_local(args.url):
         copy_tree(args.url, tempdir)
     else:
         clone(args.url, tempdir, args.version)
```

### Comparing `terragrunt-generator-0.6.6/pyproject.toml` & `terragrunt-generator-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,13 +19,13 @@
   | build
   | dist
 )/
 '''
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.6"
+version = "0.7.0"
 tag_format = "$major.$minor.$patch$prerelease"
 version_files = [
     "pyproject.toml:version",
     "generator/__init__.py",
 ]
```

### Comparing `terragrunt-generator-0.6.6/setup.py` & `terragrunt-generator-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.6/terragrunt_generator.egg-info/PKG-INFO` & `terragrunt-generator-0.7.0/terragrunt_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terragrunt-generator
-Version: 0.6.6
+Version: 0.7.0
 Summary: generate terragrunt manifest from terraform module.
 Author: Chris
 Author-email: goabonga@pm.me
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: COPYING
```

### Comparing `terragrunt-generator-0.6.6/terragrunt_generator.egg-info/SOURCES.txt` & `terragrunt-generator-0.7.0/terragrunt_generator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 terragrunt_generator.egg-info/PKG-INFO
 terragrunt_generator.egg-info/SOURCES.txt
 terragrunt_generator.egg-info/dependency_links.txt
 terragrunt_generator.egg-info/entry_points.txt
 terragrunt_generator.egg-info/requires.txt
 terragrunt_generator.egg-info/top_level.txt
 tests/__init__.py
+tests/test_cli.py
 tests/test_generate.py
 tests/test_git.py
 tests/test_reader.py
 tests/test_utils.py
```

