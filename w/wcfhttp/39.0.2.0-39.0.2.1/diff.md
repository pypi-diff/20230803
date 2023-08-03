# Comparing `tmp/wcfhttp-39.0.2.0.tar.gz` & `tmp/wcfhttp-39.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcfhttp-39.0.2.0.tar", last modified: Sun Jul 16 16:25:43 2023, max compression
+gzip compressed data, was "wcfhttp-39.0.2.1.tar", last modified: Tue Aug  1 15:52:46 2023, max compression
```

## Comparing `wcfhttp-39.0.2.0.tar` & `wcfhttp-39.0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 16:25:43.951925 wcfhttp-39.0.2.0/
--rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-39.0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1842 2023-07-16 16:25:43.951925 wcfhttp-39.0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-16 16:25:43.951925 wcfhttp-39.0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1421 2023-07-16 16:22:36.000000 wcfhttp-39.0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 16:25:43.936301 wcfhttp-39.0.2.0/wcfhttp/
--rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-39.0.2.0/wcfhttp/__init__.py
--rw-rw-rw-   0        0        0    16617 2023-07-16 16:22:36.000000 wcfhttp-39.0.2.0/wcfhttp/core.py
--rw-rw-rw-   0        0        0     2317 2023-07-15 02:26:29.000000 wcfhttp-39.0.2.0/wcfhttp/main.py
-drwxrwxrwx   0        0        0        0 2023-07-16 16:25:43.936301 wcfhttp-39.0.2.0/wcfhttp.egg-info/
--rw-rw-rw-   0        0        0     1842 2023-07-16 16:25:43.000000 wcfhttp-39.0.2.0/wcfhttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-07-16 16:25:43.000000 wcfhttp-39.0.2.0/wcfhttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 16:25:43.000000 wcfhttp-39.0.2.0/wcfhttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-16 16:25:43.000000 wcfhttp-39.0.2.0/wcfhttp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-07-16 16:25:43.000000 wcfhttp-39.0.2.0/wcfhttp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-16 16:25:43.000000 wcfhttp-39.0.2.0/wcfhttp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 15:52:46.542627 wcfhttp-39.0.2.1/
+-rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-39.0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1842 2023-08-01 15:52:46.541626 wcfhttp-39.0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-01 15:52:46.543626 wcfhttp-39.0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1421 2023-08-01 15:52:42.000000 wcfhttp-39.0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:52:46.527628 wcfhttp-39.0.2.1/wcfhttp/
+-rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-39.0.2.1/wcfhttp/__init__.py
+-rw-rw-rw-   0        0        0    16629 2023-08-01 15:51:46.000000 wcfhttp-39.0.2.1/wcfhttp/core.py
+-rw-rw-rw-   0        0        0     2317 2023-07-15 02:26:29.000000 wcfhttp-39.0.2.1/wcfhttp/main.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:52:46.539624 wcfhttp-39.0.2.1/wcfhttp.egg-info/
+-rw-rw-rw-   0        0        0     1842 2023-08-01 15:52:46.000000 wcfhttp-39.0.2.1/wcfhttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-08-01 15:52:46.000000 wcfhttp-39.0.2.1/wcfhttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 15:52:46.000000 wcfhttp-39.0.2.1/wcfhttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-01 15:52:46.000000 wcfhttp-39.0.2.1/wcfhttp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-08-01 15:52:46.000000 wcfhttp-39.0.2.1/wcfhttp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-01 15:52:46.000000 wcfhttp-39.0.2.1/wcfhttp.egg-info/top_level.txt
```

### Comparing `wcfhttp-39.0.2.0/PKG-INFO` & `wcfhttp-39.0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 39.0.2.0
+Version: 39.0.2.1
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

### Comparing `wcfhttp-39.0.2.0/setup.py` & `wcfhttp-39.0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             'wcfhttp=wcfhttp.main:main'
         ]
     },
     install_requires=[
         "setuptools",
         "fastapi",
         "uvicorn[standard]",
-        "wcferry>=39.0.2.0",
+        "wcferry>=39.0.2.1",
     ],
     classifiers=[
         "Environment :: Win32 (MS Windows)",
         "Intended Audience :: Developers",
         "Intended Audience :: Customer Service",
         "Topic :: Communications :: Chat",
         "Operating System :: Microsoft :: Windows",
```

### Comparing `wcfhttp-39.0.2.0/wcfhttp/core.py` & `wcfhttp-39.0.2.1/wcfhttp/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Any
 
 import requests
 from fastapi import Body, Query, FastAPI
 from pydantic import BaseModel
 from wcferry import Wcf, WxMsg
 
-__version__ = "39.0.2.0"
+__version__ = "39.0.2.1"
 
 
 class Msg(BaseModel):
     id: int
     ts: int
     sign: str
     type: int
@@ -78,15 +78,15 @@
         data["thumb"] = msg.thumb
         data["extra"] = msg.extra
         data["is_at"] = msg.is_at(self.wcf.self_wxid)
         data["is_self"] = msg.from_self()
         data["is_group"] = msg.from_group()
 
         try:
-            rsp = requests.post(url=cb, json=data)
+            rsp = requests.post(url=cb, json=data, timeout=30)
             if rsp.status_code != 200:
                 self.LOG.error(f"消息转发失败，HTTP 状态码为: {rsp.status_code}")
         except Exception as e:
             self.LOG.error(f"消息转发异常: {e}")
 
     def _set_cb(self, cb):
         def callback(wcf: Wcf):
```

### Comparing `wcfhttp-39.0.2.0/wcfhttp/main.py` & `wcfhttp-39.0.2.1/wcfhttp/main.py`

 * *Files identical despite different names*

### Comparing `wcfhttp-39.0.2.0/wcfhttp.egg-info/PKG-INFO` & `wcfhttp-39.0.2.1/wcfhttp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 39.0.2.0
+Version: 39.0.2.1
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

