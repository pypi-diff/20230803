# Comparing `tmp/nucleus_driver-1.5.5.tar.gz` & `tmp/nucleus_driver-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucleus_driver-1.5.5.tar", last modified: Thu Jul 20 08:10:46 2023, max compression
+gzip compressed data, was "nucleus_driver-1.5.6.tar", last modified: Thu Aug  3 09:45:38 2023, max compression
```

## Comparing `nucleus_driver-1.5.5.tar` & `nucleus_driver-1.5.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-20 08:10:46.702148 nucleus_driver-1.5.5/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.5.5/LICENSE.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     9494 2023-07-20 08:10:46.702148 nucleus_driver-1.5.5/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.5.5/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.5.5/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-07-20 08:10:46.702148 nucleus_driver-1.5.5/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-20 08:10:46.698148 nucleus_driver-1.5.5/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-20 08:10:46.702148 nucleus_driver-1.5.5/src/nucleus_driver/
--rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.5.5/src/nucleus_driver/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.5.5/src/nucleus_driver/_assert.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    50233 2023-06-26 12:27:28.000000 nucleus_driver-1.5.5/src/nucleus_driver/_commands.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    17098 2023-06-26 13:48:04.000000 nucleus_driver-1.5.5/src/nucleus_driver/_connection.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    25406 2023-06-26 13:48:04.000000 nucleus_driver-1.5.5/src/nucleus_driver/_download.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    16602 2023-06-26 13:48:04.000000 nucleus_driver-1.5.5/src/nucleus_driver/_flash.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10853 2023-06-26 13:48:04.000000 nucleus_driver-1.5.5/src/nucleus_driver/_logger.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.5.5/src/nucleus_driver/_messages.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    39942 2023-07-20 08:09:17.000000 nucleus_driver-1.5.5/src/nucleus_driver/_parser.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.5.5/src/nucleus_driver/_syslog.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    19446 2023-06-30 08:54:04.000000 nucleus_driver-1.5.5/src/nucleus_driver/app.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    11213 2023-07-20 08:10:01.000000 nucleus_driver-1.5.5/src/nucleus_driver/nucleus_driver.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-20 08:10:46.702148 nucleus_driver-1.5.5/src/nucleus_driver.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     9494 2023-07-20 08:10:46.000000 nucleus_driver-1.5.5/src/nucleus_driver.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-07-20 08:10:46.000000 nucleus_driver-1.5.5/src/nucleus_driver.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-20 08:10:46.000000 nucleus_driver-1.5.5/src/nucleus_driver.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       78 2023-07-20 08:10:46.000000 nucleus_driver-1.5.5/src/nucleus_driver.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-07-20 08:10:46.000000 nucleus_driver-1.5.5/src/nucleus_driver.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-07-20 08:10:46.000000 nucleus_driver-1.5.5/src/nucleus_driver.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-08-03 09:45:38.130408 nucleus_driver-1.5.6/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.5.6/LICENSE.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-08-03 09:45:38.130408 nucleus_driver-1.5.6/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.5.6/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.5.6/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-08-03 09:45:38.130408 nucleus_driver-1.5.6/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-08-03 09:45:38.126408 nucleus_driver-1.5.6/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-08-03 09:45:38.126408 nucleus_driver-1.5.6/src/nucleus_driver/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.5.6/src/nucleus_driver/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.5.6/src/nucleus_driver/_assert.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    50431 2023-08-03 09:28:28.000000 nucleus_driver-1.5.6/src/nucleus_driver/_commands.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    17100 2023-08-03 07:58:07.000000 nucleus_driver-1.5.6/src/nucleus_driver/_connection.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    25406 2023-06-26 13:48:04.000000 nucleus_driver-1.5.6/src/nucleus_driver/_download.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    16602 2023-06-26 13:48:04.000000 nucleus_driver-1.5.6/src/nucleus_driver/_flash.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10853 2023-06-26 13:48:04.000000 nucleus_driver-1.5.6/src/nucleus_driver/_logger.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.5.6/src/nucleus_driver/_messages.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    39942 2023-07-21 09:50:11.000000 nucleus_driver-1.5.6/src/nucleus_driver/_parser.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.5.6/src/nucleus_driver/_syslog.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    19446 2023-06-30 08:54:04.000000 nucleus_driver-1.5.6/src/nucleus_driver/app.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11213 2023-07-31 12:03:10.000000 nucleus_driver-1.5.6/src/nucleus_driver/nucleus_driver.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-08-03 09:45:38.130408 nucleus_driver-1.5.6/src/nucleus_driver.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-08-03 09:45:38.000000 nucleus_driver-1.5.6/src/nucleus_driver.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-08-03 09:45:38.000000 nucleus_driver-1.5.6/src/nucleus_driver.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-08-03 09:45:38.000000 nucleus_driver-1.5.6/src/nucleus_driver.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       77 2023-08-03 09:45:38.000000 nucleus_driver-1.5.6/src/nucleus_driver.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-08-03 09:45:38.000000 nucleus_driver-1.5.6/src/nucleus_driver.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-08-03 09:45:38.000000 nucleus_driver-1.5.6/src/nucleus_driver.egg-info/top_level.txt
```

### Comparing `nucleus_driver-1.5.5/LICENSE.txt` & `nucleus_driver-1.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.5/PKG-INFO` & `nucleus_driver-1.5.6/src/nucleus_driver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
-Name: nucleus_driver
-Version: 1.5.5
+Name: nucleus-driver
+Version: 1.5.6
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -276,8 +274,7 @@
 To run the console script, execute the command
 
 ```shell
 nucleus_driver
 ```
 
 ![Console script](docs/nucleus_driver_shell.png)
-
```

### Comparing `nucleus_driver-1.5.5/README.md` & `nucleus_driver-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.5/setup.cfg` & `nucleus_driver-1.5.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nucleus_driver
-version = 1.5.5
+version = 1.5.6
 author = Martin Bergene Johansen
 author_email = martin.johansen@nortekgroup.com
 description = driver for the Nortek Nucleus
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nortekgroup/nucleus_driver
 classifiers =
```

### Comparing `nucleus_driver-1.5.5/src/nucleus_driver/_assert.py` & `nucleus_driver-1.5.6/src/nucleus_driver/_assert.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.5/src/nucleus_driver/_commands.py` & `nucleus_driver-1.5.6/src/nucleus_driver/_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,19 +74,22 @@
         get_reply = self._get_reply(terminator=terminator, timeout=timeout, command=command)
         self._check_reply(data=get_reply, terminator=terminator, command=command)
 
         reply_list = [i + b'\r\n' for i in get_reply.split(b'\r\n') if i]
 
         if nmea:
             for reply in reply_list:
-                reply_split = reply.split(b'*')
-                nmea_checksum = self._nmea_checksum(reply_split[0])
-                if nmea_checksum != reply_split[1].rstrip(b'\r\n'):
-                    self.messages.write_warning('Reply did not pass nmea checksum: {}\t{}'.format(reply, nmea_checksum))
-
+                try:
+                    reply_split = reply.split(b'*')
+                    nmea_checksum = self._nmea_checksum(reply_split[0])
+                    if nmea_checksum != reply_split[1].rstrip(b'\r\n'):
+                        self.messages.write_warning('Reply did not pass nmea checksum: {}\t{}'.format(reply, nmea_checksum))
+                except Exception as e:
+                    self.messages.write_warning(f'Failed to split nmea reply: {reply} \t error: {e}')
+                    
         return reply_list
 
     def _nmea_checksum(self, command):
 
         checksum = 0
 
         command = command.lstrip(b'$')
```

### Comparing `nucleus_driver-1.5.5/src/nucleus_driver/_connection.py` & `nucleus_driver-1.5.6/src/nucleus_driver/_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,15 +440,15 @@
                 return None
             
         if self.get_connection_type() == 'serial':
             data = self.serial.read(size=self.serial.in_waiting)
         
         return data
 
-    def read(self, size=None, terminator: bytes = None, timeout: int = 1) -> bytes:
+    def read(self, size=None, terminator: bytes = None, timeout: float = 1) -> bytes:
 
         data = b''
         size_satisfied = False
         terminator_satisfied = False
 
         if timeout is None:
```

### Comparing `nucleus_driver-1.5.5/src/nucleus_driver/_download.py` & `nucleus_driver-1.5.6/src/nucleus_driver/_download.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.5/src/nucleus_driver/_flash.py` & `nucleus_driver-1.5.6/src/nucleus_driver/_flash.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.5/src/nucleus_driver/_logger.py` & `nucleus_driver-1.5.6/src/nucleus_driver/_logger.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.5/src/nucleus_driver/_parser.py` & `nucleus_driver-1.5.6/src/nucleus_driver/_parser.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.5/src/nucleus_driver/_syslog.py` & `nucleus_driver-1.5.6/src/nucleus_driver/_syslog.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.5/src/nucleus_driver/app.py` & `nucleus_driver-1.5.6/src/nucleus_driver/app.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.5/src/nucleus_driver/nucleus_driver.py` & `nucleus_driver-1.5.6/src/nucleus_driver/nucleus_driver.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.5/src/nucleus_driver.egg-info/PKG-INFO` & `nucleus_driver-1.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
-Name: nucleus-driver
-Version: 1.5.5
+Name: nucleus_driver
+Version: 1.5.6
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -276,8 +274,7 @@
 To run the console script, execute the command
 
 ```shell
 nucleus_driver
 ```
 
 ![Console script](docs/nucleus_driver_shell.png)
-
```

### Comparing `nucleus_driver-1.5.5/src/nucleus_driver.egg-info/SOURCES.txt` & `nucleus_driver-1.5.6/src/nucleus_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

