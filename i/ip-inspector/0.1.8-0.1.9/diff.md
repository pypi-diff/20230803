# Comparing `tmp/ip_inspector-0.1.8.tar.gz` & `tmp/ip_inspector-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ip_inspector-0.1.8.tar", max compression
+gzip compressed data, was "ip_inspector-0.1.9.tar", max compression
```

## Comparing `ip_inspector-0.1.8.tar` & `ip_inspector-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     5890 2021-07-01 23:18:11.594482 ip_inspector-0.1.8/README.md
--rw-r--r--   0        0        0       60 2021-07-04 22:41:20.840579 ip_inspector-0.1.8/ip_inspector/__init__.py
--rw-r--r--   0        0        0    15976 2021-07-04 22:40:20.920732 ip_inspector-0.1.8/ip_inspector/cli.py
--rw-r--r--   0        0        0     5458 2021-06-30 21:18:20.131673 ip_inspector-0.1.8/ip_inspector/config.py
--rw-r--r--   0        0        0    18349 2021-07-03 18:40:27.035512 ip_inspector-0.1.8/ip_inspector/database.py
--rw-r--r--   0        0        0     3011 2021-06-30 21:18:20.131673 ip_inspector-0.1.8/ip_inspector/etc/default.config.yaml
--rw-r--r--   0        0        0    15598 2021-07-03 20:11:04.349701 ip_inspector-0.1.8/ip_inspector/inspector.py
--rw-r--r--   0        0        0    12487 2021-07-03 20:09:13.865960 ip_inspector-0.1.8/ip_inspector/maxmind.py
--rw-r--r--   0        0        0     4092 2021-06-30 21:18:20.131673 ip_inspector-0.1.8/ip_inspector/tor.py
--rw-r--r--   0        0        0      838 2021-07-04 22:41:30.940553 ip_inspector-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1059 2021-07-04 22:42:37.577482 ip_inspector-0.1.8/setup.py
--rw-r--r--   0        0        0      878 2021-07-04 22:42:37.577849 ip_inspector-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     5890 2021-07-01 23:18:11.594482 ip_inspector-0.1.9/README.md
+-rw-r--r--   0        0        0       60 2021-07-05 14:57:21.106146 ip_inspector-0.1.9/ip_inspector/__init__.py
+-rw-r--r--   0        0        0    15977 2021-07-05 14:47:59.127547 ip_inspector-0.1.9/ip_inspector/cli.py
+-rw-r--r--   0        0        0     5458 2021-06-30 21:18:20.131673 ip_inspector-0.1.9/ip_inspector/config.py
+-rw-r--r--   0        0        0    18349 2021-07-03 18:40:27.035512 ip_inspector-0.1.9/ip_inspector/database.py
+-rw-r--r--   0        0        0     3011 2021-06-30 21:18:20.131673 ip_inspector-0.1.9/ip_inspector/etc/default.config.yaml
+-rw-r--r--   0        0        0    15598 2021-07-03 20:11:04.349701 ip_inspector-0.1.9/ip_inspector/inspector.py
+-rw-r--r--   0        0        0    12487 2021-07-03 20:09:13.865960 ip_inspector-0.1.9/ip_inspector/maxmind.py
+-rw-r--r--   0        0        0     4092 2021-06-30 21:18:20.131673 ip_inspector-0.1.9/ip_inspector/tor.py
+-rw-r--r--   0        0        0      839 2021-07-05 14:57:19.314150 ip_inspector-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1059 2021-07-05 15:00:25.041524 ip_inspector-0.1.9/setup.py
+-rw-r--r--   0        0        0      878 2021-07-05 15:00:25.041904 ip_inspector-0.1.9/PKG-INFO
```

### Comparing `ip_inspector-0.1.8/README.md` & `ip_inspector-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ip_inspector-0.1.8/ip_inspector/cli.py` & `ip_inspector-0.1.9/ip_inspector/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,33 +165,17 @@
         choices=CONFIG["default"]["blacklists"],
         help="The type of metadata from this IP result that should be removed from the respective blacklist. Can specify multiple times.",
     )
     bl_remove_parser.add_argument(
         "-r", "--reference", action="store", default=None, help="Remove entries with this reference."
     )
 
-    argcomplete.autocomplete(parser)
-    return parser
-
-
-def main(args=None, parser: argparse.ArgumentParser=None):
-    """The main CLI entry point."""
-
-    # configure logging
-    logging.basicConfig(level=logging.INFO, format="%(asctime)s - %(name)s - [%(levelname)s] %(message)s")
-    coloredlogs.install(level="INFO", logger=LOGGER)
-
-    if not args:
-        args = sys.argv[1:]
 
-    if parser is None:
-        parser = argparse.ArgumentParser(description="Inspect IP address metadata for IDR purposes")
-
-    parser = build_parser(parser)
-    args = parser.parse_args(args)
+def execute(args: argparse.Namespace):
+    """Execute arguments."""
 
     infrastructure_context_map = {}
     default_context_name = CONFIG["default"].get("tracking_context", DEFAULT_INFRASTRUCTURE_CONTEXT_NAME)
     with get_db_session() as session:
         infrastructure_context_map = get_infrastructure_context_map(session)
 
     if args.debug:
@@ -393,7 +377,25 @@
                     print(iip.get(field))
             else:
                 print(iip)
             return True
         return False
 
     return
+
+
+def main(args=None):
+    """The main CLI entry point."""
+
+    # configure logging
+    logging.basicConfig(level=logging.INFO, format="%(asctime)s - %(name)s - [%(levelname)s] %(message)s")
+    coloredlogs.install(level="INFO", logger=LOGGER)
+
+    if not args:
+        args = sys.argv[1:]
+
+    parser = argparse.ArgumentParser(description="Inspect IP address metadata for IDR purposes")
+    build_parser(parser)
+    argcomplete.autocomplete(parser)
+    args = parser.parse_args(args)
+
+    return execute(args)
```

### Comparing `ip_inspector-0.1.8/ip_inspector/config.py` & `ip_inspector-0.1.9/ip_inspector/config.py`

 * *Files identical despite different names*

### Comparing `ip_inspector-0.1.8/ip_inspector/database.py` & `ip_inspector-0.1.9/ip_inspector/database.py`

 * *Files identical despite different names*

### Comparing `ip_inspector-0.1.8/ip_inspector/etc/default.config.yaml` & `ip_inspector-0.1.9/ip_inspector/etc/default.config.yaml`

 * *Files identical despite different names*

### Comparing `ip_inspector-0.1.8/ip_inspector/inspector.py` & `ip_inspector-0.1.9/ip_inspector/inspector.py`

 * *Files identical despite different names*

### Comparing `ip_inspector-0.1.8/ip_inspector/maxmind.py` & `ip_inspector-0.1.9/ip_inspector/maxmind.py`

 * *Files identical despite different names*

### Comparing `ip_inspector-0.1.8/ip_inspector/tor.py` & `ip_inspector-0.1.9/ip_inspector/tor.py`

 * *Files identical despite different names*

### Comparing `ip_inspector-0.1.8/pyproject.toml` & `ip_inspector-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ip_inspector"
-version = "0.1.8"
+version = "0.1.9"
 license = "Apache-2.0"
 homepage = "https://github.com/seanmcfeely/ip-inspector"
 description = "IP inspector is an IPv4 and IPv6 address metadata enricher and tracking tool. Use it on the command line and leverage it as a library."
 authors = ["Sean McFeely <mcfeelynaes@gmail.com>"]
 include = ["README.md"]
 
 [tool.poetry.dependencies]
@@ -27,7 +27,8 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 
 [tool.poetry.scripts]
 ip-inspector = "ip_inspector.cli:main"
+
```

### Comparing `ip_inspector-0.1.8/setup.py` & `ip_inspector-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'requests>=2.25.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['ip-inspector = ip_inspector.cli:main']}
 
 setup_kwargs = {
     'name': 'ip-inspector',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'IP inspector is an IPv4 and IPv6 address metadata enricher and tracking tool. Use it on the command line and leverage it as a library.',
     'long_description': None,
     'author': 'Sean McFeely',
     'author_email': 'mcfeelynaes@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/seanmcfeely/ip-inspector',
```

### Comparing `ip_inspector-0.1.8/PKG-INFO` & `ip_inspector-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ip-inspector
-Version: 0.1.8
+Version: 0.1.9
 Summary: IP inspector is an IPv4 and IPv6 address metadata enricher and tracking tool. Use it on the command line and leverage it as a library.
 Home-page: https://github.com/seanmcfeely/ip-inspector
 License: Apache-2.0
 Author: Sean McFeely
 Author-email: mcfeelynaes@gmail.com
 Requires-Python: >=3.6.2,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

