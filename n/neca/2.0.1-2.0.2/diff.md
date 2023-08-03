# Comparing `tmp/neca-2.0.1.tar.gz` & `tmp/neca-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neca-2.0.1.tar", last modified: Thu Aug  3 17:14:46 2023, max compression
+gzip compressed data, was "neca-2.0.2.tar", last modified: Thu Aug  3 17:36:12 2023, max compression
```

## Comparing `neca-2.0.1.tar` & `neca-2.0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 17:14:46.317241 neca-2.0.1/
--rw-rw-rw-   0        0        0     1067 2023-07-28 12:22:43.000000 neca-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     1871 2023-08-03 17:14:46.316241 neca-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      926 2023-05-04 14:26:21.000000 neca-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 17:14:46.280751 neca-2.0.1/neca/
-drwxrwxrwx   0        0        0        0 2023-08-03 17:14:46.315241 neca-2.0.1/neca/neca.egg-info/
--rw-rw-rw-   0        0        0     1871 2023-08-03 17:14:46.000000 neca-2.0.1/neca/neca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-08-03 17:14:46.000000 neca-2.0.1/neca/neca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 17:14:46.000000 neca-2.0.1/neca/neca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-08-03 17:14:46.000000 neca-2.0.1/neca/neca.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-08-03 17:14:46.000000 neca-2.0.1/neca/neca.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 17:14:46.000000 neca-2.0.1/neca/neca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       92 2023-08-03 16:46:23.000000 neca-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-03 17:14:46.317241 neca-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1895 2023-08-03 17:10:56.000000 neca-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 17:36:12.934214 neca-2.0.2/
+-rw-rw-rw-   0        0        0     1067 2023-07-28 12:22:43.000000 neca-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1871 2023-08-03 17:36:12.933212 neca-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      926 2023-05-04 14:26:21.000000 neca-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 17:36:12.931214 neca-2.0.2/neca.egg-info/
+-rw-rw-rw-   0        0        0     1871 2023-08-03 17:36:12.000000 neca-2.0.2/neca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-08-03 17:36:12.000000 neca-2.0.2/neca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 17:36:12.000000 neca-2.0.2/neca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 17:36:12.000000 neca-2.0.2/neca.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-08-03 17:36:12.000000 neca-2.0.2/neca.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 17:36:12.000000 neca-2.0.2/neca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       92 2023-08-03 16:46:23.000000 neca-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 17:36:12.934214 neca-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1894 2023-08-03 17:35:30.000000 neca-2.0.2/setup.py
```

### Comparing `neca-2.0.1/LICENSE` & `neca-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neca-2.0.1/PKG-INFO` & `neca-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neca
-Version: 2.0.1
+Version: 2.0.2
 Summary: ECA: Event Condition Action 
 Home-page: https://github.com/NiekAukes/eca2
 Author: Niek Aukes
 Author-email: niek.aukes@gmail.com
 Project-URL: Bug Reports, https://github.com/NiekAukes/eca2/issues
 Project-URL: Source, https://github.com/NiekAukes/eca2
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `neca-2.0.1/README.md` & `neca-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `neca-2.0.1/neca/neca.egg-info/PKG-INFO` & `neca-2.0.2/neca.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neca
-Version: 2.0.1
+Version: 2.0.2
 Summary: ECA: Event Condition Action 
 Home-page: https://github.com/NiekAukes/eca2
 Author: Niek Aukes
 Author-email: niek.aukes@gmail.com
 Project-URL: Bug Reports, https://github.com/NiekAukes/eca2/issues
 Project-URL: Source, https://github.com/NiekAukes/eca2
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `neca-2.0.1/setup.py` & `neca-2.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "flask",
     "flask-socketio", # ?
     "flask-sock"
 ]
 
 setup(
     name='neca',
-    version='2.0.1',
+    version='2.0.2',
     description='ECA: Event Condition Action ',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/NiekAukes/eca2',
     author='Niek Aukes',
     author_email="niek.aukes@gmail.com",
     classifiers=[  # Optional
@@ -36,21 +36,21 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
     
     packages=find_packages(where="eca"),  # Required
     python_requires=">=3.7, <4",
-    package_dir={"": "neca"},
+    package_dir={"neca": "neca"},
     # read from requirements.txt
     install_requires=requirements,
     
     entry_points={
         "console_scripts": [
-            "neca=neca.neca:commandline",
+            "neca=neca:commandline",
         ]
     },
 
     project_urls={  # Optional
         "Bug Reports": "https://github.com/NiekAukes/eca2/issues",
         "Source": "https://github.com/NiekAukes/eca2"
     }
```

