# Comparing `tmp/fwdviewpy-0.2.3.tar.gz` & `tmp/fwdviewpy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fwdviewpy-0.2.3.tar", last modified: Wed Aug  2 14:56:09 2023, max compression
+gzip compressed data, was "fwdviewpy-0.2.4.tar", last modified: Wed Aug  2 16:04:24 2023, max compression
```

## Comparing `fwdviewpy-0.2.3.tar` & `fwdviewpy-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 14:56:09.878865 fwdviewpy-0.2.3/
--rw-rw-rw-   0        0        0      620 2023-08-02 14:56:09.877852 fwdviewpy-0.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 14:56:09.854268 fwdviewpy-0.2.3/fwdviewpy/
--rw-rw-rw-   0        0        0      135 2023-07-05 15:13:34.000000 fwdviewpy-0.2.3/fwdviewpy/__init__.py
--rw-rw-rw-   0        0        0    34164 2023-08-02 14:39:53.000000 fwdviewpy-0.2.3/fwdviewpy/main.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:56:09.876263 fwdviewpy-0.2.3/fwdviewpy.egg-info/
--rw-rw-rw-   0        0        0      620 2023-08-02 14:56:09.000000 fwdviewpy-0.2.3/fwdviewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-08-02 14:56:09.000000 fwdviewpy-0.2.3/fwdviewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 14:56:09.000000 fwdviewpy-0.2.3/fwdviewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-02 14:56:09.000000 fwdviewpy-0.2.3/fwdviewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-02 14:56:09.000000 fwdviewpy-0.2.3/fwdviewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 14:56:09.879179 fwdviewpy-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      818 2023-08-02 14:56:04.000000 fwdviewpy-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:04:24.379011 fwdviewpy-0.2.4/
+-rw-rw-rw-   0        0        0      620 2023-08-02 16:04:24.379011 fwdviewpy-0.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 16:04:24.344272 fwdviewpy-0.2.4/fwdviewpy/
+-rw-rw-rw-   0        0        0      135 2023-07-05 15:13:34.000000 fwdviewpy-0.2.4/fwdviewpy/__init__.py
+-rw-rw-rw-   0        0        0    34323 2023-08-02 16:02:32.000000 fwdviewpy-0.2.4/fwdviewpy/main.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:04:24.375468 fwdviewpy-0.2.4/fwdviewpy.egg-info/
+-rw-rw-rw-   0        0        0      620 2023-08-02 16:04:24.000000 fwdviewpy-0.2.4/fwdviewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-08-02 16:04:24.000000 fwdviewpy-0.2.4/fwdviewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 16:04:24.000000 fwdviewpy-0.2.4/fwdviewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 16:04:24.000000 fwdviewpy-0.2.4/fwdviewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-02 16:04:24.000000 fwdviewpy-0.2.4/fwdviewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 16:04:24.380784 fwdviewpy-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      818 2023-08-02 16:04:16.000000 fwdviewpy-0.2.4/setup.py
```

### Comparing `fwdviewpy-0.2.3/PKG-INFO` & `fwdviewpy-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwdviewpy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python package developed by FWD View - The Data Transformation Specialists.
 Author: Cameron Bose & Ryan Springett
 Author-email: cameron.bose@fwdview.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `fwdviewpy-0.2.3/fwdviewpy/main.py` & `fwdviewpy-0.2.4/fwdviewpy/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import sys
 import requests
 import time 
 import json
 import datetime
 import subprocess
+import os
 
 class RunScriptManager:
     def __init__(self,databaseType,DATABASE_NAME,PROJECT_NAME,SERVER_NAME_AND_INSTANCE=None,TNS_ENTRY=None,slackEndpoint=None,START_STEP=1,LAST_STEP=100):
         """
         This class is used to execute the pre and post scripts for the masking runs. 
 
         Args:
@@ -19,15 +20,16 @@
             TNS_ENTRY (str, optional): This is the TNS Entry, needed for Oracle databases. Defaults to None.
             slackEndpoint (str, optional): This is the endpoint for the slack channel you want to send your alerts to. Defaults to None.
             START_STEP (int, optional): This is the stage at which the user wants the script to start from. 
             LAST_STEP (int, optional): This is the stage at which the user wants the script to stop before.
         """        
         now = datetime.datetime.now()
         formatted_date_time = now.strftime("%Y-%m-%d")
-        logging.basicConfig(filename=f'Log_Archive/DelphixEngineSessionManager_{formatted_date_time}.log',
+        os.makedirs("Log_Archive", exist_ok=True)
+        logging.basicConfig(filename=f'Log_Archive/{PROJECT_NAME}_Masking_Run_{formatted_date_time}.log',
                             level=logging.INFO, format='%(asctime)s %(levelname)s:%(message)s', filemode='a')
         self.databaseType = databaseType 
         self.DATABASE_NAME = DATABASE_NAME
         self.PROJECT_NAME = PROJECT_NAME
         self.slackEndpoint = slackEndpoint
         self.SERVER_NAME_AND_INSTANCE = SERVER_NAME_AND_INSTANCE
         self.TNS_ENTRY = TNS_ENTRY
@@ -126,15 +128,14 @@
                 sys.exit()
         elif step < self.START_STEP:
             return True
         else:
             logging.info(f"Exiting Script as last step is: {self.LAST_STEP}.\n")
             sys.exit()
 
-
 class VirtualisationEngineSessionManager:
     def __init__(self, address, username, password, major, minor, micro, PROJECT_NAME, CONTAINER_NAME, slackEndpoint=None, START_STEP=1, LAST_STEP=100):
         """
         This class is used to execute actions on the Delphix Virtualisation Engine. 
     
         Args:
             address (str): This is the IP address of the Delphix Engine. 
@@ -147,15 +148,16 @@
             CONTAINER_NAME (str): The name of the self-service Delphix container you want to perform actions on. 
             slackEndpoint (str, optional): This is the endpoint for the slack channel you want to send your alerts to. Defaults to None.
             START_STEP (int, optional): This is the stage at which the user wants the script to start from. 
             LAST_STEP (int, optional): This is the stage at which the user wants the script to stop before.
         """        
         now = datetime.datetime.now()
         formatted_date_time = now.strftime("%Y-%m-%d")
-        logging.basicConfig(filename=f'Log_Archive/DelphixEngineSessionManager_{formatted_date_time}.log',
+        os.makedirs("Log_Archive", exist_ok=True)
+        logging.basicConfig(filename=f'Log_Archive/{PROJECT_NAME}_Masking_Run_{formatted_date_time}.log',
                             level=logging.INFO, format='%(asctime)s %(levelname)s:%(message)s', filemode='a')
         self.address = address
         self.username = username
         self.password = password
         self.major = major
         self.minor = minor
         self.micro = micro
@@ -410,15 +412,16 @@
             ENVIRONMENT_NAME (str): This is the name of the Environment. 
             slackEndpoint (str, optional): This is the endpoint for the slack channel you want to send your alerts to. Defaults to None.
             START_STEP (int, optional): This is the stage at which the user wants the script to start from. 
             LAST_STEP (int, optional): This is the stage at which the user wants the script to stop before.
         """        
         now = datetime.datetime.now()
         formatted_date_time = now.strftime("%Y-%m-%d")
-        logging.basicConfig(filename=f'Log_Archive/DelphixEngineSessionManager_{formatted_date_time}.log',
+        os.makedirs("Log_Archive", exist_ok=True)
+        logging.basicConfig(filename=f'Log_Archive/{PROJECT_NAME}_Masking_Run_{formatted_date_time}.log',
                             level=logging.INFO, format='%(asctime)s %(levelname)s:%(message)s', filemode='a')
         self.address=address 
         self.username=username
         self.password=password
         self.PROJECT_NAME=PROJECT_NAME
         self.ENVIRONMENT_NAME=ENVIRONMENT_NAME
         self.slackEndpoint=slackEndpoint
```

### Comparing `fwdviewpy-0.2.3/fwdviewpy.egg-info/PKG-INFO` & `fwdviewpy-0.2.4/fwdviewpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwdviewpy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python package developed by FWD View - The Data Transformation Specialists.
 Author: Cameron Bose & Ryan Springett
 Author-email: cameron.bose@fwdview.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `fwdviewpy-0.2.3/setup.py` & `fwdviewpy-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fwdviewpy',
-    version='0.2.03',
+    version='0.2.04',
     description='Python package developed by FWD View - The Data Transformation Specialists.',
     long_description='Python package developed by FWD View to automate actions on both the Delphix Virtualization engine and Delphix Continuous Compliance engine.',
     packages=find_packages(),
     author='Cameron Bose & Ryan Springett',
     author_email="cameron.bose@fwdview.com",
 
     install_requires=[
```

