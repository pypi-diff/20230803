# Comparing `tmp/hugg-0.1.2.tar.gz` & `tmp/hugg-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.1.2.tar", last modified: Thu Aug  3 16:05:01 2023, max compression
+gzip compressed data, was "hugg-0.1.3.tar", last modified: Thu Aug  3 16:14:02 2023, max compression
```

## Comparing `hugg-0.1.2.tar` & `hugg-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:05:01.261810 hugg-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 16:04:46.000000 hugg-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 16:05:01.257810 hugg-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 16:04:46.000000 hugg-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:05:01.257810 hugg-0.1.2/hugg/
--rw-r--r--   0 runner    (1001) docker     (123)    42918 2023-08-03 16:04:46.000000 hugg-0.1.2/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:05:01.257810 hugg-0.1.2/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 16:05:01.000000 hugg-0.1.2/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-03 16:05:01.000000 hugg-0.1.2/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:05:01.000000 hugg-0.1.2/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 16:05:01.000000 hugg-0.1.2/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 16:05:01.000000 hugg-0.1.2/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:05:01.261810 hugg-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3699 2023-08-03 16:04:46.000000 hugg-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:14:02.064520 hugg-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 16:13:50.000000 hugg-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 16:14:02.064520 hugg-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 16:13:50.000000 hugg-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:14:02.060520 hugg-0.1.3/hugg/
+-rw-r--r--   0 runner    (1001) docker     (123)    42903 2023-08-03 16:13:50.000000 hugg-0.1.3/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:14:02.064520 hugg-0.1.3/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 16:14:02.000000 hugg-0.1.3/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-03 16:14:02.000000 hugg-0.1.3/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:14:02.000000 hugg-0.1.3/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 16:14:02.000000 hugg-0.1.3/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 16:14:02.000000 hugg-0.1.3/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:14:02.064520 hugg-0.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3699 2023-08-03 16:13:50.000000 hugg-0.1.3/setup.py
```

### Comparing `hugg-0.1.2/LICENSE` & `hugg-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.1.2/hugg/__init__.py` & `hugg-0.1.3/hugg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
                 self.delete_file(foil)
         """
         print(']')
 
 class localdrive(mem):
     #https://python-gitlab.readthedocs.io/en/stable/index.html#installation
     #https://python-gitlab.readthedocs.io/en/stable/api-usage.html
-    def __init__(self,path:str=os.curdir, file_location,wraplambda=lambda foil:False):
+    def __init__(self,path:str=os.curdir,wraplambda=lambda foil:False):
         super().__init__(wraplambda)
         self.path = path
 
     def files(self):
         return [os.path.join(dp, f) for dp, dn, filenames in os.walk(self.path) for f in filenames if os.path.isfile(f)]
 
     def login(self):
```

### Comparing `hugg-0.1.2/setup.py` & `hugg-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

