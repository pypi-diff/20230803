# Comparing `tmp/tokentrim-0.1.2.tar.gz` & `tmp/tokentrim-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokentrim-0.1.2.tar", max compression
+gzip compressed data, was "tokentrim-0.1.3.tar", max compression
```

## Comparing `tokentrim-0.1.2.tar` & `tokentrim-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1064 2023-07-29 23:24:50.484214 tokentrim-0.1.2/LICENSE
--rw-r--r--   0        0        0      355 2023-07-30 00:38:04.714219 tokentrim-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       27 2023-07-30 00:06:48.037573 tokentrim-0.1.2/tokentrim/__init__.py
--rw-r--r--   0        0        0     5490 2023-07-30 00:37:12.542314 tokentrim-0.1.2/tokentrim/tokentrim.py
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 tokentrim-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-29 23:24:50.484214 tokentrim-0.1.3/LICENSE
+-rw-r--r--   0        0        0      355 2023-08-03 19:49:40.309471 tokentrim-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-07-30 00:06:48.037573 tokentrim-0.1.3/tokentrim/__init__.py
+-rw-r--r--   0        0        0     5495 2023-08-03 19:49:24.087898 tokentrim-0.1.3/tokentrim/tokentrim.py
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 tokentrim-0.1.3/PKG-INFO
```

### Comparing `tokentrim-0.1.2/LICENSE` & `tokentrim-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tokentrim-0.1.2/tokentrim/tokentrim.py` & `tokentrim-0.1.3/tokentrim/tokentrim.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     )
 
   # Calculate the number of tokens
   num_tokens = 0
   for message in messages:
     num_tokens += tokens_per_message
     for key, value in message.items():
-      num_tokens += len(encoding.encode(value))
+      num_tokens += len(encoding.encode(str(value)))
       if key == "name":
         num_tokens += tokens_per_name
 
   num_tokens += 3
   return num_tokens
```

### Comparing `tokentrim-0.1.2/PKG-INFO` & `tokentrim-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokentrim
-Version: 0.1.2
+Version: 0.1.3
 Summary: Easily trim 'messages' arrays for use with GPTs.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

