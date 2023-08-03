# Comparing `tmp/hugg-0.1.3.tar.gz` & `tmp/hugg-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.1.3.tar", last modified: Thu Aug  3 16:14:02 2023, max compression
+gzip compressed data, was "hugg-0.1.4.tar", last modified: Thu Aug  3 17:02:49 2023, max compression
```

## Comparing `hugg-0.1.3.tar` & `hugg-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:14:02.064520 hugg-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 16:13:50.000000 hugg-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 16:14:02.064520 hugg-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 16:13:50.000000 hugg-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:14:02.060520 hugg-0.1.3/hugg/
--rw-r--r--   0 runner    (1001) docker     (123)    42903 2023-08-03 16:13:50.000000 hugg-0.1.3/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:14:02.064520 hugg-0.1.3/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 16:14:02.000000 hugg-0.1.3/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-03 16:14:02.000000 hugg-0.1.3/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:14:02.000000 hugg-0.1.3/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 16:14:02.000000 hugg-0.1.3/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 16:14:02.000000 hugg-0.1.3/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:14:02.064520 hugg-0.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3699 2023-08-03 16:13:50.000000 hugg-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:49.312854 hugg-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 17:02:36.000000 hugg-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 17:02:49.312854 hugg-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 17:02:36.000000 hugg-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:49.308854 hugg-0.1.4/hugg/
+-rw-r--r--   0 runner    (1001) docker     (123)    42911 2023-08-03 17:02:36.000000 hugg-0.1.4/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:49.308854 hugg-0.1.4/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 17:02:49.000000 hugg-0.1.4/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-03 17:02:49.000000 hugg-0.1.4/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:02:49.000000 hugg-0.1.4/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 17:02:49.000000 hugg-0.1.4/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 17:02:49.000000 hugg-0.1.4/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:02:49.312854 hugg-0.1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3699 2023-08-03 17:02:36.000000 hugg-0.1.4/setup.py
```

### Comparing `hugg-0.1.3/LICENSE` & `hugg-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.1.3/hugg/__init__.py` & `hugg-0.1.4/hugg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         for file in files:
             ext = pathlib.Path(file).suffix
             if ext not in output:
                 output[ext] = 0
             output[ext] += 1
         return output
     def wrap(self,foil):
-        if foil != None:
+        if foil == None:
             return foil
 
         import json
         with open(foil,"r") as reader:
             content = reader.readlines()
 
         info = {
@@ -143,15 +143,15 @@
         with open(foil, "w+") as writer:
             writer.write(json.dumps(info))
 
         return foil
 
     def unwrap(self,foil):
         #Checking if there is a custom wrapping around the file, and unwrapping
-        if foil and foil.endswith(".nosj"):
+        if foil != None and foil.endswith(".nosj"):
             import json
             with open(foil, 'r') as reader:
                 content = json.load(reader)
 
             os.remove(foil)
             foil = foil.replace('.nosj','')
```

### Comparing `hugg-0.1.3/setup.py` & `hugg-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

