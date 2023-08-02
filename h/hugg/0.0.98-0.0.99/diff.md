# Comparing `tmp/hugg-0.0.98.tar.gz` & `tmp/hugg-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.0.98.tar", last modified: Wed Aug  2 21:41:09 2023, max compression
+gzip compressed data, was "hugg-0.0.99.tar", last modified: Wed Aug  2 22:01:32 2023, max compression
```

## Comparing `hugg-0.0.98.tar` & `hugg-0.0.99.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:09.854180 hugg-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 21:40:56.000000 hugg-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 21:41:09.854180 hugg-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 21:40:56.000000 hugg-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:09.854180 hugg-0.0.98/hugg/
--rw-r--r--   0 runner    (1001) docker     (123)    39643 2023-08-02 21:40:56.000000 hugg-0.0.98/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:09.854180 hugg-0.0.98/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 21:41:09.000000 hugg-0.0.98/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 21:41:09.000000 hugg-0.0.98/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:41:09.000000 hugg-0.0.98/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 21:41:09.000000 hugg-0.0.98/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 21:41:09.000000 hugg-0.0.98/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:41:09.854180 hugg-0.0.98/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3560 2023-08-02 21:40:56.000000 hugg-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:01:32.195318 hugg-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 22:01:21.000000 hugg-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 22:01:32.195318 hugg-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 22:01:21.000000 hugg-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:01:32.195318 hugg-0.0.99/hugg/
+-rw-r--r--   0 runner    (1001) docker     (123)    39593 2023-08-02 22:01:21.000000 hugg-0.0.99/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:01:32.195318 hugg-0.0.99/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 22:01:32.000000 hugg-0.0.99/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 22:01:32.000000 hugg-0.0.99/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:01:32.000000 hugg-0.0.99/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 22:01:32.000000 hugg-0.0.99/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 22:01:32.000000 hugg-0.0.99/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 22:01:32.195318 hugg-0.0.99/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3560 2023-08-02 22:01:21.000000 hugg-0.0.99/setup.py
```

### Comparing `hugg-0.0.98/LICENSE` & `hugg-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.0.98/hugg/__init__.py` & `hugg-0.0.99/hugg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,24 +67,24 @@
         if not hasattr(self,'dowraplambda'):
             setattr(self,'dowraplambda',lambda foil:False)
         return getattr(self,'dowraplambda')
 
     def setWrapLambda(self, lambd):
         setattr(self,'dowraplambda',lambd)
 
-    def download(self, file_path=None,download_to=None, wrap:bool=False):
+    def download(self, file_path=None,download_to=None):
         self.__internal_download(file_path, download_to)
 
-        if wrap or self.checkWrapLambda()(download_to):
+        if self.checkWrapLambda()(download_to):
             download_to = self.unwrap(download_to)
         
         return download_to
 
-    def upload(self, path=None,path_in_repo=None, wrap:bool=False):
-        if wrap or self.checkWrapLambda()(path):
+    def upload(self, path=None,path_in_repo=None):
+        if self.checkWrapLambda()(path):
             path = self.wrap(path)
             path_in_repo += ".nosj"
 
         return self.__internal_upload(path, path_in_repo)
 
     def __enter__(self):
         self.login()
```

### Comparing `hugg-0.0.98/setup.py` & `hugg-0.0.99/setup.py`

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
-VERSION = "0.0.98"
+VERSION = "0.0.99"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

