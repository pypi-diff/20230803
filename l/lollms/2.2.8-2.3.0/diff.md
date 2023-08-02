# Comparing `tmp/lollms-2.2.8.tar.gz` & `tmp/lollms-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-2.2.8.tar", last modified: Tue Aug  1 12:17:29 2023, max compression
+gzip compressed data, was "lollms-2.3.0.tar", last modified: Wed Aug  2 23:06:32 2023, max compression
```

## Comparing `lollms-2.2.8.tar` & `lollms-2.3.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 12:17:29.118796 lollms-2.2.8/
--rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.2.8/LICENSE
--rw-rw-rw-   0        0        0      269 2023-07-19 17:46:44.000000 lollms-2.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0    11076 2023-08-01 12:17:29.117792 lollms-2.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 12:17:29.087237 lollms-2.2.8/lollms/
--rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.2.8/lollms/__init__.py
--rw-rw-rw-   0        0        0     9679 2023-07-31 20:58:01.000000 lollms-2.2.8/lollms/app.py
-drwxrwxrwx   0        0        0        0 2023-08-01 12:17:29.103276 lollms-2.2.8/lollms/apps/
--rw-rw-rw-   0        0        0        0 2023-07-19 16:50:10.000000 lollms-2.2.8/lollms/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 12:17:29.104272 lollms-2.2.8/lollms/apps/console/
--rw-rw-rw-   0        0        0    14754 2023-07-27 19:45:11.000000 lollms-2.2.8/lollms/apps/console/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 12:17:29.105274 lollms-2.2.8/lollms/apps/playground/
--rw-rw-rw-   0        0        0      398 2023-07-19 16:42:16.000000 lollms-2.2.8/lollms/apps/playground/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 12:17:29.112791 lollms-2.2.8/lollms/apps/playground/static/
--rw-rw-rw-   0        0        0    11558 2023-07-19 16:42:16.000000 lollms-2.2.8/lollms/apps/playground/static/LICENSE
--rw-rw-rw-   0        0        0     3900 2023-07-19 16:42:16.000000 lollms-2.2.8/lollms/apps/playground/static/README.md
--rw-rw-rw-   0        0        0      566 2023-07-19 16:42:16.000000 lollms-2.2.8/lollms/apps/playground/static/index.html
--rw-rw-rw-   0        0        0   470378 2023-07-19 16:42:16.000000 lollms-2.2.8/lollms/apps/playground/static/logo.png
--rw-rw-rw-   0        0        0    16548 2023-07-19 16:42:16.000000 lollms-2.2.8/lollms/apps/playground/static/lollms_playground.html
--rw-rw-rw-   0        0        0       62 2023-07-19 16:42:16.000000 lollms-2.2.8/lollms/apps/playground/static/package.json
-drwxrwxrwx   0        0        0        0 2023-08-01 12:17:29.112791 lollms-2.2.8/lollms/apps/server/
--rw-rw-rw-   0        0        0    34757 2023-07-31 12:14:38.000000 lollms-2.2.8/lollms/apps/server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 12:17:29.114794 lollms-2.2.8/lollms/apps/settings/
--rw-rw-rw-   0        0        0     7710 2023-07-31 12:14:48.000000 lollms-2.2.8/lollms/apps/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 12:17:29.114794 lollms-2.2.8/lollms/assets/
--rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.2.8/lollms/assets/logo.png
--rw-rw-rw-   0        0        0    11094 2023-07-31 22:09:20.000000 lollms-2.2.8/lollms/binding.py
--rw-rw-rw-   0        0        0    21426 2023-07-02 17:51:25.000000 lollms-2.2.8/lollms/config.py
-drwxrwxrwx   0        0        0        0 2023-08-01 12:17:29.116791 lollms-2.2.8/lollms/configs/
--rw-rw-rw-   0        0        0      881 2023-07-19 16:42:16.000000 lollms-2.2.8/lollms/configs/config.yaml
--rw-rw-rw-   0        0        0     4418 2023-07-02 12:47:59.000000 lollms-2.2.8/lollms/data.py
--rw-rw-rw-   0        0        0     1357 2023-07-03 19:35:14.000000 lollms-2.2.8/lollms/extension.py
--rw-rw-rw-   0        0        0     3027 2023-07-16 00:19:49.000000 lollms-2.2.8/lollms/helpers.py
--rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.2.8/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7239 2023-07-03 22:53:18.000000 lollms-2.2.8/lollms/main_config.py
--rw-rw-rw-   0        0        0    13693 2023-07-20 17:32:43.000000 lollms-2.2.8/lollms/paths.py
--rw-rw-rw-   0        0        0    50348 2023-07-31 22:28:37.000000 lollms-2.2.8/lollms/personality.py
--rw-rw-rw-   0        0        0    22076 2023-07-30 22:49:52.000000 lollms-2.2.8/lollms/terminal.py
--rw-rw-rw-   0        0        0     2607 2023-07-30 23:55:13.000000 lollms-2.2.8/lollms/types.py
--rw-rw-rw-   0        0        0    28002 2023-08-01 12:08:25.000000 lollms-2.2.8/lollms/utilities.py
-drwxrwxrwx   0        0        0        0 2023-08-01 12:17:29.102278 lollms-2.2.8/lollms.egg-info/
--rw-rw-rw-   0        0        0    11076 2023-08-01 12:17:28.000000 lollms-2.2.8/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      947 2023-08-01 12:17:29.000000 lollms-2.2.8/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 12:17:28.000000 lollms-2.2.8/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2023-08-01 12:17:28.000000 lollms-2.2.8/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      245 2023-08-01 12:17:28.000000 lollms-2.2.8/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-01 12:17:28.000000 lollms-2.2.8/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 12:17:29.118796 lollms-2.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1870 2023-08-01 12:17:24.000000 lollms-2.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:06:32.052549 lollms-2.3.0/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0      269 2023-07-19 17:46:44.000000 lollms-2.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11076 2023-08-02 23:06:32.051540 lollms-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 23:06:31.962833 lollms-2.3.0/lollms/
+-rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.3.0/lollms/__init__.py
+-rw-rw-rw-   0        0        0     9679 2023-07-31 20:58:01.000000 lollms-2.3.0/lollms/app.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:06:31.986271 lollms-2.3.0/lollms/apps/
+-rw-rw-rw-   0        0        0        0 2023-07-19 16:50:10.000000 lollms-2.3.0/lollms/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:06:31.987273 lollms-2.3.0/lollms/apps/console/
+-rw-rw-rw-   0        0        0    14754 2023-07-27 19:45:11.000000 lollms-2.3.0/lollms/apps/console/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:06:31.988269 lollms-2.3.0/lollms/apps/playground/
+-rw-rw-rw-   0        0        0      398 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/apps/playground/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:06:32.038199 lollms-2.3.0/lollms/apps/playground/static/
+-rw-rw-rw-   0        0        0    11558 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/apps/playground/static/LICENSE
+-rw-rw-rw-   0        0        0     3900 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/apps/playground/static/README.md
+-rw-rw-rw-   0        0        0      566 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/apps/playground/static/index.html
+-rw-rw-rw-   0        0        0   470378 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/apps/playground/static/logo.png
+-rw-rw-rw-   0        0        0    16548 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/apps/playground/static/lollms_playground.html
+-rw-rw-rw-   0        0        0       62 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/apps/playground/static/package.json
+drwxrwxrwx   0        0        0        0 2023-08-02 23:06:32.040229 lollms-2.3.0/lollms/apps/server/
+-rw-rw-rw-   0        0        0    34757 2023-07-31 12:14:38.000000 lollms-2.3.0/lollms/apps/server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:06:32.041241 lollms-2.3.0/lollms/apps/settings/
+-rw-rw-rw-   0        0        0     7710 2023-07-31 12:14:48.000000 lollms-2.3.0/lollms/apps/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:06:32.043239 lollms-2.3.0/lollms/assets/
+-rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.3.0/lollms/assets/logo.png
+-rw-rw-rw-   0        0        0    11094 2023-07-31 22:09:20.000000 lollms-2.3.0/lollms/binding.py
+-rw-rw-rw-   0        0        0    21426 2023-07-02 17:51:25.000000 lollms-2.3.0/lollms/config.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:06:32.050270 lollms-2.3.0/lollms/configs/
+-rw-rw-rw-   0        0        0      881 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/configs/config.yaml
+-rw-rw-rw-   0        0        0     4418 2023-07-02 12:47:59.000000 lollms-2.3.0/lollms/data.py
+-rw-rw-rw-   0        0        0     1357 2023-07-03 19:35:14.000000 lollms-2.3.0/lollms/extension.py
+-rw-rw-rw-   0        0        0     3027 2023-07-16 00:19:49.000000 lollms-2.3.0/lollms/helpers.py
+-rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.3.0/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     7239 2023-07-03 22:53:18.000000 lollms-2.3.0/lollms/main_config.py
+-rw-rw-rw-   0        0        0    13693 2023-07-20 17:32:43.000000 lollms-2.3.0/lollms/paths.py
+-rw-rw-rw-   0        0        0    50389 2023-08-02 20:41:38.000000 lollms-2.3.0/lollms/personality.py
+-rw-rw-rw-   0        0        0    22076 2023-07-30 22:49:52.000000 lollms-2.3.0/lollms/terminal.py
+-rw-rw-rw-   0        0        0     2811 2023-08-02 11:44:56.000000 lollms-2.3.0/lollms/types.py
+-rw-rw-rw-   0        0        0    28641 2023-08-01 19:44:49.000000 lollms-2.3.0/lollms/utilities.py
+drwxrwxrwx   0        0        0        0 2023-08-02 23:06:31.985255 lollms-2.3.0/lollms.egg-info/
+-rw-rw-rw-   0        0        0    11076 2023-08-02 23:06:31.000000 lollms-2.3.0/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-08-02 23:06:31.000000 lollms-2.3.0/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 23:06:31.000000 lollms-2.3.0/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2023-08-02 23:06:31.000000 lollms-2.3.0/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      245 2023-08-02 23:06:31.000000 lollms-2.3.0/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 23:06:31.000000 lollms-2.3.0/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 23:06:32.052549 lollms-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1870 2023-08-02 23:06:07.000000 lollms-2.3.0/setup.py
```

### Comparing `lollms-2.2.8/LICENSE` & `lollms-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/PKG-INFO` & `lollms-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.2.8
+Version: 2.3.0
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.2.8/README.md` & `lollms-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/app.py` & `lollms-2.3.0/lollms/app.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/apps/console/__init__.py` & `lollms-2.3.0/lollms/apps/console/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/apps/playground/static/LICENSE` & `lollms-2.3.0/lollms/apps/playground/static/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/apps/playground/static/README.md` & `lollms-2.3.0/lollms/apps/playground/static/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/apps/playground/static/index.html` & `lollms-2.3.0/lollms/apps/playground/static/index.html`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/apps/playground/static/logo.png` & `lollms-2.3.0/lollms/apps/playground/static/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/apps/playground/static/lollms_playground.html` & `lollms-2.3.0/lollms/apps/playground/static/lollms_playground.html`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/apps/server/__init__.py` & `lollms-2.3.0/lollms/apps/server/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/apps/settings/__init__.py` & `lollms-2.3.0/lollms/apps/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/assets/logo.png` & `lollms-2.3.0/lollms/assets/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/binding.py` & `lollms-2.3.0/lollms/binding.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/config.py` & `lollms-2.3.0/lollms/config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/configs/config.yaml` & `lollms-2.3.0/lollms/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/data.py` & `lollms-2.3.0/lollms/data.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/extension.py` & `lollms-2.3.0/lollms/extension.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/helpers.py` & `lollms-2.3.0/lollms/helpers.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/langchain_integration.py` & `lollms-2.3.0/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/main_config.py` & `lollms-2.3.0/lollms/main_config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/paths.py` & `lollms-2.3.0/lollms/paths.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/personality.py` & `lollms-2.3.0/lollms/personality.py`

 * *Files 0% similar despite different names*

```diff
@@ -1285,26 +1285,26 @@
         """
         if not callback and self.callback:
             callback = self.callback
 
         if callback:
             callback(step_text, MSG_TYPE.MSG_TYPE_STEP_PROGRESS, {'progress':progress})
 
-    def new_message(self, message_text:str, message_type:MSG_TYPE, callback: Callable[[str, int, dict], bool]=None):
+    def new_message(self, message_text:str, message_type:MSG_TYPE, metadata=None, callback: Callable[[str, int, dict], bool]=None):
         """This sends step rogress to front end
 
         Args:
             step_text (dict): The step progress in %
             callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the progress to. Defaults to None.
         """
         if not callback and self.callback:
             callback = self.callback
 
         if callback:
-            callback(message_text, MSG_TYPE.MSG_TYPE_NEW_MESSAGE, {'type':message_type})
+            callback(message_text, MSG_TYPE.MSG_TYPE_NEW_MESSAGE, {'type':message_type.value,'metadata':metadata})
 
     def finished_message(self, message_text:str="", callback: Callable[[str, int, dict], bool]=None):
         """This sends step rogress to front end
 
         Args:
             step_text (dict): The step progress in %
             callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the progress to. Defaults to None.
```

### Comparing `lollms-2.2.8/lollms/terminal.py` & `lollms-2.3.0/lollms/terminal.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/lollms/types.py` & `lollms-2.3.0/lollms/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,14 +26,20 @@
     MSG_TYPE_UI                     = 14# A vue.js component to show (we need to build some and parse the text to show it)
 
     #Commands
     MSG_TYPE_NEW_MESSAGE            = 15# A new message
     MSG_TYPE_FINISHED_MESSAGE       = 17# End of current message
 
 
+
+class SENDER_TYPES(Enum):
+    SENDER_TYPES_USER               = 0 # Sent by user
+    SENDER_TYPES_AI                 = 1 # Sent by ai
+    SENDER_TYPES_SYSTEM             = 2 # Sent by athe system
+
 class GenerationPresets:
     """
     Class containing various generation presets.
     """
 
     @staticmethod
     def deterministic_preset():
```

### Comparing `lollms-2.2.8/lollms/utilities.py` & `lollms-2.3.0/lollms/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,35 @@
 from lollms.helpers import ASCIIColors, trace_exception
 from lollms.paths import LollmsPaths
 from sklearn.feature_extraction.text import TfidfVectorizer
 import numpy as np
 from pathlib import Path
 import json
 import re
-
+import subprocess
 class PackageManager:
     @staticmethod
     def install_package(package_name):
         import subprocess
         import sys
         subprocess.check_call([sys.executable, "-m", "pip", "install", package_name])
 
+class GitManager:
+    @staticmethod
+    def git_pull(folder_path):
+        try:
+            # Change the current working directory to the desired folder
+            subprocess.run(["git", "checkout", folder_path], check=True, cwd=folder_path)
+            # Run 'git pull' in the specified folder
+            subprocess.run(["git", "pull"], check=True, cwd=folder_path)
+            print("Git pull successful in", folder_path)
+        except subprocess.CalledProcessError as e:
+            print("Error occurred while executing Git pull:", e)
+            # Handle any specific error handling here if required
+
 class File64BitsManager:
 
     @staticmethod
     def raw_b64_img(image) -> str:
         try:
             from PIL import Image, PngImagePlugin
             import io
```

### Comparing `lollms-2.2.8/lollms.egg-info/PKG-INFO` & `lollms-2.3.0/lollms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.2.8
+Version: 2.3.0
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.2.8/lollms.egg-info/SOURCES.txt` & `lollms-2.3.0/lollms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lollms-2.2.8/setup.py` & `lollms-2.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if file_path.is_file():
             if file_path.name != "__pycache__" and file_path.suffix !=".pyc" and  file_path.name!="local_config.yaml" and file_path.name!=".installed" and file_path.name!=".git" and file_path.name!=".gitignore":
                 file_list.append("/".join(str(file_path).replace("\\","/").split("/")[1:]))
     return file_list
 
 setuptools.setup(
     name="lollms",
-    version="2.2.8",
+    version="2.3.0",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
```

