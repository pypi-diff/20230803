# Comparing `tmp/langchain_wenxin-0.8.3.tar.gz` & `tmp/langchain_wenxin-0.8.4.tar.gz`

## Comparing `langchain_wenxin-0.8.3.tar` & `langchain_wenxin-0.8.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0    14049 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/examples/Langchain_wenxin_retrieval_qa_compared.ipynb
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/src/langchain_wenxin/__about__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/src/langchain_wenxin/__init__.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/src/langchain_wenxin/chat_models.py
--rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/src/langchain_wenxin/client.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/src/langchain_wenxin/embeddings.py
--rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/src/langchain_wenxin/llms.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/src/langchain_wenxin/retrievers.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/integration_tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/integration_tests/chat_models/__init__.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/integration_tests/chat_models/test_wenxin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/integration_tests/embeddings/__init__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/integration_tests/embeddings/test_wenxin.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/integration_tests/llms/__init__.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/integration_tests/llms/test_wenxin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/tools/__init__.py
--rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/tools/test_callbacks.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/LICENSE.txt
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/README.md
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0    14049 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/examples/Langchain_wenxin_retrieval_qa_compared.ipynb
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/src/langchain_wenxin/__about__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/src/langchain_wenxin/__init__.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/src/langchain_wenxin/chat_models.py
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/src/langchain_wenxin/client.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/src/langchain_wenxin/embeddings.py
+-rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/src/langchain_wenxin/llms.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/src/langchain_wenxin/retrievers.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/tests/integration_tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/tests/integration_tests/chat_models/__init__.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/tests/integration_tests/chat_models/test_wenxin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/tests/integration_tests/embeddings/__init__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/tests/integration_tests/embeddings/test_wenxin.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/tests/integration_tests/llms/__init__.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/tests/integration_tests/llms/test_wenxin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/tests/tools/__init__.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/tests/tools/test_callbacks.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/LICENSE.txt
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/README.md
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.4/PKG-INFO
```

### Comparing `langchain_wenxin-0.8.3/examples/Langchain_wenxin_retrieval_qa_compared.ipynb` & `langchain_wenxin-0.8.4/examples/Langchain_wenxin_retrieval_qa_compared.ipynb`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.3/src/langchain_wenxin/chat_models.py` & `langchain_wenxin-0.8.4/src/langchain_wenxin/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.3/src/langchain_wenxin/client.py` & `langchain_wenxin-0.8.4/src/langchain_wenxin/client.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.3/src/langchain_wenxin/embeddings.py` & `langchain_wenxin-0.8.4/src/langchain_wenxin/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.3/src/langchain_wenxin/llms.py` & `langchain_wenxin-0.8.4/src/langchain_wenxin/llms.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,17 +38,14 @@
 
     streaming: bool = False
     """Whether to stream the results."""
 
     request_timeout: Optional[int] = 600
     """Timeout for requests to Baidu Wenxin Completion API. Default is 600 seconds."""
 
-    max_message_length: Optional[int] = 2000
-    """Maximum length of last message."""
-
     baidu_api_key: Optional[str] = None
     """Baidu Cloud API key."""
 
     baidu_secret_key: Optional[str] = None
     """Baidu Cloud secret key."""
 
     @root_validator()
@@ -80,14 +77,24 @@
         return d
 
     @property
     def _identifying_params(self) -> Mapping[str, Any]:
         """Get the identifying parameters."""
         return {**{}, **self._default_params}
 
+    @property
+    def max_message_length(self) -> int:
+        """Maximum length of last message."""
+        if self.model == "ernie-bot-turbo" or self.model == "eb-instant":
+            # https://cloud.baidu.com/doc/WENXINWORKSHOP/s/4lilb2lpf
+            return 11200
+        else:
+            # https://cloud.baidu.com/doc/WENXINWORKSHOP/s/jlil56u11
+            return 2000
+
 
 class Wenxin(LLM, BaiduCommon):
     r"""Wrapper around Baidu Wenxin large language models.
 
     To use, you should have the ``requests`` python package installed, and the
     environment variable ``BAIDU_API_KEY`` and ``BAIDU_SECRET_KEY``, or pass
     it as a named parameter to the constructor.
```

### Comparing `langchain_wenxin-0.8.3/src/langchain_wenxin/retrievers.py` & `langchain_wenxin-0.8.4/src/langchain_wenxin/retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.3/tests/integration_tests/chat_models/test_wenxin.py` & `langchain_wenxin-0.8.4/tests/integration_tests/chat_models/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.3/tests/integration_tests/embeddings/test_wenxin.py` & `langchain_wenxin-0.8.4/tests/integration_tests/embeddings/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.3/tests/integration_tests/llms/test_wenxin.py` & `langchain_wenxin-0.8.4/tests/integration_tests/llms/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.3/tests/tools/test_callbacks.py` & `langchain_wenxin-0.8.4/tests/tools/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.3/.gitignore` & `langchain_wenxin-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.3/LICENSE.txt` & `langchain_wenxin-0.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.3/README.md` & `langchain_wenxin-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.3/pyproject.toml` & `langchain_wenxin-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.3/PKG-INFO` & `langchain_wenxin-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-wenxin
-Version: 0.8.3
+Version: 0.8.4
 Project-URL: Documentation, https://github.com/ninehills/langchain-wenxin#readme
 Project-URL: Issues, https://github.com/ninehills/langchain-wenxin/issues
 Project-URL: Source, https://github.com/ninehills/langchain-wenxin
 Author-email: Tao Yang <swulling@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

