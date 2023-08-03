# Comparing `tmp/airscript-0.0.7.tar.gz` & `tmp/airscript-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airscript-0.0.7.tar", last modified: Thu Aug  3 00:41:38 2023, max compression
+gzip compressed data, was "airscript-0.0.8.tar", last modified: Thu Aug  3 01:45:13 2023, max compression
```

## Comparing `airscript-0.0.7.tar` & `airscript-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.263773 airscript-0.0.7/
--rw-rw-rw-   0        0        0      493 2023-08-03 00:41:38.262769 airscript-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       66 2023-08-02 04:15:18.000000 airscript-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.223721 airscript-0.0.7/airscript/
--rw-rw-rw-   0        0        0       44 2023-08-03 00:39:12.000000 airscript-0.0.7/airscript/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.242754 airscript-0.0.7/airscript/action/
--rw-rw-rw-   0        0        0      798 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/action/__init__.py
--rw-rw-rw-   0        0        0      258 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/action/gesture.py
--rw-rw-rw-   0        0        0     1376 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/action/key.py
--rw-rw-rw-   0        0        0     1272 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/action/path.py
--rw-rw-rw-   0        0        0      165 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/action/touch.py
--rw-rw-rw-   0        0        0      195 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/data.py
-drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.244752 airscript-0.0.7/airscript/graphics/
--rw-rw-rw-   0        0        0       85 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/graphics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.247243 airscript-0.0.7/airscript/intent/
--rw-rw-rw-   0        0        0      480 2023-08-03 00:39:12.000000 airscript-0.0.7/airscript/intent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.249252 airscript-0.0.7/airscript/node/
--rw-rw-rw-   0        0        0     4575 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/node/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.250252 airscript-0.0.7/airscript/screen/
--rw-rw-rw-   0        0        0     3960 2023-08-02 04:15:18.000000 airscript-0.0.7/airscript/screen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.254251 airscript-0.0.7/airscript/system/
--rw-rw-rw-   0        0        0      161 2023-08-03 00:39:12.000000 airscript-0.0.7/airscript/system/Prgogress.py
--rw-rw-rw-   0        0        0     2457 2023-08-03 00:39:12.000000 airscript-0.0.7/airscript/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.260769 airscript-0.0.7/airscript/ui/
--rw-rw-rw-   0        0        0     1056 2023-08-03 00:39:12.000000 airscript-0.0.7/airscript/ui/__init__.py
--rw-rw-rw-   0        0        0     1134 2023-08-03 00:39:12.000000 airscript-0.0.7/airscript/ui/dialog.py
-drwxrwxrwx   0        0        0        0 2023-08-03 00:41:38.233236 airscript-0.0.7/airscript.egg-info/
--rw-rw-rw-   0        0        0      493 2023-08-03 00:41:38.000000 airscript-0.0.7/airscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-08-03 00:41:38.000000 airscript-0.0.7/airscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 00:41:38.000000 airscript-0.0.7/airscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-03 00:41:38.000000 airscript-0.0.7/airscript.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 00:41:38.263773 airscript-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      690 2023-08-03 00:41:29.000000 airscript-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:45:13.261221 airscript-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-03 01:45:13.261221 airscript-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-03 01:45:03.000000 airscript-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:45:13.257221 airscript-0.0.8/airscript/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:45:13.261221 airscript-0.0.8/airscript/action/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/action/gesture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/action/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/action/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/action/touch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:45:13.261221 airscript-0.0.8/airscript/graphics/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/graphics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:45:13.261221 airscript-0.0.8/airscript/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/intent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:45:13.261221 airscript-0.0.8/airscript/node/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/node/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:45:13.261221 airscript-0.0.8/airscript/screen/
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/screen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:45:13.261221 airscript-0.0.8/airscript/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/system/Prgogress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:45:13.261221 airscript-0.0.8/airscript/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-03 01:45:03.000000 airscript-0.0.8/airscript/ui/dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:45:13.257221 airscript-0.0.8/airscript.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-03 01:45:13.000000 airscript-0.0.8/airscript.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-03 01:45:13.000000 airscript-0.0.8/airscript.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:45:13.000000 airscript-0.0.8/airscript.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 01:45:13.000000 airscript-0.0.8/airscript.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 01:45:13.261221 airscript-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-03 01:45:03.000000 airscript-0.0.8/setup.py
```

### Comparing `airscript-0.0.7/airscript/action/path.py` & `airscript-0.0.8/airscript/action/path.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# 手势-创建路径
-from typing import Self
-
-
-class path:
-    def __init__(self, startTime=0, duration=20, willContinue=False):
-        """
-        创建一个新的路径对象
-
-        参数:
-        - startTime (number): 延迟多久开始绘制路径，单位ms，默认为0
-        - duration (number): 路径绘制的时长，单位ms，默认为20
-        - willContinue (boolean): 在路径结束后，手指是否抬起，默认为False
-        """
-
-    def moveTo(self, x:int, y:int) -> None:
-        """
-        移动初始点到指定位置
-
-        参数:
-        - x (number): X轴坐标
-        - y (number): Y轴坐标
-        """
-        pass
-
-    def lineTo(self, x: int, y: int)-> None:
-        """
-        画直线到指定位置
-
-        参数:
-        - x (number): X轴坐标
-        - y (number): Y轴坐标
-        """
-        pass
-
-    def quadTo(self, x1: int, y1:int, x2:int, y2:int)-> None:
-        """
-        使用二次贝塞尔曲线绘制路径
-
-        参数:
-        - x1 (number): 控制点1的X轴坐标
-        - y1 (number): 控制点1的Y轴坐标
-        - x2 (number): 控制点2的X轴坐标
-        - y2 (number): 控制点2的Y轴坐标
-        """
-        pass
-
-
-
-
+# 手势-创建路径
+from typing import Self
+
+
+class path:
+    def __init__(self, startTime=0, duration=20, willContinue=False):
+        """
+        创建一个新的路径对象
+
+        参数:
+        - startTime (number): 延迟多久开始绘制路径，单位ms，默认为0
+        - duration (number): 路径绘制的时长，单位ms，默认为20
+        - willContinue (boolean): 在路径结束后，手指是否抬起，默认为False
+        """
+
+    def moveTo(self, x:int, y:int) -> None:
+        """
+        移动初始点到指定位置
+
+        参数:
+        - x (number): X轴坐标
+        - y (number): Y轴坐标
+        """
+        pass
+
+    def lineTo(self, x: int, y: int)-> None:
+        """
+        画直线到指定位置
+
+        参数:
+        - x (number): X轴坐标
+        - y (number): Y轴坐标
+        """
+        pass
+
+    def quadTo(self, x1: int, y1:int, x2:int, y2:int)-> None:
+        """
+        使用二次贝塞尔曲线绘制路径
+
+        参数:
+        - x1 (number): 控制点1的X轴坐标
+        - y1 (number): 控制点1的Y轴坐标
+        - x2 (number): 控制点2的X轴坐标
+        - y2 (number): 控制点2的Y轴坐标
+        """
+        pass
+
+
+
+
```

### Comparing `airscript-0.0.7/airscript.egg-info/SOURCES.txt` & `airscript-0.0.8/airscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airscript-0.0.7/setup.py` & `airscript-0.0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from setuptools import setup, find_packages
-
-VERSION = '0.0.7'
-DESCRIPTION = 'airscript 类型提示语言包'
-
-setup(
-    name="airscript",
-    version=VERSION,
-    author="ITisl",
-    author_email="aojoy@163.com",
-    description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=open('README.md', encoding="UTF8").read(),
-    packages=find_packages(),
-    keywords=['python', "airscript"],
-    license="MIT",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    url="https://github.com/itisl2220/airscript",
-)
+from setuptools import setup, find_packages
+
+VERSION = '0.0.8'
+DESCRIPTION = 'airscript 类型提示语言包'
+
+setup(
+    name="airscript",
+    version=VERSION,
+    author="ITisl",
+    author_email="aojoy@163.com",
+    description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=open('README.md', encoding="UTF8").read(),
+    packages=find_packages(),
+    keywords=['python', "airscript"],
+    license="MIT",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    url="https://github.com/itisl2220/airscript",
+)
```

