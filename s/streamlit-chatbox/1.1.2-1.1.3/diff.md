# Comparing `tmp/streamlit_chatbox-1.1.2-py3-none-any.whl.zip` & `tmp/streamlit_chatbox-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6305 bytes, number of entries: 8
+Zip file size: 6319 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      392 b- defN 23-Jul-30 13:49 streamlit_chatbox/__init__.py
 -rw-rw-rw-  2.0 fat     4431 b- defN 23-Aug-01 03:38 streamlit_chatbox/elements.py
 -rw-rw-rw-  2.0 fat      323 b- defN 23-Jul-31 01:37 streamlit_chatbox/flows.py
--rw-rw-rw-  2.0 fat     5439 b- defN 23-Aug-03 03:59 streamlit_chatbox/messages.py
--rw-rw-rw-  2.0 fat     4417 b- defN 23-Aug-03 04:06 streamlit_chatbox-1.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 04:06 streamlit_chatbox-1.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-03 04:06 streamlit_chatbox-1.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      677 b- defN 23-Aug-03 04:06 streamlit_chatbox-1.1.2.dist-info/RECORD
-8 files, 15789 bytes uncompressed, 5113 bytes compressed:  67.6%
+-rw-rw-rw-  2.0 fat     5589 b- defN 23-Aug-03 05:03 streamlit_chatbox/messages.py
+-rw-rw-rw-  2.0 fat     4417 b- defN 23-Aug-03 05:07 streamlit_chatbox-1.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 05:07 streamlit_chatbox-1.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-03 05:07 streamlit_chatbox-1.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      677 b- defN 23-Aug-03 05:07 streamlit_chatbox-1.1.3.dist-info/RECORD
+8 files, 15939 bytes uncompressed, 5127 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: streamlit_chatbox/flows.py
 Comment: 
 
 Filename: streamlit_chatbox/messages.py
 Comment: 
 
-Filename: streamlit_chatbox-1.1.2.dist-info/METADATA
+Filename: streamlit_chatbox-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_chatbox-1.1.2.dist-info/WHEEL
+Filename: streamlit_chatbox-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_chatbox-1.1.2.dist-info/top_level.txt
+Filename: streamlit_chatbox-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_chatbox-1.1.2.dist-info/RECORD
+Filename: streamlit_chatbox-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_chatbox/messages.py

```diff
@@ -84,32 +84,36 @@
                 e, str) else e for e in elements]
         return elements
 
     def user_say(
         self,
         elements: Union[OutputElement, str, List[Union[OutputElement, str]]],
         to_history: bool = True,
+        not_render: bool = False,
     ) -> List[OutputElement]:
         elements = self._prepare_elements(elements)
-        with st.chat_message("user", avatar=self._user_avatar):
-            for element in elements:
-                element()
+        if not not_render:
+            with st.chat_message("user", avatar=self._user_avatar):
+                for element in elements:
+                    element()
         if to_history:
             self.history.append({"role": "user", "elements": elements})
         return elements
 
     def ai_say(
         self,
         elements: Union[OutputElement, str, List[Union[OutputElement, str]]],
         to_history: bool = True,
+        not_render: bool = False,
     ) -> List[OutputElement]:
         elements = self._prepare_elements(elements)
-        with st.chat_message("assistant", avatar=self._assistant_avatar):
-            for element in elements:
-                element()
+        if not not_render:
+            with st.chat_message("assistant", avatar=self._assistant_avatar):
+                for element in elements:
+                    element()
         if to_history:
             self.history.append({"role": "assistant", "elements": elements})
         return elements
 
     def output_messages(self):
         for msg in self.history:
             avatar = self._user_avatar if msg["role"] == "user" else self._assistant_avatar
```

## Comparing `streamlit_chatbox-1.1.2.dist-info/METADATA` & `streamlit_chatbox-1.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chatbox
-Version: 1.1.2
+Version: 1.1.3
 Summary: A chat box and some helpful tools used to build chatbot app with streamlit
 Home-page: https://github.com/liunux4odoo/streamlit-chatbox
 Author: liunux
 Author-email: liunux@qq.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit (>=1.24.0)
```

## Comparing `streamlit_chatbox-1.1.2.dist-info/RECORD` & `streamlit_chatbox-1.1.3.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 streamlit_chatbox/__init__.py,sha256=okS4bZ1sk5ma0Nawlw07pLxVR_INKIqCQQFqvzkzR4A,392
 streamlit_chatbox/elements.py,sha256=G5qNHFANT_KgLtZ9BMDZ7rcCFx6gmoeXaomMfF-3iFU,4431
 streamlit_chatbox/flows.py,sha256=RvtStf1em9vGPp_sj8V7xHKbBiI5_p58RAFuvEMq2-c,323
-streamlit_chatbox/messages.py,sha256=pirSNYixJhwQeYG29d0xrm-GH-FC33UhIgVXoYfxlMA,5439
-streamlit_chatbox-1.1.2.dist-info/METADATA,sha256=Al3Dq0ELgIQpnhbN3ZiJxxHA9v0ndM-sUGDQzRn5Wpk,4417
-streamlit_chatbox-1.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-streamlit_chatbox-1.1.2.dist-info/top_level.txt,sha256=YX62-ytEEAz8BjRqwDQAYXyMt85LDTHatfKhx178XKs,18
-streamlit_chatbox-1.1.2.dist-info/RECORD,,
+streamlit_chatbox/messages.py,sha256=OFAXVVwQYADz3yV3GMUqchNxmRJHJoej6gzAnmYuveQ,5589
+streamlit_chatbox-1.1.3.dist-info/METADATA,sha256=7gACp_QPxsvIgcVeXHKoM1enjgT6PXo7FGvcvFEfHnc,4417
+streamlit_chatbox-1.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+streamlit_chatbox-1.1.3.dist-info/top_level.txt,sha256=YX62-ytEEAz8BjRqwDQAYXyMt85LDTHatfKhx178XKs,18
+streamlit_chatbox-1.1.3.dist-info/RECORD,,
```

