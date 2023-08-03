# Comparing `tmp/beiboot-1.4.2.tar.gz` & `tmp/beiboot-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beiboot-1.4.2.tar", max compression
+gzip compressed data, was "beiboot-1.4.3.tar", max compression
```

## Comparing `beiboot-1.4.2.tar` & `beiboot-1.4.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      699 2023-08-01 11:56:43.169515 beiboot-1.4.2/README.md
--rw-r--r--   0        0        0        0 2023-08-01 11:56:43.169515 beiboot-1.4.2/beiboot/__init__.py
--rw-r--r--   0        0        0      322 2023-08-01 11:56:43.169515 beiboot-1.4.2/beiboot/api/__init__.py
--rw-r--r--   0        0        0     2313 2023-08-01 11:56:43.169515 beiboot-1.4.2/beiboot/api/connect.py
--rw-r--r--   0        0        0     2199 2023-08-01 11:56:43.169515 beiboot-1.4.2/beiboot/api/create.py
--rw-r--r--   0        0        0     2256 2023-08-01 11:56:43.169515 beiboot-1.4.2/beiboot/api/create_shelf.py
--rw-r--r--   0        0        0     1558 2023-08-01 11:56:43.169515 beiboot-1.4.2/beiboot/api/delete.py
--rw-r--r--   0        0        0     1535 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/api/delete_shelf.py
--rw-r--r--   0        0        0     1977 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/api/heartbeat.py
--rw-r--r--   0        0        0     1335 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/api/list.py
--rw-r--r--   0        0        0     1335 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/api/list_shelves.py
--rw-r--r--   0        0        0      993 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/api/read.py
--rw-r--r--   0        0        0      995 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/api/read_shelf.py
--rw-r--r--   0        0        0      390 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/api/utils.py
--rw-r--r--   0        0        0     3441 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/configuration.py
--rw-r--r--   0        0        0        0 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/connection/__init__.py
--rw-r--r--   0        0        0     4217 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/connection/abstract.py
--rw-r--r--   0        0        0     1914 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/connection/dummy/__init__.py
--rw-r--r--   0        0        0     1285 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/connection/factory.py
--rw-r--r--   0        0        0       52 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/connection/ghostunnel/__init__.py
--rw-r--r--   0        0        0     5854 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/connection/ghostunnel/docker.py
--rw-r--r--   0        0        0       65 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/connection/ghostunnel/native.py
--rw-r--r--   0        0        0      137 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/connection/types.py
--rw-r--r--   0        0        0      555 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/connection/utils.py
--rw-r--r--   0        0        0        0 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/misc/__init__.py
--rw-r--r--   0        0        0      218 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/misc/comps/__init__.py
--rw-r--r--   0        0        0     1689 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/misc/comps/configmap.py
--rw-r--r--   0        0        0     1179 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/misc/comps/deployment.py
--rw-r--r--   0        0        0      262 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/misc/comps/namespace.py
--rw-r--r--   0        0        0     3582 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/misc/comps/rbac.py
--rw-r--r--   0        0        0     8194 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/misc/comps/webhook.py
--rw-r--r--   0        0        0     1626 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/misc/install.py
--rw-r--r--   0        0        0     3856 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/misc/uninstall.py
--rw-r--r--   0        0        0      481 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/misc/utils.py
--rw-r--r--   0        0        0    17952 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/types.py
--rw-r--r--   0        0        0     4665 2023-08-01 11:56:43.173514 beiboot-1.4.2/beiboot/utils.py
--rw-r--r--   0        0        0     1750 2023-08-01 11:56:43.173514 beiboot-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 beiboot-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0      699 2023-08-03 07:56:24.326473 beiboot-1.4.3/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 07:56:24.326473 beiboot-1.4.3/beiboot/__init__.py
+-rw-r--r--   0        0        0      322 2023-08-03 07:56:24.326473 beiboot-1.4.3/beiboot/api/__init__.py
+-rw-r--r--   0        0        0     2313 2023-08-03 07:56:24.326473 beiboot-1.4.3/beiboot/api/connect.py
+-rw-r--r--   0        0        0     2199 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/api/create.py
+-rw-r--r--   0        0        0     2256 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/api/create_shelf.py
+-rw-r--r--   0        0        0     1558 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/api/delete.py
+-rw-r--r--   0        0        0     1535 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/api/delete_shelf.py
+-rw-r--r--   0        0        0     1977 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/api/heartbeat.py
+-rw-r--r--   0        0        0     1335 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/api/list.py
+-rw-r--r--   0        0        0     1335 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/api/list_shelves.py
+-rw-r--r--   0        0        0      993 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/api/read.py
+-rw-r--r--   0        0        0      995 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/api/read_shelf.py
+-rw-r--r--   0        0        0      390 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/api/utils.py
+-rw-r--r--   0        0        0     3441 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/configuration.py
+-rw-r--r--   0        0        0        0 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/connection/__init__.py
+-rw-r--r--   0        0        0     4217 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/connection/abstract.py
+-rw-r--r--   0        0        0     1914 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/connection/dummy/__init__.py
+-rw-r--r--   0        0        0     1285 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/connection/factory.py
+-rw-r--r--   0        0        0       52 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/connection/ghostunnel/__init__.py
+-rw-r--r--   0        0        0     5854 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/connection/ghostunnel/docker.py
+-rw-r--r--   0        0        0       65 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/connection/ghostunnel/native.py
+-rw-r--r--   0        0        0      137 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/connection/types.py
+-rw-r--r--   0        0        0      555 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/connection/utils.py
+-rw-r--r--   0        0        0        0 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/misc/__init__.py
+-rw-r--r--   0        0        0      218 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/misc/comps/__init__.py
+-rw-r--r--   0        0        0     1689 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/misc/comps/configmap.py
+-rw-r--r--   0        0        0     1179 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/misc/comps/deployment.py
+-rw-r--r--   0        0        0      262 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/misc/comps/namespace.py
+-rw-r--r--   0        0        0     3582 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/misc/comps/rbac.py
+-rw-r--r--   0        0        0     8194 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/misc/comps/webhook.py
+-rw-r--r--   0        0        0     1626 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/misc/install.py
+-rw-r--r--   0        0        0     3856 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/misc/uninstall.py
+-rw-r--r--   0        0        0      481 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/misc/utils.py
+-rw-r--r--   0        0        0    17952 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/types.py
+-rw-r--r--   0        0        0     4665 2023-08-03 07:56:24.330473 beiboot-1.4.3/beiboot/utils.py
+-rw-r--r--   0        0        0     1750 2023-08-03 07:56:24.330473 beiboot-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 beiboot-1.4.3/PKG-INFO
```

### Comparing `beiboot-1.4.2/README.md` & `beiboot-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/api/connect.py` & `beiboot-1.4.3/beiboot/api/connect.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/api/create.py` & `beiboot-1.4.3/beiboot/api/create.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/api/create_shelf.py` & `beiboot-1.4.3/beiboot/api/create_shelf.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/api/delete.py` & `beiboot-1.4.3/beiboot/api/delete.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/api/delete_shelf.py` & `beiboot-1.4.3/beiboot/api/delete_shelf.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/api/heartbeat.py` & `beiboot-1.4.3/beiboot/api/heartbeat.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/api/list.py` & `beiboot-1.4.3/beiboot/api/list.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/api/list_shelves.py` & `beiboot-1.4.3/beiboot/api/list_shelves.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/api/read.py` & `beiboot-1.4.3/beiboot/api/read.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/api/read_shelf.py` & `beiboot-1.4.3/beiboot/api/read_shelf.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/configuration.py` & `beiboot-1.4.3/beiboot/configuration.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/connection/abstract.py` & `beiboot-1.4.3/beiboot/connection/abstract.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/connection/dummy/__init__.py` & `beiboot-1.4.3/beiboot/connection/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/connection/factory.py` & `beiboot-1.4.3/beiboot/connection/factory.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/connection/ghostunnel/docker.py` & `beiboot-1.4.3/beiboot/connection/ghostunnel/docker.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/connection/utils.py` & `beiboot-1.4.3/beiboot/connection/utils.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/misc/comps/configmap.py` & `beiboot-1.4.3/beiboot/misc/comps/configmap.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/misc/comps/deployment.py` & `beiboot-1.4.3/beiboot/misc/comps/deployment.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/misc/comps/rbac.py` & `beiboot-1.4.3/beiboot/misc/comps/rbac.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/misc/comps/webhook.py` & `beiboot-1.4.3/beiboot/misc/comps/webhook.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/misc/install.py` & `beiboot-1.4.3/beiboot/misc/install.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/misc/uninstall.py` & `beiboot-1.4.3/beiboot/misc/uninstall.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/types.py` & `beiboot-1.4.3/beiboot/types.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/beiboot/utils.py` & `beiboot-1.4.3/beiboot/utils.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.4.2/pyproject.toml` & `beiboot-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beiboot"
-version = "1.4.2"
+version = "1.4.3"
 description = "Getdeck Beiboot client project."
 authors = ["Michael Schilonka <michael@blueshoe.de>"]
 readme = "README.md"
 homepage = "https://getdeck.dev"
 repository = "https://github.com/Getdeck/beiboot"
 documentation = "https://getdeck.dev"
 keywords = [
```

### Comparing `beiboot-1.4.2/PKG-INFO` & `beiboot-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beiboot
-Version: 1.4.2
+Version: 1.4.3
 Summary: Getdeck Beiboot client project.
 Home-page: https://getdeck.dev
 Keywords: Kubernetes,Development,Cloud-native
 Author: Michael Schilonka
 Author-email: michael@blueshoe.de
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

