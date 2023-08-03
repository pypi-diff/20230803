# Comparing `tmp/octodns-powerdns-0.0.3.tar.gz` & `tmp/octodns-powerdns-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns-powerdns-0.0.3.tar", last modified: Fri Dec 23 01:52:56 2022, max compression
+gzip compressed data, was "octodns-powerdns-0.0.4.tar", last modified: Thu Aug  3 13:13:10 2023, max compression
```

## Comparing `octodns-powerdns-0.0.3.tar` & `octodns-powerdns-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2022-12-23 01:52:56.635981 octodns-powerdns-0.0.3/
--rw-r--r--   0 ross       (501) staff       (20)     2673 2022-12-23 01:52:56.635581 octodns-powerdns-0.0.3/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)     2342 2022-10-26 15:20:40.000000 octodns-powerdns-0.0.3/README.md
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2022-12-23 01:52:56.631592 octodns-powerdns-0.0.3/octodns_powerdns/
--rw-r--r--   0 ross       (501) staff       (20)    20697 2022-12-23 01:52:44.000000 octodns-powerdns-0.0.3/octodns_powerdns/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)     1728 2022-10-26 14:47:02.000000 octodns-powerdns-0.0.3/octodns_powerdns/record.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2022-12-23 01:52:56.635150 octodns-powerdns-0.0.3/octodns_powerdns.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)     2673 2022-12-23 01:52:56.000000 octodns-powerdns-0.0.3/octodns_powerdns.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      273 2022-12-23 01:52:56.000000 octodns-powerdns-0.0.3/octodns_powerdns.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2022-12-23 01:52:56.000000 octodns-powerdns-0.0.3/octodns_powerdns.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)      243 2022-12-23 01:52:56.000000 octodns-powerdns-0.0.3/octodns_powerdns.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       17 2022-12-23 01:52:56.000000 octodns-powerdns-0.0.3/octodns_powerdns.egg-info/top_level.txt
--rw-r--r--   0 ross       (501) staff       (20)       38 2022-12-23 01:52:56.636086 octodns-powerdns-0.0.3/setup.cfg
--rw-r--r--   0 ross       (501) staff       (20)     1760 2022-10-26 15:20:40.000000 octodns-powerdns-0.0.3/setup.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-03 13:13:10.252740 octodns-powerdns-0.0.4/
+-rw-r--r--   0 ross       (501) staff       (20)     2429 2023-08-03 13:13:10.252368 octodns-powerdns-0.0.4/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)     2098 2023-07-28 20:27:09.000000 octodns-powerdns-0.0.4/README.md
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-03 13:13:10.249837 octodns-powerdns-0.0.4/octodns_powerdns/
+-rw-r--r--   0 ross       (501) staff       (20)    22243 2023-08-03 13:13:00.000000 octodns-powerdns-0.0.4/octodns_powerdns/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)     1728 2023-02-04 19:19:10.000000 octodns-powerdns-0.0.4/octodns_powerdns/record.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-03 13:13:10.251258 octodns-powerdns-0.0.4/octodns_powerdns.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)     2429 2023-08-03 13:13:10.000000 octodns-powerdns-0.0.4/octodns_powerdns.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      328 2023-08-03 13:13:10.000000 octodns-powerdns-0.0.4/octodns_powerdns.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-03 13:13:10.000000 octodns-powerdns-0.0.4/octodns_powerdns.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)      246 2023-08-03 13:13:10.000000 octodns-powerdns-0.0.4/octodns_powerdns.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       17 2023-08-03 13:13:10.000000 octodns-powerdns-0.0.4/octodns_powerdns.egg-info/top_level.txt
+-rw-r--r--   0 ross       (501) staff       (20)      309 2023-02-04 19:19:10.000000 octodns-powerdns-0.0.4/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2023-08-03 13:13:10.252849 octodns-powerdns-0.0.4/setup.cfg
+-rw-r--r--   0 ross       (501) staff       (20)     2080 2023-06-28 23:41:56.000000 octodns-powerdns-0.0.4/setup.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-03 13:13:10.251807 octodns-powerdns-0.0.4/tests/
+-rw-r--r--   0 ross       (501) staff       (20)    22491 2023-08-03 13:08:53.000000 octodns-powerdns-0.0.4/tests/test_octodns_provider_powerdns.py
```

### Comparing `octodns-powerdns-0.0.3/PKG-INFO` & `octodns-powerdns-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-powerdns
-Version: 0.0.3
+Version: 0.0.4
 Summary:  PowerDNS API provider for octoDNS
 Home-page: https://github.com/octodns/octodns-powerdns
 Author: Ross McFaland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -27,46 +27,40 @@
 
 Pinning specific versions or SHAs is recommended to avoid unplanned upgrades.
 
 ##### Versions
 
 ```
 # Start with the latest versions and don't just copy what's here
-octodns==0.9.14
-octodns-powerdns==0.0.1
-requests==2.26.0
+octodns==0.9.21
+octodns-powerdns==0.0.3
+requests==2.31.0
 ```
 
 ##### SHAs
 
 ```
 # Start with the latest/specific versions and don't just copy what's here
--e git+https://git@github.com/octodns/octodns.git@9da19749e28f68407a1c246dfdf65663cdc1c422#egg=octodns
--e git+https://git@github.com/octodns/octodns-powerdns.git@ec9661f8b335241ae4746eea467a8509205e6a30#egg=octodns_powerdns
-requests==2.26.0
+-e git+https://git@github.com/octodns/octodns.git@67ea0b0ea7961e37b028cfe21c463fa3e5090c8f#egg=octodns
+-e git+https://git@github.com/octodns/octodns-powerdns.git@e33349e5edfe4e12a1d179a32a5f70a8ec4c2aad#egg=octodns_powerdns
+requests==2.31.0
 ```
 
 ### Configuration
 
 ```yaml
 providers:
   powerdns:
       class: octodns_powerdns.PowerDnsProvider
       # The host on which PowerDNS api is listening (required)
       host: fqdn
       # The port on which PowerDNS api is listening (optional, default 8081)
       port: 8081
       # The api key that grans access (required, example is using an env var)
       api_key: env/POWERDNS_API_KEY
-      # The nameservers to use for this provider (optional, default unmanaged)
-      nameserver_values:
-          - 1.2.3.4.
-          - 1.2.3.5.
-      # The nameserver record TTL when managed, (optional, default 600)
-      nameserver_ttl: 300
 ```
 
 ### Support Information
 
 #### Records
 
 All octoDNS record types are supported.
```

### Comparing `octodns-powerdns-0.0.3/README.md` & `octodns-powerdns-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,46 +14,40 @@
 
 Pinning specific versions or SHAs is recommended to avoid unplanned upgrades.
 
 ##### Versions
 
 ```
 # Start with the latest versions and don't just copy what's here
-octodns==0.9.14
-octodns-powerdns==0.0.1
-requests==2.26.0
+octodns==0.9.21
+octodns-powerdns==0.0.3
+requests==2.31.0
 ```
 
 ##### SHAs
 
 ```
 # Start with the latest/specific versions and don't just copy what's here
--e git+https://git@github.com/octodns/octodns.git@9da19749e28f68407a1c246dfdf65663cdc1c422#egg=octodns
--e git+https://git@github.com/octodns/octodns-powerdns.git@ec9661f8b335241ae4746eea467a8509205e6a30#egg=octodns_powerdns
-requests==2.26.0
+-e git+https://git@github.com/octodns/octodns.git@67ea0b0ea7961e37b028cfe21c463fa3e5090c8f#egg=octodns
+-e git+https://git@github.com/octodns/octodns-powerdns.git@e33349e5edfe4e12a1d179a32a5f70a8ec4c2aad#egg=octodns_powerdns
+requests==2.31.0
 ```
 
 ### Configuration
 
 ```yaml
 providers:
   powerdns:
       class: octodns_powerdns.PowerDnsProvider
       # The host on which PowerDNS api is listening (required)
       host: fqdn
       # The port on which PowerDNS api is listening (optional, default 8081)
       port: 8081
       # The api key that grans access (required, example is using an env var)
       api_key: env/POWERDNS_API_KEY
-      # The nameservers to use for this provider (optional, default unmanaged)
-      nameserver_values:
-          - 1.2.3.4.
-          - 1.2.3.5.
-      # The nameserver record TTL when managed, (optional, default 600)
-      nameserver_ttl: 300
 ```
 
 ### Support Information
 
 #### Records
 
 All octoDNS record types are supported.
```

### Comparing `octodns-powerdns-0.0.3/octodns_powerdns/__init__.py` & `octodns-powerdns-0.0.4/octodns_powerdns/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #
 #
 #
 
-from requests import HTTPError, Session
-from operator import itemgetter
 import logging
+from operator import itemgetter
 
-from octodns.record import Record
+from requests import HTTPError, Session
+
+from octodns import __VERSION__ as octodns_version
 from octodns.provider import ProviderException
 from octodns.provider.base import BaseProvider
+from octodns.record import Record
 
 from .record import PowerDnsLuaRecord
 
-__VERSION__ = '0.0.3'
+__VERSION__ = '0.0.4'
 
 
 def _escape_unescaped_semicolons(value):
     pieces = value.split(';')
     if len(pieces) == 1:
         return value
     last = pieces.pop()
@@ -47,14 +49,23 @@
             'TLSA',
             'TXT',
             PowerDnsLuaRecord._type,
         )
     )
     TIMEOUT = 5
 
+    POWERDNS_MODES_OF_OPERATION = {
+        'native',
+        'primary',
+        'secondary',
+        'master',
+        'slave',
+    }
+    POWERDNS_LEGACY_MODES_OF_OPERATION = {'native', 'master', 'slave'}
+
     def __init__(
         self,
         id,
         host,
         api_key,
         port=8081,
         scheme="http",
@@ -78,19 +89,35 @@
         self.port = port
         self.scheme = scheme
         self.timeout = timeout
 
         self._powerdns_version = None
 
         sess = Session()
-        sess.headers.update({'X-API-Key': api_key})
+        sess.headers.update(
+            {
+                'X-API-Key': api_key,
+                'User-Agent': f'octodns/{octodns_version} octodns-powerdns/{__VERSION__}',
+            }
+        )
         self._sess = sess
 
         self.soa_edit_api = soa_edit_api
-        self.mode_of_operation = mode_of_operation
+        # to avoid making an API call to get the pdns version during the
+        # constructor we'll check the value against the larger set of possible
+        # values. the first time we do something that requires the mode of
+        # operation we'll do the work of fully vetting it based on version
+        if mode_of_operation not in self.POWERDNS_MODES_OF_OPERATION:
+            raise ValueError(
+                f'invalid mode_of_operation "{mode_of_operation}" - available values: {self.POWERDNS_MODES_OF_OPERATION}'
+            )
+        # start out with an unset valid
+        self._mode_of_operation = None
+        # store what we were passed so that we can check it when the time comes
+        self._mode_of_operation_arg = mode_of_operation
 
     def _request(self, method, path, data=None):
         self.log.debug('_request: method=%s, path=%s', method, path)
 
         url = (
             f'{self.scheme}://{self.host}:{self.port}/api/v1/servers/'
             f'localhost/{path}'.rstrip('/')
@@ -303,43 +330,49 @@
         # True
         # >>> [4, 1, 3] >= [4, 3]
         # False
         return self._soa_edit_api
 
     @soa_edit_api.setter
     def soa_edit_api(self, value):
-        settings = [
-            "default",
-            "increase",
-            "epoch",
-            "soa-edit",
-            "soa-edit-increase",
-        ]
+        settings = {
+            'default',
+            'increase',
+            'epoch',
+            'soa-edit',
+            'soa-edit-increase',
+        }
 
         if value in settings:
             self._soa_edit_api = value
         else:
-            raise ValueError(f'"soa_edit_api" - possibile values: {settings}')
+            raise ValueError(
+                f'invalid soa_edit_api, "{value}" - available values: {settings}'
+            )
 
     @property
     def mode_of_operation(self):
-        return self._mode_of_operation
-
-    @mode_of_operation.setter
-    def mode_of_operation(self, value):
-        if self.powerdns_version >= [4, 5]:
-            settings = ["native", "primary", "secondary", "master", "slave"]
-        else:
-            settings = ["native", "master", "slave"]
-        if value in settings:
+        if self._mode_of_operation is None:
+            # start with what we were passed as a provider arg
+            value = self._mode_of_operation_arg
+            # we previously validated things against
+            # POWERDNS_MODES_OF_OPERATION, the newer/larger set. If we're
+            # running an (much) older version we need to check against the
+            # reduced set of options now that we can get the version
+            if (
+                self.powerdns_version < [4, 5]
+                and value not in self.POWERDNS_LEGACY_MODES_OF_OPERATION
+            ):
+                raise ValueError(
+                    f'invalid mode_of_operation "{value}" - available values: {self.POWERDNS_LEGACY_MODES_OF_OPERATION}'
+                )
+            # we have a value we can now confidentily use
             self._mode_of_operation = value
-        else:
-            raise ValueError(
-                f'"mode_of_operation" - possible values: {settings}'
-            )
+
+        return self._mode_of_operation
 
     @property
     def check_status_not_found(self):
         # >=4.2.x returns 404 when not found
         return self.powerdns_version >= [4, 2]
 
     def populate(self, zone, target=False, lenient=False):
```

### Comparing `octodns-powerdns-0.0.3/octodns_powerdns/record.py` & `octodns-powerdns-0.0.4/octodns_powerdns/record.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from octodns.record import Record, ValuesMixin
 from octodns.equality import EqualityTupleMixin
+from octodns.record import Record, ValuesMixin
 
 
 class _PowerDnsLuaValue(EqualityTupleMixin, dict):
     # See https://doc.powerdns.com/authoritative/lua-records/index.html for the
     # LUA record docs and
     # https://gist.github.com/ahupowerdns/1e8bfbba95a277a4fac09cb3654eb2ac
     # has some good example scripts
```

### Comparing `octodns-powerdns-0.0.3/octodns_powerdns.egg-info/PKG-INFO` & `octodns-powerdns-0.0.4/octodns_powerdns.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-powerdns
-Version: 0.0.3
+Version: 0.0.4
 Summary:  PowerDNS API provider for octoDNS
 Home-page: https://github.com/octodns/octodns-powerdns
 Author: Ross McFaland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -27,46 +27,40 @@
 
 Pinning specific versions or SHAs is recommended to avoid unplanned upgrades.
 
 ##### Versions
 
 ```
 # Start with the latest versions and don't just copy what's here
-octodns==0.9.14
-octodns-powerdns==0.0.1
-requests==2.26.0
+octodns==0.9.21
+octodns-powerdns==0.0.3
+requests==2.31.0
 ```
 
 ##### SHAs
 
 ```
 # Start with the latest/specific versions and don't just copy what's here
--e git+https://git@github.com/octodns/octodns.git@9da19749e28f68407a1c246dfdf65663cdc1c422#egg=octodns
--e git+https://git@github.com/octodns/octodns-powerdns.git@ec9661f8b335241ae4746eea467a8509205e6a30#egg=octodns_powerdns
-requests==2.26.0
+-e git+https://git@github.com/octodns/octodns.git@67ea0b0ea7961e37b028cfe21c463fa3e5090c8f#egg=octodns
+-e git+https://git@github.com/octodns/octodns-powerdns.git@e33349e5edfe4e12a1d179a32a5f70a8ec4c2aad#egg=octodns_powerdns
+requests==2.31.0
 ```
 
 ### Configuration
 
 ```yaml
 providers:
   powerdns:
       class: octodns_powerdns.PowerDnsProvider
       # The host on which PowerDNS api is listening (required)
       host: fqdn
       # The port on which PowerDNS api is listening (optional, default 8081)
       port: 8081
       # The api key that grans access (required, example is using an env var)
       api_key: env/POWERDNS_API_KEY
-      # The nameservers to use for this provider (optional, default unmanaged)
-      nameserver_values:
-          - 1.2.3.4.
-          - 1.2.3.5.
-      # The nameserver record TTL when managed, (optional, default 600)
-      nameserver_ttl: 300
 ```
 
 ### Support Information
 
 #### Records
 
 All octoDNS record types are supported.
```

