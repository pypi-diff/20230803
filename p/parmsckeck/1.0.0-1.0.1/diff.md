# Comparing `tmp/parmsckeck-1.0.0.tar.gz` & `tmp/parmsckeck-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\parmsckeck-1.0.0.tar", last modified: Thu Aug  3 10:43:09 2023, max compression
+gzip compressed data, was "dist\parmsckeck-1.0.1.tar", last modified: Thu Aug  3 12:10:43 2023, max compression
```

## Comparing `parmsckeck-1.0.0.tar` & `parmsckeck-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 10:43:09.723011 parmsckeck-1.0.0/
--rw-rw-rw-   0        0        0    11558 2023-08-03 10:02:57.000000 parmsckeck-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      263 2023-08-03 10:43:09.721010 parmsckeck-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1666 2023-08-03 10:02:57.000000 parmsckeck-1.0.0/README.md
--rw-rw-rw-   0        0        0       54 2023-08-03 10:27:47.000000 parmsckeck-1.0.0/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 10:43:09.690016 parmsckeck-1.0.0/__pycache__/
--rw-rw-rw-   0        0        0     5816 2023-08-02 17:53:10.000000 parmsckeck-1.0.0/__pycache__/typecheck.cpython-38.pyc
-drwxrwxrwx   0        0        0        0 2023-08-03 10:43:09.715010 parmsckeck-1.0.0/parmsckeck.egg-info/
--rw-rw-rw-   0        0        0      263 2023-08-03 10:43:09.000000 parmsckeck-1.0.0/parmsckeck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-08-03 10:43:09.000000 parmsckeck-1.0.0/parmsckeck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 10:43:09.000000 parmsckeck-1.0.0/parmsckeck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-08-03 10:43:09.000000 parmsckeck-1.0.0/parmsckeck.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 10:43:09.000000 parmsckeck-1.0.0/parmsckeck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 10:43:09.723011 parmsckeck-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      345 2023-08-03 10:32:28.000000 parmsckeck-1.0.0/setup.py
--rw-rw-rw-   0        0        0     4829 2023-08-03 10:28:02.000000 parmsckeck-1.0.0/test.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:10:43.465633 parmsckeck-1.0.1/
+-rw-rw-rw-   0        0        0       46 2023-08-03 11:20:31.000000 parmsckeck-1.0.1/.gitignore
+-rw-rw-rw-   0        0        0    11558 2023-08-03 11:03:35.000000 parmsckeck-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      265 2023-08-03 12:10:43.464629 parmsckeck-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1669 2023-08-03 11:03:35.000000 parmsckeck-1.0.1/README.md
+-rw-rw-rw-   0        0        0       54 2023-08-03 11:03:35.000000 parmsckeck-1.0.1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:10:43.437638 parmsckeck-1.0.1/__pycache__/
+-rw-rw-rw-   0        0        0     5816 2023-08-03 11:03:35.000000 parmsckeck-1.0.1/__pycache__/typecheck.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6470 2023-08-03 12:06:17.000000 parmsckeck-1.0.1/check.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:10:43.461629 parmsckeck-1.0.1/parmsckeck.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-08-03 12:10:43.000000 parmsckeck-1.0.1/parmsckeck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-08-03 12:10:43.000000 parmsckeck-1.0.1/parmsckeck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 12:10:43.000000 parmsckeck-1.0.1/parmsckeck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 12:10:43.000000 parmsckeck-1.0.1/parmsckeck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 12:10:43.466631 parmsckeck-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      308 2023-08-03 12:02:27.000000 parmsckeck-1.0.1/setup.py
+-rw-rw-rw-   0        0        0     4829 2023-08-03 11:03:35.000000 parmsckeck-1.0.1/test.py
```

### Comparing `parmsckeck-1.0.0/LICENSE` & `parmsckeck-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parmsckeck-1.0.0/README.md` & `parmsckeck-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# typecheck
+# parmscheck
 
 #### 介绍
 支持python函数类型检查的装饰器，提供了一种方便的方式来对函数的参数进行运行时类型检查。通过使用这个装饰器，开发者可以轻松确保函数的输入参数是否为预期的类型。
 #### 特点
 
 - 简单易用：只需要在函数上应用一个装饰器，即可对任何函数进行类型检查。无需复杂的配置或额外的代码。
 - 支持类型注解：装饰器与Python的类型注解完美结合。开发者可以简单地为函数的参数添加类型注解，装饰器会在运行时自动验证参数的类型。
 
 
 #### 安装教程
 
 你可以使用Python包管理工具pip来安装这个装饰器库：
-`pip install typecheck`
+`pip install parmscheck`
 
 
 #### 使用说明
 
 
 ```
-from typecheck import check_args,check_args_for_class
+from parmscheck import check_args,check_args_for_class
 
 T = TypeVar('T', int, float, Dict[int, str])
 P = TypeVar('P')
 @check_args
 def multiply(a: List[int], b: T) -> int:
     return a * b
```

### Comparing `parmsckeck-1.0.0/__pycache__/typecheck.cpython-38.pyc` & `parmsckeck-1.0.1/__pycache__/typecheck.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `parmsckeck-1.0.0/test.py` & `parmsckeck-1.0.1/test.py`

 * *Files identical despite different names*

