# Comparing `tmp/alertmanagermeshtastic-2023.8.2.8.tar.gz` & `tmp/alertmanagermeshtastic-2023.8.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alertmanagermeshtastic-2023.8.2.8.tar", last modified: Wed Aug  2 22:06:23 2023, max compression
+gzip compressed data, was "alertmanagermeshtastic-2023.8.2.9.tar", last modified: Wed Aug  2 22:17:42 2023, max compression
```

## Comparing `alertmanagermeshtastic-2023.8.2.8.tar` & `alertmanagermeshtastic-2023.8.2.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:06:23.541051 alertmanagermeshtastic-2023.8.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-08-02 22:06:23.545051 alertmanagermeshtastic-2023.8.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/config_example.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/config_example_docker.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/requirements-release.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-02 22:06:23.545051 alertmanagermeshtastic-2023.8.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:06:23.537050 alertmanagermeshtastic-2023.8.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:06:23.541051 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/meshtastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/tokencli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:06:23.541051 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-08-02 22:06:23.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-02 22:06:23.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:06:23.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-02 22:06:23.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:06:23.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 22:06:23.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 22:06:23.000000 alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:06:23.541051 alertmanagermeshtastic-2023.8.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/tests/test_create_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/tests/test_dummy_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/tests/test_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/tests/test_meshtastic_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/tests/test_meshtastic_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-02 22:06:14.000000 alertmanagermeshtastic-2023.8.2.8/tests/test_token_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:17:42.660809 alertmanagermeshtastic-2023.8.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-08-02 22:17:42.660809 alertmanagermeshtastic-2023.8.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/config_example.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/config_example_docker.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/requirements-release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-02 22:17:42.660809 alertmanagermeshtastic-2023.8.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:17:42.652808 alertmanagermeshtastic-2023.8.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:17:42.656808 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/meshtastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/tokencli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:17:42.660809 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-08-02 22:17:42.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-02 22:17:42.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:17:42.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-02 22:17:42.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:17:42.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 22:17:42.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 22:17:42.000000 alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:17:42.660809 alertmanagermeshtastic-2023.8.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/tests/test_create_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/tests/test_dummy_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/tests/test_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/tests/test_meshtastic_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/tests/test_meshtastic_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-02 22:17:32.000000 alertmanagermeshtastic-2023.8.2.9/tests/test_token_cli.py
```

### Comparing `alertmanagermeshtastic-2023.8.2.8/Dockerfile` & `alertmanagermeshtastic-2023.8.2.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/LICENSE` & `alertmanagermeshtastic-2023.8.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/PKG-INFO` & `alertmanagermeshtastic-2023.8.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.2.8
+Version: 2023.8.2.9
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanagermeshtastic
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanagermeshtastic
 Project-URL: Changelog, https://github.com/Apfelwurm/alertmanagermeshtastic/releases
```

### Comparing `alertmanagermeshtastic-2023.8.2.8/README.md` & `alertmanagermeshtastic-2023.8.2.9/README.md`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/setup.cfg` & `alertmanagermeshtastic-2023.8.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/cli.py` & `alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/cli.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/config.py` & `alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/http.py` & `alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/http.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/meshtastic.py` & `alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/meshtastic.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/processor.py` & `alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/processor.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic/util.py` & `alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic/util.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic.egg-info/PKG-INFO` & `alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.2.8
+Version: 2023.8.2.9
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanagermeshtastic
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanagermeshtastic
 Project-URL: Changelog, https://github.com/Apfelwurm/alertmanagermeshtastic/releases
```

### Comparing `alertmanagermeshtastic-2023.8.2.8/src/alertmanagermeshtastic.egg-info/SOURCES.txt` & `alertmanagermeshtastic-2023.8.2.9/src/alertmanagermeshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/tests/test_create_announcer.py` & `alertmanagermeshtastic-2023.8.2.9/tests/test_create_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/tests/test_dummy_announcer.py` & `alertmanagermeshtastic-2023.8.2.9/tests/test_dummy_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/tests/test_load_config.py` & `alertmanagermeshtastic-2023.8.2.9/tests/test_load_config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/tests/test_meshtastic_announcer.py` & `alertmanagermeshtastic-2023.8.2.9/tests/test_meshtastic_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/tests/test_meshtastic_channel.py` & `alertmanagermeshtastic-2023.8.2.9/tests/test_meshtastic_channel.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.2.8/tests/test_token_cli.py` & `alertmanagermeshtastic-2023.8.2.9/tests/test_token_cli.py`

 * *Files identical despite different names*

