# Comparing `tmp/DependiPy-1.0.8.tar.gz` & `tmp/DependiPy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DependiPy-1.0.8.tar", last modified: Thu Jul 20 16:58:05 2023, max compression
+gzip compressed data, was "DependiPy-1.0.9.tar", last modified: Wed Aug  2 12:33:48 2023, max compression
```

## Comparing `DependiPy-1.0.8.tar` & `DependiPy-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:58:05.044111 DependiPy-1.0.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:58:05.040111 DependiPy-1.0.8/DependiPy/
--rw-r--r--   0 root         (0) root         (0)       68 2023-07-20 16:58:04.000000 DependiPy-1.0.8/DependiPy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21373 2023-07-20 16:58:04.000000 DependiPy-1.0.8/DependiPy/archive.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-07-20 16:58:04.000000 DependiPy-1.0.8/DependiPy/librarian.py
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-20 16:58:04.000000 DependiPy-1.0.8/DependiPy/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:58:05.040111 DependiPy-1.0.8/DependiPy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11507 2023-07-20 16:58:04.000000 DependiPy-1.0.8/DependiPy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      313 2023-07-20 16:58:05.000000 DependiPy-1.0.8/DependiPy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:58:05.000000 DependiPy-1.0.8/DependiPy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-20 16:58:05.000000 DependiPy-1.0.8/DependiPy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-20 16:58:05.000000 DependiPy-1.0.8/DependiPy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-20 16:58:05.000000 DependiPy-1.0.8/DependiPy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-20 16:58:04.000000 DependiPy-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11507 2023-07-20 16:58:05.044111 DependiPy-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11287 2023-07-20 16:58:04.000000 DependiPy-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 16:58:05.044111 DependiPy-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      921 2023-07-20 16:58:04.000000 DependiPy-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:33:48.134312 DependiPy-1.0.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:33:48.130312 DependiPy-1.0.9/DependiPy/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-08-02 12:33:47.000000 DependiPy-1.0.9/DependiPy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21373 2023-08-02 12:33:47.000000 DependiPy-1.0.9/DependiPy/archive.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-08-02 12:33:47.000000 DependiPy-1.0.9/DependiPy/librarian.py
+-rw-r--r--   0 root         (0) root         (0)       17 2023-08-02 12:33:47.000000 DependiPy-1.0.9/DependiPy/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:33:48.134312 DependiPy-1.0.9/DependiPy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11507 2023-08-02 12:33:48.000000 DependiPy-1.0.9/DependiPy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      313 2023-08-02 12:33:48.000000 DependiPy-1.0.9/DependiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 12:33:48.000000 DependiPy-1.0.9/DependiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-08-02 12:33:48.000000 DependiPy-1.0.9/DependiPy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-08-02 12:33:48.000000 DependiPy-1.0.9/DependiPy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-02 12:33:48.000000 DependiPy-1.0.9/DependiPy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-08-02 12:33:47.000000 DependiPy-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11507 2023-08-02 12:33:48.134312 DependiPy-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11287 2023-08-02 12:33:47.000000 DependiPy-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 12:33:48.134312 DependiPy-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      921 2023-08-02 12:33:47.000000 DependiPy-1.0.9/setup.py
```

### Comparing `DependiPy-1.0.8/DependiPy/archive.py` & `DependiPy-1.0.9/DependiPy/archive.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
             with open("mkdocs.yml", "w") as f:
                 for s in contents_yml:
                     f.write(str(s) + "\n")
 
         ###############################
         if 'docs_only' in kwargs and kwargs.get('docs_only') == False or 'docs_only' not in kwargs:
 
-            if self.mode == 'scirpt':
+            if self.mode == 'script':
                 list_privat_reference = ['[' for _ in range(len(self.librerie_private))]
 
                 for ele in single_requirements:
                     if ele != 'waste':
                         for i, lib in enumerate(self.librerie_private):
                             if ele.split('.')[0] == lib:
                                 list_privat_reference[i] += (ele + ',')
```

### Comparing `DependiPy-1.0.8/DependiPy/librarian.py` & `DependiPy-1.0.9/DependiPy/librarian.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     parser = argparse.ArgumentParser(prog='library-mapper', description="Map the requirements of a project")
     parser.add_argument('-p', '--path',
                         help="folder/file path, if mode lib it needs the path to the folder deeper than setup.py",
                         required=True)
     parser.add_argument('-m', '--mode', help="lib parser or script parser (lib,script)", required=False)
     parser.add_argument('-c', '--config', help="config file", required=False, default='config.json')
-    parser.add_argument('-do', '--docs_only', help="generate only the documentatino", required=False, default=False)
+    parser.add_argument('-do', '--docs_only', help="generate only the documentation", required=False, default=False)
 
     kwargs = vars(parser.parse_args())
 
     try:
         with open(kwargs['config']) as json_file:
             config = json.load(json_file)
     except:
```

### Comparing `DependiPy-1.0.8/DependiPy.egg-info/PKG-INFO` & `DependiPy-1.0.9/DependiPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DependiPy
-Version: 1.0.8
+Version: 1.0.9
 Home-page: https://github.com/ajacassi/DependiPy.git
 Author: Andrea Jacassi
 Author-email: 
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `DependiPy-1.0.8/LICENSE` & `DependiPy-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `DependiPy-1.0.8/PKG-INFO` & `DependiPy-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DependiPy
-Version: 1.0.8
+Version: 1.0.9
 Home-page: https://github.com/ajacassi/DependiPy.git
 Author: Andrea Jacassi
 Author-email: 
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `DependiPy-1.0.8/README.md` & `DependiPy-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `DependiPy-1.0.8/setup.py` & `DependiPy-1.0.9/setup.py`

 * *Files identical despite different names*

