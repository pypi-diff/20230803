# Comparing `tmp/rune_ocr-0.0.3.tar.gz` & `tmp/rune_ocr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rune_ocr-0.0.3.tar", last modified: Wed Aug  2 22:41:14 2023, max compression
+gzip compressed data, was "rune_ocr-0.0.4.tar", last modified: Wed Aug  2 22:48:34 2023, max compression
```

## Comparing `rune_ocr-0.0.3.tar` & `rune_ocr-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 22:41:14.596482 rune_ocr-0.0.3/
--rw-rw-rw-   0        0        0      363 2023-08-02 22:41:14.597482 rune_ocr-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-08-01 16:27:45.976832 rune_ocr-0.0.3/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 22:41:14.584953 rune_ocr-0.0.3/rune_ocr/
--rw-rw-rw-   0        0        0      131 2023-08-01 16:27:45.988773 rune_ocr-0.0.3/rune_ocr/__init__.py
--rw-rw-rw-   0        0        0     4586 2023-08-01 15:44:11.423135 rune_ocr-0.0.3/rune_ocr/inference.py
-drwxrwxrwx   0        0        0        0 2023-08-02 22:41:14.594480 rune_ocr-0.0.3/rune_ocr/training/
--rw-rw-rw-   0        0        0      100 2023-08-01 00:03:21.940291 rune_ocr-0.0.3/rune_ocr/training/__init__.py
--rw-rw-rw-   0        0        0    14799 2023-08-01 00:03:21.941292 rune_ocr-0.0.3/rune_ocr/training/helpers.py
--rw-rw-rw-   0        0        0    11487 2023-08-01 00:03:21.942296 rune_ocr-0.0.3/rune_ocr/training/loss.py
--rw-rw-rw-   0        0        0       40 2023-08-01 00:03:21.944798 rune_ocr-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2682 2023-08-02 22:40:53.462476 rune_ocr-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:48:34.512370 rune_ocr-0.0.4/
+-rw-rw-rw-   0        0        0      353 2023-08-02 22:48:34.513384 rune_ocr-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-08-01 16:27:45.976832 rune_ocr-0.0.4/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 22:48:34.499278 rune_ocr-0.0.4/rune_ocr/
+-rw-rw-rw-   0        0        0      131 2023-08-01 16:27:45.988773 rune_ocr-0.0.4/rune_ocr/__init__.py
+-rw-rw-rw-   0        0        0     4586 2023-08-01 15:44:11.423135 rune_ocr-0.0.4/rune_ocr/inference.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:48:34.510358 rune_ocr-0.0.4/rune_ocr/training/
+-rw-rw-rw-   0        0        0      100 2023-08-01 00:03:21.940291 rune_ocr-0.0.4/rune_ocr/training/__init__.py
+-rw-rw-rw-   0        0        0    14799 2023-08-01 00:03:21.941292 rune_ocr-0.0.4/rune_ocr/training/helpers.py
+-rw-rw-rw-   0        0        0    11487 2023-08-01 00:03:21.942296 rune_ocr-0.0.4/rune_ocr/training/loss.py
+-rw-rw-rw-   0        0        0       40 2023-08-01 00:03:21.944798 rune_ocr-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2617 2023-08-02 22:48:14.080640 rune_ocr-0.0.4/setup.py
```

### Comparing `rune_ocr-0.0.3/rune_ocr/inference.py` & `rune_ocr-0.0.4/rune_ocr/inference.py`

 * *Files identical despite different names*

### Comparing `rune_ocr-0.0.3/rune_ocr/training/helpers.py` & `rune_ocr-0.0.4/rune_ocr/training/helpers.py`

 * *Files identical despite different names*

### Comparing `rune_ocr-0.0.3/rune_ocr/training/loss.py` & `rune_ocr-0.0.4/rune_ocr/training/loss.py`

 * *Files identical despite different names*

### Comparing `rune_ocr-0.0.3/setup.py` & `rune_ocr-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,34 +44,31 @@
 # print({
 #     'deps_all': deps_all,
 #     'deps_all_latest': deps_all_latest,
 #     'deps_core': deps_core,
 #     'deps_extras': deps_extras,
 # })
 
-## Get README.md
-with open(str(dir_parent / "readme.txt")) as f:
-    readme = f.read()
 
 ## Get version number
 with open(str(dir_parent / "rune_ocr" / "__init__.py"), "r") as f:
     for line in f:
         if line.startswith("__version__"):
             version = line.split("=")[1].strip().replace("\"", "").replace("\'", "")
             break
 
 setup(
     name='rune_ocr',
-    version='0.0.3',
+    version='0.0.4',
     author='Richard Hakim',
     author_email='jlind@wwidew.net',
     keywords=['runes', 'ocr'],
     license='LICENSE',
     description='A tool for optical character recognition (OCR) of runic characters using YOLO.',
-    long_description=readme,
+    long_description='Something something dark side',
     long_description_content_type="text/plain",
     url='https://github.com/RichieHakim/rune_ocr',
 
     packages=[
         'rune_ocr',
         'rune_ocr.training',
     ],
```

