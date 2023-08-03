# Comparing `tmp/python-documentcloud-3.3.9.tar.gz` & `tmp/python-documentcloud-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-documentcloud-3.3.9.tar", last modified: Tue Mar 14 16:20:49 2023, max compression
+gzip compressed data, was "python-documentcloud-3.4.0.tar", last modified: Thu Aug  3 19:08:33 2023, max compression
```

## Comparing `python-documentcloud-3.3.9.tar` & `python-documentcloud-3.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-03-14 16:20:49.603093 python-documentcloud-3.3.9/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1151 2020-06-11 15:56:14.000000 python-documentcloud-3.3.9/LICENSE
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2131 2023-03-14 16:20:49.603093 python-documentcloud-3.3.9/PKG-INFO
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1175 2022-03-23 18:09:12.000000 python-documentcloud-3.3.9/README.md
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-03-14 16:20:49.599092 python-documentcloud-3.3.9/documentcloud/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      220 2020-06-13 15:35:49.000000 python-documentcloud-3.3.9/documentcloud/__init__.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)    10750 2023-03-14 12:52:00.000000 python-documentcloud-3.3.9/documentcloud/addon.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2712 2020-06-16 14:28:21.000000 python-documentcloud-3.3.9/documentcloud/annotations.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     7143 2023-03-14 16:17:17.000000 python-documentcloud-3.3.9/documentcloud/base.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     5974 2022-03-14 16:33:38.000000 python-documentcloud-3.3.9/documentcloud/client.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      256 2021-03-11 15:48:51.000000 python-documentcloud-3.3.9/documentcloud/constants.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)    15989 2023-02-24 21:34:15.000000 python-documentcloud-3.3.9/documentcloud/documents.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1270 2020-06-15 18:35:58.000000 python-documentcloud-3.3.9/documentcloud/exceptions.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      565 2020-06-15 18:35:58.000000 python-documentcloud-3.3.9/documentcloud/organizations.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     5392 2022-03-14 16:33:38.000000 python-documentcloud-3.3.9/documentcloud/projects.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1123 2020-06-15 18:35:58.000000 python-documentcloud-3.3.9/documentcloud/sections.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2012 2020-06-15 18:35:58.000000 python-documentcloud-3.3.9/documentcloud/toolbox.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      527 2020-06-15 18:35:58.000000 python-documentcloud-3.3.9/documentcloud/users.py
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-03-14 16:20:49.603093 python-documentcloud-3.3.9/python_documentcloud.egg-info/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2131 2023-03-14 16:20:49.000000 python-documentcloud-3.3.9/python_documentcloud.egg-info/PKG-INFO
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      592 2023-03-14 16:20:49.000000 python-documentcloud-3.3.9/python_documentcloud.egg-info/SOURCES.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)        1 2023-03-14 16:20:49.000000 python-documentcloud-3.3.9/python_documentcloud.egg-info/dependency_links.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      188 2023-03-14 16:20:49.000000 python-documentcloud-3.3.9/python_documentcloud.egg-info/requires.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)       14 2023-03-14 16:20:49.000000 python-documentcloud-3.3.9/python_documentcloud.egg-info/top_level.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      102 2023-03-14 16:20:49.603093 python-documentcloud-3.3.9/setup.cfg
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1665 2023-03-14 16:20:35.000000 python-documentcloud-3.3.9/setup.py
+drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-08-03 19:08:33.663637 python-documentcloud-3.4.0/
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1151 2020-06-11 15:56:14.000000 python-documentcloud-3.4.0/LICENSE
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2131 2023-08-03 19:08:33.663637 python-documentcloud-3.4.0/PKG-INFO
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1175 2022-03-23 18:09:12.000000 python-documentcloud-3.4.0/README.md
+drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-08-03 19:08:33.659637 python-documentcloud-3.4.0/documentcloud/
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      220 2020-06-13 15:35:49.000000 python-documentcloud-3.4.0/documentcloud/__init__.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)    10750 2023-08-03 19:08:29.000000 python-documentcloud-3.4.0/documentcloud/addon.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2712 2020-06-16 14:28:21.000000 python-documentcloud-3.4.0/documentcloud/annotations.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     7143 2023-03-14 16:55:30.000000 python-documentcloud-3.4.0/documentcloud/base.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     5974 2022-03-14 16:33:38.000000 python-documentcloud-3.4.0/documentcloud/client.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2144 2023-08-03 19:08:31.000000 python-documentcloud-3.4.0/documentcloud/constants.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)    17132 2023-08-03 19:08:31.000000 python-documentcloud-3.4.0/documentcloud/documents.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1270 2020-06-15 18:35:58.000000 python-documentcloud-3.4.0/documentcloud/exceptions.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      565 2020-06-15 18:35:58.000000 python-documentcloud-3.4.0/documentcloud/organizations.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     5392 2022-03-14 16:33:38.000000 python-documentcloud-3.4.0/documentcloud/projects.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1123 2020-06-15 18:35:58.000000 python-documentcloud-3.4.0/documentcloud/sections.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2012 2020-06-15 18:35:58.000000 python-documentcloud-3.4.0/documentcloud/toolbox.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      527 2020-06-15 18:35:58.000000 python-documentcloud-3.4.0/documentcloud/users.py
+drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-08-03 19:08:33.663637 python-documentcloud-3.4.0/python_documentcloud.egg-info/
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2131 2023-08-03 19:08:33.000000 python-documentcloud-3.4.0/python_documentcloud.egg-info/PKG-INFO
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      592 2023-08-03 19:08:33.000000 python-documentcloud-3.4.0/python_documentcloud.egg-info/SOURCES.txt
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)        1 2023-08-03 19:08:33.000000 python-documentcloud-3.4.0/python_documentcloud.egg-info/dependency_links.txt
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      188 2023-08-03 19:08:33.000000 python-documentcloud-3.4.0/python_documentcloud.egg-info/requires.txt
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)       14 2023-08-03 19:08:33.000000 python-documentcloud-3.4.0/python_documentcloud.egg-info/top_level.txt
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      102 2023-08-03 19:08:33.663637 python-documentcloud-3.4.0/setup.cfg
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1665 2023-08-03 19:08:31.000000 python-documentcloud-3.4.0/setup.py
```

### Comparing `python-documentcloud-3.3.9/LICENSE` & `python-documentcloud-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.9/PKG-INFO` & `python-documentcloud-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-documentcloud
-Version: 3.3.9
+Version: 3.4.0
 Summary: A simple Python wrapper for the DocumentCloud API
 Home-page: https://github.com/muckrock/python-documentcloud
 Author: Mitchell Kotler
 Author-email: mitch@muckrock.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-documentcloud-3.3.9/README.md` & `python-documentcloud-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.9/documentcloud/addon.py` & `python-documentcloud-3.4.0/documentcloud/addon.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.9/documentcloud/annotations.py` & `python-documentcloud-3.4.0/documentcloud/annotations.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.9/documentcloud/base.py` & `python-documentcloud-3.4.0/documentcloud/base.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.9/documentcloud/client.py` & `python-documentcloud-3.4.0/documentcloud/client.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.9/documentcloud/documents.py` & `python-documentcloud-3.4.0/documentcloud/documents.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,28 +15,27 @@
 # Third Party
 from future.utils import python_2_unicode_compatible
 from requests.exceptions import RequestException
 
 # Local
 from .annotations import AnnotationClient
 from .base import APIResults, BaseAPIClient, BaseAPIObject
-from .constants import BULK_LIMIT
+from .constants import BULK_LIMIT, SUPPORTED_EXTENSIONS
 from .exceptions import APIError
 from .organizations import Organization
 from .sections import SectionClient
 from .toolbox import grouper, is_url, merge_dicts, requests_retry_session
 from .users import User
 
 try:
     from urllib.parse import urlparse
 except ImportError:
     from urlparse import urlparse
 
 
-
 logger = logging.getLogger("documentcloud")
 
 
 @python_2_unicode_compatible
 class Document(BaseAPIObject):
     """A single DocumentCloud document"""
 
@@ -51,15 +50,14 @@
         "related_article",
         "source",
         "title",
     ]
     date_fields = ["created_at", "updated_at"]
 
     def __init__(self, client, dict_):
-
         # deal with potentially nested objects
         objs = [("user", User), ("organization", Organization)]
         for name, resource in objs:
             value = dict_.get(name)
             if isinstance(value, dict):
                 dict_["_" + name] = resource(client, value)
                 dict_[name + "_id"] = value.get("id")
@@ -341,104 +339,129 @@
         doc_id = create_json["id"]
         response = self.client.post(
             "documents/{}/process/".format(doc_id), json={"force_ocr": force_ocr}
         )
 
         return Document(self.client, create_json)
 
-    def _collect_files(self, path, extension):
-        """Find the paths to all pdfs under a directory"""
+    def _collect_files(self, path, extensions):
+        """Find the paths to files with specified extensions under a directory"""
         path_list = []
-        for (dirpath, _dirname, filenames) in os.walk(path):
+        for dirpath, _, filenames in os.walk(path):
             path_list.extend(
                 [
-                    os.path.join(dirpath, i)
-                    for i in filenames
-                    if extension is None or i.lower().endswith(extension)
+                    os.path.join(dirpath, filename)
+                    for filename in filenames
+                    if os.path.splitext(filename)[1].lower() in extensions
                 ]
             )
         return path_list
 
-    def upload_directory(self, path, handle_errors=False, extension=".pdf", **kwargs):
-        """Upload all PDFs in a directory"""
+    def upload_directory(self, path, handle_errors=False, extensions=".pdf", **kwargs):
+        """Upload files with specified extensions in a directory"""
 
-        # do not set the same title for all documents
+        # Do not set the same title for all documents
         kwargs.pop("title", None)
 
-        # Loop through the path and get all the files
-        path_list = self._collect_files(path, extension)
+        # If extensions is specified as None, it will check for all suported filetypes.
+        if extensions is None:
+            extensions = SUPPORTED_EXTENSIONS
+
+        # Convert single extension to a list if provided
+        if extensions and not isinstance(extensions, list):
+            extensions = [extensions]
+
+        # Checks to see if the extensions are supported, raises an error if not.
+        invalid_extensions = set(extensions) - set(SUPPORTED_EXTENSIONS)
+        if invalid_extensions:
+            raise ValueError(
+                f"Invalid extensions provided: {', '.join(invalid_extensions)}"
+            )
+
+        # Loop through the path and get all the files with matching extensions
+        path_list = self._collect_files(path, extensions)
 
         logger.info(
             "Upload directory on %s: Found %d files to upload", path, len(path_list)
         )
 
-        # Upload all the pdfs using the bulk API to reduce the number
+        # Upload all the files using the bulk API to reduce the number
         # of API calls and improve performance
         obj_list = []
         params = self._format_upload_parameters("", **kwargs)
-        for i, pdf_paths in enumerate(grouper(path_list, BULK_LIMIT)):
+        for i, file_paths in enumerate(grouper(path_list, BULK_LIMIT)):
             # Grouper will put None's on the end of the last group
-            pdf_paths = [p for p in pdf_paths if p is not None]
+            file_paths = [p for p in file_paths if p is not None]
 
-            logger.info("Uploading group %d: %s", i + 1, "\n".join(pdf_paths))
+            logger.info("Uploading group %d: %s", i + 1, "\n".join(file_paths))
 
-            # create the documents
+            # Create the documents
             logger.info("Creating the documents...")
             try:
                 response = self.client.post(
                     "documents/",
                     json=[
-                        merge_dicts(params, {"title": self._get_title(p)})
-                        for p in pdf_paths
+                        merge_dicts(
+                            params,
+                            {
+                                "title": self._get_title(p),
+                                "original_extension": os.path.splitext(
+                                    os.path.basename(p)
+                                )[1]
+                                .lower()
+                                .lstrip("."),
+                            },
+                        )
+                        for p in file_paths
                     ],
                 )
             except (APIError, RequestException) as exc:
                 if handle_errors:
                     logger.info(
                         "Error creating the following documents: %s %s",
                         exc,
-                        "\n".join(pdf_paths),
+                        "\n".join(file_paths),
                     )
                     continue
                 else:
                     raise
 
-            # upload the files directly to storage
+            # Upload the files directly to storage
             create_json = response.json()
             obj_list.extend(create_json)
             presigned_urls = [j["presigned_url"] for j in create_json]
-            for url, pdf_path in zip(presigned_urls, pdf_paths):
-                logger.info("Uploading %s to S3...", pdf_path)
+            for url, file_path in zip(presigned_urls, file_paths):
+                logger.info("Uploading %s to S3...", file_path)
                 try:
                     response = requests_retry_session().put(
-                        url, data=open(pdf_path, "rb").read()
+                        url, data=open(file_path, "rb").read()
                     )
                     self.client.raise_for_status(response)
                 except (APIError, RequestException) as exc:
                     if handle_errors:
                         logger.info(
                             "Error uploading the following document: %s %s",
                             exc,
-                            pdf_path,
+                            file_path,
                         )
                         continue
                     else:
                         raise
 
-            # begin processing the documents
+            # Begin processing the documents
             logger.info("Processing the documents...")
             doc_ids = [j["id"] for j in create_json]
             try:
                 response = self.client.post("documents/process/", json={"ids": doc_ids})
             except (APIError, RequestException) as exc:
                 if handle_errors:
                     logger.info(
                         "Error creating the following documents: %s %s",
                         exc,
-                        "\n".join(pdf_paths),
+                        "\n".join(file_paths),
                     )
                     continue
                 else:
                     raise
 
         logger.info("Upload directory complete")
```

### Comparing `python-documentcloud-3.3.9/documentcloud/exceptions.py` & `python-documentcloud-3.4.0/documentcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.9/documentcloud/organizations.py` & `python-documentcloud-3.4.0/documentcloud/organizations.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.9/documentcloud/projects.py` & `python-documentcloud-3.4.0/documentcloud/projects.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.9/documentcloud/sections.py` & `python-documentcloud-3.4.0/documentcloud/sections.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.9/documentcloud/toolbox.py` & `python-documentcloud-3.4.0/documentcloud/toolbox.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.9/documentcloud/users.py` & `python-documentcloud-3.4.0/documentcloud/users.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.9/python_documentcloud.egg-info/PKG-INFO` & `python-documentcloud-3.4.0/python_documentcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-documentcloud
-Version: 3.3.9
+Version: 3.4.0
 Summary: A simple Python wrapper for the DocumentCloud API
 Home-page: https://github.com/muckrock/python-documentcloud
 Author: Mitchell Kotler
 Author-email: mitch@muckrock.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-documentcloud-3.3.9/python_documentcloud.egg-info/SOURCES.txt` & `python-documentcloud-3.4.0/python_documentcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.9/setup.py` & `python-documentcloud-3.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='python-documentcloud',
-    version='3.3.9',
+    version='3.4.0',
     description='A simple Python wrapper for the DocumentCloud API',
     author='Mitchell Kotler',
     author_email='mitch@muckrock.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/muckrock/python-documentcloud',
     license="MIT",
```

