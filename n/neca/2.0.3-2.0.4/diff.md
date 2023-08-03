# Comparing `tmp/neca-2.0.3.tar.gz` & `tmp/neca-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neca-2.0.3.tar", last modified: Thu Aug  3 17:42:53 2023, max compression
+gzip compressed data, was "neca-2.0.4.tar", last modified: Thu Aug  3 17:45:28 2023, max compression
```

## Comparing `neca-2.0.3.tar` & `neca-2.0.4.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 17:42:53.822120 neca-2.0.3/
--rw-rw-rw-   0        0        0     1067 2023-07-28 12:22:43.000000 neca-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     1871 2023-08-03 17:42:53.820985 neca-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      926 2023-05-04 14:26:21.000000 neca-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 17:42:53.819974 neca-2.0.3/neca.egg-info/
--rw-rw-rw-   0        0        0     1871 2023-08-03 17:42:53.000000 neca-2.0.3/neca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-08-03 17:42:53.000000 neca-2.0.3/neca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 17:42:53.000000 neca-2.0.3/neca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 17:42:53.000000 neca-2.0.3/neca.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-08-03 17:42:53.000000 neca-2.0.3/neca.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 17:42:53.000000 neca-2.0.3/neca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       92 2023-08-03 16:46:23.000000 neca-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-03 17:42:53.822120 neca-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1895 2023-08-03 17:41:54.000000 neca-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 17:45:28.311248 neca-2.0.4/
+-rw-rw-rw-   0        0        0     1067 2023-07-28 12:22:43.000000 neca-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1871 2023-08-03 17:45:28.311248 neca-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      926 2023-05-04 14:26:21.000000 neca-2.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 17:45:28.285194 neca-2.0.4/neca/
+-rw-rw-rw-   0        0        0     3402 2023-08-03 17:13:03.000000 neca-2.0.4/neca/__init__.py
+-rw-rw-rw-   0        0        0    10024 2023-08-03 17:13:09.000000 neca-2.0.4/neca/events.py
+-rw-rw-rw-   0        0        0     3816 2023-08-03 17:19:47.000000 neca-2.0.4/neca/generators.py
+-rw-rw-rw-   0        0        0      949 2023-05-04 17:08:44.000000 neca-2.0.4/neca/logging.py
+-rw-rw-rw-   0        0        0     1306 2023-05-04 20:11:12.000000 neca-2.0.4/neca/session.py
+-rw-rw-rw-   0        0        0      503 2023-08-03 17:19:47.000000 neca-2.0.4/neca/settings.py
+drwxrwxrwx   0        0        0        0 2023-08-03 17:45:28.308248 neca-2.0.4/neca.egg-info/
+-rw-rw-rw-   0        0        0     1871 2023-08-03 17:45:28.000000 neca-2.0.4/neca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-08-03 17:45:28.000000 neca-2.0.4/neca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 17:45:28.000000 neca-2.0.4/neca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 17:45:28.000000 neca-2.0.4/neca.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-08-03 17:45:28.000000 neca-2.0.4/neca.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-03 17:45:28.000000 neca-2.0.4/neca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       92 2023-08-03 16:46:23.000000 neca-2.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 17:45:28.311248 neca-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1872 2023-08-03 17:45:09.000000 neca-2.0.4/setup.py
```

### Comparing `neca-2.0.3/LICENSE` & `neca-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neca-2.0.3/PKG-INFO` & `neca-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neca
-Version: 2.0.3
+Version: 2.0.4
 Summary: ECA: Event Condition Action 
 Home-page: https://github.com/NiekAukes/eca2
 Author: Niek Aukes
 Author-email: niek.aukes@gmail.com
 Project-URL: Bug Reports, https://github.com/NiekAukes/eca2/issues
 Project-URL: Source, https://github.com/NiekAukes/eca2
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `neca-2.0.3/README.md` & `neca-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `neca-2.0.3/neca.egg-info/PKG-INFO` & `neca-2.0.4/neca.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neca
-Version: 2.0.3
+Version: 2.0.4
 Summary: ECA: Event Condition Action 
 Home-page: https://github.com/NiekAukes/eca2
 Author: Niek Aukes
 Author-email: niek.aukes@gmail.com
 Project-URL: Bug Reports, https://github.com/NiekAukes/eca2/issues
 Project-URL: Source, https://github.com/NiekAukes/eca2
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `neca-2.0.3/setup.py` & `neca-2.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "flask",
     "flask-socketio", # ?
     "flask-sock"
 ]
 
 setup(
     name='neca',
-    version='2.0.3',
+    version='2.0.4',
     description='ECA: Event Condition Action ',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/NiekAukes/eca2',
     author='Niek Aukes',
     author_email="niek.aukes@gmail.com",
     classifiers=[  # Optional
@@ -34,15 +34,15 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
     
-    packages=find_packages(where="neca"),  # Required
+    packages=find_packages(),	
     python_requires=">=3.7, <4",
     package_dir={"neca": "neca"},
     # read from requirements.txt
     install_requires=requirements,
     
     entry_points={
         "console_scripts": [
```

