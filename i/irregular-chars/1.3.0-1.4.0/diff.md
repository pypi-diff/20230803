# Comparing `tmp/irregular-chars-1.3.0.tar.gz` & `tmp/irregular-chars-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irregular-chars-1.3.0.tar", last modified: Sat Jun 24 21:19:07 2023, max compression
+gzip compressed data, was "irregular-chars-1.4.0.tar", last modified: Thu Aug  3 07:04:00 2023, max compression
```

## Comparing `irregular-chars-1.3.0.tar` & `irregular-chars-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 21:19:07.955727 irregular-chars-1.3.0/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-24 15:34:45.000000 irregular-chars-1.3.0/LICENSE
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      500 2023-06-24 21:19:07.955727 irregular-chars-1.3.0/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1983 2023-06-24 21:18:39.000000 irregular-chars-1.3.0/README.md
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 21:19:07.951727 irregular-chars-1.3.0/irregular_chars/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      523 2023-06-24 20:03:06.000000 irregular-chars-1.3.0/irregular_chars/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1450 2023-06-24 21:06:00.000000 irregular-chars-1.3.0/irregular_chars/ivs.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      719 2023-06-24 20:15:01.000000 irregular-chars-1.3.0/irregular_chars/space.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1503 2023-06-24 19:36:27.000000 irregular-chars-1.3.0/irregular_chars/splitted.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       95 2023-06-24 18:51:05.000000 irregular-chars-1.3.0/irregular_chars/unicodes.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      179 2023-06-24 20:06:39.000000 irregular-chars-1.3.0/irregular_chars/utils.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     3245 2023-06-24 19:58:04.000000 irregular-chars-1.3.0/irregular_chars/width.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 21:19:07.955727 irregular-chars-1.3.0/irregular_chars.egg-info/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      500 2023-06-24 21:19:07.000000 irregular-chars-1.3.0/irregular_chars.egg-info/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      503 2023-06-24 21:19:07.000000 irregular-chars-1.3.0/irregular_chars.egg-info/SOURCES.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-06-24 21:19:07.000000 irregular-chars-1.3.0/irregular_chars.egg-info/dependency_links.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       22 2023-06-24 21:19:07.000000 irregular-chars-1.3.0/irregular_chars.egg-info/top_level.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-06-24 21:19:07.955727 irregular-chars-1.3.0/setup.cfg
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      730 2023-06-24 21:18:59.000000 irregular-chars-1.3.0/setup.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 21:19:07.955727 irregular-chars-1.3.0/tests/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 14:44:31.000000 irregular-chars-1.3.0/tests/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     4126 2023-06-24 21:13:44.000000 irregular-chars-1.3.0/tests/test_ivs.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      966 2023-06-24 20:03:43.000000 irregular-chars-1.3.0/tests/test_sound_symbols.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      928 2023-06-24 19:04:32.000000 irregular-chars-1.3.0/tests/test_unicodes.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     7022 2023-06-24 20:58:27.000000 irregular-chars-1.3.0/tests/test_width.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      959 2023-06-24 20:03:34.000000 irregular-chars-1.3.0/tests/test_zero_width_spaces.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-08-03 07:04:00.646910 irregular-chars-1.4.0/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-24 15:34:45.000000 irregular-chars-1.4.0/LICENSE
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      500 2023-08-03 07:04:00.646910 irregular-chars-1.4.0/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1983 2023-06-24 21:18:39.000000 irregular-chars-1.4.0/README.md
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-08-03 07:04:00.642910 irregular-chars-1.4.0/irregular_chars/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      523 2023-06-24 20:03:06.000000 irregular-chars-1.4.0/irregular_chars/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1450 2023-06-24 21:06:00.000000 irregular-chars-1.4.0/irregular_chars/ivs.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      719 2023-06-24 20:15:01.000000 irregular-chars-1.4.0/irregular_chars/space.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1526 2023-08-03 07:03:11.000000 irregular-chars-1.4.0/irregular_chars/splitted.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       95 2023-06-24 18:51:05.000000 irregular-chars-1.4.0/irregular_chars/unicodes.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      179 2023-06-24 20:06:39.000000 irregular-chars-1.4.0/irregular_chars/utils.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     3245 2023-06-24 19:58:04.000000 irregular-chars-1.4.0/irregular_chars/width.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-08-03 07:04:00.642910 irregular-chars-1.4.0/irregular_chars.egg-info/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      500 2023-08-03 07:04:00.000000 irregular-chars-1.4.0/irregular_chars.egg-info/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      503 2023-08-03 07:04:00.000000 irregular-chars-1.4.0/irregular_chars.egg-info/SOURCES.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-08-03 07:04:00.000000 irregular-chars-1.4.0/irregular_chars.egg-info/dependency_links.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       22 2023-08-03 07:04:00.000000 irregular-chars-1.4.0/irregular_chars.egg-info/top_level.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-08-03 07:04:00.646910 irregular-chars-1.4.0/setup.cfg
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      730 2023-08-03 07:03:26.000000 irregular-chars-1.4.0/setup.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-08-03 07:04:00.646910 irregular-chars-1.4.0/tests/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 14:44:31.000000 irregular-chars-1.4.0/tests/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     4126 2023-06-24 21:13:44.000000 irregular-chars-1.4.0/tests/test_ivs.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      966 2023-06-24 20:03:43.000000 irregular-chars-1.4.0/tests/test_sound_symbols.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      928 2023-06-24 19:04:32.000000 irregular-chars-1.4.0/tests/test_unicodes.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     7022 2023-06-24 20:58:27.000000 irregular-chars-1.4.0/tests/test_width.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      959 2023-06-24 20:03:34.000000 irregular-chars-1.4.0/tests/test_zero_width_spaces.py
```

### Comparing `irregular-chars-1.3.0/LICENSE` & `irregular-chars-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `irregular-chars-1.3.0/README.md` & `irregular-chars-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `irregular-chars-1.3.0/irregular_chars/__init__.py` & `irregular-chars-1.4.0/irregular_chars/__init__.py`

 * *Files identical despite different names*

### Comparing `irregular-chars-1.3.0/irregular_chars/ivs.py` & `irregular-chars-1.4.0/irregular_chars/ivs.py`

 * *Files identical despite different names*

### Comparing `irregular-chars-1.3.0/irregular_chars/space.py` & `irregular-chars-1.4.0/irregular_chars/space.py`

 * *Files identical despite different names*

### Comparing `irregular-chars-1.3.0/irregular_chars/splitted.py` & `irregular-chars-1.4.0/irregular_chars/splitted.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .utils import replace_pair
 
 SOUND_SYMBOL_VARIATIONS = [
+    ("ヴ", "ヴ"),
     ("ガ", "ガ"),
     ("ギ", "ギ"),
     ("グ", "グ"),
     ("ゲ", "ゲ"),
     ("ゴ", "ゴ"),
     ("が", "が"),
     ("ぎ", "ぎ"),
```

### Comparing `irregular-chars-1.3.0/irregular_chars/width.py` & `irregular-chars-1.4.0/irregular_chars/width.py`

 * *Files identical despite different names*

### Comparing `irregular-chars-1.3.0/setup.py` & `irregular-chars-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="irregular-chars",
-    version="1.3.0",
+    version="1.4.0",
     description="A library for cleaning text, such as removing zero-width characters or"
     "converting full-width characters to half-width",
     packages=find_packages(),
     install_requires=[],
     classifiers=[  # パッケージのメタデータ（詳細は https://pypi.org/classifiers/ を参照）
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
```

### Comparing `irregular-chars-1.3.0/tests/test_ivs.py` & `irregular-chars-1.4.0/tests/test_ivs.py`

 * *Files identical despite different names*

### Comparing `irregular-chars-1.3.0/tests/test_sound_symbols.py` & `irregular-chars-1.4.0/tests/test_sound_symbols.py`

 * *Files identical despite different names*

### Comparing `irregular-chars-1.3.0/tests/test_unicodes.py` & `irregular-chars-1.4.0/tests/test_unicodes.py`

 * *Files identical despite different names*

### Comparing `irregular-chars-1.3.0/tests/test_width.py` & `irregular-chars-1.4.0/tests/test_width.py`

 * *Files identical despite different names*

### Comparing `irregular-chars-1.3.0/tests/test_zero_width_spaces.py` & `irregular-chars-1.4.0/tests/test_zero_width_spaces.py`

 * *Files identical despite different names*

