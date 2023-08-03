# Comparing `tmp/easyecs-0.4.2.tar.gz` & `tmp/easyecs-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyecs-0.4.2.tar", max compression
+gzip compressed data, was "easyecs-0.4.3.tar", max compression
```

## Comparing `easyecs-0.4.2.tar` & `easyecs-0.4.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2230 2023-08-03 11:41:46.647240 easyecs-0.4.2/README.md
--rw-r--r--   0        0        0        0 2023-08-03 11:41:46.671240 easyecs-0.4.2/easyecs/__init__.py
--rwxr-xr-x   0        0        0     8332 2023-08-03 11:41:46.671240 easyecs-0.4.2/easyecs/cli.py
--rw-r--r--   0        0        0        0 2023-08-03 11:41:46.671240 easyecs-0.4.2/easyecs/cloudformation/__init__.py
--rw-r--r--   0        0        0       90 2023-08-03 11:41:46.671240 easyecs-0.4.2/easyecs/cloudformation/client.py
--rw-r--r--   0        0        0     3522 2023-08-03 11:41:46.671240 easyecs-0.4.2/easyecs/cloudformation/fetch.py
--rw-r--r--   0        0        0        0 2023-08-03 11:41:46.671240 easyecs-0.4.2/easyecs/cloudformation/stack/__init__.py
--rw-r--r--   0        0        0     1921 2023-08-03 11:41:46.671240 easyecs-0.4.2/easyecs/cloudformation/stack/create.py
--rw-r--r--   0        0        0     1131 2023-08-03 11:41:46.671240 easyecs-0.4.2/easyecs/cloudformation/stack/delete.py
--rw-r--r--   0        0        0     3274 2023-08-03 11:41:46.671240 easyecs-0.4.2/easyecs/cloudformation/stack/update.py
--rw-r--r--   0        0        0     8573 2023-08-03 11:41:46.671240 easyecs-0.4.2/easyecs/cloudformation/template/__init__.py
--rw-r--r--   0        0        0    12418 2023-08-03 11:41:46.671240 easyecs-0.4.2/easyecs/command/__init__.py
--rw-r--r--   0        0        0     1356 2023-08-03 11:41:46.671240 easyecs-0.4.2/easyecs/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 11:41:46.675240 easyecs-0.4.2/easyecs/helpers/__init__.py
--rw-r--r--   0        0        0      264 2023-08-03 11:41:46.675240 easyecs-0.4.2/easyecs/helpers/color.py
--rw-r--r--   0        0        0     2292 2023-08-03 11:41:46.675240 easyecs-0.4.2/easyecs/helpers/common.py
--rw-r--r--   0        0        0     1895 2023-08-03 11:41:46.675240 easyecs-0.4.2/easyecs/helpers/loader.py
--rw-r--r--   0        0        0      531 2023-08-03 11:41:46.675240 easyecs-0.4.2/easyecs/helpers/selector.py
--rw-r--r--   0        0        0     3272 2023-08-03 11:41:46.675240 easyecs-0.4.2/easyecs/helpers/settings.py
--rw-r--r--   0        0        0       42 2023-08-03 11:41:46.675240 easyecs-0.4.2/easyecs/helpers/signal.py
--rw-r--r--   0        0        0     2804 2023-08-03 11:41:46.675240 easyecs-0.4.2/easyecs/model/ecs.py
--rw-r--r--   0        0        0      607 2023-08-03 11:41:46.675240 easyecs-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     2230 2023-08-03 11:55:08.399009 easyecs-0.4.3/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/__init__.py
+-rwxr-xr-x   0        0        0     8332 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cli.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/__init__.py
+-rw-r--r--   0        0        0       90 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/client.py
+-rw-r--r--   0        0        0     3522 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/fetch.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/stack/__init__.py
+-rw-r--r--   0        0        0     1921 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/stack/create.py
+-rw-r--r--   0        0        0     1131 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/stack/delete.py
+-rw-r--r--   0        0        0     3274 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/stack/update.py
+-rw-r--r--   0        0        0     8573 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/cloudformation/template/__init__.py
+-rw-r--r--   0        0        0    12418 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/command/__init__.py
+-rw-r--r--   0        0        0     1386 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/helpers/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/helpers/color.py
+-rw-r--r--   0        0        0     2292 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/helpers/common.py
+-rw-r--r--   0        0        0     1895 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/helpers/loader.py
+-rw-r--r--   0        0        0      531 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/helpers/selector.py
+-rw-r--r--   0        0        0     3272 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/helpers/settings.py
+-rw-r--r--   0        0        0       42 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/helpers/signal.py
+-rw-r--r--   0        0        0     2804 2023-08-03 11:55:08.423010 easyecs-0.4.3/easyecs/model/ecs.py
+-rw-r--r--   0        0        0      607 2023-08-03 11:55:08.423010 easyecs-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.4.3/PKG-INFO
```

### Comparing `easyecs-0.4.2/README.md` & `easyecs-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.2/easyecs/cli.py` & `easyecs-0.4.3/easyecs/cli.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.2/easyecs/cloudformation/fetch.py` & `easyecs-0.4.3/easyecs/cloudformation/fetch.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.2/easyecs/cloudformation/stack/create.py` & `easyecs-0.4.3/easyecs/cloudformation/stack/create.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.2/easyecs/cloudformation/stack/delete.py` & `easyecs-0.4.3/easyecs/cloudformation/stack/delete.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.2/easyecs/cloudformation/stack/update.py` & `easyecs-0.4.3/easyecs/cloudformation/stack/update.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.2/easyecs/cloudformation/template/__init__.py` & `easyecs-0.4.3/easyecs/cloudformation/template/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.2/easyecs/command/__init__.py` & `easyecs-0.4.3/easyecs/command/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.2/easyecs/docker/__init__.py` & `easyecs-0.4.3/easyecs/docker/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
             build_args_str = " ".join(
                 [f'--build-arg {key}="{value}"' for key, value in build_args.items()]
             )
             build_cmd = f"docker build -t {image_name} {dockerfile}"
             if target:
                 build_cmd += f" {target}"
             build_cmd += f" {build_args_str}"
+            build_cmd += " ."
             res = subprocess.Popen(
                 build_cmd,
                 shell=True,
             )
             res.wait()
             if res.poll() != 0:
                 raise Exception("There was an issue building the docker image")
```

### Comparing `easyecs-0.4.2/easyecs/helpers/common.py` & `easyecs-0.4.3/easyecs/helpers/common.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.2/easyecs/helpers/loader.py` & `easyecs-0.4.3/easyecs/helpers/loader.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.2/easyecs/helpers/selector.py` & `easyecs-0.4.3/easyecs/helpers/selector.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.2/easyecs/helpers/settings.py` & `easyecs-0.4.3/easyecs/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.2/easyecs/model/ecs.py` & `easyecs-0.4.3/easyecs/model/ecs.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.2/pyproject.toml` & `easyecs-0.4.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easyecs"
-version = "0.4.2"
+version = "0.4.3"
 description = ""
 authors = ["BONVARLET Benjamin <benjaminbonvarlet96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.6"
```

### Comparing `easyecs-0.4.2/PKG-INFO` & `easyecs-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyecs
-Version: 0.4.2
+Version: 0.4.3
 Summary: 
 Author: BONVARLET Benjamin
 Author-email: benjaminbonvarlet96@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

