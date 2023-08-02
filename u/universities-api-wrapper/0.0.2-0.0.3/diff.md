# Comparing `tmp/universities-api-wrapper-0.0.2.tar.gz` & `tmp/universities-api-wrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universities-api-wrapper-0.0.2.tar", last modified: Fri May 19 23:37:43 2023, max compression
+gzip compressed data, was "universities-api-wrapper-0.0.3.tar", last modified: Wed Aug  2 23:32:58 2023, max compression
```

## Comparing `universities-api-wrapper-0.0.2.tar` & `universities-api-wrapper-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-05-19 23:37:43.189533 universities-api-wrapper-0.0.2/
--rw-r--r--   0 juha      (1000) juha      (1000)     1076 2023-02-27 23:06:02.000000 universities-api-wrapper-0.0.2/LICENSE.txt
--rw-r--r--   0 juha      (1000) juha      (1000)      746 2023-05-19 23:37:43.190533 universities-api-wrapper-0.0.2/PKG-INFO
--rw-r--r--   0 juha      (1000) juha      (1000)     2038 2023-04-18 23:02:26.000000 universities-api-wrapper-0.0.2/README.md
--rw-r--r--   0 juha      (1000) juha      (1000)      106 2023-05-19 23:37:43.190533 universities-api-wrapper-0.0.2/setup.cfg
--rw-r--r--   0 juha      (1000) juha      (1000)     1097 2023-05-19 23:28:21.000000 universities-api-wrapper-0.0.2/setup.py
-drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-05-19 23:37:43.185533 universities-api-wrapper-0.0.2/tests/
--rw-r--r--   0 juha      (1000) juha      (1000)     1618 2023-04-18 23:02:26.000000 universities-api-wrapper-0.0.2/tests/test_universities_api_wrapper.py
-drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-05-19 23:37:43.186533 universities-api-wrapper-0.0.2/universities_api_wrapper/
--rw-r--r--   0 juha      (1000) juha      (1000)     1956 2023-04-18 23:02:26.000000 universities-api-wrapper-0.0.2/universities_api_wrapper/__init__.py
-drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-05-19 23:37:43.189533 universities-api-wrapper-0.0.2/universities_api_wrapper.egg-info/
--rw-r--r--   0 juha      (1000) juha      (1000)      746 2023-05-19 23:37:42.000000 universities-api-wrapper-0.0.2/universities_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 juha      (1000) juha      (1000)      355 2023-05-19 23:37:43.000000 universities-api-wrapper-0.0.2/universities_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 juha      (1000) juha      (1000)        1 2023-05-19 23:37:42.000000 universities-api-wrapper-0.0.2/universities_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 juha      (1000) juha      (1000)       14 2023-05-19 23:37:42.000000 universities-api-wrapper-0.0.2/universities_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 juha      (1000) juha      (1000)       25 2023-05-19 23:37:42.000000 universities-api-wrapper-0.0.2/universities_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-08-02 23:32:58.474692 universities-api-wrapper-0.0.3/
+-rw-r--r--   0 juha      (1000) juha      (1000)     1076 2023-02-27 23:06:02.000000 universities-api-wrapper-0.0.3/LICENSE.txt
+-rw-r--r--   0 juha      (1000) juha      (1000)      746 2023-08-02 23:32:58.474692 universities-api-wrapper-0.0.3/PKG-INFO
+-rw-r--r--   0 juha      (1000) juha      (1000)     2762 2023-07-09 19:21:00.000000 universities-api-wrapper-0.0.3/README.md
+-rw-r--r--   0 juha      (1000) juha      (1000)      106 2023-08-02 23:32:58.475692 universities-api-wrapper-0.0.3/setup.cfg
+-rw-r--r--   0 juha      (1000) juha      (1000)     1097 2023-08-02 23:22:29.000000 universities-api-wrapper-0.0.3/setup.py
+drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-08-02 23:32:58.470692 universities-api-wrapper-0.0.3/tests/
+-rw-r--r--   0 juha      (1000) juha      (1000)     1618 2023-04-18 23:02:26.000000 universities-api-wrapper-0.0.3/tests/test_universities_api_wrapper.py
+drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-08-02 23:32:58.471692 universities-api-wrapper-0.0.3/universities_api_wrapper/
+-rw-r--r--   0 juha      (1000) juha      (1000)     2260 2023-08-02 23:05:09.000000 universities-api-wrapper-0.0.3/universities_api_wrapper/__init__.py
+drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-08-02 23:32:58.474692 universities-api-wrapper-0.0.3/universities_api_wrapper.egg-info/
+-rw-r--r--   0 juha      (1000) juha      (1000)      746 2023-08-02 23:32:58.000000 universities-api-wrapper-0.0.3/universities_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 juha      (1000) juha      (1000)      355 2023-08-02 23:32:58.000000 universities-api-wrapper-0.0.3/universities_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 juha      (1000) juha      (1000)        1 2023-08-02 23:32:58.000000 universities-api-wrapper-0.0.3/universities_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 juha      (1000) juha      (1000)       14 2023-08-02 23:32:58.000000 universities-api-wrapper-0.0.3/universities_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 juha      (1000) juha      (1000)       25 2023-08-02 23:32:58.000000 universities-api-wrapper-0.0.3/universities_api_wrapper.egg-info/top_level.txt
```

### Comparing `universities-api-wrapper-0.0.2/LICENSE.txt` & `universities-api-wrapper-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `universities-api-wrapper-0.0.2/PKG-INFO` & `universities-api-wrapper-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: universities-api-wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Universities API Wrapper
 Home-page: https://github.com/jremes-foss/universities-api-wrapper/
-Download-URL: https://github.com/jremes-foss/universities-api-wrapper/archive/refs/tags/0.0.2.tar.gz
+Download-URL: https://github.com/jremes-foss/universities-api-wrapper/archive/refs/tags/0.0.3.tar.gz
 Author: Juha Remes
 Author-email: jremes@outlook.com
 Keywords: python,api,wrapper,education,universities
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `universities-api-wrapper-0.0.2/setup.py` & `universities-api-wrapper-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Universities API Wrapper'
 LONG_DESCRIPTION = 'Python package for consuming universities-domains-list API'
 
 # Setting up
 setup(
         name="universities-api-wrapper",
         version=VERSION,
         author="Juha Remes",
         author_email="jremes@outlook.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
         url='https://github.com/jremes-foss/universities-api-wrapper/',
-        download_url='https://github.com/jremes-foss/universities-api-wrapper/archive/refs/tags/0.0.2.tar.gz',
+        download_url='https://github.com/jremes-foss/universities-api-wrapper/archive/refs/tags/0.0.3.tar.gz',
         install_requires=['requests', 'mock'],
         keywords=['python', 'api', 'wrapper', 'education', 'universities'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 2",
             "Programming Language :: Python :: 3",
```

### Comparing `universities-api-wrapper-0.0.2/tests/test_universities_api_wrapper.py` & `universities-api-wrapper-0.0.3/tests/test_universities_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `universities-api-wrapper-0.0.2/universities_api_wrapper/__init__.py` & `universities-api-wrapper-0.0.3/universities_api_wrapper/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,22 @@
         logger.debug("Successful request: {}".format(response.status_code))
 
     @staticmethod
     def endpoints():
         """ Returns endpoints of universities API. """
         return ["name", "country"]
 
-    def search(self, country=None, name=None) -> dict:
+    def get_names(self, response: Response):
+        """ Returns names of universities in a list. """
+        names = []
+        for uni in response:
+            names.append(uni['name'])
+        return names
+
+    def search(self, country=None, name=None, filters=None) -> dict:
         """ This method searches by name and country. """
 
         base_url = self._get_method(self.method, self.port)
 
         if not country and not name:
             raise ValueError("Please provide valid university name or country.")
         elif not name:
@@ -52,13 +59,16 @@
         else:
             url = f"{base_url}?name={name.lower()}&country={country.lower()}"
 
         response = requests.get(url=url)
         self._check_online(response)
         response = response.json()
 
+        if filters == 'names':
+            response = self.get_names(response)
+
         return response
 
 
 class UniversitiesAPIError(Exception):
     """ Empty class used for raising exceptions. """
     pass
```

### Comparing `universities-api-wrapper-0.0.2/universities_api_wrapper.egg-info/PKG-INFO` & `universities-api-wrapper-0.0.3/universities_api_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: universities-api-wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Universities API Wrapper
 Home-page: https://github.com/jremes-foss/universities-api-wrapper/
-Download-URL: https://github.com/jremes-foss/universities-api-wrapper/archive/refs/tags/0.0.2.tar.gz
+Download-URL: https://github.com/jremes-foss/universities-api-wrapper/archive/refs/tags/0.0.3.tar.gz
 Author: Juha Remes
 Author-email: jremes@outlook.com
 Keywords: python,api,wrapper,education,universities
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

