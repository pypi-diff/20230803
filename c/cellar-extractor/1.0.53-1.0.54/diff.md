# Comparing `tmp/cellar_extractor-1.0.53.tar.gz` & `tmp/cellar_extractor-1.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellar_extractor-1.0.53.tar", last modified: Sat Jul 15 13:25:18 2023, max compression
+gzip compressed data, was "cellar_extractor-1.0.54.tar", last modified: Thu Aug  3 09:59:11 2023, max compression
```

## Comparing `cellar_extractor-1.0.53.tar` & `cellar_extractor-1.0.54.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 13:25:18.291472 cellar_extractor-1.0.53/
--rw-rw-rw-   0        0        0     6921 2023-07-15 13:25:18.290471 cellar_extractor-1.0.53/PKG-INFO
--rw-rw-rw-   0        0        0     6474 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 13:25:18.280472 cellar_extractor-1.0.53/cellar_extractor/
--rw-rw-rw-   0        0        0      704 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/Testing_file.py
--rw-rw-rw-   0        0        0      163 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/__init__.py
--rw-rw-rw-   0        0        0     3329 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/cellar.py
--rw-rw-rw-   0        0        0     1005 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/cellar_extra_extract.py
--rw-rw-rw-   0        0        0     5227 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/cellar_queries.py
--rw-rw-rw-   0        0        0    11308 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/citations_adder.py
--rw-rw-rw-   0        0        0     1334 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/csv_extractor.py
--rw-rw-rw-   0        0        0    16726 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/eurlex_scraping.py
--rw-rw-rw-   0        0        0     6477 2023-07-15 13:25:06.000000 cellar_extractor-1.0.53/cellar_extractor/fulltext_saving.py
--rw-rw-rw-   0        0        0     5411 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/json_to_csv.py
--rw-rw-rw-   0        0        0     1040 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/nodes_and_edges.py
--rw-rw-rw-   0        0        0     6834 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/sparql.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:25:18.288470 cellar_extractor-1.0.53/cellar_extractor.egg-info/
--rw-rw-rw-   0        0        0     6921 2023-07-15 13:25:18.000000 cellar_extractor-1.0.53/cellar_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-07-15 13:25:18.000000 cellar_extractor-1.0.53/cellar_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 13:25:18.000000 cellar_extractor-1.0.53/cellar_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-07-15 13:25:18.000000 cellar_extractor-1.0.53/cellar_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-15 13:25:18.000000 cellar_extractor-1.0.53/cellar_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 13:25:18.291472 cellar_extractor-1.0.53/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-07-15 13:25:13.000000 cellar_extractor-1.0.53/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 09:59:11.310483 cellar_extractor-1.0.54/
+-rw-rw-rw-   0        0        0     7505 2023-08-03 09:59:11.309480 cellar_extractor-1.0.54/PKG-INFO
+-rw-rw-rw-   0        0        0     7058 2023-08-03 09:57:16.000000 cellar_extractor-1.0.54/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 09:59:11.299971 cellar_extractor-1.0.54/cellar_extractor/
+-rw-rw-rw-   0        0        0      709 2023-08-03 09:56:02.000000 cellar_extractor-1.0.54/cellar_extractor/Testing_file.py
+-rw-rw-rw-   0        0        0      224 2023-08-03 09:50:44.000000 cellar_extractor-1.0.54/cellar_extractor/__init__.py
+-rw-rw-rw-   0        0        0     3694 2023-08-03 09:58:14.000000 cellar_extractor-1.0.54/cellar_extractor/cellar.py
+-rw-rw-rw-   0        0        0     1005 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/cellar_extra_extract.py
+-rw-rw-rw-   0        0        0     5227 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/cellar_queries.py
+-rw-rw-rw-   0        0        0    11308 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/citations_adder.py
+-rw-rw-rw-   0        0        0     1355 2023-08-02 12:06:01.000000 cellar_extractor-1.0.54/cellar_extractor/csv_extractor.py
+-rw-rw-rw-   0        0        0    16726 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/eurlex_scraping.py
+-rw-rw-rw-   0        0        0     6477 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/fulltext_saving.py
+-rw-rw-rw-   0        0        0     5411 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/json_to_csv.py
+-rw-rw-rw-   0        0        0     1040 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/nodes_and_edges.py
+-rw-rw-rw-   0        0        0     6834 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/sparql.py
+drwxrwxrwx   0        0        0        0 2023-08-03 09:59:11.308483 cellar_extractor-1.0.54/cellar_extractor.egg-info/
+-rw-rw-rw-   0        0        0     7505 2023-08-03 09:59:11.000000 cellar_extractor-1.0.54/cellar_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-08-03 09:59:11.000000 cellar_extractor-1.0.54/cellar_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 09:59:11.000000 cellar_extractor-1.0.54/cellar_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-08-03 09:59:11.000000 cellar_extractor-1.0.54/cellar_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-03 09:59:11.000000 cellar_extractor-1.0.54/cellar_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 09:59:11.311480 cellar_extractor-1.0.54/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-08-03 09:58:14.000000 cellar_extractor-1.0.54/setup.py
```

### Comparing `cellar_extractor-1.0.53/PKG-INFO` & `cellar_extractor-1.0.54/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellar_extractor
-Version: 1.0.53
+Version: 1.0.54
 Summary: Library for extracting cellar data
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor
@@ -65,14 +65,16 @@
     Gets all the ECLI data from the eurlex sparql endpoint, and on top of that scrapes the eurlex websites to acquire 
     the full text, keywords, case law directory code and eurovoc identifiers. If the user does have an eurlex account with access to the eurlex webservices, he can also 
     pass his webservices login credentials to the method, in order to extract data about works citing work and works 
     being cited by work. The full text is returned as a JSON file, rest of data as a CSV.  Can be in-memory or as saved files.
     <li><code>get_nodes_and_edges_lists</code></li>
     Gets 2 list objects, one for the nodes and edges of the citations within the passed dataframe.
     Allows the creation of a network graph of the citations. Can only be returned in-memory.
+    <li><code>filter_subject_matter</code></li>
+    Returns a dataframe of cases only containing a certain phrase in the column containing the subject of cases.
     <br>
 </ol>
 
 ## What are the parameters?
 <ol>
     <li><code>get_cellar</code></li>
     <strong>Parameters:</strong>
@@ -111,14 +113,21 @@
     </ul>
     <li><code>get_nodes_and_edges_lists</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
         DataFrame of cellar metadata acquired from the get_cellar_extra method with eurlex webservice credentials passed.
         This method will only work on dataframes with citations data.
     </ul>
+    <li><code>filter_subject_matter</code></li>
+    <ul>
+        <li><strong>df: DataFrame object, required, default None</strong></li>
+        DataFrame of cellar metadata acquired from any of the cellar extraction methods listed above.
+        <li><strong>phrase: string, required, default None</strong></li>
+        The phrase which has to be present in the subject matter of cases. Case insensitive.
+    </ul>
 </ol>
 
 
 ## Examples
 ```
 import cellar_extractor as cell
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.53 Summary: Library
+Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.54 Summary: Library
 for extracting cellar data Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Description-Content-Type: text/markdown ## Cellar
 extractor This library contains two functions to get cellar case law data from
 eurlex. ## Version Python 3.9 ## Contributors
@@ -21,14 +21,17 @@
       about works citing work and works being cited by work. The full text is
       returned as a JSON file, rest of data as a CSV. Can be in-memory or as
       saved files.
    5. get_nodes_and_edges_lists
    6. Gets 2 list objects, one for the nodes and edges of the citations within
       the passed dataframe. Allows the creation of a network graph of the
       citations. Can only be returned in-memory.
+   7. filter_subject_matter
+   8. Returns a dataframe of cases only containing a certain phrase in the
+      column containing the subject of cases.
 ## What are the parameters?
    1. get_cellar
    2. Parameters:
           o max_ecli: int, optional, default 100
           o Maximum number of ECLIs to retrieve.
           o sd: date, optional, default '2022-05-01'
           o The start last modification date (yyyy-mm-dd).
@@ -61,14 +64,21 @@
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
    4. get_nodes_and_edges_lists
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from the get_cellar_extra
             method with eurlex webservice credentials passed. This method will
             only work on dataframes with citations data.
+   5. filter_subject_matter
+          o df: DataFrame object, required, default None
+          o DataFrame of cellar metadata acquired from any of the cellar
+            extraction methods listed above.
+          o phrase: string, required, default None
+          o The phrase which has to be present in the subject matter of cases.
+            Case insensitive.
 ## Examples ``` import cellar_extractor as cell Below are examples for in-file
 saving: cell.get_cellar(save_file='y', max_ecli=200, sd='2022-01-01',
 file_format='csv') cell.get_cellar_extra(max_ecli=100, sd='2022-01-01',
 threads=10) Below are examples for in-memory saving: df = cell.get_cellar
 (save_file='n', file_format='csv', sd='2022-01-01', max_ecli=1000) df,json =
 cell.get_cellar_extra(save_file='n', max_ecli=100, sd='2022-01-01', threads=10)
 ``` ## License [![License: Apache 2.0](https://img.shields.io/github/license/
```

### Comparing `cellar_extractor-1.0.53/README.md` & `cellar_extractor-1.0.54/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     Gets all the ECLI data from the eurlex sparql endpoint, and on top of that scrapes the eurlex websites to acquire 
     the full text, keywords, case law directory code and eurovoc identifiers. If the user does have an eurlex account with access to the eurlex webservices, he can also 
     pass his webservices login credentials to the method, in order to extract data about works citing work and works 
     being cited by work. The full text is returned as a JSON file, rest of data as a CSV.  Can be in-memory or as saved files.
     <li><code>get_nodes_and_edges_lists</code></li>
     Gets 2 list objects, one for the nodes and edges of the citations within the passed dataframe.
     Allows the creation of a network graph of the citations. Can only be returned in-memory.
+    <li><code>filter_subject_matter</code></li>
+    Returns a dataframe of cases only containing a certain phrase in the column containing the subject of cases.
     <br>
 </ol>
 
 ## What are the parameters?
 <ol>
     <li><code>get_cellar</code></li>
     <strong>Parameters:</strong>
@@ -99,14 +101,21 @@
     </ul>
     <li><code>get_nodes_and_edges_lists</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
         DataFrame of cellar metadata acquired from the get_cellar_extra method with eurlex webservice credentials passed.
         This method will only work on dataframes with citations data.
     </ul>
+    <li><code>filter_subject_matter</code></li>
+    <ul>
+        <li><strong>df: DataFrame object, required, default None</strong></li>
+        DataFrame of cellar metadata acquired from any of the cellar extraction methods listed above.
+        <li><strong>phrase: string, required, default None</strong></li>
+        The phrase which has to be present in the subject matter of cases. Case insensitive.
+    </ul>
 </ol>
 
 
 ## Examples
 ```
 import cellar_extractor as cell
```

#### html2text {}

```diff
@@ -15,14 +15,17 @@
       about works citing work and works being cited by work. The full text is
       returned as a JSON file, rest of data as a CSV. Can be in-memory or as
       saved files.
    5. get_nodes_and_edges_lists
    6. Gets 2 list objects, one for the nodes and edges of the citations within
       the passed dataframe. Allows the creation of a network graph of the
       citations. Can only be returned in-memory.
+   7. filter_subject_matter
+   8. Returns a dataframe of cases only containing a certain phrase in the
+      column containing the subject of cases.
 ## What are the parameters?
    1. get_cellar
    2. Parameters:
           o max_ecli: int, optional, default 100
           o Maximum number of ECLIs to retrieve.
           o sd: date, optional, default '2022-05-01'
           o The start last modification date (yyyy-mm-dd).
@@ -55,14 +58,21 @@
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
    4. get_nodes_and_edges_lists
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from the get_cellar_extra
             method with eurlex webservice credentials passed. This method will
             only work on dataframes with citations data.
+   5. filter_subject_matter
+          o df: DataFrame object, required, default None
+          o DataFrame of cellar metadata acquired from any of the cellar
+            extraction methods listed above.
+          o phrase: string, required, default None
+          o The phrase which has to be present in the subject matter of cases.
+            Case insensitive.
 ## Examples ``` import cellar_extractor as cell Below are examples for in-file
 saving: cell.get_cellar(save_file='y', max_ecli=200, sd='2022-01-01',
 file_format='csv') cell.get_cellar_extra(max_ecli=100, sd='2022-01-01',
 threads=10) Below are examples for in-memory saving: df = cell.get_cellar
 (save_file='n', file_format='csv', sd='2022-01-01', max_ecli=1000) df,json =
 cell.get_cellar_extra(save_file='n', max_ecli=100, sd='2022-01-01', threads=10)
 ``` ## License [![License: Apache 2.0](https://img.shields.io/github/license/
```

### Comparing `cellar_extractor-1.0.53/cellar_extractor/Testing_file.py` & `cellar_extractor-1.0.54/cellar_extractor/Testing_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,9 +21,10 @@
 if __name__ == '__main__':
    celex = "62004CJ0292"
    site = get_entire_page(celex)
    text = get_full_text_from_html(site)
    cits = get_citations_with_extra_info(text)
    print(cits)
    data,d2 = get_cellar_extra(sd='2023-01-01',max_ecli=100,save_file='n')
-   nodes_edges = get_nodes_and_edges_lists(data)
+   d3 = filter_subject_matter(data, "prices")
+   b=2
    pass
```

### Comparing `cellar_extractor-1.0.53/cellar_extractor/cellar.py` & `cellar_extractor-1.0.54/cellar_extractor/cellar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import json
 import os
-from os.path import join
+import time
 from datetime import datetime
 from pathlib import Path
+
 from tqdm import tqdm
+
+from cellar_extractor.cellar_extra_extract import extra_cellar
 from cellar_extractor.cellar_queries import get_all_eclis, get_raw_cellar_metadata
 from cellar_extractor.json_to_csv import json_to_csv_main, json_to_csv_returning
-from cellar_extractor.cellar_extra_extract import extra_cellar
 from cellar_extractor.nodes_and_edges import get_nodes_and_edges
-import time
+
 
 def get_cellar(ed=None, save_file='y', max_ecli=100, sd="2022-05-01", file_format='csv'):
     if not ed:
         ed = datetime.now().isoformat(timespec='seconds')
     file_name = 'cellar_' + sd + '_' + ed
     file_name = file_name.replace(":", "_")
     print('\n--- PREPARATION ---\n')
@@ -24,15 +26,15 @@
     if len(eclis) > max_ecli:
         eclis = eclis[:max_ecli]
     if len(eclis) == 0:
         print(f"No data to download found between {sd} and {ed}")
         return False
     all_eclis = {}
     concurrent_docs = 100
-    for i in tqdm(range(0, len(eclis), concurrent_docs),colour="GREEN"):
+    for i in tqdm(range(0, len(eclis), concurrent_docs), colour="GREEN"):
         new_eclis = get_raw_cellar_metadata(eclis[i:(i + concurrent_docs)])
         all_eclis = {**all_eclis, **new_eclis}
     if save_file == 'y':
         Path('data').mkdir(parents=True, exist_ok=True)
         if file_format == 'csv':
             file_path = os.path.join('data', file_name + '.csv')
             json_to_csv_main(all_eclis, file_path)
@@ -58,27 +60,39 @@
         return False, False
     print("\n--- START OF EXTRA EXTRACTION ---")
     file_name = 'cellar_extra_' + sd + '_' + ed
     file_name = file_name.replace(":", "_")
     file_path = os.path.join('data', file_name + '.csv')
     if save_file == 'y':
         Path('data').mkdir(parents=True, exist_ok=True)
-        extra_cellar(data = data ,filepath=file_path, threads=threads, username=username, password=password)
+        extra_cellar(data=data, filepath=file_path, threads=threads, username=username, password=password)
         print("\n--- DONE ---")
 
     else:
-        data,json = extra_cellar(data= data, threads = threads, username= username,password=password)
+        data, json = extra_cellar(data=data, threads=threads, username=username, password=password)
         print("\n--- DONE ---")
 
-        return data,json
+        return data, json
 
-def get_nodes_and_edges_lists(df = None):
+
+def get_nodes_and_edges_lists(df=None):
     if df is None:
         print("No dataframe passed!")
         return
     else:
         try:
-            nodes,edges = get_nodes_and_edges(df)
+            nodes, edges = get_nodes_and_edges(df)
         except:
             print('Something went wrong. Nodes and edges creation unsuccessful.')
-            return False,False
-        return nodes,edges
+            return False, False
+        return nodes, edges
+
+
+def filter_subject_matter(df=None, phrase=None):
+    if df is None or phrase is None:
+        print("Incorrect input values! \n Returning... \n")
+    else:
+        try:
+            mask = df["LEGAL RESOURCE IS ABOUT SUBJECT MATTER"].str.lower().str.contains(phrase)
+            return df[mask]
+        except:
+            print("Something went wrong!\n Returning... \n")
```

### Comparing `cellar_extractor-1.0.53/cellar_extractor/cellar_extra_extract.py` & `cellar_extractor-1.0.54/cellar_extractor/cellar_extra_extract.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.53/cellar_extractor/cellar_queries.py` & `cellar_extractor-1.0.54/cellar_extractor/cellar_queries.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.53/cellar_extractor/citations_adder.py` & `cellar_extractor-1.0.54/cellar_extractor/citations_adder.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.53/cellar_extractor/csv_extractor.py` & `cellar_extractor-1.0.54/cellar_extractor/csv_extractor.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     parser = argparse.ArgumentParser()
     parser.add_argument('--amount', help='number of rows to extract', type=int, required=True)
     args = parser.parse_args()
     number = args.amount
     print("")
     print("EXTRACTION FROM CSV FILE IN DATA PROCESSED DIR STARTED")
     print("")
+    DIR_DATA_RAW=''
     csv_files = (glob.glob(DIR_DATA_RAW + "/" + "*.csv"))
     print(f"FOUND {len(csv_files)} CSV FILES")
 
     for i in range(len(csv_files)):
         # Approach for manual extraction of a specific file in a specific directory
         if "clean" not in csv_files[i]:
             print("")
```

### Comparing `cellar_extractor-1.0.53/cellar_extractor/eurlex_scraping.py` & `cellar_extractor-1.0.54/cellar_extractor/eurlex_scraping.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.53/cellar_extractor/fulltext_saving.py` & `cellar_extractor-1.0.54/cellar_extractor/fulltext_saving.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.53/cellar_extractor/json_to_csv.py` & `cellar_extractor-1.0.54/cellar_extractor/json_to_csv.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.53/cellar_extractor/nodes_and_edges.py` & `cellar_extractor-1.0.54/cellar_extractor/nodes_and_edges.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.53/cellar_extractor/sparql.py` & `cellar_extractor-1.0.54/cellar_extractor/sparql.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.53/cellar_extractor.egg-info/PKG-INFO` & `cellar_extractor-1.0.54/cellar_extractor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellar-extractor
-Version: 1.0.53
+Version: 1.0.54
 Summary: Library for extracting cellar data
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor
@@ -65,14 +65,16 @@
     Gets all the ECLI data from the eurlex sparql endpoint, and on top of that scrapes the eurlex websites to acquire 
     the full text, keywords, case law directory code and eurovoc identifiers. If the user does have an eurlex account with access to the eurlex webservices, he can also 
     pass his webservices login credentials to the method, in order to extract data about works citing work and works 
     being cited by work. The full text is returned as a JSON file, rest of data as a CSV.  Can be in-memory or as saved files.
     <li><code>get_nodes_and_edges_lists</code></li>
     Gets 2 list objects, one for the nodes and edges of the citations within the passed dataframe.
     Allows the creation of a network graph of the citations. Can only be returned in-memory.
+    <li><code>filter_subject_matter</code></li>
+    Returns a dataframe of cases only containing a certain phrase in the column containing the subject of cases.
     <br>
 </ol>
 
 ## What are the parameters?
 <ol>
     <li><code>get_cellar</code></li>
     <strong>Parameters:</strong>
@@ -111,14 +113,21 @@
     </ul>
     <li><code>get_nodes_and_edges_lists</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
         DataFrame of cellar metadata acquired from the get_cellar_extra method with eurlex webservice credentials passed.
         This method will only work on dataframes with citations data.
     </ul>
+    <li><code>filter_subject_matter</code></li>
+    <ul>
+        <li><strong>df: DataFrame object, required, default None</strong></li>
+        DataFrame of cellar metadata acquired from any of the cellar extraction methods listed above.
+        <li><strong>phrase: string, required, default None</strong></li>
+        The phrase which has to be present in the subject matter of cases. Case insensitive.
+    </ul>
 </ol>
 
 
 ## Examples
 ```
 import cellar_extractor as cell
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.53 Summary: Library
+Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.54 Summary: Library
 for extracting cellar data Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Description-Content-Type: text/markdown ## Cellar
 extractor This library contains two functions to get cellar case law data from
 eurlex. ## Version Python 3.9 ## Contributors
@@ -21,14 +21,17 @@
       about works citing work and works being cited by work. The full text is
       returned as a JSON file, rest of data as a CSV. Can be in-memory or as
       saved files.
    5. get_nodes_and_edges_lists
    6. Gets 2 list objects, one for the nodes and edges of the citations within
       the passed dataframe. Allows the creation of a network graph of the
       citations. Can only be returned in-memory.
+   7. filter_subject_matter
+   8. Returns a dataframe of cases only containing a certain phrase in the
+      column containing the subject of cases.
 ## What are the parameters?
    1. get_cellar
    2. Parameters:
           o max_ecli: int, optional, default 100
           o Maximum number of ECLIs to retrieve.
           o sd: date, optional, default '2022-05-01'
           o The start last modification date (yyyy-mm-dd).
@@ -61,14 +64,21 @@
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
    4. get_nodes_and_edges_lists
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from the get_cellar_extra
             method with eurlex webservice credentials passed. This method will
             only work on dataframes with citations data.
+   5. filter_subject_matter
+          o df: DataFrame object, required, default None
+          o DataFrame of cellar metadata acquired from any of the cellar
+            extraction methods listed above.
+          o phrase: string, required, default None
+          o The phrase which has to be present in the subject matter of cases.
+            Case insensitive.
 ## Examples ``` import cellar_extractor as cell Below are examples for in-file
 saving: cell.get_cellar(save_file='y', max_ecli=200, sd='2022-01-01',
 file_format='csv') cell.get_cellar_extra(max_ecli=100, sd='2022-01-01',
 threads=10) Below are examples for in-memory saving: df = cell.get_cellar
 (save_file='n', file_format='csv', sd='2022-01-01', max_ecli=1000) df,json =
 cell.get_cellar_extra(save_file='n', max_ecli=100, sd='2022-01-01', threads=10)
 ``` ## License [![License: Apache 2.0](https://img.shields.io/github/license/
```

### Comparing `cellar_extractor-1.0.53/cellar_extractor.egg-info/SOURCES.txt` & `cellar_extractor-1.0.54/cellar_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.53/setup.py` & `cellar_extractor-1.0.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='cellar_extractor',
     packages=find_packages(include=['cellar_extractor']),
-    version='1.0.53',
+    version='1.0.54',
     description='Library for extracting cellar data',
     author='LawTech Lab',
     license='MIT',
     install_requires=['bs4','SPARQLWrapper==2.0.0', 'requests==2.26.0', 'pandas','lxml==4.6.3','xmltodict==0.13.0','tqdm'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['cellar', 'extractor'],
     long_description=long_descr,
```

