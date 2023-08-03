# Comparing `tmp/secrets-storage-0.8.0.tar.gz` & `tmp/secrets-storage-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-storage-0.8.0.tar", last modified: Mon Aug 16 15:51:58 2021, max compression
+gzip compressed data, was "secrets-storage-0.9.0.tar", last modified: Tue Aug 17 07:30:36 2021, max compression
```

## Comparing `secrets-storage-0.8.0.tar` & `secrets-storage-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 15:51:58.831780 secrets-storage-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11466 2021-08-16 15:51:46.000000 secrets-storage-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-08-16 15:51:46.000000 secrets-storage-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2877 2021-08-16 15:51:58.831780 secrets-storage-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2021-08-16 15:51:46.000000 secrets-storage-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      424 2021-08-16 15:51:46.000000 secrets-storage-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 15:51:58.827780 secrets-storage-0.8.0/secrets_storage/
--rw-r--r--   0 runner    (1001) docker     (121)      729 2021-08-16 15:51:46.000000 secrets-storage-0.8.0/secrets_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2021-08-16 15:51:46.000000 secrets-storage-0.8.0/secrets_storage/storages.py
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-08-16 15:51:46.000000 secrets-storage-0.8.0/secrets_storage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 15:51:58.831780 secrets-storage-0.8.0/secrets_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2877 2021-08-16 15:51:58.000000 secrets-storage-0.8.0/secrets_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      368 2021-08-16 15:51:58.000000 secrets-storage-0.8.0/secrets_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-16 15:51:58.000000 secrets-storage-0.8.0/secrets_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-16 15:51:58.000000 secrets-storage-0.8.0/secrets_storage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-08-16 15:51:58.000000 secrets-storage-0.8.0/secrets_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-08-16 15:51:58.000000 secrets-storage-0.8.0/secrets_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-16 15:51:58.831780 secrets-storage-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-08-16 15:51:46.000000 secrets-storage-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 07:30:36.291679 secrets-storage-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    11466 2021-08-17 07:30:21.000000 secrets-storage-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2021-08-17 07:30:21.000000 secrets-storage-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2877 2021-08-17 07:30:36.291679 secrets-storage-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1523 2021-08-17 07:30:21.000000 secrets-storage-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2021-08-17 07:30:21.000000 secrets-storage-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 07:30:36.291679 secrets-storage-0.9.0/secrets_storage/
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2021-08-17 07:30:21.000000 secrets-storage-0.9.0/secrets_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2589 2021-08-17 07:30:21.000000 secrets-storage-0.9.0/secrets_storage/storages.py
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2021-08-17 07:30:21.000000 secrets-storage-0.9.0/secrets_storage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 07:30:36.291679 secrets-storage-0.9.0/secrets_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2877 2021-08-17 07:30:35.000000 secrets-storage-0.9.0/secrets_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2021-08-17 07:30:36.000000 secrets-storage-0.9.0/secrets_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-17 07:30:35.000000 secrets-storage-0.9.0/secrets_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-17 07:30:35.000000 secrets-storage-0.9.0/secrets_storage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-08-17 07:30:35.000000 secrets-storage-0.9.0/secrets_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-08-17 07:30:35.000000 secrets-storage-0.9.0/secrets_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-17 07:30:36.291679 secrets-storage-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-08-17 07:30:21.000000 secrets-storage-0.9.0/setup.py
```

### Comparing `secrets-storage-0.8.0/LICENSE` & `secrets-storage-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-storage-0.8.0/PKG-INFO` & `secrets-storage-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-storage
-Version: 0.8.0
+Version: 0.9.0
 Summary: Helper for getting secrets from different storage
 Home-page: https://github.com/bigbag/secrets-storage
 Author: Pavel Liashkov
 Author-email: pavel.liashkov@protonmail.com
 Maintainer: Pavel Liashkov
 Maintainer-email: pavel.liashkov@protonmail.com
 License: Apache License, Version 2.0
```

### Comparing `secrets-storage-0.8.0/README.md` & `secrets-storage-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `secrets-storage-0.8.0/secrets_storage/__init__.py` & `secrets-storage-0.9.0/secrets_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `secrets-storage-0.8.0/secrets_storage/storages.py` & `secrets-storage-0.9.0/secrets_storage/storages.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,19 +16,26 @@
         pass
 
     @abc.abstractmethod
     def get_secret(self, name: str, fallback_value: t.Any = None) -> t.Any:
         pass
 
 
+KV_VERSION1 = "v1"
+KV_VERSION2 = "v2"
+
+SUPPORT_KV_VERSIONS = (KV_VERSION1, KV_VERSION2)
+
+
 @dataclass
 class VaultStorage(BaseStorage):
     host: str
     namespace: str
     role: str
+    kv_version: str = KV_VERSION1
 
     name: str = "vault_storage"
     available: bool = True
     ssl_verify: bool = False
 
     auth_mount_point: str = "kubernetes"
     auth_token_path: str = "/var/run/secrets/kubernetes.io/serviceaccount/token"
@@ -37,35 +44,43 @@
 
     def __post_init__(self):
         if not self.enabled:
             self.secrets = {}
         else:
             self.secrets = self._get_secrets()
 
+    @property
+    def enabled(self) -> bool:
+        return bool(self.available and self.host and self.auth_token_path and self.namespace)
+
     def _get_client_token(self, client: hvac.Client) -> str:
         with open(self.auth_token_path) as f:
             sa_token = f.read()
 
         auth_info = client.auth_kubernetes(
             role=self.role, jwt=sa_token, mount_point=self.auth_mount_point
         )
         client_token = auth_info.get("auth", {}).get("client_token")
         if not client_token:
             raise ValueError("Not found vault token.")
 
         return str(client_token)
 
+    def _parse_secrets(self, raw_data: t.Dict[t.Any, t.Any]) -> t.Any:
+        if self.kv_version == KV_VERSION1:
+            return raw_data.get("data", {})
+        elif self.kv_version == KV_VERSION2:
+            return raw_data.get("data", {}).get("data", {})
+
+        raise ValueError(f"Not valifd kv version: '{self.kv_version}'")
+
     def _get_secrets(self):
         client = hvac.Client(url=self.host, verify=self.ssl_verify)
         client.token = self._get_client_token(client)
-        return client.read(self.namespace).get("data", {})
-
-    @property
-    def enabled(self) -> bool:
-        return bool(self.available and self.host and self.auth_token_path and self.namespace)
+        return self._parse_secrets(client.read(self.namespace))
 
     def get_secret(self, name: str, fallback_value: t.Any = None) -> t.Any:
         return self.secrets.get(name) or fallback_value
 
 
 @dataclass
 class ENVStorage(BaseStorage):
```

### Comparing `secrets-storage-0.8.0/secrets_storage.egg-info/PKG-INFO` & `secrets-storage-0.9.0/secrets_storage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-storage
-Version: 0.8.0
+Version: 0.9.0
 Summary: Helper for getting secrets from different storage
 Home-page: https://github.com/bigbag/secrets-storage
 Author: Pavel Liashkov
 Author-email: pavel.liashkov@protonmail.com
 Maintainer: Pavel Liashkov
 Maintainer-email: pavel.liashkov@protonmail.com
 License: Apache License, Version 2.0
```

### Comparing `secrets-storage-0.8.0/setup.py` & `secrets-storage-0.9.0/setup.py`

 * *Files identical despite different names*

