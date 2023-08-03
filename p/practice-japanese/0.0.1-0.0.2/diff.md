# Comparing `tmp/practice_japanese-0.0.1.tar.gz` & `tmp/practice_japanese-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "practice_japanese-0.0.1.tar", last modified: Thu Aug  3 13:45:58 2023, max compression
+gzip compressed data, was "practice_japanese-0.0.2.tar", last modified: Thu Aug  3 13:52:01 2023, max compression
```

## Comparing `practice_japanese-0.0.1.tar` & `practice_japanese-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-03 13:45:58.457403 practice_japanese-0.0.1/
--rw-r--r--   0 heather   (1000) heather   (1000)    18092 2023-08-03 13:07:05.000000 practice_japanese-0.0.1/LICENSE
--rw-r--r--   0 heather   (1000) heather   (1000)       42 2023-08-03 13:44:43.000000 practice_japanese-0.0.1/MANIFEST.in
--rw-r--r--   0 heather   (1000) heather   (1000)     1507 2023-08-03 13:45:58.457403 practice_japanese-0.0.1/PKG-INFO
--rw-r--r--   0 heather   (1000) heather   (1000)     1045 2023-08-03 13:35:58.000000 practice_japanese-0.0.1/README.md
-drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-03 13:45:58.453403 practice_japanese-0.0.1/practice_japanese/
--rw-r--r--   0 heather   (1000) heather   (1000)        0 2023-08-03 13:07:41.000000 practice_japanese-0.0.1/practice_japanese/__init__.py
-drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-03 13:45:58.457403 practice_japanese-0.0.1/practice_japanese/character_sets/
--rw-r--r--   0 heather   (1000) heather   (1000)        0 2023-08-03 13:07:41.000000 practice_japanese-0.0.1/practice_japanese/character_sets/__init__.py
--rw-r--r--   0 heather   (1000) heather   (1000)      939 2023-08-03 13:14:07.000000 practice_japanese-0.0.1/practice_japanese/character_sets/hiragana.py
--rwxr-xr-x   0 heather   (1000) heather   (1000)     2895 2023-08-03 13:11:11.000000 practice_japanese-0.0.1/practice_japanese/character_statistics.py
--rw-r--r--   0 heather   (1000) heather   (1000)     1704 2023-08-03 13:31:36.000000 practice_japanese-0.0.1/practice_japanese/command_line.py
--rw-r--r--   0 heather   (1000) heather   (1000)       22 2023-08-03 13:07:41.000000 practice_japanese-0.0.1/practice_japanese/version.py
-drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-03 13:45:58.457403 practice_japanese-0.0.1/practice_japanese.egg-info/
--rw-r--r--   0 heather   (1000) heather   (1000)     1507 2023-08-03 13:45:58.000000 practice_japanese-0.0.1/practice_japanese.egg-info/PKG-INFO
--rw-r--r--   0 heather   (1000) heather   (1000)      488 2023-08-03 13:45:58.000000 practice_japanese-0.0.1/practice_japanese.egg-info/SOURCES.txt
--rw-r--r--   0 heather   (1000) heather   (1000)        1 2023-08-03 13:45:58.000000 practice_japanese-0.0.1/practice_japanese.egg-info/dependency_links.txt
--rw-r--r--   0 heather   (1000) heather   (1000)       73 2023-08-03 13:45:58.000000 practice_japanese-0.0.1/practice_japanese.egg-info/entry_points.txt
--rw-r--r--   0 heather   (1000) heather   (1000)       18 2023-08-03 13:45:58.000000 practice_japanese-0.0.1/practice_japanese.egg-info/top_level.txt
--rw-r--r--   0 heather   (1000) heather   (1000)        0 2023-08-03 13:43:25.000000 practice_japanese-0.0.1/requirements.txt
--rw-r--r--   0 heather   (1000) heather   (1000)       38 2023-08-03 13:45:58.457403 practice_japanese-0.0.1/setup.cfg
--rw-r--r--   0 heather   (1000) heather   (1000)     1294 2023-08-03 13:44:04.000000 practice_japanese-0.0.1/setup.py
+drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-03 13:52:01.095422 practice_japanese-0.0.2/
+-rw-r--r--   0 heather   (1000) heather   (1000)    18092 2023-08-03 13:07:05.000000 practice_japanese-0.0.2/LICENSE
+-rw-r--r--   0 heather   (1000) heather   (1000)       42 2023-08-03 13:44:43.000000 practice_japanese-0.0.2/MANIFEST.in
+-rw-r--r--   0 heather   (1000) heather   (1000)     1507 2023-08-03 13:52:01.095422 practice_japanese-0.0.2/PKG-INFO
+-rw-r--r--   0 heather   (1000) heather   (1000)     1045 2023-08-03 13:35:58.000000 practice_japanese-0.0.2/README.md
+drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-03 13:52:01.095422 practice_japanese-0.0.2/practice_japanese/
+-rw-r--r--   0 heather   (1000) heather   (1000)        0 2023-08-03 13:07:41.000000 practice_japanese-0.0.2/practice_japanese/__init__.py
+drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-03 13:52:01.095422 practice_japanese-0.0.2/practice_japanese/character_sets/
+-rw-r--r--   0 heather   (1000) heather   (1000)        0 2023-08-03 13:07:41.000000 practice_japanese-0.0.2/practice_japanese/character_sets/__init__.py
+-rw-r--r--   0 heather   (1000) heather   (1000)      939 2023-08-03 13:14:07.000000 practice_japanese-0.0.2/practice_japanese/character_sets/hiragana.py
+-rwxr-xr-x   0 heather   (1000) heather   (1000)     2895 2023-08-03 13:11:11.000000 practice_japanese-0.0.2/practice_japanese/character_statistics.py
+-rw-r--r--   0 heather   (1000) heather   (1000)     1694 2023-08-03 13:50:05.000000 practice_japanese-0.0.2/practice_japanese/command_line.py
+-rw-r--r--   0 heather   (1000) heather   (1000)       22 2023-08-03 13:51:06.000000 practice_japanese-0.0.2/practice_japanese/version.py
+drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-03 13:52:01.095422 practice_japanese-0.0.2/practice_japanese.egg-info/
+-rw-r--r--   0 heather   (1000) heather   (1000)     1507 2023-08-03 13:52:01.000000 practice_japanese-0.0.2/practice_japanese.egg-info/PKG-INFO
+-rw-r--r--   0 heather   (1000) heather   (1000)      488 2023-08-03 13:52:01.000000 practice_japanese-0.0.2/practice_japanese.egg-info/SOURCES.txt
+-rw-r--r--   0 heather   (1000) heather   (1000)        1 2023-08-03 13:52:01.000000 practice_japanese-0.0.2/practice_japanese.egg-info/dependency_links.txt
+-rw-r--r--   0 heather   (1000) heather   (1000)       73 2023-08-03 13:52:01.000000 practice_japanese-0.0.2/practice_japanese.egg-info/entry_points.txt
+-rw-r--r--   0 heather   (1000) heather   (1000)       18 2023-08-03 13:52:01.000000 practice_japanese-0.0.2/practice_japanese.egg-info/top_level.txt
+-rw-r--r--   0 heather   (1000) heather   (1000)        0 2023-08-03 13:43:25.000000 practice_japanese-0.0.2/requirements.txt
+-rw-r--r--   0 heather   (1000) heather   (1000)       38 2023-08-03 13:52:01.095422 practice_japanese-0.0.2/setup.cfg
+-rw-r--r--   0 heather   (1000) heather   (1000)     1294 2023-08-03 13:44:04.000000 practice_japanese-0.0.2/setup.py
```

### Comparing `practice_japanese-0.0.1/LICENSE` & `practice_japanese-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `practice_japanese-0.0.1/PKG-INFO` & `practice_japanese-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: practice_japanese
-Version: 0.0.1
+Version: 0.0.2
 Summary: Practice Japanese character sets.
 Home-page: https://github.com/hkeward/practice_japanese
 Author: Heather Ward
 Author-email: heather.ward13@gmail.com
 License: gpl-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `practice_japanese-0.0.1/README.md` & `practice_japanese-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `practice_japanese-0.0.1/practice_japanese/character_sets/hiragana.py` & `practice_japanese-0.0.2/practice_japanese/character_sets/hiragana.py`

 * *Files identical despite different names*

### Comparing `practice_japanese-0.0.1/practice_japanese/character_statistics.py` & `practice_japanese-0.0.2/practice_japanese/character_statistics.py`

 * *Files identical despite different names*

### Comparing `practice_japanese-0.0.1/practice_japanese/command_line.py` & `practice_japanese-0.0.2/practice_japanese/command_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import random
 from .character_statistics import CharacterStatistics
 from .character_sets.hiragana import Hiragana
 
 
 def main(args):
     character_set = Hiragana[args.character_set].value
-    character_statistics = CharacterStatistics(args.character_statistics_file)
+    character_statistics = CharacterStatistics(args.statistics_file)
     character_statistics.load()
 
     def signal_handler(*args):
         character_statistics.print_stats()
         character_statistics.write()
         exit(0)
```

### Comparing `practice_japanese-0.0.1/practice_japanese.egg-info/PKG-INFO` & `practice_japanese-0.0.2/practice_japanese.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: practice-japanese
-Version: 0.0.1
+Version: 0.0.2
 Summary: Practice Japanese character sets.
 Home-page: https://github.com/hkeward/practice_japanese
 Author: Heather Ward
 Author-email: heather.ward13@gmail.com
 License: gpl-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `practice_japanese-0.0.1/setup.py` & `practice_japanese-0.0.2/setup.py`

 * *Files identical despite different names*

