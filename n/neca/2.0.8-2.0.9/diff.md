# Comparing `tmp/neca-2.0.8.tar.gz` & `tmp/neca-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neca-2.0.8.tar", last modified: Thu Aug  3 18:23:04 2023, max compression
+gzip compressed data, was "neca-2.0.9.tar", last modified: Thu Aug  3 19:16:28 2023, max compression
```

## Comparing `neca-2.0.8.tar` & `neca-2.0.9.tar`

### file list

```diff
@@ -1,22 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 18:23:04.884920 neca-2.0.8/
--rw-rw-rw-   0        0        0     1067 2023-07-28 12:22:43.000000 neca-2.0.8/LICENSE
--rw-rw-rw-   0        0        0     1871 2023-08-03 18:23:04.883940 neca-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      926 2023-05-04 14:26:21.000000 neca-2.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 18:23:04.853701 neca-2.0.8/neca/
--rw-rw-rw-   0        0        0      845 2023-08-03 18:15:50.000000 neca-2.0.8/neca/__init__.py
--rw-rw-rw-   0        0        0     2575 2023-08-03 18:20:31.000000 neca-2.0.8/neca/__main__.py
--rw-rw-rw-   0        0        0    10020 2023-08-03 17:53:15.000000 neca-2.0.8/neca/events.py
--rw-rw-rw-   0        0        0     3816 2023-08-03 17:19:47.000000 neca-2.0.8/neca/generators.py
--rw-rw-rw-   0        0        0      949 2023-05-04 17:08:44.000000 neca-2.0.8/neca/log.py
--rw-rw-rw-   0        0        0     1306 2023-05-04 20:11:12.000000 neca-2.0.8/neca/session.py
--rw-rw-rw-   0        0        0      503 2023-08-03 17:19:47.000000 neca-2.0.8/neca/settings.py
-drwxrwxrwx   0        0        0        0 2023-08-03 18:23:04.882238 neca-2.0.8/neca.egg-info/
--rw-rw-rw-   0        0        0     1871 2023-08-03 18:23:04.000000 neca-2.0.8/neca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-08-03 18:23:04.000000 neca-2.0.8/neca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 18:23:04.000000 neca-2.0.8/neca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-08-03 18:23:04.000000 neca-2.0.8/neca.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       54 2023-08-03 18:23:04.000000 neca-2.0.8/neca.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-03 18:23:04.000000 neca-2.0.8/neca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       92 2023-08-03 16:46:23.000000 neca-2.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-03 18:23:04.884920 neca-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1977 2023-08-03 18:22:49.000000 neca-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:16:28.133981 neca-2.0.9/
+-rw-rw-rw-   0        0        0     1067 2023-07-28 12:22:43.000000 neca-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0       36 2023-08-03 19:15:01.000000 neca-2.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1871 2023-08-03 19:16:28.133981 neca-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      926 2023-05-04 14:26:21.000000 neca-2.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 19:16:28.097976 neca-2.0.9/neca/
+-rw-rw-rw-   0        0        0      845 2023-08-03 18:15:50.000000 neca-2.0.9/neca/__init__.py
+-rw-rw-rw-   0        0        0     2575 2023-08-03 18:20:31.000000 neca-2.0.9/neca/__main__.py
+-rw-rw-rw-   0        0        0    10020 2023-08-03 17:53:15.000000 neca-2.0.9/neca/events.py
+-rw-rw-rw-   0        0        0     3816 2023-08-03 17:19:47.000000 neca-2.0.9/neca/generators.py
+-rw-rw-rw-   0        0        0      949 2023-05-04 17:08:44.000000 neca-2.0.9/neca/log.py
+-rw-rw-rw-   0        0        0     1306 2023-05-04 20:11:12.000000 neca-2.0.9/neca/session.py
+-rw-rw-rw-   0        0        0      503 2023-08-03 17:19:47.000000 neca-2.0.9/neca/settings.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:16:28.072707 neca-2.0.9/neca/templates/
+drwxrwxrwx   0        0        0        0 2023-08-03 19:16:28.108984 neca-2.0.9/neca/templates/basic/
+-rw-rw-rw-   0        0        0      734 2023-08-03 17:53:15.000000 neca-2.0.9/neca/templates/basic/main.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:16:28.074697 neca-2.0.9/neca/templates/basic/static/
+drwxrwxrwx   0        0        0        0 2023-08-03 19:16:28.119996 neca-2.0.9/neca/templates/basic/static/lib/
+-rw-rw-rw-   0        0        0     2087 2023-08-02 18:17:53.000000 neca-2.0.9/neca/templates/basic/static/lib/barchart.js
+-rw-rw-rw-   0        0        0     1204 2023-05-05 13:01:19.000000 neca-2.0.9/neca/templates/basic/static/lib/core.js
+-rw-rw-rw-   0        0        0     2205 2023-05-05 20:35:33.000000 neca-2.0.9/neca/templates/basic/static/lib/form.js
+-rw-rw-rw-   0        0        0     4169 2023-05-05 18:40:19.000000 neca-2.0.9/neca/templates/basic/static/lib/linechart.js
+-rw-rw-rw-   0        0        0      527 2023-05-05 19:40:39.000000 neca-2.0.9/neca/templates/basic/static/lib/log.js
+-rw-rw-rw-   0        0        0      357 2023-08-03 16:21:51.000000 neca-2.0.9/neca/templates/basic/static/lib/new_block.js
+-rw-rw-rw-   0        0        0     2087 2023-07-30 16:06:18.000000 neca-2.0.9/neca/templates/basic/static/lib/piechart.js
+-rw-rw-rw-   0        0        0     4173 2023-05-05 19:48:19.000000 neca-2.0.9/neca/templates/basic/static/lib/rollingchart.js
+-rw-rw-rw-   0        0        0     3481 2023-05-05 14:49:35.000000 neca-2.0.9/neca/templates/basic/static/lib/tweets.js
+drwxrwxrwx   0        0        0        0 2023-08-03 19:16:28.120983 neca-2.0.9/neca/templates/basic/static/res/
+-rw-rw-rw-   0        0        0   349649 2023-05-05 14:24:35.000000 neca-2.0.9/neca/templates/basic/static/res/DefaultTwitterUser.png
+drwxrwxrwx   0        0        0        0 2023-08-03 19:16:28.127983 neca-2.0.9/neca/templates/basic/static/style/
+-rw-rw-rw-   0        0        0     5239 2023-05-05 18:43:03.000000 neca-2.0.9/neca/templates/basic/static/style/grid.css
+-rw-rw-rw-   0        0        0     1231 2023-05-05 18:43:03.000000 neca-2.0.9/neca/templates/basic/static/style/layout.css
+-rw-rw-rw-   0        0        0     2616 2023-05-05 18:43:03.000000 neca-2.0.9/neca/templates/basic/static/style/theme.css
+-rw-rw-rw-   0        0        0      694 2023-05-05 14:58:51.000000 neca-2.0.9/neca/templates/basic/static/style/tweet.css
+-rw-rw-rw-   0        0        0     1246 2023-05-05 18:43:03.000000 neca-2.0.9/neca/templates/basic/static/style/wordcloud.css
+drwxrwxrwx   0        0        0        0 2023-08-03 19:16:28.132980 neca-2.0.9/neca/templates/basic/templates/
+-rw-rw-rw-   0        0        0     3837 2023-05-06 15:47:02.000000 neca-2.0.9/neca/templates/basic/templates/index.html
+-rw-rw-rw-   0        0        0      800 2023-05-05 19:41:55.000000 neca-2.0.9/neca/templates/basic/templates/log.html
+-rw-rw-rw-   0        0        0     1539 2023-05-05 13:36:07.000000 neca-2.0.9/neca/templates/basic/templates/socket.html
+-rw-rw-rw-   0        0        0      751 2023-05-05 14:19:46.000000 neca-2.0.9/neca/templates/basic/templates/tweet.html
+drwxrwxrwx   0        0        0        0 2023-08-03 19:16:28.107977 neca-2.0.9/neca.egg-info/
+-rw-rw-rw-   0        0        0     1871 2023-08-03 19:16:28.000000 neca-2.0.9/neca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1198 2023-08-03 19:16:28.000000 neca-2.0.9/neca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 19:16:28.000000 neca-2.0.9/neca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-08-03 19:16:28.000000 neca-2.0.9/neca.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       54 2023-08-03 19:16:28.000000 neca-2.0.9/neca.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-03 19:16:28.000000 neca-2.0.9/neca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       92 2023-08-03 16:46:23.000000 neca-2.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 19:16:28.134977 neca-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1973 2023-08-03 19:16:10.000000 neca-2.0.9/setup.py
```

### Comparing `neca-2.0.8/LICENSE` & `neca-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `neca-2.0.8/PKG-INFO` & `neca-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neca
-Version: 2.0.8
+Version: 2.0.9
 Summary: ECA: Event Condition Action 
 Home-page: https://github.com/NiekAukes/eca2
 Author: Niek Aukes
 Author-email: niek.aukes@gmail.com
 Project-URL: Bug Reports, https://github.com/NiekAukes/eca2/issues
 Project-URL: Source, https://github.com/NiekAukes/eca2
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `neca-2.0.8/README.md` & `neca-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `neca-2.0.8/neca/__init__.py` & `neca-2.0.9/neca/__init__.py`

 * *Files identical despite different names*

### Comparing `neca-2.0.8/neca/__main__.py` & `neca-2.0.9/neca/__main__.py`

 * *Files identical despite different names*

### Comparing `neca-2.0.8/neca/events.py` & `neca-2.0.9/neca/events.py`

 * *Files identical despite different names*

### Comparing `neca-2.0.8/neca/generators.py` & `neca-2.0.9/neca/generators.py`

 * *Files identical despite different names*

### Comparing `neca-2.0.8/neca/log.py` & `neca-2.0.9/neca/log.py`

 * *Files identical despite different names*

### Comparing `neca-2.0.8/neca/session.py` & `neca-2.0.9/neca/session.py`

 * *Files identical despite different names*

### Comparing `neca-2.0.8/neca.egg-info/PKG-INFO` & `neca-2.0.9/neca.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neca
-Version: 2.0.8
+Version: 2.0.9
 Summary: ECA: Event Condition Action 
 Home-page: https://github.com/NiekAukes/eca2
 Author: Niek Aukes
 Author-email: niek.aukes@gmail.com
 Project-URL: Bug Reports, https://github.com/NiekAukes/eca2/issues
 Project-URL: Source, https://github.com/NiekAukes/eca2
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `neca-2.0.8/setup.py` & `neca-2.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "PyInquirer",
     "rich",
     "typer",
 ]
 
 setup(
     name='neca',
-    version='2.0.8',
+    version='2.0.9',
     description='ECA: Event Condition Action ',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/NiekAukes/eca2',
     author='Niek Aukes',
     author_email="niek.aukes@gmail.com",
     classifiers=[  # Optional
@@ -39,18 +39,17 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
     
     packages=find_packages(),	
     python_requires=">=3.7, <4",
-    package_dir={"neca": "neca"},
     # read from requirements.txt
     install_requires=requirements,
-
+    include_package_data=True,
     package_data={
         "neca": ["templates/*"],
     },
     
     entry_points={
         "console_scripts": [
             "neca=neca.__main__:cli",
```

