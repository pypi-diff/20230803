# Comparing `tmp/license_tools-0.3.0.tar.gz` & `tmp/license_tools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_tools-0.3.0.tar", last modified: Mon Jun 19 10:45:23 2023, max compression
+gzip compressed data, was "license_tools-0.3.1.tar", last modified: Thu Aug  3 06:02:36 2023, max compression
```

## Comparing `license_tools-0.3.0.tar` & `license_tools-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-19 10:45:23.917663 license_tools-0.3.0/
--rw-r--r--   0 sdostal   (6000) users      (100)    11358 2022-05-16 19:23:11.000000 license_tools-0.3.0/LICENSE.txt
--rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-06-19 10:45:23.917663 license_tools-0.3.0/PKG-INFO
--rw-r--r--   0 sdostal   (6000) users      (100)     1618 2023-06-15 07:55:19.000000 license_tools-0.3.0/README.md
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-19 10:45:23.917663 license_tools-0.3.0/license_tools/
--rw-r--r--   0 sdostal   (6000) users      (100)        0 2021-01-11 15:34:09.000000 license_tools-0.3.0/license_tools/__init__.py
--rw-r--r--   0 sdostal   (6000) users      (100)     2569 2023-06-15 12:33:41.000000 license_tools-0.3.0/license_tools/__main__.py
--rw-r--r--   0 sdostal   (6000) users      (100)    16453 2023-06-19 10:44:27.000000 license_tools-0.3.0/license_tools/scancode_tools.py
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-19 10:45:23.917663 license_tools-0.3.0/license_tools.egg-info/
--rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-06-19 10:45:23.000000 license_tools-0.3.0/license_tools.egg-info/PKG-INFO
--rw-r--r--   0 sdostal   (6000) users      (100)      298 2023-06-19 10:45:23.000000 license_tools-0.3.0/license_tools.egg-info/SOURCES.txt
--rw-r--r--   0 sdostal   (6000) users      (100)        1 2023-06-19 10:45:23.000000 license_tools-0.3.0/license_tools.egg-info/dependency_links.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       68 2023-06-19 10:45:23.000000 license_tools-0.3.0/license_tools.egg-info/requires.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       14 2023-06-19 10:45:23.000000 license_tools-0.3.0/license_tools.egg-info/top_level.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       38 2023-06-19 10:45:23.917663 license_tools-0.3.0/setup.cfg
--rw-r--r--   0 sdostal   (6000) users      (100)     1423 2023-06-16 09:52:25.000000 license_tools-0.3.0/setup.py
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-08-03 06:02:36.287377 license_tools-0.3.1/
+-rw-r--r--   0 sdostal   (6000) users      (100)    11358 2022-05-16 19:23:11.000000 license_tools-0.3.1/LICENSE.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-08-03 06:02:36.287377 license_tools-0.3.1/PKG-INFO
+-rw-r--r--   0 sdostal   (6000) users      (100)     1618 2023-06-15 07:55:19.000000 license_tools-0.3.1/README.md
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-08-03 06:02:36.283377 license_tools-0.3.1/license_tools/
+-rw-r--r--   0 sdostal   (6000) users      (100)        0 2021-01-11 15:34:09.000000 license_tools-0.3.1/license_tools/__init__.py
+-rw-r--r--   0 sdostal   (6000) users      (100)     2569 2023-06-15 12:33:41.000000 license_tools-0.3.1/license_tools/__main__.py
+-rw-r--r--   0 sdostal   (6000) users      (100)    16750 2023-08-02 07:16:01.000000 license_tools-0.3.1/license_tools/scancode_tools.py
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-08-03 06:02:36.287377 license_tools-0.3.1/license_tools.egg-info/
+-rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-08-03 06:02:36.000000 license_tools-0.3.1/license_tools.egg-info/PKG-INFO
+-rw-r--r--   0 sdostal   (6000) users      (100)      298 2023-08-03 06:02:36.000000 license_tools-0.3.1/license_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)        1 2023-08-03 06:02:36.000000 license_tools-0.3.1/license_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)       68 2023-08-03 06:02:36.000000 license_tools-0.3.1/license_tools.egg-info/requires.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)       14 2023-08-03 06:02:36.000000 license_tools-0.3.1/license_tools.egg-info/top_level.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)       38 2023-08-03 06:02:36.287377 license_tools-0.3.1/setup.cfg
+-rw-r--r--   0 sdostal   (6000) users      (100)     1423 2023-08-02 13:24:11.000000 license_tools-0.3.1/setup.py
```

### Comparing `license_tools-0.3.0/LICENSE.txt` & `license_tools-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `license_tools-0.3.0/PKG-INFO` & `license_tools-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license_tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: Collection of tools for working with Open Source licenses
 Home-page: https://github.com/stefan6419846/license_tools
 Author: stefan6419846
 License: Apache-2.0
 Keywords: open source,license,package,dependency,licensing
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `license_tools-0.3.0/README.md` & `license_tools-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `license_tools-0.3.0/license_tools/__main__.py` & `license_tools-0.3.1/license_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `license_tools-0.3.0/license_tools/scancode_tools.py` & `license_tools-0.3.1/license_tools/scancode_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 configuration and returning `dataclass` instances instead of dictionaries.
 """
 
 from __future__ import annotations
 
 import atexit
 import datetime
+import math
 import shutil
 import subprocess
 import zipfile
 from collections import defaultdict
 from dataclasses import dataclass, field as dataclass_field
 from pathlib import Path
 from tempfile import TemporaryDirectory
@@ -545,26 +546,30 @@
                 path=Path(file_path),
                 short_path=file_path,
                 retrieval_flags=retrieval_flags,
             )
         ]
 
     # Display the file-level results.
+    max_path_length = max(len(result.short_path) for result in results)
     for result in results:
         scores = result.licenses.get_scores_of_detected_license_expression_spdx()
         print(
-            f"{result.short_path:>50}",
+            f"{result.short_path:>{max_path_length}}",
             f"{result.licenses.detected_license_expression_spdx:>70}"
             if result.licenses.detected_license_expression_spdx
             else " " * 70,
             scores if scores else "",
         )
         license_counts[result.licenses.detected_license_expression_spdx] += 1
 
     # Display the license-level results.
     print()
-    print("=" * 130)
+    columns = shutil.get_terminal_size((80, 20)).columns
+    print("=" * columns)
     print()
+    count_length = max(math.log10(count) for count in license_counts.values())
+    count_length = int(count_length) + 1
     for identifier in sorted(license_counts, key=str):
-        print(f"{identifier!s:>70}", f"{license_counts[identifier]:>4d}")
+        print(f"{identifier!s:>70}", f"{license_counts[identifier]:>{count_length + 1}d}")
 
     return results
```

### Comparing `license_tools-0.3.0/license_tools.egg-info/PKG-INFO` & `license_tools-0.3.1/license_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: Collection of tools for working with Open Source licenses
 Home-page: https://github.com/stefan6419846/license_tools
 Author: stefan6419846
 License: Apache-2.0
 Keywords: open source,license,package,dependency,licensing
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `license_tools-0.3.0/setup.py` & `license_tools-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ROOT_DIRECTORY = Path(__file__).parent.resolve()
 
 
 setuptools.setup(
     name='license_tools',
     description='Collection of tools for working with Open Source licenses',
-    version='0.3.0',
+    version='0.3.1',
     license='Apache-2.0',
     long_description=Path(ROOT_DIRECTORY / 'README.md').read_text(encoding='UTF-8'),
     long_description_content_type='text/markdown',
     author='stefan6419846',
     url='https://github.com/stefan6419846/license_tools',
     packages=setuptools.find_packages(),
     include_package_data=True,
```

