# Comparing `tmp/streamlit_chatbox-1.1.0-py3-none-any.whl.zip` & `tmp/streamlit_chatbox-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6077 bytes, number of entries: 8
+Zip file size: 6280 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      392 b- defN 23-Jul-30 13:49 streamlit_chatbox/__init__.py
 -rw-rw-rw-  2.0 fat     4431 b- defN 23-Aug-01 03:38 streamlit_chatbox/elements.py
 -rw-rw-rw-  2.0 fat      323 b- defN 23-Jul-31 01:37 streamlit_chatbox/flows.py
--rw-rw-rw-  2.0 fat     4423 b- defN 23-Aug-01 03:38 streamlit_chatbox/messages.py
--rw-rw-rw-  2.0 fat     4417 b- defN 23-Aug-01 03:46 streamlit_chatbox-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 03:46 streamlit_chatbox-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-01 03:46 streamlit_chatbox-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      677 b- defN 23-Aug-01 03:46 streamlit_chatbox-1.1.0.dist-info/RECORD
-8 files, 14773 bytes uncompressed, 4885 bytes compressed:  66.9%
+-rw-rw-rw-  2.0 fat     5264 b- defN 23-Aug-03 03:37 streamlit_chatbox/messages.py
+-rw-rw-rw-  2.0 fat     4417 b- defN 23-Aug-03 03:41 streamlit_chatbox-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 03:41 streamlit_chatbox-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-03 03:41 streamlit_chatbox-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      677 b- defN 23-Aug-03 03:41 streamlit_chatbox-1.1.1.dist-info/RECORD
+8 files, 15614 bytes uncompressed, 5088 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: streamlit_chatbox/flows.py
 Comment: 
 
 Filename: streamlit_chatbox/messages.py
 Comment: 
 
-Filename: streamlit_chatbox-1.1.0.dist-info/METADATA
+Filename: streamlit_chatbox-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_chatbox-1.1.0.dist-info/WHEEL
+Filename: streamlit_chatbox-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_chatbox-1.1.0.dist-info/top_level.txt
+Filename: streamlit_chatbox-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_chatbox-1.1.0.dist-info/RECORD
+Filename: streamlit_chatbox-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_chatbox/messages.py

```diff
@@ -1,26 +1,42 @@
 from streamlit_chatbox.elements import *
 import time
 
 
 class ChatBox:
     def __init__(
         self,
-        session_name: str = "messages",
+        chat_name: str = "default",
+        session_key: str = "messages",
         user_avatar: str = "user",
         assistant_avatar: str = "assistant",
+        greetings: Union[str, OutputElement, List[Union[str, OutputElement]]] = [],
     ) -> None:
-        self._session_name = session_name
+        self._chat_name = chat_name
+        self._session_key = session_key
         self._user_avatar = user_avatar
         self._assistant_avatar = assistant_avatar
-        st.session_state.setdefault(self._session_name, [])
+        if not isinstance(greetings, list):
+            greetings = [greetings]
+        for i, greeting in enumerate(greetings):
+            if isinstance(greeting, str):
+                greetings[i] = Markdown(greeting)
+        self._greetings = greetings
+        st.session_state.setdefault(
+            self._session_key,
+            {self._chat_name: self._greetings},
+        )
+
+    def use_chat_name(self, name: str ="default") -> None:
+        self._chat_name = name
+        self.session_state[self._session_key].setdefault(name, [self._greetings])
 
     @property
-    def history(self):
-        return st.session_state.get(self._session_name, [])
+    def history(self) -> List:
+        return st.session_state.get(self._session_key).get(self._chat_name)
 
     def filter_history(
         self,
         history_len: int,
         filter: Callable = None,
     ) -> List:
         def default_filter(index, msg):
@@ -42,14 +58,19 @@
             if filtered is not None:
                 result.insert(0, filtered)
                 if len(result) >= history_len:
                     break
 
         return result
 
+    # def export2md(self, chat_name="default", filter=None):
+    #     lines = []
+    #     for msg in self.history:
+    #         lines.append()
+
     def _prepare_elements(
         self,
         elements: Union[OutputElement, str, List[Union[OutputElement, str]]],
     ) -> List[OutputElement]:
         if isinstance(elements, str):
             elements = [Markdown(elements)]
         elif isinstance(elements, OutputElement):
```

## Comparing `streamlit_chatbox-1.1.0.dist-info/METADATA` & `streamlit_chatbox-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chatbox
-Version: 1.1.0
+Version: 1.1.1
 Summary: A chat box and some helpful tools used to build chatbot app with streamlit
 Home-page: https://github.com/liunux4odoo/streamlit-chatbox
 Author: liunux
 Author-email: liunux@qq.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit (>=1.24.0)
```

## Comparing `streamlit_chatbox-1.1.0.dist-info/RECORD` & `streamlit_chatbox-1.1.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 streamlit_chatbox/__init__.py,sha256=okS4bZ1sk5ma0Nawlw07pLxVR_INKIqCQQFqvzkzR4A,392
 streamlit_chatbox/elements.py,sha256=G5qNHFANT_KgLtZ9BMDZ7rcCFx6gmoeXaomMfF-3iFU,4431
 streamlit_chatbox/flows.py,sha256=RvtStf1em9vGPp_sj8V7xHKbBiI5_p58RAFuvEMq2-c,323
-streamlit_chatbox/messages.py,sha256=U549KtBonkt6yOYvbkymCcHl640P-HEAmEv2WPa-2Es,4423
-streamlit_chatbox-1.1.0.dist-info/METADATA,sha256=UxBfVIzIRlyy0eKCN0Z33DbnxwhQe0ziyD22hqchWTM,4417
-streamlit_chatbox-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-streamlit_chatbox-1.1.0.dist-info/top_level.txt,sha256=YX62-ytEEAz8BjRqwDQAYXyMt85LDTHatfKhx178XKs,18
-streamlit_chatbox-1.1.0.dist-info/RECORD,,
+streamlit_chatbox/messages.py,sha256=rlUVkiomINQhlhY0R2ndKRnq9enGy5fmYfbdDphKYH0,5264
+streamlit_chatbox-1.1.1.dist-info/METADATA,sha256=kidjdOYMLlmeVB3u3TdRUbol1l0L-NTsHye6AX1EHRg,4417
+streamlit_chatbox-1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+streamlit_chatbox-1.1.1.dist-info/top_level.txt,sha256=YX62-ytEEAz8BjRqwDQAYXyMt85LDTHatfKhx178XKs,18
+streamlit_chatbox-1.1.1.dist-info/RECORD,,
```

