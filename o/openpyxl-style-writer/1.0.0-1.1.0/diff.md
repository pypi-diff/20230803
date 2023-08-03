# Comparing `tmp/openpyxl_style_writer-1.0.0.tar.gz` & `tmp/openpyxl_style_writer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpyxl_style_writer-1.0.0.tar", last modified: Sun Jan 15 13:17:46 2023, max compression
+gzip compressed data, was "openpyxl_style_writer-1.1.0.tar", last modified: Thu Aug  3 03:55:41 2023, max compression
```

## Comparing `openpyxl_style_writer-1.0.0.tar` & `openpyxl_style_writer-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-15 13:17:46.725456 openpyxl_style_writer-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-01-14 08:01:15.000000 openpyxl_style_writer-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2771 2023-01-15 13:17:46.724460 openpyxl_style_writer-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2206 2023-01-15 13:16:05.000000 openpyxl_style_writer-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-01-15 13:17:46.711455 openpyxl_style_writer-1.0.0/openpyxl_style_writer/
--rw-rw-rw-   0        0        0      179 2023-01-15 07:20:29.000000 openpyxl_style_writer-1.0.0/openpyxl_style_writer/__init__.py
--rw-rw-rw-   0        0        0     9067 2023-01-15 07:20:29.000000 openpyxl_style_writer-1.0.0/openpyxl_style_writer/style.py
--rw-rw-rw-   0        0        0     1963 2023-01-15 07:20:29.000000 openpyxl_style_writer-1.0.0/openpyxl_style_writer/wirter.py
-drwxrwxrwx   0        0        0        0 2023-01-15 13:17:46.724460 openpyxl_style_writer-1.0.0/openpyxl_style_writer.egg-info/
--rw-rw-rw-   0        0        0     2771 2023-01-15 13:17:46.000000 openpyxl_style_writer-1.0.0/openpyxl_style_writer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-01-15 13:17:46.000000 openpyxl_style_writer-1.0.0/openpyxl_style_writer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-15 13:17:46.000000 openpyxl_style_writer-1.0.0/openpyxl_style_writer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-01-15 13:17:46.000000 openpyxl_style_writer-1.0.0/openpyxl_style_writer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-01-15 13:17:46.000000 openpyxl_style_writer-1.0.0/openpyxl_style_writer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-15 13:17:46.725456 openpyxl_style_writer-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      826 2023-01-15 13:14:15.000000 openpyxl_style_writer-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:55:41.718524 openpyxl_style_writer-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-03 03:55:32.000000 openpyxl_style_writer-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-08-03 03:55:41.718524 openpyxl_style_writer-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-08-03 03:55:32.000000 openpyxl_style_writer-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:55:41.718524 openpyxl_style_writer-1.1.0/openpyxl_style_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-03 03:55:32.000000 openpyxl_style_writer-1.1.0/openpyxl_style_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-08-03 03:55:32.000000 openpyxl_style_writer-1.1.0/openpyxl_style_writer/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-03 03:55:32.000000 openpyxl_style_writer-1.1.0/openpyxl_style_writer/wirter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:55:41.718524 openpyxl_style_writer-1.1.0/openpyxl_style_writer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-08-03 03:55:41.000000 openpyxl_style_writer-1.1.0/openpyxl_style_writer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-03 03:55:41.000000 openpyxl_style_writer-1.1.0/openpyxl_style_writer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 03:55:41.000000 openpyxl_style_writer-1.1.0/openpyxl_style_writer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 03:55:41.000000 openpyxl_style_writer-1.1.0/openpyxl_style_writer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 03:55:41.000000 openpyxl_style_writer-1.1.0/openpyxl_style_writer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 03:55:41.718524 openpyxl_style_writer-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-03 03:55:32.000000 openpyxl_style_writer-1.1.0/setup.py
```

### Comparing `openpyxl_style_writer-1.0.0/LICENSE` & `openpyxl_style_writer-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Jian Yu, Chen
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Jian Yu, Chen
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

