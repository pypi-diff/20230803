# Comparing `tmp/izaber-3.0.20230207.tar.gz` & `tmp/izaber-3.1.20230803.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izaber-3.0.20230207.tar", max compression
+gzip compressed data, was "izaber-3.1.20230803.tar", max compression
```

## Comparing `izaber-3.0.20230207.tar` & `izaber-3.1.20230803.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4567 2022-11-24 23:22:14.973857 izaber-3.0.20230207/izaber/__init__.py
--rw-r--r--   0        0        0      381 2021-01-11 13:26:26.391740 izaber-3.0.20230207/izaber/compat.py
--rw-r--r--   0        0        0    16299 2021-01-11 13:26:26.391740 izaber-3.0.20230207/izaber/date.py
--rw-r--r--   0        0        0     5043 2021-01-25 00:05:00.000832 izaber-3.0.20230207/izaber/email.py
--rw-r--r--   0        0        0     1228 2021-01-11 13:26:26.391740 izaber-3.0.20230207/izaber/log.py
--rw-r--r--   0        0        0     9629 2021-01-11 13:26:26.391740 izaber-3.0.20230207/izaber/paths.py
--rw-r--r--   0        0        0     1441 2022-10-21 13:42:07.443233 izaber-3.0.20230207/izaber/startup.py
--rw-r--r--   0        0        0     1200 2021-01-11 13:26:26.395740 izaber-3.0.20230207/izaber/structs.py
--rw-r--r--   0        0        0     1197 2021-01-11 13:26:26.395740 izaber-3.0.20230207/izaber/templates.py
--rw-r--r--   0        0        0    15025 2023-02-07 21:52:02.511971 izaber-3.0.20230207/izaber/zconfig.py
--rw-r--r--   0        0        0    14919 2021-01-11 13:26:26.395740 izaber-3.0.20230207/izaber/zdatetime.py
--rw-r--r--   0        0        0      838 2023-02-07 22:06:38.255533 izaber-3.0.20230207/pyproject.toml
--rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 izaber-3.0.20230207/setup.py
--rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 izaber-3.0.20230207/PKG-INFO
+-rw-r--r--   0        0        0     5988 2023-08-03 21:23:40.190470 izaber-3.1.20230803/izaber/__init__.py
+-rw-r--r--   0        0        0      381 2021-01-11 13:26:26.391740 izaber-3.1.20230803/izaber/compat.py
+-rw-r--r--   0        0        0    16299 2021-01-11 13:26:26.391740 izaber-3.1.20230803/izaber/date.py
+-rw-r--r--   0        0        0     5022 2023-08-03 21:23:40.190470 izaber-3.1.20230803/izaber/email.py
+-rw-r--r--   0        0        0     1904 2023-08-03 21:23:40.190470 izaber-3.1.20230803/izaber/log.py
+-rw-r--r--   0        0        0     9629 2021-01-11 13:26:26.391740 izaber-3.1.20230803/izaber/paths.py
+-rw-r--r--   0        0        0     2132 2023-08-03 21:23:40.190470 izaber-3.1.20230803/izaber/startup.py
+-rw-r--r--   0        0        0     1200 2021-01-11 13:26:26.395740 izaber-3.1.20230803/izaber/structs.py
+-rw-r--r--   0        0        0     1197 2021-01-11 13:26:26.395740 izaber-3.1.20230803/izaber/templates.py
+-rw-r--r--   0        0        0    15025 2023-08-03 21:23:40.190470 izaber-3.1.20230803/izaber/zconfig.py
+-rw-r--r--   0        0        0    14919 2021-01-11 13:26:26.395740 izaber-3.1.20230803/izaber/zdatetime.py
+-rw-r--r--   0        0        0     1014 2023-08-03 21:23:40.190470 izaber-3.1.20230803/pyproject.toml
+-rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 izaber-3.1.20230803/setup.py
+-rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 izaber-3.1.20230803/PKG-INFO
```

### Comparing `izaber-3.0.20230207/izaber/__init__.py` & `izaber-3.1.20230803/izaber/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import sys
 import re
-import pkg_resources
-
-__version__ = pkg_resources.get_distribution("izaber").version
-
 import importlib
 
+try:
+    from importlib.metadata import version
+    __version__ = version("izaber")
+# For older versions of python
+except:
+    import pkg_resources
+    __version__ = pkg_resources.get_distribution("izaber").version
+
 # Check to see the library has the submodule we need
 class IZaberLoaderImportlib(object):
 
     def __init__(self,spec,module_name,*args,**kwargs):
         self.spec = spec
         self.module_name = module_name
         self.args = args
@@ -33,14 +37,23 @@
                 module = importlib.util.module_from_spec(self.spec)
                 sys.modules[self.module_name] = module
                 sys.modules[module_name] = module
                 sys.modules[self.spec.name] = module
                 self.spec.loader.exec_module(module)
         return module
 
+class IZaberSpec:
+    def __init__(self, spec, module_name):
+        self.spec = spec
+        self.module_name = module_name
+        self.loader = IZaberLoaderImportlib(spec, module_name)
+
+    def __getattr__(self, k):
+        return getattr(self.spec, k)
+
 from importlib import abc as il_abc
 class IZaberFinderImportlib(il_abc.MetaPathFinder):
     """ Attempts to finds the module that may be tucked into
         a submodule.
     """
 
     def __init__(self,prefixes=None):
@@ -78,14 +91,46 @@
                     raise ModuleNotFoundError(f"No module named {module_name}")
                 package_path.append(e)
 
             return IZaberLoaderImportlib(spec,module_name)
         except ImportError:
             return
 
+    def find_spec(self, module_name, path=None, target=None):
+
+        for prefix in self.prefixes:
+            try:
+                if module_name.index(prefix) != 0:
+                    continue
+            except ValueError:
+                continue
+
+            try:
+                target_module = re.sub(
+                              '^'+prefix,
+                              prefix.replace('.','_'),
+                              module_name,
+                          )
+
+                found = None
+                spec = None
+                package_path = []
+                for e in target_module.split('.'):
+                    package = "_".join(package_path) or None
+                    spec = importlib.util.find_spec(e,package)
+                    if not spec:
+                        raise ModuleNotFoundError(f"No module named {module_name}")
+                    package_path.append(e)
+
+                return IZaberSpec(spec,module_name)
+            except ImportError:
+                return
+
+        return
+
     def find_module(self, module_name, package_path=None):
         # Only respond to izaber.* modules
         try:
             if module_name.index('izaber.') != 0:
                 return
         except:
             return
@@ -132,10 +177,10 @@
 For another example have a look at izaber.wamp (which allows the
 load of izaber.wamp.fuse)
 
 """
 
 
 autoloader = IZaberFinderImportlib()
-sys.meta_path.append(autoloader)
+sys.meta_path.insert(0, autoloader)
```

### Comparing `izaber-3.0.20230207/izaber/date.py` & `izaber-3.1.20230803/izaber/date.py`

 * *Files identical despite different names*

### Comparing `izaber-3.0.20230207/izaber/email.py` & `izaber-3.1.20230803/izaber/email.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import absolute_import
 
 import os.path
 import smtplib
 import logging
-import pkg_resources
 
 from email.parser import Parser
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.mime.application import MIMEApplication
 from email.mime.base import MIMEBase
 from email import encoders
```

### Comparing `izaber-3.0.20230207/izaber/log.py` & `izaber-3.1.20230803/izaber/log.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
+import sys
 
 from izaber.startup import initializer, request_initialize
 from izaber.zconfig import config
 
 class Logger(object):
-
     _logger = None
 
     def __call__(self,*args,**kwargs):
         self.info(*args,**kwargs)
 
     def __getattr__(self,k):
         if not self._logger:
@@ -20,16 +20,34 @@
 
 @initializer('logging')
 def initialize(**kwargs):
     request_initialize('config',**kwargs)
     logging_config = config.get('logging',{})
     logging_config.update( kwargs.get('logging',{}) )
 
-    # Find the best place to put the log
+    # We only activate logging if the logging section has
+    # configuration. This allows users to configure their
+    # own logger as desired
+    if not logging_config:
+        return
+
+    # We also allow the disabling of the internally made logging module
+    # by adding the logging.disable_internal key
+    if logging_config.get('disable_internal'):
+        return
+
+    # So we have some logging configuration, let's let izaber setup a logging
+    # handler.
+
+    # If there's no filename, let's default to stream output for logging
     if 'filename' not in logging_config:
+        logging_config.setdefault('stream', sys.stdout)
+
+    # so there's a filename but it's blank, let's default to something
+    elif not logging_config['filename']:
         for log_location in ['/tmp','/temp','.']:
             if not os.path.isdir(log_location):
                 continue
             logging_config.setdefault('filename',os.path.join(log_location,'log.log'))
             break
     logging_config.setdefault('filemode','a')
     logging_config.setdefault(
```

### Comparing `izaber-3.0.20230207/izaber/paths.py` & `izaber-3.1.20230803/izaber/paths.py`

 * *Files identical despite different names*

### Comparing `izaber-3.0.20230207/izaber/structs.py` & `izaber-3.1.20230803/izaber/structs.py`

 * *Files identical despite different names*

### Comparing `izaber-3.0.20230207/izaber/templates.py` & `izaber-3.1.20230803/izaber/templates.py`

 * *Files identical despite different names*

### Comparing `izaber-3.0.20230207/izaber/zconfig.py` & `izaber-3.1.20230803/izaber/zconfig.py`

 * *Files identical despite different names*

### Comparing `izaber-3.0.20230207/izaber/zdatetime.py` & `izaber-3.1.20230803/izaber/zdatetime.py`

 * *Files identical despite different names*

### Comparing `izaber-3.0.20230207/setup.py` & `izaber-3.1.20230803/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 ['izaber']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Jinja2>=2.11.3',
- 'PyYAML>=5.3',
+ 'PyYAML>=5.3.0,!=5.4.1,!=6.0',
  'appdirs>=1.4.4',
  'docopt>=0.6.2',
+ 'pytest-xdist==2.5.0',
  'python-dateutil>=2.8.1',
  'pytz>=2021.1',
  'six>=1.15.0']
 
 extras_require = \
 {'email': ['beautifulsoup4>=4.9.3', 'lxml>=4.6.2']}
 
 setup_kwargs = {
     'name': 'izaber',
-    'version': '3.0.20230207',
+    'version': '3.1.20230803',
     'description': 'Base load point for iZaber code',
     'long_description': 'None',
     'author': 'Aki Mimoto',
     'author_email': 'aki@zaber.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `izaber-3.0.20230207/PKG-INFO` & `izaber-3.1.20230803/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: izaber
-Version: 3.0.20230207
+Version: 3.1.20230803
 Summary: Base load point for iZaber code
 Author: Aki Mimoto
 Author-email: aki@zaber.com
 Requires-Python: >=3.6.0,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: email
 Requires-Dist: Jinja2 (>=2.11.3)
-Requires-Dist: PyYAML (>=5.3)
+Requires-Dist: PyYAML (>=5.3.0,!=5.4.1,!=6.0)
 Requires-Dist: appdirs (>=1.4.4)
 Requires-Dist: beautifulsoup4 (>=4.9.3) ; extra == "email"
 Requires-Dist: docopt (>=0.6.2)
 Requires-Dist: lxml (>=4.6.2) ; extra == "email"
+Requires-Dist: pytest-xdist (==2.5.0)
 Requires-Dist: python-dateutil (>=2.8.1)
 Requires-Dist: pytz (>=2021.1)
 Requires-Dist: six (>=1.15.0)
```

