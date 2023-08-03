# Comparing `tmp/remotion_lambda-4.0.15.tar.gz` & `tmp/remotion_lambda-4.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotion_lambda-4.0.15.tar", last modified: Tue Aug  1 07:01:51 2023, max compression
+gzip compressed data, was "remotion_lambda-4.0.16.tar", last modified: Thu Aug  3 07:56:00 2023, max compression
```

## Comparing `remotion_lambda-4.0.15.tar` & `remotion_lambda-4.0.16.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-01 07:01:51.957916 remotion_lambda-4.0.15/
--rw-r--r--   0 jonathanburger   (501) staff       (20)     2512 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/LICENSE
--rw-r--r--   0 jonathanburger   (501) staff       (20)      427 2023-08-01 07:01:51.957801 remotion_lambda-4.0.15/PKG-INFO
--rw-r--r--   0 jonathanburger   (501) staff       (20)       26 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/README.md
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-01 07:01:51.956724 remotion_lambda-4.0.15/remotion_lambda/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      202 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/remotion_lambda/__init__.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)     5252 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/remotion_lambda/models.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)     6064 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/remotion_lambda/remotionclient.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)       84 2023-08-01 06:56:26.000000 remotion_lambda-4.0.15/remotion_lambda/version.py
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-01 07:01:51.957153 remotion_lambda-4.0.15/remotion_lambda.egg-info/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      427 2023-08-01 07:01:51.000000 remotion_lambda-4.0.15/remotion_lambda.egg-info/PKG-INFO
--rw-r--r--   0 jonathanburger   (501) staff       (20)      384 2023-08-01 07:01:51.000000 remotion_lambda-4.0.15/remotion_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)        1 2023-08-01 07:01:51.000000 remotion_lambda-4.0.15/remotion_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-01 07:01:51.000000 remotion_lambda-4.0.15/remotion_lambda.egg-info/top_level.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-01 07:01:51.958026 remotion_lambda-4.0.15/setup.cfg
--rw-r--r--   0 jonathanburger   (501) staff       (20)      753 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/setup.py
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-01 07:01:51.957584 remotion_lambda-4.0.15/tests/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      131 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/tests/__init__.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)      474 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/tests/test_get_render_progress_client.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)      764 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/tests/test_render_client.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-03 07:56:00.861702 remotion_lambda-4.0.16/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     2512 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/LICENSE
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      427 2023-08-03 07:56:00.861584 remotion_lambda-4.0.16/PKG-INFO
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       26 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/README.md
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-03 07:56:00.860726 remotion_lambda-4.0.16/remotion_lambda/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      202 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/remotion_lambda/__init__.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     5252 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/remotion_lambda/models.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     6064 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/remotion_lambda/remotionclient.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       84 2023-08-03 07:29:54.000000 remotion_lambda-4.0.16/remotion_lambda/version.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-03 07:56:00.861110 remotion_lambda-4.0.16/remotion_lambda.egg-info/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      427 2023-08-03 07:56:00.000000 remotion_lambda-4.0.16/remotion_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      384 2023-08-03 07:56:00.000000 remotion_lambda-4.0.16/remotion_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)        1 2023-08-03 07:56:00.000000 remotion_lambda-4.0.16/remotion_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-03 07:56:00.000000 remotion_lambda-4.0.16/remotion_lambda.egg-info/top_level.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-03 07:56:00.861823 remotion_lambda-4.0.16/setup.cfg
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      753 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/setup.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-03 07:56:00.861440 remotion_lambda-4.0.16/tests/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      131 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/tests/__init__.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      474 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/tests/test_get_render_progress_client.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      764 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/tests/test_render_client.py
```

### Comparing `remotion_lambda-4.0.15/LICENSE` & `remotion_lambda-4.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.15/remotion_lambda/models.py` & `remotion_lambda-4.0.16/remotion_lambda/models.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.15/remotion_lambda/remotionclient.py` & `remotion_lambda-4.0.16/remotion_lambda/remotionclient.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.15/setup.py` & `remotion_lambda-4.0.16/setup.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.15/tests/test_render_client.py` & `remotion_lambda-4.0.16/tests/test_render_client.py`

 * *Files identical despite different names*

