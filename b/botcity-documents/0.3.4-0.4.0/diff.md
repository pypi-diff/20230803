# Comparing `tmp/botcity-documents-0.3.4.tar.gz` & `tmp/botcity-documents-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Mar  5 00:33:52 2023, from Unix
+gzip compressed data, last modified: Wed Aug  2 23:47:08 2023, from Unix
```

## Comparing `botcity-documents-0.3.4.tar` & `botcity-documents-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 slepicka   (501) staff       (20)        0 2023-03-05 00:33:50.000000 botcity-documents-0.3.4/
--rw-r--r--   0 slepicka   (501) staff       (20)     4929 2023-03-05 00:33:50.000000 botcity-documents-0.3.4/PKG-INFO
--rw-r--r--   0 slepicka   (501) staff       (20)       18 2022-12-05 17:46:12.000000 botcity-documents-0.3.4/requirements.txt
-drwxr-xr-x   0 slepicka   (501) staff       (20)        0 2023-03-05 00:33:50.000000 botcity-documents-0.3.4/botcity_documents.egg-info/
-drwxr-xr-x   0 slepicka   (501) staff       (20)        0 2023-03-05 00:33:50.000000 botcity-documents-0.3.4/botcity/
--rw-r--r--   0 slepicka   (501) staff       (20)      190 2022-10-25 20:54:04.000000 botcity-documents-0.3.4/MANIFEST.in
--rw-r--r--   0 slepicka   (501) staff       (20)     4734 2022-01-12 08:28:26.000000 botcity-documents-0.3.4/README.md
--rw-r--r--   0 slepicka   (501) staff       (20)      725 2021-11-09 01:26:41.000000 botcity-documents-0.3.4/setup.py
--rw-r--r--   0 slepicka   (501) staff       (20)      213 2023-03-05 00:33:50.000000 botcity-documents-0.3.4/setup.cfg
--rw-r--r--   0 slepicka   (501) staff       (20)    70144 2021-11-03 21:53:55.000000 botcity-documents-0.3.4/versioneer.py
-drwxr-xr-x   0 slepicka   (501) staff       (20)        0 2023-03-05 00:33:50.000000 botcity-documents-0.3.4/botcity/document_processing/
--rw-r--r--   0 slepicka   (501) staff       (20)      497 2023-03-05 00:33:50.000000 botcity-documents-0.3.4/botcity/document_processing/_version.py
-drwxr-xr-x   0 slepicka   (501) staff       (20)        0 2023-03-05 00:33:52.000000 botcity-documents-0.3.4/botcity/document_processing/pdf/
--rw-r--r--   0 slepicka   (501) staff       (20)      229 2021-12-01 02:05:25.000000 botcity-documents-0.3.4/botcity/document_processing/__init__.py
-drwxr-xr-x   0 slepicka   (501) staff       (20)        0 2023-03-05 00:33:52.000000 botcity-documents-0.3.4/botcity/document_processing/parser/
--rw-r--r--   0 slepicka   (501) staff       (20)      911 2022-04-18 18:19:58.000000 botcity-documents-0.3.4/botcity/document_processing/geometry.py
--rw-r--r--   0 slepicka   (501) staff       (20)      442 2021-12-18 00:17:37.000000 botcity-documents-0.3.4/botcity/document_processing/parser/matcher.py
--rw-r--r--   0 slepicka   (501) staff       (20)      102 2021-12-02 23:36:16.000000 botcity-documents-0.3.4/botcity/document_processing/parser/__init__.py
--rw-r--r--   0 slepicka   (501) staff       (20)     2128 2023-03-05 00:33:52.000000 botcity-documents-0.3.4/botcity/document_processing/parser/_priv_parser.py
--rw-r--r--   0 slepicka   (501) staff       (20)     1280 2022-12-06 18:01:37.000000 botcity-documents-0.3.4/botcity/document_processing/parser/entry.py
--rw-r--r--   0 slepicka   (501) staff       (20)     6832 2022-04-25 23:02:51.000000 botcity-documents-0.3.4/botcity/document_processing/parser/document.py
--rw-r--r--   0 slepicka   (501) staff       (20)      839 2022-10-25 20:54:04.000000 botcity-documents-0.3.4/botcity/document_processing/pdf/pdfreader.py
--rw-r--r--   0 slepicka   (501) staff       (20)    20340 2023-01-06 03:08:32.000000 botcity-documents-0.3.4/botcity/document_processing/pdf/document-processing-1.3.3.jar
--rw-r--r--   0 slepicka   (501) staff       (20)       59 2022-10-25 20:54:04.000000 botcity-documents-0.3.4/botcity/document_processing/pdf/__init__.py
--rw-r--r--   0 slepicka   (501) staff       (20)     1008 2023-03-05 00:33:51.000000 botcity-documents-0.3.4/botcity/document_processing/pdf/_priv_pdfreader.py
--rw-r--r--   0 slepicka   (501) staff       (20)  9893221 2022-10-25 20:54:04.000000 botcity-documents-0.3.4/botcity/document_processing/pdf/pdfbox-app-2.0.19.jar
--rw-r--r--   0 slepicka   (501) staff       (20)     4929 2023-03-05 00:33:50.000000 botcity-documents-0.3.4/botcity_documents.egg-info/PKG-INFO
--rw-r--r--   0 slepicka   (501) staff       (20)      886 2023-03-05 00:33:50.000000 botcity-documents-0.3.4/botcity_documents.egg-info/SOURCES.txt
--rw-r--r--   0 slepicka   (501) staff       (20)       19 2023-03-05 00:33:50.000000 botcity-documents-0.3.4/botcity_documents.egg-info/requires.txt
--rw-r--r--   0 slepicka   (501) staff       (20)        8 2023-03-05 00:33:50.000000 botcity-documents-0.3.4/botcity_documents.egg-info/top_level.txt
--rw-r--r--   0 slepicka   (501) staff       (20)        1 2023-03-05 00:33:50.000000 botcity-documents-0.3.4/botcity_documents.egg-info/dependency_links.txt
+drwxr-xr-x   0 slepicka   (501) staff       (20)        0 2023-08-02 23:47:06.000000 botcity-documents-0.4.0/
+-rw-r--r--   0 slepicka   (501) staff       (20)     4929 2023-08-02 23:47:06.000000 botcity-documents-0.4.0/PKG-INFO
+-rw-r--r--   0 slepicka   (501) staff       (20)       18 2022-12-05 17:46:12.000000 botcity-documents-0.4.0/requirements.txt
+drwxr-xr-x   0 slepicka   (501) staff       (20)        0 2023-08-02 23:47:06.000000 botcity-documents-0.4.0/botcity_documents.egg-info/
+drwxr-xr-x   0 slepicka   (501) staff       (20)        0 2023-08-02 23:47:06.000000 botcity-documents-0.4.0/botcity/
+-rw-r--r--   0 slepicka   (501) staff       (20)      190 2022-10-25 20:54:04.000000 botcity-documents-0.4.0/MANIFEST.in
+-rw-r--r--   0 slepicka   (501) staff       (20)     4734 2022-01-12 08:28:26.000000 botcity-documents-0.4.0/README.md
+-rw-r--r--   0 slepicka   (501) staff       (20)      725 2021-11-09 01:26:41.000000 botcity-documents-0.4.0/setup.py
+-rw-r--r--   0 slepicka   (501) staff       (20)      213 2023-08-02 23:47:06.000000 botcity-documents-0.4.0/setup.cfg
+-rw-r--r--   0 slepicka   (501) staff       (20)    70144 2021-11-03 21:53:55.000000 botcity-documents-0.4.0/versioneer.py
+drwxr-xr-x   0 slepicka   (501) staff       (20)        0 2023-08-02 23:47:06.000000 botcity-documents-0.4.0/botcity/document_processing/
+-rw-r--r--   0 slepicka   (501) staff       (20)      497 2023-08-02 23:47:06.000000 botcity-documents-0.4.0/botcity/document_processing/_version.py
+drwxr-xr-x   0 slepicka   (501) staff       (20)        0 2023-08-02 23:47:08.000000 botcity-documents-0.4.0/botcity/document_processing/pdf/
+-rw-r--r--   0 slepicka   (501) staff       (20)      229 2021-12-01 02:05:25.000000 botcity-documents-0.4.0/botcity/document_processing/__init__.py
+drwxr-xr-x   0 slepicka   (501) staff       (20)        0 2023-08-02 23:47:08.000000 botcity-documents-0.4.0/botcity/document_processing/parser/
+-rw-r--r--   0 slepicka   (501) staff       (20)      911 2022-04-18 18:19:58.000000 botcity-documents-0.4.0/botcity/document_processing/geometry.py
+-rw-r--r--   0 slepicka   (501) staff       (20)      442 2021-12-18 00:17:37.000000 botcity-documents-0.4.0/botcity/document_processing/parser/matcher.py
+-rw-r--r--   0 slepicka   (501) staff       (20)      102 2021-12-02 23:36:16.000000 botcity-documents-0.4.0/botcity/document_processing/parser/__init__.py
+-rw-r--r--   0 slepicka   (501) staff       (20)     2364 2023-08-02 23:47:08.000000 botcity-documents-0.4.0/botcity/document_processing/parser/_priv_parser.py
+-rw-r--r--   0 slepicka   (501) staff       (20)     1280 2022-12-06 18:01:37.000000 botcity-documents-0.4.0/botcity/document_processing/parser/entry.py
+-rw-r--r--   0 slepicka   (501) staff       (20)     7024 2023-08-02 23:46:55.000000 botcity-documents-0.4.0/botcity/document_processing/parser/document.py
+-rw-r--r--   0 slepicka   (501) staff       (20)      839 2022-10-25 20:54:04.000000 botcity-documents-0.4.0/botcity/document_processing/pdf/pdfreader.py
+-rw-r--r--   0 slepicka   (501) staff       (20)    20340 2023-01-06 03:08:32.000000 botcity-documents-0.4.0/botcity/document_processing/pdf/document-processing-1.3.3.jar
+-rw-r--r--   0 slepicka   (501) staff       (20)       59 2022-10-25 20:54:04.000000 botcity-documents-0.4.0/botcity/document_processing/pdf/__init__.py
+-rw-r--r--   0 slepicka   (501) staff       (20)     1008 2023-08-02 23:47:07.000000 botcity-documents-0.4.0/botcity/document_processing/pdf/_priv_pdfreader.py
+-rw-r--r--   0 slepicka   (501) staff       (20)  9893221 2022-10-25 20:54:04.000000 botcity-documents-0.4.0/botcity/document_processing/pdf/pdfbox-app-2.0.19.jar
+-rw-r--r--   0 slepicka   (501) staff       (20)     4929 2023-08-02 23:47:06.000000 botcity-documents-0.4.0/botcity_documents.egg-info/PKG-INFO
+-rw-r--r--   0 slepicka   (501) staff       (20)      886 2023-08-02 23:47:06.000000 botcity-documents-0.4.0/botcity_documents.egg-info/SOURCES.txt
+-rw-r--r--   0 slepicka   (501) staff       (20)       19 2023-08-02 23:47:06.000000 botcity-documents-0.4.0/botcity_documents.egg-info/requires.txt
+-rw-r--r--   0 slepicka   (501) staff       (20)        8 2023-08-02 23:47:06.000000 botcity-documents-0.4.0/botcity_documents.egg-info/top_level.txt
+-rw-r--r--   0 slepicka   (501) staff       (20)        1 2023-08-02 23:47:06.000000 botcity-documents-0.4.0/botcity_documents.egg-info/dependency_links.txt
```

### Comparing `botcity-documents-0.3.4/PKG-INFO` & `botcity-documents-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botcity-documents
-Version: 0.3.4
+Version: 0.4.0
 Home-page: https://bitbucket.org/botcitydev/botcity-documents-python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## 🤖 Computer-vision based UI Automation
 
 Recognize and interact with UI elements using state-of-art computer vision module.
```

### Comparing `botcity-documents-0.3.4/README.md` & `botcity-documents-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `botcity-documents-0.3.4/setup.py` & `botcity-documents-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `botcity-documents-0.3.4/versioneer.py` & `botcity-documents-0.4.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `botcity-documents-0.3.4/botcity/document_processing/geometry.py` & `botcity-documents-0.4.0/botcity/document_processing/geometry.py`

 * *Files identical despite different names*

### Comparing `botcity-documents-0.3.4/botcity/document_processing/parser/entry.py` & `botcity-documents-0.4.0/botcity/document_processing/parser/entry.py`

 * *Files identical despite different names*

### Comparing `botcity-documents-0.3.4/botcity/document_processing/parser/document.py` & `botcity-documents-0.4.0/botcity/document_processing/parser/document.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,31 +54,33 @@
 
         Returns:
             List[Entry]: The parser entries.
         """
         return self._parser.get_entries(self)
 
     @ensure_parser
-    def set_entries(self, entries: List[Entry]):
+    def set_entries(self, entries: List[Entry], sort: bool = True):
         """Sets the list of entries.
 
         Args:
             entries (List[Entry]): List of entries.
+            sort (bool, optional): Sort the entries. Defaults to True.
         """
-        self._parser.set_entries(self, entries)
+        self._parser.set_entries(self, entries, sort)
 
     @ensure_parser
-    def load_entries(self, entries: List):
+    def load_entries(self, entries: List, sort: bool = True):
         """Load entries into the parser.
 
         Args:
             entries (List): List of Entry objects or
                 List of List containing the required information.
+            sort (bool, optional): Sort the entries. Defaults to True.
         """
-        self._parser.load_entries(self, entries)
+        self._parser.load_entries(self, entries, sort)
 
     @ensure_parser
     def get_full_text(self) -> str:
         """Returns the full document text.
 
         Returns:
             str: The document text.
```

### Comparing `botcity-documents-0.3.4/botcity/document_processing/pdf/pdfreader.py` & `botcity-documents-0.4.0/botcity/document_processing/pdf/pdfreader.py`

 * *Files identical despite different names*

### Comparing `botcity-documents-0.3.4/botcity/document_processing/pdf/document-processing-1.3.3.jar` & `botcity-documents-0.4.0/botcity/document_processing/pdf/document-processing-1.3.3.jar`

 * *Files identical despite different names*

### Comparing `botcity-documents-0.3.4/botcity/document_processing/pdf/_priv_pdfreader.py` & `botcity-documents-0.4.0/botcity/document_processing/pdf/_priv_pdfreader.py`

 * *Files identical despite different names*

### Comparing `botcity-documents-0.3.4/botcity/document_processing/pdf/pdfbox-app-2.0.19.jar` & `botcity-documents-0.4.0/botcity/document_processing/pdf/pdfbox-app-2.0.19.jar`

 * *Files identical despite different names*

### Comparing `botcity-documents-0.3.4/botcity_documents.egg-info/PKG-INFO` & `botcity-documents-0.4.0/botcity_documents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botcity-documents
-Version: 0.3.4
+Version: 0.4.0
 Home-page: https://bitbucket.org/botcitydev/botcity-documents-python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## 🤖 Computer-vision based UI Automation
 
 Recognize and interact with UI elements using state-of-art computer vision module.
```

### Comparing `botcity-documents-0.3.4/botcity_documents.egg-info/SOURCES.txt` & `botcity-documents-0.4.0/botcity_documents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

