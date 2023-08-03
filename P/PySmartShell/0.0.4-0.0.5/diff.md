# Comparing `tmp/PySmartShell-0.0.4.tar.gz` & `tmp/PySmartShell-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySmartShell-0.0.4.tar", last modified: Tue Nov  1 19:22:14 2022, max compression
+gzip compressed data, was "PySmartShell-0.0.5.tar", last modified: Thu Aug  3 08:54:09 2023, max compression
```

## Comparing `PySmartShell-0.0.4.tar` & `PySmartShell-0.0.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2022-11-01 19:22:14.955222 PySmartShell-0.0.4/
--rw-rw-r--   0 mirko     (1000) mirko     (1000)        0 2022-11-01 17:31:07.000000 PySmartShell-0.0.4/LICENCE
--rw-rw-r--   0 mirko     (1000) mirko     (1000)        0 2022-11-01 17:31:01.000000 PySmartShell-0.0.4/MANIFEST.in
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      306 2022-11-01 19:22:14.955222 PySmartShell-0.0.4/PKG-INFO
--rw-rw-r--   0 mirko     (1000) mirko     (1000)     5425 2022-11-01 18:18:02.000000 PySmartShell-0.0.4/README.md
--rw-rw-r--   0 mirko     (1000) mirko     (1000)       38 2022-11-01 19:22:14.955222 PySmartShell-0.0.4/setup.cfg
--rw-rw-r--   0 mirko     (1000) mirko     (1000)     1197 2022-11-01 19:22:03.000000 PySmartShell-0.0.4/setup.py
-drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2022-11-01 19:22:14.951222 PySmartShell-0.0.4/src/
-drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2022-11-01 19:22:14.951222 PySmartShell-0.0.4/src/PySmartShell.egg-info/
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      306 2022-11-01 19:22:14.000000 PySmartShell-0.0.4/src/PySmartShell.egg-info/PKG-INFO
--rw-rw-r--   0 mirko     (1000) mirko     (1000)     1516 2022-11-01 19:22:14.000000 PySmartShell-0.0.4/src/PySmartShell.egg-info/SOURCES.txt
--rw-rw-r--   0 mirko     (1000) mirko     (1000)        1 2022-11-01 19:22:14.000000 PySmartShell-0.0.4/src/PySmartShell.egg-info/dependency_links.txt
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      561 2022-11-01 19:22:14.000000 PySmartShell-0.0.4/src/PySmartShell.egg-info/requires.txt
--rw-rw-r--   0 mirko     (1000) mirko     (1000)       13 2022-11-01 19:22:14.000000 PySmartShell-0.0.4/src/PySmartShell.egg-info/top_level.txt
-drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2022-11-01 19:22:14.951222 PySmartShell-0.0.4/src/pysmartshell/
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      986 2022-11-01 19:20:57.000000 PySmartShell-0.0.4/src/pysmartshell/AbstractAction.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)     1136 2022-11-01 19:13:48.000000 PySmartShell-0.0.4/src/pysmartshell/AbstractActionWithConfiguration.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      632 2022-11-01 19:13:52.000000 PySmartShell-0.0.4/src/pysmartshell/ActionLoader.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)     1518 2022-11-01 19:17:09.000000 PySmartShell-0.0.4/src/pysmartshell/ActionsLoader.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      993 2022-11-01 19:13:34.000000 PySmartShell-0.0.4/src/pysmartshell/ArgParser.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)     1090 2022-09-19 10:00:39.000000 PySmartShell-0.0.4/src/pysmartshell/Argument.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)     1223 2022-11-01 19:14:04.000000 PySmartShell-0.0.4/src/pysmartshell/ConfigurationHandler.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      103 2022-11-01 19:13:07.000000 PySmartShell-0.0.4/src/pysmartshell/__init__.py
-drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2022-11-01 19:22:14.951222 PySmartShell-0.0.4/src/pysmartshell/adaptors/
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      892 2022-09-28 21:17:44.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/InputAdaptorHandler.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)     1237 2022-09-28 21:17:51.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/OutputAdaptorHandler.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)        0 2022-09-15 09:31:37.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/__init__.py
-drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2022-11-01 19:22:14.955222 PySmartShell-0.0.4/src/pysmartshell/adaptors/input/
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      329 2022-09-20 12:35:55.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/input/AbstractInputAdaptor.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      429 2022-09-20 13:13:46.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/input/InputCSVFileAdaptor.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      445 2022-09-28 21:18:31.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/input/InputHTMLFileAdaptor.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      514 2022-09-28 21:19:24.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/input/InputJSONFileAdaptor.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      461 2022-09-28 21:19:11.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/input/InputJSONLFileAdaptor.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      443 2022-09-28 21:18:22.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/input/InputTextFileAdaptor.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      390 2022-09-20 13:13:40.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/input/InputURLAdaptor.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)        0 2022-09-19 13:51:06.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/input/__init__.py
-drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2022-11-01 19:22:14.955222 PySmartShell-0.0.4/src/pysmartshell/adaptors/output/
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      331 2022-09-20 14:15:11.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/output/AbstractOutputAdaptor.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      437 2022-09-20 14:15:05.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/output/OutputCSVFileAdaptor.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      364 2022-09-28 21:18:06.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/output/OutputHTMLFileAdaptor.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      378 2022-09-28 21:19:40.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/output/OutputJSONFileAdaptor.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      427 2022-09-28 21:19:45.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/output/OutputJSONLFileAdaptor.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)      375 2022-09-28 21:18:12.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/output/OutputTextFileAdaptor.py
--rw-rw-r--   0 mirko     (1000) mirko     (1000)        0 2022-09-19 13:51:14.000000 PySmartShell-0.0.4/src/pysmartshell/adaptors/output/__init__.py
-drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2022-11-01 19:22:14.955222 PySmartShell-0.0.4/src/pysmartshell/tests/
--rw-rw-r--   0 mirko     (1000) mirko     (1000)        0 2022-09-21 08:27:08.000000 PySmartShell-0.0.4/src/pysmartshell/tests/__init__.py
+drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2023-08-03 08:54:09.114435 PySmartShell-0.0.5/
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)        0 2022-11-01 17:31:07.000000 PySmartShell-0.0.5/LICENCE
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)        0 2022-11-01 17:31:01.000000 PySmartShell-0.0.5/MANIFEST.in
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      306 2023-08-03 08:54:09.110435 PySmartShell-0.0.5/PKG-INFO
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)     5425 2022-11-01 18:18:02.000000 PySmartShell-0.0.5/README.md
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)       38 2023-08-03 08:54:09.114435 PySmartShell-0.0.5/setup.cfg
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)     1322 2023-08-03 08:20:18.000000 PySmartShell-0.0.5/setup.py
+drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2023-08-03 08:54:09.106435 PySmartShell-0.0.5/src/
+drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2023-08-03 08:54:09.110435 PySmartShell-0.0.5/src/PySmartShell.egg-info/
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      306 2023-08-03 08:54:09.000000 PySmartShell-0.0.5/src/PySmartShell.egg-info/PKG-INFO
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)     1516 2023-08-03 08:54:09.000000 PySmartShell-0.0.5/src/PySmartShell.egg-info/SOURCES.txt
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)        1 2023-08-03 08:54:09.000000 PySmartShell-0.0.5/src/PySmartShell.egg-info/dependency_links.txt
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      561 2023-08-03 08:54:09.000000 PySmartShell-0.0.5/src/PySmartShell.egg-info/requires.txt
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)       13 2023-08-03 08:54:09.000000 PySmartShell-0.0.5/src/PySmartShell.egg-info/top_level.txt
+drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2023-08-03 08:54:09.110435 PySmartShell-0.0.5/src/pysmartshell/
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)     1055 2023-08-03 08:17:20.000000 PySmartShell-0.0.5/src/pysmartshell/AbstractAction.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)     1230 2023-08-03 08:17:13.000000 PySmartShell-0.0.5/src/pysmartshell/AbstractActionWithConfiguration.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      740 2023-08-03 08:17:04.000000 PySmartShell-0.0.5/src/pysmartshell/ActionLoader.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)     1815 2023-08-03 08:19:07.000000 PySmartShell-0.0.5/src/pysmartshell/ActionsLoader.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)     1283 2023-08-03 08:17:29.000000 PySmartShell-0.0.5/src/pysmartshell/ArgParser.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)     1273 2023-08-03 08:17:36.000000 PySmartShell-0.0.5/src/pysmartshell/Argument.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)     1338 2023-08-03 08:17:41.000000 PySmartShell-0.0.5/src/pysmartshell/ConfigurationHandler.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      103 2022-11-01 19:13:07.000000 PySmartShell-0.0.5/src/pysmartshell/__init__.py
+drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2023-08-03 08:54:09.110435 PySmartShell-0.0.5/src/pysmartshell/adaptors/
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      892 2022-09-28 21:17:44.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/InputAdaptorHandler.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)     1237 2022-09-28 21:17:51.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/OutputAdaptorHandler.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)        0 2022-09-15 09:31:37.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/__init__.py
+drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2023-08-03 08:54:09.110435 PySmartShell-0.0.5/src/pysmartshell/adaptors/input/
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      329 2022-09-20 12:35:55.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/input/AbstractInputAdaptor.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      429 2022-09-20 13:13:46.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/input/InputCSVFileAdaptor.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      445 2022-09-28 21:18:31.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/input/InputHTMLFileAdaptor.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      514 2022-09-28 21:19:24.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/input/InputJSONFileAdaptor.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      461 2022-09-28 21:19:11.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/input/InputJSONLFileAdaptor.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      443 2022-09-28 21:18:22.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/input/InputTextFileAdaptor.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      390 2022-09-20 13:13:40.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/input/InputURLAdaptor.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)        0 2022-09-19 13:51:06.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/input/__init__.py
+drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2023-08-03 08:54:09.110435 PySmartShell-0.0.5/src/pysmartshell/adaptors/output/
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      331 2022-09-20 14:15:11.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/output/AbstractOutputAdaptor.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      437 2022-09-20 14:15:05.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/output/OutputCSVFileAdaptor.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      364 2022-09-28 21:18:06.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/output/OutputHTMLFileAdaptor.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      378 2022-09-28 21:19:40.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/output/OutputJSONFileAdaptor.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      427 2022-09-28 21:19:45.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/output/OutputJSONLFileAdaptor.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)      375 2022-09-28 21:18:12.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/output/OutputTextFileAdaptor.py
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)        0 2022-09-19 13:51:14.000000 PySmartShell-0.0.5/src/pysmartshell/adaptors/output/__init__.py
+drwxrwxr-x   0 mirko     (1000) mirko     (1000)        0 2023-08-03 08:54:09.110435 PySmartShell-0.0.5/src/pysmartshell/tests/
+-rw-rw-r--   0 mirko     (1000) mirko     (1000)        0 2022-09-21 08:27:08.000000 PySmartShell-0.0.5/src/pysmartshell/tests/__init__.py
```

### Comparing `PySmartShell-0.0.4/README.md` & `PySmartShell-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `PySmartShell-0.0.4/setup.py` & `PySmartShell-0.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
-  name = 'PySmartShell',
-  version = '0.0.4',
-  description = 'PySmartShell is a quick context creator provider for command creation',
-  python_requires = '>3.10.0',
-  author = 'Colageo Mirko',
-  author_email = 'mirko.colageo@gmail.com',
-  install_requires = [
-    "bleach==5.0.1",
-    "certifi==2022.9.24",
-    "cffi==1.15.1",
-    "charset-normalizer==2.1.1",
-    "commonmark==0.9.1",
-    "cryptography==38.0.1",
-    "decorator==5.1.1",
-    "docutils==0.19",
-    "idna==3.4",
-    "importlib-metadata==5.0.0",
-    "jaraco.classes==3.2.3",
-    "jeepney==0.8.0",
-    "keyring==23.9.3",
-    "more-itertools==9.0.0",
-    "numpy==1.23.4",
-    "pandas==1.5.1",
-    "pkginfo==1.8.3",
-    "pycparser==2.21",
-    "Pygments==2.13.0",
-    "python-dateutil==2.8.2",
-    "pytz==2022.6",
-    "readme-renderer==37.3",
-    "requests==2.28.1",
-    "requests-toolbelt==0.10.1",
-    "rfc3986==2.0.0",
-    "rich==12.6.0",
-    "SecretStorage==3.3.3",
-    "six==1.16.0",
-    "urllib3==1.26.12",
-    "validators==0.20.0",
-    "webencodings==0.5.1",
-    "zipp==3.10.0",
-  ],
-  
-  package_dir = { '':'src' },
-  packages = find_packages('src'),
-)  
+    name="PySmartShell",
+    version="0.0.5",
+    description="PySmartShell is a quick context creator provider for command creation",
+    python_requires=">3.10.0",
+    author="Colageo Mirko",
+    author_email="mirko.colageo@gmail.com",
+    install_requires=[
+        "bleach==5.0.1",
+        "certifi==2022.9.24",
+        "cffi==1.15.1",
+        "charset-normalizer==2.1.1",
+        "commonmark==0.9.1",
+        "cryptography==38.0.1",
+        "decorator==5.1.1",
+        "docutils==0.19",
+        "idna==3.4",
+        "importlib-metadata==5.0.0",
+        "jaraco.classes==3.2.3",
+        "jeepney==0.8.0",
+        "keyring==23.9.3",
+        "more-itertools==9.0.0",
+        "numpy==1.23.4",
+        "pandas==1.5.1",
+        "pkginfo==1.8.3",
+        "pycparser==2.21",
+        "Pygments==2.13.0",
+        "python-dateutil==2.8.2",
+        "pytz==2022.6",
+        "readme-renderer==37.3",
+        "requests==2.28.1",
+        "requests-toolbelt==0.10.1",
+        "rfc3986==2.0.0",
+        "rich==12.6.0",
+        "SecretStorage==3.3.3",
+        "six==1.16.0",
+        "urllib3==1.26.12",
+        "validators==0.20.0",
+        "webencodings==0.5.1",
+        "zipp==3.10.0",
+    ],
+    package_dir={"": "src"},
+    packages=find_packages("src"),
+)
```

### Comparing `PySmartShell-0.0.4/src/PySmartShell.egg-info/SOURCES.txt` & `PySmartShell-0.0.5/src/PySmartShell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySmartShell-0.0.4/src/PySmartShell.egg-info/requires.txt` & `PySmartShell-0.0.5/src/PySmartShell.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `PySmartShell-0.0.4/src/pysmartshell/AbstractAction.py` & `PySmartShell-0.0.5/src/pysmartshell/AbstractAction.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,37 +2,36 @@
 from argparse import Namespace
 from abc import ABC, abstractmethod
 
 from .Argument import Argument
 from .adaptors.InputAdaptorHandler import InputAdaptorHandler
 from .adaptors.OutputAdaptorHandler import OutputAdaptorHandler
 
-class AbstractAction(ABC):
-  name:str
-  helpInfo:str
 
-  def getArgs(self, args:Namespace) -> dict:
-    toRet = {}
-    for key, value in args._get_kwargs():
-      toRet[key] = value
-    return toRet
-
-  @staticmethod
-  def getArgsSchema() -> list[Argument]:
-    return []
-
-  def execute(self, args:Namespace):
-    dictArgs = self.getArgs(args)
-    logging.debug(f'{self.name}.execute started with args', dictArgs)
-    return self.executeVertical(dictArgs)
-
-  @abstractmethod
-  def executeVertical(self, args:dict):
-    raise NotImplementedError
+class AbstractAction(ABC):
+    name: str
+    helpInfo: str
 
-  def open(self, inputData):
-    return InputAdaptorHandler.withInput(inputData).getContent()
+    def getArgs(self, args: Namespace) -> dict:
+        toRet = {}
+        for key, value in args._get_kwargs():
+            toRet[key] = value
+        return toRet
+
+    @staticmethod
+    def getArgsSchema() -> list[Argument]:
+        return []
+
+    def execute(self, args: Namespace):
+        dictArgs = self.getArgs(args)
+        logging.debug(f"{self.name}.execute started with args", dictArgs)
+        return self.executeVertical(dictArgs)
+
+    @abstractmethod
+    def executeVertical(self, args: dict):
+        raise NotImplementedError
 
-  def saveAs(self, data, filePath:str):
-    return OutputAdaptorHandler.withFile(filePath).save(data)
+    def open(self, inputData):
+        return InputAdaptorHandler.withInput(inputData).getContent()
 
-  
+    def saveAs(self, data, filePath: str):
+        return OutputAdaptorHandler.withFile(filePath).save(data)
```

### Comparing `PySmartShell-0.0.4/src/pysmartshell/AbstractActionWithConfiguration.py` & `PySmartShell-0.0.5/src/pysmartshell/AbstractActionWithConfiguration.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,36 +3,37 @@
 
 from .Argument import Argument
 from .AbstractAction import AbstractAction
 from .ConfigurationHandler import ConfigurationHandler
 
 
 class AbstractActionWithConfiguration(AbstractAction):
-  confHandler:ConfigurationHandler
+    confHandler: ConfigurationHandler
 
-  def __init__(self):
-    super().__init__()
-    self.confHandler = ConfigurationHandler(self.name)
-
-  @staticmethod
-  def getArgsSchema() -> list[Argument]:
-    return [
-      Argument.create(longCommand='--set-conf'),
-      Argument.create(longCommand='--get-conf'),
-    ]
-
-  def execute(self, args:Namespace):
-    logging.debug(f'{self.name}.execute started with args', self.getArgs(args))
-
-    dictArgs = self.getArgs(args)
-    if dictArgs.get('get_conf'):
-      return self.getConfiguration(dictArgs.get('get_conf'))
-
-    if dictArgs.get('set_conf'):
-      return self.confHandler.set(dictArgs.get('set_conf'))
-    
-    return self.executeVertical(dictArgs)
-
-  def getConfiguration(self, key:str):
-    confValue = self.confHandler.get(f'{self.name}:{key}')
-    if confValue: return confValue
-    raise Exception(f'Missing required configuration for key {key}') 
+    def __init__(self):
+        super().__init__()
+        self.confHandler = ConfigurationHandler(self.name)
+
+    @staticmethod
+    def getArgsSchema() -> list[Argument]:
+        return [
+            Argument.create(longCommand="--set-conf"),
+            Argument.create(longCommand="--get-conf"),
+        ]
+
+    def execute(self, args: Namespace):
+        logging.debug(f"{self.name}.execute started with args", self.getArgs(args))
+
+        dictArgs = self.getArgs(args)
+        if dictArgs.get("get_conf"):
+            return self.getConfiguration(dictArgs.get("get_conf"))
+
+        if dictArgs.get("set_conf"):
+            return self.confHandler.set(dictArgs.get("set_conf"))
+
+        return self.executeVertical(dictArgs)
+
+    def getConfiguration(self, key: str):
+        confValue = self.confHandler.get(f"{self.name}:{key}")
+        if confValue:
+            return confValue
+        raise Exception(f"Missing required configuration for key {key}")
```

### Comparing `PySmartShell-0.0.4/src/pysmartshell/ActionLoader.py` & `PySmartShell-0.0.5/src/pysmartshell/ActionLoader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import sys
 import logging
 import pkgutil
 
 from .AbstractAction import AbstractAction
 
-class ActionLoader:
 
-  @staticmethod
-  def loadFrom(directoryPath:str) -> list[AbstractAction]:
-    sys.path.append(directoryPath)
-
-    packages = []
-    for package in pkgutil.iter_modules([directoryPath]):
-      if not package.ispkg: continue
-
-      packages.append( 
-        getattr(
-          getattr(
-            __import__( package.name, fromlist = [package.name]),
-            package.name
-          ),
-          package.name
-        )()
-      )
-      logging.debug(f'loaded action {package.name}')
+class ActionLoader:
+    @staticmethod
+    def loadFrom(directoryPath: str) -> list[AbstractAction]:
+        sys.path.append(directoryPath)
+
+        packages = []
+        for package in pkgutil.iter_modules([directoryPath]):
+            if not package.ispkg:
+                continue
+
+            packages.append(
+                getattr(
+                    getattr(
+                        __import__(package.name, fromlist=[package.name]), package.name
+                    ),
+                    package.name,
+                )()
+            )
+            logging.debug(f"loaded action {package.name}")
 
-    sys.path.pop()
-    return packages
+        sys.path.pop()
+        return packages
```

### Comparing `PySmartShell-0.0.4/src/pysmartshell/ActionsLoader.py` & `PySmartShell-0.0.5/src/pysmartshell/ActionsLoader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,58 @@
 import os
 import sys
 import logging
 from os.path import join
 
-from .ArgParser import ArgParser 
+from .ArgParser import ArgParser
 from .ActionLoader import ActionLoader
 from .AbstractAction import AbstractAction
 from .ConfigurationHandler import ConfigurationHandler
 
-def ActionsLoader(unparsed_args):
-  try:
-    folderPath = join(os.getcwd(), ConfigurationHandler().get('actionsPath'))
-  except:
-    folderPath = join(os.getcwd(), 'actions')
-
-  actions:list[AbstractAction] = ActionLoader.loadFrom(folderPath)
-  args = ArgParser(actions).getParser(unparsed_args)
-
-  __LOG_FILEPATH__  = join(os.getcwd(), 'logs/')
-  os.makedirs(__LOG_FILEPATH__, exist_ok=True)
-
-  logging.basicConfig(
-    level = args.log_level,
-    format = '%(asctime)s [%(levelname)s] %(name)s - %(message)s',
-    handlers = [
-      logging.FileHandler(join(__LOG_FILEPATH__, 'logger.log')),
-      logging.StreamHandler()
-    ],
-    encoding='utf-8',
-  )
-
-  if args.log_level == 'INFO':
-    sys.tracebacklimit = 0
-
-  if args.action:
-    availableActions = {}
-    for action in actions:
-      availableActions[action.name] = action
-    return availableActions.get(args.action).execute(args)
-
-  if args.set_conf:
-    ConfigurationHandler().set(args.set_conf)
-    logging.info('Requested configuration change done!')
-    return
-
-  if args.get_conf:
-    confValue = ConfigurationHandler().get(args.get_conf)
-    if confValue:
-      logging.info('Requested configuration value is:', confValue, '.')
-    else:
-      logging.info('Requested key is not setted in configuration.')
-    return
+
+def ActionsLoader(unparsed_args: list[str], configFolderPath: str = ""):
+    if not configFolderPath:
+        try:
+            configFolderPath = join(
+                os.getcwd(), ConfigurationHandler().get("actionsPath")
+            )
+        except Exception as e:
+            logging.info(e)
+            configFolderPath = join(os.getcwd(), "actions")
+
+    actions: list[AbstractAction] = ActionLoader.loadFrom(configFolderPath)
+    args = ArgParser(actions).getParser(unparsed_args)
+
+    __LOG_FILEPATH__ = join(os.getcwd(), "logs/")
+    os.makedirs(__LOG_FILEPATH__, exist_ok=True)
+
+    logging.basicConfig(
+        level=args.log_level,
+        format="%(asctime)s [%(levelname)s] %(name)s - %(message)s",
+        handlers=[
+            logging.FileHandler(join(__LOG_FILEPATH__, "logger.log")),
+            logging.StreamHandler(),
+        ],
+        encoding="utf-8",
+    )
+
+    if args.log_level == "INFO":
+        sys.tracebacklimit = 0
+
+    if args.action:
+        availableActions = {}
+        for action in actions:
+            availableActions[action.name] = action
+        return availableActions.get(args.action).execute(args)
+
+    if args.set_conf:
+        ConfigurationHandler().set(args.set_conf)
+        logging.info("Requested configuration change done!")
+        return
+
+    if args.get_conf:
+        confValue = ConfigurationHandler().get(args.get_conf)
+        if confValue:
+            logging.info("Requested configuration value is:", confValue, ".")
+        else:
+            logging.info("Requested key is not setted in configuration.")
+        return
```

### Comparing `PySmartShell-0.0.4/src/pysmartshell/ConfigurationHandler.py` & `PySmartShell-0.0.5/src/pysmartshell/ConfigurationHandler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 from os import path
 
 from .adaptors.input.InputJSONFileAdaptor import InputJSONFileAdaptor
 from .adaptors.output.OutputJSONFileAdaptor import OutputJSONFileAdaptor
 
-FILE_PATH = path.abspath(path.join(path.dirname(__file__), '../conf.json'))
+FILE_PATH = path.abspath(path.join(path.dirname(__file__), "../conf.json"))
+
 
 class ConfigurationHandler:
-  __key:str = None
-  
-  def __init__(self, key:str=None) -> None:
-    self.__key = key
-
-  def set(self, args:str):
-    configurations = self.__getConf()
-
-    vals = args.split('=')
-    if not self.__key:
-      configurations[vals[0]] = vals[1]
-    else:
-      if not self.__key in configurations:
-        configurations[self.__key] = {}
-      
-      configurations[self.__key][vals[0]] = vals[1]
-
-    OutputJSONFileAdaptor(FILE_PATH).save(configurations)
-
-  def get(self, fieldName:str):
-    configurations = self.__getConf()
-    fieldNameSplitted = fieldName.split(':')
-    if len(fieldNameSplitted) == 0: return configurations.get(fieldName)
-
-    confValue = configurations.get(fieldNameSplitted[0], {})
-    for key in fieldNameSplitted[1:]:
-      confValue = confValue.get(key, {})
-
-    return confValue
-
-  def __getConf(self) -> dict:
-    if not path.exists(FILE_PATH): 
-      return {}
+    __key: str = None
+
+    def __init__(self, key: str = None) -> None:
+        self.__key = key
+
+    def set(self, args: str):
+        configurations = self.__getConf()
+
+        vals = args.split("=")
+        if not self.__key:
+            configurations[vals[0]] = vals[1]
+        else:
+            if not self.__key in configurations:
+                configurations[self.__key] = {}
+
+            configurations[self.__key][vals[0]] = vals[1]
+
+        OutputJSONFileAdaptor(FILE_PATH).save(configurations)
+
+    def get(self, fieldName: str):
+        configurations = self.__getConf()
+        fieldNameSplitted = fieldName.split(":")
+        if len(fieldNameSplitted) == 0:
+            return configurations.get(fieldName)
+
+        confValue = configurations.get(fieldNameSplitted[0], {})
+        for key in fieldNameSplitted[1:]:
+            confValue = confValue.get(key, {})
+
+        return confValue
+
+    def __getConf(self) -> dict:
+        if not path.exists(FILE_PATH):
+            return {}
 
-    return InputJSONFileAdaptor(FILE_PATH).getContent() or {}
+        return InputJSONFileAdaptor(FILE_PATH).getContent() or {}
```

### Comparing `PySmartShell-0.0.4/src/pysmartshell/adaptors/InputAdaptorHandler.py` & `PySmartShell-0.0.5/src/pysmartshell/adaptors/InputAdaptorHandler.py`

 * *Files identical despite different names*

### Comparing `PySmartShell-0.0.4/src/pysmartshell/adaptors/OutputAdaptorHandler.py` & `PySmartShell-0.0.5/src/pysmartshell/adaptors/OutputAdaptorHandler.py`

 * *Files identical despite different names*

### Comparing `PySmartShell-0.0.4/src/pysmartshell/adaptors/input/InputJSONFileAdaptor.py` & `PySmartShell-0.0.5/src/pysmartshell/adaptors/input/InputJSONFileAdaptor.py`

 * *Files identical despite different names*

