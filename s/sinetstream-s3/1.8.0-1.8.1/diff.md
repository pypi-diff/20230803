# Comparing `tmp/sinetstream-s3-1.8.0.tar.gz` & `tmp/sinetstream-s3-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinetstream-s3-1.8.0.tar", last modified: Tue May 16 06:40:43 2023, max compression
+gzip compressed data, was "sinetstream-s3-1.8.1.tar", last modified: Thu Aug  3 07:51:41 2023, max compression
```

## Comparing `sinetstream-s3-1.8.0.tar` & `sinetstream-s3-1.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:43.230475 sinetstream-s3-1.8.0/
--rw-rw-r--   0 koie      (1004) koie      (1004)      541 2023-05-16 06:40:43.230475 sinetstream-s3-1.8.0/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)     1612 2023-05-16 06:40:43.230475 sinetstream-s3-1.8.0/setup.cfg
--rw-rw-r--   0 koie      (1004) koie      (1004)       39 2023-01-12 00:12:25.000000 sinetstream-s3-1.8.0/setup.py
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:43.222475 sinetstream-s3-1.8.0/src/
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:43.230475 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/
--rw-rw-r--   0 koie      (1004) koie      (1004)      541 2023-05-16 06:40:43.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)      392 2023-05-16 06:40:43.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/SOURCES.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-05-16 06:40:43.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/dependency_links.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)      249 2023-05-16 06:40:43.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/entry_points.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-05-16 06:40:43.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/namespace_packages.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-01-12 00:15:59.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/not-zip-safe
--rw-rw-r--   0 koie      (1004) koie      (1004)       25 2023-05-16 06:40:43.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/requires.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-05-16 06:40:43.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/top_level.txt
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:43.230475 sinetstream-s3-1.8.0/src/sinetstreamplugin/
--rw-rw-r--   0 koie      (1004) koie      (1004)    14948 2023-01-12 00:12:25.000000 sinetstream-s3-1.8.0/src/sinetstreamplugin/s3.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:41.601126 sinetstream-s3-1.8.1/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      541 2023-08-03 07:51:41.601126 sinetstream-s3-1.8.1/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1612 2023-08-03 07:51:41.601126 sinetstream-s3-1.8.1/setup.cfg
+-rw-rw-r--   0 koie      (1004) koie      (1004)       39 2023-08-02 07:22:54.000000 sinetstream-s3-1.8.1/setup.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:41.597126 sinetstream-s3-1.8.1/src/
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:41.597126 sinetstream-s3-1.8.1/src/sinetstream_s3.egg-info/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      541 2023-08-03 07:51:41.000000 sinetstream-s3-1.8.1/src/sinetstream_s3.egg-info/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)      392 2023-08-03 07:51:41.000000 sinetstream-s3-1.8.1/src/sinetstream_s3.egg-info/SOURCES.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-08-03 07:51:41.000000 sinetstream-s3-1.8.1/src/sinetstream_s3.egg-info/dependency_links.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)      249 2023-08-03 07:51:41.000000 sinetstream-s3-1.8.1/src/sinetstream_s3.egg-info/entry_points.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-08-03 07:51:41.000000 sinetstream-s3-1.8.1/src/sinetstream_s3.egg-info/namespace_packages.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-08-03 07:51:41.000000 sinetstream-s3-1.8.1/src/sinetstream_s3.egg-info/not-zip-safe
+-rw-rw-r--   0 koie      (1004) koie      (1004)       25 2023-08-03 07:51:41.000000 sinetstream-s3-1.8.1/src/sinetstream_s3.egg-info/requires.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-08-03 07:51:41.000000 sinetstream-s3-1.8.1/src/sinetstream_s3.egg-info/top_level.txt
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:41.601126 sinetstream-s3-1.8.1/src/sinetstreamplugin/
+-rw-rw-r--   0 koie      (1004) koie      (1004)    14948 2023-08-02 07:22:54.000000 sinetstream-s3-1.8.1/src/sinetstreamplugin/s3.py
```

### Comparing `sinetstream-s3-1.8.0/PKG-INFO` & `sinetstream-s3-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sinetstream-s3
-Version: 1.8.0
+Version: 1.8.1
 Summary: S3 plugin for SINETStream library
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

### Comparing `sinetstream-s3-1.8.0/setup.cfg` & `sinetstream-s3-1.8.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sinetstream-s3
-version = 1.8.0
+version = 1.8.1
 description = S3 plugin for SINETStream library
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
 	boto3
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

### Comparing `sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/PKG-INFO` & `sinetstream-s3-1.8.1/src/sinetstream_s3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sinetstream-s3
-Version: 1.8.0
+Version: 1.8.1
 Summary: S3 plugin for SINETStream library
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

### Comparing `sinetstream-s3-1.8.0/src/sinetstreamplugin/s3.py` & `sinetstream-s3-1.8.1/src/sinetstreamplugin/s3.py`

 * *Files identical despite different names*

