# Comparing `tmp/streamlit_chatbox-1.1.1-py3-none-any.whl.zip` & `tmp/streamlit_chatbox-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6280 bytes, number of entries: 8
+Zip file size: 6305 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      392 b- defN 23-Jul-30 13:49 streamlit_chatbox/__init__.py
 -rw-rw-rw-  2.0 fat     4431 b- defN 23-Aug-01 03:38 streamlit_chatbox/elements.py
 -rw-rw-rw-  2.0 fat      323 b- defN 23-Jul-31 01:37 streamlit_chatbox/flows.py
--rw-rw-rw-  2.0 fat     5264 b- defN 23-Aug-03 03:37 streamlit_chatbox/messages.py
--rw-rw-rw-  2.0 fat     4417 b- defN 23-Aug-03 03:41 streamlit_chatbox-1.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 03:41 streamlit_chatbox-1.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-03 03:41 streamlit_chatbox-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      677 b- defN 23-Aug-03 03:41 streamlit_chatbox-1.1.1.dist-info/RECORD
-8 files, 15614 bytes uncompressed, 5088 bytes compressed:  67.4%
+-rw-rw-rw-  2.0 fat     5439 b- defN 23-Aug-03 03:59 streamlit_chatbox/messages.py
+-rw-rw-rw-  2.0 fat     4417 b- defN 23-Aug-03 04:06 streamlit_chatbox-1.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 04:06 streamlit_chatbox-1.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-03 04:06 streamlit_chatbox-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      677 b- defN 23-Aug-03 04:06 streamlit_chatbox-1.1.2.dist-info/RECORD
+8 files, 15789 bytes uncompressed, 5113 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: streamlit_chatbox/flows.py
 Comment: 
 
 Filename: streamlit_chatbox/messages.py
 Comment: 
 
-Filename: streamlit_chatbox-1.1.1.dist-info/METADATA
+Filename: streamlit_chatbox-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_chatbox-1.1.1.dist-info/WHEEL
+Filename: streamlit_chatbox-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_chatbox-1.1.1.dist-info/top_level.txt
+Filename: streamlit_chatbox-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_chatbox-1.1.1.dist-info/RECORD
+Filename: streamlit_chatbox-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_chatbox/messages.py

```diff
@@ -17,22 +17,26 @@
         self._assistant_avatar = assistant_avatar
         if not isinstance(greetings, list):
             greetings = [greetings]
         for i, greeting in enumerate(greetings):
             if isinstance(greeting, str):
                 greetings[i] = Markdown(greeting)
         self._greetings = greetings
-        st.session_state.setdefault(
-            self._session_key,
-            {self._chat_name: self._greetings},
-        )
+
+        if self._session_key not in st.session_state:
+            st.session_state[self._session_key] = {
+                self._chat_name: [{
+                    "role": "assistant",
+                    "elements": self._greetings,
+            }]}
 
     def use_chat_name(self, name: str ="default") -> None:
         self._chat_name = name
-        self.session_state[self._session_key].setdefault(name, [self._greetings])
+        if name not in self.session_state[self._session_key]:
+            self.session_state[self._session_key] = self._greetings
 
     @property
     def history(self) -> List:
         return st.session_state.get(self._session_key).get(self._chat_name)
 
     def filter_history(
         self,
```

## Comparing `streamlit_chatbox-1.1.1.dist-info/METADATA` & `streamlit_chatbox-1.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chatbox
-Version: 1.1.1
+Version: 1.1.2
 Summary: A chat box and some helpful tools used to build chatbot app with streamlit
 Home-page: https://github.com/liunux4odoo/streamlit-chatbox
 Author: liunux
 Author-email: liunux@qq.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit (>=1.24.0)
```

