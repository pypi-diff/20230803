# Comparing `tmp/quiltcore-0.3.1.tar.gz` & `tmp/quiltcore-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiltcore-0.3.1.tar", max compression
+gzip compressed data, was "quiltcore-0.3.2.tar", max compression
```

## Comparing `quiltcore-0.3.1.tar` & `quiltcore-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-06-10 04:58:49.699035 quiltcore-0.3.1/LICENSE
--rw-r--r--   0        0        0     1573 2023-07-20 22:18:01.855543 quiltcore-0.3.1/README.md
--rw-r--r--   0        0        0     1115 2023-07-30 04:14:15.411310 quiltcore-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1291 2023-07-26 23:35:28.000000 quiltcore-0.3.1/quiltcore/__init__.py
--rw-r--r--   0        0        0     1765 2023-07-27 23:33:36.768064 quiltcore-0.3.1/quiltcore/builder.py
--rw-r--r--   0        0        0     1924 2023-07-27 23:33:36.768534 quiltcore-0.3.1/quiltcore/changes.py
--rw-r--r--   0        0        0     2063 2023-07-27 23:33:36.769027 quiltcore-0.3.1/quiltcore/delta.py
--rw-r--r--   0        0        0     2081 2023-07-27 23:33:36.769455 quiltcore-0.3.1/quiltcore/entry.py
--rw-r--r--   0        0        0     1451 2023-07-27 23:33:36.769904 quiltcore-0.3.1/quiltcore/header.py
--rw-r--r--   0        0        0     2863 2023-07-29 05:16:43.683126 quiltcore-0.3.1/quiltcore/manifest.py
--rw-r--r--   0        0        0      800 2023-08-01 16:27:18.649723 quiltcore-0.3.1/quiltcore/namespace.py
--rw-r--r--   0        0        0     1812 2023-07-29 04:11:49.929380 quiltcore-0.3.1/quiltcore/registry.py
--rw-r--r--   0        0        0     4881 2023-07-29 05:23:24.560119 quiltcore-0.3.1/quiltcore/resource.py
--rw-r--r--   0        0        0     3176 2023-07-25 20:35:00.181308 quiltcore-0.3.1/quiltcore/resource_key.py
--rw-r--r--   0        0        0     1609 2023-07-30 04:10:07.329505 quiltcore-0.3.1/quiltcore/resource_path.py
--rw-r--r--   0        0        0     1859 2023-07-27 23:33:36.771096 quiltcore-0.3.1/quiltcore/table.py
--rw-r--r--   0        0        0     6090 2023-08-01 18:44:37.119423 quiltcore-0.3.1/quiltcore/volume.py
--rw-r--r--   0        0        0     8926 2023-07-27 23:33:36.772396 quiltcore-0.3.1/quiltcore/yaml/codec.py
--rw-r--r--   0        0        0      848 2023-07-25 20:35:00.185720 quiltcore-0.3.1/quiltcore/yaml/config.py
--rw-r--r--   0        0        0     1217 2023-07-27 23:33:36.772841 quiltcore-0.3.1/quiltcore/yaml/quiltcore.yaml
--rw-r--r--   0        0        0      833 2023-07-27 22:07:49.354966 quiltcore-0.3.1/quiltcore/yaml/quiltspec.yaml
--rw-r--r--   0        0        0      160 2023-07-20 04:22:58.224611 quiltcore-0.3.1/quiltcore/yaml/schema.yaml
--rw-r--r--   0        0        0     1053 2023-07-20 22:23:12.863928 quiltcore-0.3.1/quiltcore/yaml/spec.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 quiltcore-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-10 04:58:49.699035 quiltcore-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1573 2023-07-20 22:18:01.855543 quiltcore-0.3.2/README.md
+-rw-r--r--   0        0        0     1115 2023-08-03 18:18:17.388152 quiltcore-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1291 2023-07-26 23:35:28.000000 quiltcore-0.3.2/quiltcore/__init__.py
+-rw-r--r--   0        0        0     1765 2023-07-27 23:33:36.768064 quiltcore-0.3.2/quiltcore/builder.py
+-rw-r--r--   0        0        0     1924 2023-07-27 23:33:36.768534 quiltcore-0.3.2/quiltcore/changes.py
+-rw-r--r--   0        0        0     2062 2023-08-03 18:18:17.388962 quiltcore-0.3.2/quiltcore/delta.py
+-rw-r--r--   0        0        0     2081 2023-07-27 23:33:36.769455 quiltcore-0.3.2/quiltcore/entry.py
+-rw-r--r--   0        0        0     1451 2023-07-27 23:33:36.769904 quiltcore-0.3.2/quiltcore/header.py
+-rw-r--r--   0        0        0     2861 2023-08-03 18:18:17.389822 quiltcore-0.3.2/quiltcore/manifest.py
+-rw-r--r--   0        0        0     1009 2023-08-03 18:18:17.390655 quiltcore-0.3.2/quiltcore/namespace.py
+-rw-r--r--   0        0        0     1812 2023-08-01 18:57:11.606738 quiltcore-0.3.2/quiltcore/registry.py
+-rw-r--r--   0        0        0     4881 2023-08-01 18:57:11.607998 quiltcore-0.3.2/quiltcore/resource.py
+-rw-r--r--   0        0        0     3176 2023-07-25 20:35:00.181308 quiltcore-0.3.2/quiltcore/resource_key.py
+-rw-r--r--   0        0        0     1629 2023-08-03 18:18:17.391507 quiltcore-0.3.2/quiltcore/resource_path.py
+-rw-r--r--   0        0        0     1859 2023-07-27 23:33:36.771096 quiltcore-0.3.2/quiltcore/table.py
+-rw-r--r--   0        0        0     6090 2023-08-01 18:57:11.610016 quiltcore-0.3.2/quiltcore/volume.py
+-rw-r--r--   0        0        0     8926 2023-07-27 23:33:36.772396 quiltcore-0.3.2/quiltcore/yaml/codec.py
+-rw-r--r--   0        0        0      869 2023-08-03 18:18:17.392591 quiltcore-0.3.2/quiltcore/yaml/config.py
+-rw-r--r--   0        0        0     1217 2023-07-27 23:33:36.772841 quiltcore-0.3.2/quiltcore/yaml/quiltcore.yaml
+-rw-r--r--   0        0        0      833 2023-07-27 22:07:49.354966 quiltcore-0.3.2/quiltcore/yaml/quiltspec.yaml
+-rw-r--r--   0        0        0      160 2023-07-20 04:22:58.224611 quiltcore-0.3.2/quiltcore/yaml/schema.yaml
+-rw-r--r--   0        0        0     1036 2023-08-03 18:18:17.393423 quiltcore-0.3.2/quiltcore/yaml/spec.py
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 quiltcore-0.3.2/PKG-INFO
```

### Comparing `quiltcore-0.3.1/LICENSE` & `quiltcore-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/README.md` & `quiltcore-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/pyproject.toml` & `quiltcore-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quiltcore"
-version = "0.3.1"
+version = "0.3.2"
 description = "low-level plubming to read/write Quilt packages"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `quiltcore-0.3.1/quiltcore/__init__.py` & `quiltcore-0.3.2/quiltcore/__init__.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/quiltcore/builder.py` & `quiltcore-0.3.2/quiltcore/builder.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/quiltcore/changes.py` & `quiltcore-0.3.2/quiltcore/changes.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/quiltcore/delta.py` & `quiltcore-0.3.2/quiltcore/delta.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,8 +70,7 @@
 
     def to_dict(self) -> dict:
         return {
             self.KEY_ACT: self.action,
             self.cf.K_NAM: self.name,
             self.cf.K_PLC: str(self.path),
         }
-
```

### Comparing `quiltcore-0.3.1/quiltcore/entry.py` & `quiltcore-0.3.2/quiltcore/entry.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/quiltcore/header.py` & `quiltcore-0.3.2/quiltcore/header.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/quiltcore/manifest.py` & `quiltcore-0.3.2/quiltcore/manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,26 +29,26 @@
                 for row in rows:
                     if not isinstance(row, Dict3):
                         raise ValueError("")
                     writer.write(asdict(row))
 
     def __init__(self, path: Path, **kwargs):
         super().__init__(path, **kwargs)
-        self._table: Table|None = None
+        self._table: Table | None = None
 
     def table(self) -> Table:
         if not hasattr(self, "_table") or self._table is None:
             try:
                 self._table = Table(self.path, **self.args)
             except FileNotFoundError:
                 logging.warning(f"Manifest not found: {self.path}")
         if not isinstance(self._table, Table):
             raise TypeError(f"Expected Table, got {type(self._table)}")
         return self._table
-    
+
     def head(self):
         return self.table().head
 
     #
     # Hash functions
     #
```

### Comparing `quiltcore-0.3.1/quiltcore/namespace.py` & `quiltcore-0.3.2/quiltcore/namespace.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,31 @@
 
 
 class Namespace(ResourcePath):
     """
     Namespace of Manifests by Hash
     list/get returns a specific Manifest
     """
+
     SEP = "/"
+    HASH_LEN = 64
 
     def __init__(self, path: Path, **kwargs):
         super().__init__(path, **kwargs)
         self.manifests = kwargs[self.KEY_MAN]
         self.name = self.pkg_name()
 
     def hash(self, tag: str = ResourcePath.TAG_DEFAULT) -> str:
         hash_file = self.path / tag
         return hash_file.read_text()
 
-    def _child_path(self, key: str) -> Path:
+    def _child_path(self, key: str, **kwargs) -> Path:
         """Return the path for a child resource."""
-        # TODO: match on partial hashes
-        hash = self.hash(key)
-        return self.manifests / hash
+        hash = kwargs.get(self.KEY_HSH) or self.hash(key)
+        if len(hash) == self.HASH_LEN:
+            return self.manifests / hash
+        for match in self.manifests.glob(f"{hash}*"):
+            return match
+        raise ValueError(f"hash must be {self.HASH_LEN} chars long")
 
     def pkg_name(self) -> str:
-        return self.SEP.join(self.path.parts[-2:])
+        return self.SEP.join(self.path.parts[-2:])
```

### Comparing `quiltcore-0.3.1/quiltcore/registry.py` & `quiltcore-0.3.2/quiltcore/registry.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/quiltcore/resource.py` & `quiltcore-0.3.2/quiltcore/resource.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/quiltcore/resource_key.py` & `quiltcore-0.3.2/quiltcore/resource_key.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/quiltcore/resource_path.py` & `quiltcore-0.3.2/quiltcore/resource_path.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         """Return a child resource."""
         args = self._child_args(key)
         args[self.KEY_KEY] = key
         merged = {**self.args, **args}
         self.CheckPath(path)
         return self.klass(path, **merged)
 
-    def _child_path(self, key: str) -> Path:
+    def _child_path(self, key: str, **kwargs) -> Path:
         """Return the path for a child resource."""
         return self.path / key
 
     def _child_list(self) -> list[Path]:
         """List/generator of valid child paths; defaults to self.glob"""
         return sorted(self.path.glob(self.glob))
 
@@ -44,13 +44,13 @@
 
     def list(self, **kwargs) -> list["Resource"]:
         """List all child resources."""
         return [self.child(x) for x in self._child_list()]
 
     def get(self, key: str, **kwargs) -> "Resource":
         """Get a child resource by name."""
-        path = self._child_path(key)
+        path = self._child_path(key, **kwargs)
         if not path.exists():
             if not kwargs.get(self.KEY_FRC, False):
                 raise KeyError(f"Key {key} not found in {self.path}")
             path.mkdir(parents=True)
         return self.child(path, key)
```

### Comparing `quiltcore-0.3.1/quiltcore/table.py` & `quiltcore-0.3.2/quiltcore/table.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/quiltcore/volume.py` & `quiltcore-0.3.2/quiltcore/volume.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/quiltcore/yaml/codec.py` & `quiltcore-0.3.2/quiltcore/yaml/codec.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/quiltcore/yaml/config.py` & `quiltcore-0.3.2/quiltcore/yaml/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from un_yaml import UnYaml  # type: ignore
 from upath import UPath
 
 
 class Config(UnYaml):
     CONFIG_FILE = "quiltcore.yaml"
+    K_CFG = "config"
+    K_HSH = "hash"
     K_MAP = "map"
     K_NAM = "name"
     K_PLC = "place"
-    K_HSH = "hash"
 
     @classmethod
     def DefaultConfig(cls) -> dict:
         return UnYaml.LoadYaml(cls.CONFIG_FILE, __package__)
 
     def __init__(self, yaml_data: dict = {}) -> None:
         data = yaml_data if len(yaml_data) > 0 else self.DefaultConfig()
```

### Comparing `quiltcore-0.3.1/quiltcore/yaml/quiltcore.yaml` & `quiltcore-0.3.2/quiltcore/yaml/quiltcore.yaml`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/quiltcore/yaml/quiltspec.yaml` & `quiltcore-0.3.2/quiltcore/yaml/quiltspec.yaml`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.1/quiltcore/yaml/spec.py` & `quiltcore-0.3.2/quiltcore/yaml/spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from .config import Config
 
 
 class Spec(Config):
     """Manage quiltspec parameters"""
 
     CONFIG_FILE = "quiltspec.yaml"
-    K_PKG = "config"
 
     def __init__(self, name=None, update=None) -> None:
         super().__init__()
         self.name = name
         self.update = update
 
     def pkg(self, key: str) -> str:
-        _pkg = self.get_dict(self.K_PKG)
+        _pkg = self.get_dict(self.K_CFG)
         return _pkg.get(key, "<missing>")
 
     # Configuration
 
     def registry(self) -> str:
         return self.pkg("registry")
 
     def namespace(self) -> str:
         return self.name or self.pkg("namespace")
 
     def hash(self) -> str:
-        return self.pkg("hash")
+        return self.pkg(self.K_HSH)
 
     def tag(self) -> str:
         return str(self.pkg("tag"))
 
     # Contents
 
     def files(self) -> dict:
```

### Comparing `quiltcore-0.3.1/PKG-INFO` & `quiltcore-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quiltcore
-Version: 0.3.1
+Version: 0.3.2
 Summary: low-level plubming to read/write Quilt packages
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

