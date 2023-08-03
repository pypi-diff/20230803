# Comparing `tmp/fotoobo-1.0.0.tar.gz` & `tmp/fotoobo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fotoobo-1.0.0.tar", max compression
+gzip compressed data, was "fotoobo-1.0.1.tar", max compression
```

## Comparing `fotoobo-1.0.0.tar` & `fotoobo-1.0.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     7633 2023-08-03 09:50:30.968500 fotoobo-1.0.0/LICENSE
--rw-r--r--   0        0        0     2520 2023-08-03 09:50:30.968500 fotoobo-1.0.0/README.md
--rw-r--r--   0        0        0      409 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/__init__.py
--rw-r--r--   0        0        0      195 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/__init__.py
--rw-r--r--   0        0        0     1817 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/convert.py
--rw-r--r--   0        0        0       20 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/ems/__init__.py
--rw-r--r--   0        0        0     1488 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/ems/get_commands.py
--rw-r--r--   0        0        0      784 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/ems/main.py
--rw-r--r--   0        0        0    11047 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/ems/monitor_commands.py
--rw-r--r--   0        0        0       20 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/faz/__init__.py
--rw-r--r--   0        0        0      976 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/faz/get_commands.py
--rw-r--r--   0        0        0      639 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/faz/main.py
--rw-r--r--   0        0        0       20 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fgt/__init__.py
--rw-r--r--   0        0        0     2172 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fgt/config_commands.py
--rw-r--r--   0        0        0     1241 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fgt/get_commands.py
--rw-r--r--   0        0        0     3547 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fgt/main.py
--rw-r--r--   0        0        0     3951 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fgt/monitor_commands.py
--rw-r--r--   0        0        0       20 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fmg/__init__.py
--rw-r--r--   0        0        0     2631 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fmg/get_commands.py
--rw-r--r--   0        0        0     2394 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fmg/main.py
--rw-r--r--   0        0        0     1802 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/get.py
--rw-r--r--   0        0        0     4825 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/main.py
--rw-r--r--   0        0        0      196 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/exceptions/__init__.py
--rw-r--r--   0        0        0     1966 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/exceptions/exceptions.py
--rw-r--r--   0        0        0      423 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/__init__.py
--rw-r--r--   0        0        0    13927 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/convert.py
--rw-r--r--   0        0        0     1023 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/fortianalyzer.py
--rw-r--r--   0        0        0     5602 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/forticlientems.py
--rw-r--r--   0        0        0     2961 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/fortigate.py
--rw-r--r--   0        0        0    11488 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/fortigate_config.py
--rw-r--r--   0        0        0     8714 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/fortigate_config_check.py
--rw-r--r--   0        0        0      584 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/fortigate_info.py
--rw-r--r--   0        0        0    12434 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/fortimanager.py
--rw-r--r--   0        0        0     6431 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/fortinet.py
--rw-r--r--   0        0        0      322 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/helpers/__init__.py
--rw-r--r--   0        0        0     1227 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/helpers/cli.py
--rw-r--r--   0        0        0     3617 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/helpers/config.py
--rw-r--r--   0        0        0     5408 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/helpers/files.py
--rw-r--r--   0        0        0    10994 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/helpers/log.py
--rw-r--r--   0        0        0     4958 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/helpers/output.py
--rw-r--r--   0        0        0    10362 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/helpers/result.py
--rw-r--r--   0        0        0      128 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/inventory/__init__.py
--rw-r--r--   0        0        0      568 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/inventory/generic.py
--rw-r--r--   0        0        0     5203 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/inventory/inventory.py
--rwxr-xr-x   0        0        0     1359 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/main.py
--rw-r--r--   0        0        0      428 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/__init__.py
--rw-r--r--   0        0        0     1284 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/convert.py
--rw-r--r--   0        0        0       92 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/ems/__init__.py
--rw-r--r--   0        0        0     1626 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/ems/get.py
--rw-r--r--   0        0        0     8338 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/ems/monitor.py
--rw-r--r--   0        0        0       56 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/faz/__init__.py
--rw-r--r--   0        0        0      809 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/faz/get.py
--rw-r--r--   0        0        0      129 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fgt/__init__.py
--rw-r--r--   0        0        0     4619 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fgt/config.py
--rw-r--r--   0        0        0     2377 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fgt/get.py
--rw-r--r--   0        0        0     2978 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fgt/main.py
--rw-r--r--   0        0        0     4274 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fgt/monitor.py
--rw-r--r--   0        0        0      105 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fmg/__init__.py
--rw-r--r--   0        0        0     4417 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fmg/get.py
--rw-r--r--   0        0        0     2733 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fmg/main.py
--rw-r--r--   0        0        0     1882 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/get.py
--rw-r--r--   0        0        0     1306 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/greet.py
--rw-r--r--   0        0        0     3711 2023-08-03 09:50:30.976501 fotoobo-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 fotoobo-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7633 2023-08-03 11:04:57.682871 fotoobo-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2520 2023-08-03 11:04:57.682871 fotoobo-1.0.1/README.md
+-rw-r--r--   0        0        0      409 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/__init__.py
+-rw-r--r--   0        0        0      195 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/__init__.py
+-rw-r--r--   0        0        0     1817 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/convert.py
+-rw-r--r--   0        0        0       20 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/ems/__init__.py
+-rw-r--r--   0        0        0     1488 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/ems/get_commands.py
+-rw-r--r--   0        0        0      784 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/ems/main.py
+-rw-r--r--   0        0        0    11047 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/ems/monitor_commands.py
+-rw-r--r--   0        0        0       20 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/faz/__init__.py
+-rw-r--r--   0        0        0      976 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/faz/get_commands.py
+-rw-r--r--   0        0        0      639 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/faz/main.py
+-rw-r--r--   0        0        0       20 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/fgt/__init__.py
+-rw-r--r--   0        0        0     2172 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/fgt/config_commands.py
+-rw-r--r--   0        0        0     1241 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/fgt/get_commands.py
+-rw-r--r--   0        0        0     3547 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/fgt/main.py
+-rw-r--r--   0        0        0     3951 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/fgt/monitor_commands.py
+-rw-r--r--   0        0        0       20 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/fmg/__init__.py
+-rw-r--r--   0        0        0     2631 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/fmg/get_commands.py
+-rw-r--r--   0        0        0     2394 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/fmg/main.py
+-rw-r--r--   0        0        0     1802 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/get.py
+-rw-r--r--   0        0        0     4825 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/cli/main.py
+-rw-r--r--   0        0        0      196 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/exceptions/__init__.py
+-rw-r--r--   0        0        0     1966 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/exceptions/exceptions.py
+-rw-r--r--   0        0        0      423 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/fortinet/__init__.py
+-rw-r--r--   0        0        0    13927 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/fortinet/convert.py
+-rw-r--r--   0        0        0     1023 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/fortinet/fortianalyzer.py
+-rw-r--r--   0        0        0     5602 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/fortinet/forticlientems.py
+-rw-r--r--   0        0        0     2961 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/fortinet/fortigate.py
+-rw-r--r--   0        0        0    11488 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/fortinet/fortigate_config.py
+-rw-r--r--   0        0        0     8714 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/fortinet/fortigate_config_check.py
+-rw-r--r--   0        0        0      584 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/fortinet/fortigate_info.py
+-rw-r--r--   0        0        0    12434 2023-08-03 11:04:57.686871 fotoobo-1.0.1/fotoobo/fortinet/fortimanager.py
+-rw-r--r--   0        0        0     6431 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/fortinet/fortinet.py
+-rw-r--r--   0        0        0      322 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/helpers/__init__.py
+-rw-r--r--   0        0        0     1227 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/helpers/cli.py
+-rw-r--r--   0        0        0     3617 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/helpers/config.py
+-rw-r--r--   0        0        0     5408 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/helpers/files.py
+-rw-r--r--   0        0        0    10994 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/helpers/log.py
+-rw-r--r--   0        0        0     4958 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/helpers/output.py
+-rw-r--r--   0        0        0    10362 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/helpers/result.py
+-rw-r--r--   0        0        0      128 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/inventory/__init__.py
+-rw-r--r--   0        0        0      568 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/inventory/generic.py
+-rw-r--r--   0        0        0     5203 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/inventory/inventory.py
+-rwxr-xr-x   0        0        0     1359 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/main.py
+-rw-r--r--   0        0        0      428 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/__init__.py
+-rw-r--r--   0        0        0     1284 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/convert.py
+-rw-r--r--   0        0        0       92 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/ems/__init__.py
+-rw-r--r--   0        0        0     1626 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/ems/get.py
+-rw-r--r--   0        0        0     8338 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/ems/monitor.py
+-rw-r--r--   0        0        0       56 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/faz/__init__.py
+-rw-r--r--   0        0        0      809 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/faz/get.py
+-rw-r--r--   0        0        0      129 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/fgt/__init__.py
+-rw-r--r--   0        0        0     4619 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/fgt/config.py
+-rw-r--r--   0        0        0     2377 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/fgt/get.py
+-rw-r--r--   0        0        0     2978 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/fgt/main.py
+-rw-r--r--   0        0        0     4274 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/fgt/monitor.py
+-rw-r--r--   0        0        0      105 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/fmg/__init__.py
+-rw-r--r--   0        0        0     4417 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/fmg/get.py
+-rw-r--r--   0        0        0     2733 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/fmg/main.py
+-rw-r--r--   0        0        0     1882 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/get.py
+-rw-r--r--   0        0        0     1306 2023-08-03 11:04:57.690871 fotoobo-1.0.1/fotoobo/tools/greet.py
+-rw-r--r--   0        0        0     3711 2023-08-03 11:04:57.690871 fotoobo-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 fotoobo-1.0.1/PKG-INFO
```

### Comparing `fotoobo-1.0.0/LICENSE` & `fotoobo-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/README.md` & `fotoobo-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/cli/convert.py` & `fotoobo-1.0.1/fotoobo/cli/convert.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/cli/ems/get_commands.py` & `fotoobo-1.0.1/fotoobo/cli/ems/get_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/cli/ems/main.py` & `fotoobo-1.0.1/fotoobo/cli/ems/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/cli/ems/monitor_commands.py` & `fotoobo-1.0.1/fotoobo/cli/ems/monitor_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/cli/faz/get_commands.py` & `fotoobo-1.0.1/fotoobo/cli/faz/get_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/cli/faz/main.py` & `fotoobo-1.0.1/fotoobo/cli/faz/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/cli/fgt/config_commands.py` & `fotoobo-1.0.1/fotoobo/cli/fgt/config_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/cli/fgt/get_commands.py` & `fotoobo-1.0.1/fotoobo/cli/fgt/get_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/cli/fgt/main.py` & `fotoobo-1.0.1/fotoobo/cli/fgt/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/cli/fgt/monitor_commands.py` & `fotoobo-1.0.1/fotoobo/cli/fgt/monitor_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/cli/fmg/get_commands.py` & `fotoobo-1.0.1/fotoobo/cli/fmg/get_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/cli/fmg/main.py` & `fotoobo-1.0.1/fotoobo/cli/fmg/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/cli/get.py` & `fotoobo-1.0.1/fotoobo/cli/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/cli/main.py` & `fotoobo-1.0.1/fotoobo/cli/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/exceptions/exceptions.py` & `fotoobo-1.0.1/fotoobo/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/fortinet/convert.py` & `fotoobo-1.0.1/fotoobo/fortinet/convert.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/fortinet/fortianalyzer.py` & `fotoobo-1.0.1/fotoobo/fortinet/fortianalyzer.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/fortinet/forticlientems.py` & `fotoobo-1.0.1/fotoobo/fortinet/forticlientems.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/fortinet/fortigate.py` & `fotoobo-1.0.1/fotoobo/fortinet/fortigate.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/fortinet/fortigate_config.py` & `fotoobo-1.0.1/fotoobo/fortinet/fortigate_config.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/fortinet/fortigate_config_check.py` & `fotoobo-1.0.1/fotoobo/fortinet/fortigate_config_check.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/fortinet/fortigate_info.py` & `fotoobo-1.0.1/fotoobo/fortinet/fortigate_info.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/fortinet/fortimanager.py` & `fotoobo-1.0.1/fotoobo/fortinet/fortimanager.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/fortinet/fortinet.py` & `fotoobo-1.0.1/fotoobo/fortinet/fortinet.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/helpers/cli.py` & `fotoobo-1.0.1/fotoobo/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/helpers/config.py` & `fotoobo-1.0.1/fotoobo/helpers/config.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/helpers/files.py` & `fotoobo-1.0.1/fotoobo/helpers/files.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/helpers/log.py` & `fotoobo-1.0.1/fotoobo/helpers/log.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/helpers/output.py` & `fotoobo-1.0.1/fotoobo/helpers/output.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/helpers/result.py` & `fotoobo-1.0.1/fotoobo/helpers/result.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/inventory/generic.py` & `fotoobo-1.0.1/fotoobo/inventory/generic.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/inventory/inventory.py` & `fotoobo-1.0.1/fotoobo/inventory/inventory.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/main.py` & `fotoobo-1.0.1/fotoobo/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/tools/convert.py` & `fotoobo-1.0.1/fotoobo/tools/convert.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/tools/ems/get.py` & `fotoobo-1.0.1/fotoobo/tools/ems/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/tools/ems/monitor.py` & `fotoobo-1.0.1/fotoobo/tools/ems/monitor.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/tools/faz/get.py` & `fotoobo-1.0.1/fotoobo/tools/faz/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/tools/fgt/config.py` & `fotoobo-1.0.1/fotoobo/tools/fgt/config.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/tools/fgt/get.py` & `fotoobo-1.0.1/fotoobo/tools/fgt/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/tools/fgt/main.py` & `fotoobo-1.0.1/fotoobo/tools/fgt/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/tools/fgt/monitor.py` & `fotoobo-1.0.1/fotoobo/tools/fgt/monitor.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/tools/fmg/get.py` & `fotoobo-1.0.1/fotoobo/tools/fmg/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/tools/fmg/main.py` & `fotoobo-1.0.1/fotoobo/tools/fmg/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/tools/get.py` & `fotoobo-1.0.1/fotoobo/tools/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/fotoobo/tools/greet.py` & `fotoobo-1.0.1/fotoobo/tools/greet.py`

 * *Files identical despite different names*

### Comparing `fotoobo-1.0.0/pyproject.toml` & `fotoobo-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fotoobo"
-version = "1.0.0"
+version = "1.0.1"
 description = "The awesome Fortinet Toolbox"
 authors = ["Patrik Spiess <patrik.spiess@mgb.ch>", "Lukas Murer-Jäckle <lukas.murer@mgb.ch>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.0, <3.12"
 typer = "~0.6.0"
```

### Comparing `fotoobo-1.0.0/PKG-INFO` & `fotoobo-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fotoobo
-Version: 1.0.0
+Version: 1.0.1
 Summary: The awesome Fortinet Toolbox
 Author: Patrik Spiess
 Author-email: patrik.spiess@mgb.ch
 Requires-Python: >=3.8.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

