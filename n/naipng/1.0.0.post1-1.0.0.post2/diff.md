# Comparing `tmp/naipng-1.0.0.post1.tar.gz` & `tmp/naipng-1.0.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naipng-1.0.0.post1.tar", last modified: Thu Aug  3 07:47:58 2023, max compression, from Unix
+gzip compressed data, was "naipng-1.0.0.post2.tar", last modified: Thu Aug  3 07:54:07 2023, max compression, from Unix
```

## Comparing `naipng-1.0.0.post1.tar` & `naipng-1.0.0.post2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:47:58.046023 naipng-1.0.0.post1/
--rwxrwxrwx   0 root         (0) root         (0)      859 2023-08-03 00:07:01.000000 naipng-1.0.0.post1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     8259 2023-08-03 07:47:58.044023 naipng-1.0.0.post1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     7537 2023-08-03 07:40:34.000000 naipng-1.0.0.post1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:47:58.001022 naipng-1.0.0.post1/naipng/
--rwxrwxrwx   0 root         (0) root         (0)    18711 2023-08-03 07:40:08.000000 naipng-1.0.0.post1/naipng/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4038 2023-08-03 06:45:28.000000 naipng-1.0.0.post1/naipng/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:47:58.035022 naipng-1.0.0.post1/naipng.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     8259 2023-08-03 07:47:57.000000 naipng-1.0.0.post1/naipng.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      223 2023-08-03 07:47:57.000000 naipng-1.0.0.post1/naipng.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-08-03 07:47:57.000000 naipng-1.0.0.post1/naipng.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       48 2023-08-03 07:47:57.000000 naipng-1.0.0.post1/naipng.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-08-03 07:47:57.000000 naipng-1.0.0.post1/naipng.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     1093 2023-08-03 07:47:04.000000 naipng-1.0.0.post1/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-08-03 07:47:58.046023 naipng-1.0.0.post1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:54:07.248181 naipng-1.0.0.post2/
+-rwxrwxrwx   0 root         (0) root         (0)      859 2023-08-03 00:07:01.000000 naipng-1.0.0.post2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     8259 2023-08-03 07:54:07.247181 naipng-1.0.0.post2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     7537 2023-08-03 07:40:34.000000 naipng-1.0.0.post2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:54:07.209182 naipng-1.0.0.post2/naipng/
+-rwxrwxrwx   0 root         (0) root         (0)    18711 2023-08-03 07:40:08.000000 naipng-1.0.0.post2/naipng/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4030 2023-08-03 07:52:51.000000 naipng-1.0.0.post2/naipng/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:54:07.239181 naipng-1.0.0.post2/naipng.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     8259 2023-08-03 07:54:07.000000 naipng-1.0.0.post2/naipng.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      223 2023-08-03 07:54:07.000000 naipng-1.0.0.post2/naipng.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-08-03 07:54:07.000000 naipng-1.0.0.post2/naipng.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       48 2023-08-03 07:54:07.000000 naipng-1.0.0.post2/naipng.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-08-03 07:54:07.000000 naipng-1.0.0.post2/naipng.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1093 2023-08-03 07:53:41.000000 naipng-1.0.0.post2/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-08-03 07:54:07.249182 naipng-1.0.0.post2/setup.cfg
```

### Comparing `naipng-1.0.0.post1/LICENSE` & `naipng-1.0.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `naipng-1.0.0.post1/PKG-INFO` & `naipng-1.0.0.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naipng
-Version: 1.0.0.post1
+Version: 1.0.0.post2
 Summary: Library and command-line tool to read NovelAI data encoded in PNG files
 Author: Eta
 License: zlib/libpng License
 Project-URL: Homepage, https://github.com/Eta0/naipng
 Keywords: novelai,nai,png,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: zlib/libpng License
```

### Comparing `naipng-1.0.0.post1/README.md` & `naipng-1.0.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `naipng-1.0.0.post1/naipng/__init__.py` & `naipng-1.0.0.post2/naipng/__init__.py`

 * *Files identical despite different names*

### Comparing `naipng-1.0.0.post1/naipng/__main__.py` & `naipng-1.0.0.post2/naipng/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
               (saving to a file)
               %(prog)s image.png naidata.json
 
               (redirecting stdin and stdout)
               %(prog)s - < image.png > naidata.json
 
               (with external tools curl & jq)
-              curl -fs https://files.catbox.moe/3b6dux.png | %(prog)s -c image.png | jq
+              curl -fs https://files.catbox.moe/3b6dux.png | %(prog)s -c - | jq
         """),
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser.add_argument(
         "file",
         type=argparse.FileType(mode="rb"),
         help="PNG file to read, or - for stdin",
```

### Comparing `naipng-1.0.0.post1/naipng.egg-info/PKG-INFO` & `naipng-1.0.0.post2/naipng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naipng
-Version: 1.0.0.post1
+Version: 1.0.0.post2
 Summary: Library and command-line tool to read NovelAI data encoded in PNG files
 Author: Eta
 License: zlib/libpng License
 Project-URL: Homepage, https://github.com/Eta0/naipng
 Keywords: novelai,nai,png,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: zlib/libpng License
```

### Comparing `naipng-1.0.0.post1/pyproject.toml` & `naipng-1.0.0.post2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "naipng"
-version = "1.0.0.post1"
+version = "1.0.0.post2"
 license = { text = "zlib/libpng License" }
 keywords = ["novelai", "nai", "png", "cli"]
 authors = [
   { name="Eta" }
 ]
 description = "Library and command-line tool to read NovelAI data encoded in PNG files"
 readme = "README.md"
```

