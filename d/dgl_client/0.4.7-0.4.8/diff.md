# Comparing `tmp/dgl_client-0.4.7.tar.gz` & `tmp/dgl_client-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgl_client-0.4.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dgl_client-0.4.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dgl_client-0.4.7.tar` & `dgl_client-0.4.8.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0       62 2023-06-26 10:49:28.405914 dgl_client-0.4.7/.gitignore
--rw-r--r--   0        0        0     1599 2023-05-30 07:01:38.904624 dgl_client-0.4.7/README.md
--rw-r--r--   0        0        0       64 2023-06-26 13:30:40.475890 dgl_client-0.4.7/dgl_client/__init__.py
--rw-r--r--   0        0        0    10956 2023-06-26 13:29:13.126672 dgl_client-0.4.7/dgl_client/api_cli.py
--rw-r--r--   0        0        0        0 2023-06-22 08:43:15.967703 dgl_client-0.4.7/dgl_client/commands/__init__.py
--rw-r--r--   0        0        0     1642 2023-06-26 12:41:45.269957 dgl_client-0.4.7/dgl_client/commands/chat.py
--rw-r--r--   0        0        0     3362 2023-06-26 13:23:47.179330 dgl_client-0.4.7/dgl_client/commands/collections.py
--rw-r--r--   0        0        0     1566 2023-06-26 12:48:07.639757 dgl_client-0.4.7/dgl_client/commands/ls.py
--rw-r--r--   0        0        0     1142 2023-06-26 13:25:15.779834 dgl_client-0.4.7/dgl_client/commands/utils.py
--rw-r--r--   0        0        0     5011 2023-06-21 14:26:36.680782 dgl_client-0.4.7/dgl_client/main.py
--rw-r--r--   0        0        0      942 2023-06-26 13:01:10.194593 dgl_client-0.4.7/dgl_client/main2.py
--rw-r--r--   0        0        0     2652 2023-06-26 13:30:15.364075 dgl_client-0.4.7/dgl_client/utils.py
--rw-r--r--   0        0        0     2033 2023-05-30 13:59:58.346248 dgl_client-0.4.7/notebook.ipynb
--rw-r--r--   0        0        0      498 2023-06-26 12:41:56.393164 dgl_client-0.4.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 14:22:35.775422 dgl_client-0.4.7/tests/__init__.py
--rw-r--r--   0        0        0      784 2023-06-14 14:42:24.721364 dgl_client-0.4.7/tests/test_collections.py
--rw-r--r--   0        0        0      383 1970-01-01 00:00:00.000000 dgl_client-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0       62 2023-08-01 09:54:43.901554 dgl_client-0.4.8/.gitignore
+-rw-r--r--   0        0        0     1599 2023-08-01 09:54:43.901796 dgl_client-0.4.8/README.md
+-rw-r--r--   0        0        0       65 2023-08-03 09:20:18.746838 dgl_client-0.4.8/dgl_client/__init__.py
+-rw-r--r--   0        0        0    10973 2023-08-01 09:54:43.902358 dgl_client-0.4.8/dgl_client/api_cli.py
+-rw-r--r--   0        0        0        0 2023-08-01 09:54:43.902521 dgl_client-0.4.8/dgl_client/commands/__init__.py
+-rw-r--r--   0        0        0     1753 2023-08-03 12:40:04.406576 dgl_client-0.4.8/dgl_client/commands/chat.py
+-rw-r--r--   0        0        0     3555 2023-08-03 12:40:51.045242 dgl_client-0.4.8/dgl_client/commands/collections.py
+-rw-r--r--   0        0        0      723 2023-08-03 12:41:22.998122 dgl_client-0.4.8/dgl_client/commands/login.py
+-rw-r--r--   0        0        0     1603 2023-08-03 12:41:05.709457 dgl_client-0.4.8/dgl_client/commands/ls.py
+-rw-r--r--   0        0        0      948 2023-08-03 12:38:50.087759 dgl_client-0.4.8/dgl_client/commands/utils.py
+-rw-r--r--   0        0        0     1124 2023-08-03 14:41:59.074423 dgl_client-0.4.8/dgl_client/config.py
+-rw-r--r--   0        0        0     5011 2023-08-01 09:54:43.903515 dgl_client-0.4.8/dgl_client/main.py
+-rw-r--r--   0        0        0     1063 2023-08-03 12:15:36.927554 dgl_client-0.4.8/dgl_client/main2.py
+-rw-r--r--   0        0        0     2822 2023-08-03 09:18:42.550872 dgl_client-0.4.8/dgl_client/utils.py
+-rw-r--r--   0        0        0     2033 2023-08-01 09:54:43.904158 dgl_client-0.4.8/notebook.ipynb
+-rw-r--r--   0        0        0      523 2023-08-03 09:23:28.457731 dgl_client-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 09:54:43.904704 dgl_client-0.4.8/tests/__init__.py
+-rw-r--r--   0        0        0      784 2023-08-01 09:54:43.904896 dgl_client-0.4.8/tests/test_collections.py
+-rw-r--r--   0        0        0     1602 2023-08-01 09:54:43.905060 dgl_client-0.4.8/tests/test_decode.py
+-rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 dgl_client-0.4.8/PKG-INFO
```

### Comparing `dgl_client-0.4.7/README.md` & `dgl_client-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.7/dgl_client/api_cli.py` & `dgl_client-0.4.8/dgl_client/api_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 import json
 import requests
 import sseclient
 import uuid
 import shutil
 from rich import print
 
-
 from .utils import inf_ak2token, inf_login_check, inf_prepare_token, inf_refresh_token
 from .utils import bck_ak2token, bck_login_check
 
 class BaseClient:
-    
     def __init__(self, backend_url, http_client=requests, debug=False):
         self.backend_url = backend_url
         self.http_client = http_client
         self.auth_headers = None
 
         if debug:
             import http.client as http_client
@@ -229,15 +227,15 @@
         )
         response.raise_for_status()
         embed = response.json()['data'][0]['embedding']
         print("EMBED",embed)
         return embed
         
 
-    def send_message(self, message, model_config_name, collection=None):
+    def send_message(self, message, model_config_name, collection=None, override_prompt=False):
         print("PARENT:",self.message_id)
         response = self.http_client.post(
             f"{self.backend_url}/chats/{self.chat_id}/prompter_message",
             json={
                 "parent_id": self.message_id,
                 "content": message,
                 "data": {"collection": collection}
```

### Comparing `dgl_client-0.4.7/dgl_client/commands/chat.py` & `dgl_client-0.4.8/dgl_client/commands/chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import typer
 from loguru import logger
 
 from ..api_cli import APIClient, InferenceClient
-from .utils import get_inf_client, do_login, DGL_INF_ENDPOINT
+from .utils import get_inf_client, do_login
+from ..config import settings
 
 app = typer.Typer()
 
 @app.callback(invoke_without_command=True)
 def send_message(
     msg:str ,
     model: str,
     chat_id: str = "",
     interactive: bool = False,
     collection: str = "",
-    endpoint: str = typer.Option(default=DGL_INF_ENDPOINT),
-    inference_url: str = typer.Option(default="inference"),
-    access_key: str = typer.Option(default="inference")
+    endpoint: str = typer.Option(default=settings.INFERENCE_ENDPOINT),
+    inference_url: str = typer.Option(default=settings.INFERENCE_API_PATH),
+    access_key: str = typer.Option(default=settings.INFERENCE_API_KEY),
+    override_prompt: bool = typer.Option(default=False)
 ):
     """
     Send a message MSG to a MODEL
 
     Use --interactive to enter in a conversation loop with the agent
     Use --collection <CID> to add documents in the collection to the context of the chat
```

### Comparing `dgl_client-0.4.7/dgl_client/commands/collections.py` & `dgl_client-0.4.8/dgl_client/commands/collections.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import typer
 from rich import print
 from loguru import logger
 
-
-from .utils import get_back_client, do_login, DGL_BCK_ENDPOINT
+from ..config import settings
+from .utils import get_back_client, do_login
 
 app = typer.Typer()
 
 @app.command("create")
 def create_collection(
   name: str,
   descr: str,
   bucket: str|None = None,
-  access_key: str = typer.Option(help="The authorization key"),
-  endpoint: str = typer.Option(default=DGL_BCK_ENDPOINT,help="The main endpoint of the system"),
-  inference_url: str = typer.Option(default="api/v1/"),
+  access_key: str = typer.Option(default=settings.BACKEND_API_KEY,help="The authorization key"),
+  endpoint: str = typer.Option(default=settings.BACKEND_ENDPOINT,help="The main endpoint of the system"),
+  inference_url: str = typer.Option(default=settings.BACKEND_API_PATH),
   debug: bool = typer.Option(default=False),  
   ):
     client = get_back_client(endpoint, inference_url, debug=debug)    
     if (client.login(access_key)):
         coll = client.create_collection(
             name = name,
             descr = descr,
@@ -30,16 +30,16 @@
         logger.error("Login failed")
         typer.Exit(-1)
 
 @app.command("upload")
 def upload_dcoment(
   cid: str,
   path: str,
-  access_key: str = typer.Option(help="The authorization key"),
-  endpoint: str = typer.Option(default=DGL_BCK_ENDPOINT,help="The main endpoint of the system"),
+  access_key: str = typer.Option(default=settings.BACKEND_API_KEY,help="The authorization key"),
+  endpoint: str = typer.Option(default=settings.BACKEND_ENDPOINT,help="The main endpoint of the system"),
   inference_url: str = typer.Option(default="api/v1/"),
   debug: bool = typer.Option(default=False),  
   ):
     client = get_back_client(endpoint, inference_url, debug=debug)    
     if (client.login(access_key)):
         coll = client.upload_document(
             cid = cid,
@@ -49,16 +49,16 @@
             print(coll)
     else:
         logger.error("Login failed")
         typer.Exit(-1)
 
 @app.command("ls")
 def list_collections(
-  access_key: str = typer.Option(help="The authorization key"),
-  endpoint: str = typer.Option(default=DGL_BCK_ENDPOINT),
+  access_key: str = typer.Option(default=settings.BACKEND_API_KEY,help="The authorization key"),
+  endpoint: str = typer.Option(default=settings.BACKEND_ENDPOINT),
   inference_url: str = typer.Option(default="api/v1/"),
   debug: bool = typer.Option(default=False),  
   ):
     client = get_back_client(endpoint, inference_url, debug=debug)    
     if (client.login(access_key)):
         collections = client.get_collections()
         for coll in collections:
@@ -66,16 +66,16 @@
     else:
         logger.error("Login failed")
         typer.Exit(-1)
 
 @app.command("lsd")
 def list_documents(
   cid: str, 
-  access_key: str = typer.Option(help="The authorization key"),
-  endpoint: str = typer.Option(default=DGL_BCK_ENDPOINT),
+  access_key: str = typer.Option(default=settings.BACKEND_API_KEY,help="The authorization key"),
+  endpoint: str = typer.Option(default=settings.BACKEND_ENDPOINT),
   inference_url: str = typer.Option(default="api/v1/"),
   debug: bool = typer.Option(default=False),
   ):
     client = get_back_client(endpoint, inference_url, debug=debug)    
     if (client.login(access_key)):
         documents = client.get_documents(cid)
         print(documents)
@@ -85,17 +85,17 @@
         logger.error("Login failed")
         typer.Exit(-1)       
 
 @app.command("download")
 def download_document(
   cid: str, 
   did: str,
-  filename: str = typer.Option(help="File name to save to"),
-  access_key: str = typer.Option(help="The authorization key"),
-  endpoint: str = typer.Option(default=DGL_BCK_ENDPOINT),
+  filename: str,
+  access_key: str = typer.Option(default=settings.BACKEND_API_KEY,help="The authorization key"),
+  endpoint: str = typer.Option(default=settings.BACKEND_ENDPOINT),
   inference_url: str = typer.Option(default="api/v1/"),
   debug: bool = typer.Option(default=False),
   ):
     client = get_back_client(endpoint, inference_url, debug=debug)    
     if (client.login(access_key)):
         client.download_document(cid, did, filename)
     else:
```

### Comparing `dgl_client-0.4.7/dgl_client/commands/ls.py` & `dgl_client-0.4.8/dgl_client/commands/ls.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typer
 from rich import print
 from typing import Optional
 from loguru import logger
-from .utils import get_inf_client, do_login, DGL_INF_ENDPOINT
+from .utils import get_inf_client, do_login
+from ..config import settings
 
 app = typer.Typer()
 
 def list_models(client):
   available_models = client.get_available_models()
   logger.info("Available models %s"%str(available_models))
 
@@ -34,16 +35,16 @@
     print(message)
 
   return messages
 
 @app.callback(invoke_without_command=True)
 def ls(
   resource: str,
-  endpoint: str = typer.Option(default=DGL_INF_ENDPOINT),
-  inference_url: str = typer.Option(default="/inference/"),
+  endpoint: str = typer.Option(default=settings.INFERENCE_ENDPOINT),
+  inference_url: str = typer.Option(default=settings.INFERENCE_API_PATH),
   ):
     client = get_inf_client(endpoint, inference_url)
 
     match resource:
         case "models":
             list_models(client)
         case "model":
```

### Comparing `dgl_client-0.4.7/dgl_client/main.py` & `dgl_client-0.4.8/dgl_client/main.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.7/dgl_client/main2.py` & `dgl_client-0.4.8/dgl_client/main2.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,35 +4,37 @@
 import os
 import sys
 from .api_cli import APIClient, InferenceClient
 import uuid
 from glob import glob
 import json
 from rich import print
-
+from .config import settings
 
 from .commands.chat import app as chat
 from .commands.collections import app as coll
 from .commands.ls import app as ls
+from .commands.login import app as login_app
 
 app = typer.Typer()
+app.add_typer(login_app, name="login")
 app.add_typer(ls, name="ls")
 app.add_typer(chat, name="chat")
 app.add_typer(coll, name="collection")
 
 @app.callback(invoke_without_command=True)
 def main(ctx: typer.Context):
     """
     Example of a CLI app with two subcommands imported from external modules
     """
     if ctx.invoked_subcommand is None:
         print(f"About to execute command: {ctx.invoked_subcommand}")
 
 def do_run():
-    LOGDIR="./logs"
+    LOGDIR="./vast_api_logs"
     if not os.path.exists(LOGDIR):
         os.makedirs(LOGDIR)
 
     logger.add(os.path.join(LOGDIR, "file_{time}.log"))
 
     app()
```

### Comparing `dgl_client-0.4.7/dgl_client/utils.py` & `dgl_client-0.4.8/dgl_client/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 from base64 import b64decode, b64encode
 import requests
 from loguru import logger
+from .config import settings
 
 def inf_prepare_token(api_key: str, user_id: str , provider_account_id: str, username: str, client="website"):
     token_data = {
         "api_key": api_key,
         "client": client,
         "user_id": user_id,
         "provider_account_id": provider_account_id,
@@ -87,15 +88,17 @@
     except:
       raise
     logger.debug("New token is %s"%str(new_tok))
 
     return new_tok    
 
 def bck_login_check(endp, access_key):
-    logger.info("Trying to login...")
+    logger.info("Trying to login to %s with api key %s"%(settings.backend_uri,settings.BACKEND_API_KEY))
+    endp = settings.backend_uri
+    access_key = settings.BACKEND_API_KEY
     username = None
     try:
       response = requests.get(
           os.path.join(endp, 
             f"auth/check_client"
             ),
           json={},
```

### Comparing `dgl_client-0.4.7/notebook.ipynb` & `dgl_client-0.4.8/notebook.ipynb`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.7/tests/test_collections.py` & `dgl_client-0.4.8/tests/test_collections.py`

 * *Files identical despite different names*

