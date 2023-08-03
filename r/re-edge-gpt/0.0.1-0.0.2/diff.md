# Comparing `tmp/re_edge_gpt-0.0.1.tar.gz` & `tmp/re_edge_gpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re_edge_gpt-0.0.1.tar", last modified: Wed Aug  2 07:09:11 2023, max compression
+gzip compressed data, was "re_edge_gpt-0.0.2.tar", last modified: Thu Aug  3 11:00:37 2023, max compression
```

## Comparing `re_edge_gpt-0.0.1.tar` & `re_edge_gpt-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 07:09:11.470560 re_edge_gpt-0.0.1/
--rw-rw-rw-   0        0        0     1085 2023-06-22 06:27:17.000000 re_edge_gpt-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     5862 2023-08-02 07:09:11.469578 re_edge_gpt-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5140 2023-08-02 06:55:43.000000 re_edge_gpt-0.0.1/README.md
--rw-rw-rw-   0        0        0     1103 2023-08-02 07:06:14.000000 re_edge_gpt-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-08-02 07:09:11.431458 re_edge_gpt-0.0.1/re_edge_gpt/
--rw-rw-rw-   0        0        0      154 2023-08-02 06:42:08.000000 re_edge_gpt-0.0.1/re_edge_gpt/__init__.py
--rw-rw-rw-   0        0        0     9541 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.1/re_edge_gpt/chathub.py
--rw-rw-rw-   0        0        0     2453 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.1/re_edge_gpt/constants.py
--rw-rw-rw-   0        0        0     4460 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.1/re_edge_gpt/conversation.py
--rw-rw-rw-   0        0        0     1256 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.1/re_edge_gpt/conversation_style.py
--rw-rw-rw-   0        0        0       46 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.1/re_edge_gpt/exceptions.py
--rw-rw-rw-   0        0        0     2247 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.1/re_edge_gpt/locale.py
--rw-rw-rw-   0        0        0     7489 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.1/re_edge_gpt/main.py
--rw-rw-rw-   0        0        0     7755 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.1/re_edge_gpt/re_edge_gpt.py
--rw-rw-rw-   0        0        0     5792 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.1/re_edge_gpt/request.py
--rw-rw-rw-   0        0        0      967 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.1/re_edge_gpt/utilities.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:09:11.468560 re_edge_gpt-0.0.1/re_edge_gpt.egg-info/
--rw-rw-rw-   0        0        0     5862 2023-08-02 07:09:11.000000 re_edge_gpt-0.0.1/re_edge_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2023-08-02 07:09:11.000000 re_edge_gpt-0.0.1/re_edge_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 07:09:11.000000 re_edge_gpt-0.0.1/re_edge_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-08-02 07:09:11.000000 re_edge_gpt-0.0.1/re_edge_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-02 07:09:11.000000 re_edge_gpt-0.0.1/re_edge_gpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 07:09:11.470560 re_edge_gpt-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 11:00:37.945272 re_edge_gpt-0.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-06-22 06:27:17.000000 re_edge_gpt-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5789 2023-08-03 11:00:37.944274 re_edge_gpt-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5065 2023-08-02 08:31:13.000000 re_edge_gpt-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1103 2023-08-03 11:00:24.000000 re_edge_gpt-0.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-03 11:00:37.917816 re_edge_gpt-0.0.2/re_edge_gpt/
+-rw-rw-rw-   0        0        0      154 2023-08-02 06:42:08.000000 re_edge_gpt-0.0.2/re_edge_gpt/__init__.py
+-rw-rw-rw-   0        0        0     9541 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.2/re_edge_gpt/chathub.py
+-rw-rw-rw-   0        0        0     2453 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.2/re_edge_gpt/constants.py
+-rw-rw-rw-   0        0        0     4460 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.2/re_edge_gpt/conversation.py
+-rw-rw-rw-   0        0        0     1256 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.2/re_edge_gpt/conversation_style.py
+-rw-rw-rw-   0        0        0       46 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.2/re_edge_gpt/exceptions.py
+-rw-rw-rw-   0        0        0     2247 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.2/re_edge_gpt/locale.py
+-rw-rw-rw-   0        0        0     7489 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.2/re_edge_gpt/main.py
+-rw-rw-rw-   0        0        0     7755 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.2/re_edge_gpt/re_edge_gpt.py
+-rw-rw-rw-   0        0        0     5792 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.2/re_edge_gpt/request.py
+-rw-rw-rw-   0        0        0      967 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.2/re_edge_gpt/utilities.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:00:37.944274 re_edge_gpt-0.0.2/re_edge_gpt.egg-info/
+-rw-rw-rw-   0        0        0     5789 2023-08-03 11:00:37.000000 re_edge_gpt-0.0.2/re_edge_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-08-03 11:00:37.000000 re_edge_gpt-0.0.2/re_edge_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 11:00:37.000000 re_edge_gpt-0.0.2/re_edge_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-08-03 11:00:37.000000 re_edge_gpt-0.0.2/re_edge_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-03 11:00:37.000000 re_edge_gpt-0.0.2/re_edge_gpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 11:00:37.945272 re_edge_gpt-0.0.2/setup.cfg
```

### Comparing `re_edge_gpt-0.0.1/LICENSE` & `re_edge_gpt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.1/PKG-INFO` & `re_edge_gpt-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re_edge_gpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Microsoft's Bing Chat AI
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Integration-Automation/ReEdgeGPT
 Project-URL: Code, https://github.com/Integration-Automation/ReEdgeGPT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -61,24 +61,24 @@
 1. Get a browser that looks like Microsoft Edge.
 2. Open [bing.com/chat](https://bing.com/chat)
 3. If you see a chat feature, you are good to continue...
 4. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
 5. Go to [bing.com](https://bing.com)
 6. Open the extension
 7. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
-8. Paste your cookies into a file `bing_cookies_*.json`.
-   - NOTE: The **cookies file name MUST follow the regex pattern `bing_cookies_*.json`**, so that they could be recognized by internal cookie processing mechanisms
+8. Paste your cookies into a file `bing_cookies.json`.
+   - NOTE: The **cookies file name MUST follow the regex pattern `bing_cookies.json`**, so that they could be recognized by internal cookie processing mechanisms
 
 ### Use cookies in code:
 
 ```python
 import json
 from re_edge_gpt import Chatbot
 
-cookies = json.loads(open("./path/to/bing_cookies.json", encoding="utf-8").read())  # might omit cookies option
+cookies = json.loads(open("./path/to/bing_cookies.json", encoding="utf-8").read())
 bot = await Chatbot.create(cookies=cookies)
 ```
 
 </details>
 
 <summary>
 
@@ -89,23 +89,21 @@
 <details open>
 
 ## Run from Command Line
 
 ```
  $ python3 -m EdgeGPT.EdgeGPT -h
 
-        EdgeGPT - A demo of reverse engineering the Bing GPT chatbot
-        Repo: github.com/acheong08/EdgeGPT
-        By: Antonio Cheong
+        re_edge_gpt - A demo of reverse engineering the Bing GPT chatbot
 
         !help for help
 
         Type !exit to exit
 
-usage: EdgeGPT.py [-h] [--enter-once] [--search-result] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK]
+usage: re_edge_gpt.py [-h] [--enter-once] [--search-result] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK]
                   [--style {creative,balanced,precise}] [--prompt PROMPT] [--cookie-file COOKIE_FILE]
                   [--history-file HISTORY_FILE] [--locale LOCALE]
 
 options:
   -h, --help            show this help message and exit
   --enter-once
   --search-result
@@ -135,15 +133,15 @@
 
 from pathlib import Path
 from re_edge_gpt import Chatbot, ConversationStyle
 
 cookies = json.loads(open(str(Path(str(Path.cwd()) + "/bing_cookies.json")), encoding="utf-8").read())
 
 async def main():
-    bot = await Chatbot.create(cookies=cookies) # Passing cookies is "optional", as explained above
+    bot = await Chatbot.create(cookies=cookies)
     response = await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative, simplify_response=True)
     print(json.dumps(response, indent=2)) # Returns
     """
 {
     "text": str,
     "author": str,
     "sources": list[dict],
@@ -155,7 +153,11 @@
     await bot.close()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 </details>
+
+---
+> Origin repo (archived): https://github.com/acheong08/EdgeGPT
+---
```

### Comparing `re_edge_gpt-0.0.1/README.md` & `re_edge_gpt-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -42,24 +42,24 @@
 1. Get a browser that looks like Microsoft Edge.
 2. Open [bing.com/chat](https://bing.com/chat)
 3. If you see a chat feature, you are good to continue...
 4. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
 5. Go to [bing.com](https://bing.com)
 6. Open the extension
 7. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
-8. Paste your cookies into a file `bing_cookies_*.json`.
-   - NOTE: The **cookies file name MUST follow the regex pattern `bing_cookies_*.json`**, so that they could be recognized by internal cookie processing mechanisms
+8. Paste your cookies into a file `bing_cookies.json`.
+   - NOTE: The **cookies file name MUST follow the regex pattern `bing_cookies.json`**, so that they could be recognized by internal cookie processing mechanisms
 
 ### Use cookies in code:
 
 ```python
 import json
 from re_edge_gpt import Chatbot
 
-cookies = json.loads(open("./path/to/bing_cookies.json", encoding="utf-8").read())  # might omit cookies option
+cookies = json.loads(open("./path/to/bing_cookies.json", encoding="utf-8").read())
 bot = await Chatbot.create(cookies=cookies)
 ```
 
 </details>
 
 <summary>
 
@@ -70,23 +70,21 @@
 <details open>
 
 ## Run from Command Line
 
 ```
  $ python3 -m EdgeGPT.EdgeGPT -h
 
-        EdgeGPT - A demo of reverse engineering the Bing GPT chatbot
-        Repo: github.com/acheong08/EdgeGPT
-        By: Antonio Cheong
+        re_edge_gpt - A demo of reverse engineering the Bing GPT chatbot
 
         !help for help
 
         Type !exit to exit
 
-usage: EdgeGPT.py [-h] [--enter-once] [--search-result] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK]
+usage: re_edge_gpt.py [-h] [--enter-once] [--search-result] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK]
                   [--style {creative,balanced,precise}] [--prompt PROMPT] [--cookie-file COOKIE_FILE]
                   [--history-file HISTORY_FILE] [--locale LOCALE]
 
 options:
   -h, --help            show this help message and exit
   --enter-once
   --search-result
@@ -116,15 +114,15 @@
 
 from pathlib import Path
 from re_edge_gpt import Chatbot, ConversationStyle
 
 cookies = json.loads(open(str(Path(str(Path.cwd()) + "/bing_cookies.json")), encoding="utf-8").read())
 
 async def main():
-    bot = await Chatbot.create(cookies=cookies) # Passing cookies is "optional", as explained above
+    bot = await Chatbot.create(cookies=cookies)
     response = await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative, simplify_response=True)
     print(json.dumps(response, indent=2)) # Returns
     """
 {
     "text": str,
     "author": str,
     "sources": list[dict],
@@ -136,7 +134,11 @@
     await bot.close()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 </details>
+
+---
+> Origin repo (archived): https://github.com/acheong08/EdgeGPT
+---
```

### Comparing `re_edge_gpt-0.0.1/pyproject.toml` & `re_edge_gpt-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "re_edge_gpt"
-version = "0.0.01"
+version = "0.0.02"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 dependencies = [
     "aiohttp", "certifi", "httpx", "prompt_toolkit", "requests", "rich"
 ]
 description = "Microsoft's Bing Chat AI"
```

### Comparing `re_edge_gpt-0.0.1/re_edge_gpt/chathub.py` & `re_edge_gpt-0.0.2/re_edge_gpt/chathub.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.1/re_edge_gpt/constants.py` & `re_edge_gpt-0.0.2/re_edge_gpt/constants.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.1/re_edge_gpt/conversation.py` & `re_edge_gpt-0.0.2/re_edge_gpt/conversation.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.1/re_edge_gpt/conversation_style.py` & `re_edge_gpt-0.0.2/re_edge_gpt/conversation_style.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.1/re_edge_gpt/locale.py` & `re_edge_gpt-0.0.2/re_edge_gpt/locale.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.1/re_edge_gpt/main.py` & `re_edge_gpt-0.0.2/re_edge_gpt/main.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.1/re_edge_gpt/re_edge_gpt.py` & `re_edge_gpt-0.0.2/re_edge_gpt/re_edge_gpt.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.1/re_edge_gpt/request.py` & `re_edge_gpt-0.0.2/re_edge_gpt/request.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.1/re_edge_gpt/utilities.py` & `re_edge_gpt-0.0.2/re_edge_gpt/utilities.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.1/re_edge_gpt.egg-info/PKG-INFO` & `re_edge_gpt-0.0.2/re_edge_gpt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-edge-gpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Microsoft's Bing Chat AI
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Integration-Automation/ReEdgeGPT
 Project-URL: Code, https://github.com/Integration-Automation/ReEdgeGPT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -61,24 +61,24 @@
 1. Get a browser that looks like Microsoft Edge.
 2. Open [bing.com/chat](https://bing.com/chat)
 3. If you see a chat feature, you are good to continue...
 4. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
 5. Go to [bing.com](https://bing.com)
 6. Open the extension
 7. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
-8. Paste your cookies into a file `bing_cookies_*.json`.
-   - NOTE: The **cookies file name MUST follow the regex pattern `bing_cookies_*.json`**, so that they could be recognized by internal cookie processing mechanisms
+8. Paste your cookies into a file `bing_cookies.json`.
+   - NOTE: The **cookies file name MUST follow the regex pattern `bing_cookies.json`**, so that they could be recognized by internal cookie processing mechanisms
 
 ### Use cookies in code:
 
 ```python
 import json
 from re_edge_gpt import Chatbot
 
-cookies = json.loads(open("./path/to/bing_cookies.json", encoding="utf-8").read())  # might omit cookies option
+cookies = json.loads(open("./path/to/bing_cookies.json", encoding="utf-8").read())
 bot = await Chatbot.create(cookies=cookies)
 ```
 
 </details>
 
 <summary>
 
@@ -89,23 +89,21 @@
 <details open>
 
 ## Run from Command Line
 
 ```
  $ python3 -m EdgeGPT.EdgeGPT -h
 
-        EdgeGPT - A demo of reverse engineering the Bing GPT chatbot
-        Repo: github.com/acheong08/EdgeGPT
-        By: Antonio Cheong
+        re_edge_gpt - A demo of reverse engineering the Bing GPT chatbot
 
         !help for help
 
         Type !exit to exit
 
-usage: EdgeGPT.py [-h] [--enter-once] [--search-result] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK]
+usage: re_edge_gpt.py [-h] [--enter-once] [--search-result] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK]
                   [--style {creative,balanced,precise}] [--prompt PROMPT] [--cookie-file COOKIE_FILE]
                   [--history-file HISTORY_FILE] [--locale LOCALE]
 
 options:
   -h, --help            show this help message and exit
   --enter-once
   --search-result
@@ -135,15 +133,15 @@
 
 from pathlib import Path
 from re_edge_gpt import Chatbot, ConversationStyle
 
 cookies = json.loads(open(str(Path(str(Path.cwd()) + "/bing_cookies.json")), encoding="utf-8").read())
 
 async def main():
-    bot = await Chatbot.create(cookies=cookies) # Passing cookies is "optional", as explained above
+    bot = await Chatbot.create(cookies=cookies)
     response = await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative, simplify_response=True)
     print(json.dumps(response, indent=2)) # Returns
     """
 {
     "text": str,
     "author": str,
     "sources": list[dict],
@@ -155,7 +153,11 @@
     await bot.close()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 </details>
+
+---
+> Origin repo (archived): https://github.com/acheong08/EdgeGPT
+---
```

