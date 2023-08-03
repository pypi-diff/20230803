# Comparing `tmp/pyjt-0.2.0.tar.gz` & `tmp/pyjt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjt-0.2.0.tar", last modified: Wed Aug  2 14:50:36 2023, max compression
+gzip compressed data, was "pyjt-0.2.1.tar", last modified: Wed Aug  2 17:48:19 2023, max compression
```

## Comparing `pyjt-0.2.0.tar` & `pyjt-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:36.896167 pyjt-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-02 14:49:48.000000 pyjt-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-02 14:50:36.896167 pyjt-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 14:49:48.000000 pyjt-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:36.892167 pyjt-0.2.0/pyjt/
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/ComponentFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/Fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/Frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/Inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/Robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:36.896167 pyjt-0.2.0/pyjt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-02 14:50:36.000000 pyjt-0.2.0/pyjt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-02 14:50:36.000000 pyjt-0.2.0/pyjt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:50:36.000000 pyjt-0.2.0/pyjt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 14:50:36.000000 pyjt-0.2.0/pyjt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 14:50:36.000000 pyjt-0.2.0/pyjt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:50:36.896167 pyjt-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:36.896167 pyjt-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 14:49:48.000000 pyjt-0.2.0/tests/test_framefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 14:49:48.000000 pyjt-0.2.0/tests/test_textfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:48:19.170328 pyjt-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-02 17:47:30.000000 pyjt-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-02 17:48:19.170328 pyjt-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 17:47:30.000000 pyjt-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:48:19.170328 pyjt-0.2.1/pyjt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/ComponentFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/Fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/Robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:48:19.170328 pyjt-0.2.1/pyjt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-02 17:48:19.000000 pyjt-0.2.1/pyjt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-02 17:48:19.000000 pyjt-0.2.1/pyjt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:48:19.000000 pyjt-0.2.1/pyjt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 17:48:19.000000 pyjt-0.2.1/pyjt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 17:48:19.000000 pyjt-0.2.1/pyjt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:48:19.170328 pyjt-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:48:19.170328 pyjt-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 17:47:30.000000 pyjt-0.2.1/tests/test_framefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-02 17:47:30.000000 pyjt-0.2.1/tests/test_textfield.py
```

### Comparing `pyjt-0.2.0/LICENSE` & `pyjt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjt-0.2.0/PKG-INFO` & `pyjt-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.2.0
+Version: 0.2.1
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyjt-0.2.0/README.md` & `pyjt-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyjt-0.2.0/pyjt/ComponentFinder.py` & `pyjt-0.2.1/pyjt/ComponentFinder.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.2.0/pyjt/Fixture.py` & `pyjt-0.2.1/pyjt/Fixture.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.2.0/pyjt/Frame.py` & `pyjt-0.2.1/pyjt/Frame.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.2.0/pyjt/Inspector.py` & `pyjt-0.2.1/pyjt/Inspector.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.2.0/pyjt/Proxy.py` & `pyjt-0.2.1/pyjt/Proxy.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.2.0/pyjt/Robot.py` & `pyjt-0.2.1/pyjt/Robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,36 +94,36 @@
                 '8': [KeyEvent.VK_8],
                 '9': [KeyEvent.VK_9],
                 '-': [KeyEvent.VK_MINUS],
                 '=': [KeyEvent.VK_EQUALS],
                 '~': [KeyEvent.VK_SHIFT, KeyEvent.VK_BACK_QUOTE],
                 '!': [KeyEvent.VK_SHIFT, KeyEvent.VK_1],
                 '@': [KeyEvent.VK_SHIFT, KeyEvent.VK_2],
-                '#': [KeyEvent.VK_NUMBER_SIGN],
-                '$': [KeyEvent.VK_DOLLAR],
+                '#': [KeyEvent.VK_SHIFT, KeyEvent.VK_NUMBER_SIGN],
+                '$': [KeyEvent.VK_SHIFT, KeyEvent.VK_4],
                 '%': [KeyEvent.VK_SHIFT, KeyEvent.VK_5],
-                '^': [KeyEvent.VK_CIRCUMFLEX],
-                '&': [KeyEvent.VK_AMPERSAND],
-                '*': [KeyEvent.VK_ASTERISK],
+                '^': [KeyEvent.VK_SHIFT, KeyEvent.VK_CIRCUMFLEX],
+                '&': [KeyEvent.VK_SHIFT, KeyEvent.VK_AMPERSAND],
+                '*': [KeyEvent.VK_SHIFT, KeyEvent.VK_ASTERISK],
                 '(': [KeyEvent.VK_LEFT_PARENTHESIS],
                 ')': [KeyEvent.VK_RIGHT_PARENTHESIS],
-                '_': [KeyEvent.VK_UNDERSCORE],
+                '_': [KeyEvent.VK_SHIFT, KeyEvent.VK_UNDERSCORE],
                 '+': [KeyEvent.VK_PLUS],
                 '\t': [KeyEvent.VK_TAB],
                 '\n': [KeyEvent.VK_ENTER],
                 '[': [KeyEvent.VK_OPEN_BRACKET],
                 ']': [KeyEvent.VK_CLOSE_BRACKET],
                 '\\': [KeyEvent.VK_BACK_SLASH],
                 '{': [KeyEvent.VK_SHIFT, KeyEvent.VK_OPEN_BRACKET],
                 '}': [KeyEvent.VK_SHIFT, KeyEvent.VK_CLOSE_BRACKET],
                 '|': [KeyEvent.VK_SHIFT, KeyEvent.VK_BACK_SLASH],
                 ';': [KeyEvent.VK_SEMICOLON],
                 ':': [KeyEvent.VK_COLON],
                 '\'': [KeyEvent.VK_QUOTE],
-                '"': [KeyEvent.VK_QUOTEDBL],
+                '"': [KeyEvent.VK_SHIFT, KeyEvent.VK_QUOTEDBL],
                 ',': [KeyEvent.VK_COMMA],
                 '<': [KeyEvent.VK_SHIFT, KeyEvent.VK_COMMA],
                 '.': [KeyEvent.VK_PERIOD],
                 '>': [KeyEvent.VK_SHIFT, KeyEvent.VK_PERIOD],
                 '/': [KeyEvent.VK_SLASH],
                 '?': [KeyEvent.VK_SHIFT, KeyEvent.VK_SLASH],
                 ' ': [KeyEvent.VK_SPACE],
```

### Comparing `pyjt-0.2.0/pyjt/__init__.py` & `pyjt-0.2.1/pyjt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     """ Start the pyjt JVM.
 
         Needs to be called before using pyjt.
 
         :param classpath:   If set, use this classpath for the JVM, otherwise
                             use CLASSPATH environment variable.
     """
-    jpype.startJVM(jpype.getDefaultJVMPath(), f"-Djava.class.path={os.environ.get('CLASSPATH', '')}")
+    cp = os.environ.get('CLASSPATH', '') if classpath is None else classpath
+    jpype.startJVM(jpype.getDefaultJVMPath(), f"-Djava.class.path={cp}")
 
 def stop():
     jpype.shutdownJVM()
 
 
 
 def run(app, args=[""]):
```

### Comparing `pyjt-0.2.0/pyjt.egg-info/PKG-INFO` & `pyjt-0.2.1/pyjt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.2.0
+Version: 0.2.1
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyjt-0.2.0/pyproject.toml` & `pyjt-0.2.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyjt"
-version = "0.2.0"
+version = "0.2.1"
 description="test automation for java UI applications from python"
 authors = [
     { name="Claudio Klingler", email="ck@realtime-projects.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.7"
```

