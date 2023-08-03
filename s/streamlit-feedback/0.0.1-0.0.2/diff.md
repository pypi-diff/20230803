# Comparing `tmp/streamlit-feedback-0.0.1.tar.gz` & `tmp/streamlit-feedback-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-feedback-0.0.1.tar", last modified: Thu Aug  3 16:36:58 2023, max compression
+gzip compressed data, was "streamlit-feedback-0.0.2.tar", last modified: Thu Aug  3 16:54:50 2023, max compression
```

## Comparing `streamlit-feedback-0.0.1.tar` & `streamlit-feedback-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2023-08-03 16:36:58.894566 streamlit-feedback-0.0.1/
--rw-r--r--   0 jeffkayne   (501) staff       (20)     1063 2023-08-03 08:05:16.000000 streamlit-feedback-0.0.1/LICENSE
--rw-r--r--   0 jeffkayne   (501) staff       (20)       54 2023-08-03 08:05:16.000000 streamlit-feedback-0.0.1/MANIFEST.in
--rw-r--r--   0 jeffkayne   (501) staff       (20)     1685 2023-08-03 16:36:58.894425 streamlit-feedback-0.0.1/PKG-INFO
--rw-r--r--   0 jeffkayne   (501) staff       (20)     1385 2023-08-03 16:24:01.000000 streamlit-feedback-0.0.1/README.md
--rw-r--r--   0 jeffkayne   (501) staff       (20)       38 2023-08-03 16:36:58.894613 streamlit-feedback-0.0.1/setup.cfg
--rw-r--r--   0 jeffkayne   (501) staff       (20)      814 2023-08-03 10:01:43.000000 streamlit-feedback-0.0.1/setup.py
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2023-08-03 16:36:58.887031 streamlit-feedback-0.0.1/streamlit_feedback/
--rw-r--r--   0 jeffkayne   (501) staff       (20)     3918 2023-08-03 16:33:17.000000 streamlit-feedback-0.0.1/streamlit_feedback/__init__.py
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2023-08-03 16:36:58.885921 streamlit-feedback-0.0.1/streamlit_feedback/frontend/
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2023-08-03 16:36:58.889391 streamlit-feedback-0.0.1/streamlit_feedback/frontend/build/
--rw-r--r--   0 jeffkayne   (501) staff       (20)      221 2023-08-03 09:46:15.000000 streamlit-feedback-0.0.1/streamlit_feedback/frontend/build/asset-manifest.json
--rw-r--r--   0 jeffkayne   (501) staff       (20)   197459 2023-08-03 09:46:05.000000 streamlit-feedback-0.0.1/streamlit_feedback/frontend/build/bootstrap.min.css
--rw-r--r--   0 jeffkayne   (501) staff       (20)      492 2023-08-03 09:46:15.000000 streamlit-feedback-0.0.1/streamlit_feedback/frontend/build/index.html
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2023-08-03 16:36:58.886085 streamlit-feedback-0.0.1/streamlit_feedback/frontend/build/static/
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2023-08-03 16:36:58.891666 streamlit-feedback-0.0.1/streamlit_feedback/frontend/build/static/js/
--rw-r--r--   0 jeffkayne   (501) staff       (20)   492893 2023-08-03 09:46:15.000000 streamlit-feedback-0.0.1/streamlit_feedback/frontend/build/static/js/main.d715fd8f.js
--rw-r--r--   0 jeffkayne   (501) staff       (20)     1868 2023-08-03 09:46:15.000000 streamlit-feedback-0.0.1/streamlit_feedback/frontend/build/static/js/main.d715fd8f.js.LICENSE.txt
--rw-r--r--   0 jeffkayne   (501) staff       (20)  1878683 2023-08-03 09:46:15.000000 streamlit-feedback-0.0.1/streamlit_feedback/frontend/build/static/js/main.d715fd8f.js.map
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2023-08-03 16:36:58.887827 streamlit-feedback-0.0.1/streamlit_feedback.egg-info/
--rw-r--r--   0 jeffkayne   (501) staff       (20)     1685 2023-08-03 16:36:58.000000 streamlit-feedback-0.0.1/streamlit_feedback.egg-info/PKG-INFO
--rw-r--r--   0 jeffkayne   (501) staff       (20)      628 2023-08-03 16:36:58.000000 streamlit-feedback-0.0.1/streamlit_feedback.egg-info/SOURCES.txt
--rw-r--r--   0 jeffkayne   (501) staff       (20)        1 2023-08-03 16:36:58.000000 streamlit-feedback-0.0.1/streamlit_feedback.egg-info/dependency_links.txt
--rw-r--r--   0 jeffkayne   (501) staff       (20)       16 2023-08-03 16:36:58.000000 streamlit-feedback-0.0.1/streamlit_feedback.egg-info/requires.txt
--rw-r--r--   0 jeffkayne   (501) staff       (20)       19 2023-08-03 16:36:58.000000 streamlit-feedback-0.0.1/streamlit_feedback.egg-info/top_level.txt
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2023-08-03 16:54:50.957930 streamlit-feedback-0.0.2/
+-rw-r--r--   0 jeffkayne   (501) staff       (20)     1063 2023-08-03 08:05:16.000000 streamlit-feedback-0.0.2/LICENSE
+-rw-r--r--   0 jeffkayne   (501) staff       (20)       54 2023-08-03 08:05:16.000000 streamlit-feedback-0.0.2/MANIFEST.in
+-rw-r--r--   0 jeffkayne   (501) staff       (20)     1685 2023-08-03 16:54:50.957790 streamlit-feedback-0.0.2/PKG-INFO
+-rw-r--r--   0 jeffkayne   (501) staff       (20)     1385 2023-08-03 16:24:01.000000 streamlit-feedback-0.0.2/README.md
+-rw-r--r--   0 jeffkayne   (501) staff       (20)       38 2023-08-03 16:54:50.957978 streamlit-feedback-0.0.2/setup.cfg
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      814 2023-08-03 16:54:42.000000 streamlit-feedback-0.0.2/setup.py
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2023-08-03 16:54:50.950415 streamlit-feedback-0.0.2/streamlit_feedback/
+-rw-r--r--   0 jeffkayne   (501) staff       (20)     3918 2023-08-03 16:53:08.000000 streamlit-feedback-0.0.2/streamlit_feedback/__init__.py
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2023-08-03 16:54:50.949386 streamlit-feedback-0.0.2/streamlit_feedback/frontend/
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2023-08-03 16:54:50.952715 streamlit-feedback-0.0.2/streamlit_feedback/frontend/build/
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      221 2023-08-03 09:46:15.000000 streamlit-feedback-0.0.2/streamlit_feedback/frontend/build/asset-manifest.json
+-rw-r--r--   0 jeffkayne   (501) staff       (20)   197459 2023-08-03 09:46:05.000000 streamlit-feedback-0.0.2/streamlit_feedback/frontend/build/bootstrap.min.css
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      492 2023-08-03 09:46:15.000000 streamlit-feedback-0.0.2/streamlit_feedback/frontend/build/index.html
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2023-08-03 16:54:50.949576 streamlit-feedback-0.0.2/streamlit_feedback/frontend/build/static/
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2023-08-03 16:54:50.955034 streamlit-feedback-0.0.2/streamlit_feedback/frontend/build/static/js/
+-rw-r--r--   0 jeffkayne   (501) staff       (20)   492893 2023-08-03 09:46:15.000000 streamlit-feedback-0.0.2/streamlit_feedback/frontend/build/static/js/main.d715fd8f.js
+-rw-r--r--   0 jeffkayne   (501) staff       (20)     1868 2023-08-03 09:46:15.000000 streamlit-feedback-0.0.2/streamlit_feedback/frontend/build/static/js/main.d715fd8f.js.LICENSE.txt
+-rw-r--r--   0 jeffkayne   (501) staff       (20)  1878683 2023-08-03 09:46:15.000000 streamlit-feedback-0.0.2/streamlit_feedback/frontend/build/static/js/main.d715fd8f.js.map
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2023-08-03 16:54:50.951184 streamlit-feedback-0.0.2/streamlit_feedback.egg-info/
+-rw-r--r--   0 jeffkayne   (501) staff       (20)     1685 2023-08-03 16:54:50.000000 streamlit-feedback-0.0.2/streamlit_feedback.egg-info/PKG-INFO
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      628 2023-08-03 16:54:50.000000 streamlit-feedback-0.0.2/streamlit_feedback.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffkayne   (501) staff       (20)        1 2023-08-03 16:54:50.000000 streamlit-feedback-0.0.2/streamlit_feedback.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffkayne   (501) staff       (20)       16 2023-08-03 16:54:50.000000 streamlit-feedback-0.0.2/streamlit_feedback.egg-info/requires.txt
+-rw-r--r--   0 jeffkayne   (501) staff       (20)       19 2023-08-03 16:54:50.000000 streamlit-feedback-0.0.2/streamlit_feedback.egg-info/top_level.txt
```

### Comparing `streamlit-feedback-0.0.1/LICENSE` & `streamlit-feedback-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-feedback-0.0.1/PKG-INFO` & `streamlit-feedback-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-feedback
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit component that allows you to collect user feedback in your apps
 Home-page: 
 Author: Jeff Kayne
 Author-email: jeff.kayne@trubrics.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-feedback-0.0.1/README.md` & `streamlit-feedback-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-feedback-0.0.1/setup.py` & `streamlit-feedback-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-feedback",
-    version="0.0.1",
+    version="0.0.2",
     author="Jeff Kayne",
     author_email="jeff.kayne@trubrics.com",
     description="Streamlit component that allows you to collect user feedback in your apps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-feedback-0.0.1/streamlit_feedback/__init__.py` & `streamlit-feedback-0.0.2/streamlit_feedback/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-feedback-0.0.1/streamlit_feedback/frontend/build/bootstrap.min.css` & `streamlit-feedback-0.0.2/streamlit_feedback/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-feedback-0.0.1/streamlit_feedback/frontend/build/static/js/main.d715fd8f.js` & `streamlit-feedback-0.0.2/streamlit_feedback/frontend/build/static/js/main.d715fd8f.js`

 * *Files identical despite different names*

### Comparing `streamlit-feedback-0.0.1/streamlit_feedback/frontend/build/static/js/main.d715fd8f.js.LICENSE.txt` & `streamlit-feedback-0.0.2/streamlit_feedback/frontend/build/static/js/main.d715fd8f.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-feedback-0.0.1/streamlit_feedback/frontend/build/static/js/main.d715fd8f.js.map` & `streamlit-feedback-0.0.2/streamlit_feedback/frontend/build/static/js/main.d715fd8f.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-feedback-0.0.1/streamlit_feedback.egg-info/PKG-INFO` & `streamlit-feedback-0.0.2/streamlit_feedback.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-feedback
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit component that allows you to collect user feedback in your apps
 Home-page: 
 Author: Jeff Kayne
 Author-email: jeff.kayne@trubrics.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-feedback-0.0.1/streamlit_feedback.egg-info/SOURCES.txt` & `streamlit-feedback-0.0.2/streamlit_feedback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

