# Comparing `tmp/autosubmitconfigparser-1.0.42.tar.gz` & `tmp/autosubmitconfigparser-1.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmitconfigparser-1.0.42.tar", last modified: Fri Jul 21 08:55:23 2023, max compression
+gzip compressed data, was "autosubmitconfigparser-1.0.43.tar", last modified: Thu Aug  3 10:26:38 2023, max compression
```

## Comparing `autosubmitconfigparser-1.0.42.tar` & `autosubmitconfigparser-1.0.43.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:55:23.084870 autosubmitconfigparser-1.0.42/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.42/MANIFEST.in
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-07-21 08:55:23.084870 autosubmitconfigparser-1.0.42/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.42/README.md
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:55:23.080870 autosubmitconfigparser-1.0.42/autosubmitconfigparser/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:48:23.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:55:23.084870 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:49:24.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/__init__.py
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/basicconfig.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   107552 2023-07-21 08:27:49.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/configcommon.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:55:23.084870 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/autosubmit-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/autosubmit.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/expdef-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/expdef.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/git-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/jobs-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/jobs.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/local-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/platforms-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/platforms.yml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      275 2023-06-07 12:06:41.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/yamlparser.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:55:23.084870 autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-07-21 08:55:23.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1029 2023-07-21 08:55:23.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/SOURCES.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-07-21 08:55:23.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/dependency_links.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      321 2023-07-21 08:55:23.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/requires.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-07-21 08:55:23.000000 autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/top_level.txt
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:55:23.084870 autosubmitconfigparser-1.0.42/log/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.42/log/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.42/log/fd_show.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.42/log/log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-07-21 08:55:23.084870 autosubmitconfigparser-1.0.42/setup.cfg
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1461 2023-07-21 08:52:24.000000 autosubmitconfigparser-1.0.42/setup.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-03 10:26:38.325893 autosubmitconfigparser-1.0.43/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.43/MANIFEST.in
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-08-03 10:26:38.325893 autosubmitconfigparser-1.0.43/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.43/README.md
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-03 10:26:38.325893 autosubmitconfigparser-1.0.43/autosubmitconfigparser/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:48:23.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-03 10:26:38.325893 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:49:24.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/__init__.py
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/basicconfig.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   108079 2023-08-02 10:21:05.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/configcommon.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-03 10:26:38.325893 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/autosubmit-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/autosubmit.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/expdef-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/expdef.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/git-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/jobs-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/jobs.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/local-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/platforms-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/platforms.yml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      275 2023-06-07 12:06:41.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/yamlparser.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-03 10:26:38.325893 autosubmitconfigparser-1.0.43/autosubmitconfigparser.egg-info/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-08-03 10:26:38.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser.egg-info/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1029 2023-08-03 10:26:38.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-08-03 10:26:38.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      321 2023-08-03 10:26:38.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser.egg-info/requires.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-08-03 10:26:38.000000 autosubmitconfigparser-1.0.43/autosubmitconfigparser.egg-info/top_level.txt
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-03 10:26:38.325893 autosubmitconfigparser-1.0.43/log/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.43/log/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.43/log/fd_show.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.43/log/log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-08-03 10:26:38.325893 autosubmitconfigparser-1.0.43/setup.cfg
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1461 2023-08-03 10:24:31.000000 autosubmitconfigparser-1.0.43/setup.py
```

### Comparing `autosubmitconfigparser-1.0.42/PKG-INFO` & `autosubmitconfigparser-1.0.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.42
+Version: 1.0.43
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 Keywords: climate,weather,workflow,HPC
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `autosubmitconfigparser-1.0.42/README.md` & `autosubmitconfigparser-1.0.43/README.md`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/basicconfig.py` & `autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/basicconfig.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/configcommon.py` & `autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/configcommon.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,23 +52,26 @@
     def __init__(self, expid, basic_config=BasicConfig, parser_factory=YAMLParserFactory()):
         self.data_changed = False
         self.ignore_undefined_platforms = False
         self.ignore_file_path = False
         self.expid = expid
         self.basic_config = basic_config
         self.basic_config.read()
+        if not Path(BasicConfig.LOCAL_ROOT_DIR, expid).exists():
+            raise IOError(f"Experiment {expid} does not exist")
         self.parser_factory = parser_factory
         self.experiment_data = {}
         self.last_experiment_data = {}
         self.data_loops = list()
 
 
         self.current_loaded_files = dict()
         self.conf_folder_yaml = Path(BasicConfig.LOCAL_ROOT_DIR, expid, "conf")
-
+        if not Path(BasicConfig.LOCAL_ROOT_DIR, expid, "conf").exists():
+            raise IOError(f"Experiment {expid}/conf does not exist")
         self.wrong_config = defaultdict(list)
         self.warn_config = defaultdict(list)
         self.dynamic_variables = list()
         self.special_dynamic_variables = list() # variables that will be sustituted after all files is loaded
         self.starter_conf = dict()
 
     @property
@@ -193,15 +196,15 @@
         """
         Gets the chunk increase to wallclock  
         :param section: job type
         :type section: str
         :return: wallclock increase per chunk
         :rtype: str
         """
-        return self.get_section([section, 'WCHUNKINC'], "")
+        return self.jobs_data.get(section,{}).get('WCHUNKINC',"")
 
     def get_synchronize(self, section):
         """
         Gets wallclock for the given job type
         :param section: job type
         :type section: str
         :return: wallclock time
@@ -1411,29 +1414,34 @@
             # IF expid and hpcarch are not defined, use the ones from the minimal.yml file
             self.deep_add_missing_starter_conf(self.experiment_data,starter_conf)
             self.experiment_data = self.substitute_dynamic_variables(self.experiment_data)
             self.experiment_data = self.normalize_variables(self.experiment_data)
             self.experiment_data = self.substitute_dynamic_variables(self.experiment_data,in_the_end=True)
 
     def load_last_run(self):
-        self.metadata_folder = Path(self.conf_folder_yaml) / "metadata"
-        if not self.metadata_folder.exists():
-            os.makedirs(self.metadata_folder)
-            os.chmod(self.metadata_folder, 0o775)
-        if not os.access(self.metadata_folder, os.W_OK):
-            print(f"WARNING: Can't save the experiment data into {self.metadata_folder}, no write permissions")
-        else:
-            # Load data from last run
-            if (Path(self.metadata_folder) / "experiment_data.yml").exists():
-                with open(Path(self.metadata_folder) / "experiment_data.yml", 'r') as stream:
-                    self.last_experiment_data = yaml.load(stream, Loader=yaml.SafeLoader)
-                self.data_changed = self.quick_deep_diff(self.experiment_data, self.last_experiment_data)
+        try:
+            self.metadata_folder = Path(self.conf_folder_yaml) / "metadata"
+            if not self.metadata_folder.exists():
+                os.makedirs(self.metadata_folder)
+                os.chmod(self.metadata_folder, 0o775)
+            if not os.access(self.metadata_folder, os.W_OK):
+                print(f"WARNING: Can't save the experiment data into {self.metadata_folder}, no write permissions")
             else:
-                self.last_experiment_data = {}
-                self.data_changed = True
+                # Load data from last run
+                if (Path(self.metadata_folder) / "experiment_data.yml").exists():
+                    with open(Path(self.metadata_folder) / "experiment_data.yml", 'r') as stream:
+                        self.last_experiment_data = yaml.load(stream, Loader=yaml.SafeLoader)
+                    self.data_changed = self.quick_deep_diff(self.experiment_data, self.last_experiment_data)
+                else:
+                    self.last_experiment_data = {}
+                    self.data_changed = True
+        except IOError as e:
+            self.last_experiment_data = {}
+            self.data_changed = True
+            Log.warning(f"Can't load the last experiment data: {e}")
     def save(self):
         """
         Saves the experiment data into the experiment_folder/conf/metadata folder as a yaml file
         :return: True if the data has changed, False otherwise
         """
         changed = False
         # check if the folder exists and we have write permissions, if folder doesn't exist create it with rwx/rwx/r-x permissions
```

### Comparing `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/expdef-dummy.yml` & `autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/expdef-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/expdef.yml` & `autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/expdef.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/jobs-dummy.yml` & `autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/jobs-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/jobs.yml` & `autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/jobs.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/platforms-dummy.yml` & `autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/platforms-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.42/autosubmitconfigparser/config/files/platforms.yml` & `autosubmitconfigparser-1.0.43/autosubmitconfigparser/config/files/platforms.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/PKG-INFO` & `autosubmitconfigparser-1.0.43/autosubmitconfigparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.42
+Version: 1.0.43
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 Keywords: climate,weather,workflow,HPC
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `autosubmitconfigparser-1.0.42/autosubmitconfigparser.egg-info/SOURCES.txt` & `autosubmitconfigparser-1.0.43/autosubmitconfigparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.42/log/fd_show.py` & `autosubmitconfigparser-1.0.43/log/fd_show.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.42/log/log.py` & `autosubmitconfigparser-1.0.43/log/log.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.42/setup.py` & `autosubmitconfigparser-1.0.43/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autosubmitconfigparser",
-    version="1.0.42",
+    version="1.0.43",
     author="Daniel Beltran Mora",
     author_email="daniel.beltran@bsc.es",
     description="An utility library that allows to read an Autosubmit 4 experiment configuration.",
     keywords=['climate', 'weather', 'workflow', 'HPC'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git",
```

