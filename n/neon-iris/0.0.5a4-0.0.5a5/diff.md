# Comparing `tmp/neon-iris-0.0.5a4.tar.gz` & `tmp/neon-iris-0.0.5a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-iris-0.0.5a4.tar", last modified: Tue Jul 25 23:48:10 2023, max compression
+gzip compressed data, was "neon-iris-0.0.5a5.tar", last modified: Wed Aug  2 23:07:27 2023, max compression
```

## Comparing `neon-iris-0.0.5a4.tar` & `neon-iris-0.0.5a5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:48:10.917517 neon-iris-0.0.5a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-25 23:48:05.000000 neon-iris-0.0.5a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-25 23:48:10.917517 neon-iris-0.0.5a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-25 23:48:05.000000 neon-iris-0.0.5a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:48:10.913517 neon-iris-0.0.5a4/neon_iris/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-25 23:48:05.000000 neon-iris-0.0.5a4/neon_iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-07-25 23:48:05.000000 neon-iris-0.0.5a4/neon_iris/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-07-25 23:48:05.000000 neon-iris-0.0.5a4/neon_iris/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-25 23:48:05.000000 neon-iris-0.0.5a4/neon_iris/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-25 23:48:05.000000 neon-iris-0.0.5a4/neon_iris/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-25 23:48:05.000000 neon-iris-0.0.5a4/neon_iris/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:48:10.917517 neon-iris-0.0.5a4/neon_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-25 23:48:10.000000 neon-iris-0.0.5a4/neon_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 23:48:10.000000 neon-iris-0.0.5a4/neon_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:48:10.000000 neon-iris-0.0.5a4/neon_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-25 23:48:10.000000 neon-iris-0.0.5a4/neon_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-25 23:48:10.000000 neon-iris-0.0.5a4/neon_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 23:48:10.000000 neon-iris-0.0.5a4/neon_iris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 23:48:10.917517 neon-iris-0.0.5a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-25 23:48:05.000000 neon-iris-0.0.5a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:07:27.368949 neon-iris-0.0.5a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-02 23:07:23.000000 neon-iris-0.0.5a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-02 23:07:27.368949 neon-iris-0.0.5a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-02 23:07:23.000000 neon-iris-0.0.5a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:07:27.368949 neon-iris-0.0.5a5/neon_iris/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-02 23:07:23.000000 neon-iris-0.0.5a5/neon_iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-08-02 23:07:23.000000 neon-iris-0.0.5a5/neon_iris/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-08-02 23:07:23.000000 neon-iris-0.0.5a5/neon_iris/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-08-02 23:07:23.000000 neon-iris-0.0.5a5/neon_iris/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-02 23:07:23.000000 neon-iris-0.0.5a5/neon_iris/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-02 23:07:23.000000 neon-iris-0.0.5a5/neon_iris/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:07:27.368949 neon-iris-0.0.5a5/neon_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-02 23:07:27.000000 neon-iris-0.0.5a5/neon_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-02 23:07:27.000000 neon-iris-0.0.5a5/neon_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:07:27.000000 neon-iris-0.0.5a5/neon_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 23:07:27.000000 neon-iris-0.0.5a5/neon_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-02 23:07:27.000000 neon-iris-0.0.5a5/neon_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 23:07:27.000000 neon-iris-0.0.5a5/neon_iris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 23:07:27.368949 neon-iris-0.0.5a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-08-02 23:07:23.000000 neon-iris-0.0.5a5/setup.py
```

### Comparing `neon-iris-0.0.5a4/LICENSE.md` & `neon-iris-0.0.5a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-iris-0.0.5a4/PKG-INFO` & `neon-iris-0.0.5a5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-iris
-Version: 0.0.5a4
+Version: 0.0.5a5
 Summary: Interactive Relay for Intelligence Systems
 Home-page: https://github.com/neongeckocom/neon-iris
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-iris-0.0.5a4/README.md` & `neon-iris-0.0.5a5/README.md`

 * *Files identical despite different names*

### Comparing `neon-iris-0.0.5a4/neon_iris/__init__.py` & `neon-iris-0.0.5a5/neon_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.0.5a4/neon_iris/cli.py` & `neon-iris-0.0.5a5/neon_iris/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,16 +67,20 @@
               help="Path to User Config file")
 @click.option('--lang', '-l', default="en-us",
               help="Language to accept input in")
 @click.option('--audio', '-a', is_flag=True, default=False,
               help="Flag to enable audio playback")
 def start_client(mq_config, user_config, lang, audio):
     from neon_iris.client import CLIClient
+    _print_config()
     if mq_config:
         mq_config = load_config_file(expanduser(mq_config))
+    else:
+        from ovos_config.config import Configuration
+        mq_config = Configuration().get("MQ")
     if user_config:
         user_config = load_config_file(expanduser(user_config))
     client = CLIClient(mq_config, user_config)
     LOG.init({"level": logging.WARNING})
 
     client.audio_enabled = audio
     click.echo("Enter '!{lang}' to change language\n"
@@ -110,14 +114,37 @@
                 sleep(1)
     except Exception as e:
         click.echo(e)
     click.echo("Shutting Down Client")
     client.shutdown()
 
 
+@neon_iris_cli.command(help="Transcribe an audio file")
+@click.option('--lang', '-l', default='en-us',
+              help="language of input audio")
+@click.argument("audio_file")
+def get_stt(audio_file, lang):
+    from neon_iris.util import get_stt
+    _print_config()
+    resp = get_stt(audio_file, lang)
+    click.echo(pformat(resp))
+
+
+@neon_iris_cli.command(help="Transcribe an audio file")
+@click.option('--lang', '-l', default='en-us',
+              help="language of input audio")
+@click.argument("utterance")
+def get_tts(utterance, lang):
+    from neon_iris.util import get_tts
+    _print_config()
+    resp = get_tts(utterance, lang)
+    click.echo(pformat(resp))
+
+
+# Backend
 @neon_iris_cli.command(help="Query a weather endpoint")
 @click.option('--unit', '-u', default='imperial',
               help="units to use ('metric' or 'imperial')")
 @click.option('--latitude', '--lat', default=47.6815,
               help="location latitude")
 @click.option('--longitude', '--lon', default=-122.2087,
               help="location latitude")
```

### Comparing `neon-iris-0.0.5a4/neon_iris/client.py` & `neon-iris-0.0.5a5/neon_iris/client.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.0.5a4/neon_iris/llm.py` & `neon-iris-0.0.5a5/neon_iris/llm.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.0.5a4/neon_iris/util.py` & `neon-iris-0.0.5a5/neon_iris/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 import json
 import yaml
 
 from os.path import isfile
 from ovos_utils.log import LOG
 
+from neon_utils.file_utils import encode_file_to_base64_string
+
 
 def load_config_file(file_path: str) -> dict:
     """
     Load a config file (json or yaml) and return the dict contents
     :param file_path: path to config file to load
     """
     if not isfile(file_path):
@@ -86,7 +88,45 @@
         text = f.read()
     metadata = metadata or {}
     response = send_mq_request("/neon_script_parser", {"text": text,
                                                        "metadata": metadata},
                                "neon_script_parser_input",
                                "neon_script_parser_output", timeout)
     return response
+
+
+def query_neon(msg_type: str, data: dict, timeout: int = 10) -> dict:
+    """
+    Query a Neon Core service on the `/neon_chat_api`
+    :param msg_type: string message type to emit
+    :param data: message data to send
+    :param timeout: seconds to wait for a response
+    """
+    from neon_mq_connector.utils.client_utils import send_mq_request
+    query = {"msg_type": msg_type, "data": data, "context": {"source": "iris"}}
+    response = send_mq_request("/neon_chat_api", query, "neon_chat_api_request",
+                               timeout=timeout)
+    if response:
+        response["context"]["session"] = \
+            set(response["context"].pop("session").keys())
+    return response
+
+
+def get_stt(audio_file: str, lang: str = "en-us") -> dict:
+    data = {"audio_file": audio_file,
+            "audio_data": encode_file_to_base64_string(audio_file),
+            "utterances": [""],  # TODO: For MQ Connector compat.
+            "lang": lang}
+    response = query_neon("neon.get_stt", data, 20)
+    return response
+
+
+def get_tts(string: str, lang: str = "en-us") -> dict:
+    data = {"text": string,
+            "utterance": string,  # TODO: For MQ Connector compat.
+            "utterances": [""],  # TODO: For MQ Connector compat.
+            "speaker": {"name": "Neon",
+                        "language": lang,
+                        "gender": "female"},  # TODO: For neon_audio compat.
+            "lang": lang}
+    response = query_neon("neon.get_tts", data)
+    return response
```

### Comparing `neon-iris-0.0.5a4/neon_iris/version.py` & `neon-iris-0.0.5a5/neon_iris/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.0.5a4"
+__version__ = "0.0.5a5"
```

### Comparing `neon-iris-0.0.5a4/neon_iris.egg-info/PKG-INFO` & `neon-iris-0.0.5a5/neon_iris.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-iris
-Version: 0.0.5a4
+Version: 0.0.5a5
 Summary: Interactive Relay for Intelligence Systems
 Home-page: https://github.com/neongeckocom/neon-iris
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-iris-0.0.5a4/setup.py` & `neon-iris-0.0.5a5/setup.py`

 * *Files identical despite different names*

