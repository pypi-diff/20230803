# Comparing `tmp/rune_ocr-0.0.1.tar.gz` & `tmp/rune_ocr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rune_ocr-0.0.1.tar", last modified: Wed Aug  2 22:29:13 2023, max compression
+gzip compressed data, was "rune_ocr-0.0.2.tar", last modified: Wed Aug  2 22:32:48 2023, max compression
```

## Comparing `rune_ocr-0.0.1.tar` & `rune_ocr-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 22:29:13.650407 rune_ocr-0.0.1/
--rw-rw-rw-   0        0        0      363 2023-08-02 22:29:13.651893 rune_ocr-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-08-01 16:27:45.976832 rune_ocr-0.0.1/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 22:29:13.638859 rune_ocr-0.0.1/rune_ocr/
--rw-rw-rw-   0        0        0      131 2023-08-01 16:27:45.988773 rune_ocr-0.0.1/rune_ocr/__init__.py
--rw-rw-rw-   0        0        0     4586 2023-08-01 15:44:11.423135 rune_ocr-0.0.1/rune_ocr/inference.py
-drwxrwxrwx   0        0        0        0 2023-08-02 22:29:13.649404 rune_ocr-0.0.1/rune_ocr/training/
--rw-rw-rw-   0        0        0      100 2023-08-01 00:03:21.940291 rune_ocr-0.0.1/rune_ocr/training/__init__.py
--rw-rw-rw-   0        0        0    14799 2023-08-01 00:03:21.941292 rune_ocr-0.0.1/rune_ocr/training/helpers.py
--rw-rw-rw-   0        0        0    11487 2023-08-01 00:03:21.942296 rune_ocr-0.0.1/rune_ocr/training/loss.py
--rw-rw-rw-   0        0        0       40 2023-08-01 00:03:21.944798 rune_ocr-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2687 2023-08-02 22:28:51.342548 rune_ocr-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:32:48.981310 rune_ocr-0.0.2/
+-rw-rw-rw-   0        0        0      363 2023-08-02 22:32:48.982312 rune_ocr-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-08-01 16:27:45.976832 rune_ocr-0.0.2/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 22:32:48.968695 rune_ocr-0.0.2/rune_ocr/
+-rw-rw-rw-   0        0        0      131 2023-08-01 16:27:45.988773 rune_ocr-0.0.2/rune_ocr/__init__.py
+-rw-rw-rw-   0        0        0     4586 2023-08-01 15:44:11.423135 rune_ocr-0.0.2/rune_ocr/inference.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:32:48.979233 rune_ocr-0.0.2/rune_ocr/training/
+-rw-rw-rw-   0        0        0      100 2023-08-01 00:03:21.940291 rune_ocr-0.0.2/rune_ocr/training/__init__.py
+-rw-rw-rw-   0        0        0    14799 2023-08-01 00:03:21.941292 rune_ocr-0.0.2/rune_ocr/training/helpers.py
+-rw-rw-rw-   0        0        0    11487 2023-08-01 00:03:21.942296 rune_ocr-0.0.2/rune_ocr/training/loss.py
+-rw-rw-rw-   0        0        0       40 2023-08-01 00:03:21.944798 rune_ocr-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2687 2023-08-02 22:32:26.883763 rune_ocr-0.0.2/setup.py
```

### Comparing `rune_ocr-0.0.1/rune_ocr/inference.py` & `rune_ocr-0.0.2/rune_ocr/inference.py`

 * *Files identical despite different names*

### Comparing `rune_ocr-0.0.1/rune_ocr/training/helpers.py` & `rune_ocr-0.0.2/rune_ocr/training/helpers.py`

 * *Files identical despite different names*

### Comparing `rune_ocr-0.0.1/rune_ocr/training/loss.py` & `rune_ocr-0.0.2/rune_ocr/training/loss.py`

 * *Files identical despite different names*

### Comparing `rune_ocr-0.0.1/setup.py` & `rune_ocr-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,27 +45,27 @@
 #     'deps_all': deps_all,
 #     'deps_all_latest': deps_all_latest,
 #     'deps_core': deps_core,
 #     'deps_extras': deps_extras,
 # })
 
 ## Get README.md
-with open(str(dir_parent / "README.txt"), "r") as f:
+with open(str(dir_parent / "readme.txt"), "r") as f:
     readme = f.read()
 
 ## Get version number
 with open(str(dir_parent / "rune_ocr" / "__init__.py"), "r") as f:
     for line in f:
         if line.startswith("__version__"):
             version = line.split("=")[1].strip().replace("\"", "").replace("\'", "")
             break
 
 setup(
     name='rune_ocr',
-    version=version,
+    version='0.0.2',
     author='Richard Hakim',
     author_email='jlind@wwidew.net',
     keywords=['runes', 'ocr'],
     license='LICENSE',
     description='A tool for optical character recognition (OCR) of runic characters using YOLO.',
     long_description=readme,
     long_description_content_type="text/plain",
```

