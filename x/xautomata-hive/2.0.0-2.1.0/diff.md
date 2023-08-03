# Comparing `tmp/xautomata-hive-2.0.0.tar.gz` & `tmp/xautomata-hive-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xautomata-hive-2.0.0.tar", last modified: Thu Aug  3 07:51:21 2023, max compression
+gzip compressed data, was "xautomata-hive-2.1.0.tar", last modified: Thu Aug  3 14:09:33 2023, max compression
```

## Comparing `xautomata-hive-2.0.0.tar` & `xautomata-hive-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:51:21.849428 xautomata-hive-2.0.0/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-08-03 07:51:21.000000 xautomata-hive-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10656 2023-08-03 07:51:21.849428 xautomata-hive-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10385 2023-08-03 07:51:21.000000 xautomata-hive-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:51:21.845428 xautomata-hive-2.0.0/hive/
--rw-r--r--   0 root         (0) root         (0)       68 2023-08-03 07:51:21.000000 xautomata-hive-2.0.0/hive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32021 2023-08-03 07:51:21.000000 xautomata-hive-2.0.0/hive/api.py
--rw-r--r--   0 root         (0) root         (0)     8770 2023-08-03 07:51:21.000000 xautomata-hive-2.0.0/hive/decorators.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-08-03 07:51:21.000000 xautomata-hive-2.0.0/hive/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3570 2023-08-03 07:51:21.000000 xautomata-hive-2.0.0/hive/infrastrucure_keys.py
--rw-r--r--   0 root         (0) root         (0)       17 2023-08-03 07:51:21.000000 xautomata-hive-2.0.0/hive/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 07:51:21.849428 xautomata-hive-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      884 2023-08-03 07:51:21.000000 xautomata-hive-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:51:21.849428 xautomata-hive-2.0.0/xautomata_hive.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10656 2023-08-03 07:51:21.000000 xautomata-hive-2.0.0/xautomata_hive.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      325 2023-08-03 07:51:21.000000 xautomata-hive-2.0.0/xautomata_hive.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 07:51:21.000000 xautomata-hive-2.0.0/xautomata_hive.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-08-03 07:51:21.000000 xautomata-hive-2.0.0/xautomata_hive.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-08-03 07:51:21.000000 xautomata-hive-2.0.0/xautomata_hive.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 14:09:33.977884 xautomata-hive-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-08-03 14:09:33.000000 xautomata-hive-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10656 2023-08-03 14:09:33.977884 xautomata-hive-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10385 2023-08-03 14:09:33.000000 xautomata-hive-2.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 14:09:33.977884 xautomata-hive-2.1.0/hive/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-08-03 14:09:33.000000 xautomata-hive-2.1.0/hive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32020 2023-08-03 14:09:33.000000 xautomata-hive-2.1.0/hive/api.py
+-rw-r--r--   0 root         (0) root         (0)     8770 2023-08-03 14:09:33.000000 xautomata-hive-2.1.0/hive/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-08-03 14:09:33.000000 xautomata-hive-2.1.0/hive/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3570 2023-08-03 14:09:33.000000 xautomata-hive-2.1.0/hive/infrastrucure_keys.py
+-rw-r--r--   0 root         (0) root         (0)       17 2023-08-03 14:09:33.000000 xautomata-hive-2.1.0/hive/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 14:09:33.977884 xautomata-hive-2.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      882 2023-08-03 14:09:33.000000 xautomata-hive-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 14:09:33.977884 xautomata-hive-2.1.0/xautomata_hive.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10656 2023-08-03 14:09:33.000000 xautomata-hive-2.1.0/xautomata_hive.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      325 2023-08-03 14:09:33.000000 xautomata-hive-2.1.0/xautomata_hive.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 14:09:33.000000 xautomata-hive-2.1.0/xautomata_hive.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-08-03 14:09:33.000000 xautomata-hive-2.1.0/xautomata_hive.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-03 14:09:33.000000 xautomata-hive-2.1.0/xautomata_hive.egg-info/top_level.txt
```

### Comparing `xautomata-hive-2.0.0/LICENSE` & `xautomata-hive-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.0.0/PKG-INFO` & `xautomata-hive-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xautomata-hive
-Version: 2.0.0
+Version: 2.1.0
 Home-page: https://github.com/sherlogic/xautomata-hive.git
 Author: Enrico Ferro - Andrea Jacassi
 Author-email: 
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `xautomata-hive-2.0.0/README.md` & `xautomata-hive-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.0.0/hive/api.py` & `xautomata-hive-2.1.0/hive/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 def get_session():
     """
     Add retry logic and policies about methods and statuses for requests
     """
     ss = requests.Session()
-    retry_strategy = Retry(connect=3, total=3, status_forcelist=FORCE_STATUS, method_whitelist=METHODS)
+    retry_strategy = Retry(connect=3, total=3, status_forcelist=FORCE_STATUS, allowed_methods=METHODS)
     ss.mount('https://', HTTPAdapter(max_retries=retry_strategy))
     ss.mount('http://', HTTPAdapter(max_retries=retry_strategy))
     return ss
 
 
 class ApiManager:
     """
```

### Comparing `xautomata-hive-2.0.0/hive/decorators.py` & `xautomata-hive-2.1.0/hive/decorators.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.0.0/hive/infrastrucure_keys.py` & `xautomata-hive-2.1.0/hive/infrastrucure_keys.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.0.0/setup.py` & `xautomata-hive-2.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 with open("hive/version.py", "r") as f:
     for line in f:
         version.append(str(line.strip()))
 
 version = version[0].split("'")[1]
 
 # version go
+requests = 'requests==2.31.0'
+urllib3 = 'urllib3==2.0.4'
 tqdm = 'tqdm==4.64.1'
-urllib3 = 'urllib3==1.26.13'
-requests = 'requests==2.28.1'
 # version end
 
 setup(
     name='xautomata-hive',
     python_requires='>=3.8.0',
     version=version,
     packages=find_packages(include=['hive']),
```

### Comparing `xautomata-hive-2.0.0/xautomata_hive.egg-info/PKG-INFO` & `xautomata-hive-2.1.0/xautomata_hive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xautomata-hive
-Version: 2.0.0
+Version: 2.1.0
 Home-page: https://github.com/sherlogic/xautomata-hive.git
 Author: Enrico Ferro - Andrea Jacassi
 Author-email: 
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

