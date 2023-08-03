# Comparing `tmp/tuyau-1.1.tar.gz` & `tmp/tuyau-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuyau-1.1.tar", last modified: Wed Aug  2 16:32:08 2023, max compression
+gzip compressed data, was "tuyau-1.2.tar", last modified: Thu Aug  3 15:44:09 2023, max compression
```

## Comparing `tuyau-1.1.tar` & `tuyau-1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 guiforge  (1000) guiforge  (1000)        0 2023-08-02 16:32:08.540334 tuyau-1.1/
--rw-rw-r--   0 guiforge  (1000) guiforge  (1000)     1073 2023-07-31 22:59:08.000000 tuyau-1.1/LICENSE
--rw-rw-r--   0 guiforge  (1000) guiforge  (1000)     4048 2023-08-02 16:32:08.540334 tuyau-1.1/PKG-INFO
--rw-rw-r--   0 guiforge  (1000) guiforge  (1000)     2164 2023-08-02 16:28:20.000000 tuyau-1.1/Readme.md
--rw-rw-r--   0 guiforge  (1000) guiforge  (1000)     1749 2023-08-02 16:28:20.000000 tuyau-1.1/pyproject.toml
--rw-rw-r--   0 guiforge  (1000) guiforge  (1000)       38 2023-08-02 16:32:08.540334 tuyau-1.1/setup.cfg
-drwxrwxr-x   0 guiforge  (1000) guiforge  (1000)        0 2023-08-02 16:32:08.540334 tuyau-1.1/tests/
--rw-rw-r--   0 guiforge  (1000) guiforge  (1000)      708 2023-08-02 15:36:13.000000 tuyau-1.1/tests/test_tube.py
-drwxrwxr-x   0 guiforge  (1000) guiforge  (1000)        0 2023-08-02 16:32:08.540334 tuyau-1.1/tuyau/
--rw-rw-r--   0 guiforge  (1000) guiforge  (1000)     1234 2023-08-02 16:28:20.000000 tuyau-1.1/tuyau/__init__.py
-drwxrwxr-x   0 guiforge  (1000) guiforge  (1000)        0 2023-08-02 16:32:08.540334 tuyau-1.1/tuyau.egg-info/
--rw-rw-r--   0 guiforge  (1000) guiforge  (1000)     4048 2023-08-02 16:32:08.000000 tuyau-1.1/tuyau.egg-info/PKG-INFO
--rw-rw-r--   0 guiforge  (1000) guiforge  (1000)      185 2023-08-02 16:32:08.000000 tuyau-1.1/tuyau.egg-info/SOURCES.txt
--rw-rw-r--   0 guiforge  (1000) guiforge  (1000)        1 2023-08-02 16:32:08.000000 tuyau-1.1/tuyau.egg-info/dependency_links.txt
--rw-rw-r--   0 guiforge  (1000) guiforge  (1000)        6 2023-08-02 16:32:08.000000 tuyau-1.1/tuyau.egg-info/top_level.txt
+drwxrwxr-x   0 guiforge  (1000) guiforge  (1000)        0 2023-08-03 15:44:09.554350 tuyau-1.2/
+-rw-rw-r--   0 guiforge  (1000) guiforge  (1000)     1073 2023-07-31 22:59:08.000000 tuyau-1.2/LICENSE
+-rw-rw-r--   0 guiforge  (1000) guiforge  (1000)     4603 2023-08-03 15:44:09.554350 tuyau-1.2/PKG-INFO
+-rw-rw-r--   0 guiforge  (1000) guiforge  (1000)     2719 2023-08-03 15:42:51.000000 tuyau-1.2/Readme.md
+-rw-rw-r--   0 guiforge  (1000) guiforge  (1000)     1749 2023-08-03 15:42:51.000000 tuyau-1.2/pyproject.toml
+-rw-rw-r--   0 guiforge  (1000) guiforge  (1000)       38 2023-08-03 15:44:09.554350 tuyau-1.2/setup.cfg
+drwxrwxr-x   0 guiforge  (1000) guiforge  (1000)        0 2023-08-03 15:44:09.554350 tuyau-1.2/tests/
+-rw-rw-r--   0 guiforge  (1000) guiforge  (1000)      919 2023-08-03 15:43:25.000000 tuyau-1.2/tests/test_tube.py
+drwxrwxr-x   0 guiforge  (1000) guiforge  (1000)        0 2023-08-03 15:44:09.554350 tuyau-1.2/tuyau/
+-rw-rw-r--   0 guiforge  (1000) guiforge  (1000)      111 2023-08-03 15:42:51.000000 tuyau-1.2/tuyau/__init__.py
+-rw-rw-r--   0 guiforge  (1000) guiforge  (1000)     1213 2023-08-03 15:28:50.000000 tuyau-1.2/tuyau/tube.py
+drwxrwxr-x   0 guiforge  (1000) guiforge  (1000)        0 2023-08-03 15:44:09.554350 tuyau-1.2/tuyau.egg-info/
+-rw-rw-r--   0 guiforge  (1000) guiforge  (1000)     4603 2023-08-03 15:44:09.000000 tuyau-1.2/tuyau.egg-info/PKG-INFO
+-rw-rw-r--   0 guiforge  (1000) guiforge  (1000)      199 2023-08-03 15:44:09.000000 tuyau-1.2/tuyau.egg-info/SOURCES.txt
+-rw-rw-r--   0 guiforge  (1000) guiforge  (1000)        1 2023-08-03 15:44:09.000000 tuyau-1.2/tuyau.egg-info/dependency_links.txt
+-rw-rw-r--   0 guiforge  (1000) guiforge  (1000)        6 2023-08-03 15:44:09.000000 tuyau-1.2/tuyau.egg-info/top_level.txt
```

### Comparing `tuyau-1.1/LICENSE` & `tuyau-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tuyau-1.1/PKG-INFO` & `tuyau-1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuyau
-Version: 1.1
+Version: 1.2
 Summary: Tuyau is a library that allows you to process values through a sequence of steps, similar to a pipe.
 Author-email: Guillaume Pouyat <guillaume.pouyat@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Guillaume Pouyat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tuyau
 
-[![Version](https://img.shields.io/badge/version-1.1-blue.svg)](https://github.com/guiforge/tuyau)
+[![Version](https://img.shields.io/badge/version-1.2-blue.svg)](https://github.com/guiforge/tuyau)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 Tuyau is a library that allows you to process values through a sequence of steps, similar to a pipe.
 
 ```python
 # Before 
 for name in names:
@@ -109,14 +109,36 @@
 
 ```python
 tube = Tube(lambda x: x + 1, lambda x: x * 2)
 
 result = tube(3)
 print(result)  # Output: 8 (3 + 1 = 4, 4 * 2 = 8)
 ```
+## Typing
+## Typing
+
+The `Tube` class is designed to support typing for both input and output. 
+
+```python
+from tuyau import Tube
+
+def add_one(num: int) -> int:
+    return num + 1
+
+def multiply_by_two(num: int) -> int:
+    return num * 2
+
+# Create Tube with multiple callables that take and return int
+tube: Tube[int, int] = Tube(add_one, multiply_by_two)
+tube: Tube[int, str] = Tube(add_one, multiply_by_two, str)
+
+# Process integers through the tubes
+result: int = tube(3)# Output: 6 (3 + 1 * 2) 
+result2: str = tube(3)# Output: "6" str(3 + 1 * 2) 
+```
 
 ## Contributing
 
 Contributions are welcome! If you find a bug or have a suggestion for improvement, please create an issue or a pull request on [GitHub](https://github.com/guiforge/tuyau).
 
 ### Local dev
 install .venv with all dev dep
```

### Comparing `tuyau-1.1/Readme.md` & `tuyau-1.2/Readme.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Tuyau
 
-[![Version](https://img.shields.io/badge/version-1.1-blue.svg)](https://github.com/guiforge/tuyau)
+[![Version](https://img.shields.io/badge/version-1.2-blue.svg)](https://github.com/guiforge/tuyau)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 Tuyau is a library that allows you to process values through a sequence of steps, similar to a pipe.
 
 ```python
 # Before 
 for name in names:
@@ -71,14 +71,36 @@
 
 ```python
 tube = Tube(lambda x: x + 1, lambda x: x * 2)
 
 result = tube(3)
 print(result)  # Output: 8 (3 + 1 = 4, 4 * 2 = 8)
 ```
+## Typing
+## Typing
+
+The `Tube` class is designed to support typing for both input and output. 
+
+```python
+from tuyau import Tube
+
+def add_one(num: int) -> int:
+    return num + 1
+
+def multiply_by_two(num: int) -> int:
+    return num * 2
+
+# Create Tube with multiple callables that take and return int
+tube: Tube[int, int] = Tube(add_one, multiply_by_two)
+tube: Tube[int, str] = Tube(add_one, multiply_by_two, str)
+
+# Process integers through the tubes
+result: int = tube(3)# Output: 6 (3 + 1 * 2) 
+result2: str = tube(3)# Output: "6" str(3 + 1 * 2) 
+```
 
 ## Contributing
 
 Contributions are welcome! If you find a bug or have a suggestion for improvement, please create an issue or a pull request on [GitHub](https://github.com/guiforge/tuyau).
 
 ### Local dev
 install .venv with all dev dep
```

### Comparing `tuyau-1.1/pyproject.toml` & `tuyau-1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tuyau"
-version = "1.1"
+version = "1.2"
 dependencies = []
 description = "Tuyau is a library that allows you to process values through a sequence of steps, similar to a pipe."
 authors = [{name = "Guillaume Pouyat", email="guillaume.pouyat@protonmail.com"}]
 license = { file = "LICENSE" }
 readme = "Readme.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `tuyau-1.1/tests/test_tube.py` & `tuyau-1.2/tests/test_tube.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,27 +5,32 @@
 
 
 def add_one(number: int) -> int:
     """Simple steps, add one to number."""
     return number + 1
 
 
+def test_simple_return() -> None:
+    """Test sending values through the Tuyau. and get result."""
+    _number = 42
+    assert Tube(str, int)(_number) == _number  # noqa: S101
+
+
 def test_simple_send() -> None:
     """Test sending values through the Tuyau. with .send."""
     _ret: list[int] = []
-
-    tuyau = Tube(*[add_one] * 100, lambda v: _ret.append(v))
+    tuyau: Tube[int, None] = Tube(*[add_one] * 100, lambda v: _ret.append(v))
     for i in range(1, 4):
         tuyau.send(i)
 
     assert _ret == [101, 102, 103]  # noqa: S101
 
 
 def test_simple_call() -> None:
     """Test calling the Tuyau directly with values. call directly."""
     _ret: list[int] = []
 
-    tuyau = Tube(*[add_one] * 100, lambda v: _ret.append(v))
+    tuyau: Tube[int, None] = Tube(*[add_one] * 100, lambda v: _ret.append(v))
     for i in range(1, 4):
         tuyau(i)
 
     assert _ret == [101, 102, 103]  # noqa: S101
```

### Comparing `tuyau-1.1/tuyau/__init__.py` & `tuyau-1.2/tuyau/tube.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Library allowing using tuyau like pipe."""
 
-__version__ = "1.1"
-
 from collections.abc import Callable
 from typing import Any
 
 
 class Tube:
     """A tuyau that processes values through a sequence of steps."""
```

### Comparing `tuyau-1.1/tuyau.egg-info/PKG-INFO` & `tuyau-1.2/tuyau.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuyau
-Version: 1.1
+Version: 1.2
 Summary: Tuyau is a library that allows you to process values through a sequence of steps, similar to a pipe.
 Author-email: Guillaume Pouyat <guillaume.pouyat@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Guillaume Pouyat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tuyau
 
-[![Version](https://img.shields.io/badge/version-1.1-blue.svg)](https://github.com/guiforge/tuyau)
+[![Version](https://img.shields.io/badge/version-1.2-blue.svg)](https://github.com/guiforge/tuyau)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 Tuyau is a library that allows you to process values through a sequence of steps, similar to a pipe.
 
 ```python
 # Before 
 for name in names:
@@ -109,14 +109,36 @@
 
 ```python
 tube = Tube(lambda x: x + 1, lambda x: x * 2)
 
 result = tube(3)
 print(result)  # Output: 8 (3 + 1 = 4, 4 * 2 = 8)
 ```
+## Typing
+## Typing
+
+The `Tube` class is designed to support typing for both input and output. 
+
+```python
+from tuyau import Tube
+
+def add_one(num: int) -> int:
+    return num + 1
+
+def multiply_by_two(num: int) -> int:
+    return num * 2
+
+# Create Tube with multiple callables that take and return int
+tube: Tube[int, int] = Tube(add_one, multiply_by_two)
+tube: Tube[int, str] = Tube(add_one, multiply_by_two, str)
+
+# Process integers through the tubes
+result: int = tube(3)# Output: 6 (3 + 1 * 2) 
+result2: str = tube(3)# Output: "6" str(3 + 1 * 2) 
+```
 
 ## Contributing
 
 Contributions are welcome! If you find a bug or have a suggestion for improvement, please create an issue or a pull request on [GitHub](https://github.com/guiforge/tuyau).
 
 ### Local dev
 install .venv with all dev dep
```

