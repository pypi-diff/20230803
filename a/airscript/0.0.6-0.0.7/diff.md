# Comparing `tmp/airscript-0.0.6.tar.gz` & `tmp/airscript-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airscript-0.0.6.tar", last modified: Wed Aug  2 04:26:44 2023, max compression
+gzip compressed data, was "airscript-0.0.7.tar", last modified: Thu Aug  3 00:41:38 2023, max compression
```

## Comparing `airscript-0.0.6.tar` & `airscript-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.995959 airscript-0.0.6/
--rw-rw-rw-   0        0        0      493 2023-08-02 04:26:43.993954 airscript-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       66 2023-08-02 04:15:18.000000 airscript-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.961944 airscript-0.0.6/airscript/
--rw-rw-rw-   0        0        0      138 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.976944 airscript-0.0.6/airscript/action/
--rw-rw-rw-   0        0        0      798 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/action/__init__.py
--rw-rw-rw-   0        0        0      258 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/action/gesture.py
--rw-rw-rw-   0        0        0     1376 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/action/key.py
--rw-rw-rw-   0        0        0     1272 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/action/path.py
--rw-rw-rw-   0        0        0      165 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/action/touch.py
--rw-rw-rw-   0        0        0      195 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/data.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.978953 airscript-0.0.6/airscript/graphics/
--rw-rw-rw-   0        0        0       85 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/graphics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.980946 airscript-0.0.6/airscript/intent/
--rw-rw-rw-   0        0        0      111 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/intent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.982944 airscript-0.0.6/airscript/node/
--rw-rw-rw-   0        0        0     4575 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/node/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.983944 airscript-0.0.6/airscript/screen/
--rw-rw-rw-   0        0        0     3960 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/screen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.984947 airscript-0.0.6/airscript/system/
--rw-rw-rw-   0        0        0      716 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.989953 airscript-0.0.6/airscript/ui/
--rw-rw-rw-   0        0        0      631 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/ui/__init__.py
--rw-rw-rw-   0        0        0      961 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/ui/dialog.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.968945 airscript-0.0.6/airscript.egg-info/
--rw-rw-rw-   0        0        0      493 2023-08-02 04:26:43.000000 airscript-0.0.6/airscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-08-02 04:26:43.000000 airscript-0.0.6/airscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 04:26:43.000000 airscript-0.0.6/airscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-02 04:26:43.000000 airscript-0.0.6/airscript.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 04:26:43.995959 airscript-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      690 2023-08-02 04:25:19.000000 airscript-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.263773 airscript-0.0.7/
+-rw-rw-rw-   0        0        0      493 2023-08-03 00:41:38.262769 airscript-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2023-08-02 04:15:18.000000 airscript-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.223721 airscript-0.0.7/airscript/
+-rw-rw-rw-   0        0        0       44 2023-08-03 00:39:12.000000 airscript-0.0.7/airscript/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.242754 airscript-0.0.7/airscript/action/
+-rw-rw-rw-   0        0        0      798 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/action/__init__.py
+-rw-rw-rw-   0        0        0      258 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/action/gesture.py
+-rw-rw-rw-   0        0        0     1376 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/action/key.py
+-rw-rw-rw-   0        0        0     1272 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/action/path.py
+-rw-rw-rw-   0        0        0      165 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/action/touch.py
+-rw-rw-rw-   0        0        0      195 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/data.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.244752 airscript-0.0.7/airscript/graphics/
+-rw-rw-rw-   0        0        0       85 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/graphics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.247243 airscript-0.0.7/airscript/intent/
+-rw-rw-rw-   0        0        0      480 2023-08-03 00:39:12.000000 airscript-0.0.7/airscript/intent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.249252 airscript-0.0.7/airscript/node/
+-rw-rw-rw-   0        0        0     4575 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/node/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.250252 airscript-0.0.7/airscript/screen/
+-rw-rw-rw-   0        0        0     3960 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/screen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.254251 airscript-0.0.7/airscript/system/
+-rw-rw-rw-   0        0        0      161 2023-08-03 00:39:12.000000 airscript-0.0.7/airscript/system/Prgogress.py
+-rw-rw-rw-   0        0        0     2457 2023-08-03 00:39:12.000000 airscript-0.0.7/airscript/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.260769 airscript-0.0.7/airscript/ui/
+-rw-rw-rw-   0        0        0     1056 2023-08-03 00:39:12.000000 airscript-0.0.7/airscript/ui/__init__.py
+-rw-rw-rw-   0        0        0     1134 2023-08-03 00:39:12.000000 airscript-0.0.7/airscript/ui/dialog.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.233236 airscript-0.0.7/airscript.egg-info/
+-rw-rw-rw-   0        0        0      493 2023-08-03 00:41:38.000000 airscript-0.0.7/airscript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2023-08-03 00:41:38.000000 airscript-0.0.7/airscript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 00:41:38.000000 airscript-0.0.7/airscript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-03 00:41:38.000000 airscript-0.0.7/airscript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 00:41:38.263773 airscript-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      690 2023-08-03 00:41:29.000000 airscript-0.0.7/setup.py
```

### Comparing `airscript-0.0.6/airscript/action/__init__.py` & `airscript-0.0.7/airscript/action/__init__.py`

 * *Files identical despite different names*

### Comparing `airscript-0.0.6/airscript/action/key.py` & `airscript-0.0.7/airscript/action/key.py`

 * *Files identical despite different names*

### Comparing `airscript-0.0.6/airscript/action/path.py` & `airscript-0.0.7/airscript/action/path.py`

 * *Files identical despite different names*

### Comparing `airscript-0.0.6/airscript/node/__init__.py` & `airscript-0.0.7/airscript/node/__init__.py`

 * *Files identical despite different names*

### Comparing `airscript-0.0.6/airscript/screen/__init__.py` & `airscript-0.0.7/airscript/screen/__init__.py`

 * *Files identical despite different names*

### Comparing `airscript-0.0.6/airscript/system/__init__.py` & `airscript-0.0.7/airscript/ui/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,60 @@
-from typing import Any
+from typing import Any, Union
 
 
-class R:
-    def __init__(self, path: str) -> None:
+class Window:
+    def __init__(self, layout: str, tunnel: Any = None):
         pass
 
-    def sd(self, childpath: str) -> str:
+    def model(self, model: int):
         pass
 
-    def context(self) -> str:
+    def width(self, size: Union[int, str]):
         pass
 
-    def root(self, childpath: str) -> str:
+    def height(self, size: Union[int, str]):
         pass
 
-    def res(self, childpath: str) -> str:
+    def background(self, bgcolor: str):
         pass
 
-class Device:
+    def drag(self, isDrag: bool):
+        pass
 
-    def display(self) -> Any:
+    def dimAmount(self, dim: float):
+        """
+        数值在 0-1之间
+        0 :完全没有遮罩,1:完全黑的遮罩,0.5:半透明遮罩,默认为0.5
+        """
         pass
 
+    def gravity(self, g: int):
+        """
+        居中位置（引力） 该方法会影响 x，y 函数 的相对位置
+        """
+        pass
 
-    def name(self) -> str:
+    def x(self, x: int):
         pass
 
-    def brand(self) -> str:
+    def y(self, y: int):
         pass
 
-    def model(self) -> str:
+    def show(self):
         pass
 
-    def sdk(self) -> str:
+    def close(self):
         pass
 
-    def version(self) -> str:
+    def call(self, func: Any):
         pass
 
 
-    def ip(self) -> str:
+class Float:
+    def hide(self):
         pass
 
-    def currentAppInfo(self) -> Any:
+    def show(self):
         pass
 
 
 
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `airscript-0.0.6/airscript/ui/dialog.py` & `airscript-0.0.7/airscript/ui/dialog.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any
 
 
-def toast(msg: str, duration: int = 2, x=-1, y=-1) -> None:
+def toast(msg: str, duration: int = 3, x=-1, y=-1) -> None:
     pass
 
 
 def alert(msg: str, submit: str) -> None:
     pass
 
 
@@ -47,13 +47,20 @@
 
     def cancel(self, msg: str) -> 'promat':
         pass
 
     def close(self):
         pass
 
-    def show(self, pyfun: Any):
+    def show(self, pyfun: Any = None):
         pass
 
 
+class loger:
+    def __init__(self):
+        pass
 
+    def show(self, pyfun: Any = None):
+        pass
 
+    def title(self, title: str) -> 'loger':
+        pass
```

### Comparing `airscript-0.0.6/airscript.egg-info/SOURCES.txt` & `airscript-0.0.7/airscript.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 airscript/action/key.py
 airscript/action/path.py
 airscript/action/touch.py
 airscript/graphics/__init__.py
 airscript/intent/__init__.py
 airscript/node/__init__.py
 airscript/screen/__init__.py
+airscript/system/Prgogress.py
 airscript/system/__init__.py
 airscript/ui/__init__.py
 airscript/ui/dialog.py
```

### Comparing `airscript-0.0.6/setup.py` & `airscript-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'airscript 类型提示语言包'
 
 setup(
     name="airscript",
     version=VERSION,
     author="ITisl",
     author_email="aojoy@163.com",
```

