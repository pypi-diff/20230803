# Comparing `tmp/naipng-1.0.0.tar.gz` & `tmp/naipng-1.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naipng-1.0.0.tar", last modified: Thu Aug  3 06:54:06 2023, max compression, from Unix
+gzip compressed data, was "naipng-1.0.0.post1.tar", last modified: Thu Aug  3 07:47:58 2023, max compression, from Unix
```

## Comparing `naipng-1.0.0.tar` & `naipng-1.0.0.post1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 06:54:05.991838 naipng-1.0.0/
--rwxrwxrwx   0 root         (0) root         (0)      859 2023-08-03 00:07:01.000000 naipng-1.0.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     8252 2023-08-03 06:54:05.990840 naipng-1.0.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     7536 2023-08-03 06:51:33.000000 naipng-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 06:54:05.952838 naipng-1.0.0/naipng/
--rwxrwxrwx   0 root         (0) root         (0)    18708 2023-08-03 06:41:52.000000 naipng-1.0.0/naipng/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4038 2023-08-03 06:45:28.000000 naipng-1.0.0/naipng/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 06:54:05.984838 naipng-1.0.0/naipng.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     8252 2023-08-03 06:54:05.000000 naipng-1.0.0/naipng.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      223 2023-08-03 06:54:05.000000 naipng-1.0.0/naipng.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-08-03 06:54:05.000000 naipng-1.0.0/naipng.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       48 2023-08-03 06:54:05.000000 naipng-1.0.0/naipng.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-08-03 06:54:05.000000 naipng-1.0.0/naipng.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     1087 2023-08-03 05:51:57.000000 naipng-1.0.0/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-08-03 06:54:05.992839 naipng-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:47:58.046023 naipng-1.0.0.post1/
+-rwxrwxrwx   0 root         (0) root         (0)      859 2023-08-03 00:07:01.000000 naipng-1.0.0.post1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     8259 2023-08-03 07:47:58.044023 naipng-1.0.0.post1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     7537 2023-08-03 07:40:34.000000 naipng-1.0.0.post1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:47:58.001022 naipng-1.0.0.post1/naipng/
+-rwxrwxrwx   0 root         (0) root         (0)    18711 2023-08-03 07:40:08.000000 naipng-1.0.0.post1/naipng/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4038 2023-08-03 06:45:28.000000 naipng-1.0.0.post1/naipng/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:47:58.035022 naipng-1.0.0.post1/naipng.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     8259 2023-08-03 07:47:57.000000 naipng-1.0.0.post1/naipng.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      223 2023-08-03 07:47:57.000000 naipng-1.0.0.post1/naipng.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-08-03 07:47:57.000000 naipng-1.0.0.post1/naipng.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       48 2023-08-03 07:47:57.000000 naipng-1.0.0.post1/naipng.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-08-03 07:47:57.000000 naipng-1.0.0.post1/naipng.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1093 2023-08-03 07:47:04.000000 naipng-1.0.0.post1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-08-03 07:47:58.046023 naipng-1.0.0.post1/setup.cfg
```

### Comparing `naipng-1.0.0/LICENSE` & `naipng-1.0.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `naipng-1.0.0/PKG-INFO` & `naipng-1.0.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naipng
-Version: 1.0.0
+Version: 1.0.0.post1
 Summary: Library and command-line tool to read NovelAI data encoded in PNG files
 Author: Eta
 License: zlib/libpng License
 Project-URL: Homepage, https://github.com/Eta0/naipng
 Keywords: novelai,nai,png,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: zlib/libpng License
@@ -91,15 +91,15 @@
 
 # Using a file-like object
 with open("image.png", "rb") as file:
     decoded = naipng.read(file)
 
 if decoded is None:
     # No NovelAI data found encoded in the image
-    parsed = {}
+    print("N/A")
 else:
     # naipng.read() returns a dict object representing the first data found
     for k, v in decoded.items():
         print(k, "->", v)
 ```
 
 Another example, using `bytes` as input to `naipng.read`:
```

### Comparing `naipng-1.0.0/README.md` & `naipng-1.0.0.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 # Using a file-like object
 with open("image.png", "rb") as file:
     decoded = naipng.read(file)
 
 if decoded is None:
     # No NovelAI data found encoded in the image
-    parsed = {}
+    print("N/A")
 else:
     # naipng.read() returns a dict object representing the first data found
     for k, v in decoded.items():
         print(k, "->", v)
 ```
 
 Another example, using `bytes` as input to `naipng.read`:
```

### Comparing `naipng-1.0.0/naipng/__init__.py` & `naipng-1.0.0.post1/naipng/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             import naipng
 
             with open("image.png", "rb") as file:
                 decoded = naipng.read(file)
 
             if decoded is None:
                 # No NovelAI data found encoded in the image
-                parsed = {}
+                print("N/A")
             else:
                 # naipng.read() returns a dict object
                 # representing the first data found
                 for k, v in decoded.items():
                     print(k, "->", v)
 
         Reading from a ``bytes`` object::
@@ -226,15 +226,15 @@
             import naipng
 
             with open("image.png", "rb") as file:
                 decoded = naipng.read_text_gen(file)
 
             if decoded is None:
                 # No NovelAI text generation data found encoded in the image
-                parsed = {}
+                print("N/A")
             else:
                 # naipng.read_text_gen() returns a dict object
                 # representing the first data found
                 for k, v in decoded.items():
                     print(k, "->", v)
 
         Reading from a ``bytes`` object::
@@ -307,15 +307,15 @@
             import naipng
 
             with open("image.png", "rb") as file:
                 decoded = naipng.read_image_gen(file)
 
             if decoded is None:
                 # No NovelAI data found encoded in the image
-                parsed = {}
+                print("N/A")
             else:
                 # naipng.read_image_gen() returns a dict object
                 # representing the first data found
                 for k, v in decoded.items():
                     print(k, "->", v)
 
         Reading from a ``bytes`` object::
```

### Comparing `naipng-1.0.0/naipng/__main__.py` & `naipng-1.0.0.post1/naipng/__main__.py`

 * *Files identical despite different names*

### Comparing `naipng-1.0.0/naipng.egg-info/PKG-INFO` & `naipng-1.0.0.post1/naipng.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naipng
-Version: 1.0.0
+Version: 1.0.0.post1
 Summary: Library and command-line tool to read NovelAI data encoded in PNG files
 Author: Eta
 License: zlib/libpng License
 Project-URL: Homepage, https://github.com/Eta0/naipng
 Keywords: novelai,nai,png,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: zlib/libpng License
@@ -91,15 +91,15 @@
 
 # Using a file-like object
 with open("image.png", "rb") as file:
     decoded = naipng.read(file)
 
 if decoded is None:
     # No NovelAI data found encoded in the image
-    parsed = {}
+    print("N/A")
 else:
     # naipng.read() returns a dict object representing the first data found
     for k, v in decoded.items():
         print(k, "->", v)
 ```
 
 Another example, using `bytes` as input to `naipng.read`:
```

### Comparing `naipng-1.0.0/pyproject.toml` & `naipng-1.0.0.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "naipng"
-version = "1.0.0"
+version = "1.0.0.post1"
 license = { text = "zlib/libpng License" }
 keywords = ["novelai", "nai", "png", "cli"]
 authors = [
   { name="Eta" }
 ]
 description = "Library and command-line tool to read NovelAI data encoded in PNG files"
 readme = "README.md"
```

