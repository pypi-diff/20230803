# Comparing `tmp/toxinpred3-1.1.tar.gz` & `tmp/toxinpred3-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toxinpred3-1.1.tar", last modified: Thu Aug  3 14:40:05 2023, max compression
+gzip compressed data, was "toxinpred3-1.2.tar", last modified: Thu Aug  3 14:48:56 2023, max compression
```

## Comparing `toxinpred3-1.1.tar` & `toxinpred3-1.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 anandr     (501) staff       (20)        0 2023-08-03 14:40:05.666523 toxinpred3-1.1/
--rw-r--r--   0 anandr     (501) staff       (20)    35149 2023-07-29 06:06:02.000000 toxinpred3-1.1/LICENSE.txt
--rw-r--r--   0 anandr     (501) staff       (20)     3229 2023-08-03 14:40:05.666402 toxinpred3-1.1/PKG-INFO
--rw-r--r--   0 anandr     (501) staff       (20)     2979 2023-08-03 14:35:53.000000 toxinpred3-1.1/README.md
--rw-r--r--   0 anandr     (501) staff       (20)       38 2023-08-03 14:40:05.666563 toxinpred3-1.1/setup.cfg
--rw-r--r--   0 anandr     (501) staff       (20)     1012 2023-08-03 14:39:46.000000 toxinpred3-1.1/setup.py
-drwxr-xr-x   0 anandr     (501) staff       (20)        0 2023-08-03 14:40:05.542474 toxinpred3-1.1/src/
-drwxr-xr-x   0 anandr     (501) staff       (20)        0 2023-08-03 14:40:05.542568 toxinpred3-1.1/src/toxinpred3/
-drwxr-xr-x   0 anandr     (501) staff       (20)        0 2023-08-03 14:40:05.543939 toxinpred3-1.1/src/toxinpred3/model/
--rw-r--r--   0 anandr     (501) staff       (20) 52672827 2023-05-18 06:36:08.000000 toxinpred3-1.1/src/toxinpred3/model/toxinpred3.0_model.pkl
-drwxr-xr-x   0 anandr     (501) staff       (20)        0 2023-08-03 14:40:05.664500 toxinpred3-1.1/src/toxinpred3/python_scripts/
--rw-r--r--   0 anandr     (501) staff       (20)        0 2023-07-19 11:42:32.000000 toxinpred3-1.1/src/toxinpred3/python_scripts/__init__.py
--rw-r--r--   0 anandr     (501) staff       (20)    14745 2023-08-03 14:28:28.000000 toxinpred3-1.1/src/toxinpred3/python_scripts/toxinpred3.py
-drwxr-xr-x   0 anandr     (501) staff       (20)        0 2023-08-03 14:40:05.543683 toxinpred3-1.1/src/toxinpred3.egg-info/
--rw-r--r--   0 anandr     (501) staff       (20)     3229 2023-08-03 14:40:05.000000 toxinpred3-1.1/src/toxinpred3.egg-info/PKG-INFO
--rw-r--r--   0 anandr     (501) staff       (20)      390 2023-08-03 14:40:05.000000 toxinpred3-1.1/src/toxinpred3.egg-info/SOURCES.txt
--rw-r--r--   0 anandr     (501) staff       (20)        1 2023-08-03 14:40:05.000000 toxinpred3-1.1/src/toxinpred3.egg-info/dependency_links.txt
--rw-r--r--   0 anandr     (501) staff       (20)       73 2023-08-03 14:40:05.000000 toxinpred3-1.1/src/toxinpred3.egg-info/entry_points.txt
--rw-r--r--   0 anandr     (501) staff       (20)       22 2023-08-03 14:40:05.000000 toxinpred3-1.1/src/toxinpred3.egg-info/requires.txt
--rw-r--r--   0 anandr     (501) staff       (20)       11 2023-08-03 14:40:05.000000 toxinpred3-1.1/src/toxinpred3.egg-info/top_level.txt
+drwxr-xr-x   0 anandr     (501) staff       (20)        0 2023-08-03 14:48:56.256777 toxinpred3-1.2/
+-rw-r--r--   0 anandr     (501) staff       (20)    35149 2023-07-29 06:06:02.000000 toxinpred3-1.2/LICENSE.txt
+-rw-r--r--   0 anandr     (501) staff       (20)     3229 2023-08-03 14:48:56.256656 toxinpred3-1.2/PKG-INFO
+-rw-r--r--   0 anandr     (501) staff       (20)     2979 2023-08-03 14:35:53.000000 toxinpred3-1.2/README.md
+-rw-r--r--   0 anandr     (501) staff       (20)       38 2023-08-03 14:48:56.256822 toxinpred3-1.2/setup.cfg
+-rw-r--r--   0 anandr     (501) staff       (20)     1005 2023-08-03 14:48:10.000000 toxinpred3-1.2/setup.py
+drwxr-xr-x   0 anandr     (501) staff       (20)        0 2023-08-03 14:48:56.170268 toxinpred3-1.2/src/
+drwxr-xr-x   0 anandr     (501) staff       (20)        0 2023-08-03 14:48:56.170434 toxinpred3-1.2/src/toxinpred3/
+drwxr-xr-x   0 anandr     (501) staff       (20)        0 2023-08-03 14:48:56.171474 toxinpred3-1.2/src/toxinpred3/merci/
+-rwxr-xr-x   0 anandr     (501) staff       (20)    12749 2023-07-18 12:12:33.000000 toxinpred3-1.2/src/toxinpred3/merci/MERCI_motif_locator.pl
+drwxr-xr-x   0 anandr     (501) staff       (20)        0 2023-08-03 14:48:56.172611 toxinpred3-1.2/src/toxinpred3/model/
+-rw-r--r--   0 anandr     (501) staff       (20) 52672827 2023-05-18 06:36:08.000000 toxinpred3-1.2/src/toxinpred3/model/toxinpred3.0_model.pkl
+drwxr-xr-x   0 anandr     (501) staff       (20)        0 2023-08-03 14:48:56.255541 toxinpred3-1.2/src/toxinpred3/python_scripts/
+-rw-r--r--   0 anandr     (501) staff       (20)        0 2023-07-19 11:42:32.000000 toxinpred3-1.2/src/toxinpred3/python_scripts/__init__.py
+-rw-r--r--   0 anandr     (501) staff       (20)    14745 2023-08-03 14:48:32.000000 toxinpred3-1.2/src/toxinpred3/python_scripts/toxinpred3.py
+drwxr-xr-x   0 anandr     (501) staff       (20)        0 2023-08-03 14:48:56.171374 toxinpred3-1.2/src/toxinpred3.egg-info/
+-rw-r--r--   0 anandr     (501) staff       (20)     3229 2023-08-03 14:48:56.000000 toxinpred3-1.2/src/toxinpred3.egg-info/PKG-INFO
+-rw-r--r--   0 anandr     (501) staff       (20)      434 2023-08-03 14:48:56.000000 toxinpred3-1.2/src/toxinpred3.egg-info/SOURCES.txt
+-rw-r--r--   0 anandr     (501) staff       (20)        1 2023-08-03 14:48:56.000000 toxinpred3-1.2/src/toxinpred3.egg-info/dependency_links.txt
+-rw-r--r--   0 anandr     (501) staff       (20)       73 2023-08-03 14:48:56.000000 toxinpred3-1.2/src/toxinpred3.egg-info/entry_points.txt
+-rw-r--r--   0 anandr     (501) staff       (20)       22 2023-08-03 14:48:56.000000 toxinpred3-1.2/src/toxinpred3.egg-info/requires.txt
+-rw-r--r--   0 anandr     (501) staff       (20)       11 2023-08-03 14:48:56.000000 toxinpred3-1.2/src/toxinpred3.egg-info/top_level.txt
```

### Comparing `toxinpred3-1.1/LICENSE.txt` & `toxinpred3-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `toxinpred3-1.1/PKG-INFO` & `toxinpred3-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toxinpred3
-Version: 1.1
+Version: 1.2
 Summary: A tool to predict toxic and non-toxic peptides
 Home-page: https://github.com/raghavagps/toxinpred3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Toxinpred3.0
```

### Comparing `toxinpred3-1.1/README.md` & `toxinpred3-1.2/README.md`

 * *Files identical despite different names*

### Comparing `toxinpred3-1.1/setup.py` & `toxinpred3-1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='toxinpred3',
-    version='1.1',
+    version='1.2',
     description='A tool to predict toxic and non-toxic peptides',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license_files = ('LICENSE.txt',),
     url='https://github.com/raghavagps/toxinpred3', 
     packages=find_namespace_packages(where="src"),
     package_dir={'':'src'},
     package_data={ 'toxinpred3.model':['*'],
     'toxinpred3.motif':['*'],
-    'toxinpred3.perl_scripts':['*']},
+    'toxinpred3.merci':['*']},
     entry_points={ 'console_scripts' : ['toxinpred3 = toxinpred3.python_scripts.toxinpred3:main']},
     include_package_data=True,
     python_requires='>=3.6',
     install_requires=[
         'numpy', 'pandas' , 'argparse' # Add any Python dependencies here
     ]
 )
```

### Comparing `toxinpred3-1.1/src/toxinpred3/model/toxinpred3.0_model.pkl` & `toxinpred3-1.2/src/toxinpred3/model/toxinpred3.0_model.pkl`

 * *Files identical despite different names*

### Comparing `toxinpred3-1.1/src/toxinpred3/python_scripts/toxinpred3.py` & `toxinpred3-1.2/src/toxinpred3/python_scripts/toxinpred3.py`

 * *Files identical despite different names*

### Comparing `toxinpred3-1.1/src/toxinpred3.egg-info/PKG-INFO` & `toxinpred3-1.2/src/toxinpred3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toxinpred3
-Version: 1.1
+Version: 1.2
 Summary: A tool to predict toxic and non-toxic peptides
 Home-page: https://github.com/raghavagps/toxinpred3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Toxinpred3.0
```

