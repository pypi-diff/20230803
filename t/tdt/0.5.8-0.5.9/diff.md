# Comparing `tmp/tdt-0.5.8.tar.gz` & `tmp/tdt-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tdt-0.5.8.tar", last modified: Fri Jun 23 20:38:53 2023, max compression
+gzip compressed data, was "dist\tdt-0.5.9.tar", last modified: Thu Aug  3 17:12:49 2023, max compression
```

## Comparing `tdt-0.5.8.tar` & `tdt-0.5.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 20:38:53.000000 tdt-0.5.8/
--rw-rw-rw-   0        0        0     1265 2023-06-23 20:38:53.000000 tdt-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-06-23 20:38:23.000000 tdt-0.5.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 20:38:53.000000 tdt-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0      740 2023-06-23 20:38:22.000000 tdt-0.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 20:38:53.000000 tdt-0.5.8/tdt/
--rw-rw-rw-   0        0        0     9386 2023-06-23 20:38:22.000000 tdt-0.5.8/tdt/BH32.py
--rw-rw-rw-   0        0        0     3202 2023-06-23 20:38:23.000000 tdt-0.5.8/tdt/PynapseUDP.py
--rw-rw-rw-   0        0        0    31632 2023-06-23 20:38:23.000000 tdt-0.5.8/tdt/SynapseAPI.py
--rw-rw-rw-   0        0        0     4989 2023-06-23 20:38:23.000000 tdt-0.5.8/tdt/TDTUDP.py
--rw-rw-rw-   0        0        0   111293 2023-06-23 20:38:22.000000 tdt-0.5.8/tdt/TDTbin2py.py
--rw-rw-rw-   0        0        0    18957 2023-06-23 20:38:23.000000 tdt-0.5.8/tdt/TDTfilter.py
--rw-rw-rw-   0        0        0     4445 2023-06-23 20:38:22.000000 tdt-0.5.8/tdt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 20:38:53.000000 tdt-0.5.8/tdt.egg-info/
--rw-rw-rw-   0        0        0     1265 2023-06-23 20:38:46.000000 tdt-0.5.8/tdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-06-23 20:38:47.000000 tdt-0.5.8/tdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 20:38:46.000000 tdt-0.5.8/tdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-23 20:38:46.000000 tdt-0.5.8/tdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-23 20:38:46.000000 tdt-0.5.8/tdt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 17:12:49.000000 tdt-0.5.9/
+-rw-rw-rw-   0        0        0     1265 2023-08-03 17:12:49.000000 tdt-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-08-03 17:12:37.000000 tdt-0.5.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 17:12:49.000000 tdt-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-08-03 17:12:37.000000 tdt-0.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 17:12:49.000000 tdt-0.5.9/tdt/
+-rw-rw-rw-   0        0        0     9386 2023-08-03 17:12:37.000000 tdt-0.5.9/tdt/BH32.py
+-rw-rw-rw-   0        0        0     3202 2023-08-03 17:12:37.000000 tdt-0.5.9/tdt/PynapseUDP.py
+-rw-rw-rw-   0        0        0    31632 2023-08-03 17:12:37.000000 tdt-0.5.9/tdt/SynapseAPI.py
+-rw-rw-rw-   0        0        0     4989 2023-08-03 17:12:37.000000 tdt-0.5.9/tdt/TDTUDP.py
+-rw-rw-rw-   0        0        0   111279 2023-08-03 17:12:37.000000 tdt-0.5.9/tdt/TDTbin2py.py
+-rw-rw-rw-   0        0        0    18957 2023-08-03 17:12:37.000000 tdt-0.5.9/tdt/TDTfilter.py
+-rw-rw-rw-   0        0        0     4445 2023-08-03 17:12:37.000000 tdt-0.5.9/tdt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 17:12:49.000000 tdt-0.5.9/tdt.egg-info/
+-rw-rw-rw-   0        0        0     1265 2023-08-03 17:12:44.000000 tdt-0.5.9/tdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-08-03 17:12:44.000000 tdt-0.5.9/tdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 17:12:44.000000 tdt-0.5.9/tdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-03 17:12:44.000000 tdt-0.5.9/tdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-03 17:12:44.000000 tdt-0.5.9/tdt.egg-info/top_level.txt
```

### Comparing `tdt-0.5.8/PKG-INFO` & `tdt-0.5.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdt
-Version: 0.5.8
+Version: 0.5.9
 Summary: Tucker-Davis Technologies (TDT) Python APIs for reading data and interacting with Synapse software
 Home-page: UNKNOWN
 Author: Mark Hanus
 Author-email: mhanus@tdt.com
 License: UNKNOWN
 Description: # tdt
```

### Comparing `tdt-0.5.8/README.md` & `tdt-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `tdt-0.5.8/setup.py` & `tdt-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `tdt-0.5.8/tdt/BH32.py` & `tdt-0.5.9/tdt/BH32.py`

 * *Files identical despite different names*

### Comparing `tdt-0.5.8/tdt/PynapseUDP.py` & `tdt-0.5.9/tdt/PynapseUDP.py`

 * *Files identical despite different names*

### Comparing `tdt-0.5.8/tdt/SynapseAPI.py` & `tdt-0.5.9/tdt/SynapseAPI.py`

 * *Files identical despite different names*

### Comparing `tdt-0.5.8/tdt/TDTUDP.py` & `tdt-0.5.9/tdt/TDTUDP.py`

 * *Files identical despite different names*

### Comparing `tdt-0.5.8/tdt/TDTbin2py.py` & `tdt-0.5.9/tdt/TDTbin2py.py`

 * *Files 0% similar despite different names*

```diff
@@ -886,15 +886,17 @@
                 raise Exception('block path {0} not found'.format(block_path))
             
             if 'streams' in evtype:
                 warnings.warn('no tsq file found, attempting to read sev files', Warning, stacklevel=2)
                 return read_sev(block_path, channel=channel, event_name=store, t1=t1,
                     t2=t2, ranges=ranges, verbose=verbose, export=export, scale=scale,
                     dtype=dtype, outdir=outdir, prefix=prefix)
-           
+            else:
+                raise Exception('no TSQ file found in {0}'.format(block_path))
+        
         elif len(tsq_list) > 1:
             raise Exception('multiple TSQ files found\n{0}'.format(','.join(tsq_list)))
         
         try:
             tsq = open(tsq_list[0], 'rb')
         except:
             raise Exception('tsq file {0} could not be opened'.format(tsq_list[0]))
@@ -2182,15 +2184,13 @@
             if hasattr(data[bitwisetype][bitwise].bitwise, ffield):
                 if len(data[bitwisetype][bitwise].bitwise[ffield].onset) - 1 == len(data[bitwisetype][bitwise].bitwise[ffield].offset):
                     data[bitwisetype][bitwise].bitwise[ffield].offset = np.concatenate([data[bitwisetype][bitwise].bitwise[ffield].offset, [np.inf]])
     
     return data
 
 if __name__ == '__main__':
-    BLOCK_PATH = 'C:\\TDT\\TDTExampleData\\Algernon-180308-130351'
-    BLOCK_PATH = 'G:\\CASETANK\\Block-1'
     BLOCK_PATH = 'C:\\TDT\\TDTMatlabSDK\\Examples\\ExampleData\\VTA4-190125-100559'
     start = time.time()
     data = read_block(BLOCK_PATH)
     print(time.time() - start, 'elapsed')
     print(data)
     print(data.epocs.Note)
```

### Comparing `tdt-0.5.8/tdt/TDTfilter.py` & `tdt-0.5.9/tdt/TDTfilter.py`

 * *Files identical despite different names*

### Comparing `tdt-0.5.8/tdt/__init__.py` & `tdt-0.5.9/tdt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.5.8'
+__version__ = '0.5.9'
 
 import os
 import re
 
 import numpy as np
 
 # Tank event types (tsqEventHeader.type)
```

### Comparing `tdt-0.5.8/tdt.egg-info/PKG-INFO` & `tdt-0.5.9/tdt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdt
-Version: 0.5.8
+Version: 0.5.9
 Summary: Tucker-Davis Technologies (TDT) Python APIs for reading data and interacting with Synapse software
 Home-page: UNKNOWN
 Author: Mark Hanus
 Author-email: mhanus@tdt.com
 License: UNKNOWN
 Description: # tdt
```

