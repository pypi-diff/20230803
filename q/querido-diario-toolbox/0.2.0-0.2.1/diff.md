# Comparing `tmp/querido-diario-toolbox-0.2.0.tar.gz` & `tmp/querido-diario-toolbox-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querido-diario-toolbox-0.2.0.tar", last modified: Tue Oct 12 17:14:25 2021, max compression
+gzip compressed data, was "querido-diario-toolbox-0.2.1.tar", last modified: Thu Aug  3 15:50:57 2023, max compression
```

## Comparing `querido-diario-toolbox-0.2.0.tar` & `querido-diario-toolbox-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 gcc       (1000) users      (985)        0 2021-10-12 17:14:25.789919 querido-diario-toolbox-0.2.0/
--rw-r--r--   0 gcc       (1000) users      (985)     1109 2021-06-20 20:48:01.000000 querido-diario-toolbox-0.2.0/LICENSE
--rw-r--r--   0 gcc       (1000) users      (985)       26 2021-10-12 15:26:51.000000 querido-diario-toolbox-0.2.0/MANIFEST.in
--rw-r--r--   0 gcc       (1000) users      (985)     4951 2021-10-12 17:14:25.789919 querido-diario-toolbox-0.2.0/PKG-INFO
--rw-r--r--   0 gcc       (1000) users      (985)     3473 2021-10-12 17:09:57.000000 querido-diario-toolbox-0.2.0/README.md
-drwxr-xr-x   0 gcc       (1000) users      (985)        0 2021-10-12 17:14:25.789919 querido-diario-toolbox-0.2.0/querido_diario_toolbox/
--rw-r--r--   0 gcc       (1000) users      (985)       68 2021-10-12 15:05:21.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox/__init__.py
--rw-r--r--   0 gcc       (1000) users      (985)       63 2021-10-12 17:14:00.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox/__version__.py
-drwxr-xr-x   0 gcc       (1000) users      (985)        0 2021-10-12 17:14:25.789919 querido-diario-toolbox-0.2.0/querido_diario_toolbox/etl/
--rw-r--r--   0 gcc       (1000) users      (985)        0 2021-06-20 20:48:01.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox/etl/__init__.py
--rw-r--r--   0 gcc       (1000) users      (985)     3464 2021-10-12 15:35:02.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox/etl/apache_tika_text_extractor.py
--rw-r--r--   0 gcc       (1000) users      (985)     6408 2021-10-12 15:05:21.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox/etl/file_transform.py
--rw-r--r--   0 gcc       (1000) users      (985)      367 2021-10-12 15:34:44.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox/etl/text_extractor.py
--rw-r--r--   0 gcc       (1000) users      (985)      911 2021-10-12 15:05:21.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox/etl/text_extractor_interface.py
--rw-r--r--   0 gcc       (1000) users      (985)     2351 2021-10-12 15:05:21.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox/gazette.py
--rw-r--r--   0 gcc       (1000) users      (985)     1549 2021-10-12 15:05:21.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox/page.py
-drwxr-xr-x   0 gcc       (1000) users      (985)        0 2021-10-12 17:14:25.789919 querido-diario-toolbox-0.2.0/querido_diario_toolbox/process/
--rw-r--r--   0 gcc       (1000) users      (985)        0 2021-06-20 20:48:01.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox/process/__init__.py
--rw-r--r--   0 gcc       (1000) users      (985)     2291 2021-10-12 15:05:21.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox/process/edition_process.py
--rw-r--r--   0 gcc       (1000) users      (985)     1740 2021-10-12 15:05:21.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox/process/text_process.py
-drwxr-xr-x   0 gcc       (1000) users      (985)        0 2021-10-12 17:14:25.789919 querido-diario-toolbox-0.2.0/querido_diario_toolbox.egg-info/
--rw-r--r--   0 gcc       (1000) users      (985)     4951 2021-10-12 17:14:25.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 gcc       (1000) users      (985)      786 2021-10-12 17:14:25.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 gcc       (1000) users      (985)        1 2021-10-12 17:14:25.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 gcc       (1000) users      (985)       13 2021-10-12 17:14:25.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox.egg-info/requires.txt
--rw-r--r--   0 gcc       (1000) users      (985)       23 2021-10-12 17:14:25.000000 querido-diario-toolbox-0.2.0/querido_diario_toolbox.egg-info/top_level.txt
--rw-r--r--   0 gcc       (1000) users      (985)       38 2021-10-12 17:14:25.789919 querido-diario-toolbox-0.2.0/setup.cfg
--rw-r--r--   0 gcc       (1000) users      (985)     2867 2021-10-12 17:09:58.000000 querido-diario-toolbox-0.2.0/setup.py
+drwxr-xr-x   0 gcc       (1000) gcc       (1000)        0 2023-08-03 15:50:57.113598 querido-diario-toolbox-0.2.1/
+-rw-r--r--   0 gcc       (1000) gcc       (1000)     1109 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/LICENSE.md
+-rw-r--r--   0 gcc       (1000) gcc       (1000)       31 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/MANIFEST.in
+-rw-r--r--   0 gcc       (1000) gcc       (1000)    10850 2023-08-03 15:50:57.113598 querido-diario-toolbox-0.2.1/PKG-INFO
+drwxr-xr-x   0 gcc       (1000) gcc       (1000)        0 2023-08-03 15:50:57.106931 querido-diario-toolbox-0.2.1/docs/
+-rw-r--r--   0 gcc       (1000) gcc       (1000)     9084 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/docs/README.md
+drwxr-xr-x   0 gcc       (1000) gcc       (1000)        0 2023-08-03 15:50:57.106931 querido-diario-toolbox-0.2.1/querido_diario_toolbox/
+-rw-r--r--   0 gcc       (1000) gcc       (1000)       68 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox/__init__.py
+-rw-r--r--   0 gcc       (1000) gcc       (1000)       63 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox/__version__.py
+drwxr-xr-x   0 gcc       (1000) gcc       (1000)        0 2023-08-03 15:50:57.110264 querido-diario-toolbox-0.2.1/querido_diario_toolbox/etl/
+-rw-r--r--   0 gcc       (1000) gcc       (1000)        0 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox/etl/__init__.py
+-rw-r--r--   0 gcc       (1000) gcc       (1000)     3464 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox/etl/apache_tika_text_extractor.py
+-rw-r--r--   0 gcc       (1000) gcc       (1000)     6408 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox/etl/file_transform.py
+-rw-r--r--   0 gcc       (1000) gcc       (1000)      367 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox/etl/text_extractor.py
+-rw-r--r--   0 gcc       (1000) gcc       (1000)      911 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox/etl/text_extractor_interface.py
+-rw-r--r--   0 gcc       (1000) gcc       (1000)     2351 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox/gazette.py
+-rw-r--r--   0 gcc       (1000) gcc       (1000)     1549 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox/page.py
+drwxr-xr-x   0 gcc       (1000) gcc       (1000)        0 2023-08-03 15:50:57.110264 querido-diario-toolbox-0.2.1/querido_diario_toolbox/process/
+-rw-r--r--   0 gcc       (1000) gcc       (1000)        0 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox/process/__init__.py
+-rw-r--r--   0 gcc       (1000) gcc       (1000)     2291 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox/process/edition_process.py
+-rw-r--r--   0 gcc       (1000) gcc       (1000)     1740 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox/process/text_process.py
+drwxr-xr-x   0 gcc       (1000) gcc       (1000)        0 2023-08-03 15:50:57.110264 querido-diario-toolbox-0.2.1/querido_diario_toolbox.egg-info/
+-rw-r--r--   0 gcc       (1000) gcc       (1000)    10850 2023-08-03 15:50:56.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 gcc       (1000) gcc       (1000)      794 2023-08-03 15:50:56.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 gcc       (1000) gcc       (1000)        1 2023-08-03 15:50:56.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 gcc       (1000) gcc       (1000)       13 2023-08-03 15:50:56.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox.egg-info/requires.txt
+-rw-r--r--   0 gcc       (1000) gcc       (1000)       23 2023-08-03 15:50:56.000000 querido-diario-toolbox-0.2.1/querido_diario_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 gcc       (1000) gcc       (1000)       38 2023-08-03 15:50:57.113598 querido-diario-toolbox-0.2.1/setup.cfg
+-rw-r--r--   0 gcc       (1000) gcc       (1000)     2904 2023-08-03 15:40:45.000000 querido-diario-toolbox-0.2.1/setup.py
```

### Comparing `querido-diario-toolbox-0.2.0/LICENSE` & `querido-diario-toolbox-0.2.1/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Open Knowledge Brasil - Rede pelo Conhecimento Livre
+Copyright (c) 2021 Open Knowledge Brasil - Rede pelo Conhecimento Livre
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `querido-diario-toolbox-0.2.0/querido_diario_toolbox/etl/apache_tika_text_extractor.py` & `querido-diario-toolbox-0.2.1/querido_diario_toolbox/etl/apache_tika_text_extractor.py`

 * *Files identical despite different names*

### Comparing `querido-diario-toolbox-0.2.0/querido_diario_toolbox/etl/file_transform.py` & `querido-diario-toolbox-0.2.1/querido_diario_toolbox/etl/file_transform.py`

 * *Files identical despite different names*

### Comparing `querido-diario-toolbox-0.2.0/querido_diario_toolbox/etl/text_extractor_interface.py` & `querido-diario-toolbox-0.2.1/querido_diario_toolbox/etl/text_extractor_interface.py`

 * *Files identical despite different names*

### Comparing `querido-diario-toolbox-0.2.0/querido_diario_toolbox/gazette.py` & `querido-diario-toolbox-0.2.1/querido_diario_toolbox/gazette.py`

 * *Files identical despite different names*

### Comparing `querido-diario-toolbox-0.2.0/querido_diario_toolbox/page.py` & `querido-diario-toolbox-0.2.1/querido_diario_toolbox/page.py`

 * *Files identical despite different names*

### Comparing `querido-diario-toolbox-0.2.0/querido_diario_toolbox/process/edition_process.py` & `querido-diario-toolbox-0.2.1/querido_diario_toolbox/process/edition_process.py`

 * *Files identical despite different names*

### Comparing `querido-diario-toolbox-0.2.0/querido_diario_toolbox/process/text_process.py` & `querido-diario-toolbox-0.2.1/querido_diario_toolbox/process/text_process.py`

 * *Files identical despite different names*

### Comparing `querido-diario-toolbox-0.2.0/querido_diario_toolbox.egg-info/SOURCES.txt` & `querido-diario-toolbox-0.2.1/querido_diario_toolbox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-LICENSE
+LICENSE.md
 MANIFEST.in
-README.md
 setup.py
+docs/README.md
 querido_diario_toolbox/__init__.py
 querido_diario_toolbox/__version__.py
 querido_diario_toolbox/gazette.py
 querido_diario_toolbox/page.py
 querido_diario_toolbox.egg-info/PKG-INFO
 querido_diario_toolbox.egg-info/SOURCES.txt
 querido_diario_toolbox.egg-info/dependency_links.txt
```

### Comparing `querido-diario-toolbox-0.2.0/setup.py` & `querido-diario-toolbox-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 
 # Pacotes obrigatórios
 REQUIRED = ["python-magic"]
 
 # Pacotes extras
 EXTRAS = {}
 
-here = os.path.abspath(os.path.dirname(__file__))
+PROJECT_ROOT = os.path.abspath(os.path.dirname(__file__))
 
 # README.md como descrição longa
 try:
-    with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
+    with io.open(os.path.join(PROJECT_ROOT, "docs/README.md"), encoding="utf-8") as f:
         long_description = "\n" + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 about = {}
 
 # Versão do pacote
 project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-with open(os.path.join(here, project_slug, "__version__.py")) as f:
+with open(os.path.join(PROJECT_ROOT, project_slug, "__version__.py")) as f:
     exec(f.read(), about)
 
 
 class UploadCommand(Command):
     """Apóia a publicação com o setup.py"""
 
     description = "Build and publish the package."
@@ -51,15 +51,15 @@
 
     def finalize_options(self):
         pass
 
     def run(self):
         try:
             self.status("Removing previous builds…")
-            rmtree(os.path.join(here, "dist"))
+            rmtree(os.path.join(PROJECT_ROOT, "dist"))
         except OSError:
             pass
 
         self.status("Building Source and Wheel (universal) distribution…")
         os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
 
         self.status("Uploading the package to PyPI via Twine…")
```

