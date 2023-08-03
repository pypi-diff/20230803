# Comparing `tmp/mutalyzer_retriever-0.3.1.tar.gz` & `tmp/mutalyzer_retriever-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/mihai/projects/lumc/mutalyzer/retriever/dist/.tmp-wub87_6n/mutalyzer_retriever-0.3.1.tar", last modified: Mon Mar 13 09:33:43 2023, max compression
+gzip compressed data, was "/home/mihai/projects/mutalyzer/retriever/dist/.tmp-tfz3n6yp/mutalyzer_retriever-0.3.2.tar", last modified: Thu Aug  3 15:51:41 2023, max compression
```

## Comparing `mutalyzer_retriever-0.3.1.tar` & `mutalyzer_retriever-0.3.2.tar`

### file list

```diff
@@ -1,44 +1,41 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-03-13 09:33:43.502423 mutalyzer_retriever-0.3.1/
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1089 2018-12-18 12:36:10.000000 mutalyzer_retriever-0.3.1/LICENSE
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1654 2023-03-13 09:33:43.502423 mutalyzer_retriever-0.3.1/PKG-INFO
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1059 2021-03-11 19:54:13.000000 mutalyzer_retriever-0.3.1/README.md
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-03-13 09:33:43.498423 mutalyzer_retriever-0.3.1/mutalyzer_retriever/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      765 2020-10-29 12:53:48.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5697 2023-01-23 14:38:45.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/cli.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1893 2023-01-23 14:38:45.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/configuration.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1657 2021-09-02 14:16:20.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/ensembl_client_temp.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2729 2021-09-24 07:06:00.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/get_related_tests.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      688 2021-04-22 09:24:29.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/parser.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-03-13 09:33:43.498423 mutalyzer_retriever-0.3.1/mutalyzer_retriever/parsers/
--rw-r--r--   0 mihai     (1000) mihai     (1000)       17 2020-07-02 19:54:36.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/parsers/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      378 2020-10-29 12:53:48.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/parsers/fasta.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    11631 2023-01-26 13:43:50.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/parsers/gff3.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6582 2021-08-18 08:29:40.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/parsers/lrg.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3284 2023-01-23 14:38:45.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/reference.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    10322 2023-01-23 14:38:45.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/related.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      996 2022-05-10 11:07:51.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/request.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    12786 2023-01-23 14:38:45.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/retriever.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)      638 2020-07-02 20:02:18.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/schema_validation.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-03-13 09:33:43.498423 mutalyzer_retriever-0.3.1/mutalyzer_retriever/sources/
--rw-r--r--   0 mihai     (1000) mihai     (1000)        0 2020-07-02 19:54:36.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/sources/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7594 2022-05-10 11:41:45.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/sources/cache.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4372 2022-05-10 12:12:27.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/sources/ensembl.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2756 2022-11-17 08:04:09.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/sources/lrg.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6127 2023-01-23 14:39:39.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/sources/ncbi.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    14735 2023-01-23 14:38:45.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/sources/ncbi_assemblies.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      612 2023-01-23 14:38:45.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever/util.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-03-13 09:33:43.498423 mutalyzer_retriever-0.3.1/mutalyzer_retriever.egg-info/
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1654 2023-03-13 09:33:43.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever.egg-info/PKG-INFO
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1206 2023-03-13 09:33:43.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever.egg-info/SOURCES.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2023-03-13 09:33:43.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever.egg-info/dependency_links.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       69 2023-03-13 09:33:43.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever.egg-info/entry_points.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       71 2023-03-13 09:33:43.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever.egg-info/requires.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       20 2023-03-13 09:33:43.000000 mutalyzer_retriever-0.3.1/mutalyzer_retriever.egg-info/top_level.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1194 2023-03-13 09:33:43.502423 mutalyzer_retriever-0.3.1/setup.cfg
--rw-r--r--   0 mihai     (1000) mihai     (1000)       38 2020-07-06 12:26:44.000000 mutalyzer_retriever-0.3.1/setup.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-03-13 09:33:43.502423 mutalyzer_retriever-0.3.1/tests/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4121 2022-10-06 13:04:34.000000 mutalyzer_retriever-0.3.1/tests/test_cli.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2739 2022-03-10 08:41:30.000000 mutalyzer_retriever-0.3.1/tests/test_fetch.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2445 2022-03-08 20:23:17.000000 mutalyzer_retriever-0.3.1/tests/test_model_validation.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2609 2021-09-28 11:15:46.000000 mutalyzer_retriever-0.3.1/tests/test_related.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2750 2023-01-23 14:38:45.000000 mutalyzer_retriever-0.3.1/tests/test_retriever_model.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-03 15:51:41.783808 mutalyzer_retriever-0.3.2/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1089 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.2/LICENSE
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1654 2023-08-03 15:51:41.783808 mutalyzer_retriever-0.3.2/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1059 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.2/README.md
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-03 15:51:41.779808 mutalyzer_retriever-0.3.2/mutalyzer_retriever/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      765 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5697 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/cli.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1893 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/configuration.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      688 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/parser.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-03 15:51:41.779808 mutalyzer_retriever-0.3.2/mutalyzer_retriever/parsers/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       17 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/parsers/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      378 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/parsers/fasta.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11631 2023-08-03 15:10:07.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/parsers/gff3.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6582 2021-07-23 07:32:49.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/parsers/lrg.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3284 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/reference.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    10322 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/related.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      996 2022-06-03 13:11:00.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/request.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    12786 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/retriever.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      638 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/schema_validation.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-03 15:51:41.779808 mutalyzer_retriever-0.3.2/mutalyzer_retriever/sources/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/sources/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4372 2022-06-03 13:11:00.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/sources/ensembl.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2756 2022-06-03 13:11:00.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/sources/lrg.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6127 2023-08-03 15:10:07.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/sources/ncbi.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    14735 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/sources/ncbi_assemblies.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      612 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever/util.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-03 15:51:41.779808 mutalyzer_retriever-0.3.2/mutalyzer_retriever.egg-info/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1654 2023-08-03 15:51:41.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1085 2023-08-03 15:51:41.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2023-08-03 15:51:41.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       69 2023-08-03 15:51:41.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever.egg-info/entry_points.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       64 2023-08-03 15:51:41.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       20 2023-08-03 15:51:41.000000 mutalyzer_retriever-0.3.2/mutalyzer_retriever.egg-info/top_level.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1187 2023-08-03 15:51:41.783808 mutalyzer_retriever-0.3.2/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.2/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-03 15:51:41.783808 mutalyzer_retriever-0.3.2/tests/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4121 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.2/tests/test_cli.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2739 2022-06-03 13:11:00.000000 mutalyzer_retriever-0.3.2/tests/test_fetch.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2445 2022-06-03 13:11:00.000000 mutalyzer_retriever-0.3.2/tests/test_model_validation.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2609 2021-10-14 13:27:57.000000 mutalyzer_retriever-0.3.2/tests/test_related.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2750 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.2/tests/test_retriever_model.py
```

### Comparing `mutalyzer_retriever-0.3.1/LICENSE` & `mutalyzer_retriever-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/PKG-INFO` & `mutalyzer_retriever-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutalyzer_retriever
-Version: 0.3.1
+Version: 0.3.2
 Summary: Mutalyzer genomic reference retriever.
 Home-page: https://github.com/mutalyzer/retriever
 Author: Mihai Lefter
 Author-email: M.Lefter@lumc.nl
 License: MIT
 Keywords: Mutalyzer,HGVS,reference,retriever,genomic
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mutalyzer_retriever-0.3.1/README.md` & `mutalyzer_retriever-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/__init__.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/__init__.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/cli.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/cli.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/configuration.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/configuration.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/parser.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/parser.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/parsers/gff3.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/parsers/gff3.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/parsers/lrg.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/parsers/lrg.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/reference.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/reference.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/related.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/related.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/request.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/request.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/retriever.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/retriever.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/schema_validation.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/schema_validation.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/sources/ensembl.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/sources/ensembl.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/sources/lrg.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/sources/lrg.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/sources/ncbi.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/sources/ncbi.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/sources/ncbi_assemblies.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/sources/ncbi_assemblies.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever/util.py` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever/util.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever.egg-info/PKG-INFO` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutalyzer-retriever
-Version: 0.3.1
+Version: 0.3.2
 Summary: Mutalyzer genomic reference retriever.
 Home-page: https://github.com/mutalyzer/retriever
 Author: Mihai Lefter
 Author-email: M.Lefter@lumc.nl
 License: MIT
 Keywords: Mutalyzer,HGVS,reference,retriever,genomic
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mutalyzer_retriever-0.3.1/mutalyzer_retriever.egg-info/SOURCES.txt` & `mutalyzer_retriever-0.3.2/mutalyzer_retriever.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 mutalyzer_retriever/__init__.py
 mutalyzer_retriever/cli.py
 mutalyzer_retriever/configuration.py
-mutalyzer_retriever/ensembl_client_temp.py
-mutalyzer_retriever/get_related_tests.py
 mutalyzer_retriever/parser.py
 mutalyzer_retriever/reference.py
 mutalyzer_retriever/related.py
 mutalyzer_retriever/request.py
 mutalyzer_retriever/retriever.py
 mutalyzer_retriever/schema_validation.py
 mutalyzer_retriever/util.py
@@ -21,15 +19,14 @@
 mutalyzer_retriever.egg-info/requires.txt
 mutalyzer_retriever.egg-info/top_level.txt
 mutalyzer_retriever/parsers/__init__.py
 mutalyzer_retriever/parsers/fasta.py
 mutalyzer_retriever/parsers/gff3.py
 mutalyzer_retriever/parsers/lrg.py
 mutalyzer_retriever/sources/__init__.py
-mutalyzer_retriever/sources/cache.py
 mutalyzer_retriever/sources/ensembl.py
 mutalyzer_retriever/sources/lrg.py
 mutalyzer_retriever/sources/ncbi.py
 mutalyzer_retriever/sources/ncbi_assemblies.py
 tests/test_cli.py
 tests/test_fetch.py
 tests/test_model_validation.py
```

### Comparing `mutalyzer_retriever-0.3.1/setup.cfg` & `mutalyzer_retriever-0.3.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mutalyzer_retriever
-version = 0.3.1
+version = 0.3.2
 description = Mutalyzer genomic reference retriever.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Mihai Lefter
 author_email = M.Lefter@lumc.nl
 url = https://github.com/mutalyzer/retriever
 keywords = Mutalyzer, HGVS, reference, retriever, genomic
@@ -15,16 +15,16 @@
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Topic :: Scientific/Engineering :: Bio-Informatics
 
 [options]
 packages = find:
 install_requires = 
-	biopython>=1.78,<=1.80
-	bcbio-gff>=0.6.6
+	biopython>=1.78
+	bcbio-gff>=0.7.0
 	requests>=2.26.0
 	schema>=0.7.4
 tests_require = 
 	pytest>=6.2.5
 
 [options.entry_points]
 console_scripts =
```

### Comparing `mutalyzer_retriever-0.3.1/tests/test_cli.py` & `mutalyzer_retriever-0.3.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/tests/test_fetch.py` & `mutalyzer_retriever-0.3.2/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/tests/test_model_validation.py` & `mutalyzer_retriever-0.3.2/tests/test_model_validation.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/tests/test_related.py` & `mutalyzer_retriever-0.3.2/tests/test_related.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.1/tests/test_retriever_model.py` & `mutalyzer_retriever-0.3.2/tests/test_retriever_model.py`

 * *Files identical despite different names*

