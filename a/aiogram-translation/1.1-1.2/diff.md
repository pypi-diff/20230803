# Comparing `tmp/aiogram_translation-1.1.tar.gz` & `tmp/aiogram_translation-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram_translation-1.1.tar", last modified: Sun Jun 25 17:54:14 2023, max compression
+gzip compressed data, was "aiogram_translation-1.2.tar", last modified: Sat Jul  8 15:37:45 2023, max compression
```

## Comparing `aiogram_translation-1.1.tar` & `aiogram_translation-1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 17:54:14.533846 aiogram_translation-1.1/
--rw-rw-rw-   0        0        0      559 2023-06-25 17:54:14.533846 aiogram_translation-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-25 17:10:11.000000 aiogram_translation-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 17:54:14.516843 aiogram_translation-1.1/aiogram_translation/
--rw-rw-rw-   0        0        0       89 2023-05-21 17:59:56.000000 aiogram_translation-1.1/aiogram_translation/__init__.py
--rw-rw-rw-   0        0        0     2242 2023-06-25 17:30:56.000000 aiogram_translation-1.1/aiogram_translation/_translator.py
--rw-rw-rw-   0        0        0      113 2023-05-21 17:38:51.000000 aiogram_translation-1.1/aiogram_translation/errors.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:54:14.532843 aiogram_translation-1.1/aiogram_translation/middlewares/
--rw-rw-rw-   0        0        0     1061 2023-06-25 17:26:42.000000 aiogram_translation-1.1/aiogram_translation/middlewares/TranslationMiddleware.py
--rw-rw-rw-   0        0        0       87 2023-05-21 17:59:56.000000 aiogram_translation-1.1/aiogram_translation/middlewares/__init__.py
--rw-rw-rw-   0        0        0      177 2023-06-25 17:10:12.000000 aiogram_translation-1.1/aiogram_translation/models.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:54:14.530840 aiogram_translation-1.1/aiogram_translation.egg-info/
--rw-rw-rw-   0        0        0      559 2023-06-25 17:54:14.000000 aiogram_translation-1.1/aiogram_translation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2023-06-25 17:54:14.000000 aiogram_translation-1.1/aiogram_translation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 17:54:14.000000 aiogram_translation-1.1/aiogram_translation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-25 17:54:14.000000 aiogram_translation-1.1/aiogram_translation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-25 17:54:14.000000 aiogram_translation-1.1/aiogram_translation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 17:54:14.533846 aiogram_translation-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1001 2023-06-25 17:52:27.000000 aiogram_translation-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:37:45.303111 aiogram_translation-1.2/
+-rw-rw-rw-   0        0        0      559 2023-07-08 15:37:45.303111 aiogram_translation-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-25 17:10:11.000000 aiogram_translation-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 15:37:45.285594 aiogram_translation-1.2/aiogram_translation/
+-rw-rw-rw-   0        0        0       89 2023-05-21 17:59:56.000000 aiogram_translation-1.2/aiogram_translation/__init__.py
+-rw-rw-rw-   0        0        0     2242 2023-06-25 17:30:56.000000 aiogram_translation-1.2/aiogram_translation/_translator.py
+-rw-rw-rw-   0        0        0      113 2023-05-21 17:38:51.000000 aiogram_translation-1.2/aiogram_translation/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:37:45.302117 aiogram_translation-1.2/aiogram_translation/middlewares/
+-rw-rw-rw-   0        0        0     1153 2023-07-08 15:35:06.000000 aiogram_translation-1.2/aiogram_translation/middlewares/TranslationMiddleware.py
+-rw-rw-rw-   0        0        0       87 2023-05-21 17:59:56.000000 aiogram_translation-1.2/aiogram_translation/middlewares/__init__.py
+-rw-rw-rw-   0        0        0      177 2023-06-25 17:10:12.000000 aiogram_translation-1.2/aiogram_translation/models.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:37:45.301114 aiogram_translation-1.2/aiogram_translation.egg-info/
+-rw-rw-rw-   0        0        0      559 2023-07-08 15:37:45.000000 aiogram_translation-1.2/aiogram_translation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2023-07-08 15:37:45.000000 aiogram_translation-1.2/aiogram_translation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 15:37:45.000000 aiogram_translation-1.2/aiogram_translation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-08 15:37:45.000000 aiogram_translation-1.2/aiogram_translation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-08 15:37:45.000000 aiogram_translation-1.2/aiogram_translation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 15:37:45.304113 aiogram_translation-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1001 2023-07-08 15:35:33.000000 aiogram_translation-1.2/setup.py
```

### Comparing `aiogram_translation-1.1/PKG-INFO` & `aiogram_translation-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram_translation
-Version: 1.1
+Version: 1.2
 Summary: Simple translation addon for AIOGram
 Home-page: UNKNOWN
 Author: sushka
 Author-email: barabum@duck.com
 License: UNKNOWN
 Keywords: python,aiogram,translation
 Platform: UNKNOWN
```

### Comparing `aiogram_translation-1.1/aiogram_translation/_translator.py` & `aiogram_translation-1.2/aiogram_translation/_translator.py`

 * *Files identical despite different names*

### Comparing `aiogram_translation-1.1/aiogram_translation/middlewares/TranslationMiddleware.py` & `aiogram_translation-1.2/aiogram_translation/middlewares/TranslationMiddleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,10 +17,13 @@
     ) -> Any:
         update = event.callback_query or event.message or event.channel_post\
                 or event.chat_member or event.edited_message or event.chat_join_request\
                 or event.chosen_inline_result or event.edited_channel_post\
                 or event.my_chat_member or event.poll_answer.user or event.shipping_query\
                 or event.pre_checkout_query
         user = update.from_user
-        code = user.language_code
+        if user:
+            code = user.language_code
+        else:
+            code = self._translator.get_default_key()
         data[self._key] = self._translator.get_translation(code)
         return await handler(event, data)
```

### Comparing `aiogram_translation-1.1/aiogram_translation.egg-info/PKG-INFO` & `aiogram_translation-1.2/aiogram_translation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram-translation
-Version: 1.1
+Version: 1.2
 Summary: Simple translation addon for AIOGram
 Home-page: UNKNOWN
 Author: sushka
 Author-email: barabum@duck.com
 License: UNKNOWN
 Keywords: python,aiogram,translation
 Platform: UNKNOWN
```

### Comparing `aiogram_translation-1.1/setup.py` & `aiogram_translation-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.01'
+VERSION = '1.02'
 DESCRIPTION = 'Simple translation addon for AIOGram'
 LONG_DESCRIPTION = 'This python package is a translation addon for AIOGram v3'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="aiogram_translation",
```

