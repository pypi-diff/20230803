# Comparing `tmp/nonebot_plugin_csornament-0.1.1.tar.gz` & `tmp/nonebot_plugin_csornament-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_csornament-0.1.1.tar", last modified: Thu Aug  3 15:33:18 2023, max compression
+gzip compressed data, was "nonebot_plugin_csornament-0.1.2.tar", last modified: Thu Aug  3 16:05:51 2023, max compression
```

## Comparing `nonebot_plugin_csornament-0.1.1.tar` & `nonebot_plugin_csornament-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2023-08-03 15:33:09.351118 nonebot_plugin_csornament-0.1.1/LICENSE
--rw-r--r--   0        0        0     2377 2023-08-03 15:33:09.351118 nonebot_plugin_csornament-0.1.1/README.md
--rw-r--r--   0        0        0     6187 2023-08-03 15:33:09.351118 nonebot_plugin_csornament-0.1.1/nonebot_plugin_csornament/__init__.py
--rw-r--r--   0        0        0      114 2023-08-03 15:33:09.351118 nonebot_plugin_csornament-0.1.1/nonebot_plugin_csornament/config.py
--rw-r--r--   0        0        0      432 2023-08-03 15:33:18.722963 nonebot_plugin_csornament-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 nonebot_plugin_csornament-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-03 16:05:43.900146 nonebot_plugin_csornament-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2377 2023-08-03 16:05:43.900146 nonebot_plugin_csornament-0.1.2/README.md
+-rw-r--r--   0        0        0     6187 2023-08-03 16:05:43.900146 nonebot_plugin_csornament-0.1.2/nonebot_plugin_csornament/__init__.py
+-rw-r--r--   0        0        0      114 2023-08-03 16:05:43.900146 nonebot_plugin_csornament-0.1.2/nonebot_plugin_csornament/config.py
+-rw-r--r--   0        0        0      453 2023-08-03 16:05:51.408127 nonebot_plugin_csornament-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2725 1970-01-01 00:00:00.000000 nonebot_plugin_csornament-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_csornament-0.1.1/LICENSE` & `nonebot_plugin_csornament-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_csornament-0.1.1/README.md` & `nonebot_plugin_csornament-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_csornament-0.1.1/nonebot_plugin_csornament/__init__.py` & `nonebot_plugin_csornament-0.1.2/nonebot_plugin_csornament/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_csornament-0.1.1/PKG-INFO` & `nonebot_plugin_csornament-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_csornament
-Version: 0.1.1
+Version: 0.1.2
 Summary: nonebot社区插件，查询CSGO饰品
 Author-Email: Sydrr0 <2562312527@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: lxml>=4.9.3
 Requires-Dist: bs4>=0.0.1
 Requires-Dist: nonebot2>=2.0.1
+Requires-Dist: httpx>=0.23.3
 Description-Content-Type: text/markdown
 
 <div align="center">
 
   <a href="https://v2.nonebot.dev/">
     <img src="https://pic.imgdb.cn/item/64ca75781ddac507ccf21163.webp">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_csornament Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_csornament Version: 0.1.2 Summary:
 nonebotç¤¾åºæä»¶ï¼æ¥è¯¢CSGOé¥°å Author-Email: Sydrr0 <2562312527@qq.com>
 License: MIT Requires-Python: >=3.8 Requires-Dist: lxml>=4.9.3 Requires-Dist:
-bs4>=0.0.1 Requires-Dist: nonebot2>=2.0.1 Description-Content-Type: text/
-markdown
+bs4>=0.0.1 Requires-Dist: nonebot2>=2.0.1 Requires-Dist: httpx>=0.23.3
+Description-Content-Type: text/markdown
            [https://pic.imgdb.cn/item/64ca75781ddac507ccf21163.webp]
               _ð¼å¥½çåï¼å¥½ççè¯å°±ç¹ä¸ªâ­å§ï¼è¿
 (~å§å§~)å¯ä»¥ç»äºä½èæå¤§çå¨åå¦ð¼_ # nonebot-plugin-csornament
            _â¨ [Nonebot2](https://githubfast.com/nonebot/nonebot2)
   æä»¶ï¼æ¥ææ¨çé¥°åæ¥è¯¢æºå¨äºº â¨_ ![tip](https://badgen.net/
    badge/python/3.8+/orange?i) ![tip](https://badgen.net/badge/windows/10+/
 green?i) ![tip](https://badgen.net/badge/ubuntu/20.04+/pink?i) ![tip](https://
```

