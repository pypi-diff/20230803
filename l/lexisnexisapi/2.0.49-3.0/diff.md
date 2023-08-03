# Comparing `tmp/lexisnexisapi-2.0.49.tar.gz` & `tmp/lexisnexisapi-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexisnexisapi-2.0.49.tar", last modified: Tue Jul 18 18:16:03 2023, max compression
+gzip compressed data, was "lexisnexisapi-3.0.tar", last modified: Thu Aug  3 15:32:45 2023, max compression
```

## Comparing `lexisnexisapi-2.0.49.tar` & `lexisnexisapi-3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 18:16:03.408857 lexisnexisapi-2.0.49/
--rw-rw-rw-   0        0        0      466 2022-12-20 12:40:20.000000 lexisnexisapi-2.0.49/LICENSE.txt
--rw-rw-rw-   0        0        0     6289 2023-07-18 18:16:03.405857 lexisnexisapi-2.0.49/PKG-INFO
--rw-rw-rw-   0        0        0     5734 2023-07-18 18:14:15.000000 lexisnexisapi-2.0.49/README.md
--rw-rw-rw-   0        0        0      619 2023-07-18 18:14:32.000000 lexisnexisapi-2.0.49/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 18:16:03.409858 lexisnexisapi-2.0.49/setup.cfg
--rw-rw-rw-   0        0        0      766 2023-07-18 18:14:43.000000 lexisnexisapi-2.0.49/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:16:03.327858 lexisnexisapi-2.0.49/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 18:16:03.372858 lexisnexisapi-2.0.49/src/lexisnexisapi/
--rw-rw-rw-   0        0        0        0 2023-01-28 19:22:50.000000 lexisnexisapi-2.0.49/src/lexisnexisapi/__init__.py
--rw-rw-rw-   0        0        0     1863 2023-02-02 17:25:44.000000 lexisnexisapi-2.0.49/src/lexisnexisapi/credentials.py
--rw-rw-rw-   0        0        0     9920 2023-06-29 14:53:39.000000 lexisnexisapi-2.0.49/src/lexisnexisapi/metabase.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:16:03.399859 lexisnexisapi-2.0.49/src/lexisnexisapi.egg-info/
--rw-rw-rw-   0        0        0     6289 2023-07-18 18:16:03.000000 lexisnexisapi-2.0.49/src/lexisnexisapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-18 18:16:03.000000 lexisnexisapi-2.0.49/src/lexisnexisapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 18:16:03.000000 lexisnexisapi-2.0.49/src/lexisnexisapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-18 18:16:03.000000 lexisnexisapi-2.0.49/src/lexisnexisapi.egg-info/top_level.txt
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-03 15:32:45.731744 lexisnexisapi-3.0/
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      466 2023-08-02 01:16:32.000000 lexisnexisapi-3.0/LICENSE.txt
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     6031 2023-08-03 15:32:45.731488 lexisnexisapi-3.0/PKG-INFO
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     5659 2023-08-03 15:24:28.000000 lexisnexisapi-3.0/README.md
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      616 2023-08-03 15:21:57.000000 lexisnexisapi-3.0/pyproject.toml
+-rw-r--r--   0 rwcuffney   (501) staff       (20)       38 2023-08-03 15:32:45.731817 lexisnexisapi-3.0/setup.cfg
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      765 2023-08-03 15:21:25.000000 lexisnexisapi-3.0/setup.py
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-03 15:32:45.727594 lexisnexisapi-3.0/src/
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-03 15:32:45.729909 lexisnexisapi-3.0/src/lexisnexisapi/
+-rw-r--r--   0 rwcuffney   (501) staff       (20)        0 2023-08-02 01:16:32.000000 lexisnexisapi-3.0/src/lexisnexisapi/__init__.py
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     2338 2023-08-02 20:21:18.000000 lexisnexisapi-3.0/src/lexisnexisapi/credentials.py
+-rw-r--r--   0 rwcuffney   (501) staff       (20)    10144 2023-08-02 20:20:42.000000 lexisnexisapi-3.0/src/lexisnexisapi/metabase.py
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-03 15:32:45.731132 lexisnexisapi-3.0/src/lexisnexisapi.egg-info/
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     6031 2023-08-03 15:32:45.000000 lexisnexisapi-3.0/src/lexisnexisapi.egg-info/PKG-INFO
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      302 2023-08-03 15:32:45.000000 lexisnexisapi-3.0/src/lexisnexisapi.egg-info/SOURCES.txt
+-rw-r--r--   0 rwcuffney   (501) staff       (20)        1 2023-08-03 15:32:45.000000 lexisnexisapi-3.0/src/lexisnexisapi.egg-info/dependency_links.txt
+-rw-r--r--   0 rwcuffney   (501) staff       (20)       14 2023-08-03 15:32:45.000000 lexisnexisapi-3.0/src/lexisnexisapi.egg-info/top_level.txt
```

### Comparing `lexisnexisapi-2.0.49/PKG-INFO` & `lexisnexisapi-3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,181 +1,180 @@
-Metadata-Version: 2.1
-Name: lexisnexisapi
-Version: 2.0.49
-Summary: A module to support the lexisnexis metabase search api
-Home-page: 
-Author: Robert Cuffney
-Author-email: Robert Cuffney <robert.cuffney@lexisnexis.com>, Ozgur Aycan <ozgur.aycan@lexisnexis.co.uk>
-License: MIT
-Keywords: example project
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# Metabase.py Documentation
-
-## 1. Introduction
-
-### Overview
-
-The `metabase.py` module provides a Python interface to interact with the Metabase API. It allows you to perform searches and retrieve articles using the Metabase API. The module facilitates the creation of Python objects representing the API response, making it easy to work with the data.
-
-### Authors
-
-- Robert Cuffney
-- Ozgur Aycan
-- CS Integration Consultants @ LexisNexis
-
-### Version
-
-Current version: 2.0.49
-## 2. Installation
-
-### Dependencies
-
-To use the `metabase.py` module, you need the following dependencies:
-
-- requests
-- json
-- pandas
-- datetime
-- lexisnexisapi
-
-### Installation
-
-You can install the required dependencies using pip:
-
-```bash
-pip install requests pandas lexisnexisapi
-```
-
-## 3. Usage
-
-### Importing the Module
-
-To use the `metabase.py` module in your Python script, import it as follows:
-
-```python
-from lexisnexisapi import metabase
-```
-
-### Search Class
-
-The `Search` class is the main interface to perform searches and retrieve articles from Metabase. It has the following attributes and methods:
-
-#### Attributes:
-
-- `parameters`: A dictionary of Metabase search parameters.
-- `articles`: A list containing the articles retrieved from the Metabase API response.
-- `totalResults`: The total number of articles available in the search results.
-
-#### Methods:
-
-- `__init__(self, full_dataset=False, **kwargs)`: Initializes the Search object and performs the API request. If `full_dataset` is set to `True`, it retrieves all available articles by making multiple API calls.
-- `articles_dataframe(self, *args)`: Returns a Pandas DataFrame containing the articles' data. You can pass a list of desired fields (`*args`) to filter the DataFrame.
-- `create_file(self, file='articles.json')`: Creates a JSON file with the articles retrieved from the search.
-- `set_parameters(self, p)`: Sets the Metabase search parameters based on the input dictionary `p`.
-
-### Streamline Class
-
-The `Streamline` class helps maximize Metabase search calls without exceeding the rate limit. It keeps track of the remaining API calls per minute and waits for a new minute if needed.
-
-#### Attributes:
-
-- `key`: Metabase API key.
-- `start_minute`: The starting minute when the Streamline object is instantiated.
-- `minute_limit`: The maximum number of API calls allowed per minute based on the rate limit.
-- `calls_remaining`: The remaining API calls within the current minute.
-
-#### Methods:
-
-- `__init__(self, key)`: Initializes the Streamline object with the Metabase API key and fetches the rate limit information.
-- `track_calls(self)`: Updates the remaining API calls and waits for a new minute if the limit is reached.
-- `restart(self)`: Restarts the Streamline object.
-- `wait_for_new_min(self)`: Pauses execution until a new minute starts.
-- `get_current_minute(self)`: Returns the current minute as an integer.
-
-### Article Class
-
-The `Article` class represents an instance of a single article retrieved from Metabase. It sets each key from the article dictionary as an attribute of the class.
-
-### Helper Functions
-
-The module also provides some helper functions:
-
-- `http_request(p)`: Performs an HTTP request to the Metabase API with the given parameters `p` and returns the API response as a dictionary.
-- `rate_check(mbkey)`: Calls the Metabase rate limit API and returns the results as a list of dictionaries.
-- `set_mb_search_key(v)`: Sets the Metabase search key in the credentials.
-- `mb_search_key()`: Retrieves the Metabase search key from the credentials.
-- `get_time()`: Returns the current minute as an integer.
-
-## 4. Examples
-
-### Basic Search Example
-
-```python
-from lexisnexisapi import metabase
-
-# Set the Metabase search key (optional, you can set it in the parameters directly)
-metabase.set_mb_search_key("your_metabase_key")
-
-# Perform a basic search
-search = metabase.Search(query="your_query_here", limit=100)
-
-# Get the DataFrame of articles
-df = search.articles_dataframe("title", "author", "published_date")
-print(df.head())
-```
-
-### Full Dataset Search Example
-
-```python
-from lexisnexisapi import metabase
-
-# Set the Metabase search key (optional, you can set it in the parameters directly)
-metabase.set_mb_search_key("your_metabase_key")
-
-# Perform a full dataset search
-search = metabase.Search(full_dataset=True, query="your_query_here")
-
-# Create a JSON file with all the articles
-search.create_file("articles_full.json")
-```
-
-### Article Instance Example
-
-```python
-from lexisnexisapi  import metabase
-
-# Set the Metabase search key (optional, you can set it in the parameters directly)
-metabase.set_mb_search_key("your_metabase_key")
-
-# Perform a search and get an article instance
-search = metabase.Search(query="your_query_here", limit=1)
-article_instance = metabase.Article(search.articles[0])
-
-# Access attributes of the article instance
-print(article_instance.title)
-print(article_instance.author)
-print(article_instance.published_date)
-```
-
-### Index Terms Example
-
-```python
-from lexisnexisapi import metabase
-
-# Set the Metabase search key (optional, you can set it in the parameters directly)
-metabase.set_mb_search_key("your_metabase_key")
-
-# Perform a search
-search = metabase.Search(query="your_query_here", limit=100)
-
-# Get the DataFrame of index terms
-index_terms_df = metabase.indexTerms(search, "economy", "politics", "technology")
-print(index_terms_df.head())
-```
-
-Please note that you should replace `your_metabase_key` and `your_query_here` with your actual Metabase API key and desired search query, respectively, in the examples.
+Metadata-Version: 2.1
+Name: lexisnexisapi
+Version: 3.0
+Summary: A module to support the lexisnexis metabase search api
+Home-page: 
+Author: Robert Cuffney
+Author-email: Robert Cuffney <robert.cuffney@lexisnexis.com>, Ozgur Aycan <ozgur.aycan@lexisnexis.co.uk>
+License: MIT
+Keywords: example project
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Metabase.py Documentation
+
+## 1. Introduction
+
+### Overview
+
+The `metabase.py` module provides a Python interface to interact with the Metabase API. It allows you to perform searches and retrieve articles using the Metabase API. The module facilitates the creation of Python objects representing the API response, making it easy to work with the data.
+
+### Authors
+
+- Robert Cuffney
+- Ozgur Aycan
+- CS Integration Consultants @ LexisNexis
+
+### Version
+
+Current version: 3.0
+## 2. Installation
+
+### Dependencies
+
+To use the `metabase.py` module, you need the following dependencies:
+
+- requests
+- json
+- pandas
+- datetime
+- lexisnexisapi
+
+### Installation
+
+You can install the required dependencies using pip:
+
+```bash
+pip install requests pandas lexisnexisapi
+```
+
+## 3. Usage
+
+### Importing the Module
+
+To use the `metabase.py` module in your Python script, import it as follows:
+
+```python
+from lexisnexisapi import metabase
+```
+
+### Search Class
+
+The `Search` class is the main interface to perform searches and retrieve articles from Metabase. It has the following attributes and methods:
+
+#### Attributes:
+
+- `parameters`: A dictionary of Metabase search parameters.
+- `articles`: A list containing the articles retrieved from the Metabase API response.
+- `totalResults`: The total number of articles available in the search results.
+
+#### Methods:
+
+- `__init__(self, full_dataset=False, **kwargs)`: Initializes the Search object and performs the API request. If `full_dataset` is set to `True`, it retrieves all available articles by making multiple API calls.
+- `articles_dataframe(self, *args)`: Returns a Pandas DataFrame containing the articles' data. You can pass a list of desired fields (`*args`) to filter the DataFrame.
+- `create_file(self, file='articles.json')`: Creates a JSON file with the articles retrieved from the search.
+- `set_parameters(self, p)`: Sets the Metabase search parameters based on the input dictionary `p`.
+
+### Streamline Class
+
+The `Streamline` class helps maximize Metabase search calls without exceeding the rate limit. It keeps track of the remaining API calls per minute and waits for a new minute if needed.
+
+#### Attributes:
+
+- `key`: Metabase API key.
+- `start_minute`: The starting minute when the Streamline object is instantiated.
+- `minute_limit`: The maximum number of API calls allowed per minute based on the rate limit.
+- `calls_remaining`: The remaining API calls within the current minute.
+
+#### Methods:
+
+- `__init__(self, key)`: Initializes the Streamline object with the Metabase API key and fetches the rate limit information.
+- `track_calls(self)`: Updates the remaining API calls and waits for a new minute if the limit is reached.
+- `restart(self)`: Restarts the Streamline object.
+- `wait_for_new_min(self)`: Pauses execution until a new minute starts.
+- `get_current_minute(self)`: Returns the current minute as an integer.
+
+### Article Class
+
+The `Article` class represents an instance of a single article retrieved from Metabase. It sets each key from the article dictionary as an attribute of the class.
+
+### Helper Functions
+
+The module also provides some helper functions:
+
+- `http_request(p)`: Performs an HTTP request to the Metabase API with the given parameters `p` and returns the API response as a dictionary.
+- `rate_check(mbkey)`: Calls the Metabase rate limit API and returns the results as a list of dictionaries.
+- `set_Metabase_Search_Key(v)`: Sets the Metabase search key in the credentials.
+- `get_time()`: Returns the current minute as an integer.
+
+## 4. Examples
+
+### Basic Search Example
+
+```python
+from lexisnexisapi import metabase
+
+# Set the Metabase search key (optional, you can set it in the parameters directly)
+metabase.set_mb_search_key("your_metabase_key")
+
+# Perform a basic search
+search = metabase.Search(query="your_query_here", limit=100)
+
+# Get the DataFrame of articles
+df = search.articles_dataframe("title", "author", "published_date")
+print(df.head())
+```
+
+### Full Dataset Search Example
+
+```python
+from lexisnexisapi import metabase
+
+# Set the Metabase search key (optional, you can set it in the parameters directly)
+metabase.set_mb_search_key("your_metabase_key")
+
+# Perform a full dataset search
+search = metabase.Search(full_dataset=True, query="your_query_here")
+
+# Create a JSON file with all the articles
+search.create_file("articles_full.json")
+```
+
+### Article Instance Example
+
+```python
+from lexisnexisapi  import metabase
+
+# Set the Metabase search key (optional, you can set it in the parameters directly)
+metabase.set_mb_search_key("your_metabase_key")
+
+# Perform a search and get an article instance
+search = metabase.Search(query="your_query_here", limit=1)
+article_instance = metabase.Article(search.articles[0])
+
+# Access attributes of the article instance
+print(article_instance.title)
+print(article_instance.author)
+print(article_instance.published_date)
+```
+
+### Index Terms Example
+
+```python
+from lexisnexisapi import metabase
+
+# Set the Metabase search key (optional, you can set it in the parameters directly)
+metabase.set_mb_search_key("your_metabase_key")
+
+# Perform a search
+search = metabase.Search(query="your_query_here", limit=100)
+
+# Get the DataFrame of index terms
+index_terms_df = metabase.indexTerms(search, "economy", "politics", "technology")
+print(index_terms_df.head())
+```
+
+Please note that you should replace `your_metabase_key` and `your_query_here` with your actual Metabase API key and desired search query, respectively, in the examples.
```

### Comparing `lexisnexisapi-2.0.49/README.md` & `lexisnexisapi-3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 - Robert Cuffney
 - Ozgur Aycan
 - CS Integration Consultants @ LexisNexis
 
 ### Version
 
-Current version: 2.0.49
+Current version: 3.0
 ## 2. Installation
 
 ### Dependencies
 
 To use the `metabase.py` module, you need the following dependencies:
 
 - requests
@@ -87,16 +87,15 @@
 
 ### Helper Functions
 
 The module also provides some helper functions:
 
 - `http_request(p)`: Performs an HTTP request to the Metabase API with the given parameters `p` and returns the API response as a dictionary.
 - `rate_check(mbkey)`: Calls the Metabase rate limit API and returns the results as a list of dictionaries.
-- `set_mb_search_key(v)`: Sets the Metabase search key in the credentials.
-- `mb_search_key()`: Retrieves the Metabase search key from the credentials.
+- `set_Metabase_Search_Key(v)`: Sets the Metabase search key in the credentials.
 - `get_time()`: Returns the current minute as an integer.
 
 ## 4. Examples
 
 ### Basic Search Example
 
 ```python
```

### Comparing `lexisnexisapi-2.0.49/pyproject.toml` & `lexisnexisapi-3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lexisnexisapi"
-version = "2.0.49"
+version = "3.0"
 authors = [{ name = "Robert Cuffney", email = "robert.cuffney@lexisnexis.com" },
 		   { name = "Ozgur Aycan", email = "ozgur.aycan@lexisnexis.co.uk" }
 ]
 description = "A module to support the lexisnexis metabase search api"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lexisnexisapi-2.0.49/setup.py` & `lexisnexisapi-3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="lexisnexisapi",
-    version='2.0.49',
+    version='3.0',
     license='MIT',
     author="Robert Cuffney",
     author_email='robert.cuffney@lexisnexis.com',
     description = 'a module to support the lexisnexis metabase search api',
     long_description = ' module provides a Python interface to interact with the Metabase API. It allows you to perform searches and retrieve articles using the Metabase API. The module facilitates the creation of Python objects representing the API response, making it easy to work with the data.',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     include_package_data=True,
     url='',
     keywords='example project',
     install_requires=[],
      
 
-)
+)
```

### Comparing `lexisnexisapi-2.0.49/src/lexisnexisapi/metabase.py` & `lexisnexisapi-3.0/src/lexisnexisapi/metabase.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 from datetime import datetime
 from lexisnexisapi import credentials as cred
 import time
 import ast
 
 
-__version__ = '0.1'
+__version__ = '2.0'
 __author__ = "Robert Cuffney & Ozgur Aycan, CS Integration Consultants @ LexisNexis"
 
 #Constants are usually defined on a module level and written in all capital letters with underscores separating words. 
 #Examples include MAX_OVERFLOW and TOTAL.
 
 #url = 'http://metabase.moreover.com/api/v10/searchArticles?'
 
@@ -24,72 +24,71 @@
     '''
     mbSearch class
     returns API response as a python class
     accepts either a string query, or a dictionary of all metabase parameters
     full_dataset = True -- activates the option to create a full dataset of total results 
     '''
     def __init__(self,  full_dataset = False,**kwargs):
-        self.parameters = self.set_parameters(kwargs)
-        if full_dataset:
-            data = self.get_fulldataset()
-            print(data['totalResults'])
-        else:
-            data = http_request(self.parameters)
-        if type(data)==dict:
-            self.__dict__.update(data)
-        else:
-            print("Something went wrong, No data was returned")
+        try:
+            self.parameters = self.set_parameters(kwargs)
+            if full_dataset:
+                data = self.get_fulldataset()
+                print(data['totalResults'])
+            else:
+                data = http_request(self.parameters)
+            if type(data)==dict:
+                self.__dict__.update(data)
+            else:
+                print("Something went wrong, No data was returned")
+        except Exception as e:
+            print(f"Error occurred: {e}")
     def set_parameters(self,p):
-        if 'key' not in p:
-            p['key']= cred.get_Key("Metabase_Search_Key")
-        if 'limit' not in p:
-            p['limit']='1000'
-        p['format']='json'
-        if p['key']=='':
-            msg ='''
-            No key saved or sent 
-            to save a key:
-            use metabase.set_mb_search_key("your key here")
-            to send a key:
-            include key parameter in your metabase.Search parameters (e.g. metabase.Search(key="your key here", query="your query")
-            '''
-            print(msg)
-        return p
+        try:
+            p.setdefault('key', cred.get_Key("Metabase_Search_Key"))
+            p.setdefault('limit','10000')
+            p['format']='json'
+            return p
+        except Exception as e:
+            print(f"Error occurred: {e}")
     def articles_dataframe(self,*args):
         '''
         returns a data frame of the articles
         optional parameter fields, is a list of desired fields to return
         '''
-        #df = pd.DataFrame()
-        df = pd.DataFrame.from_records(self.articles)
-        ## Filter dataframe, if *args are provided
-        if args:
-            series = list(args)
-            df = df[series]
-        return df
+        try:
+            df = pd.DataFrame.from_records(self.articles)
+            ## Filter dataframe, if *args are provided
+            if args:
+                series = list(args)
+                df = df[series]
+            return df
+        except Exception as e:
+            print(f"Error occurred: {e}")
     def create_file(self,file='articles.json'):
         '''
         creates a json file
         '''
-        if self.totalResults != 0:
-            with open(file, "w") as my_file:
-                my_file.write(json.dumps(self.articles, indent=4))
-                print(f'{len(self.articles)} article(s) successfully written to a file:{file}')
-        else:
-            print("no articles to write to file!") 
+        try:
+            if self.totalResults != 0:
+                with open(file, "w") as my_file:
+                    my_file.write(json.dumps(self.articles, indent=4))
+                    print(f'{len(self.articles)} article(s) successfully written to a file:{file}')
+            else:
+                print("no articles to write to file!") 
+        except Exception as e:
+            print(f"Error occurred: {e}")
 
 #### Below Functions, within this class, used only for FullDataSet
     def get_fulldataset(self):
         self.parameters.pop('sequence_id',"")                 #get rid of 'sequence_id' if it's there
         #self.parameters['limit']='1000'                       #This will set the limit to the maximum allowed per their key  
         t_lst =[]                                             #this will be the list of all articles
         x=1                                                   #this will represent the number of articles left
         try:
             i=1                                               #i counts the number of loops occurring
-            #self.call_counter()  
             mc = Streamline(self.parameters['key'])
             while x > 0:                                      #run while x (number of articles remaining)
                 #self.set_calls()                               #use set_calls object to determine calls left in minute
                 mc.track_calls()
                 myData = http_request(self.parameters)             #call API
                 t_lst = t_lst + myData['articles']            #add articles to t_lst  
                 s_id = myData['articles'][-1]['sequenceId']   #find the last sequence id available
@@ -102,15 +101,15 @@
             print("all done")                                 #print to notify user of completion  
             #total = len(t_lst)                               #total of all articles pulled, should equal original 'totalResults'
             myData['articles']= t_lst                         #set the total list of articles as the value in the key 'articles'
             myData['totalResults']= len(t_lst)                #make sure the 'totalResults' key is set to the original 'totalResults'
             return myData
         #error handling:
         except Exception as e:
-            print(f"error:{e}")
+            print(f"Error occurred: {e}")
 
 class Streamline:
     '''
     This is a class object to maximize metabase search calls without going over the
     calls per minute limit.  Class is used as a counter
     Upon instantiation the rate limit API is called. 
     The Streamline object will reset it's calls_remaining to the minute_limit at the beginning of every new minute.
@@ -145,43 +144,43 @@
         self.start_minute = current_minute
         self.calls_remaining= self.minute_limit -1
     def get_current_minute(self):
         return datetime.now().minute
         
     
 def http_request(p):
-    url = METABASE_SEARCH_URL 
-    r = requests.get(url, params=p) 
-    data = r.__dict__.copy()
-    data.pop('_content', None)
-    data.update(r.json())
-    if r.status_code != 200:
-        print(r.text)
-        print('An error occurred while attempting to retrieve data from the API.')   
-    return data
-def rate_check(mbkey):
+    try:
+        url = METABASE_SEARCH_URL 
+        r = requests.get(url, params=p) 
+        data = r.__dict__.copy()
+        data.pop('_content', None)
+        data.update(r.json())
+        if r.status_code != 200:
+            print(r.text)
+            print('An error occurred while attempting to retrieve data from the API.')   
+        return data
+    except Exception as e:
+        print(f"Error occurred: {e}")
+def rate_check(key):
     '''
     Calls the Metabase rate limit API and returns the results as a list of dictionaries
     '''
-    if not mbkey:
-        mbkey = cred.get_Key('Metabase_Search_Key')
-    rateCheckUrl = METABASE_RATE_CHECK_URL + mbkey
-    r = requests.get(rateCheckUrl)
-    if r.status_code == 200:
-        data = r.json()
-    return data['rateLimits']
+    try:
+        if not key:
+            key = cred.get_Key('Metabase_Search_Key')
+        rateCheckUrl = METABASE_RATE_CHECK_URL + key
+        r = requests.get(rateCheckUrl)
+        if r.status_code == 200:
+            data = r.json()
+        return data['rateLimits']
+    except Exception as e:
+        print(f"Error occurred: {e}")
         
-def set_mb_search_key(v):
+def set_Metabase_Search_Key(v):
     cred.set_Key(Metabase_Search_Key=v)
-def mb_search_key(): 
-    '''
-    Uses mycred.json file to determine Metabase Search Key
-    '''
-    myMBkey = cred.get_Key('Metabase_Search_Key')
-    return myMBkey
 def get_time():
     '''
     returns the current minute
     '''
     return datetime.now().minute 
 class Article:
     '''
@@ -200,37 +199,40 @@
 def indexTerms(obj,*args):
     '''
     returns a dataframe of index terms
     accepts either an instance of Search, or an instance of Article.
     if Search is sent, df return is an aggregate count of the terms
     if Article is sent, df return is a dataframe of all index terms
     '''
-    if isinstance(obj, Search):
-        if obj.articles:
-            df=  pd.concat(
-                [
-                    pd.DataFrame.from_dict(article["indexTerms"], orient="columns")
-                    for article in obj.articles
-                ]
-            )
-            df['count'] = df.groupby(['name'])['domains'].transform('count')
-            df= df.drop(columns=['score','code'])
-            df = df.dropna()
-            df = df.drop_duplicates(['name'])
-            df = df.sort_values('count', ascending=False)
-        else:
-            print("no indexTerms to show!")
-    if isinstance(obj, Article):
-        indexterms_lst = obj.indexTerms
-        for x in indexterms_lst:
-            if not 'domains' in x:
-                x.remove(x)
-        df = pd.DataFrame.from_records(indexterms_lst)
-    ## Filter dataframe, if *args are provided
-    if args:
-        lst =[x.upper() for x in args]
-        df["INCLUDE"] = df["domains"].apply(lambda v: len(list(set(v).intersection(lst)) )!=0 )
-        df =  df[df['INCLUDE']].reset_index(drop=True)
-        del df['INCLUDE']
-        df
-    return df
+    try:
+        if isinstance(obj, Search):
+            if obj.articles:
+                df=  pd.concat(
+                    [
+                        pd.DataFrame.from_dict(article["indexTerms"], orient="columns")
+                        for article in obj.articles
+                    ]
+                )
+                df['count'] = df.groupby(['name'])['domains'].transform('count')
+                df= df.drop(columns=['score','code'])
+                df = df.dropna()
+                df = df.drop_duplicates(['name'])
+                df = df.sort_values('count', ascending=False)
+            else:
+                print("no indexTerms to show!")
+        if isinstance(obj, Article):
+            indexterms_lst = obj.indexTerms
+            for x in indexterms_lst:
+                if not 'domains' in x:
+                    x.remove(x)
+            df = pd.DataFrame.from_records(indexterms_lst)
+        ## Filter dataframe, if *args are provided
+        if args:
+            lst =[x.upper() for x in args]
+            df["INCLUDE"] = df["domains"].apply(lambda v: len(list(set(v).intersection(lst)) )!=0 )
+            df =  df[df['INCLUDE']].reset_index(drop=True)
+            del df['INCLUDE']
+            df
+        return df
+    except Exception as e:
+        print(f"Error occurred: {e}")
```

### Comparing `lexisnexisapi-2.0.49/src/lexisnexisapi.egg-info/PKG-INFO` & `lexisnexisapi-3.0/src/lexisnexisapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,181 +1,180 @@
-Metadata-Version: 2.1
-Name: lexisnexisapi
-Version: 2.0.49
-Summary: A module to support the lexisnexis metabase search api
-Home-page: 
-Author: Robert Cuffney
-Author-email: Robert Cuffney <robert.cuffney@lexisnexis.com>, Ozgur Aycan <ozgur.aycan@lexisnexis.co.uk>
-License: MIT
-Keywords: example project
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# Metabase.py Documentation
-
-## 1. Introduction
-
-### Overview
-
-The `metabase.py` module provides a Python interface to interact with the Metabase API. It allows you to perform searches and retrieve articles using the Metabase API. The module facilitates the creation of Python objects representing the API response, making it easy to work with the data.
-
-### Authors
-
-- Robert Cuffney
-- Ozgur Aycan
-- CS Integration Consultants @ LexisNexis
-
-### Version
-
-Current version: 2.0.49
-## 2. Installation
-
-### Dependencies
-
-To use the `metabase.py` module, you need the following dependencies:
-
-- requests
-- json
-- pandas
-- datetime
-- lexisnexisapi
-
-### Installation
-
-You can install the required dependencies using pip:
-
-```bash
-pip install requests pandas lexisnexisapi
-```
-
-## 3. Usage
-
-### Importing the Module
-
-To use the `metabase.py` module in your Python script, import it as follows:
-
-```python
-from lexisnexisapi import metabase
-```
-
-### Search Class
-
-The `Search` class is the main interface to perform searches and retrieve articles from Metabase. It has the following attributes and methods:
-
-#### Attributes:
-
-- `parameters`: A dictionary of Metabase search parameters.
-- `articles`: A list containing the articles retrieved from the Metabase API response.
-- `totalResults`: The total number of articles available in the search results.
-
-#### Methods:
-
-- `__init__(self, full_dataset=False, **kwargs)`: Initializes the Search object and performs the API request. If `full_dataset` is set to `True`, it retrieves all available articles by making multiple API calls.
-- `articles_dataframe(self, *args)`: Returns a Pandas DataFrame containing the articles' data. You can pass a list of desired fields (`*args`) to filter the DataFrame.
-- `create_file(self, file='articles.json')`: Creates a JSON file with the articles retrieved from the search.
-- `set_parameters(self, p)`: Sets the Metabase search parameters based on the input dictionary `p`.
-
-### Streamline Class
-
-The `Streamline` class helps maximize Metabase search calls without exceeding the rate limit. It keeps track of the remaining API calls per minute and waits for a new minute if needed.
-
-#### Attributes:
-
-- `key`: Metabase API key.
-- `start_minute`: The starting minute when the Streamline object is instantiated.
-- `minute_limit`: The maximum number of API calls allowed per minute based on the rate limit.
-- `calls_remaining`: The remaining API calls within the current minute.
-
-#### Methods:
-
-- `__init__(self, key)`: Initializes the Streamline object with the Metabase API key and fetches the rate limit information.
-- `track_calls(self)`: Updates the remaining API calls and waits for a new minute if the limit is reached.
-- `restart(self)`: Restarts the Streamline object.
-- `wait_for_new_min(self)`: Pauses execution until a new minute starts.
-- `get_current_minute(self)`: Returns the current minute as an integer.
-
-### Article Class
-
-The `Article` class represents an instance of a single article retrieved from Metabase. It sets each key from the article dictionary as an attribute of the class.
-
-### Helper Functions
-
-The module also provides some helper functions:
-
-- `http_request(p)`: Performs an HTTP request to the Metabase API with the given parameters `p` and returns the API response as a dictionary.
-- `rate_check(mbkey)`: Calls the Metabase rate limit API and returns the results as a list of dictionaries.
-- `set_mb_search_key(v)`: Sets the Metabase search key in the credentials.
-- `mb_search_key()`: Retrieves the Metabase search key from the credentials.
-- `get_time()`: Returns the current minute as an integer.
-
-## 4. Examples
-
-### Basic Search Example
-
-```python
-from lexisnexisapi import metabase
-
-# Set the Metabase search key (optional, you can set it in the parameters directly)
-metabase.set_mb_search_key("your_metabase_key")
-
-# Perform a basic search
-search = metabase.Search(query="your_query_here", limit=100)
-
-# Get the DataFrame of articles
-df = search.articles_dataframe("title", "author", "published_date")
-print(df.head())
-```
-
-### Full Dataset Search Example
-
-```python
-from lexisnexisapi import metabase
-
-# Set the Metabase search key (optional, you can set it in the parameters directly)
-metabase.set_mb_search_key("your_metabase_key")
-
-# Perform a full dataset search
-search = metabase.Search(full_dataset=True, query="your_query_here")
-
-# Create a JSON file with all the articles
-search.create_file("articles_full.json")
-```
-
-### Article Instance Example
-
-```python
-from lexisnexisapi  import metabase
-
-# Set the Metabase search key (optional, you can set it in the parameters directly)
-metabase.set_mb_search_key("your_metabase_key")
-
-# Perform a search and get an article instance
-search = metabase.Search(query="your_query_here", limit=1)
-article_instance = metabase.Article(search.articles[0])
-
-# Access attributes of the article instance
-print(article_instance.title)
-print(article_instance.author)
-print(article_instance.published_date)
-```
-
-### Index Terms Example
-
-```python
-from lexisnexisapi import metabase
-
-# Set the Metabase search key (optional, you can set it in the parameters directly)
-metabase.set_mb_search_key("your_metabase_key")
-
-# Perform a search
-search = metabase.Search(query="your_query_here", limit=100)
-
-# Get the DataFrame of index terms
-index_terms_df = metabase.indexTerms(search, "economy", "politics", "technology")
-print(index_terms_df.head())
-```
-
-Please note that you should replace `your_metabase_key` and `your_query_here` with your actual Metabase API key and desired search query, respectively, in the examples.
+Metadata-Version: 2.1
+Name: lexisnexisapi
+Version: 3.0
+Summary: A module to support the lexisnexis metabase search api
+Home-page: 
+Author: Robert Cuffney
+Author-email: Robert Cuffney <robert.cuffney@lexisnexis.com>, Ozgur Aycan <ozgur.aycan@lexisnexis.co.uk>
+License: MIT
+Keywords: example project
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Metabase.py Documentation
+
+## 1. Introduction
+
+### Overview
+
+The `metabase.py` module provides a Python interface to interact with the Metabase API. It allows you to perform searches and retrieve articles using the Metabase API. The module facilitates the creation of Python objects representing the API response, making it easy to work with the data.
+
+### Authors
+
+- Robert Cuffney
+- Ozgur Aycan
+- CS Integration Consultants @ LexisNexis
+
+### Version
+
+Current version: 3.0
+## 2. Installation
+
+### Dependencies
+
+To use the `metabase.py` module, you need the following dependencies:
+
+- requests
+- json
+- pandas
+- datetime
+- lexisnexisapi
+
+### Installation
+
+You can install the required dependencies using pip:
+
+```bash
+pip install requests pandas lexisnexisapi
+```
+
+## 3. Usage
+
+### Importing the Module
+
+To use the `metabase.py` module in your Python script, import it as follows:
+
+```python
+from lexisnexisapi import metabase
+```
+
+### Search Class
+
+The `Search` class is the main interface to perform searches and retrieve articles from Metabase. It has the following attributes and methods:
+
+#### Attributes:
+
+- `parameters`: A dictionary of Metabase search parameters.
+- `articles`: A list containing the articles retrieved from the Metabase API response.
+- `totalResults`: The total number of articles available in the search results.
+
+#### Methods:
+
+- `__init__(self, full_dataset=False, **kwargs)`: Initializes the Search object and performs the API request. If `full_dataset` is set to `True`, it retrieves all available articles by making multiple API calls.
+- `articles_dataframe(self, *args)`: Returns a Pandas DataFrame containing the articles' data. You can pass a list of desired fields (`*args`) to filter the DataFrame.
+- `create_file(self, file='articles.json')`: Creates a JSON file with the articles retrieved from the search.
+- `set_parameters(self, p)`: Sets the Metabase search parameters based on the input dictionary `p`.
+
+### Streamline Class
+
+The `Streamline` class helps maximize Metabase search calls without exceeding the rate limit. It keeps track of the remaining API calls per minute and waits for a new minute if needed.
+
+#### Attributes:
+
+- `key`: Metabase API key.
+- `start_minute`: The starting minute when the Streamline object is instantiated.
+- `minute_limit`: The maximum number of API calls allowed per minute based on the rate limit.
+- `calls_remaining`: The remaining API calls within the current minute.
+
+#### Methods:
+
+- `__init__(self, key)`: Initializes the Streamline object with the Metabase API key and fetches the rate limit information.
+- `track_calls(self)`: Updates the remaining API calls and waits for a new minute if the limit is reached.
+- `restart(self)`: Restarts the Streamline object.
+- `wait_for_new_min(self)`: Pauses execution until a new minute starts.
+- `get_current_minute(self)`: Returns the current minute as an integer.
+
+### Article Class
+
+The `Article` class represents an instance of a single article retrieved from Metabase. It sets each key from the article dictionary as an attribute of the class.
+
+### Helper Functions
+
+The module also provides some helper functions:
+
+- `http_request(p)`: Performs an HTTP request to the Metabase API with the given parameters `p` and returns the API response as a dictionary.
+- `rate_check(mbkey)`: Calls the Metabase rate limit API and returns the results as a list of dictionaries.
+- `set_Metabase_Search_Key(v)`: Sets the Metabase search key in the credentials.
+- `get_time()`: Returns the current minute as an integer.
+
+## 4. Examples
+
+### Basic Search Example
+
+```python
+from lexisnexisapi import metabase
+
+# Set the Metabase search key (optional, you can set it in the parameters directly)
+metabase.set_mb_search_key("your_metabase_key")
+
+# Perform a basic search
+search = metabase.Search(query="your_query_here", limit=100)
+
+# Get the DataFrame of articles
+df = search.articles_dataframe("title", "author", "published_date")
+print(df.head())
+```
+
+### Full Dataset Search Example
+
+```python
+from lexisnexisapi import metabase
+
+# Set the Metabase search key (optional, you can set it in the parameters directly)
+metabase.set_mb_search_key("your_metabase_key")
+
+# Perform a full dataset search
+search = metabase.Search(full_dataset=True, query="your_query_here")
+
+# Create a JSON file with all the articles
+search.create_file("articles_full.json")
+```
+
+### Article Instance Example
+
+```python
+from lexisnexisapi  import metabase
+
+# Set the Metabase search key (optional, you can set it in the parameters directly)
+metabase.set_mb_search_key("your_metabase_key")
+
+# Perform a search and get an article instance
+search = metabase.Search(query="your_query_here", limit=1)
+article_instance = metabase.Article(search.articles[0])
+
+# Access attributes of the article instance
+print(article_instance.title)
+print(article_instance.author)
+print(article_instance.published_date)
+```
+
+### Index Terms Example
+
+```python
+from lexisnexisapi import metabase
+
+# Set the Metabase search key (optional, you can set it in the parameters directly)
+metabase.set_mb_search_key("your_metabase_key")
+
+# Perform a search
+search = metabase.Search(query="your_query_here", limit=100)
+
+# Get the DataFrame of index terms
+index_terms_df = metabase.indexTerms(search, "economy", "politics", "technology")
+print(index_terms_df.head())
+```
+
+Please note that you should replace `your_metabase_key` and `your_query_here` with your actual Metabase API key and desired search query, respectively, in the examples.
```

