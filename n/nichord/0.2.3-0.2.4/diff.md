# Comparing `tmp/nichord-0.2.3.tar.gz` & `tmp/nichord-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nichord-0.2.3.tar", last modified: Thu Aug  3 16:02:44 2023, max compression
+gzip compressed data, was "nichord-0.2.4.tar", last modified: Thu Aug  3 16:44:10 2023, max compression
```

## Comparing `nichord-0.2.3.tar` & `nichord-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 16:02:44.280580 nichord-0.2.3/
--rw-rw-rw-   0        0        0      850 2023-08-03 16:02:44.279579 nichord-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     9376 2023-07-30 22:02:27.000000 nichord-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 16:02:44.273579 nichord-0.2.3/nichord/
--rw-rw-rw-   0        0        0      756 2022-11-12 03:49:12.000000 nichord-0.2.3/nichord/__init__.py
--rw-rw-rw-   0        0        0    34573 2023-07-30 17:47:59.000000 nichord-0.2.3/nichord/chord.py
--rw-rw-rw-   0        0        0     4893 2022-11-13 19:54:36.000000 nichord-0.2.3/nichord/combine.py
--rw-rw-rw-   0        0        0      482 2022-05-22 13:31:30.000000 nichord-0.2.3/nichord/convert.py
--rw-rw-rw-   0        0        0     5404 2023-08-03 16:00:59.000000 nichord-0.2.3/nichord/coord_labeler.py
--rw-rw-rw-   0        0        0     5731 2022-11-12 03:52:39.000000 nichord-0.2.3/nichord/glassbrain.py
--rw-rw-rw-   0        0        0     2156 2023-07-24 20:52:49.000000 nichord-0.2.3/nichord/patch_RendererAgg.py
--rw-rw-rw-   0        0        0     4394 2023-08-03 16:00:59.000000 nichord-0.2.3/nichord/peak.py
-drwxrwxrwx   0        0        0        0 2023-08-03 16:02:44.279579 nichord-0.2.3/nichord.egg-info/
--rw-rw-rw-   0        0        0      850 2023-08-03 16:02:43.000000 nichord-0.2.3/nichord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-08-03 16:02:43.000000 nichord-0.2.3/nichord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 16:02:43.000000 nichord-0.2.3/nichord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-08-03 16:02:43.000000 nichord-0.2.3/nichord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-03 16:02:43.000000 nichord-0.2.3/nichord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 16:02:44.280580 nichord-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1492 2023-08-03 15:58:14.000000 nichord-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:44:10.017349 nichord-0.2.4/
+-rw-rw-rw-   0        0        0      850 2023-08-03 16:44:10.017349 nichord-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9376 2023-07-30 22:02:27.000000 nichord-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 16:44:10.010347 nichord-0.2.4/nichord/
+-rw-rw-rw-   0        0        0      756 2022-11-12 03:49:12.000000 nichord-0.2.4/nichord/__init__.py
+-rw-rw-rw-   0        0        0    34573 2023-07-30 17:47:59.000000 nichord-0.2.4/nichord/chord.py
+-rw-rw-rw-   0        0        0     4893 2022-11-13 19:54:36.000000 nichord-0.2.4/nichord/combine.py
+-rw-rw-rw-   0        0        0      482 2022-05-22 13:31:30.000000 nichord-0.2.4/nichord/convert.py
+-rw-rw-rw-   0        0        0     5404 2023-08-03 16:00:59.000000 nichord-0.2.4/nichord/coord_labeler.py
+-rw-rw-rw-   0        0        0     5731 2022-11-12 03:52:39.000000 nichord-0.2.4/nichord/glassbrain.py
+-rw-rw-rw-   0        0        0     2156 2023-07-24 20:52:49.000000 nichord-0.2.4/nichord/patch_RendererAgg.py
+-rw-rw-rw-   0        0        0     4394 2023-08-03 16:00:59.000000 nichord-0.2.4/nichord/peak.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:44:10.016348 nichord-0.2.4/nichord.egg-info/
+-rw-rw-rw-   0        0        0      850 2023-08-03 16:44:09.000000 nichord-0.2.4/nichord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-08-03 16:44:09.000000 nichord-0.2.4/nichord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 16:44:09.000000 nichord-0.2.4/nichord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-08-03 16:44:09.000000 nichord-0.2.4/nichord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-03 16:44:09.000000 nichord-0.2.4/nichord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 16:44:10.017349 nichord-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1526 2023-08-03 16:43:35.000000 nichord-0.2.4/setup.py
```

### Comparing `nichord-0.2.3/PKG-INFO` & `nichord-0.2.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nichord
-Version: 0.2.3
+Version: 0.2.4
 Summary: Creates chord diagrams for connectivity/graph data
 Home-page: https://github.com/paulcbogdan/NiChord
 Author: paulcbogdan
 Author-email: paulcbogdan@gmail.com
 License: MIT
 Keywords: plotting,fmri,plotting,chord
 Classifier: Programming Language :: Python
```

### Comparing `nichord-0.2.3/README.md` & `nichord-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nichord-0.2.3/nichord/__init__.py` & `nichord-0.2.4/nichord/__init__.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.3/nichord/chord.py` & `nichord-0.2.4/nichord/chord.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.3/nichord/combine.py` & `nichord-0.2.4/nichord/combine.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.3/nichord/coord_labeler.py` & `nichord-0.2.4/nichord/coord_labeler.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.3/nichord/glassbrain.py` & `nichord-0.2.4/nichord/glassbrain.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.3/nichord/patch_RendererAgg.py` & `nichord-0.2.4/nichord/patch_RendererAgg.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.3/nichord/peak.py` & `nichord-0.2.4/nichord/peak.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.3/nichord.egg-info/PKG-INFO` & `nichord-0.2.4/nichord.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nichord
-Version: 0.2.3
+Version: 0.2.4
 Summary: Creates chord diagrams for connectivity/graph data
 Home-page: https://github.com/paulcbogdan/NiChord
 Author: paulcbogdan
 Author-email: paulcbogdan@gmail.com
 License: MIT
 Keywords: plotting,fmri,plotting,chord
 Classifier: Programming Language :: Python
```

### Comparing `nichord-0.2.3/setup.py` & `nichord-0.2.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 'To find out more about the package and see an example, see its .'
 
 setup(
     name="nichord",
     description="Creates chord diagrams for connectivity/graph data",
     long_description=desc,
     long_description_content_type="text/markdown",
-    version="v0.2.3",
+    version="v0.2.4",
     packages=["nichord"],
     python_requires=">=3.7",
     url="https://github.com/paulcbogdan/NiChord",
     author="paulcbogdan",
     author_email="paulcbogdan@gmail.com",
     install_requires=["nilearn",
                       "pandas",
@@ -35,9 +35,10 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    license="MIT"
+    license="MIT",
+    license_files="LICENSE.txt"
 )
```

