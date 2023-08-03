# Comparing `tmp/sinetstream-kafka-1.8.0.tar.gz` & `tmp/sinetstream-kafka-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinetstream-kafka-1.8.0.tar", last modified: Tue May 16 06:38:50 2023, max compression
+gzip compressed data, was "sinetstream-kafka-1.8.1.tar", last modified: Thu Aug  3 07:51:30 2023, max compression
```

## Comparing `sinetstream-kafka-1.8.0.tar` & `sinetstream-kafka-1.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:38:50.110501 sinetstream-kafka-1.8.0/
--rw-rw-r--   0 koie      (1004) koie      (1004)      554 2023-05-16 06:38:50.110501 sinetstream-kafka-1.8.0/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)     1682 2023-05-16 06:38:50.114501 sinetstream-kafka-1.8.0/setup.cfg
--rw-rw-r--   0 koie      (1004) koie      (1004)       39 2023-01-12 00:12:25.000000 sinetstream-kafka-1.8.0/setup.py
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:38:50.102501 sinetstream-kafka-1.8.0/src/
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:38:50.102501 sinetstream-kafka-1.8.0/src/sinetstream_kafka.egg-info/
--rw-rw-r--   0 koie      (1004) koie      (1004)      554 2023-05-16 06:38:49.000000 sinetstream-kafka-1.8.0/src/sinetstream_kafka.egg-info/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)      419 2023-05-16 06:38:50.000000 sinetstream-kafka-1.8.0/src/sinetstream_kafka.egg-info/SOURCES.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-05-16 06:38:49.000000 sinetstream-kafka-1.8.0/src/sinetstream_kafka.egg-info/dependency_links.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)      285 2023-05-16 06:38:49.000000 sinetstream-kafka-1.8.0/src/sinetstream_kafka.egg-info/entry_points.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-05-16 06:38:49.000000 sinetstream-kafka-1.8.0/src/sinetstream_kafka.egg-info/namespace_packages.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-01-12 00:15:55.000000 sinetstream-kafka-1.8.0/src/sinetstream_kafka.egg-info/not-zip-safe
--rw-rw-r--   0 koie      (1004) koie      (1004)       45 2023-05-16 06:38:49.000000 sinetstream-kafka-1.8.0/src/sinetstream_kafka.egg-info/requires.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-05-16 06:38:49.000000 sinetstream-kafka-1.8.0/src/sinetstream_kafka.egg-info/top_level.txt
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:38:50.102501 sinetstream-kafka-1.8.0/src/sinetstreamplugin/
--rw-rw-r--   0 koie      (1004) koie      (1004)    11871 2023-01-12 00:12:25.000000 sinetstream-kafka-1.8.0/src/sinetstreamplugin/kafka.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:30.085119 sinetstream-kafka-1.8.1/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      554 2023-08-03 07:51:30.085119 sinetstream-kafka-1.8.1/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1682 2023-08-03 07:51:30.085119 sinetstream-kafka-1.8.1/setup.cfg
+-rw-rw-r--   0 koie      (1004) koie      (1004)       39 2023-08-02 07:22:54.000000 sinetstream-kafka-1.8.1/setup.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:30.081119 sinetstream-kafka-1.8.1/src/
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:30.085119 sinetstream-kafka-1.8.1/src/sinetstream_kafka.egg-info/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      554 2023-08-03 07:51:29.000000 sinetstream-kafka-1.8.1/src/sinetstream_kafka.egg-info/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)      419 2023-08-03 07:51:30.000000 sinetstream-kafka-1.8.1/src/sinetstream_kafka.egg-info/SOURCES.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-08-03 07:51:29.000000 sinetstream-kafka-1.8.1/src/sinetstream_kafka.egg-info/dependency_links.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)      285 2023-08-03 07:51:29.000000 sinetstream-kafka-1.8.1/src/sinetstream_kafka.egg-info/entry_points.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-08-03 07:51:29.000000 sinetstream-kafka-1.8.1/src/sinetstream_kafka.egg-info/namespace_packages.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-08-03 07:51:29.000000 sinetstream-kafka-1.8.1/src/sinetstream_kafka.egg-info/not-zip-safe
+-rw-rw-r--   0 koie      (1004) koie      (1004)       45 2023-08-03 07:51:29.000000 sinetstream-kafka-1.8.1/src/sinetstream_kafka.egg-info/requires.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-08-03 07:51:29.000000 sinetstream-kafka-1.8.1/src/sinetstream_kafka.egg-info/top_level.txt
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-08-03 07:51:30.085119 sinetstream-kafka-1.8.1/src/sinetstreamplugin/
+-rw-rw-r--   0 koie      (1004) koie      (1004)    11871 2023-08-02 07:22:54.000000 sinetstream-kafka-1.8.1/src/sinetstreamplugin/kafka.py
```

### Comparing `sinetstream-kafka-1.8.0/PKG-INFO` & `sinetstream-kafka-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sinetstream-kafka
-Version: 1.8.0
+Version: 1.8.1
 Summary: Apache Kafka plugin for SINETStream library
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

### Comparing `sinetstream-kafka-1.8.0/setup.cfg` & `sinetstream-kafka-1.8.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sinetstream-kafka
-version = 1.8.0
+version = 1.8.1
 description = Apache Kafka plugin for SINETStream library
 license = Apache License, Version 2.0
 license_files = 
 	../../../../LICENSE
 url = https://github.com/nii-gakunin-cloud/sinetstream
 classifiers = 
 	Development Status :: 4 - Beta
@@ -16,29 +16,29 @@
 
 [options]
 package_dir = 
 	=src
 packages = find_namespace:
 zip_safe = False
 install_requires = 
-	sinetstream>=1.8.0
+	sinetstream>=1.8.1
 	kafka-python>=2.0
 	promise
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

### Comparing `sinetstream-kafka-1.8.0/src/sinetstream_kafka.egg-info/PKG-INFO` & `sinetstream-kafka-1.8.1/src/sinetstream_kafka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sinetstream-kafka
-Version: 1.8.0
+Version: 1.8.1
 Summary: Apache Kafka plugin for SINETStream library
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

### Comparing `sinetstream-kafka-1.8.0/src/sinetstreamplugin/kafka.py` & `sinetstream-kafka-1.8.1/src/sinetstreamplugin/kafka.py`

 * *Files identical despite different names*

