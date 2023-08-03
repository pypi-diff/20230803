# Comparing `tmp/whatsapp-converter-0.6.1.tar.gz` & `tmp/whatsapp-converter-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-converter-0.6.1.tar", last modified: Sun Jul  3 19:16:31 2022, max compression
+gzip compressed data, was "whatsapp-converter-0.6.3.tar", last modified: Thu Aug  3 12:19:32 2023, max compression
```

## Comparing `whatsapp-converter-0.6.1.tar` & `whatsapp-converter-0.6.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-03 19:16:31.545189 whatsapp-converter-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1069 2022-07-03 19:16:13.000000 whatsapp-converter-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     5056 2022-07-03 19:16:31.545189 whatsapp-converter-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4141 2022-07-03 19:16:13.000000 whatsapp-converter-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-07-03 19:16:31.545189 whatsapp-converter-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1757 2022-07-03 19:16:13.000000 whatsapp-converter-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-03 19:16:31.545189 whatsapp-converter-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-03 19:16:13.000000 whatsapp-converter-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      514 2022-07-03 19:16:13.000000 whatsapp-converter-0.6.1/tests/test_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-03 19:16:31.545189 whatsapp-converter-0.6.1/whatsapp_converter/
--rw-r--r--   0 runner    (1001) docker     (116)      104 2022-07-03 19:16:13.000000 whatsapp-converter-0.6.1/whatsapp_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2859 2022-07-03 19:16:13.000000 whatsapp-converter-0.6.1/whatsapp_converter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      287 2022-07-03 19:16:13.000000 whatsapp-converter-0.6.1/whatsapp_converter/colors.py
--rw-r--r--   0 runner    (1001) docker     (116)      123 2022-07-03 19:16:13.000000 whatsapp-converter-0.6.1/whatsapp_converter/version.py
--rw-r--r--   0 runner    (1001) docker     (116)    11375 2022-07-03 19:16:13.000000 whatsapp-converter-0.6.1/whatsapp_converter/whatsapp_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-03 19:16:31.545189 whatsapp-converter-0.6.1/whatsapp_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5056 2022-07-03 19:16:30.000000 whatsapp-converter-0.6.1/whatsapp_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      480 2022-07-03 19:16:31.000000 whatsapp-converter-0.6.1/whatsapp_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-07-03 19:16:30.000000 whatsapp-converter-0.6.1/whatsapp_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       72 2022-07-03 19:16:31.000000 whatsapp-converter-0.6.1/whatsapp_converter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       40 2022-07-03 19:16:31.000000 whatsapp-converter-0.6.1/whatsapp_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       25 2022-07-03 19:16:31.000000 whatsapp-converter-0.6.1/whatsapp_converter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:19:32.679329 whatsapp-converter-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-03 12:19:32.679329 whatsapp-converter-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:19:32.679329 whatsapp-converter-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:19:32.675329 whatsapp-converter-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:19:32.679329 whatsapp-converter-0.6.3/whatsapp_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/whatsapp_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/whatsapp_converter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/whatsapp_converter/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/whatsapp_converter/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-08-03 12:19:18.000000 whatsapp-converter-0.6.3/whatsapp_converter/whatsapp_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:19:32.679329 whatsapp-converter-0.6.3/whatsapp_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-03 12:19:32.000000 whatsapp-converter-0.6.3/whatsapp_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-03 12:19:32.000000 whatsapp-converter-0.6.3/whatsapp_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:19:32.000000 whatsapp-converter-0.6.3/whatsapp_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 12:19:32.000000 whatsapp-converter-0.6.3/whatsapp_converter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-03 12:19:32.000000 whatsapp-converter-0.6.3/whatsapp_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 12:19:32.000000 whatsapp-converter-0.6.3/whatsapp_converter.egg-info/top_level.txt
```

### Comparing `whatsapp-converter-0.6.1/LICENSE` & `whatsapp-converter-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-converter-0.6.1/PKG-INFO` & `whatsapp-converter-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: whatsapp-converter
-Version: 0.6.1
+Version: 0.6.3
 Summary: Use whatsapp-converter to convert your exported WhatsApp chat to a CSV or XLS (Excel spreadsheet) file.
 Home-page: https://github.com/sandsturm/whatsapp-converter
 Author: Martin Sand
 Author-email: marti.sand.dev@gmail.com
 License: LICENSE.txt
 Project-URL: Source, https://github.com/sandsturm/whatsapp-converter/
 Project-URL: Bug Reports, https://github.com/sandsturm/whatsapp-converter/issues
 Keywords: whatsapp text converter conversion analysis
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Text Processing
 Requires-Python: >=3
```

### Comparing `whatsapp-converter-0.6.1/README.md` & `whatsapp-converter-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp-converter-0.6.1/setup.py` & `whatsapp-converter-0.6.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     install_requires=[
         'tqdm',
         'pyexcel',
         'pyexcel-xlsxw',
         'pyexcel-ods3'
     ],
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: End Users/Desktop",
         "Topic :: Text Processing",
     ],
```

### Comparing `whatsapp-converter-0.6.1/tests/test_parse.py` & `whatsapp-converter-0.6.3/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `whatsapp-converter-0.6.1/whatsapp_converter/__main__.py` & `whatsapp-converter-0.6.3/whatsapp_converter/__main__.py`

 * *Files identical despite different names*

### Comparing `whatsapp-converter-0.6.1/whatsapp_converter/whatsapp_converter.py` & `whatsapp-converter-0.6.3/whatsapp_converter/whatsapp_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import sys
 import re
 import datetime
 from datetime import date
 import pyexcel
 from tqdm import tqdm
 
-from whatsapp_converter.colors import BCOLORS
 
 # ---------------------------------------------
 # The main regex logic to identify the date and message
 pattern_date = '^\[?((\d{1,2})([\/|\.])(\d{1,2})[\/|\.](\d{1,4}))\,?\ (\d{1,2}[:|.]\d{1,2})([:|.]\d{1,2})?\ ?(AM|PM|am|pm)?([\:\ |\ \-\ |\]\ ][^:])'
 pattern = pattern_date + '(.+?)\:\ (.*)'
 
 lastentry = {
@@ -56,26 +55,26 @@
 def parse(line, filename, resultset, newline, verbose, debug):
     '''Parse each line
 
     line = Single line to parse
     args = Arguments from the command line. In this case only verbose and debug switches.
     '''
 
+    # ---------------------------------------------
+    # The main regex logic to identify the date and message
+    pattern_date = re.compile('^\[?((\d{1,2})([\/|\.])(\d{1,2})[\/|\.](\d{1,4}))\,?\ (\d{1,2}[:|.]\d{1,2})([:|.]\d{1,2})?\ ?(AM|PM|am|pm)?([\:\ |\ \-\ |\]\ ][^:])(.+?)\:\ (.*)')
+    match = pattern_date.match(line)
     dataset = ['empty', '', '', '', '', '']
 
     # ---------------------------------------------
     # if verbose: print(prefix + line)
     # if verbose: print(BCOLORS.FAIL + prefix + line)
     # Identify the date format in the chat line
 
-    if re.match(re.compile(pattern, re.VERBOSE), line):
-
-        # ---------------------------------------------
-        # Make the match, assign to the groups
-        match = re.match(re.compile(pattern, re.VERBOSE), line)
+    if match:
 
         if match and match.group(10) !=  'M':
 
             date = datetime.datetime.strptime(match.group(1), date_formats["date_format"]).date()
 
             if match.group(8):
                 time = datetime.datetime.strptime(match.group(6) + " " + match.group(8), "%I:%M %p").time()
@@ -144,24 +143,16 @@
     if debug:
         print("Debug turned on")
 
     try:
         with io.open(filename, "r", encoding="utf-8") as file:
             print("Reading import file")
 
-            content = []
-
-            for line in file:
-                # ---------------------------------------------
-                # Explicetly opened the file two times to show progress in user interface
-                line_count += 1
-
-                # ---------------------------------------------
-                # Read lines into a list
-                content.append(line)
+            content = file.readlines()  # Read all lines at once
+            line_count = len(content)  # Get the number of read lines
 
                 if re.match(re.compile(pattern, re.VERBOSE), line):
 
                     # ---------------------------------------------
                     # Make the match, assign to the groups
                     match = re.match(re.compile(pattern, re.VERBOSE), line)
```

### Comparing `whatsapp-converter-0.6.1/whatsapp_converter.egg-info/PKG-INFO` & `whatsapp-converter-0.6.3/whatsapp_converter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: whatsapp-converter
-Version: 0.6.1
+Version: 0.6.3
 Summary: Use whatsapp-converter to convert your exported WhatsApp chat to a CSV or XLS (Excel spreadsheet) file.
 Home-page: https://github.com/sandsturm/whatsapp-converter
 Author: Martin Sand
 Author-email: marti.sand.dev@gmail.com
 License: LICENSE.txt
 Project-URL: Source, https://github.com/sandsturm/whatsapp-converter/
 Project-URL: Bug Reports, https://github.com/sandsturm/whatsapp-converter/issues
 Keywords: whatsapp text converter conversion analysis
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Text Processing
 Requires-Python: >=3
```

