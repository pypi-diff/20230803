# Comparing `tmp/alertmanagermeshtastic-2023.8.3.2.tar.gz` & `tmp/alertmanagermeshtastic-2023.8.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alertmanagermeshtastic-2023.8.3.2.tar", last modified: Thu Aug  3 19:10:07 2023, max compression
+gzip compressed data, was "alertmanagermeshtastic-2023.8.3.3.tar", last modified: Thu Aug  3 19:17:42 2023, max compression
```

## Comparing `alertmanagermeshtastic-2023.8.3.2.tar` & `alertmanagermeshtastic-2023.8.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:10:07.474912 alertmanagermeshtastic-2023.8.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-08-03 19:10:07.474912 alertmanagermeshtastic-2023.8.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/config_example.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/config_example_docker.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/requirements-release.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-03 19:10:07.474912 alertmanagermeshtastic-2023.8.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:10:07.466912 alertmanagermeshtastic-2023.8.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:10:07.470912 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/meshtastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/tokencli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:10:07.474912 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-08-03 19:10:07.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-03 19:10:07.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:10:07.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-03 19:10:07.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:10:07.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-03 19:10:07.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 19:10:07.000000 alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:10:07.474912 alertmanagermeshtastic-2023.8.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/tests/test_create_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/tests/test_dummy_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/tests/test_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/tests/test_meshtastic_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/tests/test_meshtastic_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-03 19:10:00.000000 alertmanagermeshtastic-2023.8.3.2/tests/test_token_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:17:42.677606 alertmanagermeshtastic-2023.8.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-08-03 19:17:42.677606 alertmanagermeshtastic-2023.8.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/config_example.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/config_example_docker.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/requirements-release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-03 19:17:42.677606 alertmanagermeshtastic-2023.8.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:17:42.665606 alertmanagermeshtastic-2023.8.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:17:42.673606 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/meshtastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/tokencli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:17:42.673606 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-08-03 19:17:42.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-03 19:17:42.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:17:42.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-03 19:17:42.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:17:42.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-03 19:17:42.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 19:17:42.000000 alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:17:42.677606 alertmanagermeshtastic-2023.8.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/tests/test_create_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/tests/test_dummy_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/tests/test_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/tests/test_meshtastic_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/tests/test_meshtastic_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-03 19:17:34.000000 alertmanagermeshtastic-2023.8.3.3/tests/test_token_cli.py
```

### Comparing `alertmanagermeshtastic-2023.8.3.2/Dockerfile` & `alertmanagermeshtastic-2023.8.3.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/LICENSE` & `alertmanagermeshtastic-2023.8.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/PKG-INFO` & `alertmanagermeshtastic-2023.8.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.3.2
+Version: 2023.8.3.3
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanagermeshtastic
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanagermeshtastic
 Project-URL: Changelog, https://github.com/Apfelwurm/alertmanagermeshtastic/releases
```

### Comparing `alertmanagermeshtastic-2023.8.3.2/README.md` & `alertmanagermeshtastic-2023.8.3.3/README.md`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/setup.cfg` & `alertmanagermeshtastic-2023.8.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/cli.py` & `alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/cli.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/config.py` & `alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/http.py` & `alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/http.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/meshtastic.py` & `alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/meshtastic.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/processor.py` & `alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         logger.debug('\t Messages in queue: %d', self.message_queue.qsize())
         """Process a message from the queue."""
         alert = self.message_queue.get(timeout=timeout_seconds)
         logger.debug(
             '\t [%s][%d] processing message ', alert["fingerprint"], alert["qn"]
         )
         self.announce_message(alert)
+        queue_size_updated.send(self.message_queue.qsize())
 
     def run(self) -> None:
         """Run the main loop."""
         self.announcer.start()
         start_receive_server(self.config.http)
 
         logger.info('\t Starting to process queue ...')
```

### Comparing `alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic/util.py` & `alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic/util.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic.egg-info/PKG-INFO` & `alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.3.2
+Version: 2023.8.3.3
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanagermeshtastic
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanagermeshtastic
 Project-URL: Changelog, https://github.com/Apfelwurm/alertmanagermeshtastic/releases
```

### Comparing `alertmanagermeshtastic-2023.8.3.2/src/alertmanagermeshtastic.egg-info/SOURCES.txt` & `alertmanagermeshtastic-2023.8.3.3/src/alertmanagermeshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/tests/test_create_announcer.py` & `alertmanagermeshtastic-2023.8.3.3/tests/test_create_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/tests/test_dummy_announcer.py` & `alertmanagermeshtastic-2023.8.3.3/tests/test_dummy_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/tests/test_load_config.py` & `alertmanagermeshtastic-2023.8.3.3/tests/test_load_config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/tests/test_meshtastic_announcer.py` & `alertmanagermeshtastic-2023.8.3.3/tests/test_meshtastic_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/tests/test_meshtastic_channel.py` & `alertmanagermeshtastic-2023.8.3.3/tests/test_meshtastic_channel.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.3.2/tests/test_token_cli.py` & `alertmanagermeshtastic-2023.8.3.3/tests/test_token_cli.py`

 * *Files identical despite different names*

