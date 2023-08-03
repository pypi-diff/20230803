# Comparing `tmp/jarbas_hive_mind-0.9.0.tar.gz` & `tmp/jarbas_hive_mind-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jarbas_hive_mind-0.9.0.tar", last modified: Wed Feb 26 04:58:40 2020, max compression
+gzip compressed data, was "dist/jarbas_hive_mind-0.9.1.tar", last modified: Tue Apr 28 18:38:09 2020, max compression
```

## Comparing `jarbas_hive_mind-0.9.0.tar` & `jarbas_hive_mind-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/
--rw-rw-r--   0 user      (1000) user      (1000)      829 2020-02-26 04:58:15.000000 jarbas_hive_mind-0.9.0/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/configuration/
--rw-rw-r--   0 user      (1000) user      (1000)     1122 2020-02-11 00:15:37.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/configuration/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     6511 2020-02-11 00:15:37.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/interface.py
--rw-rw-r--   0 user      (1000) user      (1000)      562 2020-02-04 01:12:03.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/settings.py
--rw-rw-r--   0 user      (1000) user      (1000)      757 2020-02-11 00:15:37.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/exceptions.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/database/
--rw-rw-r--   0 user      (1000) user      (1000)     4567 2020-02-11 00:15:37.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/database/sql_db.py
--rw-rw-r--   0 user      (1000) user      (1000)     4411 2020-02-11 00:15:37.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/database/json_db.py
--rw-rw-r--   0 user      (1000) user      (1000)      738 2020-02-02 03:03:44.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/database/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/slave/
--rw-rw-r--   0 user      (1000) user      (1000)     7305 2020-02-11 00:15:37.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/slave/terminal.py
--rw-rw-r--   0 user      (1000) user      (1000)     3752 2020-02-11 00:15:37.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/slave/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/utils/
--rw-rw-r--   0 user      (1000) user      (1000)     2780 2020-02-11 00:15:37.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/utils/emulation.py
--rw-rw-r--   0 user      (1000) user      (1000)     5139 2020-02-04 02:35:37.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/utils/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     7092 2020-02-11 00:15:37.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/master/
--rw-rw-r--   0 user      (1000) user      (1000)    14181 2020-02-26 04:27:30.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind/master/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      267 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)       17 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       91 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      657 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)      267 2020-02-26 04:58:40.000000 jarbas_hive_mind-0.9.0/jarbas_hive_mind.egg-info/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/
+-rw-rw-r--   0 user      (1000) user      (1000)      829 2020-04-28 00:02:17.000000 jarbas_hive_mind-0.9.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/configuration/
+-rw-rw-r--   0 user      (1000) user      (1000)     1122 2020-04-27 23:16:50.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/configuration/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6511 2020-04-27 23:16:50.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/interface.py
+-rw-rw-r--   0 user      (1000) user      (1000)      562 2020-04-27 23:16:50.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)      757 2020-04-27 23:16:50.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/exceptions.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/database/
+-rw-rw-r--   0 user      (1000) user      (1000)     4567 2020-04-27 23:16:50.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/database/sql_db.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4411 2020-04-27 23:16:50.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/database/json_db.py
+-rw-rw-r--   0 user      (1000) user      (1000)      738 2020-04-27 23:16:50.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/database/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/slave/
+-rw-rw-r--   0 user      (1000) user      (1000)     7305 2020-04-27 23:16:50.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/slave/terminal.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3752 2020-04-27 23:16:50.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/slave/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/utils/
+-rw-rw-r--   0 user      (1000) user      (1000)     2780 2020-04-27 23:16:50.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/utils/emulation.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5139 2020-04-27 23:16:50.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/utils/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7864 2020-04-28 05:09:12.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/master/
+-rw-rw-r--   0 user      (1000) user      (1000)    14486 2020-04-28 00:53:09.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind/master/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      267 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       91 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      657 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      267 2020-04-28 18:38:09.000000 jarbas_hive_mind-0.9.1/jarbas_hive_mind.egg-info/PKG-INFO
```

### Comparing `jarbas_hive_mind-0.9.0/setup.py` & `jarbas_hive_mind-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='jarbas_hive_mind',
-    version='0.9.0',
+    version='0.9.1',
     packages=['jarbas_hive_mind',
               'jarbas_hive_mind.master',
               'jarbas_hive_mind.slave',
               'jarbas_hive_mind.configuration',
               'jarbas_hive_mind.database',
               'jarbas_hive_mind.utils'],
     include_package_data=True,
```

### Comparing `jarbas_hive_mind-0.9.0/jarbas_hive_mind/configuration/__init__.py` & `jarbas_hive_mind-0.9.1/jarbas_hive_mind/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `jarbas_hive_mind-0.9.0/jarbas_hive_mind/interface.py` & `jarbas_hive_mind-0.9.1/jarbas_hive_mind/interface.py`

 * *Files identical despite different names*

### Comparing `jarbas_hive_mind-0.9.0/jarbas_hive_mind/settings.py` & `jarbas_hive_mind-0.9.1/jarbas_hive_mind/settings.py`

 * *Files identical despite different names*

### Comparing `jarbas_hive_mind-0.9.0/jarbas_hive_mind/exceptions.py` & `jarbas_hive_mind-0.9.1/jarbas_hive_mind/exceptions.py`

 * *Files identical despite different names*

### Comparing `jarbas_hive_mind-0.9.0/jarbas_hive_mind/database/sql_db.py` & `jarbas_hive_mind-0.9.1/jarbas_hive_mind/database/sql_db.py`

 * *Files identical despite different names*

### Comparing `jarbas_hive_mind-0.9.0/jarbas_hive_mind/database/json_db.py` & `jarbas_hive_mind-0.9.1/jarbas_hive_mind/database/json_db.py`

 * *Files identical despite different names*

### Comparing `jarbas_hive_mind-0.9.0/jarbas_hive_mind/database/__init__.py` & `jarbas_hive_mind-0.9.1/jarbas_hive_mind/database/__init__.py`

 * *Files identical despite different names*

### Comparing `jarbas_hive_mind-0.9.0/jarbas_hive_mind/slave/terminal.py` & `jarbas_hive_mind-0.9.1/jarbas_hive_mind/slave/terminal.py`

 * *Files identical despite different names*

### Comparing `jarbas_hive_mind-0.9.0/jarbas_hive_mind/slave/__init__.py` & `jarbas_hive_mind-0.9.1/jarbas_hive_mind/slave/__init__.py`

 * *Files identical despite different names*

### Comparing `jarbas_hive_mind-0.9.0/jarbas_hive_mind/utils/emulation.py` & `jarbas_hive_mind-0.9.1/jarbas_hive_mind/utils/emulation.py`

 * *Files identical despite different names*

### Comparing `jarbas_hive_mind-0.9.0/jarbas_hive_mind/utils/__init__.py` & `jarbas_hive_mind-0.9.1/jarbas_hive_mind/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `jarbas_hive_mind-0.9.0/jarbas_hive_mind/__init__.py` & `jarbas_hive_mind-0.9.1/jarbas_hive_mind/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import base64
 from twisted.internet import reactor, ssl
+from twisted.internet.error import ReactorNotRunning
 from jarbas_hive_mind.master import HiveMind, HiveMindProtocol
 from jarbas_hive_mind.configuration import CONFIGURATION
 from jarbas_hive_mind.settings import DEFAULT_PORT
 from jarbas_hive_mind.utils import create_self_signed_cert
 from jarbas_hive_mind.exceptions import SecureConnectionFailed, ConnectionError
 from jarbas_utils.messagebus import get_mycroft_bus
 from jarbas_utils.log import LOG
@@ -154,51 +155,69 @@
         name = key_name.split("/")[-1].replace(".key", "")
         create_self_signed_cert(path, name)
         cert = path + "/" + name + ".crt"
         key = path + "/" + name + ".key"
         LOG.info("key created at: " + key)
         LOG.info("crt created at: " + cert)
 
-    def secure_listen(self, key=None, cert=None):
+    def secure_listen(self, key=None, cert=None, factory=None, protocol=None):
         self._use_ssl = True
         key = key or self.ssl_key
         cert = cert or self.ssl_cert
 
         # SSL server context: load server key and certificate
         contextFactory = ssl.DefaultOpenSSLContextFactory(key, cert)
 
-        factory = HiveMind(bus=self.bus)
-        factory.protocol = HiveMindProtocol
+        factory = factory or HiveMind(bus=self.bus)
+        factory.protocol = protocol or HiveMindProtocol
         if self.max_cons >= 0:
             factory.setProtocolOptions(maxConnections=self.max_cons)
         factory.bind(self)
+        self.factory = factory
         reactor.listenSSL(self.port, factory, contextFactory)
         LOG.info("HiveMind Listening: " + self.address)
         if self._autorun and not reactor.running:
             reactor.run()
         return factory
 
-    def unsafe_listen(self):
+    def unsafe_listen(self, factory=None, protocol=None):
         self._use_ssl = False
-        factory = HiveMind(bus=self.bus)
-        factory.protocol = HiveMindProtocol
+        factory = factory or HiveMind(bus=self.bus)
+        factory.protocol = protocol or HiveMindProtocol
         if self.max_cons >= 0:
             factory.setProtocolOptions(maxConnections=self.max_cons)
         factory.bind(self)
+        self.factory = factory
         reactor.listenTCP(self.port, factory)
         LOG.info("HiveMind Listening (UNSECURED): " + self.address)
         if self._autorun and not reactor.running:
             reactor.run()
         return factory
 
-    def listen(self):
+    def listen(self, factory=None, protocol=None):
         if self.is_secure:
-            return self.secure_listen()
+            return self.secure_listen(factory=factory, protocol=protocol)
         else:
-            return self.unsafe_listen()
+            return self.unsafe_listen(factory=factory, protocol=protocol)
+
+    def stop(self):
+        """Stop the reactor and join the reactor thread until it stops.
+        """
+        try:
+            reactor.stop()
+        except ReactorNotRunning:
+            LOG.info("twisted reactor stopped")
+        except Exception as e:
+            LOG.error(e)
+
+    def stop_from_thread(self):
+        reactor.callFromThread(self.stop)
+        for p in reactor.getDelayedCalls():
+            if p.active():
+                p.cancel()
 
 
 def get_listener(port=DEFAULT_PORT, max_connections=-1, bus=None):
     return HiveMindListener(port, max_connections, bus)
 
 
 def get_connection(host="127.0.0.1", port=DEFAULT_PORT):
```

### Comparing `jarbas_hive_mind-0.9.0/jarbas_hive_mind/master/__init__.py` & `jarbas_hive_mind-0.9.1/jarbas_hive_mind/master/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,39 @@
 
 
 platform = "HiveMindV0.7"
 
 
 # protocol
 class HiveMindProtocol(WebSocketServerProtocol):
-    def onConnect(self, request):
 
-        LOG.info("Client connecting: {0}".format(request.peer))
+    @staticmethod
+    def decode_auth(request):
         auth = request.headers.get("authorization")
         if not auth:
             cookie = request.headers.get("cookie")
             if cookie:
                 auth = cookie.replace("X-Authorization=", "")
                 userpass_encoded = bytes(auth, encoding="utf-8")
         else:
-            userpass_encoded = bytes(auth, encoding="utf-8")[2:-1]
+            userpass_encoded = bytes(auth, encoding="utf-8")
+            if userpass_encoded.startswith(b"Basic "):
+                userpass_encoded = userpass_encoded[6:-2]
+            else:
+                userpass_encoded = userpass_encoded[2:-1]
 
         userpass_decoded = base64.b64decode(userpass_encoded).decode("utf-8")
         name, key = userpass_decoded.split(":")
+        return name, key
+
+    def onConnect(self, request):
+
+        LOG.info("Client connecting: {0}".format(request.peer))
+
+        name, key = self.decode_auth(request)
 
         ip = request.peer.split(":")[1]
         context = {"source": self.peer}
         self.platform = request.headers.get("platform", "unknown")
 
         try:
             with ClientDatabase() as users:
```

### Comparing `jarbas_hive_mind-0.9.0/jarbas_hive_mind.egg-info/SOURCES.txt` & `jarbas_hive_mind-0.9.1/jarbas_hive_mind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

