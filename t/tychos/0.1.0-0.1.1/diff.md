# Comparing `tmp/tychos-0.1.0.tar.gz` & `tmp/tychos-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tychos-0.1.0.tar", last modified: Wed Jul 19 15:32:07 2023, max compression
+gzip compressed data, was "tychos-0.1.1.tar", last modified: Thu Aug  3 16:18:17 2023, max compression
```

## Comparing `tychos-0.1.0.tar` & `tychos-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-19 15:32:07.727715 tychos-0.1.0/
--rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.1.0/LICENSE
--rw-r--r--   0 abe732     (501) staff       (20)     2694 2023-07-19 15:32:07.727381 tychos-0.1.0/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)     2507 2023-07-19 15:30:24.000000 tychos-0.1.0/README.md
--rw-r--r--   0 abe732     (501) staff       (20)       38 2023-07-19 15:32:07.727781 tychos-0.1.0/setup.cfg
--rw-r--r--   0 abe732     (501) staff       (20)      502 2023-07-19 15:29:30.000000 tychos-0.1.0/setup.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-19 15:32:07.722829 tychos-0.1.0/tychos/
--rw-r--r--   0 abe732     (501) staff       (20)      276 2023-07-10 18:55:06.000000 tychos-0.1.0/tychos/__init__.py
--rw-r--r--   0 abe732     (501) staff       (20)     1092 2023-07-10 19:02:06.000000 tychos-0.1.0/tychos/cli.py
--rw-r--r--   0 abe732     (501) staff       (20)      213 2023-07-10 18:12:08.000000 tychos-0.1.0/tychos/config.py
--rw-r--r--   0 abe732     (501) staff       (20)     1497 2023-07-19 15:29:14.000000 tychos-0.1.0/tychos/vector.py
--rw-r--r--   0 abe732     (501) staff       (20)     1695 2023-07-19 15:28:59.000000 tychos-0.1.0/tychos/vector_data_store.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-19 15:32:07.725728 tychos-0.1.0/tychos.egg-info/
--rw-r--r--   0 abe732     (501) staff       (20)     2694 2023-07-19 15:32:07.000000 tychos-0.1.0/tychos.egg-info/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)      303 2023-07-19 15:32:07.000000 tychos-0.1.0/tychos.egg-info/SOURCES.txt
--rw-r--r--   0 abe732     (501) staff       (20)        1 2023-07-19 15:32:07.000000 tychos-0.1.0/tychos.egg-info/dependency_links.txt
--rw-r--r--   0 abe732     (501) staff       (20)       47 2023-07-19 15:32:07.000000 tychos-0.1.0/tychos.egg-info/entry_points.txt
--rw-r--r--   0 abe732     (501) staff       (20)        9 2023-07-19 15:32:07.000000 tychos-0.1.0/tychos.egg-info/requires.txt
--rw-r--r--   0 abe732     (501) staff       (20)        7 2023-07-19 15:32:07.000000 tychos-0.1.0/tychos.egg-info/top_level.txt
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-08-03 16:18:17.279374 tychos-0.1.1/
+-rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-07-19 15:35:45.000000 tychos-0.1.1/LICENSE
+-rw-r--r--   0 abe732     (501) staff       (20)     3447 2023-08-03 16:18:17.279193 tychos-0.1.1/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)     3259 2023-08-03 16:15:53.000000 tychos-0.1.1/README.md
+-rw-r--r--   0 abe732     (501) staff       (20)       38 2023-08-03 16:18:17.279422 tychos-0.1.1/setup.cfg
+-rw-r--r--   0 abe732     (501) staff       (20)      502 2023-08-03 16:17:44.000000 tychos-0.1.1/setup.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-08-03 16:18:17.277768 tychos-0.1.1/tychos/
+-rw-r--r--   0 abe732     (501) staff       (20)      276 2023-07-10 18:55:06.000000 tychos-0.1.1/tychos/__init__.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1092 2023-07-10 19:02:06.000000 tychos-0.1.1/tychos/cli.py
+-rw-r--r--   0 abe732     (501) staff       (20)      213 2023-07-10 18:12:08.000000 tychos-0.1.1/tychos/config.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1497 2023-08-03 15:53:19.000000 tychos-0.1.1/tychos/vector.py
+-rw-r--r--   0 abe732     (501) staff       (20)     2117 2023-08-03 15:58:24.000000 tychos-0.1.1/tychos/vector_data_store.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-08-03 16:18:17.278960 tychos-0.1.1/tychos.egg-info/
+-rw-r--r--   0 abe732     (501) staff       (20)     3447 2023-08-03 16:18:17.000000 tychos-0.1.1/tychos.egg-info/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)      303 2023-08-03 16:18:17.000000 tychos-0.1.1/tychos.egg-info/SOURCES.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        1 2023-08-03 16:18:17.000000 tychos-0.1.1/tychos.egg-info/dependency_links.txt
+-rw-r--r--   0 abe732     (501) staff       (20)       47 2023-08-03 16:18:17.000000 tychos-0.1.1/tychos.egg-info/entry_points.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        9 2023-08-03 16:18:17.000000 tychos-0.1.1/tychos.egg-info/requires.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        7 2023-08-03 16:18:17.000000 tychos-0.1.1/tychos.egg-info/top_level.txt
```

### Comparing `tychos-0.1.0/LICENSE` & `tychos-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tychos-0.1.0/PKG-INFO` & `tychos-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tychos
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python client library for the Tychos API.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
@@ -48,41 +48,51 @@
 ```
 
 Query live vector datasets
 ```python
 # initialize data store
 data_store = tychos.VectorDataStore()
 
-# query the data store object
+# query a single dataset from the data store object
 query_results = data_store.query(
-    index_name = "pub-med-abstracts", # dataset
+    name = "pub-med-abstracts", # dataset index can be a string or an array
     query_string = "What is the latest research on molecular peptides", # search string
     limit = 5, # number of results
 )
 
+# query multiple datasets and return the global top results
+query_results = data_store.query(
+    name = ["arxiv-abstracts", "pub-med-abstracts"], # dataset index can be a string or an array
+    query_string = "What is the latest research on molecular peptides", # search string
+    limit = 5, # number of results (across all datasets queried)
+)
+
 # print the metadata associated with the first result
 print(query_results[0]['payload'])
 ```
 
 ## Command-line interface
 This library additionally provides a tychos command-line utility to make it easy to interact with the API from your terminal. Run tychos-cli -h for usage.
 
 ```sh
 tychos-cli query --api-key <YOUR-API-KEY> --name pub-med-abstracts --query-string <"Your query string"> --limit 5
 
 ```
 
 ## Datasets available
-We currently support the PubMed dataset and have plans to add additional sources in the coming weeks. If there's a particular dataset you'd like to incorporate into your LLM application, feel free to [reach out][twitter].
+We currently support the full PubMed and ArXiv datasets and have plans to add additional sources in the coming weeks. If there's a particular dataset you'd like to incorporate into your LLM application, feel free to [reach out][twitter] or raise a GitHub issue.
 
 ### Vector datasets
--   PubMed abstracts ([source][pub-med]): 33.8M documents, updated daily at 07:00 UTC.
-
+| Dataset | Name | Size | Update Cadence | Update Time |
+| --------------- | --------------- | --------------- | --------------- | --------------- |
+| PubMed Abstracts ([source][pub-med]) | pub-med-abstracts | 35.5M documents | Daily | 07:00 UTC |
+| Arxiv Abstracts ([source][arxiv]) | arxiv-abstracts | 2.3M documents | Weekly | 07:00 UTC on Sunday|
 
 
 ## Feedback and support
-If you'd like to provide feedback, run into issues, or need support using embeddings, feel free to [reach out][twitter] or raise an issue via GitHub.
+If you'd like to provide feedback, run into issues, or need support using embeddings, feel free to [reach out][twitter] or raise a GitHub issue.
 
 
 [api-keys]: https://tychos.ai/
 [twitter]: https://twitter.com/etpuisfume
 [pub-med]: https://pubmed.ncbi.nlm.nih.gov/download/
+[arxiv]: https://info.arxiv.org/help/bulk_data/index.html
```

### Comparing `tychos-0.1.0/README.md` & `tychos-0.1.1/tychos.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: tychos
+Version: 0.1.1
+Summary: Python client library for the Tychos API.
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
 applications written in the Python language. The Tychos API allows you to query live, hosted vector datasets in your LLM application without needing to manage your own vector database / embedding pipelines.
 
 To see the Tychos API in action, you can test out our [PubMed Demo App](https://tychos.ai/demo).
 
 ## Installation
@@ -40,41 +48,51 @@
 ```
 
 Query live vector datasets
 ```python
 # initialize data store
 data_store = tychos.VectorDataStore()
 
-# query the data store object
+# query a single dataset from the data store object
 query_results = data_store.query(
-    index_name = "pub-med-abstracts", # dataset
+    name = "pub-med-abstracts", # dataset index can be a string or an array
     query_string = "What is the latest research on molecular peptides", # search string
     limit = 5, # number of results
 )
 
+# query multiple datasets and return the global top results
+query_results = data_store.query(
+    name = ["arxiv-abstracts", "pub-med-abstracts"], # dataset index can be a string or an array
+    query_string = "What is the latest research on molecular peptides", # search string
+    limit = 5, # number of results (across all datasets queried)
+)
+
 # print the metadata associated with the first result
 print(query_results[0]['payload'])
 ```
 
 ## Command-line interface
 This library additionally provides a tychos command-line utility to make it easy to interact with the API from your terminal. Run tychos-cli -h for usage.
 
 ```sh
 tychos-cli query --api-key <YOUR-API-KEY> --name pub-med-abstracts --query-string <"Your query string"> --limit 5
 
 ```
 
 ## Datasets available
-We currently support the PubMed dataset and have plans to add additional sources in the coming weeks. If there's a particular dataset you'd like to incorporate into your LLM application, feel free to [reach out][twitter].
+We currently support the full PubMed and ArXiv datasets and have plans to add additional sources in the coming weeks. If there's a particular dataset you'd like to incorporate into your LLM application, feel free to [reach out][twitter] or raise a GitHub issue.
 
 ### Vector datasets
--   PubMed abstracts ([source][pub-med]): 33.8M documents, updated daily at 07:00 UTC.
-
+| Dataset | Name | Size | Update Cadence | Update Time |
+| --------------- | --------------- | --------------- | --------------- | --------------- |
+| PubMed Abstracts ([source][pub-med]) | pub-med-abstracts | 35.5M documents | Daily | 07:00 UTC |
+| Arxiv Abstracts ([source][arxiv]) | arxiv-abstracts | 2.3M documents | Weekly | 07:00 UTC on Sunday|
 
 
 ## Feedback and support
-If you'd like to provide feedback, run into issues, or need support using embeddings, feel free to [reach out][twitter] or raise an issue via GitHub.
+If you'd like to provide feedback, run into issues, or need support using embeddings, feel free to [reach out][twitter] or raise a GitHub issue.
 
 
 [api-keys]: https://tychos.ai/
 [twitter]: https://twitter.com/etpuisfume
 [pub-med]: https://pubmed.ncbi.nlm.nih.gov/download/
+[arxiv]: https://info.arxiv.org/help/bulk_data/index.html
```

### Comparing `tychos-0.1.0/tychos/cli.py` & `tychos-0.1.1/tychos/cli.py`

 * *Files identical despite different names*

### Comparing `tychos-0.1.0/tychos/vector.py` & `tychos-0.1.1/tychos/vector.py`

 * *Files identical despite different names*

### Comparing `tychos-0.1.0/tychos/vector_data_store.py` & `tychos-0.1.1/tychos/vector_data_store.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,14 +14,22 @@
         # vectorize query string
         query_vector = self.vector.create(
             type="text_embedding",
             input_text=query_string,
             model="text-embedding-ada-002"
         )
 
+        # validate index name
+        available_indices = ['pub-med-abstracts', 'arxiv-abstracts']
+        if not isinstance(name, list):
+            name = [name]
+        invalid_names = [n for n in name if n not in available_indices]
+        if invalid_names:
+            raise ValueError(f"Invalid index name(s): {', '.join(invalid_names)}. The current available datasets are: {', '.join(available_indices)}")
+        
         # send query request to vector data store
         url = f'{self.base_url}vector_data_store/query'
         headers = {'api_key': self.api_key}
         payload = {
                     'name': name,
                     'query_vector': query_vector,
                     'top': limit,
```

### Comparing `tychos-0.1.0/tychos.egg-info/PKG-INFO` & `tychos-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: tychos
-Version: 0.1.0
-Summary: Python client library for the Tychos API.
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
 applications written in the Python language. The Tychos API allows you to query live, hosted vector datasets in your LLM application without needing to manage your own vector database / embedding pipelines.
 
 To see the Tychos API in action, you can test out our [PubMed Demo App](https://tychos.ai/demo).
 
 ## Installation
@@ -48,41 +40,51 @@
 ```
 
 Query live vector datasets
 ```python
 # initialize data store
 data_store = tychos.VectorDataStore()
 
-# query the data store object
+# query a single dataset from the data store object
 query_results = data_store.query(
-    index_name = "pub-med-abstracts", # dataset
+    name = "pub-med-abstracts", # dataset index can be a string or an array
     query_string = "What is the latest research on molecular peptides", # search string
     limit = 5, # number of results
 )
 
+# query multiple datasets and return the global top results
+query_results = data_store.query(
+    name = ["arxiv-abstracts", "pub-med-abstracts"], # dataset index can be a string or an array
+    query_string = "What is the latest research on molecular peptides", # search string
+    limit = 5, # number of results (across all datasets queried)
+)
+
 # print the metadata associated with the first result
 print(query_results[0]['payload'])
 ```
 
 ## Command-line interface
 This library additionally provides a tychos command-line utility to make it easy to interact with the API from your terminal. Run tychos-cli -h for usage.
 
 ```sh
 tychos-cli query --api-key <YOUR-API-KEY> --name pub-med-abstracts --query-string <"Your query string"> --limit 5
 
 ```
 
 ## Datasets available
-We currently support the PubMed dataset and have plans to add additional sources in the coming weeks. If there's a particular dataset you'd like to incorporate into your LLM application, feel free to [reach out][twitter].
+We currently support the full PubMed and ArXiv datasets and have plans to add additional sources in the coming weeks. If there's a particular dataset you'd like to incorporate into your LLM application, feel free to [reach out][twitter] or raise a GitHub issue.
 
 ### Vector datasets
--   PubMed abstracts ([source][pub-med]): 33.8M documents, updated daily at 07:00 UTC.
-
+| Dataset | Name | Size | Update Cadence | Update Time |
+| --------------- | --------------- | --------------- | --------------- | --------------- |
+| PubMed Abstracts ([source][pub-med]) | pub-med-abstracts | 35.5M documents | Daily | 07:00 UTC |
+| Arxiv Abstracts ([source][arxiv]) | arxiv-abstracts | 2.3M documents | Weekly | 07:00 UTC on Sunday|
 
 
 ## Feedback and support
-If you'd like to provide feedback, run into issues, or need support using embeddings, feel free to [reach out][twitter] or raise an issue via GitHub.
+If you'd like to provide feedback, run into issues, or need support using embeddings, feel free to [reach out][twitter] or raise a GitHub issue.
 
 
 [api-keys]: https://tychos.ai/
 [twitter]: https://twitter.com/etpuisfume
 [pub-med]: https://pubmed.ncbi.nlm.nih.gov/download/
+[arxiv]: https://info.arxiv.org/help/bulk_data/index.html
```

