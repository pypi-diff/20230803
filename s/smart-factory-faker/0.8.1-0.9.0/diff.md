# Comparing `tmp/smart_factory_faker-0.8.1.tar.gz` & `tmp/smart_factory_faker-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_factory_faker-0.8.1.tar", last modified: Wed Aug  2 06:38:05 2023, max compression
+gzip compressed data, was "smart_factory_faker-0.9.0.tar", last modified: Thu Aug  3 05:04:31 2023, max compression
```

## Comparing `smart_factory_faker-0.8.1.tar` & `smart_factory_faker-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 06:38:05.359368 smart_factory_faker-0.8.1/
--rw-rw-rw-   0        0        0     1091 2023-08-02 06:03:18.000000 smart_factory_faker-0.8.1/LICENSE
--rw-rw-rw-   0        0        0     1894 2023-08-02 06:38:05.359368 smart_factory_faker-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-02 06:38:05.360256 smart_factory_faker-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0      973 2023-08-02 06:38:01.000000 smart_factory_faker-0.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 06:38:05.357339 smart_factory_faker-0.8.1/smart_factory_faker.egg-info/
--rw-rw-rw-   0        0        0     1894 2023-08-02 06:38:05.000000 smart_factory_faker-0.8.1/smart_factory_faker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-08-02 06:38:05.000000 smart_factory_faker-0.8.1/smart_factory_faker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 06:38:05.000000 smart_factory_faker-0.8.1/smart_factory_faker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-08-02 06:38:05.000000 smart_factory_faker-0.8.1/smart_factory_faker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 06:38:05.000000 smart_factory_faker-0.8.1/smart_factory_faker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 05:04:31.428011 smart_factory_faker-0.9.0/
+-rw-rw-rw-   0        0        0     1091 2023-08-02 06:03:18.000000 smart_factory_faker-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0     2039 2023-08-03 05:04:31.426349 smart_factory_faker-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-03 05:04:31.428011 smart_factory_faker-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      973 2023-08-03 05:02:01.000000 smart_factory_faker-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 05:04:31.425554 smart_factory_faker-0.9.0/smart_factory_faker.egg-info/
+-rw-rw-rw-   0        0        0     2039 2023-08-03 05:04:31.000000 smart_factory_faker-0.9.0/smart_factory_faker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-08-03 05:04:31.000000 smart_factory_faker-0.9.0/smart_factory_faker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 05:04:31.000000 smart_factory_faker-0.9.0/smart_factory_faker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-08-03 05:04:31.000000 smart_factory_faker-0.9.0/smart_factory_faker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 05:04:31.000000 smart_factory_faker-0.9.0/smart_factory_faker.egg-info/top_level.txt
```

### Comparing `smart_factory_faker-0.8.1/LICENSE` & `smart_factory_faker-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_factory_faker-0.8.1/PKG-INFO` & `smart_factory_faker-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart_factory_faker
-Version: 0.8.1
+Version: 0.9.0
 Summary: Smart-Factory-Faker
 Home-page: https://github.com/HyoungSooo/smart-factory-faker
 Author: HyoungSooo
 Author-email: aaa57403@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -69,7 +69,11 @@
 * fixed bug
 
 ### V 0.7.3
 * Change the code to get the next node
 
 ### V 0.8.0
 * Can be separated by facility
+
+### V 0.9.0
+* refactoring code
+* can see facilities history(Facility performance record => DataFrame(columns = [@timestamp, expire, wait]))
```

### Comparing `smart_factory_faker-0.8.1/setup.py` & `smart_factory_faker-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="smart_factory_faker",  # Replace with your own username
-    version="0.8.1",
+    version="0.9.0",
     author="HyoungSooo",
     author_email="aaa57403@gmail.com",
     description="Smart-Factory-Faker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/HyoungSooo/smart-factory-faker",
     packages=setuptools.find_packages(),
```

### Comparing `smart_factory_faker-0.8.1/smart_factory_faker.egg-info/PKG-INFO` & `smart_factory_faker-0.9.0/smart_factory_faker.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-factory-faker
-Version: 0.8.1
+Version: 0.9.0
 Summary: Smart-Factory-Faker
 Home-page: https://github.com/HyoungSooo/smart-factory-faker
 Author: HyoungSooo
 Author-email: aaa57403@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -69,7 +69,11 @@
 * fixed bug
 
 ### V 0.7.3
 * Change the code to get the next node
 
 ### V 0.8.0
 * Can be separated by facility
+
+### V 0.9.0
+* refactoring code
+* can see facilities history(Facility performance record => DataFrame(columns = [@timestamp, expire, wait]))
```

