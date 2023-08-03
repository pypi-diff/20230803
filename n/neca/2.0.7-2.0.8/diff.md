# Comparing `tmp/neca-2.0.7.tar.gz` & `tmp/neca-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neca-2.0.7.tar", last modified: Thu Aug  3 18:00:56 2023, max compression
+gzip compressed data, was "neca-2.0.8.tar", last modified: Thu Aug  3 18:23:04 2023, max compression
```

## Comparing `neca-2.0.7.tar` & `neca-2.0.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 18:00:56.009266 neca-2.0.7/
--rw-rw-rw-   0        0        0     1067 2023-07-28 12:22:43.000000 neca-2.0.7/LICENSE
--rw-rw-rw-   0        0        0     1871 2023-08-03 18:00:56.008263 neca-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      926 2023-05-04 14:26:21.000000 neca-2.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 18:00:55.984866 neca-2.0.7/neca/
--rw-rw-rw-   0        0        0     3402 2023-08-03 17:13:03.000000 neca-2.0.7/neca/__init__.py
--rw-rw-rw-   0        0        0    10020 2023-08-03 17:53:15.000000 neca-2.0.7/neca/events.py
--rw-rw-rw-   0        0        0     3816 2023-08-03 17:19:47.000000 neca-2.0.7/neca/generators.py
--rw-rw-rw-   0        0        0      949 2023-05-04 17:08:44.000000 neca-2.0.7/neca/log.py
--rw-rw-rw-   0        0        0     1306 2023-05-04 20:11:12.000000 neca-2.0.7/neca/session.py
--rw-rw-rw-   0        0        0      503 2023-08-03 17:19:47.000000 neca-2.0.7/neca/settings.py
-drwxrwxrwx   0        0        0        0 2023-08-03 18:00:56.007271 neca-2.0.7/neca.egg-info/
--rw-rw-rw-   0        0        0     1871 2023-08-03 18:00:55.000000 neca-2.0.7/neca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-08-03 18:00:55.000000 neca-2.0.7/neca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 18:00:55.000000 neca-2.0.7/neca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 18:00:55.000000 neca-2.0.7/neca.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       54 2023-08-03 18:00:55.000000 neca-2.0.7/neca.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-03 18:00:55.000000 neca-2.0.7/neca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       92 2023-08-03 16:46:23.000000 neca-2.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-03 18:00:56.009266 neca-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1976 2023-08-03 18:00:41.000000 neca-2.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 18:23:04.884920 neca-2.0.8/
+-rw-rw-rw-   0        0        0     1067 2023-07-28 12:22:43.000000 neca-2.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1871 2023-08-03 18:23:04.883940 neca-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      926 2023-05-04 14:26:21.000000 neca-2.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 18:23:04.853701 neca-2.0.8/neca/
+-rw-rw-rw-   0        0        0      845 2023-08-03 18:15:50.000000 neca-2.0.8/neca/__init__.py
+-rw-rw-rw-   0        0        0     2575 2023-08-03 18:20:31.000000 neca-2.0.8/neca/__main__.py
+-rw-rw-rw-   0        0        0    10020 2023-08-03 17:53:15.000000 neca-2.0.8/neca/events.py
+-rw-rw-rw-   0        0        0     3816 2023-08-03 17:19:47.000000 neca-2.0.8/neca/generators.py
+-rw-rw-rw-   0        0        0      949 2023-05-04 17:08:44.000000 neca-2.0.8/neca/log.py
+-rw-rw-rw-   0        0        0     1306 2023-05-04 20:11:12.000000 neca-2.0.8/neca/session.py
+-rw-rw-rw-   0        0        0      503 2023-08-03 17:19:47.000000 neca-2.0.8/neca/settings.py
+drwxrwxrwx   0        0        0        0 2023-08-03 18:23:04.882238 neca-2.0.8/neca.egg-info/
+-rw-rw-rw-   0        0        0     1871 2023-08-03 18:23:04.000000 neca-2.0.8/neca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-08-03 18:23:04.000000 neca-2.0.8/neca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 18:23:04.000000 neca-2.0.8/neca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-08-03 18:23:04.000000 neca-2.0.8/neca.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       54 2023-08-03 18:23:04.000000 neca-2.0.8/neca.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-03 18:23:04.000000 neca-2.0.8/neca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       92 2023-08-03 16:46:23.000000 neca-2.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 18:23:04.884920 neca-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1977 2023-08-03 18:22:49.000000 neca-2.0.8/setup.py
```

### Comparing `neca-2.0.7/LICENSE` & `neca-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `neca-2.0.7/PKG-INFO` & `neca-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neca
-Version: 2.0.7
+Version: 2.0.8
 Summary: ECA: Event Condition Action 
 Home-page: https://github.com/NiekAukes/eca2
 Author: Niek Aukes
 Author-email: niek.aukes@gmail.com
 Project-URL: Bug Reports, https://github.com/NiekAukes/eca2/issues
 Project-URL: Source, https://github.com/NiekAukes/eca2
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `neca-2.0.7/README.md` & `neca-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `neca-2.0.7/neca/events.py` & `neca-2.0.8/neca/events.py`

 * *Files identical despite different names*

### Comparing `neca-2.0.7/neca/generators.py` & `neca-2.0.8/neca/generators.py`

 * *Files identical despite different names*

### Comparing `neca-2.0.7/neca/log.py` & `neca-2.0.8/neca/log.py`

 * *Files identical despite different names*

### Comparing `neca-2.0.7/neca/session.py` & `neca-2.0.8/neca/session.py`

 * *Files identical despite different names*

### Comparing `neca-2.0.7/neca.egg-info/PKG-INFO` & `neca-2.0.8/neca.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neca
-Version: 2.0.7
+Version: 2.0.8
 Summary: ECA: Event Condition Action 
 Home-page: https://github.com/NiekAukes/eca2
 Author: Niek Aukes
 Author-email: niek.aukes@gmail.com
 Project-URL: Bug Reports, https://github.com/NiekAukes/eca2/issues
 Project-URL: Source, https://github.com/NiekAukes/eca2
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `neca-2.0.7/setup.py` & `neca-2.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "PyInquirer",
     "rich",
     "typer",
 ]
 
 setup(
     name='neca',
-    version='2.0.7',
+    version='2.0.8',
     description='ECA: Event Condition Action ',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/NiekAukes/eca2',
     author='Niek Aukes',
     author_email="niek.aukes@gmail.com",
     classifiers=[  # Optional
@@ -49,15 +49,15 @@
 
     package_data={
         "neca": ["templates/*"],
     },
     
     entry_points={
         "console_scripts": [
-            "neca=neca:commandline",
+            "neca=neca.__main__:cli",
         ]
     },
 
     project_urls={  # Optional
         "Bug Reports": "https://github.com/NiekAukes/eca2/issues",
         "Source": "https://github.com/NiekAukes/eca2"
     }
```

