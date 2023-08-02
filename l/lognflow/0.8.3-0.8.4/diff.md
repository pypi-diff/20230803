# Comparing `tmp/lognflow-0.8.3.tar.gz` & `tmp/lognflow-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.8.3.tar", last modified: Wed Aug  2 11:53:47 2023, max compression
+gzip compressed data, was "lognflow-0.8.4.tar", last modified: Wed Aug  2 23:05:52 2023, max compression
```

## Comparing `lognflow-0.8.3.tar` & `lognflow-0.8.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:53:47.523294 lognflow-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 11:53:32.000000 lognflow-0.8.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-02 11:53:32.000000 lognflow-0.8.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-08-02 11:53:32.000000 lognflow-0.8.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-02 11:53:32.000000 lognflow-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-02 11:53:32.000000 lognflow-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-08-02 11:53:47.523294 lognflow-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-02 11:53:32.000000 lognflow-0.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:53:47.519294 lognflow-0.8.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:53:47.519294 lognflow-0.8.3/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-02 11:53:32.000000 lognflow-0.8.3/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62863 2023-08-02 11:53:32.000000 lognflow-0.8.3/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-08-02 11:53:32.000000 lognflow-0.8.3/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-08-02 11:53:32.000000 lognflow-0.8.3/lognflow/printprogress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-02 11:53:32.000000 lognflow-0.8.3/lognflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:53:47.519294 lognflow-0.8.3/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-08-02 11:53:47.000000 lognflow-0.8.3/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-02 11:53:47.000000 lognflow-0.8.3/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:53:47.000000 lognflow-0.8.3/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:53:47.000000 lognflow-0.8.3/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 11:53:47.000000 lognflow-0.8.3/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 11:53:47.000000 lognflow-0.8.3/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 11:53:47.523294 lognflow-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-02 11:53:32.000000 lognflow-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:53:47.523294 lognflow-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 11:53:32.000000 lognflow-0.8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-08-02 11:53:32.000000 lognflow-0.8.3/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-08-02 11:53:32.000000 lognflow-0.8.3/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-02 11:53:32.000000 lognflow-0.8.3/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:05:52.218510 lognflow-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 23:05:41.000000 lognflow-0.8.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-02 23:05:41.000000 lognflow-0.8.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-08-02 23:05:41.000000 lognflow-0.8.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-02 23:05:41.000000 lognflow-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-02 23:05:41.000000 lognflow-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-08-02 23:05:52.218510 lognflow-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-02 23:05:41.000000 lognflow-0.8.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:05:52.214510 lognflow-0.8.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:05:52.218510 lognflow-0.8.4/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-02 23:05:41.000000 lognflow-0.8.4/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64809 2023-08-02 23:05:41.000000 lognflow-0.8.4/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-08-02 23:05:41.000000 lognflow-0.8.4/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-08-02 23:05:41.000000 lognflow-0.8.4/lognflow/printprogress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-02 23:05:41.000000 lognflow-0.8.4/lognflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:05:52.218510 lognflow-0.8.4/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-08-02 23:05:52.000000 lognflow-0.8.4/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-02 23:05:52.000000 lognflow-0.8.4/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:05:52.000000 lognflow-0.8.4/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:05:52.000000 lognflow-0.8.4/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 23:05:52.000000 lognflow-0.8.4/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 23:05:52.000000 lognflow-0.8.4/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 23:05:52.218510 lognflow-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-02 23:05:41.000000 lognflow-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:05:52.218510 lognflow-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 23:05:41.000000 lognflow-0.8.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-08-02 23:05:41.000000 lognflow-0.8.4/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-08-02 23:05:41.000000 lognflow-0.8.4/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-02 23:05:41.000000 lognflow-0.8.4/tests/test_printprogress.py
```

### Comparing `lognflow-0.8.3/CONTRIBUTING.rst` & `lognflow-0.8.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.3/HISTORY.rst` & `lognflow-0.8.4/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -131,8 +131,14 @@
 0.8.2 (2023-08-02)
 ------------------
 * the word save_as is now replaced with suffix as is in pathlib
 * all loggers can take the suffix as the extension in the parameter_name
 
 0.8.3 (2023-08-02)
 -----------------
-* critical bug fixed in log_var to support v0.8.2
+* critical bug fixed in log_var to support v0.8.2
+
+0.8.4 (2023-08-03)
+-----------------
+* variable names that are pecular will always be fixed first.
+* suffix can be read form the file name.
+* time_tag will always accompany file name unless stated otherwised.
```

### Comparing `lognflow-0.8.3/LICENSE` & `lognflow-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.3/PKG-INFO` & `lognflow-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.8.3
+Version: 0.8.4
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -225,7 +225,13 @@
 ------------------
 * the word save_as is now replaced with suffix as is in pathlib
 * all loggers can take the suffix as the extension in the parameter_name
 
 0.8.3 (2023-08-02)
 -----------------
 * critical bug fixed in log_var to support v0.8.2
+
+0.8.4 (2023-08-03)
+-----------------
+* variable names that are pecular will always be fixed first.
+* suffix can be read form the file name.
+* time_tag will always accompany file name unless stated otherwised.
```

### Comparing `lognflow-0.8.3/README.rst` & `lognflow-0.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.3/docs/Makefile` & `lognflow-0.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.3/docs/conf.py` & `lognflow-0.8.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.3/docs/installation.rst` & `lognflow-0.8.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.3/docs/make.bat` & `lognflow-0.8.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.3/lognflow/lognflow.py` & `lognflow-0.8.4/lognflow/lognflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -263,26 +263,36 @@
             + 'Perhaps you forgot to pass the name of the variable first.'
         parameter_name = ''.join(
             [_ for _ in repr(repr_raw(parameter_name))  if _ != '\''])
         parameter_name = replace_all(parameter_name, ' ', '_')
         parameter_name = replace_all(parameter_name, '\\', '/')
         parameter_name = replace_all(parameter_name, '//', '/')
         
-        param_dir = self.log_dir /  parameter_name
+        # param_dir = self.log_dir /  parameter_name
         
         if(parameter_name[-1] == '/'):
             param_name = ''
+            param_dir = parameter_name
         else:
-            param_name = param_dir.name
-            param_dir = param_dir.parent
+            parameter_name_split = parameter_name.split('/')
+            if len(parameter_name_split) == 1:
+                param_name = parameter_name
+                param_dir = ''
+            else:
+                param_name = parameter_name_split[-1]
+                param_dir = '/'.join(parameter_name_split[:-1])
         
         if(suffix == 'mat'):
             if(len(param_name) == 0):
-                param_name = param_dir.name            
-        
+                param_dir_split = param_dir.split('/')
+                if param_dir_split[-1] == '/':
+                    param_name = param_dir_split[-2]
+                else:
+                    param_name = param_dir_split[-1]
+                    
         if(suffix is None):
             param_name_split = param_name.split('.')
             if len(param_name_split) > 1:
                 param_suffix = param_name_split[-1]
                 #Here you can check if it is a valid extention
                 param_name = '.'.join(param_name_split[:-1])
             else:
@@ -293,73 +303,87 @@
             if len(param_name_split) > 1:
                 fname_suffix = param_name_split[-1]
                 if fname_suffix == param_suffix:
                     param_name = '.'.join(param_name_split[:-1])
     
         return(param_dir, param_name, param_suffix)
 
-    def _get_fpath(self, param_dir: pathlib.Path, param_name: str, 
-                   suffix: str, time_tag: bool = None) -> pathlib.Path:
+    def _get_fpath(self, param_dir: pathlib.Path, param_name: str = None, 
+                   suffix: str = None, time_tag: bool = None) -> pathlib.Path:
         
         time_tag = self.time_tag if (time_tag is None) else time_tag
         
-        if(not param_dir.is_dir()):
-            self.log_text(self.log_name,
-                          f'Creating directory: {param_dir.absolute()}')
-            param_dir.mkdir(parents = True, exist_ok = True)
+        _param_dir = self.log_dir / param_dir
         
-        if(len(param_name) > 0):
-            fname = f'{param_name}'
-            if(time_tag):
-                fname += f'_{self.time_stamp:>6.6f}'
+        if(not _param_dir.is_dir()):
+            self.log_text(self.log_name,
+                          f'Creating directory: {_param_dir.absolute()}')
+            _param_dir.mkdir(parents = True, exist_ok = True)
+            
+        if(param_name is not None):
+            if(len(param_name) > 0):
+                fname = f'{param_name}'
+                if(time_tag):
+                    fname += f'_{self.time_stamp:>6.6f}'
+            else:
+                fname = f'{self.time_stamp:>6.6f}'
+                
+            if(suffix is None):
+                fpath = _param_dir / f'{fname}'
+            else:
+                fpath = _param_dir / f'{fname}.{suffix}'
+            return fpath
         else:
-            fname = f'{self.time_stamp:>6.6f}'
-        
-        fpath = param_dir / f'{fname}.{suffix}'
-        
-        return fpath
+            return _param_dir
         
     def _log_text_handler(self, log_name: str, 
                          log_size_limit: int = int(1e+7),
                          time_tag: bool = None,
                          log_flush_period = None,
                          suffix = None):
         
         if (log_flush_period is None):
             log_flush_period = self.log_flush_period
         param_dir, param_name, suffix = self._param_dir_name_suffix(
             log_name, suffix)
         if suffix is None:
             suffix = 'txt'
+        log_dirnamesuffix = param_dir + '/' + param_name + '.' + suffix
+        
         fpath = self._get_fpath(param_dir, param_name, suffix, time_tag)
-        self._loggers_dict[log_name] = textinlog(
+        self._loggers_dict[log_dirnamesuffix] = textinlog(
             to_be_logged=[],      
             log_fpath=fpath,         
             log_size_limit=log_size_limit,    
             log_size=0,          
             last_log_flush_time=0,
             log_flush_period=log_flush_period)  
 
-    def log_text_flush(self, log_name = None, 
-                       flush = False):
+    def log_text_flush(self, log_name = None, flush = False, suffix = None):
         """ Flush the text logs
             Writing text to open(file, 'a') does not constantly happen on HDD.
             There is an OS buffer in between. This funciton should be called
             regularly. lognflow calls it once in a while when log_text is
             called multiple times. but use needs to also call it once in a
             while.
             In later versions, a timer will be used to call it automatically.
             :param flush:
                 force the flush regardless of when the last time was.
                 default: False
             :type flush: bool
         """
         log_name = self.log_name if (log_name is None) else log_name
         
-        curr_textinlog = self._loggers_dict[log_name]
+        param_dir, param_name, suffix = self._param_dir_name_suffix(
+            log_name, suffix)
+        if suffix is None:
+            suffix = 'txt'
+        log_dirnamesuffix = param_dir + '/' + param_name + '.' + suffix
+        
+        curr_textinlog = self._loggers_dict[log_dirnamesuffix]
         
         if((self.time_stamp - curr_textinlog.last_log_flush_time \
                                            > curr_textinlog.log_flush_period)
            | flush):
             
             with open(curr_textinlog.log_fpath, 'a+') as f:
                 f.writelines(curr_textinlog.to_be_logged)
@@ -417,28 +441,34 @@
                    suffix is the extension of the file name.
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
         log_flush_period = self.log_flush_period \
             if (log_flush_period is None) else log_flush_period
         log_name = self.log_name if (log_name is None) else log_name
 
-        if ( (not (log_name in self._loggers_dict)) or new_file):
-            self._log_text_handler(log_name, 
+        param_dir, param_name, suffix = self._param_dir_name_suffix(
+            log_name, suffix)
+        if suffix is None:
+            suffix = 'txt'
+        log_dirnamesuffix = param_dir + '/' + param_name + '.' + suffix
+
+        if ( (not (log_dirnamesuffix in self._loggers_dict)) or new_file):
+            self._log_text_handler(log_dirnamesuffix, 
                                    log_size_limit = log_size_limit,
                                    time_tag = time_tag,
                                    suffix = suffix)
 
         if((print_text is None) | (print_text is True)):
             print_text = self._print_text
         if(print_text):
             if(log_time_stamp):
                 print(f'T:{self.time_stamp:>6.6f}| ', end='')
             print(to_be_logged, end = end)
 
-        curr_textinlog = self._loggers_dict[log_name]
+        curr_textinlog = self._loggers_dict[log_dirnamesuffix]
         _logger = []
         if(log_time_stamp):
             _time_str = f'T:{self.time_stamp:>6.6f}| '
             _logger.append(_time_str)
         if(isinstance(to_be_logged, list)):
             for _ in to_be_logged:
                 _tolog = str(_)
@@ -453,22 +483,22 @@
             _logger.append(end)
         log_size = 0
         for _logger_el in _logger:
             curr_textinlog.to_be_logged.append(_logger_el)
             log_size += len(_logger_el)
         curr_textinlog.log_size += log_size
         
-        self.log_text_flush(log_name, flush)        
+        self.log_text_flush(log_dirnamesuffix, flush)        
 
         if(log_size >= curr_textinlog.log_size_limit):
-            self._log_text_handler(log_name, 
+            self._log_text_handler(log_dirnamesuffix, 
                                    log_size_limit = curr_textinlog.log_size_limit,
                                    time_tag = curr_textinlog.time_tag,
                                    suffix = suffix)
-            curr_textinlog = self._loggers_dict[log_name]
+            curr_textinlog = self._loggers_dict[log_dirnamesuffix]
         return curr_textinlog.log_fpath
                         
 
     def _get_log_counter_limit(self, param, log_size_limit):
         cnt_limit = int(log_size_limit/(param.size*param.itemsize))
         return cnt_limit
 
@@ -499,34 +529,36 @@
                     
         """
         try:
             _ = parameter_value.shape
         except:
             parameter_value = np.array([parameter_value])
         
-        _, _, suffix = self._param_dir_name_suffix(parameter_name, suffix)
+        param_dir, param_name, suffix = self._param_dir_name_suffix(
+            parameter_name, suffix)
         if(suffix is None):
             suffix = 'npz'
+        log_dirnamesuffix = param_dir + '/' + param_name + '.' + suffix
         
         log_counter_limit = self._get_log_counter_limit(\
             parameter_value, log_size_limit)
 
-        if(parameter_name in self._vars_dict):
-            _var = self._vars_dict[parameter_name]
+        if(log_dirnamesuffix in self._vars_dict):
+            _var = self._vars_dict[log_dirnamesuffix]
             data_array, time_array, curr_index, \
                 file_start_time, suffix, log_counter_limit = \
                 (_var.data_array, _var.time_array, _var.curr_index, \
                     _var.file_start_time, _var.suffix, _var.log_counter_limit)
             curr_index += 1
         else:
             file_start_time = self.time_stamp
             curr_index = 0
 
         if(curr_index >= log_counter_limit):
-            self.log_var_flush(parameter_name)
+            self.log_var_flush(log_dirnamesuffix)
             file_start_time = self.time_stamp
             curr_index = 0
 
         if(curr_index == 0):
             data_array = np.zeros((log_counter_limit, ) + parameter_value.shape,
                                   dtype = parameter_value.dtype)
             time_array = np.zeros(log_counter_limit)
@@ -538,68 +570,80 @@
                 self.log_name,
                 f'current index {curr_index} cannot be used in the logger')
         if(parameter_value.shape == data_array[curr_index].shape):
             data_array[curr_index] = parameter_value
         else:
             self.log_text(
                 self.log_name,
-                f'Shape of variable {parameter_name} cannot change shape '\
+                f'Shape of variable {log_dirnamesuffix} cannot change shape '\
                 f'from {data_array[curr_index].shape} '\
                 f'to {parameter_value.shape}. Coppying from the last time.')
             data_array[curr_index] = data_array[curr_index - 1]
-        self._vars_dict[parameter_name] = varinlog(data_array, 
-                                                   time_array, 
-                                                   curr_index,
-                                                   file_start_time,
-                                                   suffix,
-                                                   log_counter_limit)
+        self._vars_dict[log_dirnamesuffix] = varinlog(data_array, 
+                                                      time_array, 
+                                                      curr_index,
+                                                      file_start_time,
+                                                      suffix,
+                                                      log_counter_limit)
 
-    def log_var_flush(self, parameter_name: str):
+    def log_var_flush(self, parameter_name: str, suffix: str = None):
         """ Flush the buffered numpy arrays
             If you have been using log_ver, this will flush all the buffered
             arrays. It is called using log_size_limit for a variable and als
             when the code that made the logger ends.
             :param parameter_name: str
                 examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
         """
-        param_dir, param_name, _ = self._param_dir_name_suffix(parameter_name)
+        param_dir, param_name, suffix = self._param_dir_name_suffix(
+            parameter_name, suffix)
+        if(suffix is None):
+            suffix = 'npz'
+        log_dirnamesuffix = param_dir + '/' + param_name + '.' + suffix
+        
+        _param_dir = self._get_fpath(param_dir)
         
-        _var = self._vars_dict[parameter_name]
+        _var = self._vars_dict[log_dirnamesuffix]
         _var_data_array = _var.data_array[_var.time_array > 0]
         _var_time_array = _var.time_array[_var.time_array > 0]
         if((_var.suffix == 'npz') | (_var.suffix == 'npy')):
-            fpath = param_dir / f'{param_name}_{_var.file_start_time}.npz'
+            fpath = _param_dir / f'{param_name}_{_var.file_start_time}.npz'
             np.savez(fpath,
                 time_array = _var_time_array,
                 data_array = _var_data_array)
         else:
-            fpath = param_dir / f'{param_name}_time_{_var.file_start_time}.txt'
+            fpath = _param_dir / f'{param_name}_time_{_var.file_start_time}.txt'
             np.savetxt(fpath, _var_time_array)
-            fpath = param_dir / f'{param_name}_data_{_var.file_start_time}.txt'
+            fpath = _param_dir / f'{param_name}_data_{_var.file_start_time}.txt'
             np.savetxt(fpath, _var_data_array)
         return fpath
     
-    def get_var(self, parameter_name: str) -> tuple:
+    def get_var(self, parameter_name: str, suffix: str = None) -> tuple:
         """ Get the buffered numpy arrays
             If you need the buffered variable back.
             :param parameter_name: str
                 examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
             
             :return: 
                 A tuple including two np.ndarray. The first on is 1d time
                 and the second one is nd buffered data.
             :rtype: 
                 tuple of two nd.arrays
         
         """
-        _var = self._vars_dict[parameter_name]
+        param_dir, param_name, suffix = self._param_dir_name_suffix(
+            parameter_name, suffix)
+        if(suffix is None):
+            suffix = 'npz'
+        log_dirnamesuffix = param_dir + '/' + param_name + '.' + suffix
+        
+        _var = self._vars_dict[log_dirnamesuffix]
         data_array = _var.data_array[_var.time_array>0].copy()
         time_array = _var.time_array[_var.time_array>0].copy()
         return(time_array, data_array)
 
     def log_single(self, parameter_name: str, 
                          parameter_value,
                          suffix = None,
@@ -1427,17 +1471,17 @@
                     n_f x n_r x n_c or n_f x n_r x n_c x 3
                     stack[cnt] needs to be plotable by plt.imshow()
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
             
-        param_dir, param_name, _ = self._param_dir_name_suffix(parameter_name, 
-                                                               'gif')
-        fpath = self._get_fpath(param_dir, param_name, 'gif', time_tag)
+        param_dir, param_name, suffix = self._param_dir_name_suffix(
+            parameter_name, 'gif')
+        fpath = self._get_fpath(param_dir, param_name, suffix, time_tag)
 
         fig, ax = plt.subplots()
         ims = []
         for img in stack:    
             im = ax.imshow(img, animated=True)
             plt.xticks([]),plt.yticks([])
             ims.append([im])
```

### Comparing `lognflow-0.8.3/lognflow/logviewer.py` & `lognflow-0.8.4/lognflow/logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.3/lognflow/printprogress.py` & `lognflow-0.8.4/lognflow/printprogress.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.3/lognflow/utils.py` & `lognflow-0.8.4/lognflow/utils.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.3/lognflow.egg-info/PKG-INFO` & `lognflow-0.8.4/lognflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.8.3
+Version: 0.8.4
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -225,7 +225,13 @@
 ------------------
 * the word save_as is now replaced with suffix as is in pathlib
 * all loggers can take the suffix as the extension in the parameter_name
 
 0.8.3 (2023-08-02)
 -----------------
 * critical bug fixed in log_var to support v0.8.2
+
+0.8.4 (2023-08-03)
+-----------------
+* variable names that are pecular will always be fixed first.
+* suffix can be read form the file name.
+* time_tag will always accompany file name unless stated otherwised.
```

### Comparing `lognflow-0.8.3/lognflow.egg-info/SOURCES.txt` & `lognflow-0.8.4/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.3/setup.py` & `lognflow-0.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.8.3'
+__version__ = '0.8.4'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.8.3/tests/test_lognflow.py` & `lognflow-0.8.4/tests/test_lognflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,16 @@
            'This is a new log file for another script', suffix = 'io')
     logger.log_text('test.to\not_main_script4.top',
                     'For other log files you need to mention the log_name')
     logger.log_text('not_main_script2',
            'This is a new log file for another script')
     logger.log_text('not_main_script2.test',
                     'For other log files you need to mention the log_name')
+    logger.log_text('test.to\not_main_script4.top',
+                    'To see if variable names are OK when passed properly')
     for _ in range(10000):
         logger(f'{_}')
 
 def test_logger():
     ''' test the logger call funciton
         when lognflow object is made, you can call it.
         If it is called with a string as input, it will log that into the
@@ -308,17 +310,17 @@
     logger(data_out)
     
 if __name__ == '__main__':
     
     #-----IF RUN BY PYTHON------#
     temp_dir = select_directory()
     #---------------------------#
-    test_log_single()
     test_log_var()
     test_log_text()
+    test_log_single()
     test_log_single_text()
     test_log_imshow_complex()
     test_log_imshow()
     test_log_surface()
     test_lognflow_conflict_in_names()
     test_rename()
     test_log_plot()
```

### Comparing `lognflow-0.8.3/tests/test_logviewer.py` & `lognflow-0.8.4/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.3/tests/test_printprogress.py` & `lognflow-0.8.4/tests/test_printprogress.py`

 * *Files identical despite different names*

