# Comparing `tmp/shareddata-2.3.2.tar.gz` & `tmp/shareddata-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.3.2.tar", last modified: Wed Aug  2 09:04:15 2023, max compression
+gzip compressed data, was "shareddata-2.3.5.tar", last modified: Thu Aug  3 10:20:48 2023, max compression
```

## Comparing `shareddata-2.3.2.tar` & `shareddata-2.3.5.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 09:04:15.857180 shareddata-2.3.2/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.3.2/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-02 09:04:15.857180 shareddata-2.3.2/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.3.2/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.3.2/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-02 09:04:15.857180 shareddata-2.3.2/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 09:04:15.853180 shareddata-2.3.2/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 09:04:15.857180 shareddata-2.3.2/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/AWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/AWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10837 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/DataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/LoggerConsumerProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4251 2023-08-02 08:56:01.000000 shareddata-2.3.2/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3389 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/RealTime.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2476 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/RealTimeProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7535 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9165 2023-08-02 08:55:08.000000 shareddata-2.3.2/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    30167 2023-08-02 08:55:08.000000 shareddata-2.3.2/src/SharedData/Table.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/TableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/TableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13509 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/TimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/TimeseriesContainer.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.3.2/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.3.2/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 09:04:15.857180 shareddata-2.3.2/src/shareddata.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-02 09:04:15.000000 shareddata-2.3.2/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      782 2023-08-02 09:04:15.000000 shareddata-2.3.2/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-02 09:04:15.000000 shareddata-2.3.2/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-02 09:04:15.000000 shareddata-2.3.2/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-02 09:04:15.000000 shareddata-2.3.2/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 10:20:48.411446 shareddata-2.3.5/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.3.5/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-03 10:20:48.411446 shareddata-2.3.5/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.3.5/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.3.5/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-03 10:20:48.411446 shareddata-2.3.5/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 10:20:48.411446 shareddata-2.3.5/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 10:20:48.411446 shareddata-2.3.5/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/AWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/AWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10577 2023-08-03 10:07:54.000000 shareddata-2.3.5/src/SharedData/DataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4251 2023-08-02 08:56:01.000000 shareddata-2.3.5/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8458 2023-08-03 10:19:49.000000 shareddata-2.3.5/src/SharedData/RealTime.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7485 2023-08-03 10:08:20.000000 shareddata-2.3.5/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9244 2023-08-03 10:09:20.000000 shareddata-2.3.5/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    30749 2023-08-03 10:04:28.000000 shareddata-2.3.5/src/SharedData/Table.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-08-02 13:49:16.000000 shareddata-2.3.5/src/SharedData/TableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/TableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13186 2023-08-03 10:08:05.000000 shareddata-2.3.5/src/SharedData/TimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/TimeseriesContainer.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.3.5/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.3.5/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 10:20:48.411446 shareddata-2.3.5/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-03 10:20:48.000000 shareddata-2.3.5/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      748 2023-08-03 10:20:48.000000 shareddata-2.3.5/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-03 10:20:48.000000 shareddata-2.3.5/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-03 10:20:48.000000 shareddata-2.3.5/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-03 10:20:48.000000 shareddata-2.3.5/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.3.2/LICENSE` & `shareddata-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.2/PKG-INFO` & `shareddata-2.3.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.3.2
+Version: 2.3.5
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.3.2/README.md` & `shareddata-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.2/setup.cfg` & `shareddata-2.3.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shareddata
-version = 2.3.2
+version = 2.3.5
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Shared Memory Database with S3 repository
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/SharedData
 project_urls =
```

### Comparing `shareddata-2.3.2/src/SharedData/AWSKinesis.py` & `shareddata-2.3.5/src/SharedData/AWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.2/src/SharedData/AWSS3.py` & `shareddata-2.3.5/src/SharedData/AWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.2/src/SharedData/DataFrame.py` & `shareddata-2.3.5/src/SharedData/DataFrame.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from pathlib import Path
 from multiprocessing import shared_memory
 from datetime import datetime, timedelta
 
 
 from SharedData.Logger import Logger
 from SharedData.AWSS3 import S3Download,S3Upload,UpdateModTime
-from SharedData.RealTime import SharedDataRealTime
 
 
 class SharedDataFrame:
 
     def __init__(self, sharedDataPeriod, tag, df=None):        
         self.sharedDataPeriod = sharedDataPeriod
         self.tag = tag
@@ -280,17 +279,8 @@
         io_obj.write(md5hash_b)        
         return io_obj
 
     def write_file(io_obj,path,mtime):
         with open(path, 'wb') as f:
             f.write(io_obj.getbuffer())
             f.flush()
-        os.utime(path, (mtime, mtime))
-     
-    # MESSAGES
-    def Broadcast(self,idx,col):
-        SharedDataRealTime.Broadcast(
-            self.sharedData,
-            self.feeder,
-            self.period,
-            self.tag,
-            idx,col)
+        os.utime(path, (mtime, mtime))
```

### Comparing `shareddata-2.3.2/src/SharedData/Defaults.py` & `shareddata-2.3.5/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.2/src/SharedData/Logger.py` & `shareddata-2.3.5/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.2/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.3.5/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.2/src/SharedData/Metadata.py` & `shareddata-2.3.5/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.2/src/SharedData/MultiProc.py` & `shareddata-2.3.5/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.2/src/SharedData/SharedData.py` & `shareddata-2.3.5/src/SharedData/SharedData.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import SharedData.Defaults as Defaults 
 from SharedData.Logger import Logger
 from SharedData.Table import Table
 from SharedData.TimeseriesContainer import TimeseriesContainer
 from SharedData.TimeSeries import TimeSeries
 from SharedData.DataFrame import SharedDataFrame
-from SharedData.RealTime import SharedDataRealTime
+
 from SharedData.Utils import remove_shm_from_resource_tracker
 
 class SharedData:    
     
     def __init__(self,source,user='guest'):
         self.source = source
         self.user = user
```

### Comparing `shareddata-2.3.2/src/SharedData/SharedNumpy.py` & `shareddata-2.3.5/src/SharedData/SharedNumpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
     def __new__(cls, shape, dtype=None, buffer=None, offset=0, strides=None, order=None):
         obj = np.ndarray.__new__(
             cls, shape, dtype, buffer, offset, strides, order)
         obj.table = None
         return obj
 
+    def subscribe(self,host,port):
+        self.table.subscribe(host, port)
+
     def preallocate(self):
         arr = super().__getitem__(slice(0, self.size))
         arr['mtime'][:] = np.datetime64('NaT')
     ############################## KEYLESS OPERATIONS ########################################
 
     def insert(self, new_records):
         self.table.acquire()
@@ -80,36 +83,36 @@
             Logger.log.error('Error overwriting records!\n%s' % (e))
 
         self.table.release()
 
     ############################## PRIMARY KEY OPERATIONS ########################################
     def upsert(self, new_records):
         if new_records.size>0:
-            self.table.acquire()
+                        
+            # convert to same dtype record
+            if isinstance(new_records, pd.DataFrame):
+                new_records = self.table.df2records(new_records)
+            elif (self.dtype != new_records.dtype):
+                new_records = self.convert(new_records)
 
-            try:
+            # fill mtime
+            nidx = np.isnat(new_records['mtime'])
+            if nidx.any():
+                new_records['mtime'][nidx] = time.time_ns()
+
+            # single record to array
+            if new_records.shape == ():
+                new_records = np.array([new_records])
+
+            self.table.acquire()
+            
+            try:                
                 # initialize pkey
                 if not self.keys.initialized:
                     self.keys.initialize()
-
-                # convert to same dtype record
-                if isinstance(new_records, pd.DataFrame):
-                    new_records = self.table.df2records(new_records)
-                elif (self.dtype != new_records.dtype):
-                    new_records = self.convert(new_records)
-
-                # fill mtime
-                nidx = np.isnat(new_records['mtime'])
-                if nidx.any():
-                    new_records['mtime'][nidx] = time.time_ns()
-
-                # single record to array
-                if new_records.shape == ():
-                    new_records = np.array([new_records])
-
                 # upsert
                 minchgid = self.count
                 arr = super().__getitem__(slice(0, self.size))
                 if 'date_portfolio_' in self.table.keys.pkeystr:
                     self.count, minchgid = self.keys.upsert_func(
                         arr, self.count, new_records, self.pkey,\
                         self.keys.dateiniidx,self.keys.dateendidx,self.keys.dateunit,\
@@ -203,17 +206,15 @@
         dtendid = self.keys.dateendidx[dtint]        
         return [dtiniid,dtendid+1]
     
     def get_index_date_portfolio(self,keys):    
         if not self.keys.initialized:
             self.keys.initialize()    
         return self.keys.get_index_date_portfolio_func(self[:], keys, self.pkey, self.keys.portiniidx,self.keys.portlist)
-        
-
-    
+            
     ############################## GETTERS / SETTERS ##############################
 
     def __getitem__(self, key):
         if hasattr(self, 'table'):
             arr = super().__getitem__(slice(0, self.count))  # slice arr
             if self.count > 0:                
                 return arr.__getitem__(key)
```

### Comparing `shareddata-2.3.2/src/SharedData/Table.py` & `shareddata-2.3.5/src/SharedData/Table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import os
-import random
+import os,threading,time
 import pandas as pd
 import numpy as np
 from pathlib import Path
-import time
 from multiprocessing import shared_memory
 import gzip,io,hashlib
 from datetime import datetime
 from tqdm import tqdm
 
 from SharedData.Logger import Logger
 from SharedData.AWSS3 import S3Upload,S3Download,UpdateModTime
 from SharedData.TableIndex import TableIndex
 from SharedData.SharedNumpy import SharedNumpy
+from SharedData.RealTime import RealTime
 
 if os.name == 'posix':
     from SharedData.Utils  import cpp
 
 class Table:
 
     def __init__(self, shareddata, database, period, source, tablename,\
@@ -26,14 +25,15 @@
         self.database = database
         self.period = period        
         self.source = source
         self.tablename = tablename
         if os.name != 'posix':
             overwrite = False
         
+        self.subscription_thread = None
         self.keys = TableIndex(self)
         
         self.init_time = time.time()
         self.download_time = pd.NaT
                         
         # file partitioning threshold
         self.maxtailbytes = int(100*10**6)
@@ -486,14 +486,15 @@
         nb_head = int(self.hdr['headsize']*self.hdr['itemsize'])
         nb_tail = int(tailsize*self.hdr['itemsize'])
         
         self.tailhdr['mtime'] = self.hdr['mtime']
         self.tailhdr['tailsize'] = tailsize
 
         if md5hash is None:
+            # TODO: create one md5 hash for head and one for tail
             self.hdr['md5hash']=0 # reset the hash value
             nb_records_mb = (nb_header+nb_head+nb_tail)/(1024*1024)
             if nb_records_mb<=100:
                 m = hashlib.md5(self.shm.buf[nb_header:nb_header+nb_head+nb_tail])
             else:
                 message = 'Creating md5 hash:%iMB %s/%s' % (nb_records_mb,self.source,self.tablename)
                 block_size = 100 * 1024 * 1024 # or any other block size that you prefer
@@ -650,8 +651,22 @@
             self.hdr['semaphore'] = 0
         
     def free(self):
         path, shm_name = self.get_path()            
         self.shareddata.free(shm_name)
         self.shareddata.free(shm_name+'#pkey')
         self.shareddata.free(shm_name+'#dateidx')
-        self.shareddata.free(shm_name+'#portidx')
+        self.shareddata.free(shm_name+'#portidx')
+
+
+    def subscribe(self, host, port):
+        if self.subscription_thread is None:
+            self.subscription_thread = threading.Thread(
+                target=RealTime.table_subscribe_thread, \
+                args=(self, host, port)
+                )
+            self.subscription_thread.start()
+            Logger.log.debug('Subscription started!')
+        else:
+            Logger.log.error('Subscription already running!')
+    
+
```

### Comparing `shareddata-2.3.2/src/SharedData/TableIndex.py` & `shareddata-2.3.5/src/SharedData/TableIndex.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.2/src/SharedData/TableIndexJit.py` & `shareddata-2.3.5/src/SharedData/TableIndexJit.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.2/src/SharedData/TimeSeries.py` & `shareddata-2.3.5/src/SharedData/TimeSeries.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 import io, gzip, hashlib, shutil
 from threading import Thread
 
 from subprocess import run, PIPE
 from datetime import datetime, timedelta
 
 from SharedData.Logger import Logger
-from SharedData.AWSS3 import S3Upload,S3Download,UpdateModTime
-from SharedData.RealTime import SharedDataRealTime
 
 class TimeSeries:
 
     def __init__(self, shareddata, container, database, period, source, tag,\
             value=None,startDate=None,columns=None,overwrite=False,user='master'):
         
         self.shareddata = shareddata
@@ -193,23 +191,14 @@
                         columns=self.columns,\
                         copy=False)
         
             return True
         except Exception as e:
             Logger.log.error('Failed to malloc_map\n%s' % str(e))
             return False
-
-    # MESSAGES
-    def broadcast(self,idx,col):
-        SharedDataRealTime.broadcast(
-            self.shareddata,
-            self.source,
-            self.period,
-            self.tag,
-            idx,col)
     
     # get / set
     def get_loc_symbol(self, symbol):
         if symbol in self.symbolidx.keys():
             return self.symbolidx[symbol]
         else:
             return np.nan
```

### Comparing `shareddata-2.3.2/src/SharedData/TimeseriesContainer.py` & `shareddata-2.3.5/src/SharedData/TimeseriesContainer.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.2/src/SharedData/Utils.py` & `shareddata-2.3.5/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.2/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.3.5/src/shareddata.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.3.2
+Version: 2.3.5
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.3.2/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.3.5/src/shareddata.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 src/SharedData/DataFrame.py
 src/SharedData/Defaults.py
 src/SharedData/Logger.py
 src/SharedData/LoggerConsumerProcess.py
 src/SharedData/Metadata.py
 src/SharedData/MultiProc.py
 src/SharedData/RealTime.py
-src/SharedData/RealTimeProcess.py
 src/SharedData/SharedData.py
 src/SharedData/SharedNumpy.py
 src/SharedData/Table.py
 src/SharedData/TableIndex.py
 src/SharedData/TableIndexJit.py
 src/SharedData/TimeSeries.py
 src/SharedData/TimeseriesContainer.py
```

