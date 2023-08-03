# Comparing `tmp/iamlistening-3.0.2.tar.gz` & `tmp/iamlistening-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-3.0.2.tar", max compression
+gzip compressed data, was "iamlistening-3.1.0.tar", max compression
```

## Comparing `iamlistening-3.0.2.tar` & `iamlistening-3.1.0.tar`

### file list

```diff
@@ -1,13 +1,20 @@
--rw-r--r--   0        0        0     1064 2023-07-25 15:31:53.820480 iamlistening-3.0.2/LICENSE
--rw-r--r--   0        0        0     2746 2023-07-25 15:31:53.820480 iamlistening-3.0.2/README.md
--rw-r--r--   0        0        0      136 2023-07-25 15:31:56.152507 iamlistening-3.0.2/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/config.py
--rw-r--r--   0        0        0     2722 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     1660 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/main.py
--rw-r--r--   0        0        0      151 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/platform/__init__.py
--rw-r--r--   0        0        0      761 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/platform/discord.py
--rw-r--r--   0        0        0     1489 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/platform/matrix.py
--rw-r--r--   0        0        0      609 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/platform/rocket_chat.py
--rw-r--r--   0        0        0      808 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/platform/telegram.py
--rw-r--r--   0        0        0     3198 2023-07-25 15:31:56.144507 iamlistening-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 iamlistening-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-03 19:56:07.875240 iamlistening-3.1.0/LICENSE
+-rw-r--r--   0        0        0     2769 2023-08-03 19:56:07.875240 iamlistening-3.1.0/README.md
+-rw-r--r--   0        0        0       81 2023-08-03 19:56:38.895485 iamlistening-3.1.0/iamlistening/__init__.py
+-rw-r--r--   0        0        0      686 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/config.py
+-rw-r--r--   0        0        0     1376 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     1673 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/main.py
+-rw-r--r--   0        0        0        0 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/platform/__init__.py
+-rw-r--r--   0        0        0     3275 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/platform/chat_manager.py
+-rw-r--r--   0        0        0        0 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/platform/clients/__init__.py
+-rw-r--r--   0        0        0      876 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/platform/clients/discord.py
+-rw-r--r--   0        0        0      738 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/platform/clients/guilded.py
+-rw-r--r--   0        0        0      672 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/platform/clients/lemmy.py
+-rw-r--r--   0        0        0     1349 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/platform/clients/mastodon.py
+-rw-r--r--   0        0        0     1616 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/platform/clients/matrix.py
+-rw-r--r--   0        0        0      912 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/platform/clients/revolt.py
+-rw-r--r--   0        0        0      806 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/platform/clients/rocket_chat.py
+-rw-r--r--   0        0        0     1176 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/platform/clients/telegram.py
+-rw-r--r--   0        0        0      568 2023-08-03 19:56:07.875240 iamlistening-3.1.0/iamlistening/platform/clients/tinode.py
+-rw-r--r--   0        0        0     3221 2023-08-03 19:56:38.887485 iamlistening-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4019 1970-01-01 00:00:00.000000 iamlistening-3.1.0/PKG-INFO
```

### Comparing `iamlistening-3.0.2/LICENSE` & `iamlistening-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-3.0.2/README.md` & `iamlistening-3.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       <a href="https://github.com/mraniki/iamlistening/"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/iamlistening/%F0%9F%91%B7Flow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
    <a href="https://talky.readthedocs.io/"><img src="https://readthedocs.org/projects/iamlistening/badge/?version=latest&style=for-the-badge"></a><br>
    <a href="https://codebeat.co/projects/github-com-mraniki-iamlistening-main"><img src="https://codebeat.co/badges/4085334e-4590-41f6-a70c-69e9a2641c79"/></a><br>
    <a href="https://codecov.io/gh/mraniki/iamlistening"> <img src="https://codecov.io/gh/mraniki/iamlistening/branch/main/graph/badge.svg?token=QZ55U6KQFN"/></a><br>
     </td>
     <td align="left"> 
        A python package to listen to messaging platforms,<br>
-       such as discord, telegram and matrix.
+       such as discord, telegram, matrix, guilded, mastodon, lemmy.
     </td>
      
   </tr>
 </table>
 
 <h5>How to use it</h5>
 <pre>
```

#### html2text {}

```diff
@@ -12,17 +12,17 @@
 [https://img.shields.io/pypi/v/iamlistening?style=for-the-
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/pypi/dm/iamlistening?style=for-the-
 badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey] A python package to
 [https://img.shields.io/github/actions/workflow/status/     listen to messaging
 mraniki/iamlistening/%F0%9F%91%B7Flow.yml?style=for-the-    platforms,
 badge&logo=GitHub&logoColor=white]                          such as discord,
-[https://readthedocs.org/projects/iamlistening/badge/       telegram and
-?version=latest&style=for-the-badge]                        matrix.
-[https://codebeat.co/badges/4085334e-4590-41f6-a70c-
+[https://readthedocs.org/projects/iamlistening/badge/       telegram, matrix,
+?version=latest&style=for-the-badge]                        guilded, mastodon,
+[https://codebeat.co/badges/4085334e-4590-41f6-a70c-        lemmy.
 69e9a2641c79]
 [https://codecov.io/gh/mraniki/iamlistening/branch/main/
 graph/badge.svg?token=QZ55U6KQFN]
 ** How to use it **
 
       from iamlistening import Listener
       listener = Listener()
```

### Comparing `iamlistening-3.0.2/iamlistening/config.py` & `iamlistening-3.1.0/iamlistening/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 # Define the root path of the project
 ROOT = os.path.dirname(__file__)
 
 # Load the default settings file
 settings = Dynaconf(
     envvar_prefix="TT",
     # Set the root path of the project
-    root_path=os.path.dirname(ROOT),
+   # root_path=os.path.dirname(ROOT),
     # Load the default settings file
     settings_files=[
         os.path.join(ROOT, "default_settings.toml"),
         'talky_settings.toml',
         'settings.toml',
         '.secrets.toml'
     ],
     # Load the.env file
     load_dotenv=True,
     # Set the environments to True
     environments=True,
+    merge_enabled=True,
     # Set the default environment
     default_env="default",)
```

### Comparing `iamlistening-3.0.2/iamlistening/platform/discord.py` & `iamlistening-3.1.0/iamlistening/platform/clients/discord.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,31 +3,40 @@
 """
 import asyncio
 
 import discord
 from loguru import logger
 
 from iamlistening.config import settings
-from iamlistening.main import ChatManager
+from iamlistening.platform.chat_manager import ChatManager
 
 
 class DiscordHandler(ChatManager):
 
     def __init__(self):
+        """
+        Initialize the Discord handler.
+
+ 
+        """
         super().__init__()
 
     async def start(self):
-        """Start the Discord handler."""
+        """
+        Start the Discord handler.
+        
+        """
+
         logger.debug("Discord setup")
         intents = discord.Intents.default()
         intents.message_content = True
-        bot = discord.Bot(intents=intents)
+        self.bot = discord.Bot(intents=intents)
 
-        @bot.event
+        @self.bot.event
         async def on_ready():
-            logger.info("listener is online")
+            self.connected()
 
-        @bot.event
+        @self.bot.event
         async def on_message(message: discord.Message):
             await self.handle_message(message.content)
     
-        await bot.start(settings.bot_token)
+        await self.bot.start(settings.bot_token)
```

### Comparing `iamlistening-3.0.2/iamlistening/platform/matrix.py` & `iamlistening-3.1.0/iamlistening/platform/clients/matrix.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,48 +3,53 @@
 """
 import asyncio
 
 import simplematrixbotlib as botlib
 from loguru import logger
 
 from iamlistening.config import settings
-from iamlistening.main import ChatManager
+from iamlistening.platform.chat_manager import ChatManager
 
 
 class MatrixHandler(ChatManager):
 
     def __init__(self):
+        """
+        Initialize the Matrix handler.
+        """
         super().__init__()
 
     async def start(self):
-        """Start the Matrix handler."""
+        """
+        Start the Matrix handler.
+        """
         logger.debug("Matrix setup")
         config = botlib.Config()
         config.emoji_verify = True
         config.ignore_unverified_devices = True
         config.store_path = './config/matrix/'
         creds = botlib.Creds(
-                    settings.matrix_hostname,
-                    settings.matrix_user,
-                    settings.matrix_pass
+                    settings.bot_hostname,
+                    settings.bot_user,
+                    settings.bot_pass
                     )
-        bot = botlib.Bot(creds, config)
+        self.bot = botlib.Bot(creds, config)
  
-        @bot.listener.on_startup
+        @self.bot.listener.on_startup
         async def room_joined(room):
-            logger.info("listener is online")
+            self.connected()
 
-        @bot.listener.on_message_event
+        @self.bot.listener.on_message_event
         async def on_matrix_message(room, message):
             await self.handle_message(message.body)
-        await bot.api.login()
-        bot.api.async_client.callbacks = botlib.Callbacks(
-            bot.api.async_client, bot
+        await self.bot.api.login()
+        self.bot.api.async_client.callbacks = botlib.Callbacks(
+            self.bot.api.async_client, self.bot
             )
-        await bot.api.async_client.callbacks.setup_callbacks()
-        for action in bot.listener._startup_registry:
-            for room_id in bot.api.async_client.rooms:
+        await self.bot.api.async_client.callbacks.setup_callbacks()
+        for action in self.bot.listener._startup_registry:
+            for room_id in self.bot.api.async_client.rooms:
                 await action(room_id)
-        await bot.api.async_client.sync_forever(
+        await self.bot.api.async_client.sync_forever(
             timeout=3000,
             full_state=True
             )
```

### Comparing `iamlistening-3.0.2/pyproject.toml` & `iamlistening-3.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,86 +1,91 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "3.0.2"
+version = "3.1.0"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "bot","messaging",
     "discord", "telegram","matrix","rocket chat",
     ]
 packages = [
     {include = "iamlistening"}
 ]
 
-
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/iamlistening/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/iamlistening/discussions"
 "Issues" =  "https://github.com/mraniki/iamlistening/issues"
 
+
+
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
 loguru = "^0.7.0"
+beautifulsoup4 = "^4.12.2"
 telethon= "^1.28.5"
 py-cord= "^2.4.1"
 simplematrixbotlib= "^2.9.0"
 rocketchat-API= "^1.30.0"
+"Mastodon.py" = "^1.8.1"
+"guilded.py" = "^1.9.1"
+tinode_grpc = "^0.22.3"
+"revolt.py" = "^0.1.11"
+
 
 
 [tool.poetry.group.dev.dependencies]
-python-semantic-release = "^8.0.1"
-ruff = ">=0.0.278,<0.0.281"
+python-semantic-release = "^8.0.4"
+ruff = "^0.0.281"
+
+
 
 [tool.ruff]
 select = [
   "E",  # pycodestyle
   "F",  # pyflakes
   "I",  # isort
 ]
 exclude = [
   ".github/*",
 ]
 ignore = ["E401","F401","F811"]
 format = "github"
 fixable = ["ALL"]
 
+
 [tool.pylint.exceptions]
 overgeneral-exceptions = [
     "builtins.BaseException",
     "builtins.Exception",
     "builtins.RuntimeError",
 ]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
-pytest-asyncio = "^0.21.0"
+pytest-asyncio = "^0.21.1"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.2.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = ">=6,<8"
+sphinx = ">=5,<6"
 sphinx_bootstrap_theme = "^0.8.1"
-sphinx-autoapi = "^2.1.1"
-sphinx-copybutton= "^0.5.2"
-myst-parser = "^2.0.0"
-sphinx-notfound-page = "^0.8.3"
 sphinxext-remoteliteralinclude = "^0.4.0"
-sphinx-togglebutton = "*"
 
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
@@ -94,14 +99,16 @@
 omit = [
     "tests/*",
     "examples/*",
     "docs/*",
     "*/config.py"
 ]
 
+[tool.bandit]
+exclude_dirs = ["tests"]
 
 [tool.semantic_release]
 upload_to_vcs_release = true
 version_variables = ["pyproject.toml:version","iamlistening/__init__.py:__version__"]
 build_command = "pip install poetry && poetry build"
 commit_parser = "emoji"
```

### Comparing `iamlistening-3.0.2/PKG-INFO` & `iamlistening-3.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 3.0.2
+Version: 3.1.0
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: bot,messaging,discord,telegram,matrix,rocket chat
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Mastodon.py (>=1.8.1,<2.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: guilded.py (>=1.9.1,<2.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: py-cord (>=2.4.1,<3.0.0)
+Requires-Dist: revolt.py (>=0.1.11,<0.2.0)
 Requires-Dist: rocketchat-API (>=1.30.0,<2.0.0)
 Requires-Dist: simplematrixbotlib (>=2.9.0,<3.0.0)
 Requires-Dist: telethon (>=1.28.5,<2.0.0)
+Requires-Dist: tinode_grpc (>=0.22.3,<0.23.0)
 Project-URL: Changelog, https://github.com/mraniki/iamlistening/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/iamlistening/issues
 Project-URL: Support, https://github.com/mraniki/iamlistening/discussions
 Description-Content-Type: text/markdown
 
 
 <table style="border: 1px solid transparent">
@@ -41,15 +46,15 @@
       <a href="https://github.com/mraniki/iamlistening/"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/iamlistening/%F0%9F%91%B7Flow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
    <a href="https://talky.readthedocs.io/"><img src="https://readthedocs.org/projects/iamlistening/badge/?version=latest&style=for-the-badge"></a><br>
    <a href="https://codebeat.co/projects/github-com-mraniki-iamlistening-main"><img src="https://codebeat.co/badges/4085334e-4590-41f6-a70c-69e9a2641c79"/></a><br>
    <a href="https://codecov.io/gh/mraniki/iamlistening"> <img src="https://codecov.io/gh/mraniki/iamlistening/branch/main/graph/badge.svg?token=QZ55U6KQFN"/></a><br>
     </td>
     <td align="left"> 
        A python package to listen to messaging platforms,<br>
-       such as discord, telegram and matrix.
+       such as discord, telegram, matrix, guilded, mastodon, lemmy.
     </td>
      
   </tr>
 </table>
 
 <h5>How to use it</h5>
 <pre>
```

#### html2text {}

```diff
@@ -1,17 +1,20 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 3.0.2 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 3.1.0 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 bot,messaging,discord,telegram,matrix,rocket chat Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
-(>=3.1.12,<4.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist: py-cord
-(>=2.4.1,<3.0.0) Requires-Dist: rocketchat-API (>=1.30.0,<2.0.0) Requires-Dist:
-simplematrixbotlib (>=2.9.0,<3.0.0) Requires-Dist: telethon (>=1.28.5,<2.0.0)
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Mastodon.py
+(>=1.8.1,<2.0.0) Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist:
+dynaconf (>=3.1.12,<4.0.0) Requires-Dist: guilded.py (>=1.9.1,<2.0.0) Requires-
+Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist: py-cord (>=2.4.1,<3.0.0) Requires-
+Dist: revolt.py (>=0.1.11,<0.2.0) Requires-Dist: rocketchat-API
+(>=1.30.0,<2.0.0) Requires-Dist: simplematrixbotlib (>=2.9.0,<3.0.0) Requires-
+Dist: telethon (>=1.28.5,<2.0.0) Requires-Dist: tinode_grpc (>=0.22.3,<0.23.0)
 Project-URL: Changelog, https://github.com/mraniki/iamlistening/blob/dev/
 CHANGELOG.rst Project-URL: Issues, https://github.com/mraniki/iamlistening/
 issues Project-URL: Support, https://github.com/mraniki/iamlistening/
 discussions Description-Content-Type: text/markdown
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
 the-badge&logo=wikipedia&logoColor=white]
 [https://img.shields.io/badge/github-
@@ -26,17 +29,17 @@
 [https://img.shields.io/pypi/v/iamlistening?style=for-the-
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/pypi/dm/iamlistening?style=for-the-
 badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey] A python package to
 [https://img.shields.io/github/actions/workflow/status/     listen to messaging
 mraniki/iamlistening/%F0%9F%91%B7Flow.yml?style=for-the-    platforms,
 badge&logo=GitHub&logoColor=white]                          such as discord,
-[https://readthedocs.org/projects/iamlistening/badge/       telegram and
-?version=latest&style=for-the-badge]                        matrix.
-[https://codebeat.co/badges/4085334e-4590-41f6-a70c-
+[https://readthedocs.org/projects/iamlistening/badge/       telegram, matrix,
+?version=latest&style=for-the-badge]                        guilded, mastodon,
+[https://codebeat.co/badges/4085334e-4590-41f6-a70c-        lemmy.
 69e9a2641c79]
 [https://codecov.io/gh/mraniki/iamlistening/branch/main/
 graph/badge.svg?token=QZ55U6KQFN]
 ** How to use it **
 
       from iamlistening import Listener
       listener = Listener()
```

