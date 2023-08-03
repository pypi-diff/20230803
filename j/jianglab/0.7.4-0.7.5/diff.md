# Comparing `tmp/jianglab-0.7.4.tar.gz` & `tmp/jianglab-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.7.4.tar", last modified: Thu Aug  3 15:10:33 2023, max compression
+gzip compressed data, was "jianglab-0.7.5.tar", last modified: Thu Aug  3 15:16:24 2023, max compression
```

## Comparing `jianglab-0.7.4.tar` & `jianglab-0.7.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-03 15:10:33.706579 jianglab-0.7.4/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-03 15:10:33.706189 jianglab-0.7.4/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.7.4/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-03 15:10:33.702057 jianglab-0.7.4/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.7.4/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    49302 2023-08-03 15:09:59.000000 jianglab-0.7.4/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.7.4/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-03 15:10:33.705545 jianglab-0.7.4/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-03 15:10:33.000000 jianglab-0.7.4/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-03 15:10:33.000000 jianglab-0.7.4/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-03 15:10:33.000000 jianglab-0.7.4/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      173 2023-08-03 15:10:33.000000 jianglab-0.7.4/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-03 15:10:33.000000 jianglab-0.7.4/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-03 15:10:33.706718 jianglab-0.7.4/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1177 2023-08-03 15:10:08.000000 jianglab-0.7.4/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-03 15:16:24.528164 jianglab-0.7.5/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-03 15:16:24.527811 jianglab-0.7.5/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.7.5/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-03 15:16:24.524032 jianglab-0.7.5/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.7.5/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    49302 2023-08-03 15:09:59.000000 jianglab-0.7.5/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.7.5/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-03 15:16:24.527053 jianglab-0.7.5/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-03 15:16:24.000000 jianglab-0.7.5/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-03 15:16:24.000000 jianglab-0.7.5/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-03 15:16:24.000000 jianglab-0.7.5/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      168 2023-08-03 15:16:24.000000 jianglab-0.7.5/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-03 15:16:24.000000 jianglab-0.7.5/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-03 15:16:24.528298 jianglab-0.7.5/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1162 2023-08-03 15:16:15.000000 jianglab-0.7.5/setup.py
```

### Comparing `jianglab-0.7.4/PKG-INFO` & `jianglab-0.7.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.7.4
+Version: 0.7.5
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.7.4/README.md` & `jianglab-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.7.4/jianglab/common_functions.py` & `jianglab-0.7.5/jianglab/common_functions.py`

 * *Files identical despite different names*

### Comparing `jianglab-0.7.4/jianglab.egg-info/PKG-INFO` & `jianglab-0.7.5/jianglab.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.7.4
+Version: 0.7.5
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.7.4/setup.py` & `jianglab-0.7.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.7.4',
+    version='0.7.5',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
@@ -19,15 +19,14 @@
         "ipython",
         "seaborn",
         "optuna",
         "xgboost",
         "scikit-learn",
         "umap-learn",
         "missingno",
-        "glob"
 
     ],
     author = "Jiang Zheng",
     author_email = "zjiang314@gmail.com",
     description = "A package for Jiang lab",
     url = "https://github.com/jiang-lab-retina/jianglab.git",
     classifiers=[
```

