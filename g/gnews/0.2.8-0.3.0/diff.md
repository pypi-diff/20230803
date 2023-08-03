# Comparing `tmp/gnews-0.2.8.tar.gz` & `tmp/gnews-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnews-0.2.8.tar", last modified: Wed Aug  2 14:38:15 2023, max compression
+gzip compressed data, was "gnews-0.3.0.tar", last modified: Wed Aug  2 14:44:06 2023, max compression
```

## Comparing `gnews-0.2.8.tar` & `gnews-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:15.423370 gnews-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 14:38:04.000000 gnews-0.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17336 2023-08-02 14:38:15.423370 gnews-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16112 2023-08-02 14:38:04.000000 gnews-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:15.415369 gnews-0.2.8/gnews/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 14:38:04.000000 gnews-0.2.8/gnews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-08-02 14:38:04.000000 gnews-0.2.8/gnews/gnews.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:15.415369 gnews-0.2.8/gnews/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:04.000000 gnews-0.2.8/gnews/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24441 2023-08-02 14:38:04.000000 gnews-0.2.8/gnews/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-08-02 14:38:04.000000 gnews-0.2.8/gnews/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:15.415369 gnews-0.2.8/gnews.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17336 2023-08-02 14:38:15.000000 gnews-0.2.8/gnews.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-02 14:38:15.000000 gnews-0.2.8/gnews.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:38:15.000000 gnews-0.2.8/gnews.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-02 14:38:15.000000 gnews-0.2.8/gnews.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 14:38:15.000000 gnews-0.2.8/gnews.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:38:15.423370 gnews-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-02 14:38:04.000000 gnews-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:06.173660 gnews-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 14:43:55.000000 gnews-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17336 2023-08-02 14:44:06.173660 gnews-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16112 2023-08-02 14:43:55.000000 gnews-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:06.169660 gnews-0.3.0/gnews/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 14:43:55.000000 gnews-0.3.0/gnews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-08-02 14:43:55.000000 gnews-0.3.0/gnews/gnews.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:06.173660 gnews-0.3.0/gnews/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:55.000000 gnews-0.3.0/gnews/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24441 2023-08-02 14:43:55.000000 gnews-0.3.0/gnews/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-08-02 14:43:55.000000 gnews-0.3.0/gnews/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:06.173660 gnews-0.3.0/gnews.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17336 2023-08-02 14:44:06.000000 gnews-0.3.0/gnews.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-02 14:44:06.000000 gnews-0.3.0/gnews.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:44:06.000000 gnews-0.3.0/gnews.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-02 14:44:06.000000 gnews-0.3.0/gnews.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 14:44:06.000000 gnews-0.3.0/gnews.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:44:06.173660 gnews-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-02 14:43:55.000000 gnews-0.3.0/setup.py
```

### Comparing `gnews-0.2.8/LICENSE.txt` & `gnews-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gnews-0.2.8/PKG-INFO` & `gnews-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnews
-Version: 0.2.8
+Version: 0.3.0
 Summary: Provide an API to search for articles on Google News and returns a usable JSON response.
 Home-page: https://github.com/ranahaani/GNews/
 Author: Muhammad Abdullah
 Author-email: ranahaani@gmail.com
 Project-URL: Documentation, https://github.com/ranahaani/GNews/blob/master/README.md
 Project-URL: Source, https://github.com/ranahaani/GNews/
 Project-URL: Tracker, https://github.com/ranahaani/GNews/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gnews Version: 0.2.8 Summary: Provide an API to
+Metadata-Version: 2.1 Name: gnews Version: 0.3.0 Summary: Provide an API to
 search for articles on Google News and returns a usable JSON response. Home-
 page: https://github.com/ranahaani/GNews/ Author: Muhammad Abdullah Author-
 email: ranahaani@gmail.com Project-URL: Documentation, https://github.com/
 ranahaani/GNews/blob/master/README.md Project-URL: Source, https://github.com/
 ranahaani/GNews/ Project-URL: Tracker, https://github.com/ranahaani/GNews/
 issues Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
```

### Comparing `gnews-0.2.8/README.md` & `gnews-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gnews-0.2.8/gnews/gnews.py` & `gnews-0.3.0/gnews/gnews.py`

 * *Files identical despite different names*

### Comparing `gnews-0.2.8/gnews/utils/constants.py` & `gnews-0.3.0/gnews/utils/constants.py`

 * *Files identical despite different names*

### Comparing `gnews-0.2.8/gnews/utils/utils.py` & `gnews-0.3.0/gnews/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gnews-0.2.8/gnews.egg-info/PKG-INFO` & `gnews-0.3.0/gnews.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnews
-Version: 0.2.8
+Version: 0.3.0
 Summary: Provide an API to search for articles on Google News and returns a usable JSON response.
 Home-page: https://github.com/ranahaani/GNews/
 Author: Muhammad Abdullah
 Author-email: ranahaani@gmail.com
 Project-URL: Documentation, https://github.com/ranahaani/GNews/blob/master/README.md
 Project-URL: Source, https://github.com/ranahaani/GNews/
 Project-URL: Tracker, https://github.com/ranahaani/GNews/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gnews Version: 0.2.8 Summary: Provide an API to
+Metadata-Version: 2.1 Name: gnews Version: 0.3.0 Summary: Provide an API to
 search for articles on Google News and returns a usable JSON response. Home-
 page: https://github.com/ranahaani/GNews/ Author: Muhammad Abdullah Author-
 email: ranahaani@gmail.com Project-URL: Documentation, https://github.com/
 ranahaani/GNews/blob/master/README.md Project-URL: Source, https://github.com/
 ranahaani/GNews/ Project-URL: Tracker, https://github.com/ranahaani/GNews/
 issues Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
```

### Comparing `gnews-0.2.8/setup.py` & `gnews-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='gnews',
-    version='0.2.8',
+    version='0.3.0',
     author="Muhammad Abdullah",
     author_email="ranahaani@gmail.com",
     description='Provide an API to search for articles on Google News and returns a usable JSON response.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=requirements,
```

