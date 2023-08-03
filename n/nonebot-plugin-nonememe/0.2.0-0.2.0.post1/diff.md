# Comparing `tmp/nonebot_plugin_nonememe-0.2.0.tar.gz` & `tmp/nonebot_plugin_nonememe-0.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nonememe-0.2.0.tar", last modified: Thu Aug  3 10:49:39 2023, max compression
+gzip compressed data, was "nonebot_plugin_nonememe-0.2.0.post1.tar", last modified: Thu Aug  3 14:04:28 2023, max compression
```

## Comparing `nonebot_plugin_nonememe-0.2.0.tar` & `nonebot_plugin_nonememe-0.2.0.post1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-08-03 10:49:24.605922 nonebot_plugin_nonememe-0.2.0/LICENSE
--rw-r--r--   0        0        0     3613 2023-08-03 10:49:24.605922 nonebot_plugin_nonememe-0.2.0/README.md
--rw-r--r--   0        0        0      891 2023-08-03 10:49:24.605922 nonebot_plugin_nonememe-0.2.0/nonebot_plugin_nonememe/__init__.py
--rw-r--r--   0        0        0     2240 2023-08-03 10:49:24.605922 nonebot_plugin_nonememe-0.2.0/nonebot_plugin_nonememe/__main__.py
--rw-r--r--   0        0        0      842 2023-08-03 10:49:24.605922 nonebot_plugin_nonememe-0.2.0/nonebot_plugin_nonememe/config.py
--rw-r--r--   0        0        0     3282 2023-08-03 10:49:24.605922 nonebot_plugin_nonememe-0.2.0/nonebot_plugin_nonememe/data_source.py
--rw-r--r--   0        0        0      728 2023-08-03 10:49:39.554132 nonebot_plugin_nonememe-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 nonebot_plugin_nonememe-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-03 14:04:12.691332 nonebot_plugin_nonememe-0.2.0.post1/LICENSE
+-rw-r--r--   0        0        0     3613 2023-08-03 14:04:12.691332 nonebot_plugin_nonememe-0.2.0.post1/README.md
+-rw-r--r--   0        0        0      891 2023-08-03 14:04:12.691332 nonebot_plugin_nonememe-0.2.0.post1/nonebot_plugin_nonememe/__init__.py
+-rw-r--r--   0        0        0     2240 2023-08-03 14:04:12.691332 nonebot_plugin_nonememe-0.2.0.post1/nonebot_plugin_nonememe/__main__.py
+-rw-r--r--   0        0        0      842 2023-08-03 14:04:12.691332 nonebot_plugin_nonememe-0.2.0.post1/nonebot_plugin_nonememe/config.py
+-rw-r--r--   0        0        0     3282 2023-08-03 14:04:12.691332 nonebot_plugin_nonememe-0.2.0.post1/nonebot_plugin_nonememe/data_source.py
+-rw-r--r--   0        0        0      734 2023-08-03 14:04:28.635323 nonebot_plugin_nonememe-0.2.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     4309 1970-01-01 00:00:00.000000 nonebot_plugin_nonememe-0.2.0.post1/PKG-INFO
```

### Comparing `nonebot_plugin_nonememe-0.2.0/LICENSE` & `nonebot_plugin_nonememe-0.2.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nonememe-0.2.0/README.md` & `nonebot_plugin_nonememe-0.2.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nonememe-0.2.0/nonebot_plugin_nonememe/__init__.py` & `nonebot_plugin_nonememe-0.2.0.post1/nonebot_plugin_nonememe/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nonememe-0.2.0/nonebot_plugin_nonememe/__main__.py` & `nonebot_plugin_nonememe-0.2.0.post1/nonebot_plugin_nonememe/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nonememe-0.2.0/nonebot_plugin_nonememe/config.py` & `nonebot_plugin_nonememe-0.2.0.post1/nonebot_plugin_nonememe/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Optional, TypedDict, Union
-from typing_extensions import NotRequired
+from typing import Optional, Union
+from typing_extensions import NotRequired, TypedDict
 
 from nonebot import get_driver
 from pydantic import BaseModel
 
 
 class CronDict(TypedDict):
     year: NotRequired[Union[str, int]]
```

### Comparing `nonebot_plugin_nonememe-0.2.0/nonebot_plugin_nonememe/data_source.py` & `nonebot_plugin_nonememe-0.2.0.post1/nonebot_plugin_nonememe/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nonememe-0.2.0/pyproject.toml` & `nonebot_plugin_nonememe-0.2.0.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-nonememe"
-version = "0.2.0"
+version = "0.2.0.post1"
 description = "The daily life of the NoneBot group members"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-plugin-send-anything-anywhere>=0.2.7",
```

### Comparing `nonebot_plugin_nonememe-0.2.0/PKG-INFO` & `nonebot_plugin_nonememe-0.2.0.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nonememe
-Version: 0.2.0
+Version: 0.2.0.post1
 Summary: The daily life of the NoneBot group members
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-nonememe
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-nonememe
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nonememe Version: 0.2.0 Summary: The
-daily life of the NoneBot group members Home-page: https://github.com/lgc-
-NB2Dev/nonebot-plugin-nonememe Author-Email: student_2333
+Metadata-Version: 2.1 Name: nonebot-plugin-nonememe Version: 0.2.0.post1
+Summary: The daily life of the NoneBot group members Home-page: https://
+github.com/lgc-NB2Dev/nonebot-plugin-nonememe Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-nonememe Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.7
 Requires-Dist: nonebot-plugin-apscheduler>=0.3.0 Requires-Dist:
 pydantic<2,>=1.10.4 Requires-Dist: httpx>=0.24.1 Requires-Dist: json5>=0.9.14
 Requires-Dist: anyio>=3.7.1 Requires-Dist: typing-extensions>=4.7.1
 Description-Content-Type: text/markdown
```

