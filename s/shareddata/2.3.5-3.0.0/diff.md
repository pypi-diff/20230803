# Comparing `tmp/shareddata-2.3.5.tar.gz` & `tmp/shareddata-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.3.5.tar", last modified: Thu Aug  3 10:20:48 2023, max compression
+gzip compressed data, was "shareddata-3.0.0.tar", last modified: Thu Aug  3 11:08:10 2023, max compression
```

## Comparing `shareddata-2.3.5.tar` & `shareddata-3.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 10:20:48.411446 shareddata-2.3.5/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.3.5/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-03 10:20:48.411446 shareddata-2.3.5/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.3.5/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.3.5/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-03 10:20:48.411446 shareddata-2.3.5/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 10:20:48.411446 shareddata-2.3.5/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 10:20:48.411446 shareddata-2.3.5/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/AWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/AWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10577 2023-08-03 10:07:54.000000 shareddata-2.3.5/src/SharedData/DataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/LoggerConsumerProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4251 2023-08-02 08:56:01.000000 shareddata-2.3.5/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8458 2023-08-03 10:19:49.000000 shareddata-2.3.5/src/SharedData/RealTime.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7485 2023-08-03 10:08:20.000000 shareddata-2.3.5/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9244 2023-08-03 10:09:20.000000 shareddata-2.3.5/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    30749 2023-08-03 10:04:28.000000 shareddata-2.3.5/src/SharedData/Table.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-08-02 13:49:16.000000 shareddata-2.3.5/src/SharedData/TableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/TableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13186 2023-08-03 10:08:05.000000 shareddata-2.3.5/src/SharedData/TimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-08-01 11:14:58.000000 shareddata-2.3.5/src/SharedData/TimeseriesContainer.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.3.5/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.3.5/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 10:20:48.411446 shareddata-2.3.5/src/shareddata.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-03 10:20:48.000000 shareddata-2.3.5/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      748 2023-08-03 10:20:48.000000 shareddata-2.3.5/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-03 10:20:48.000000 shareddata-2.3.5/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-03 10:20:48.000000 shareddata-2.3.5/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-03 10:20:48.000000 shareddata-2.3.5/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 11:08:10.943004 shareddata-3.0.0/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-3.0.0/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-03 11:08:10.943004 shareddata-3.0.0/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-3.0.0/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-3.0.0/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-03 11:08:10.943004 shareddata-3.0.0/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 11:08:10.943004 shareddata-3.0.0/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 11:08:10.943004 shareddata-3.0.0/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/AWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/AWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10577 2023-08-03 10:07:54.000000 shareddata-3.0.0/src/SharedData/DataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4251 2023-08-02 08:56:01.000000 shareddata-3.0.0/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8428 2023-08-03 11:07:23.000000 shareddata-3.0.0/src/SharedData/RealTime.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7485 2023-08-03 10:08:20.000000 shareddata-3.0.0/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9244 2023-08-03 10:09:20.000000 shareddata-3.0.0/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    30749 2023-08-03 10:04:28.000000 shareddata-3.0.0/src/SharedData/Table.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-08-02 13:49:16.000000 shareddata-3.0.0/src/SharedData/TableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/TableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13186 2023-08-03 10:08:05.000000 shareddata-3.0.0/src/SharedData/TimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/TimeseriesContainer.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-3.0.0/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-3.0.0/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 11:08:10.943004 shareddata-3.0.0/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-03 11:08:10.000000 shareddata-3.0.0/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      748 2023-08-03 11:08:10.000000 shareddata-3.0.0/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-03 11:08:10.000000 shareddata-3.0.0/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-03 11:08:10.000000 shareddata-3.0.0/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-03 11:08:10.000000 shareddata-3.0.0/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.3.5/LICENSE` & `shareddata-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/PKG-INFO` & `shareddata-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.3.5
+Version: 3.0.0
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.3.5/README.md` & `shareddata-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/setup.cfg` & `shareddata-3.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shareddata
-version = 2.3.5
+version = 3.0.0
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Shared Memory Database with S3 repository
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/SharedData
 project_urls =
```

### Comparing `shareddata-2.3.5/src/SharedData/AWSKinesis.py` & `shareddata-3.0.0/src/SharedData/AWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/AWSS3.py` & `shareddata-3.0.0/src/SharedData/AWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/DataFrame.py` & `shareddata-3.0.0/src/SharedData/DataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/Defaults.py` & `shareddata-3.0.0/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/Logger.py` & `shareddata-3.0.0/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/LoggerConsumerProcess.py` & `shareddata-3.0.0/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/Metadata.py` & `shareddata-3.0.0/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/MultiProc.py` & `shareddata-3.0.0/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/RealTime.py` & `shareddata-3.0.0/src/SharedData/RealTime.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,32 +8,30 @@
     
     # Dict to keep track of all connected client sockets
     clients = {}
     # Create a lock to protect access to the clients Dict
     lock = threading.Lock()    
     server = None
     shdata = None
+    accept_clients = None
+
 
     @staticmethod
     def runserver(shdata,host,port):
 
         RealTime.shdata = shdata
 
         RealTime.server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         # This line allows the address to be reused
         RealTime.server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
         # Create the server and start accepting clients in a new thread
-        threading.Thread(target=RealTime.accept_clients_thread, args=(host, port)).start()
-        
-        # Keep the main server loop running
-        while True:
-            for client in RealTime.clients:
-                Logger.log.info(str(client))
-            time.sleep(10)
+        RealTime.accept_clients = threading.Thread(target=RealTime.accept_clients_thread, args=(host, port))
+        RealTime.accept_clients.start()
+                
 
     @staticmethod
     def accept_clients_thread(host, port):    
         RealTime.server.bind((host, port))
         RealTime.server.listen()
 
         Logger.log.info(f'Serving on {host}:{port}')
@@ -88,32 +86,33 @@
                             Logger.log.info(f"Client {addr} disconnected.")
                             break
                     
                     if 'table' in sockdata:
                         table = sockdata['table']                    
                         ids2send = []
 
-                        lastcount = sockdata['count']
-                        curcount = table.count.copy()
-                        if curcount>lastcount:
-                            newids = np.arange(lastcount,curcount)
-                            ids2send.extend(newids)
-                            sockdata['count'] = curcount
-                        
                         lastmtime = sockdata['mtime']
                         lookbackid = table.count-1000
                         if lookbackid<0:
                             lookbackid=0
                         updtids = np.where(table[lookbackid:]['mtime']>lastmtime)
                         if len(updtids)>0:
                             ids2send.extend(updtids[0]+lookbackid)
                             sockdata['mtime'] = max(table[lookbackid:]['mtime'])
-                        
+
+                        lastcount = sockdata['count']
+                        curcount = table.count.copy()
+                        if curcount>lastcount:
+                            newids = np.arange(lastcount,curcount)
+                            ids2send.extend(newids)
+                            sockdata['count'] = curcount
+                                                
                         if len(ids2send)>0:
                             ids2send = np.unique(ids2send)
+                            ids2send = np.sort(ids2send)
                             maxrows = sockdata['maxrows']
                             rows2send = len(ids2send)
                             sentrows = 0
                             while sentrows<rows2send:
                                 msgsize = min(maxrows,rows2send)
                                 msg = table[ids2send[sentrows:msgsize]].tobytes()
                                 conn.sendall(msg)
```

### Comparing `shareddata-2.3.5/src/SharedData/SharedData.py` & `shareddata-3.0.0/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/SharedNumpy.py` & `shareddata-3.0.0/src/SharedData/SharedNumpy.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/Table.py` & `shareddata-3.0.0/src/SharedData/Table.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/TableIndex.py` & `shareddata-3.0.0/src/SharedData/TableIndex.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/TableIndexJit.py` & `shareddata-3.0.0/src/SharedData/TableIndexJit.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/TimeSeries.py` & `shareddata-3.0.0/src/SharedData/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/TimeseriesContainer.py` & `shareddata-3.0.0/src/SharedData/TimeseriesContainer.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/SharedData/Utils.py` & `shareddata-3.0.0/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.5/src/shareddata.egg-info/PKG-INFO` & `shareddata-3.0.0/src/shareddata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.3.5
+Version: 3.0.0
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.3.5/src/shareddata.egg-info/SOURCES.txt` & `shareddata-3.0.0/src/shareddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

