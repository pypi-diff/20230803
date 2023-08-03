# Comparing `tmp/nonebot_plugin_blocker-0.3.8.tar.gz` & `tmp/nonebot_plugin_blocker-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blocker-0.3.8.tar", last modified: Wed Aug  2 20:11:07 2023, max compression
+gzip compressed data, was "nonebot_plugin_blocker-0.3.9.tar", last modified: Wed Aug  2 21:15:15 2023, max compression
```

## Comparing `nonebot_plugin_blocker-0.3.8.tar` & `nonebot_plugin_blocker-0.3.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-08-02 20:10:51.280478 nonebot_plugin_blocker-0.3.8/LICENSE
--rw-r--r--   0        0        0     2950 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/README.md
--rw-r--r--   0        0        0      381 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0        0        0     3242 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0        0        0     3928 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/config.py
--rw-r--r--   0        0        0     2709 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/__init__.py
--rw-r--r--   0        0        0     3208 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/webpage/main.html
--rw-r--r--   0        0        0     6180 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/webpage/main.js
--rw-r--r--   0        0        0     2292 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/webpage/style.css
--rw-r--r--   0        0        0      640 2023-08-02 20:11:07.584829 nonebot_plugin_blocker-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     4560 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-02 21:14:56.991885 nonebot_plugin_blocker-0.3.9/LICENSE
+-rw-r--r--   0        0        0     2950 2023-08-02 21:14:56.991885 nonebot_plugin_blocker-0.3.9/README.md
+-rw-r--r--   0        0        0      381 2023-08-02 21:14:56.991885 nonebot_plugin_blocker-0.3.9/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0        0        0     3242 2023-08-02 21:14:56.991885 nonebot_plugin_blocker-0.3.9/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0        0        0     3926 2023-08-02 21:14:56.991885 nonebot_plugin_blocker-0.3.9/nonebot_plugin_blocker/config.py
+-rw-r--r--   0        0        0     2709 2023-08-02 21:14:56.991885 nonebot_plugin_blocker-0.3.9/nonebot_plugin_blocker/web/__init__.py
+-rw-r--r--   0        0        0     3208 2023-08-02 21:14:56.991885 nonebot_plugin_blocker-0.3.9/nonebot_plugin_blocker/web/webpage/main.html
+-rw-r--r--   0        0        0     6180 2023-08-02 21:14:56.991885 nonebot_plugin_blocker-0.3.9/nonebot_plugin_blocker/web/webpage/main.js
+-rw-r--r--   0        0        0     2292 2023-08-02 21:14:56.991885 nonebot_plugin_blocker-0.3.9/nonebot_plugin_blocker/web/webpage/style.css
+-rw-r--r--   0        0        0      640 2023-08-02 21:15:15.943989 nonebot_plugin_blocker-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4560 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.9/PKG-INFO
```

### Comparing `nonebot_plugin_blocker-0.3.8/LICENSE` & `nonebot_plugin_blocker-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.8/README.md` & `nonebot_plugin_blocker-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/__main__.py` & `nonebot_plugin_blocker-0.3.9/nonebot_plugin_blocker/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/config.py` & `nonebot_plugin_blocker-0.3.9/nonebot_plugin_blocker/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         except:
             logger.info("[Blocker]Add Blocker Failed.")
 
     def del_blocker(self,gid: int, uin: str):
         try:
             self.blocklist.get(uin).remove(gid)
             logger.info("[Blocker]Delete Blocker Successful.")
-        except (AttributeError,ValueError):
+        except (AttributeError,KeyError):
             logger.info("[Blocker]Delete Blocker Failed.")
     
     def change_blocker_type(self,uin: str, val: bool = False):
         try:
             self.blocker_type[uin] = val
         except KeyError:
             self.blocker_type.setdefault(uin, val)
```

### Comparing `nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/__init__.py` & `nonebot_plugin_blocker-0.3.9/nonebot_plugin_blocker/web/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/webpage/main.html` & `nonebot_plugin_blocker-0.3.9/nonebot_plugin_blocker/web/webpage/main.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/webpage/main.js` & `nonebot_plugin_blocker-0.3.9/nonebot_plugin_blocker/web/webpage/main.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/webpage/style.css` & `nonebot_plugin_blocker-0.3.9/nonebot_plugin_blocker/web/webpage/style.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.8/pyproject.toml` & `nonebot_plugin_blocker-0.3.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-blocker"
-version = "0.3.8"
+version = "0.3.9"
 description = "Message Blocker"
 authors = [
     { name = "MerCuJerry", email = "mercujerry@gmail.com" },
 ]
 keywords = [
     "nonebot",
     "nonebot2",
```

### Comparing `nonebot_plugin_blocker-0.3.8/PKG-INFO` & `nonebot_plugin_blocker-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.3.8
+Version: 0.3.9
 Summary: Message Blocker
 Keywords: nonebot nonebot2 qqbot bot
 Home-page: https://github.com/MerCuJerry/nonebot-plugin-blocker
 Author-Email: MerCuJerry <mercujerry@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 MerCuJerry
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.9 Summary:
 Message Blocker Keywords: nonebot nonebot2 qqbot bot Home-page: https://
 github.com/MerCuJerry/nonebot-plugin-blocker Author-Email: MerCuJerry
 gmail.com> License: MIT License Copyright (c) 2023 MerCuJerry Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

