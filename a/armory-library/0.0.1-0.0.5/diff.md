# Comparing `tmp/armory_library-0.0.1-py3-none-any.whl.zip` & `tmp/armory_library-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3163 bytes, number of entries: 8
+Zip file size: 3286 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      137 b- defN 20-Feb-02 00:00 charmory/__about__.py
 -rw-r--r--  2.0 unx      115 b- defN 20-Feb-02 00:00 charmory/__init__.py
--rw-r--r--  2.0 unx      111 b- defN 20-Feb-02 00:00 charmory/charmory.py
-?rw-r--r--  2.0 unx     1048 b- defN 20-Feb-02 00:00 armory_library-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 armory_library-0.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx       52 b- defN 20-Feb-02 00:00 armory_library-0.0.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1107 b- defN 20-Feb-02 00:00 armory_library-0.0.1.dist-info/licenses/LICENSE.txt
-?rw-r--r--  2.0 unx      666 b- defN 20-Feb-02 00:00 armory_library-0.0.1.dist-info/RECORD
-8 files, 3323 bytes uncompressed, 1991 bytes compressed:  40.1%
+-rw-r--r--  2.0 unx      243 b- defN 20-Feb-02 00:00 charmory/main.py
+?rw-r--r--  2.0 unx     1165 b- defN 20-Feb-02 00:00 armory_library-0.0.5.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 armory_library-0.0.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx       48 b- defN 20-Feb-02 00:00 armory_library-0.0.5.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1107 b- defN 20-Feb-02 00:00 armory_library-0.0.5.dist-info/licenses/LICENSE.txt
+?rw-r--r--  2.0 unx      662 b- defN 20-Feb-02 00:00 armory_library-0.0.5.dist-info/RECORD
+8 files, 3564 bytes uncompressed, 2122 bytes compressed:  40.5%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: charmory/__about__.py
 Comment: 
 
 Filename: charmory/__init__.py
 Comment: 
 
-Filename: charmory/charmory.py
+Filename: charmory/main.py
 Comment: 
 
-Filename: armory_library-0.0.1.dist-info/METADATA
+Filename: armory_library-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: armory_library-0.0.1.dist-info/WHEEL
+Filename: armory_library-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: armory_library-0.0.1.dist-info/entry_points.txt
+Filename: armory_library-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: armory_library-0.0.1.dist-info/licenses/LICENSE.txt
+Filename: armory_library-0.0.5.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: armory_library-0.0.1.dist-info/RECORD
+Filename: armory_library-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## charmory/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present matt wartell <matt.wartell@twosixtech.com>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "0.0.1"
+__version__ = "0.0.5"
```

## Comparing `armory_library-0.0.1.dist-info/METADATA` & `armory_library-0.0.5.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: armory-library
-Version: 0.0.1
+Version: 0.0.5
 Project-URL: Documentation, https://github.com/mwartell/armory-library#readme
 Project-URL: Issues, https://github.com/mwartell/armory-library/issues
 Project-URL: Source, https://github.com/mwartell/armory-library
 Author-email: matt wartell <matt.wartell@twosixtech.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
+Requires-Dist: black
+Requires-Dist: pytest
 Description-Content-Type: text/markdown
 
 # armory-library
 
+This is a placeholder for the release of armory-library expected in 2023
+
 [![PyPI - Version](https://img.shields.io/pypi/v/armory-library.svg)](https://pypi.org/project/armory-library)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/armory-library.svg)](https://pypi.org/project/armory-library)
 
 -----
 
 **Table of Contents**
```

## Comparing `armory_library-0.0.1.dist-info/licenses/LICENSE.txt` & `armory_library-0.0.5.dist-info/licenses/LICENSE.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 MIT License
 
 Copyright (c) 2023-present matt wartell <matt.wartell@twosixtech.com>
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this
+software and associated documentation files (the "Software"), to deal in the Software
+without restriction, including without limitation the rights to use, copy, modify,
+merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to the following
+conditions:
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all copies or
+substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
+INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR
+PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT
+OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+OTHER DEALINGS IN THE SOFTWARE.
```

