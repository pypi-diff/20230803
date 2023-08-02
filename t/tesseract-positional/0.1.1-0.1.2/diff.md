# Comparing `tmp/tesseract_positional-0.1.1.tar.gz` & `tmp/tesseract_positional-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tesseract_positional-0.1.1.tar", last modified: Mon May  6 01:09:26 2019, max compression
+gzip compressed data, was "tesseract_positional-0.1.2.tar", last modified: Wed Aug  2 22:07:59 2023, max compression
```

## Comparing `tesseract_positional-0.1.1.tar` & `tesseract_positional-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2019-05-06 01:09:26.000000 tesseract_positional-0.1.1/
--rw-rw-rw-   0        0        0      307 2019-05-06 01:09:26.000000 tesseract_positional-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1850 2019-05-06 01:06:53.000000 tesseract_positional-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2019-05-06 01:09:26.000000 tesseract_positional-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      575 2019-05-06 01:07:45.000000 tesseract_positional-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2019-05-06 01:09:26.000000 tesseract_positional-0.1.1/tesseract_positional/
--rw-rw-rw-   0        0        0      850 2019-05-06 01:07:48.000000 tesseract_positional-0.1.1/tesseract_positional/cmd_line.py
--rw-rw-rw-   0        0        0     4825 2019-05-06 01:07:51.000000 tesseract_positional-0.1.1/tesseract_positional/positional_ocr.py
--rw-rw-rw-   0        0        0      185 2019-05-06 01:07:43.000000 tesseract_positional-0.1.1/tesseract_positional/__init__.py
-drwxrwxrwx   0        0        0        0 2019-05-06 01:09:26.000000 tesseract_positional-0.1.1/tesseract_positional.egg-info/
--rw-rw-rw-   0        0        0        1 2019-05-06 01:09:26.000000 tesseract_positional-0.1.1/tesseract_positional.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2019-05-06 01:09:26.000000 tesseract_positional-0.1.1/tesseract_positional.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2019-05-06 01:09:26.000000 tesseract_positional-0.1.1/tesseract_positional.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      307 2019-05-06 01:09:26.000000 tesseract_positional-0.1.1/tesseract_positional.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       19 2019-05-06 01:09:26.000000 tesseract_positional-0.1.1/tesseract_positional.egg-info/requires.txt
--rw-rw-rw-   0        0        0      432 2019-05-06 01:09:26.000000 tesseract_positional-0.1.1/tesseract_positional.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       21 2019-05-06 01:09:26.000000 tesseract_positional-0.1.1/tesseract_positional.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:07:59.301917 tesseract_positional-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 22:07:49.000000 tesseract_positional-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-02 22:07:59.301917 tesseract_positional-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-02 22:07:49.000000 tesseract_positional-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-02 22:07:49.000000 tesseract_positional-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 22:07:59.301917 tesseract_positional-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:07:59.297917 tesseract_positional-0.1.2/tesseract_positional/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-02 22:07:49.000000 tesseract_positional-0.1.2/tesseract_positional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-02 22:07:49.000000 tesseract_positional-0.1.2/tesseract_positional/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-08-02 22:07:49.000000 tesseract_positional-0.1.2/tesseract_positional/positional_ocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:07:59.301917 tesseract_positional-0.1.2/tesseract_positional.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-02 22:07:59.000000 tesseract_positional-0.1.2/tesseract_positional.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-02 22:07:59.000000 tesseract_positional-0.1.2/tesseract_positional.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:07:59.000000 tesseract_positional-0.1.2/tesseract_positional.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-02 22:07:59.000000 tesseract_positional-0.1.2/tesseract_positional.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 22:07:59.000000 tesseract_positional-0.1.2/tesseract_positional.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 22:07:59.000000 tesseract_positional-0.1.2/tesseract_positional.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tesseract_positional-0.1.1/README.md` & `tesseract_positional-0.1.2/tesseract_positional.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,72 @@
-# Tesseract-Positional
-A tool to save positional OCR data to a text file
-
-[![GitHub version](https://badge.fury.io/gh/tjkessler%2Ftesseract-positional.svg)](https://badge.fury.io/gh/tjkessler%2Ftesseract-positional)
-[![PyPI version](https://badge.fury.io/py/tesseract-positional.svg)](https://badge.fury.io/py/tesseract-positional)
-[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/tjkessler/tesseract-positional/master/LICENSE.txt)
-
-Tesseract-Positional allows positional data extracted using OCR to be saved as plain-text. Positional data includes text spacing and line breaks.
-
-## Installation
-
-Installation via pip:
-
-```
-$ pip install tesseract-positional
-```
-
-Installation via cloned repository:
-
-```
-$ cd tesseract-positional
-$ python setup.py install
-```
-
-Additional dependencies (pytesseract, Pillow) will be installed during Tesseract-Positional's installation.
-
-## Basic Usage
-
-### Via a Python script
-
-Saving extracted text to a file:
-
-```python
-from tesseract_positional import positional_ocr
-positional_ocr('image.tiff', 'output.txt')
-```
-
-Obtaining extracted text:
-
-```python
-from tesseract_positional import positional_ocr
-text = positional_ocr('image.tiff')
-```
-
-### Via the command line
-
-```
-$ tesseract-positional image.tiff output.txt
-```
-
-## Contributing, Reporting Issues and Other Support
-
-To contribute to Tesseract-Positional, make a pull request. Contributions should include tests for new features added, as well as extensive documentation.
-
-To report problems with the software or feature requests, file an issue. When reporting problems, include information such as error messages, your OS/environment and Python version.
-
-For additional support/questions, contact Travis Kessler (travis.j.kessler@gmail.com).
+Metadata-Version: 2.1
+Name: tesseract-positional
+Version: 0.1.2
+Summary: Tool to save positional OCR data to a text file
+Author-email: Travis Kessler <travis.j.kessler@gmail.com>
+Project-URL: Homepage, https://github.com/tjkessler/tesseract-positional
+Project-URL: Bug Tracker, https://github.com/tjkessler/tesseract-positional/issues
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Tesseract-Positional
+A tool to save positional OCR data to a text file
+
+[![GitHub version](https://badge.fury.io/gh/tjkessler%2Ftesseract-positional.svg)](https://badge.fury.io/gh/tjkessler%2Ftesseract-positional)
+[![PyPI version](https://badge.fury.io/py/tesseract-positional.svg)](https://badge.fury.io/py/tesseract-positional)
+[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/tjkessler/tesseract-positional/master/LICENSE.txt)
+
+Tesseract-Positional allows positional data extracted using OCR to be saved as plain-text. Positional data includes text spacing and line breaks.
+
+## Installation
+
+Installation via pip:
+
+```
+$ pip install tesseract-positional
+```
+
+Installation via cloned repository:
+
+```
+$ git clone https://github.com/tjkessler/tesseract-positional
+$ cd tesseract-positional
+$ pip install .
+```
+
+Additional dependencies (pytesseract, Pillow) will be installed during Tesseract-Positional's installation.
+
+## Basic Usage
+
+### Via a Python script
+
+Saving extracted text to a file:
+
+```python
+from tesseract_positional import positional_ocr
+positional_ocr('image.tiff', 'output.txt')
+```
+
+Obtaining extracted text:
+
+```python
+from tesseract_positional import positional_ocr
+text = positional_ocr('image.tiff')
+```
+
+### Via the command line
+
+```
+$ tesseract-positional image.tiff output.txt
+```
+
+## Contributing, Reporting Issues and Other Support
+
+To contribute to Tesseract-Positional, make a pull request. Contributions should include tests for new features added, as well as extensive documentation.
+
+To report problems with the software or feature requests, file an issue. When reporting problems, include information such as error messages, your OS/environment and Python version.
+
+For additional support/questions, contact Travis Kessler (travis.j.kessler@gmail.com).
```

### Comparing `tesseract_positional-0.1.1/tesseract_positional/positional_ocr.py` & `tesseract_positional-0.1.2/tesseract_positional/positional_ocr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,166 +1,156 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-# tesseract_positional/positional_ocr.py
-# v.0.1.1
-# Developed in 2019 by Travis Kessler <travis.j.kessler@gmail.com>
-#
-# Contains function for generating a positional text file from an image
-#
-
-# Stdlib includes
-import re
-
-# 3rd party imports
-import pytesseract
-try:
-    from PIL import Image
-except ImportError:
-    import Image
-
-
-# RegEx's for identifying file extensions
-_IMG_RE = re.compile(r'\.((jp(e)?g)|(png)|(tif(f)?))$', flags=re.IGNORECASE)
-_TXT_RE = re.compile(r'\.txt$', flags=re.IGNORECASE)
-
-# Constant scalars for applying vert/hor spacing based on image dims
-_VERT_SPACING_SCALAR = 0.012
-_HOR_SPACING_SCALAR = 0.018
-
-
-class _Word:
-
-    def __init__(self, word, left, top):
-        ''' _Word object: houses information about a specific extracted word
-
-        Args:
-            word (str): extracted word
-            left (int): position of the word's left bound, in reference to
-                left side of image
-            top (int): position of the word's top bound, in reference to the
-                top of the image
-        '''
-
-        self.word = word
-        self.left = left
-        self.top = top
-
-
-class _Row:
-
-    def __init__(self, top):
-        ''' _Row object: houses words within each horizontal line of the image
-
-        Args:
-            top (int): position of the row's top bound, in reference to the
-                top of the image
-        '''
-
-        self.top = top
-        self.words = []
-
-    @property
-    def row_min(self):
-        ''' Minimum allowed value for same-row association; range of 8 below
-        row's top bound is allowed
-        '''
-
-        return self.top - 8
-
-    @property
-    def row_max(self):
-        ''' Maximum allowed value for same-row association; range of 8 above
-        row's top bound is allowed
-        '''
-
-        return self.top + 8
-
-    def add_word(self, word):
-        ''' Adds a word to the row, sorts all words by left bound
-
-        Args:
-            word (_Word): word to add to row
-        '''
-
-        self.words.append(word)
-        self.words.sort(key=lambda w: w.left)
-
-
-def positional_ocr(base_file, output_file=None):
-    ''' positional_ocr function: extracts text from supplied image, saves
-    positional data to .txt file
-
-    Args:
-        base_file (str): image file (e.g. JPG, PNG, TIF)
-        output_file (str): optional output file, .txt
-
-    Returns:
-        str: string containing extracted positional text
-    '''
-
-    # check for correct extensions
-    if _IMG_RE.search(base_file) is None:
-        raise ValueError('Base file `{}` is not an image'.format(base_file))
-
-    # read image, get dimensions
-    image = Image.open(base_file)
-    im_width, im_height = image.size
-
-    # extract positional data for each word in image
-    data = pytesseract.image_to_data(
-        image,
-        output_type=pytesseract.Output.DICT
-    )
-
-    # create Word objects for each word
-    words = [_Word(word, data['left'][idx], data['top'][idx])
-             for idx, word in enumerate(data['text'])]
-
-    # construct rows from position coordinates
-    rows = []
-    for word in words:
-        row_upper_bounds = [row.row_max for row in rows]
-        row_lower_bounds = [row.row_min for row in rows]
-        new_row = True
-        for idx, ub in enumerate(row_upper_bounds):
-            if word.top < ub and word.top > row_lower_bounds[idx]:
-                rows[idx].add_word(word)
-                new_row = False
-                break
-        if new_row:
-            rows.append(_Row(word.top))
-            rows[-1].add_word(word)
-
-    # convert rows to string
-    text = ''
-    prev_top = 0
-    for row in rows:
-        # add vertical spacing between rows
-        for _ in range(max(int((row.top - prev_top) /
-                       (_VERT_SPACING_SCALAR * im_height)), 1)):
-            text += '\n'
-        prev_top = row.top
-
-        # add horizontal spacing between words
-        left_start = 0
-        prev_word_len = 0
-        for word in row.words:
-            for _ in range(max(int((word.left - left_start - prev_word_len) /
-                           (_HOR_SPACING_SCALAR * im_width)), 1)):
-                text += ' '
-            text += word.word
-            left_start = word.left
-            prev_word_len = len(word.word)
-
-    # if output file specified, save text
-    if output_file is not None:
-        if _TXT_RE.search(output_file) is None:
-            raise ValueError('Output file `{}` is not .txt'.format(
-                output_file
-            ))
-        with open(output_file, 'w') as out_file:
-            out_file.write(text)
-        out_file.close()
-
-    # return text
-    return text
+# Stdlib includes
+import re
+
+# 3rd party imports
+import pytesseract
+try:
+    from PIL import Image
+except ImportError:
+    import Image
+
+
+# RegEx's for identifying file extensions
+_IMG_RE = re.compile(r'\.((jp(e)?g)|(png)|(tif(f)?))$', flags=re.IGNORECASE)
+_TXT_RE = re.compile(r'\.txt$', flags=re.IGNORECASE)
+
+# Constant scalars for applying vert/hor spacing based on image dims
+_VERT_SPACING_SCALAR = 0.012
+_HOR_SPACING_SCALAR = 0.018
+
+
+class _Word:
+
+    def __init__(self, word, left, top):
+        ''' _Word object: houses information about a specific extracted word
+
+        Args:
+            word (str): extracted word
+            left (int): position of the word's left bound, in reference to
+                left side of image
+            top (int): position of the word's top bound, in reference to the
+                top of the image
+        '''
+
+        self.word = word
+        self.left = left
+        self.top = top
+
+
+class _Row:
+
+    def __init__(self, top):
+        ''' _Row object: houses words within each horizontal line of the image
+
+        Args:
+            top (int): position of the row's top bound, in reference to the
+                top of the image
+        '''
+
+        self.top = top
+        self.words = []
+
+    @property
+    def row_min(self):
+        ''' Minimum allowed value for same-row association; range of 8 below
+        row's top bound is allowed
+        '''
+
+        return self.top - 8
+
+    @property
+    def row_max(self):
+        ''' Maximum allowed value for same-row association; range of 8 above
+        row's top bound is allowed
+        '''
+
+        return self.top + 8
+
+    def add_word(self, word):
+        ''' Adds a word to the row, sorts all words by left bound
+
+        Args:
+            word (_Word): word to add to row
+        '''
+
+        self.words.append(word)
+        self.words.sort(key=lambda w: w.left)
+
+
+def positional_ocr(base_file, output_file=None):
+    ''' positional_ocr function: extracts text from supplied image, saves
+    positional data to .txt file
+
+    Args:
+        base_file (str): image file (e.g. JPG, PNG, TIF)
+        output_file (str): optional output file, .txt
+
+    Returns:
+        str: string containing extracted positional text
+    '''
+
+    # check for correct extensions
+    if _IMG_RE.search(base_file) is None:
+        raise ValueError('Base file `{}` is not an image'.format(base_file))
+
+    # read image, get dimensions
+    image = Image.open(base_file)
+    im_width, im_height = image.size
+
+    # extract positional data for each word in image
+    data = pytesseract.image_to_data(
+        image,
+        output_type=pytesseract.Output.DICT
+    )
+
+    # create Word objects for each word
+    words = [_Word(word, data['left'][idx], data['top'][idx])
+             for idx, word in enumerate(data['text'])]
+
+    # construct rows from position coordinates
+    rows = []
+    for word in words:
+        row_upper_bounds = [row.row_max for row in rows]
+        row_lower_bounds = [row.row_min for row in rows]
+        new_row = True
+        for idx, ub in enumerate(row_upper_bounds):
+            if word.top < ub and word.top > row_lower_bounds[idx]:
+                rows[idx].add_word(word)
+                new_row = False
+                break
+        if new_row:
+            rows.append(_Row(word.top))
+            rows[-1].add_word(word)
+
+    # convert rows to string
+    text = ''
+    prev_top = 0
+    for row in rows:
+        # add vertical spacing between rows
+        for _ in range(max(int((row.top - prev_top) /
+                       (_VERT_SPACING_SCALAR * im_height)), 1)):
+            text += '\n'
+        prev_top = row.top
+
+        # add horizontal spacing between words
+        left_start = 0
+        prev_word_len = 0
+        for word in row.words:
+            for _ in range(max(int((word.left - left_start - prev_word_len) /
+                           (_HOR_SPACING_SCALAR * im_width)), 1)):
+                text += ' '
+            text += word.word
+            left_start = word.left
+            prev_word_len = len(word.word)
+
+    # if output file specified, save text
+    if output_file is not None:
+        if _TXT_RE.search(output_file) is None:
+            raise ValueError('Output file `{}` is not .txt'.format(
+                output_file
+            ))
+        with open(output_file, 'w') as out_file:
+            out_file.write(text)
+        out_file.close()
+
+    # return text
+    return text
```

