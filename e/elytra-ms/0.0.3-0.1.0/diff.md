# Comparing `tmp/elytra_ms-0.0.3.tar.gz` & `tmp/elytra_ms-0.1.0.tar.gz`

## Comparing `elytra_ms-0.0.3.tar` & `elytra_ms-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/const.py
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/core.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/protocols.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/bedrock_realms/__init__.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/bedrock_realms/models.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/scripts/auth_device_code.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/scripts/authenticate.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/__init__.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/core.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/rta.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/club/__init__.py
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/club/models.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/peoplehub/__init__.py
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/peoplehub/models.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/profile/__init__.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/profile/models.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/LICENSE
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/README.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/const.py
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/core.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/protocols.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/bedrock_realms/__init__.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/bedrock_realms/models.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/scripts/auth_device_code.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/scripts/authenticate.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/xbox/__init__.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/xbox/core.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/xbox/rta.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/xbox/club/__init__.py
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/xbox/club/models.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/xbox/peoplehub/__init__.py
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/xbox/peoplehub/models.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/xbox/profile/__init__.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/elytra/xbox/profile/models.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/README.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 elytra_ms-0.1.0/PKG-INFO
```

### Comparing `elytra_ms-0.0.3/elytra/core.py` & `elytra_ms-0.1.0/elytra/core.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/elytra/protocols.py` & `elytra_ms-0.1.0/elytra/protocols.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/elytra/bedrock_realms/__init__.py` & `elytra_ms-0.1.0/elytra/bedrock_realms/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/elytra/bedrock_realms/models.py` & `elytra_ms-0.1.0/elytra/bedrock_realms/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     minigame_name: NoneType
     minigame_id: NoneType
     minigame_image: NoneType
     active_slot: int
     slots: NoneType
     member: bool
     subscription_refresh_status: NoneType
+    owner_uuid: str = msgspec.field(name="ownerUUID")
     club_id: typing.Optional[int] = None
-    owner_uuid: typing.Optional[str] = None
     motd: typing.Optional[str] = None
 
 
 @add_decoder
 class MultiRealmResponse(ParsableCamelModel):
     servers: list[FullRealm]
```

### Comparing `elytra_ms-0.0.3/elytra/scripts/auth_device_code.py` & `elytra_ms-0.1.0/elytra/scripts/auth_device_code.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/elytra/scripts/authenticate.py` & `elytra_ms-0.1.0/elytra/scripts/authenticate.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/elytra/xbox/rta.py` & `elytra_ms-0.1.0/elytra/xbox/rta.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/elytra/xbox/club/__init__.py` & `elytra_ms-0.1.0/elytra/xbox/club/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/elytra/xbox/club/models.py` & `elytra_ms-0.1.0/elytra/xbox/club/models.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/elytra/xbox/peoplehub/__init__.py` & `elytra_ms-0.1.0/elytra/xbox/peoplehub/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/elytra/xbox/peoplehub/models.py` & `elytra_ms-0.1.0/elytra/xbox/peoplehub/models.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/elytra/xbox/profile/__init__.py` & `elytra_ms-0.1.0/elytra/xbox/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/.gitignore` & `elytra_ms-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/LICENSE` & `elytra_ms-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/README.md` & `elytra_ms-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/pyproject.toml` & `elytra_ms-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.3/PKG-INFO` & `elytra_ms-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elytra-ms
-Version: 0.0.3
+Version: 0.1.0
 Summary: A Python Library for various Microsoft APIs, including the Xbox and Bedrock Realms APIs.
 Project-URL: Homepage, https://github.com/AstreaTSS/elytra-ms
 Author: AstreaTSS
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

