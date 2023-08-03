# Comparing `tmp/nonebot-plugin-chatgpt-plus-0.8.7.tar.gz` & `tmp/nonebot-plugin-chatgpt-plus-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-plus-0.8.7.tar", last modified: Fri Jun  9 07:40:42 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-plus-0.8.8.tar", last modified: Thu Aug  3 08:41:30 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-plus-0.8.7.tar` & `nonebot-plugin-chatgpt-plus-0.8.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-06-09 07:40:33.678234 nonebot-plugin-chatgpt-plus-0.8.7/LICENSE
--rw-r--r--   0        0        0     7068 2023-06-09 07:40:33.678234 nonebot-plugin-chatgpt-plus-0.8.7/README.md
--rw-r--r--   0        0        0    13921 2023-06-09 07:40:33.678234 nonebot-plugin-chatgpt-plus-0.8.7/nonebot_plugin_chatgpt_plus/__init__.py
--rw-r--r--   0        0        0    15430 2023-06-09 07:40:33.678234 nonebot-plugin-chatgpt-plus-0.8.7/nonebot_plugin_chatgpt_plus/chatgpt.py
--rw-r--r--   0        0        0     1152 2023-06-09 07:40:33.678234 nonebot-plugin-chatgpt-plus-0.8.7/nonebot_plugin_chatgpt_plus/config.py
--rw-r--r--   0        0        0      900 2023-06-09 07:40:33.678234 nonebot-plugin-chatgpt-plus-0.8.7/nonebot_plugin_chatgpt_plus/data.py
--rw-r--r--   0        0        0     5678 2023-06-09 07:40:33.678234 nonebot-plugin-chatgpt-plus-0.8.7/nonebot_plugin_chatgpt_plus/utils.py
--rw-r--r--   0        0        0      725 2023-06-09 07:40:33.678234 nonebot-plugin-chatgpt-plus-0.8.7/pyproject.toml
--rw-r--r--   0        0        0     7465 1970-01-01 00:00:00.000000 nonebot-plugin-chatgpt-plus-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-03 08:41:22.929958 nonebot-plugin-chatgpt-plus-0.8.8/LICENSE
+-rw-r--r--   0        0        0     7068 2023-08-03 08:41:22.929958 nonebot-plugin-chatgpt-plus-0.8.8/README.md
+-rw-r--r--   0        0        0    13921 2023-08-03 08:41:22.929958 nonebot-plugin-chatgpt-plus-0.8.8/nonebot_plugin_chatgpt_plus/__init__.py
+-rw-r--r--   0        0        0    15473 2023-08-03 08:41:22.929958 nonebot-plugin-chatgpt-plus-0.8.8/nonebot_plugin_chatgpt_plus/chatgpt.py
+-rw-r--r--   0        0        0     1152 2023-08-03 08:41:22.929958 nonebot-plugin-chatgpt-plus-0.8.8/nonebot_plugin_chatgpt_plus/config.py
+-rw-r--r--   0        0        0      900 2023-08-03 08:41:22.929958 nonebot-plugin-chatgpt-plus-0.8.8/nonebot_plugin_chatgpt_plus/data.py
+-rw-r--r--   0        0        0     5678 2023-08-03 08:41:22.929958 nonebot-plugin-chatgpt-plus-0.8.8/nonebot_plugin_chatgpt_plus/utils.py
+-rw-r--r--   0        0        0      725 2023-08-03 08:41:22.929958 nonebot-plugin-chatgpt-plus-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0     7465 1970-01-01 00:00:00.000000 nonebot-plugin-chatgpt-plus-0.8.8/PKG-INFO
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.7/LICENSE` & `nonebot-plugin-chatgpt-plus-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-plus-0.8.7/README.md` & `nonebot-plugin-chatgpt-plus-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-plus-0.8.7/nonebot_plugin_chatgpt_plus/__init__.py` & `nonebot-plugin-chatgpt-plus-0.8.8/nonebot_plugin_chatgpt_plus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 查看人格/查询人格 + 名称   查看已有的人格预设（超级用户）
 人格设定/设置人格 + 名称 + 人格信息 编辑人格信息（超级用户）
 刷新token   强制刷新token（超级用户）""",
     extra={
         "unique_name": "chatgpt-plus",
         "example": """@bot 人格设定 香草""",
         "author": "A-kirami",
-        "version": "0.8.7",
+        "version": "0.8.8",
     },
 )
 __plugin_settings__ = {
     "level": 5,
     "default_status": True,
     "limit_superuser": False,
     "cmd": [
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.7/nonebot_plugin_chatgpt_plus/chatgpt.py` & `nonebot-plugin-chatgpt-plus-0.8.8/nonebot_plugin_chatgpt_plus/chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
                                 try:
                                     data_list.append(json.loads(data))
                                 except Exception as e:
                                     logger.warning(f"ChatGPT数据解析未知错误：{e}: {data}")
                     if not data_list:
                         return "ChatGPT 服务器未返回任何内容"
                     idx = -1
-                    while data_list[idx]["error"]:
+                    while data_list[idx].get("error") or data_list[idx].get("is_completion"):
                         idx -= 1
                     response = data_list[idx]
                 self.parent_id = response["message"]["id"]
                 self.conversation_id = response["conversation_id"]
                 not_complete = ""
                 if not response["message"].get("end_turn", True):
                     if self.auto_continue:
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.7/nonebot_plugin_chatgpt_plus/config.py` & `nonebot-plugin-chatgpt-plus-0.8.8/nonebot_plugin_chatgpt_plus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-plus-0.8.7/nonebot_plugin_chatgpt_plus/data.py` & `nonebot-plugin-chatgpt-plus-0.8.8/nonebot_plugin_chatgpt_plus/data.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-plus-0.8.7/nonebot_plugin_chatgpt_plus/utils.py` & `nonebot-plugin-chatgpt-plus-0.8.8/nonebot_plugin_chatgpt_plus/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-plus-0.8.7/pyproject.toml` & `nonebot-plugin-chatgpt-plus-0.8.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-chatgpt-plus"
-version = "0.8.7"
+version = "0.8.8"
 description = "NoneBot2 plugin for AI chat"
 authors = [
     { name = "Akirami", email = "Akiramiaya@outlook.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc2",
     "nonebot-adapter-onebot>=2.1.5",
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.7/PKG-INFO` & `nonebot-plugin-chatgpt-plus-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-plus
-Version: 0.8.7
+Version: 0.8.8
 Summary: NoneBot2 plugin for AI chat
 License: MIT
 Author-email: Akirami <Akiramiaya@outlook.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/AkashiCoin/nonebot-plugin-chatgpt-plus
 Project-URL: Repository, https://github.com/AkashiCoin/nonebot-plugin-chatgpt-plus
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-chatgpt-plus Version: 0.8.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-chatgpt-plus Version: 0.8.8 Summary:
 NoneBot2 plugin for AI chat License: MIT Author-email: Akirami
 outlook.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 AkashiCoin/nonebot-plugin-chatgpt-plus Project-URL: Repository, https://
 github.com/AkashiCoin/nonebot-plugin-chatgpt-plus Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
```

