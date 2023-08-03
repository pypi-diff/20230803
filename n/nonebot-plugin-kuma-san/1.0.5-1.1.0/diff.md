# Comparing `tmp/nonebot_plugin_kuma_san-1.0.5.tar.gz` & `tmp/nonebot_plugin_kuma_san-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_kuma_san-1.0.5.tar", last modified: Thu Aug  3 06:25:39 2023, max compression
+gzip compressed data, was "nonebot_plugin_kuma_san-1.1.0.tar", last modified: Thu Aug  3 06:38:20 2023, max compression
```

## Comparing `nonebot_plugin_kuma_san-1.0.5.tar` & `nonebot_plugin_kuma_san-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 06:25:39.815342 nonebot_plugin_kuma_san-1.0.5/
--rw-rw-rw-   0        0        0     1069 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     1943 2023-08-03 06:25:39.813897 nonebot_plugin_kuma_san-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1358 2023-08-03 06:08:28.000000 nonebot_plugin_kuma_san-1.0.5/README.md
--rw-rw-rw-   0        0        0      756 2023-08-03 06:06:37.000000 nonebot_plugin_kuma_san-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-03 06:25:39.815342 nonebot_plugin_kuma_san-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-03 06:25:39.720553 nonebot_plugin_kuma_san-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-08-03 06:25:39.749194 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/
--rw-rw-rw-   0        0        0     6250 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/__init__.py
--rw-rw-rw-   0        0        0     1799 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/model.py
-drwxrwxrwx   0        0        0        0 2023-08-03 06:25:39.782392 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/services/
--rw-rw-rw-   0        0        0        0 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/services/__init__.py
--rw-rw-rw-   0        0        0     3299 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/services/stage_service.py
-drwxrwxrwx   0        0        0        0 2023-08-03 06:25:39.812854 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/utils/
--rw-rw-rw-   0        0        0        0 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/utils/__init__.py
--rw-rw-rw-   0        0        0      554 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/utils/api_parse.py
--rw-rw-rw-   0        0        0      698 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/utils/common.py
--rw-rw-rw-   0        0        0      430 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/utils/constants.py
--rw-rw-rw-   0        0        0     4457 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/utils/translate.py
-drwxrwxrwx   0        0        0        0 2023-08-03 06:25:39.778863 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san.egg-info/
--rw-rw-rw-   0        0        0     1943 2023-08-03 06:25:39.000000 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-08-03 06:25:39.000000 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 06:25:39.000000 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-08-03 06:25:39.000000 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-08-03 06:25:39.000000 nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 06:38:20.588418 nonebot_plugin_kuma_san-1.1.0/
+-rw-rw-rw-   0        0        0     1069 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1874 2023-08-03 06:38:20.588418 nonebot_plugin_kuma_san-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1289 2023-08-03 06:37:12.000000 nonebot_plugin_kuma_san-1.1.0/README.md
+-rw-rw-rw-   0        0        0      756 2023-08-03 06:37:12.000000 nonebot_plugin_kuma_san-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 06:38:20.588418 nonebot_plugin_kuma_san-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 06:38:20.544106 nonebot_plugin_kuma_san-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 06:38:20.551220 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/
+-rw-rw-rw-   0        0        0     6250 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/__init__.py
+-rw-rw-rw-   0        0        0     1799 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/model.py
+drwxrwxrwx   0        0        0        0 2023-08-03 06:38:20.579744 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/services/
+-rw-rw-rw-   0        0        0        0 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/services/__init__.py
+-rw-rw-rw-   0        0        0     3299 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/services/stage_service.py
+drwxrwxrwx   0        0        0        0 2023-08-03 06:38:20.587388 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/utils/
+-rw-rw-rw-   0        0        0        0 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/utils/__init__.py
+-rw-rw-rw-   0        0        0      554 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/utils/api_parse.py
+-rw-rw-rw-   0        0        0      698 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/utils/common.py
+-rw-rw-rw-   0        0        0      430 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/utils/constants.py
+-rw-rw-rw-   0        0        0     4457 2023-08-02 14:18:33.000000 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/utils/translate.py
+drwxrwxrwx   0        0        0        0 2023-08-03 06:38:20.578548 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san.egg-info/
+-rw-rw-rw-   0        0        0     1874 2023-08-03 06:38:20.000000 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-08-03 06:38:20.000000 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 06:38:20.000000 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-08-03 06:38:20.000000 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-08-03 06:38:20.000000 nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san.egg-info/top_level.txt
```

### Comparing `nonebot_plugin_kuma_san-1.0.5/LICENSE` & `nonebot_plugin_kuma_san-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kuma_san-1.0.5/PKG-INFO` & `nonebot_plugin_kuma_san-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_kuma_san
-Version: 1.0.5
+Version: 1.1.0
 Summary: 一个获取斯普拉遁3场地信息用的nonebot插件
 Author-email: ReiiNoki <reiinoki@outlook.com>
 Project-URL: Homepage, https://github.com/ReiiNoki/nonebot_plugin_kuma_san
 Project-URL: Bug Tracker, https://github.com/ReiiNoki/nonebot_plugin_kuma_san/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,19 +30,17 @@
 
 ```
 nb plugin install nonebot_plugin_kuma_san
 ```
 ```
 pip install nonebot_plugin_kuma_san
 ```
-## 更新
-v.1.0.1 2023.8.3 更新武器和场地的中日文翻译
 
 ## 更新
-v.1.0.5 2023.8.3 更新武器和场地的中日文翻译，添加新版本的武器和场地信息
+v.1.1.0 2023.8.3 更新武器和场地的中日文翻译，添加新版本的武器和场地信息
 
 ## 使用
 
 对已安装本插件的nonebot发送以下指令可获取对应的场地信息
 
 reg (涂地)/chal (真格挑战)/open (真格开放)/baito (打工)/fest (祭典)/x (x段) + (可选)now/next
```

### Comparing `nonebot_plugin_kuma_san-1.0.5/README.md` & `nonebot_plugin_kuma_san-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 
 ```
 nb plugin install nonebot_plugin_kuma_san
 ```
 ```
 pip install nonebot_plugin_kuma_san
 ```
-## 更新
-v.1.0.1 2023.8.3 更新武器和场地的中日文翻译
 
 ## 更新
-v.1.0.5 2023.8.3 更新武器和场地的中日文翻译，添加新版本的武器和场地信息
+v.1.1.0 2023.8.3 更新武器和场地的中日文翻译，添加新版本的武器和场地信息
 
 ## 使用
 
 对已安装本插件的nonebot发送以下指令可获取对应的场地信息
 
 reg (涂地)/chal (真格挑战)/open (真格开放)/baito (打工)/fest (祭典)/x (x段) + (可选)now/next
```

### Comparing `nonebot_plugin_kuma_san-1.0.5/pyproject.toml` & `nonebot_plugin_kuma_san-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nonebot_plugin_kuma_san"
-version = "1.0.5"
+version = "1.1.0"
 authors = [
   { name="ReiiNoki", email="reiinoki@outlook.com" },
 ]
 description = "一个获取斯普拉遁3场地信息用的nonebot插件"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/__init__.py` & `nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/model.py` & `nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/services/stage_service.py` & `nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/services/stage_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/utils/api_parse.py` & `nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/utils/api_parse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/utils/common.py` & `nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/utils/common.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san/utils/translate.py` & `nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san/utils/translate.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san.egg-info/PKG-INFO` & `nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-kuma-san
-Version: 1.0.5
+Version: 1.1.0
 Summary: 一个获取斯普拉遁3场地信息用的nonebot插件
 Author-email: ReiiNoki <reiinoki@outlook.com>
 Project-URL: Homepage, https://github.com/ReiiNoki/nonebot_plugin_kuma_san
 Project-URL: Bug Tracker, https://github.com/ReiiNoki/nonebot_plugin_kuma_san/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,19 +30,17 @@
 
 ```
 nb plugin install nonebot_plugin_kuma_san
 ```
 ```
 pip install nonebot_plugin_kuma_san
 ```
-## 更新
-v.1.0.1 2023.8.3 更新武器和场地的中日文翻译
 
 ## 更新
-v.1.0.5 2023.8.3 更新武器和场地的中日文翻译，添加新版本的武器和场地信息
+v.1.1.0 2023.8.3 更新武器和场地的中日文翻译，添加新版本的武器和场地信息
 
 ## 使用
 
 对已安装本插件的nonebot发送以下指令可获取对应的场地信息
 
 reg (涂地)/chal (真格挑战)/open (真格开放)/baito (打工)/fest (祭典)/x (x段) + (可选)now/next
```

### Comparing `nonebot_plugin_kuma_san-1.0.5/src/nonebot_plugin_kuma_san.egg-info/SOURCES.txt` & `nonebot_plugin_kuma_san-1.1.0/src/nonebot_plugin_kuma_san.egg-info/SOURCES.txt`

 * *Files identical despite different names*

