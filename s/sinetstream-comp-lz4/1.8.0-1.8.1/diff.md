# Comparing `tmp/sinetstream-comp-lz4-1.8.0.tar.gz` & `tmp/sinetstream-comp-lz4-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinetstream-comp-lz4-1.8.0.tar", last modified: Tue May 16 06:41:38 2023, max compression
+gzip compressed data, was "sinetstream-comp-lz4-1.8.1.tar", last modified: Thu Aug  3 07:51:51 2023, max compression
```

## Comparing `sinetstream-comp-lz4-1.8.0.tar` & `sinetstream-comp-lz4-1.8.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:41:38.522462 sinetstream-comp-lz4-1.8.0/
--rw-rw-r--   0 koie      (1004) koie      (1004)      560 2023-05-16 06:41:38.522462 sinetstream-comp-lz4-1.8.0/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)     1458 2023-05-16 06:41:38.526462 sinetstream-comp-lz4-1.8.0/setup.cfg
--rw-rw-r--   0 koie      (1004) koie      (1004)       39 2023-01-12 00:12:25.000000 sinetstream-comp-lz4-1.8.0/setup.py
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:41:38.510462 sinetstream-comp-lz4-1.8.0/src/
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:41:38.522462 sinetstream-comp-lz4-1.8.0/src/sinetstream_comp_lz4.egg-info/
--rw-rw-r--   0 koie      (1004) koie      (1004)      560 2023-05-16 06:41:38.000000 sinetstream-comp-lz4-1.8.0/src/sinetstream_comp_lz4.egg-info/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)      453 2023-05-16 06:41:38.000000 sinetstream-comp-lz4-1.8.0/src/sinetstream_comp_lz4.egg-info/SOURCES.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-05-16 06:41:38.000000 sinetstream-comp-lz4-1.8.0/src/sinetstream_comp_lz4.egg-info/dependency_links.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       81 2023-05-16 06:41:38.000000 sinetstream-comp-lz4-1.8.0/src/sinetstream_comp_lz4.egg-info/entry_points.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-05-16 06:41:38.000000 sinetstream-comp-lz4-1.8.0/src/sinetstream_comp_lz4.egg-info/namespace_packages.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-01-12 00:15:52.000000 sinetstream-comp-lz4-1.8.0/src/sinetstream_comp_lz4.egg-info/not-zip-safe
--rw-rw-r--   0 koie      (1004) koie      (1004)       23 2023-05-16 06:41:38.000000 sinetstream-comp-lz4-1.8.0/src/sinetstream_comp_lz4.egg-info/requires.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-05-16 06:41:38.000000 sinetstream-comp-lz4-1.8.0/src/sinetstream_comp_lz4.egg-info/top_level.txt
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:41:38.510462 sinetstream-comp-lz4-1.8.0/src/sinetstreamplugin/
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:41:38.522462 sinetstream-comp-lz4-1.8.0/src/sinetstreamplugin/compression/
--rw-rw-r--   0 koie      (1004) koie      (1004)     1517 2023-01-12 00:12:25.000000 sinetstream-comp-lz4-1.8.0/src/sinetstreamplugin/compression/lz4.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:51.977132 sinetstream-comp-lz4-1.8.1/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      560 2023-08-03 07:51:51.977132 sinetstream-comp-lz4-1.8.1/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1458 2023-08-03 07:51:51.977132 sinetstream-comp-lz4-1.8.1/setup.cfg
+-rw-rw-r--   0 koie      (1004) koie      (1004)       39 2023-08-02 07:22:54.000000 sinetstream-comp-lz4-1.8.1/setup.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:51.969132 sinetstream-comp-lz4-1.8.1/src/
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:51.973132 sinetstream-comp-lz4-1.8.1/src/sinetstream_comp_lz4.egg-info/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      560 2023-08-03 07:51:51.000000 sinetstream-comp-lz4-1.8.1/src/sinetstream_comp_lz4.egg-info/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)      453 2023-08-03 07:51:51.000000 sinetstream-comp-lz4-1.8.1/src/sinetstream_comp_lz4.egg-info/SOURCES.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-08-03 07:51:51.000000 sinetstream-comp-lz4-1.8.1/src/sinetstream_comp_lz4.egg-info/dependency_links.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       81 2023-08-03 07:51:51.000000 sinetstream-comp-lz4-1.8.1/src/sinetstream_comp_lz4.egg-info/entry_points.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-08-03 07:51:51.000000 sinetstream-comp-lz4-1.8.1/src/sinetstream_comp_lz4.egg-info/namespace_packages.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-08-03 07:51:51.000000 sinetstream-comp-lz4-1.8.1/src/sinetstream_comp_lz4.egg-info/not-zip-safe
+-rw-rw-r--   0 koie      (1004) koie      (1004)       23 2023-08-03 07:51:51.000000 sinetstream-comp-lz4-1.8.1/src/sinetstream_comp_lz4.egg-info/requires.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-08-03 07:51:51.000000 sinetstream-comp-lz4-1.8.1/src/sinetstream_comp_lz4.egg-info/top_level.txt
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:51.969132 sinetstream-comp-lz4-1.8.1/src/sinetstreamplugin/
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:51.977132 sinetstream-comp-lz4-1.8.1/src/sinetstreamplugin/compression/
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1517 2023-08-02 07:22:54.000000 sinetstream-comp-lz4-1.8.1/src/sinetstreamplugin/compression/lz4.py
```

### Comparing `sinetstream-comp-lz4-1.8.0/PKG-INFO` & `sinetstream-comp-lz4-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sinetstream-comp-lz4
-Version: 1.8.0
+Version: 1.8.1
 Summary: LZ4 compression plugin for SINETStream library
 Home-page: https://github.com/nii-gakunin-cloud/sinetstream
 License: Apache License, Version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
```

### Comparing `sinetstream-comp-lz4-1.8.0/setup.cfg` & `sinetstream-comp-lz4-1.8.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sinetstream-comp-lz4
-version = 1.8.0
+version = 1.8.1
 description = LZ4 compression plugin for SINETStream library
 license = Apache License, Version 2.0
 license_files = 
 	../../../../LICENSE
 url = https://github.com/nii-gakunin-cloud/sinetstream
 classifiers = 
 	Development Status :: 4 - Beta
@@ -16,28 +16,28 @@
 
 [options]
 package_dir = 
 	=src
 packages = find_namespace:
 zip_safe = False
 install_requires = 
-	sinetstream>=1.8.0
+	sinetstream>=1.8.1
 	lz4
 tests_require = 
 	pytest
 	pytest-cov
 	pytest-flake8
 	pytest-timeout
 	pytest-html==3.2.0
 	flake8>=4.0.0,<5.0.0  # workaround: https://github.com/tholo/pytest-flake8/issues/87
 setup_requires = 
 	pytest-runner
 namespace_packages = 
 	sinetstreamplugin
-python_requires = >= 3.7
+python_requires = >= 3.8
 
 [options.packages.find]
 where = src
 
 [aliases]
 test = pytest
```

### Comparing `sinetstream-comp-lz4-1.8.0/src/sinetstream_comp_lz4.egg-info/PKG-INFO` & `sinetstream-comp-lz4-1.8.1/src/sinetstream_comp_lz4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sinetstream-comp-lz4
-Version: 1.8.0
+Version: 1.8.1
 Summary: LZ4 compression plugin for SINETStream library
 Home-page: https://github.com/nii-gakunin-cloud/sinetstream
 License: Apache License, Version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
```

### Comparing `sinetstream-comp-lz4-1.8.0/src/sinetstreamplugin/compression/lz4.py` & `sinetstream-comp-lz4-1.8.1/src/sinetstreamplugin/compression/lz4.py`

 * *Files identical despite different names*

