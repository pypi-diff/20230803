# Comparing `tmp/bleuio-1.2.0-py3-none-any.whl.zip` & `tmp/bleuio-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18486 bytes, number of entries: 12
+Zip file size: 19740 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat        0 b- defN 20-Nov-05 12:17 bleuio_lib/__init__.py
--rw-rw-rw-  2.0 fat    62717 b- defN 23-Mar-09 17:06 bleuio_lib/bleuio_funcs.py
+-rw-rw-rw-  2.0 fat    68552 b- defN 23-Aug-03 07:20 bleuio_lib/bleuio_funcs.py
 -rw-rw-rw-  2.0 fat      150 b- defN 20-Nov-06 08:33 bleuio_lib/exceptions.py
 -rw-rw-rw-  2.0 fat        0 b- defN 20-Nov-05 12:20 bleuio_tests/__init__.py
 -rw-rw-rw-  2.0 fat     9476 b- defN 21-Jul-01 11:49 bleuio_tests/test_bleuio_funcs.py
 -rw-rw-rw-  2.0 fat        0 b- defN 20-Nov-05 12:20 tests/__init__.py
 -rw-rw-rw-  2.0 fat     2840 b- defN 20-Nov-10 12:43 tests/test_bleuio_funcs.py
--rw-rw-rw-  2.0 fat     1086 b- defN 23-Mar-09 17:21 bleuio-1.2.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    28622 b- defN 23-Mar-09 17:21 bleuio-1.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Mar-09 17:21 bleuio-1.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Mar-09 17:21 bleuio-1.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      948 b- defN 23-Mar-09 17:21 bleuio-1.2.0.dist-info/RECORD
-12 files, 105947 bytes uncompressed, 16892 bytes compressed:  84.1%
+-rw-rw-rw-  2.0 fat     1086 b- defN 23-Aug-03 07:31 bleuio-1.3.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    31418 b- defN 23-Aug-03 07:31 bleuio-1.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Aug-03 07:31 bleuio-1.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Aug-03 07:31 bleuio-1.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      948 b- defN 23-Aug-03 07:31 bleuio-1.3.0.dist-info/RECORD
+12 files, 114578 bytes uncompressed, 18146 bytes compressed:  84.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_bleuio_funcs.py
 Comment: 
 
-Filename: bleuio-1.2.0.dist-info/LICENSE.txt
+Filename: bleuio-1.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: bleuio-1.2.0.dist-info/METADATA
+Filename: bleuio-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: bleuio-1.2.0.dist-info/WHEEL
+Filename: bleuio-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: bleuio-1.2.0.dist-info/top_level.txt
+Filename: bleuio-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: bleuio-1.2.0.dist-info/RECORD
+Filename: bleuio-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bleuio_lib/bleuio_funcs.py

```diff
@@ -38,14 +38,29 @@
         self._reader_alive = None
         self._evt_cb = None
         self._scan_cb = None
         self.gaproles = self.GapRoles()
         self.status = self.BLEStatus()
         self.__threadLock = threading.Lock()
 
+        # Constants
+        self.UUID = "UUID"
+        self.CHAR_PROPERTY = "PROP"
+        self.CHAR_PERMISSION = "PERM"
+        self.CHAR_LENGTH = "LEN"
+        self.CHAR_VALUE = "VALUE"
+        self.CHAR_HEX_VALUE = "VALUEB"
+        self.DESC_PERMISSION = "DPERM"
+        self.DESC_LENGTH = "DLEN"
+        self.DESC_VALUE = "DVALUE"
+        self.DESC_HEX_VALUE = "DVALUEB"
+        self.NAME = "DVALUE"
+        self.MFSID = "MFSID"
+        self.CLEAR = "CLEAR"
+
         if port == "auto":
             dongle_count = 1
             port_list = []
             while len(DONGLE_ARRAY) == 0 and retry_count < 10:
                 all_ports = serial.tools.list_ports.comports(include_links=False)
                 for d_port in all_ports:
                     if str(d_port.hwid).__contains__("VID:PID=2DCF"):
@@ -91,19 +106,21 @@
                         print("Make sure the dongle is not already in use.")
                         exit()
                     else:
                         if self._debug:
                             print(
                                 "Error occurred while trying to open port. "
                                 + str(e)
-                                + " Retrying %d/%d...",
+                                + " Retrying",
                                 retry_count,
+                                "/",
                                 3,
+                                "...",
                             )
-                        time.sleep(1)
+                        time.sleep(5)
 
             self._serial.flushInput()
             self._serial.flushOutput()
 
         signal.signal(signal.SIGINT, self.__signal_handler)
         atexit.register(self.exit_handler)
 
@@ -112,15 +129,15 @@
         self.rx_response = []
         self.rx_scanning_results = []
         self.rx_evt_results = []
 
         self._start_reader()
         self.send_command("stop")
         self.send_command("ATV1")
-        self.send_command("ATE")
+        self.send_command("ATE1")
         self.send_command("ATI")
         # end of BleuIO.__init__()
 
     class BLEStatus:
         def __init__(self):
             """A class used to handle BLE Statuses
 
@@ -177,18 +194,26 @@
                     careObj.Cmd = json.loads(line)
                 if ('{"A"') in line.decode("utf-8", "ignore"):
                     careObj.Ack = json.loads(line)
                 if ('{"R"') in line.decode("utf-8", "ignore"):
                     careObj.Rsp.append(json.loads(line))
                 if ('{"E"') in line.decode("utf-8", "ignore"):
                     careObj.End = json.loads(line)
-                if ('{"SE"') in line.decode("utf-8", "ignore"):
+                if ('{"SE":') in line.decode("utf-8", "ignore"):
                     careObj.Ack = json.loads(line)
         except Exception as e:
-            raise self.BleuIOException("Exception: " + str(e))
+            raise self.BleuIOException(
+                "Exception: " + str(e) + "\r\nError line: " + str(line)
+            )
+        if self._debug:
+            try:
+                print("debug(__parseRspIntoJSON response): " + str(response))
+                print("debug(__parseRspIntoJSON line): " + str(line))
+            except Exception:
+                pass
 
     def exit_handler(self):
         self._serial.write("\x03".encode())
         self._serial.write("\x1B".encode())
         self._stop_reader()
         self._serial.close()
 
@@ -258,14 +283,24 @@
                         self.__threadLock.release()
 
                     if str.encode('"action":"advertising"') in self.rx_buffer:
                         self.__threadLock.acquire()
                         self.status.isAdvertising = True
                         self.__threadLock.release()
 
+                    if str.encode('"action":"connected"') in self.rx_buffer:
+                        self.__threadLock.acquire()
+                        self.status.isConnected = True
+                        self.__threadLock.release()  # "action":"disconnected"
+
+                    if str.encode('"action":"disconnected"') in self.rx_buffer:
+                        self.__threadLock.acquire()
+                        self.status.isConnected = False
+                        self.__threadLock.release()
+
                     if str.encode('"evt":') in self.rx_buffer and self.__saveEvtRsp:
                         if self._evt_cb != None:
                             decoded_evt_result = self.rx_buffer.decode(
                                 "utf-8", "ignore"
                             )
                             decoded_evt_resultList = []
                             decoded_evt_resultList = decoded_evt_result.split("\r\n")
@@ -337,21 +372,24 @@
                                                     "Cannot read firmware version!"
                                                 )
                                             if checkVer < 221:
                                                 raise self.BleuIOException(
                                                     "BleuIO firmware version is not supported by the BleuIO Python Library!\nSupported version is >= 2.2.1."
                                                 )
 
-                                    if '"connected"' in line and not '"action"':
+                                    if '"connected"' in line and not '"action"' in line:
                                         jsonStr = json.loads(line)
                                         self.__threadLock.acquire()
                                         self.status.isConnected = jsonStr["connected"]
                                         self.__threadLock.release()
 
-                                    if '"advertising"' in line and not '"action"':
+                                    if (
+                                        '"advertising"' in line
+                                        and not '"action"' in line
+                                    ):
                                         jsonStr = json.loads(line)
                                         self.__threadLock.acquire()
                                         self.status.isAdvertising = jsonStr[
                                             "advertising"
                                         ]
                                         self.__threadLock.release()
 
@@ -801,14 +839,40 @@
     def __at_target_conn(self, conn_idx):
 
         if conn_idx == "":
             return self.send_command("AT+TARGETCONN")
         else:
             return self.send_command("AT+TARGETCONN=" + conn_idx)
 
+    def __at_scanfilter(self, sftype, value):
+        if sftype == None and value == "":
+            return self.send_command("AT+SCANFILTER")
+        else:
+            if value == "":
+                return self.send_command("AT+SCANFILTER=" + str(sftype))
+            else:
+                return self.send_command("AT+SCANFILTER=" + str(sftype) + "=" + value)
+
+    def __at_customservice(self, idx, cstype, value):
+        if idx == None and cstype == None and value == "":
+            return self.send_command("AT+CUSTOMSERVICE")
+        else:
+            return self.send_command(
+                "AT+CUSTOMSERVICE=" + str(idx) + "=" + str(cstype) + "=" + value
+            )
+
+    def __at_customservice_start(self):
+        return self.send_command("AT+CUSTOMSERVICESTART")
+
+    def __at_customservice_stop(self):
+        return self.send_command("AT+CUSTOMSERVICESTOP")
+
+    def __at_customservice_reset(self):
+        return self.send_command("AT+CUSTOMSERVICERESET")
+
     def __help(self):
 
         return self.send_command("--H")
 
     def __stop_scan(self):
 
         return self.send_command("stop")
@@ -1113,15 +1177,15 @@
         """
         care = self.__at_enter_passkey(passkey)
         response = self.BleuIORESP()
         self.__parseRspIntoJSON(care, response)
 
         return response
 
-    def at_findscandata(self, scandata, timeout=0):
+    def at_findscandata(self, scandata="", timeout=0):
         """Scans for all advertising/response data which contains the search params.
 
         :param scandata: Hex string to filter the advertising/scan response data. Can be left blank to scan for everything. Format XXXX..
         :type scandata: str
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
         :rtype: obj BleuIORESP
         """
@@ -1604,14 +1668,88 @@
         """
         care = self.__at_target_conn(conn_idx)
         response = self.BleuIORESP()
         self.__parseRspIntoJSON(care, response)
 
         return response
 
+    def at_scanfilter(self, sftype: str = None, value: str = ""):
+        """Sets or queries the scanfilter. There are three types of scanfilter, filter by name, filter by uuid or by manufacturer specific ID.
+
+        :param sftype: scan filter parameter type
+        :type sftype : str
+        :param value: value
+        :type value : str
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+        care = self.__at_scanfilter(sftype, value)
+        response = self.BleuIORESP()
+        self.__parseRspIntoJSON(care, response)
+
+        return response
+
+    def at_customservice(self, idx: int = None, cstype: str = None, value: str = ""):
+        """Sets or queries Custom Service. Max 5 Characteristics can be added.
+            Several values cannot be changed while connected/connecting or advertising.
+
+        :param idx: service index
+        :type idx : number
+        :param cstype: custom service parameter type
+        :type cstype : str
+        :param value: value
+        :type value : str
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+        care = self.__at_customservice(idx, cstype, value)
+        response = self.BleuIORESP()
+        self.__parseRspIntoJSON(care, response)
+
+        return response
+
+    def at_customservice_start(self):
+        """Starts the Custom Service based on the settings set by AT+CUSTOMSERVICE= Command.
+            Cannot be started while connected/connecting or advertising
+
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+        care = self.__at_customservice_start()
+        response = self.BleuIORESP()
+        self.__parseRspIntoJSON(care, response)
+
+        return response
+
+    def at_customservice_stop(self):
+        """Stops the Custom Service.
+            Cannot be changed while connected/connecting or advertising.
+
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+        care = self.__at_customservice_stop()
+        response = self.BleuIORESP()
+        self.__parseRspIntoJSON(care, response)
+
+        return response
+
+    def at_customservice_reset(self):
+        """Stops the Custom Service and resets the Custom Service settings set by the AT+CUSTOMSERVICE= command to it's default values.
+            Cannot be changed while connected/connecting or advertising..
+
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+        care = self.__at_customservice_reset()
+        response = self.BleuIORESP()
+        self.__parseRspIntoJSON(care, response)
+
+        return response
+
     def help(self):
         """Shows all AT-Commands.
 
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects. except for Rsp which contains a list of JSON objects.
         :rtype obj BleuIORESP
         """
         care = self.__help()
```

## Comparing `bleuio-1.2.0.dist-info/LICENSE.txt` & `bleuio-1.3.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `bleuio-1.2.0.dist-info/METADATA` & `bleuio-1.3.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 Metadata-Version: 2.1
 Name: bleuio
-Version: 1.2.0
+Version: 1.3.0
 Summary: Library for using the bleuio dongle.
 Home-page: https://smart-sensor-devices-ab.github.io/ssd005-manual/
 Author: Smart Sensor Devices
 Author-email: smartzenzor@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Requires-Dist: pyserial
 
-## Python library v1.2.0 for BleuIO
+## Python library v1.3.0 for BleuIO
 
-### Supports BleuIO v.2.2.1 or later
+### Supports BleuIO v.2.3.0 or later
 
 > NOTE: Does not support 2.2.0 or earlier version of BleuIO firmware
 
+### Changes
+
+#### 1.3.0
+
+- Added support for commands introduced in BleuIO fw version 2.2.2 and 2.3.0
+- Fixed a bug where the BLE status variables for connection wasn't updated properly.
+- Increased the time trying to connect to the selected Dongle COM port before aborting.
+
+#### 1.2.0
+
+- Supports and makes use of the new Verbose mode introduced 2.2.1
+
 ### Instructions
 
 - Install the library by running:
 
 ```shell
 pip install bleuio
 ```
@@ -697,14 +709,63 @@
 
         :param conn_idx: connection index, format: xxxx
         :type conn_idx : hex str
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
         :rtype: obj BleuIORESP
         """
 
+    def at_scanfilter(self, sftype: str = None, value: str = ""):
+        """Sets or queries the scanfilter. There are three types of scanfilter, filter by name, filter by uuid or by manufacturer specific ID.
+
+        :param sftype: scan filter parameter type
+        :type sftype : str
+        :param value: value
+        :type value : str
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+
+    def at_customservice(self, idx: int = None, cstype: str = None, value: str = ""):
+        """Sets or queries Custom Service. Max 5 Characteristics can be added.
+            Several values cannot be changed while connected/connecting or advertising.
+
+        :param idx: service index
+        :type idx : number
+        :param cstype: custom service parameter type
+        :type cstype : str
+        :param value: value
+        :type value : str
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+
+    def at_customservice_start(self):
+        """Starts the Custom Service based on the settings set by AT+CUSTOMSERVICE= Command.
+            Cannot be started while connected/connecting or advertising
+
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+
+    def at_customservice_stop(self):
+        """Stops the Custom Service.
+            Cannot be changed while connected/connecting or advertising.
+
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+
+    def at_customservice_reset(self):
+        """Stops the Custom Service and resets the Custom Service settings set by the AT+CUSTOMSERVICE= command to it's default values.
+            Cannot be changed while connected/connecting or advertising..
+
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+
     def help(self):
         """Shows all AT-Commands.
 
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects. except for Rsp which contains a list of JSON objects.
         :rtype obj BleuIORESP
         """
```

## Comparing `bleuio-1.2.0.dist-info/RECORD` & `bleuio-1.3.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 bleuio_lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-bleuio_lib/bleuio_funcs.py,sha256=NqTrO7uiiHJxLevwnvPLE_fFcxhTjtgt-7MhhuGV648,62717
+bleuio_lib/bleuio_funcs.py,sha256=284cCvhdR2lKHg_aI7yfYhNgSsVAmY8Z48Xzj67n6PI,68552
 bleuio_lib/exceptions.py,sha256=nhsxieAzx-XkSOIDzOuIN4puTvqby4QW3DH-JIxfSxQ,150
 bleuio_tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bleuio_tests/test_bleuio_funcs.py,sha256=dCjpg3dOM5rZY75BReJj2oiow1GVTXBSgebBsmT4ztg,9476
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_bleuio_funcs.py,sha256=lSewBOnSJVnMGlQZqXFG2KDaFnp7nRDFTzShZqr4imc,2840
-bleuio-1.2.0.dist-info/LICENSE.txt,sha256=_MmtOZ8tMxjdtEDkBcnSHLzX7b2JQP7sqMz_LChR4TQ,1086
-bleuio-1.2.0.dist-info/METADATA,sha256=727xqhyA4cCzkyQMWyQPp9r7_UpsMpcsm4JqvRKbWeo,28622
-bleuio-1.2.0.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-bleuio-1.2.0.dist-info/top_level.txt,sha256=U4c2S2JgfJYrt3NsAsmbxMlWPtWuAuhdHzIYtahVtyg,11
-bleuio-1.2.0.dist-info/RECORD,,
+bleuio-1.3.0.dist-info/LICENSE.txt,sha256=_MmtOZ8tMxjdtEDkBcnSHLzX7b2JQP7sqMz_LChR4TQ,1086
+bleuio-1.3.0.dist-info/METADATA,sha256=MjENUd181Uue63ki8qHHIDT_ZmQ_tKzHTmmShnlONK0,31418
+bleuio-1.3.0.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
+bleuio-1.3.0.dist-info/top_level.txt,sha256=U4c2S2JgfJYrt3NsAsmbxMlWPtWuAuhdHzIYtahVtyg,11
+bleuio-1.3.0.dist-info/RECORD,,
```

