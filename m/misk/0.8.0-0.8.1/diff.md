# Comparing `tmp/misk-0.8.0.tar.gz` & `tmp/misk-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misk-0.8.0.tar", last modified: Thu Aug  3 12:41:47 2023, max compression
+gzip compressed data, was "misk-0.8.1.tar", last modified: Thu Aug  3 12:48:10 2023, max compression
```

## Comparing `misk-0.8.0.tar` & `misk-0.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 12:41:47.947018 misk-0.8.0/
--rw-rw-rw-   0        0        0     1094 2021-04-14 17:40:14.000000 misk-0.8.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1789 2023-08-03 12:41:47.947018 misk-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0       73 2021-04-14 20:52:46.000000 misk-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 12:41:47.942019 misk-0.8.0/misk/
--rw-rw-rw-   0        0        0      331 2023-07-17 08:39:10.000000 misk-0.8.0/misk/__init__.py
--rw-rw-rw-   0        0        0    13658 2023-08-03 12:40:38.000000 misk-0.8.0/misk/functions.py
--rw-rw-rw-   0        0        0     1342 2023-07-17 08:39:06.000000 misk-0.8.0/misk/timers.py
-drwxrwxrwx   0        0        0        0 2023-08-03 12:41:47.946018 misk-0.8.0/misk.egg-info/
--rw-rw-rw-   0        0        0     1789 2023-08-03 12:41:47.000000 misk-0.8.0/misk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-08-03 12:41:47.000000 misk-0.8.0/misk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 12:41:47.000000 misk-0.8.0/misk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-03 12:41:47.000000 misk-0.8.0/misk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-03 12:41:47.000000 misk-0.8.0/misk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 12:41:47.947018 misk-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1679 2023-08-03 12:38:34.000000 misk-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:48:10.358135 misk-0.8.1/
+-rw-rw-rw-   0        0        0     1094 2021-04-14 17:40:14.000000 misk-0.8.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1789 2023-08-03 12:48:10.358135 misk-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2021-04-14 20:52:46.000000 misk-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 12:48:10.353136 misk-0.8.1/misk/
+-rw-rw-rw-   0        0        0      331 2023-07-17 08:39:10.000000 misk-0.8.1/misk/__init__.py
+-rw-rw-rw-   0        0        0    13664 2023-08-03 12:47:16.000000 misk-0.8.1/misk/functions.py
+-rw-rw-rw-   0        0        0     1342 2023-07-17 08:39:06.000000 misk-0.8.1/misk/timers.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:48:10.357135 misk-0.8.1/misk.egg-info/
+-rw-rw-rw-   0        0        0     1789 2023-08-03 12:48:10.000000 misk-0.8.1/misk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-08-03 12:48:10.000000 misk-0.8.1/misk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 12:48:10.000000 misk-0.8.1/misk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-03 12:48:10.000000 misk-0.8.1/misk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-03 12:48:10.000000 misk-0.8.1/misk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 12:48:10.358135 misk-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1679 2023-08-03 12:47:59.000000 misk-0.8.1/setup.py
```

### Comparing `misk-0.8.0/LICENSE.txt` & `misk-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `misk-0.8.0/PKG-INFO` & `misk-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misk
-Version: 0.8.0
+Version: 0.8.1
 Summary: Miscellaneous useful bits for python 3.
 Home-page: https://github.com/marzer/misk
 Download-URL: https://pypi.org/project/misk/
 Author: Mark Gillard
 Author-email: mark.gillard@outlook.com.au
 License: MIT
 Project-URL: Source, https://github.com/marzer/misk
```

### Comparing `misk-0.8.0/misk/functions.py` & `misk-0.8.1/misk/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -520,22 +520,22 @@
 		if s[i]:
 			s[i] = tabify(indent + s[i][lstrip:], tab_width=tab_width)
 
 	return '\n'.join(s)
 
 
 
-def repeat_pattern(pattern: str, len: int) -> str:
+def repeat_pattern(pattern: str, length: int) -> str:
 	'''
 	Repeats a string pattern up to a specific length.
 	'''
 	if len(pattern) == 1:
-		return pattern * len
+		return pattern * length
 	text = ''
-	for i in range(0, len):
+	for i in range(length):
 		text = text + pattern[i % len(pattern)]
 	return text
 
 
 
 def reflow_text(text: str, line_length=120, tab_size=4) -> str:
 	'''
```

### Comparing `misk-0.8.0/misk/timers.py` & `misk-0.8.1/misk/timers.py`

 * *Files identical despite different names*

### Comparing `misk-0.8.0/misk.egg-info/PKG-INFO` & `misk-0.8.1/misk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misk
-Version: 0.8.0
+Version: 0.8.1
 Summary: Miscellaneous useful bits for python 3.
 Home-page: https://github.com/marzer/misk
 Download-URL: https://pypi.org/project/misk/
 Author: Mark Gillard
 Author-email: mark.gillard@outlook.com.au
 License: MIT
 Project-URL: Source, https://github.com/marzer/misk
```

### Comparing `misk-0.8.0/setup.py` & `misk-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 CHANGELOG = ''
 with open(r'CHANGELOG.md', encoding=r'utf-8') as file:
 	CHANGELOG = f'\n\n{file.read()}\n\n'
 CHANGELOG = re.sub(r'\n#+\s*Changelog\s*?\n', '\n## Changelog\n', CHANGELOG, flags=re.I).strip()
 
 SETUP_ARGS = {
 	r'name': r'misk',
-	r'version': r'0.8.0',
+	r'version': r'0.8.1',
 	r'description': r'Miscellaneous useful bits for python 3.',
 	r'long_description_content_type': r'text/markdown',
 	r'long_description': f'{README}\n<br><br>\n{CHANGELOG}'.strip(),
 	r'license': r'MIT',
 	r'packages': find_packages(),
 	r'author': r'Mark Gillard',
 	r'author_email': r'mark.gillard@outlook.com.au',
```

