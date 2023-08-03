# Comparing `tmp/aiogram_translation-1.2.tar.gz` & `tmp/aiogram-translation-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram_translation-1.2.tar", last modified: Sat Jul  8 15:37:45 2023, max compression
+gzip compressed data, was "aiogram-translation-1.2.1.tar", last modified: Thu Aug  3 13:40:59 2023, max compression
```

## Comparing `aiogram_translation-1.2.tar` & `aiogram-translation-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 15:37:45.303111 aiogram_translation-1.2/
--rw-rw-rw-   0        0        0      559 2023-07-08 15:37:45.303111 aiogram_translation-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-25 17:10:11.000000 aiogram_translation-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 15:37:45.285594 aiogram_translation-1.2/aiogram_translation/
--rw-rw-rw-   0        0        0       89 2023-05-21 17:59:56.000000 aiogram_translation-1.2/aiogram_translation/__init__.py
--rw-rw-rw-   0        0        0     2242 2023-06-25 17:30:56.000000 aiogram_translation-1.2/aiogram_translation/_translator.py
--rw-rw-rw-   0        0        0      113 2023-05-21 17:38:51.000000 aiogram_translation-1.2/aiogram_translation/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:37:45.302117 aiogram_translation-1.2/aiogram_translation/middlewares/
--rw-rw-rw-   0        0        0     1153 2023-07-08 15:35:06.000000 aiogram_translation-1.2/aiogram_translation/middlewares/TranslationMiddleware.py
--rw-rw-rw-   0        0        0       87 2023-05-21 17:59:56.000000 aiogram_translation-1.2/aiogram_translation/middlewares/__init__.py
--rw-rw-rw-   0        0        0      177 2023-06-25 17:10:12.000000 aiogram_translation-1.2/aiogram_translation/models.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:37:45.301114 aiogram_translation-1.2/aiogram_translation.egg-info/
--rw-rw-rw-   0        0        0      559 2023-07-08 15:37:45.000000 aiogram_translation-1.2/aiogram_translation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2023-07-08 15:37:45.000000 aiogram_translation-1.2/aiogram_translation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 15:37:45.000000 aiogram_translation-1.2/aiogram_translation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-08 15:37:45.000000 aiogram_translation-1.2/aiogram_translation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-08 15:37:45.000000 aiogram_translation-1.2/aiogram_translation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 15:37:45.304113 aiogram_translation-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1001 2023-07-08 15:35:33.000000 aiogram_translation-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:40:59.481410 aiogram-translation-1.2.1/
+-rw-rw-rw-   0        0        0     4286 2023-08-03 13:40:59.481410 aiogram-translation-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3378 2023-08-03 13:37:25.000000 aiogram-translation-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 13:40:59.466406 aiogram-translation-1.2.1/aiogram_translation/
+-rw-rw-rw-   0        0        0       89 2023-05-21 17:59:56.000000 aiogram-translation-1.2.1/aiogram_translation/__init__.py
+-rw-rw-rw-   0        0        0     2242 2023-06-25 17:30:56.000000 aiogram-translation-1.2.1/aiogram_translation/_translator.py
+-rw-rw-rw-   0        0        0      113 2023-05-21 17:38:51.000000 aiogram-translation-1.2.1/aiogram_translation/errors.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:40:59.480409 aiogram-translation-1.2.1/aiogram_translation/middlewares/
+-rw-rw-rw-   0        0        0     1153 2023-07-08 15:35:06.000000 aiogram-translation-1.2.1/aiogram_translation/middlewares/TranslationMiddleware.py
+-rw-rw-rw-   0        0        0       87 2023-05-21 17:59:56.000000 aiogram-translation-1.2.1/aiogram_translation/middlewares/__init__.py
+-rw-rw-rw-   0        0        0      177 2023-06-25 17:10:12.000000 aiogram-translation-1.2.1/aiogram_translation/models.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:40:59.479405 aiogram-translation-1.2.1/aiogram_translation.egg-info/
+-rw-rw-rw-   0        0        0     4286 2023-08-03 13:40:59.000000 aiogram-translation-1.2.1/aiogram_translation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-08-03 13:40:59.000000 aiogram-translation-1.2.1/aiogram_translation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 13:40:59.000000 aiogram-translation-1.2.1/aiogram_translation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-08-03 13:40:59.000000 aiogram-translation-1.2.1/aiogram_translation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-03 13:40:59.000000 aiogram-translation-1.2.1/aiogram_translation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       54 2023-05-21 17:38:51.000000 aiogram-translation-1.2.1/requirements.txt
+-rw-rw-rw-   0        0        0     1000 2023-08-03 13:40:59.486406 aiogram-translation-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-07-13 17:40:00.000000 aiogram-translation-1.2.1/setup.py
```

### Comparing `aiogram_translation-1.2/aiogram_translation/_translator.py` & `aiogram-translation-1.2.1/aiogram_translation/_translator.py`

 * *Files identical despite different names*

### Comparing `aiogram_translation-1.2/aiogram_translation/middlewares/TranslationMiddleware.py` & `aiogram-translation-1.2.1/aiogram_translation/middlewares/TranslationMiddleware.py`

 * *Files identical despite different names*

