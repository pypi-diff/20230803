# Comparing `tmp/misk-0.7.1.tar.gz` & `tmp/misk-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misk-0.7.1.tar", last modified: Mon Jul 17 08:40:55 2023, max compression
+gzip compressed data, was "misk-0.8.0.tar", last modified: Thu Aug  3 12:41:47 2023, max compression
```

## Comparing `misk-0.7.1.tar` & `misk-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 08:40:55.800930 misk-0.7.1/
--rw-rw-rw-   0        0        0     1094 2021-04-14 17:40:14.000000 misk-0.7.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1562 2023-07-17 08:40:55.800930 misk-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0       73 2021-04-14 20:52:46.000000 misk-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 08:40:55.795930 misk-0.7.1/misk/
--rw-rw-rw-   0        0        0      331 2023-07-17 08:39:10.000000 misk-0.7.1/misk/__init__.py
--rw-rw-rw-   0        0        0    12151 2023-07-17 08:39:03.000000 misk-0.7.1/misk/functions.py
--rw-rw-rw-   0        0        0     1342 2023-07-17 08:39:06.000000 misk-0.7.1/misk/timers.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:40:55.799930 misk-0.7.1/misk.egg-info/
--rw-rw-rw-   0        0        0     1562 2023-07-17 08:40:55.000000 misk-0.7.1/misk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-07-17 08:40:55.000000 misk-0.7.1/misk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:40:55.000000 misk-0.7.1/misk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 08:40:55.000000 misk-0.7.1/misk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-17 08:40:55.000000 misk-0.7.1/misk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 08:40:55.800930 misk-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1679 2023-07-17 08:39:12.000000 misk-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:41:47.947018 misk-0.8.0/
+-rw-rw-rw-   0        0        0     1094 2021-04-14 17:40:14.000000 misk-0.8.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1789 2023-08-03 12:41:47.947018 misk-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2021-04-14 20:52:46.000000 misk-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 12:41:47.942019 misk-0.8.0/misk/
+-rw-rw-rw-   0        0        0      331 2023-07-17 08:39:10.000000 misk-0.8.0/misk/__init__.py
+-rw-rw-rw-   0        0        0    13658 2023-08-03 12:40:38.000000 misk-0.8.0/misk/functions.py
+-rw-rw-rw-   0        0        0     1342 2023-07-17 08:39:06.000000 misk-0.8.0/misk/timers.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:41:47.946018 misk-0.8.0/misk.egg-info/
+-rw-rw-rw-   0        0        0     1789 2023-08-03 12:41:47.000000 misk-0.8.0/misk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-08-03 12:41:47.000000 misk-0.8.0/misk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 12:41:47.000000 misk-0.8.0/misk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-03 12:41:47.000000 misk-0.8.0/misk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-03 12:41:47.000000 misk-0.8.0/misk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 12:41:47.947018 misk-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1679 2023-08-03 12:38:34.000000 misk-0.8.0/setup.py
```

### Comparing `misk-0.7.1/LICENSE.txt` & `misk-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `misk-0.7.1/PKG-INFO` & `misk-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 Metadata-Version: 2.1
 Name: misk
-Version: 0.7.1
+Version: 0.8.0
 Summary: Miscellaneous useful bits for python 3.
 Home-page: https://github.com/marzer/misk
 Download-URL: https://pypi.org/project/misk/
 Author: Mark Gillard
 Author-email: mark.gillard@outlook.com.au
 License: MIT
 Project-URL: Source, https://github.com/marzer/misk
 Project-URL: Tracker, https://github.com/marzer/misk/issues
 Keywords: utilities
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # misk
 Miscellaneous useful bits for python 3.
 
 ```
 pip install misk
 ```
 
 <br><br>
 ## Changelog
 
+## v0.8.0 - 2023-08-03
+
+-   Fixed `replace_metavar` erroneously treating `\` as regex escapes
+-   Added `repeat_pattern()`
+-   Added `reflow_text()`
+-   Added `to_snake_case()`
+-   Added `to_pascal_case()`
+-   Added `remove_duplicates()`
+
 ## v0.7.1 - 2023-07-17
 
 -   Fixed `copy_file()` not following symlinks
 
 ## v0.7.0 - 2022-09-05
 
 -   Added `none` filter to `enumerate_files()`
@@ -61,8 +69,7 @@
 ## v0.3.0 - 2021-04-20
 
 -   Decoupled begin and end logger for `ScopeTimer`
 
 ## v0.2.0 - 2021-04-18
 
 -   Fixed incorrect boolean logic in `assert_existing_XXXXX()`
-
```

### Comparing `misk-0.7.1/misk/functions.py` & `misk-0.8.0/misk/functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import io
 import logging
 import pathlib
 import re
 import shutil
 import subprocess
 import sys
+import textwrap
 import traceback
 from pathlib import Path
 from typing import List, Union
 
 import requests
 
 __all__ = [
@@ -40,14 +41,19 @@
 	r'sha256',
 	r'is_pow2',
 	r'next_pow2',
 	r'replace_metavar',
 	r'tabify',
 	r'untabify',
 	r'reindent',
+	r'repeat_pattern',
+	r'reflow_text',
+	r'remove_duplicates',
+	r'to_snake_case',
+	r'to_pascal_case'
 ]
 
 #=======================================================================================================================
 # shared lib state
 #=======================================================================================================================
 
 
@@ -421,14 +427,15 @@
 	assert text is not None
 
 	if not isinstance(name, str):
 		name = str(name)
 	name = re.escape(name.strip())
 	if not isinstance(repl, str):
 		repl = str(repl)
+	repl = repl.replace('\\','\\\\')
 	if not isinstance(text, str):
 		text = str(text)
 
 	#  {% name %}
 	text = re.sub(rf'{{%[\t ]*{name}[\t ]*%}}', repl, text)
 
 	#  $( name ) and %( name )
@@ -510,7 +517,73 @@
 		lstrip = min(len(s[i]) - len(stripped), lstrip)
 
 	for i in range(len(s)):
 		if s[i]:
 			s[i] = tabify(indent + s[i][lstrip:], tab_width=tab_width)
 
 	return '\n'.join(s)
+
+
+
+def repeat_pattern(pattern: str, len: int) -> str:
+	'''
+	Repeats a string pattern up to a specific length.
+	'''
+	if len(pattern) == 1:
+		return pattern * len
+	text = ''
+	for i in range(0, len):
+		text = text + pattern[i % len(pattern)]
+	return text
+
+
+
+def reflow_text(text: str, line_length=120, tab_size=4) -> str:
+	'''
+	Re-wraps text over lines of a particular length.
+	'''
+	text = text.replace('\n\n', '\b')
+	text = text.replace('\n', ' ')
+	text = text.replace('\b', '\n')
+	text = text.split('\n')
+	for i in range(len(text)):
+		text[i] = '\n'.join(textwrap.wrap(text[i], width=int(line_length), tabsize=int(tab_size)))
+	return '\n\n'.join(text)
+
+
+
+def remove_duplicates(vals: list) -> list:
+	'''
+	Removes duplicate items from a list while preserving order.
+	'''
+	new_vals = []
+	for v in coerce_collection(vals):
+		if v not in new_vals:
+			new_vals.append(v)
+	return new_vals
+
+
+
+def to_snake_case(s: str) -> str:
+	'''
+	Converts text to snake_case.
+	'''
+	s = str(s)
+	s = s.strip()
+	s = re.sub('(?:\s|-)+', '_', s)
+	s = re.sub('__+', '_', s)
+	s = re.sub('([a-z])([A-Z])', lambda m: m[1] + '_' + m[2].lower(), s)
+	s = s.lower()
+	return s
+
+
+
+def to_pascal_case(s: str) -> str:
+	'''
+	Converts text to PascalCase.
+	'''
+	s = to_snake_case(s)
+	s = re.sub('_([a-z])', lambda m: m[1].upper(), s)
+	s = s.strip('_')
+	if len(s):
+		s = s[:1].upper() + s[1:]
+	return s
```

### Comparing `misk-0.7.1/misk/timers.py` & `misk-0.8.0/misk/timers.py`

 * *Files identical despite different names*

### Comparing `misk-0.7.1/misk.egg-info/PKG-INFO` & `misk-0.8.0/misk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 Metadata-Version: 2.1
 Name: misk
-Version: 0.7.1
+Version: 0.8.0
 Summary: Miscellaneous useful bits for python 3.
 Home-page: https://github.com/marzer/misk
 Download-URL: https://pypi.org/project/misk/
 Author: Mark Gillard
 Author-email: mark.gillard@outlook.com.au
 License: MIT
 Project-URL: Source, https://github.com/marzer/misk
 Project-URL: Tracker, https://github.com/marzer/misk/issues
 Keywords: utilities
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # misk
 Miscellaneous useful bits for python 3.
 
 ```
 pip install misk
 ```
 
 <br><br>
 ## Changelog
 
+## v0.8.0 - 2023-08-03
+
+-   Fixed `replace_metavar` erroneously treating `\` as regex escapes
+-   Added `repeat_pattern()`
+-   Added `reflow_text()`
+-   Added `to_snake_case()`
+-   Added `to_pascal_case()`
+-   Added `remove_duplicates()`
+
 ## v0.7.1 - 2023-07-17
 
 -   Fixed `copy_file()` not following symlinks
 
 ## v0.7.0 - 2022-09-05
 
 -   Added `none` filter to `enumerate_files()`
@@ -61,8 +69,7 @@
 ## v0.3.0 - 2021-04-20
 
 -   Decoupled begin and end logger for `ScopeTimer`
 
 ## v0.2.0 - 2021-04-18
 
 -   Fixed incorrect boolean logic in `assert_existing_XXXXX()`
-
```

### Comparing `misk-0.7.1/setup.py` & `misk-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 CHANGELOG = ''
 with open(r'CHANGELOG.md', encoding=r'utf-8') as file:
 	CHANGELOG = f'\n\n{file.read()}\n\n'
 CHANGELOG = re.sub(r'\n#+\s*Changelog\s*?\n', '\n## Changelog\n', CHANGELOG, flags=re.I).strip()
 
 SETUP_ARGS = {
 	r'name': r'misk',
-	r'version': r'0.7.1',
+	r'version': r'0.8.0',
 	r'description': r'Miscellaneous useful bits for python 3.',
 	r'long_description_content_type': r'text/markdown',
 	r'long_description': f'{README}\n<br><br>\n{CHANGELOG}'.strip(),
 	r'license': r'MIT',
 	r'packages': find_packages(),
 	r'author': r'Mark Gillard',
 	r'author_email': r'mark.gillard@outlook.com.au',
```

