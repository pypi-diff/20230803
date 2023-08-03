# Comparing `tmp/sungrow_http_config-0.0.3.tar.gz` & `tmp/sungrow_http_config-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sungrow_http_config-0.0.3.tar", last modified: Wed Aug  2 01:09:33 2023, max compression
+gzip compressed data, was "sungrow_http_config-0.0.4.tar", last modified: Thu Aug  3 12:37:27 2023, max compression
```

## Comparing `sungrow_http_config-0.0.3.tar` & `sungrow_http_config-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 01:09:33.564301 sungrow_http_config-0.0.3/
--rw-r--r--   0 ross       (501) staff       (20)     1072 2023-08-01 09:53:21.000000 sungrow_http_config-0.0.3/LICENSE
--rw-r--r--   0 ross       (501) staff       (20)     1305 2023-08-02 01:09:33.564035 sungrow_http_config-0.0.3/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      747 2023-08-01 09:51:37.000000 sungrow_http_config-0.0.3/README.md
--rw-r--r--   0 ross       (501) staff       (20)      698 2023-08-02 01:09:14.000000 sungrow_http_config-0.0.3/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)       38 2023-08-02 01:09:33.564394 sungrow_http_config-0.0.3/setup.cfg
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 01:09:33.557514 sungrow_http_config-0.0.3/src/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 01:09:33.560613 sungrow_http_config-0.0.3/src/sungrow_http_config/
--rw-r--r--   0 ross       (501) staff       (20)     7222 2023-08-01 11:14:11.000000 sungrow_http_config-0.0.3/src/sungrow_http_config/SungrowHttpConfig.py
--rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-01 09:55:24.000000 sungrow_http_config-0.0.3/src/sungrow_http_config/__init__.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 01:09:33.563626 sungrow_http_config-0.0.3/src/sungrow_http_config.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)     1305 2023-08-02 01:09:33.000000 sungrow_http_config-0.0.3/src/sungrow_http_config.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      347 2023-08-02 01:09:33.000000 sungrow_http_config-0.0.3/src/sungrow_http_config.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-02 01:09:33.000000 sungrow_http_config-0.0.3/src/sungrow_http_config.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)       37 2023-08-02 01:09:33.000000 sungrow_http_config-0.0.3/src/sungrow_http_config.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       20 2023-08-02 01:09:33.000000 sungrow_http_config-0.0.3/src/sungrow_http_config.egg-info/top_level.txt
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-03 12:37:27.032416 sungrow_http_config-0.0.4/
+-rw-r--r--   0 ross       (501) staff       (20)     1072 2023-08-01 09:53:21.000000 sungrow_http_config-0.0.4/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)     1760 2023-08-03 12:37:27.032133 sungrow_http_config-0.0.4/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)     1202 2023-08-03 12:35:38.000000 sungrow_http_config-0.0.4/README.md
+-rw-r--r--   0 ross       (501) staff       (20)      711 2023-08-03 12:36:43.000000 sungrow_http_config-0.0.4/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2023-08-03 12:37:27.032536 sungrow_http_config-0.0.4/setup.cfg
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-03 12:37:27.027213 sungrow_http_config-0.0.4/src/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-03 12:37:27.029603 sungrow_http_config-0.0.4/src/sungrow_http_config/
+-rw-r--r--   0 ross       (501) staff       (20)     9980 2023-08-03 12:32:17.000000 sungrow_http_config-0.0.4/src/sungrow_http_config/SungrowHttpConfig.py
+-rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-01 09:55:24.000000 sungrow_http_config-0.0.4/src/sungrow_http_config/__init__.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-03 12:37:27.031673 sungrow_http_config-0.0.4/src/sungrow_http_config.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)     1760 2023-08-03 12:37:27.000000 sungrow_http_config-0.0.4/src/sungrow_http_config.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      347 2023-08-03 12:37:27.000000 sungrow_http_config-0.0.4/src/sungrow_http_config.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-03 12:37:27.000000 sungrow_http_config-0.0.4/src/sungrow_http_config.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)       46 2023-08-03 12:37:27.000000 sungrow_http_config-0.0.4/src/sungrow_http_config.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       20 2023-08-03 12:37:27.000000 sungrow_http_config-0.0.4/src/sungrow_http_config.egg-info/top_level.txt
```

### Comparing `sungrow_http_config-0.0.3/LICENSE` & `sungrow_http_config-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sungrow_http_config-0.0.3/PKG-INFO` & `sungrow_http_config-0.0.4/src/sungrow_http_config.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sungrow_http_config
-Version: 0.0.3
+Name: sungrow-http-config
+Version: 0.0.4
 Summary: A package to manipulate settings on Sungrow Inverters
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/sungrow_exportlimit
 Project-URL: Bug Tracker, https://github.com/ross-w/sungrow_exportlimit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,13 +12,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sungrow HTTP Config
 
 This is a package to use the Sungrow Local Access HTTP API to configure parameters that are not available over Modbus
 
-It currently only supports settting or unsetting a zero export limit, which is useful if on a variable-rate tariff that can go negative (ie charging you for exports at times there's oversupply in the grid), such as [Amber Electric](http://amber.com.au/) in Australia
+It currently only supports settting or unsetting an export limit, which is useful if on a variable-rate tariff that can go negative (ie charging you for exports at times there's oversupply in the grid), such as [Amber Electric](http://amber.com.au/) in Australia.
+
+Please note that a 0kW export limit is equivalent to unlimited, to set as close to zero as possible, use 0.01kW (1 dekawatt.)
+
+Additionally, note that the reaction time of the inverter to changes in loads can be a little slow, which could result in more use of grid power than anticipated if a new load is switched on. Depending on your differential in price between imports and exports, you may want to configure a bigger export "buffer" to mitigate this.
 
 **WARNING**
 This package has only been tested on a single inverter, and the protocol is not well understood. Using it with anything else could damage your equipment, void your warranty, cause physical damage, or violate your agreement with your network operator.
 
 Do not use this package if you have an export limit normally configured.
```

### Comparing `sungrow_http_config-0.0.3/README.md` & `sungrow_http_config-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Sungrow HTTP Config
 
 This is a package to use the Sungrow Local Access HTTP API to configure parameters that are not available over Modbus
 
-It currently only supports settting or unsetting a zero export limit, which is useful if on a variable-rate tariff that can go negative (ie charging you for exports at times there's oversupply in the grid), such as [Amber Electric](http://amber.com.au/) in Australia
+It currently only supports settting or unsetting an export limit, which is useful if on a variable-rate tariff that can go negative (ie charging you for exports at times there's oversupply in the grid), such as [Amber Electric](http://amber.com.au/) in Australia.
+
+Please note that a 0kW export limit is equivalent to unlimited, to set as close to zero as possible, use 0.01kW (1 dekawatt.)
+
+Additionally, note that the reaction time of the inverter to changes in loads can be a little slow, which could result in more use of grid power than anticipated if a new load is switched on. Depending on your differential in price between imports and exports, you may want to configure a bigger export "buffer" to mitigate this.
 
 **WARNING**
 This package has only been tested on a single inverter, and the protocol is not well understood. Using it with anything else could damage your equipment, void your warranty, cause physical damage, or violate your agreement with your network operator.
 
 Do not use this package if you have an export limit normally configured.
```

### Comparing `sungrow_http_config-0.0.3/pyproject.toml` & `sungrow_http_config-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sungrow_http_config"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
   "requests_retry_on_exceptions",
   "urllib3",
+  "pymodbus"
 ]
 authors = [
   { name="Ross Williamson", email="ross@inertia.net.nz" },
 ]
 description = "A package to manipulate settings on Sungrow Inverters"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `sungrow_http_config-0.0.3/src/sungrow_http_config/SungrowHttpConfig.py` & `sungrow_http_config-0.0.4/src/sungrow_http_config/SungrowHttpConfig.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from urllib3.exceptions import TimeoutStateError
 import requests_retry_on_exceptions as requests
 import json
 import urllib3
 import logging
+import codecs as c
+from pymodbus.constants import Endian
+from pymodbus.payload import BinaryPayloadDecoder
+import pymodbus.register_write_message as modbus_register_write
+from pymodbus.transaction import ModbusRtuFramer
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 class SungrowHttpConfig():
     """ Implementation of the Sungrow Local Access HTTP API
     """
 
@@ -127,35 +132,59 @@
             "lang": self.lang,
             "msgLength": (len(msgValue) // 2),
             "msgType": msgType,
             "msgValue": msgValue,
             "token": self.token
         }
         resp = self._callAPI("/device/passthroughway", req)
+        if not resp.get("result_code")==1:
+            raise Exception("Got unsuccessful message back from device: {resp}".format(resp=resp))
         return resp.get("result_data")
 
-    def setZeroExportLimit(self):
+    def _generateExportLimitCommand(self, dekawattLimit):
+        """ Generates the appropriate modbus command to send for the given limit
+        :param dekawattLimit: Limit to set, in dekawatts (kW * 100)
+        :returns: String containing modbus command string
+        """
+        framer = ModbusRtuFramer(None)
+        arguments = {
+            "address": 31221,
+            "value": dekawattLimit,
+            "write_address": 31221,
+            "transaction": 1,
+            "slave": 1,
+            "protocol": 0x00,
+        }
+        message = modbus_register_write.WriteSingleRegisterRequest(**arguments)
+        raw_packet = framer.buildPacket(message)
+        packet = c.encode(raw_packet, "hex_codec").decode("utf-8").upper()
+        return packet
+
+    def setExportLimit(self, dekawattLimit):
         """ Enable export limit and set to 0kW (zero export limit)
+        :param dekawattLimit: Limit to set, in dekawatts (kW * 100). Note 0 == unlimited, so set 1 for 0.01kW
         :returns: True if successful
         """
 
         msg1 = self._sendHexMessageToDevice("010679F400AA511B") # Turn on feed-in limitation
         msg1resp = msg1.get("data")
         if msg1resp == "010679F400AA511B":
             logging.debug("Feed-in limitation enabled")
         else:
             logging.warning("Problem enabling feed-in limitation")
             return False
 
-        msg2 = self._sendHexMessageToDevice("011079F5000306000003E80000F77E") # Set limit to 0kW
+        exportLimitCommand = self._generateExportLimitCommand(dekawattLimit)
+        logging.debug("Generated modbus export limit command as {command}".format(command=exportLimitCommand))
+        msg2 = self._sendHexMessageToDevice(exportLimitCommand) # Set limit
         msg2resp = msg2.get("data")
-        if msg2resp == "011079F500038966":
-            logging.debug("Feed-in limitation set at 0kW")
+        if msg2resp == exportLimitCommand:
+            logging.debug("Feed-in limitation set at {power}kW".format(power=dekawattLimit/100))
         else:
-            logging.warning("Problem setting feed-in limitation to 0kW")
+            logging.warning("Problem setting feed-in limitation to {power}kW, modbus response was {resp}".format(power=dekawattLimit/100,resp=msg2resp))
             return False
         return True
 
     def unsetExportLimit(self):
         """ Turns off any export limit in place (no limit)
         :returns: True if successful
         """
@@ -163,7 +192,34 @@
         msg1resp = msg1.get("data")
         if msg1resp == "010679F40055115B":
             logging.debug("Feed-in limitation disabled")
         else:
             logging.warning("Problem disabling feed-in limitation")
             return False
         return True
+
+    def _decodeModbusExportLimitPayload(self, modbusMsg):
+        """ Decodes the supplied modbus message into individual registers
+        :param modbusMsg: The hex string representing the modbus response
+        :returns Array of register values
+        """
+        response_data = bytes.fromhex(modbusMsg)
+        data_section = response_data[4:-4]
+        num_registers = len(data_section) // 2
+        registers = [int.from_bytes(data_section[i:i+2], byteorder='little', signed=False) for i in range(0, len(data_section), 2)]
+        return registers
+
+    def getCurrentExportLimit(self):
+        """ Obtains the current export limit setting
+        :returns: The current export limit in dekawatts, or 0 if no limit set
+        """
+        msg1 = self._sendHexMessageToDevice("010379F400081CA2") # Is feed-in limitation on?
+        msg1resp = msg1.get("data")
+        registers = self._decodeModbusExportLimitPayload(msg1resp)
+        if (registers[0]==341): # Feed-in limitation is disabled
+            return 0
+        elif (registers[0]==170):
+            return registers[1]
+        else:
+            raise Exception("Unknown response to query for current export limit: {resp}".format(resp=msg1resp))
+
+        return 0
```

### Comparing `sungrow_http_config-0.0.3/src/sungrow_http_config.egg-info/PKG-INFO` & `sungrow_http_config-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sungrow-http-config
-Version: 0.0.3
+Name: sungrow_http_config
+Version: 0.0.4
 Summary: A package to manipulate settings on Sungrow Inverters
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/sungrow_exportlimit
 Project-URL: Bug Tracker, https://github.com/ross-w/sungrow_exportlimit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,13 +12,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sungrow HTTP Config
 
 This is a package to use the Sungrow Local Access HTTP API to configure parameters that are not available over Modbus
 
-It currently only supports settting or unsetting a zero export limit, which is useful if on a variable-rate tariff that can go negative (ie charging you for exports at times there's oversupply in the grid), such as [Amber Electric](http://amber.com.au/) in Australia
+It currently only supports settting or unsetting an export limit, which is useful if on a variable-rate tariff that can go negative (ie charging you for exports at times there's oversupply in the grid), such as [Amber Electric](http://amber.com.au/) in Australia.
+
+Please note that a 0kW export limit is equivalent to unlimited, to set as close to zero as possible, use 0.01kW (1 dekawatt.)
+
+Additionally, note that the reaction time of the inverter to changes in loads can be a little slow, which could result in more use of grid power than anticipated if a new load is switched on. Depending on your differential in price between imports and exports, you may want to configure a bigger export "buffer" to mitigate this.
 
 **WARNING**
 This package has only been tested on a single inverter, and the protocol is not well understood. Using it with anything else could damage your equipment, void your warranty, cause physical damage, or violate your agreement with your network operator.
 
 Do not use this package if you have an export limit normally configured.
```

