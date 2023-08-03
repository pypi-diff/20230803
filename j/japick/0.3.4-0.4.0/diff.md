# Comparing `tmp/japick-0.3.4.tar.gz` & `tmp/japick-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "japick-0.3.4.tar", last modified: Fri Sep 17 05:53:21 2021, max compression
+gzip compressed data, was "japick-0.4.0.tar", last modified: Thu Aug  3 06:11:24 2023, max compression
```

## Comparing `japick-0.3.4.tar` & `japick-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxrwxr-x   0 hirokiky  (1000) hirokiky  (1000)        0 2021-09-17 05:53:21.421707 japick-0.3.4/
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      229 2021-09-17 05:53:21.421707 japick-0.3.4/PKG-INFO
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      471 2021-08-31 08:25:02.000000 japick-0.3.4/README.md
-drwxrwxr-x   0 hirokiky  (1000) hirokiky  (1000)        0 2021-09-17 05:53:21.417706 japick-0.3.4/japick/
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      118 2021-09-02 05:27:50.000000 japick-0.3.4/japick/__init__.py
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1309 2021-09-05 06:06:16.000000 japick-0.3.4/japick/cleaner.py
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1722 2021-09-05 06:18:33.000000 japick-0.3.4/japick/lines.py
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      528 2021-08-31 08:22:13.000000 japick-0.3.4/japick/main.py
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     3395 2021-09-05 06:51:23.000000 japick-0.3.4/japick/paragraph.py
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      743 2021-09-17 05:51:49.000000 japick-0.3.4/japick/syntax.py
-drwxrwxr-x   0 hirokiky  (1000) hirokiky  (1000)        0 2021-09-17 05:53:21.421707 japick-0.3.4/japick.egg-info/
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      229 2021-09-17 05:53:21.000000 japick-0.3.4/japick.egg-info/PKG-INFO
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      287 2021-09-17 05:53:21.000000 japick-0.3.4/japick.egg-info/SOURCES.txt
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)        1 2021-09-17 05:53:21.000000 japick-0.3.4/japick.egg-info/dependency_links.txt
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)       35 2021-09-17 05:53:21.000000 japick-0.3.4/japick.egg-info/requires.txt
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)        7 2021-09-17 05:53:21.000000 japick-0.3.4/japick.egg-info/top_level.txt
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      244 2021-08-31 00:04:28.000000 japick-0.3.4/pyproject.toml
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)       38 2021-09-17 05:53:21.421707 japick-0.3.4/setup.cfg
--rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      306 2021-09-17 05:52:45.000000 japick-0.3.4/setup.py
+drwxrwxr-x   0 hirokiky  (1000) hirokiky  (1000)        0 2023-08-03 06:11:24.666008 japick-0.4.0/
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      156 2023-08-03 06:11:24.666008 japick-0.4.0/PKG-INFO
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      471 2021-08-31 08:25:02.000000 japick-0.4.0/README.md
+drwxrwxr-x   0 hirokiky  (1000) hirokiky  (1000)        0 2023-08-03 06:11:24.662008 japick-0.4.0/japick/
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      118 2021-09-02 05:27:50.000000 japick-0.4.0/japick/__init__.py
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1309 2021-09-05 06:06:16.000000 japick-0.4.0/japick/cleaner.py
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1722 2021-09-05 06:18:33.000000 japick-0.4.0/japick/lines.py
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      528 2021-08-31 08:22:13.000000 japick-0.4.0/japick/main.py
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     3477 2023-08-03 06:05:51.000000 japick-0.4.0/japick/paragraph.py
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      743 2021-09-17 05:51:49.000000 japick-0.4.0/japick/syntax.py
+drwxrwxr-x   0 hirokiky  (1000) hirokiky  (1000)        0 2023-08-03 06:11:24.662008 japick-0.4.0/japick.egg-info/
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      156 2023-08-03 06:11:24.000000 japick-0.4.0/japick.egg-info/PKG-INFO
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      372 2023-08-03 06:11:24.000000 japick-0.4.0/japick.egg-info/SOURCES.txt
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)        1 2023-08-03 06:11:24.000000 japick-0.4.0/japick.egg-info/dependency_links.txt
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)       35 2023-08-03 06:11:24.000000 japick-0.4.0/japick.egg-info/requires.txt
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)        7 2023-08-03 06:11:24.000000 japick-0.4.0/japick.egg-info/top_level.txt
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      244 2021-08-31 00:04:28.000000 japick-0.4.0/pyproject.toml
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)       38 2023-08-03 06:11:24.666008 japick-0.4.0/setup.cfg
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)      306 2023-08-03 06:10:08.000000 japick-0.4.0/setup.py
+drwxrwxr-x   0 hirokiky  (1000) hirokiky  (1000)        0 2023-08-03 06:11:24.662008 japick-0.4.0/tests/
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     5356 2021-09-05 06:16:49.000000 japick-0.4.0/tests/test_cleaner.py
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     2222 2021-09-05 06:18:33.000000 japick-0.4.0/tests/test_lines.py
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     1328 2021-09-05 06:52:29.000000 japick-0.4.0/tests/test_main.py
+-rw-rw-r--   0 hirokiky  (1000) hirokiky  (1000)     3303 2023-08-03 06:07:36.000000 japick-0.4.0/tests/test_paragraph.py
```

### Comparing `japick-0.3.4/japick/cleaner.py` & `japick-0.4.0/japick/cleaner.py`

 * *Files identical despite different names*

### Comparing `japick-0.3.4/japick/lines.py` & `japick-0.4.0/japick/lines.py`

 * *Files identical despite different names*

### Comparing `japick-0.3.4/japick/main.py` & `japick-0.4.0/japick/main.py`

 * *Files identical despite different names*

### Comparing `japick-0.3.4/japick/paragraph.py` & `japick-0.4.0/japick/paragraph.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,36 +42,36 @@
     @property
     def body(self):
         if self._body is not None:
             return self._body
         self._body = "\n".join(line.strip().replace(NULL_SYMBOL, "") for line in self.lines)
         return self._body
 
-    def as_original_pos(self, index) -> Pos:
+    def as_original_pos(self, index, lazy=False) -> Pos:
         before_lines = self.body[:index].split("\n")
         pos = Pos(
             len(before_lines) - 1,
             len(before_lines[-1]),
         )
         # Convert column number to original position.
         line = self.lines[pos.line]
         left_margin = len(line) - len(line.lstrip())
         chunks = line[left_margin:].split(NULL_SYMBOL)
         num_null_symbols = 0
         current = 0
         for num_null_symbols, chunk in enumerate(chunks):
             current += len(chunk)
-            if pos.ch < current:
+            if (not lazy and pos.ch < current) or (lazy and pos.ch <= current):
                 break
         pos.line += self.number
         pos.ch += left_margin + num_null_symbols
         return pos
 
-    def as_original_index(self, index: int) -> int:
-        pos = self.as_original_pos(index)
+    def as_original_index(self, index: int, lazy=False) -> int:
+        pos = self.as_original_pos(index, lazy=lazy)
         num_lines = pos.line - self.number
         before_index = sum(len(line) for line in self.lines[:num_lines]) + num_lines
         return self.index + before_index + pos.ch
 
     def __str__(self) -> str:
         return self.body
```

### Comparing `japick-0.3.4/japick/syntax.py` & `japick-0.4.0/japick/syntax.py`

 * *Files identical despite different names*

