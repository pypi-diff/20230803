# Comparing `tmp/streamlit_chatbox-1.1.3-py3-none-any.whl.zip` & `tmp/streamlit_chatbox-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6319 bytes, number of entries: 8
+Zip file size: 6425 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      392 b- defN 23-Jul-30 13:49 streamlit_chatbox/__init__.py
 -rw-rw-rw-  2.0 fat     4431 b- defN 23-Aug-01 03:38 streamlit_chatbox/elements.py
 -rw-rw-rw-  2.0 fat      323 b- defN 23-Jul-31 01:37 streamlit_chatbox/flows.py
--rw-rw-rw-  2.0 fat     5589 b- defN 23-Aug-03 05:03 streamlit_chatbox/messages.py
--rw-rw-rw-  2.0 fat     4417 b- defN 23-Aug-03 05:07 streamlit_chatbox-1.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 05:07 streamlit_chatbox-1.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-03 05:07 streamlit_chatbox-1.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      677 b- defN 23-Aug-03 05:07 streamlit_chatbox-1.1.3.dist-info/RECORD
-8 files, 15939 bytes uncompressed, 5127 bytes compressed:  67.8%
+-rw-rw-rw-  2.0 fat     6118 b- defN 23-Aug-03 06:09 streamlit_chatbox/messages.py
+-rw-rw-rw-  2.0 fat     4417 b- defN 23-Aug-03 06:39 streamlit_chatbox-1.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 06:39 streamlit_chatbox-1.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-03 06:39 streamlit_chatbox-1.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      677 b- defN 23-Aug-03 06:39 streamlit_chatbox-1.1.4.dist-info/RECORD
+8 files, 16468 bytes uncompressed, 5233 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: streamlit_chatbox/flows.py
 Comment: 
 
 Filename: streamlit_chatbox/messages.py
 Comment: 
 
-Filename: streamlit_chatbox-1.1.3.dist-info/METADATA
+Filename: streamlit_chatbox-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_chatbox-1.1.3.dist-info/WHEEL
+Filename: streamlit_chatbox-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_chatbox-1.1.3.dist-info/top_level.txt
+Filename: streamlit_chatbox-1.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_chatbox-1.1.3.dist-info/RECORD
+Filename: streamlit_chatbox-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_chatbox/messages.py

```diff
@@ -17,26 +17,43 @@
         self._assistant_avatar = assistant_avatar
         if not isinstance(greetings, list):
             greetings = [greetings]
         for i, greeting in enumerate(greetings):
             if isinstance(greeting, str):
                 greetings[i] = Markdown(greeting)
         self._greetings = greetings
-
         if self._session_key not in st.session_state:
-            st.session_state[self._session_key] = {
-                self._chat_name: [{
-                    "role": "assistant",
-                    "elements": self._greetings,
-            }]}
+            st.session_state[self._session_key] = {}
+            self.reset_history()
+
+    def reset_history(self, name=None):
+        name = name or self._chat_name
+        st.session_state[self._session_key].update({
+            name: [{
+                "role": "assistant",
+                "elements": self._greetings,
+        }]})
 
     def use_chat_name(self, name: str ="default") -> None:
         self._chat_name = name
-        if name not in self.session_state[self._session_key]:
-            self.session_state[self._session_key] = self._greetings
+        if name not in st.session_state[self._session_key]:
+            self.reset_history(name)
+
+    def del_chat_name(self, name: str):
+        if name in st.session_state[self._session_key]:
+            msgs = st.session_state[self._session_key].pop(name)
+            self._chat_name=self.get_chat_names()[0]
+        return msgs
+
+    def get_chat_names(self):
+        return list(st.session_state[self._session_key].keys())
+
+    @property
+    def cur_chat_name(self):
+        return self._chat_name
 
     @property
     def history(self) -> List:
         return st.session_state.get(self._session_key).get(self._chat_name)
 
     def filter_history(
         self,
```

## Comparing `streamlit_chatbox-1.1.3.dist-info/METADATA` & `streamlit_chatbox-1.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chatbox
-Version: 1.1.3
+Version: 1.1.4
 Summary: A chat box and some helpful tools used to build chatbot app with streamlit
 Home-page: https://github.com/liunux4odoo/streamlit-chatbox
 Author: liunux
 Author-email: liunux@qq.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit (>=1.24.0)
```

## Comparing `streamlit_chatbox-1.1.3.dist-info/RECORD` & `streamlit_chatbox-1.1.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 streamlit_chatbox/__init__.py,sha256=okS4bZ1sk5ma0Nawlw07pLxVR_INKIqCQQFqvzkzR4A,392
 streamlit_chatbox/elements.py,sha256=G5qNHFANT_KgLtZ9BMDZ7rcCFx6gmoeXaomMfF-3iFU,4431
 streamlit_chatbox/flows.py,sha256=RvtStf1em9vGPp_sj8V7xHKbBiI5_p58RAFuvEMq2-c,323
-streamlit_chatbox/messages.py,sha256=OFAXVVwQYADz3yV3GMUqchNxmRJHJoej6gzAnmYuveQ,5589
-streamlit_chatbox-1.1.3.dist-info/METADATA,sha256=7gACp_QPxsvIgcVeXHKoM1enjgT6PXo7FGvcvFEfHnc,4417
-streamlit_chatbox-1.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-streamlit_chatbox-1.1.3.dist-info/top_level.txt,sha256=YX62-ytEEAz8BjRqwDQAYXyMt85LDTHatfKhx178XKs,18
-streamlit_chatbox-1.1.3.dist-info/RECORD,,
+streamlit_chatbox/messages.py,sha256=S2e74di03Anmf5GtAlzY-G4m6jQbuWxI_ErekCsUwcY,6118
+streamlit_chatbox-1.1.4.dist-info/METADATA,sha256=OJdJzRv5quwbMiFhL8gwa8XrCFnDllC7hWnPzIrOjBw,4417
+streamlit_chatbox-1.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+streamlit_chatbox-1.1.4.dist-info/top_level.txt,sha256=YX62-ytEEAz8BjRqwDQAYXyMt85LDTHatfKhx178XKs,18
+streamlit_chatbox-1.1.4.dist-info/RECORD,,
```

