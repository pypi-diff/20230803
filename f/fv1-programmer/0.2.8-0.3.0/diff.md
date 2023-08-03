# Comparing `tmp/fv1_programmer-0.2.8.tar.gz` & `tmp/fv1_programmer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fv1_programmer-0.2.8.tar", max compression
+gzip compressed data, was "fv1_programmer-0.3.0.tar", max compression
```

## Comparing `fv1_programmer-0.2.8.tar` & `fv1_programmer-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1065 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/LICENSE
--rw-r--r--   0        0        0      613 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/README.md
--rw-r--r--   0        0        0     1140 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/adaptor/adapter.py
--rw-r--r--   0        0        0     1083 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/adaptor/mcp2221.py
--rw-r--r--   0        0        0       30 2023-08-01 20:49:20.371855 fv1_programmer-0.2.8/asfv1/.git
--rw-r--r--   0        0        0     1157 2023-08-01 20:49:21.771947 fv1_programmer-0.2.8/asfv1/.gitignore
--rw-r--r--   0        0        0     1075 2023-08-01 20:49:21.771947 fv1_programmer-0.2.8/asfv1/LICENSE
--rw-r--r--   0        0        0    36334 2023-08-01 20:49:21.771947 fv1_programmer-0.2.8/asfv1/README.md
--rw-r--r--   0        0        0    54482 2023-08-01 20:49:21.771947 fv1_programmer-0.2.8/asfv1/asfv1.py
--rw-r--r--   0        0        0      561 2023-08-01 20:49:21.771947 fv1_programmer-0.2.8/asfv1/example.asm
--rw-r--r--   0        0        0      801 2023-08-01 20:49:21.771947 fv1_programmer-0.2.8/asfv1/setup.py
--rw-r--r--   0        0        0       31 2023-08-01 20:49:20.959894 fv1_programmer-0.2.8/disfv1/.git
--rw-r--r--   0        0        0     1157 2023-08-01 20:49:21.775947 fv1_programmer-0.2.8/disfv1/.gitignore
--rw-r--r--   0        0        0     1075 2023-08-01 20:49:21.775947 fv1_programmer-0.2.8/disfv1/LICENSE
--rw-r--r--   0        0        0     4816 2023-08-01 20:49:21.775947 fv1_programmer-0.2.8/disfv1/README.md
--rw-r--r--   0        0        0    17532 2023-08-01 20:49:21.775947 fv1_programmer-0.2.8/disfv1/disfv1.py
--rw-r--r--   0        0        0      512 2023-08-01 20:49:21.775947 fv1_programmer-0.2.8/disfv1/example.bin
--rw-r--r--   0        0        0      798 2023-08-01 20:49:21.775947 fv1_programmer-0.2.8/disfv1/setup.py
--rw-r--r--   0        0        0     6747 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/eeprom/eeprom.py
--rw-r--r--   0        0        0     1717 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/fv1_programmer/fv1.py
--rw-r--r--   0        0        0     3081 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/fv1_programmer/main.py
--rw-r--r--   0        0        0     3160 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/fv1_programmer/tui.css
--rw-r--r--   0        0        0    22380 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/fv1_programmer/tui.py
--rw-r--r--   0        0        0     1267 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 fv1_programmer-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-03 17:31:32.020557 fv1_programmer-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1409 2023-08-03 17:31:32.020557 fv1_programmer-0.3.0/README.md
+-rw-r--r--   0        0        0     1140 2023-08-03 17:31:32.020557 fv1_programmer-0.3.0/adaptor/adapter.py
+-rw-r--r--   0        0        0     1083 2023-08-03 17:31:32.020557 fv1_programmer-0.3.0/adaptor/mcp2221.py
+-rw-r--r--   0        0        0       30 2023-08-03 17:31:32.468561 fv1_programmer-0.3.0/asfv1/.git
+-rw-r--r--   0        0        0     1157 2023-08-03 17:31:33.484569 fv1_programmer-0.3.0/asfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2023-08-03 17:31:33.484569 fv1_programmer-0.3.0/asfv1/LICENSE
+-rw-r--r--   0        0        0    36334 2023-08-03 17:31:33.484569 fv1_programmer-0.3.0/asfv1/README.md
+-rw-r--r--   0        0        0    54482 2023-08-03 17:31:33.488569 fv1_programmer-0.3.0/asfv1/asfv1.py
+-rw-r--r--   0        0        0      561 2023-08-03 17:31:33.488569 fv1_programmer-0.3.0/asfv1/example.asm
+-rw-r--r--   0        0        0      801 2023-08-03 17:31:33.488569 fv1_programmer-0.3.0/asfv1/setup.py
+-rw-r--r--   0        0        0       31 2023-08-03 17:31:32.784563 fv1_programmer-0.3.0/disfv1/.git
+-rw-r--r--   0        0        0     1157 2023-08-03 17:31:33.492569 fv1_programmer-0.3.0/disfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2023-08-03 17:31:33.492569 fv1_programmer-0.3.0/disfv1/LICENSE
+-rw-r--r--   0        0        0     4816 2023-08-03 17:31:33.492569 fv1_programmer-0.3.0/disfv1/README.md
+-rw-r--r--   0        0        0    17532 2023-08-03 17:31:33.492569 fv1_programmer-0.3.0/disfv1/disfv1.py
+-rw-r--r--   0        0        0      512 2023-08-03 17:31:33.492569 fv1_programmer-0.3.0/disfv1/example.bin
+-rw-r--r--   0        0        0      798 2023-08-03 17:31:33.492569 fv1_programmer-0.3.0/disfv1/setup.py
+-rw-r--r--   0        0        0     6747 2023-08-03 17:31:32.020557 fv1_programmer-0.3.0/eeprom/eeprom.py
+-rw-r--r--   0        0        0     1717 2023-08-03 17:31:32.020557 fv1_programmer-0.3.0/fv1_programmer/fv1.py
+-rw-r--r--   0        0        0     3081 2023-08-03 17:31:32.020557 fv1_programmer-0.3.0/fv1_programmer/main.py
+-rw-r--r--   0        0        0     3160 2023-08-03 17:31:32.020557 fv1_programmer-0.3.0/fv1_programmer/tui.css
+-rw-r--r--   0        0        0    22346 2023-08-03 17:31:32.020557 fv1_programmer-0.3.0/fv1_programmer/tui.py
+-rw-r--r--   0        0        0     1323 2023-08-03 17:31:32.020557 fv1_programmer-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 fv1_programmer-0.3.0/PKG-INFO
```

### Comparing `fv1_programmer-0.2.8/LICENSE` & `fv1_programmer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/adaptor/adapter.py` & `fv1_programmer-0.3.0/adaptor/adapter.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/adaptor/mcp2221.py` & `fv1_programmer-0.3.0/adaptor/mcp2221.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/asfv1/.gitignore` & `fv1_programmer-0.3.0/asfv1/.gitignore`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/asfv1/LICENSE` & `fv1_programmer-0.3.0/asfv1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/asfv1/README.md` & `fv1_programmer-0.3.0/asfv1/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/asfv1/asfv1.py` & `fv1_programmer-0.3.0/asfv1/asfv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/asfv1/example.asm` & `fv1_programmer-0.3.0/asfv1/example.asm`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/asfv1/setup.py` & `fv1_programmer-0.3.0/asfv1/setup.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/disfv1/.gitignore` & `fv1_programmer-0.3.0/disfv1/.gitignore`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/disfv1/LICENSE` & `fv1_programmer-0.3.0/disfv1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/disfv1/README.md` & `fv1_programmer-0.3.0/disfv1/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/disfv1/disfv1.py` & `fv1_programmer-0.3.0/disfv1/disfv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/disfv1/setup.py` & `fv1_programmer-0.3.0/disfv1/setup.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/eeprom/eeprom.py` & `fv1_programmer-0.3.0/eeprom/eeprom.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/fv1_programmer/fv1.py` & `fv1_programmer-0.3.0/fv1_programmer/fv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/fv1_programmer/main.py` & `fv1_programmer-0.3.0/fv1_programmer/main.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/fv1_programmer/tui.css` & `fv1_programmer-0.3.0/fv1_programmer/tui.css`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.8/fv1_programmer/tui.py` & `fv1_programmer-0.3.0/fv1_programmer/tui.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 from typing import Iterable
 from pathlib import Path
 from fv1_programmer.fv1 import FV1Program, FV1_PROGRAM_MAX_BYTES
 import pyperclip
 
 
-__version__ = "0.2.8"
+__version__ = "0.3.0"
 
 _title = "FV1 Programmer"
 
 class BusyScreen(ModalScreen):
     def __init__(self, message : str) -> None:
         self.message = message
         super().__init__()
@@ -569,9 +569,8 @@
     def do_exit(self, result = None) -> None:
         super().exit(result)
 
     def on_mount(self) -> None:
         self.push_screen("main")
 
     def show_toast(self, message, title=None, severity="information", timeout=4.0) -> None:
-        self.logger.info(message)
         self.notify(message, title=title, severity=severity, timeout=timeout)
```

### Comparing `fv1_programmer-0.2.8/pyproject.toml` & `fv1_programmer-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [tool.poetry]
 name = "fv1-programmer"
-version = "0.2.8"
+version = "0.3.0"
+homepage = "https://github.com/audiofab/fv1_programmer"
 description = "An EEPROM programming tool for the FV-1 DSP"
 authors = ["Mark Melvin <mark.melvin@audiofab.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

