# Comparing `tmp/tinyecs-0.2.2.tar.gz` & `tmp/tinyecs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyecs-0.2.2.tar", last modified: Wed Aug  2 12:56:54 2023, max compression
+gzip compressed data, was "tinyecs-0.2.3.tar", last modified: Thu Aug  3 21:21:50 2023, max compression
```

## Comparing `tinyecs-0.2.2.tar` & `tinyecs-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 12:56:54.071899 tinyecs-0.2.2/
--rw-rw-rw-   0        0        0     1090 2022-03-20 08:49:01.000000 tinyecs-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     1697 2023-08-02 12:56:54.070899 tinyecs-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2023-08-02 12:55:47.000000 tinyecs-0.2.2/README.md
--rw-rw-rw-   0        0        0      895 2023-08-02 12:56:18.000000 tinyecs-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-02 12:56:54.071899 tinyecs-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-02 12:56:54.040086 tinyecs-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-08-02 12:56:54.045678 tinyecs-0.2.2/src/tinyecs/
--rw-rw-rw-   0        0        0    10753 2023-07-23 09:54:19.000000 tinyecs-0.2.2/src/tinyecs/__init__.py
--rw-rw-rw-   0        0        0     3130 2023-08-02 12:31:52.000000 tinyecs-0.2.2/src/tinyecs/components.py
--rw-rw-rw-   0        0        0      849 2023-07-20 20:23:53.000000 tinyecs-0.2.2/src/tinyecs/demo.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:56:54.069891 tinyecs-0.2.2/src/tinyecs/demos/
--rw-rw-rw-   0        0        0        0 2023-05-22 20:58:41.000000 tinyecs-0.2.2/src/tinyecs/demos/__init__.py
--rw-rw-rw-   0        0        0     2990 2023-07-20 19:43:19.000000 tinyecs-0.2.2/src/tinyecs/demos/background.py
--rw-rw-rw-   0        0        0     2768 2023-07-20 19:51:31.000000 tinyecs-0.2.2/src/tinyecs/demos/bouncing_sprites.py
--rw-rw-rw-   0        0        0     4145 2023-07-20 19:56:34.000000 tinyecs-0.2.2/src/tinyecs/demos/example.py
--rw-rw-rw-   0        0        0     7300 2023-08-02 12:31:52.000000 tinyecs-0.2.2/src/tinyecs/demos/homing-missiles.py
--rw-rw-rw-   0        0        0     3150 2023-08-02 12:31:52.000000 tinyecs-0.2.2/src/tinyecs/demos/marquee.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:56:54.065029 tinyecs-0.2.2/src/tinyecs.egg-info/
--rw-rw-rw-   0        0        0     1697 2023-08-02 12:56:54.000000 tinyecs-0.2.2/src/tinyecs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      531 2023-08-02 12:56:54.000000 tinyecs-0.2.2/src/tinyecs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 12:56:54.000000 tinyecs-0.2.2/src/tinyecs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-08-02 12:56:54.000000 tinyecs-0.2.2/src/tinyecs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-08-02 12:56:54.000000 tinyecs-0.2.2/src/tinyecs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 12:56:54.000000 tinyecs-0.2.2/src/tinyecs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 12:56:54.070899 tinyecs-0.2.2/tests/
--rw-rw-rw-   0        0        0     8828 2023-08-02 12:31:52.000000 tinyecs-0.2.2/tests/test_tinyecs.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:21:50.008046 tinyecs-0.2.3/
+-rw-rw-rw-   0        0        0     1090 2022-03-20 08:49:01.000000 tinyecs-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     1697 2023-08-03 21:21:50.007046 tinyecs-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2023-08-02 12:55:47.000000 tinyecs-0.2.3/README.md
+-rw-rw-rw-   0        0        0      895 2023-08-03 21:20:37.000000 tinyecs-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 21:21:50.008046 tinyecs-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 21:21:49.958013 tinyecs-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 21:21:49.963140 tinyecs-0.2.3/src/tinyecs/
+-rw-rw-rw-   0        0        0    10753 2023-07-23 09:54:19.000000 tinyecs-0.2.3/src/tinyecs/__init__.py
+-rw-rw-rw-   0        0        0     9288 2023-08-03 21:16:26.000000 tinyecs-0.2.3/src/tinyecs/components.py
+-rw-rw-rw-   0        0        0      849 2023-07-20 20:23:53.000000 tinyecs-0.2.3/src/tinyecs/demo.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:21:49.994513 tinyecs-0.2.3/src/tinyecs/demos/
+-rw-rw-rw-   0        0        0        0 2023-05-22 20:58:41.000000 tinyecs-0.2.3/src/tinyecs/demos/__init__.py
+-rw-rw-rw-   0        0        0     2990 2023-07-20 19:43:19.000000 tinyecs-0.2.3/src/tinyecs/demos/background.py
+-rw-rw-rw-   0        0        0     2768 2023-07-20 19:51:31.000000 tinyecs-0.2.3/src/tinyecs/demos/bouncing_sprites.py
+-rw-rw-rw-   0        0        0     4145 2023-07-20 19:56:34.000000 tinyecs-0.2.3/src/tinyecs/demos/example.py
+-rw-rw-rw-   0        0        0     7300 2023-08-02 12:31:52.000000 tinyecs-0.2.3/src/tinyecs/demos/homing-missiles.py
+-rw-rw-rw-   0        0        0     3150 2023-08-02 12:31:52.000000 tinyecs-0.2.3/src/tinyecs/demos/marquee.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:21:49.988507 tinyecs-0.2.3/src/tinyecs.egg-info/
+-rw-rw-rw-   0        0        0     1697 2023-08-03 21:21:49.000000 tinyecs-0.2.3/src/tinyecs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      531 2023-08-03 21:21:49.000000 tinyecs-0.2.3/src/tinyecs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 21:21:49.000000 tinyecs-0.2.3/src/tinyecs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-08-03 21:21:49.000000 tinyecs-0.2.3/src/tinyecs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-08-03 21:21:49.000000 tinyecs-0.2.3/src/tinyecs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-03 21:21:49.000000 tinyecs-0.2.3/src/tinyecs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 21:21:50.006044 tinyecs-0.2.3/tests/
+-rw-rw-rw-   0        0        0     8828 2023-08-02 12:31:52.000000 tinyecs-0.2.3/tests/test_tinyecs.py
```

### Comparing `tinyecs-0.2.2/LICENSE` & `tinyecs-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyecs-0.2.2/PKG-INFO` & `tinyecs-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyecs
-Version: 0.2.2
+Version: 0.2.3
 Summary: The teeniest, tiniest ECS system
 Author-email: Michael Lamertz <michael.lamertz@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries :: pygame
```

### Comparing `tinyecs-0.2.2/README.md` & `tinyecs-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tinyecs-0.2.2/pyproject.toml` & `tinyecs-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "tinyecs"
 description = "The teeniest, tiniest ECS system"
-version = "0.2.2"
+version = "0.2.3"
 readme = "README.md"
 
 authors = [
     { name="Michael Lamertz", email="michael.lamertz@gmail.com" }
 ]
 
 classifiers = [
```

### Comparing `tinyecs-0.2.2/src/tinyecs/__init__.py` & `tinyecs-0.2.3/src/tinyecs/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyecs-0.2.2/src/tinyecs/demo.py` & `tinyecs-0.2.3/src/tinyecs/demo.py`

 * *Files identical despite different names*

### Comparing `tinyecs-0.2.2/src/tinyecs/demos/background.py` & `tinyecs-0.2.3/src/tinyecs/demos/background.py`

 * *Files identical despite different names*

### Comparing `tinyecs-0.2.2/src/tinyecs/demos/bouncing_sprites.py` & `tinyecs-0.2.3/src/tinyecs/demos/bouncing_sprites.py`

 * *Files identical despite different names*

### Comparing `tinyecs-0.2.2/src/tinyecs/demos/example.py` & `tinyecs-0.2.3/src/tinyecs/demos/example.py`

 * *Files identical despite different names*

### Comparing `tinyecs-0.2.2/src/tinyecs/demos/homing-missiles.py` & `tinyecs-0.2.3/src/tinyecs/demos/homing-missiles.py`

 * *Files identical despite different names*

### Comparing `tinyecs-0.2.2/src/tinyecs/demos/marquee.py` & `tinyecs-0.2.3/src/tinyecs/demos/marquee.py`

 * *Files identical despite different names*

### Comparing `tinyecs-0.2.2/src/tinyecs.egg-info/PKG-INFO` & `tinyecs-0.2.3/src/tinyecs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyecs
-Version: 0.2.2
+Version: 0.2.3
 Summary: The teeniest, tiniest ECS system
 Author-email: Michael Lamertz <michael.lamertz@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries :: pygame
```

### Comparing `tinyecs-0.2.2/src/tinyecs.egg-info/SOURCES.txt` & `tinyecs-0.2.3/src/tinyecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tinyecs-0.2.2/tests/test_tinyecs.py` & `tinyecs-0.2.3/tests/test_tinyecs.py`

 * *Files identical despite different names*

