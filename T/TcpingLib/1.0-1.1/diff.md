# Comparing `tmp/TcpingLib-1.0.tar.gz` & `tmp/TcpingLib-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TcpingLib-1.0.tar", last modified: Thu Aug  3 01:17:18 2023, max compression
+gzip compressed data, was "dist\TcpingLib-1.1.tar", last modified: Thu Aug  3 01:24:27 2023, max compression
```

## Comparing `TcpingLib-1.0.tar` & `TcpingLib-1.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 01:17:18.722953 TcpingLib-1.0/
--rw-rw-rw-   0        0        0     1088 2023-08-03 01:13:38.000000 TcpingLib-1.0/LICENSE
--rw-rw-rw-   0        0        0      760 2023-08-03 01:17:18.721778 TcpingLib-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-08-03 01:03:35.000000 TcpingLib-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 01:17:18.718789 TcpingLib-1.0/TcpingLib.egg-info/
--rw-rw-rw-   0        0        0      760 2023-08-03 01:17:18.000000 TcpingLib-1.0/TcpingLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-08-03 01:17:18.000000 TcpingLib-1.0/TcpingLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 01:17:18.000000 TcpingLib-1.0/TcpingLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-08-03 01:17:18.000000 TcpingLib-1.0/TcpingLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 01:17:18.000000 TcpingLib-1.0/TcpingLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 01:17:18.722953 TcpingLib-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1417 2023-08-03 01:15:00.000000 TcpingLib-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:24:27.956913 TcpingLib-1.1/
+-rw-rw-rw-   0        0        0     1088 2023-08-03 01:13:38.000000 TcpingLib-1.1/LICENSE
+-rw-rw-rw-   0        0        0      760 2023-08-03 01:24:27.956913 TcpingLib-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-08-03 01:03:35.000000 TcpingLib-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 01:24:27.953718 TcpingLib-1.1/TcpingLib.egg-info/
+-rw-rw-rw-   0        0        0      760 2023-08-03 01:24:27.000000 TcpingLib-1.1/TcpingLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-08-03 01:24:27.000000 TcpingLib-1.1/TcpingLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 01:24:27.000000 TcpingLib-1.1/TcpingLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 01:24:27.000000 TcpingLib-1.1/TcpingLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 01:24:27.958067 TcpingLib-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1338 2023-08-03 01:23:17.000000 TcpingLib-1.1/setup.py
```

### Comparing `TcpingLib-1.0/LICENSE` & `TcpingLib-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TcpingLib-1.0/PKG-INFO` & `TcpingLib-1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TcpingLib
-Version: 1.0
+Version: 1.1
 Summary: A Tcping Lib
 Home-page: https://puqiar.top
 Author: PuqiAR
 Author-email: 2758126410@qq.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `TcpingLib-1.0/TcpingLib.egg-info/PKG-INFO` & `TcpingLib-1.1/TcpingLib.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TcpingLib
-Version: 1.0
+Version: 1.1
 Summary: A Tcping Lib
 Home-page: https://puqiar.top
 Author: PuqiAR
 Author-email: 2758126410@qq.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `TcpingLib-1.0/setup.py` & `TcpingLib-1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # you need to change all these
-VERSION = '1.0'
+VERSION = '1.1'
 DESCRIPTION = 'A Tcping Lib'
 
 setup(
     name="TcpingLib",
     version=VERSION,
     author="PuqiAR",
     author_email="2758126410@qq.com",
@@ -24,20 +24,15 @@
     long_description=long_description,
     # 使用find_packages()自动发现项目中的所有包
     packages=find_packages(),
     # 许可协议
     license='MIT',
     url='https://puqiar.top',
     # 要安装的依赖包
-    install_requires=[
-        "socket",
-        "struct",
-        "array",
-        "time",
-    ],
+    install_requires=[],
     # keywords=['python', 'menu', 'dumb_menu','windows','mac','linux'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

