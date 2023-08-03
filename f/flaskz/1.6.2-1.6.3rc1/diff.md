# Comparing `tmp/flaskz-1.6.2.tar.gz` & `tmp/flaskz-1.6.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskz-1.6.2.tar", last modified: Thu Jul  6 03:11:18 2023, max compression
+gzip compressed data, was "flaskz-1.6.3rc1.tar", last modified: Thu Aug  3 02:20:54 2023, max compression
```

## Comparing `flaskz-1.6.2.tar` & `flaskz-1.6.3rc1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.739321 flaskz-1.6.2/
--rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2022-12-30 08:48:07.000000 flaskz-1.6.2/LICENSE
--rw-r--r--   0 taozh      (501) staff       (20)     7215 2023-07-06 03:11:18.739468 flaskz-1.6.2/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)     6769 2023-07-06 02:34:05.000000 flaskz-1.6.2/README.md
--rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.6.2/pyproject.toml
--rwxrwxrwx   0 taozh      (501) staff       (20)      776 2023-07-06 03:11:18.740287 flaskz-1.6.2/setup.cfg
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.711022 flaskz-1.6.2/src/
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.716218 flaskz-1.6.2/src/flaskz/
--rwxrwxrwx   0 taozh      (501) staff       (20)       23 2023-07-06 02:20:13.000000 flaskz-1.6.2/src/flaskz/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.719566 flaskz-1.6.2/src/flaskz/auth/
--rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.6.2/src/flaskz/auth/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8831 2022-09-19 02:16:30.000000 flaskz-1.6.2/src/flaskz/auth/_jws.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.721735 flaskz-1.6.2/src/flaskz/ext/
--rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.6.2/src/flaskz/ext/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-04-26 10:31:33.000000 flaskz-1.6.2/src/flaskz/ext/cypher.py
--rw-r--r--   0 taozh      (501) staff       (20)    13548 2023-07-06 03:10:54.000000 flaskz-1.6.2/src/flaskz/ext/ssh.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.722370 flaskz-1.6.2/src/flaskz/log/
--rwxrwxrwx   0 taozh      (501) staff       (20)     2395 2023-07-06 02:14:56.000000 flaskz-1.6.2/src/flaskz/log/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.726255 flaskz-1.6.2/src/flaskz/models/
--rwxrwxrwx   0 taozh      (501) staff       (20)     5524 2023-07-06 02:21:14.000000 flaskz-1.6.2/src/flaskz/models/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    29523 2023-07-06 02:23:24.000000 flaskz-1.6.2/src/flaskz/models/_base.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    10649 2023-06-17 12:07:38.000000 flaskz-1.6.2/src/flaskz/models/_model.py
--rw-r--r--   0 taozh      (501) staff       (20)     9352 2023-06-26 02:18:53.000000 flaskz-1.6.2/src/flaskz/models/_query_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     7426 2023-06-21 08:20:49.000000 flaskz-1.6.2/src/flaskz/models/_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.6.2/src/flaskz/res_status_codes.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.729022 flaskz-1.6.2/src/flaskz/rest/
--rwxrwxrwx   0 taozh      (501) staff       (20)    19434 2023-06-25 06:21:35.000000 flaskz-1.6.2/src/flaskz/rest/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.6.2/src/flaskz/rest/_mgmt.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     3931 2023-05-16 02:55:12.000000 flaskz-1.6.2/src/flaskz/rest/_util.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.738293 flaskz-1.6.2/src/flaskz/utils/
--rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-06-21 05:37:43.000000 flaskz-1.6.2/src/flaskz/utils/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2359 2023-05-08 02:37:05.000000 flaskz-1.6.2/src/flaskz/utils/_app.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2771 2023-05-16 03:06:45.000000 flaskz-1.6.2/src/flaskz/utils/_cache.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     6947 2023-04-26 10:28:36.000000 flaskz-1.6.2/src/flaskz/utils/_cls.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    10394 2023-05-06 11:11:55.000000 flaskz-1.6.2/src/flaskz/utils/_common.py
--rw-r--r--   0 taozh      (501) staff       (20)      839 2023-04-26 10:28:36.000000 flaskz-1.6.2/src/flaskz/utils/_func.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.6.2/src/flaskz/utils/_magic.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     6570 2023-06-25 10:52:01.000000 flaskz-1.6.2/src/flaskz/utils/_request_api.py
--rwxrwxrwx   0 taozh      (501) staff       (20)      973 2023-07-06 02:17:15.000000 flaskz-1.6.2/src/flaskz/utils/_request_args.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2617 2023-05-16 03:06:45.000000 flaskz-1.6.2/src/flaskz/utils/_response.py
--rw-r--r--   0 taozh      (501) staff       (20)     4522 2023-06-29 07:20:02.000000 flaskz-1.6.2/src/flaskz/utils/_timer.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.718433 flaskz-1.6.2/src/flaskz.egg-info/
--rwxrwxrwx   0 taozh      (501) staff       (20)     7215 2023-07-06 03:11:18.000000 flaskz-1.6.2/src/flaskz.egg-info/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)      952 2023-07-06 03:11:18.000000 flaskz-1.6.2/src/flaskz.egg-info/SOURCES.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        1 2023-07-06 03:11:18.000000 flaskz-1.6.2/src/flaskz.egg-info/dependency_links.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)       88 2023-07-06 03:11:18.000000 flaskz-1.6.2/src/flaskz.egg-info/requires.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        7 2023-07-06 03:11:18.000000 flaskz-1.6.2/src/flaskz.egg-info/top_level.txt
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-08-03 02:20:54.202298 flaskz-1.6.3rc1/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2022-12-30 08:48:07.000000 flaskz-1.6.3rc1/LICENSE
+-rw-r--r--   0 taozh      (501) staff       (20)     7333 2023-08-03 02:20:54.202559 flaskz-1.6.3rc1/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6886 2023-08-03 02:20:42.000000 flaskz-1.6.3rc1/README.md
+-rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.6.3rc1/pyproject.toml
+-rwxrwxrwx   0 taozh      (501) staff       (20)      779 2023-08-03 02:20:54.203813 flaskz-1.6.3rc1/setup.cfg
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-08-03 02:20:54.171656 flaskz-1.6.3rc1/src/
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-08-03 02:20:54.176431 flaskz-1.6.3rc1/src/flaskz/
+-rwxrwxrwx   0 taozh      (501) staff       (20)       26 2023-08-03 02:19:33.000000 flaskz-1.6.3rc1/src/flaskz/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-08-03 02:20:54.180915 flaskz-1.6.3rc1/src/flaskz/auth/
+-rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.6.3rc1/src/flaskz/auth/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8831 2022-09-19 02:16:30.000000 flaskz-1.6.3rc1/src/flaskz/auth/_jws.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-08-03 02:20:54.183825 flaskz-1.6.3rc1/src/flaskz/ext/
+-rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.6.3rc1/src/flaskz/ext/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-04-26 10:31:33.000000 flaskz-1.6.3rc1/src/flaskz/ext/cypher.py
+-rw-r--r--   0 taozh      (501) staff       (20)    11563 2023-07-10 03:21:16.000000 flaskz-1.6.3rc1/src/flaskz/ext/ssh.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-08-03 02:20:54.184600 flaskz-1.6.3rc1/src/flaskz/log/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2395 2023-07-06 02:14:56.000000 flaskz-1.6.3rc1/src/flaskz/log/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-08-03 02:20:54.189395 flaskz-1.6.3rc1/src/flaskz/models/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     5524 2023-07-06 02:21:14.000000 flaskz-1.6.3rc1/src/flaskz/models/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    29523 2023-07-06 02:23:24.000000 flaskz-1.6.3rc1/src/flaskz/models/_base.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    10649 2023-06-17 12:07:38.000000 flaskz-1.6.3rc1/src/flaskz/models/_model.py
+-rw-r--r--   0 taozh      (501) staff       (20)     9513 2023-08-01 02:37:52.000000 flaskz-1.6.3rc1/src/flaskz/models/_query_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7426 2023-06-21 08:20:49.000000 flaskz-1.6.3rc1/src/flaskz/models/_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.6.3rc1/src/flaskz/res_status_codes.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-08-03 02:20:54.191963 flaskz-1.6.3rc1/src/flaskz/rest/
+-rwxrwxrwx   0 taozh      (501) staff       (20)    20357 2023-08-01 02:44:43.000000 flaskz-1.6.3rc1/src/flaskz/rest/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.6.3rc1/src/flaskz/rest/_mgmt.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     4091 2023-07-31 08:20:50.000000 flaskz-1.6.3rc1/src/flaskz/rest/_util.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-08-03 02:20:54.201421 flaskz-1.6.3rc1/src/flaskz/utils/
+-rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-06-21 05:37:43.000000 flaskz-1.6.3rc1/src/flaskz/utils/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2359 2023-05-08 02:37:05.000000 flaskz-1.6.3rc1/src/flaskz/utils/_app.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2771 2023-05-16 03:06:45.000000 flaskz-1.6.3rc1/src/flaskz/utils/_cache.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6947 2023-04-26 10:28:36.000000 flaskz-1.6.3rc1/src/flaskz/utils/_cls.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    10394 2023-05-06 11:11:55.000000 flaskz-1.6.3rc1/src/flaskz/utils/_common.py
+-rw-r--r--   0 taozh      (501) staff       (20)      839 2023-04-26 10:28:36.000000 flaskz-1.6.3rc1/src/flaskz/utils/_func.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.6.3rc1/src/flaskz/utils/_magic.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6570 2023-06-25 10:52:01.000000 flaskz-1.6.3rc1/src/flaskz/utils/_request_api.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)      973 2023-07-06 02:17:15.000000 flaskz-1.6.3rc1/src/flaskz/utils/_request_args.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2617 2023-05-16 03:06:45.000000 flaskz-1.6.3rc1/src/flaskz/utils/_response.py
+-rw-r--r--   0 taozh      (501) staff       (20)     4522 2023-06-29 07:20:02.000000 flaskz-1.6.3rc1/src/flaskz/utils/_timer.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-08-03 02:20:54.179425 flaskz-1.6.3rc1/src/flaskz.egg-info/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7333 2023-08-03 02:20:54.000000 flaskz-1.6.3rc1/src/flaskz.egg-info/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)      952 2023-08-03 02:20:54.000000 flaskz-1.6.3rc1/src/flaskz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        1 2023-08-03 02:20:54.000000 flaskz-1.6.3rc1/src/flaskz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)       88 2023-08-03 02:20:54.000000 flaskz-1.6.3rc1/src/flaskz.egg-info/requires.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        7 2023-08-03 02:20:54.000000 flaskz-1.6.3rc1/src/flaskz.egg-info/top_level.txt
```

### Comparing `flaskz-1.6.2/LICENSE` & `flaskz-1.6.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/PKG-INFO` & `flaskz-1.6.3rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.6.2
+Version: 1.6.3rc1
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,14 +25,16 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.6.3rc1** `2023/08/03`
+    - [A] `flaskz.rest.register_model_*`路由生成函数添加路由`endpoint`参数
 - **1.6.2** `2023/07/06`
     - [F] 修复`flaskz.utils._request_args.py`中`import parse_pss as get_pss`的导入问题
 - **1.6.1** `2023/07/01`
     - [C] `flaskz.utils.get_pss`(`flaskz.models.parse_pss`)函数返回项由SQL字符串拼接改为参数化模式以预防SQL注入
     - [A] 添加`flaskz.utils.run_at`函数用于执行定时函数
 - **1.6** `2023/06/16`
     - [A] `BaseModelMixin`添加`count`方法, 用于数量查询(全量/条件)
```

### Comparing `flaskz-1.6.2/README.md` & `flaskz-1.6.3rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.6.3rc1** `2023/08/03`
+    - [A] `flaskz.rest.register_model_*`路由生成函数添加路由`endpoint`参数
 - **1.6.2** `2023/07/06`
     - [F] 修复`flaskz.utils._request_args.py`中`import parse_pss as get_pss`的导入问题
 - **1.6.1** `2023/07/01`
     - [C] `flaskz.utils.get_pss`(`flaskz.models.parse_pss`)函数返回项由SQL字符串拼接改为参数化模式以预防SQL注入
     - [A] 添加`flaskz.utils.run_at`函数用于执行定时函数
 - **1.6** `2023/06/16`
     - [A] `BaseModelMixin`添加`count`方法, 用于数量查询(全量/条件)
```

### Comparing `flaskz-1.6.2/setup.cfg` & `flaskz-1.6.3rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flaskz
-version = 1.6.2
+version = 1.6.3rc1
 author = Zhang Tao
 author_email = taozh1982@gmail.com
 description = Flask and SQLAlchemy extensions for web applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/taozh1982/flaskz
 project_urls =
```

### Comparing `flaskz-1.6.2/src/flaskz/auth/_jws.py` & `flaskz-1.6.3rc1/src/flaskz/auth/_jws.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/ext/cypher.py` & `flaskz-1.6.3rc1/src/flaskz/ext/cypher.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/ext/ssh.py` & `flaskz-1.6.3rc1/src/flaskz/ext/ssh.py`

 * *Files 18% similar despite different names*

```diff
@@ -88,43 +88,45 @@
     def channel(self):
         if not hasattr(self, '_channel'):
             self._channel = self.ssh.invoke_shell(height=100000)
             if self._timeout > 0:
                 self._channel.settimeout(self._timeout)
         return self._channel
 
-    def run_command(self, command, recv=True):
+    def run_command(self, command, recv=True, clean=True):
         """
         Run the command.
         If recv is False, just run the command and return immediately, without waiting for the result
 
-        .. versionupdated:: 1.6.1   - @2023-06-26 add recv parameter
+        .. versionupdated::
+            1.6.1   - @2023-06-26 add recv parameter
+            1.6.3   - @2023-07-10 add clean parameter
 
         Example:
             ssh.run_command('ls -l')
             ssh.run_command('show run')
+            ssh.run_command({
+                'command': ' ',
+                'clean': False,
+            })
 
          :param command: the command to run.
          :param recv: wait for the result or not.
+         :param clean: clean output info or not, default True(clean)
 
          :return: the output of the command
         """
-        if type(command) is dict:
-            _command = command.get('command')
-            _recv = command.get('recv') is not False
-        else:
-            _command = command
-            _recv = recv
+        _command, _recv, _clean = _get_command_arg(command, recv=recv, clean=clean)
 
         _command = _command.strip()
         self.channel.send(_command + '\n')
         if _recv is False:
             return None
 
-        output = self._get_output(_command)
+        output = self._get_output(_command, clean=_clean)
         enable_commands = ('sudo', 'enable')
         secondary_password = self._secondary_password  # or self._password
         if secondary_password and \
                 _command.lower().startswith(enable_commands) and \
                 'assword' in output:  # input password
             pwd_output = self.run_command(secondary_password)
             # if 'assword' in pwd_output:
@@ -217,17 +219,18 @@
         except IOError as e:
             if e.errno == errno.ENOENT:
                 return False
             raise
         else:
             return True
 
-    def _get_output(self, command):
+    def _get_output(self, command, clean=True):
         output = self._recv_data()
-        output = _clear_redundant(output, command)
+        if clean is not False:
+            output = _clean_output_info(output, command)
         return output
 
     def _recv_data(self):
         """Receive the command output"""
         while not self.channel.recv_ready():
             time.sleep(0.01)
         res_list = []
@@ -242,14 +245,26 @@
             if len(info) < 1024:  # read speed > write speed
                 if info.endswith(self.recv_endswith):  # Cisco C9300:# /
                     break
 
         return ''.join(res_list)
 
 
+def _get_command_arg(command, recv, clean):
+    if type(command) is dict:
+        _command = command.get('command')
+        _recv = command.get('recv') is not False if 'recv' in command else recv
+        _clean = command.get('clean') is not False if 'clean' in command else clean
+    else:
+        _command = command
+        _recv = recv
+        _clean = clean
+    return _command, _recv, _clean
+
+
 def _create_socket(hostname, port, timeout=0):
     """
     Create socket instance.
     If timeout>0, set the timeout of the instance, otherwise use the default timeout(maybe 75s).
 
     :param hostname:
     :param port:
@@ -274,15 +289,15 @@
     else:
         raise SSHException(
             'Unable to connect to {}: {}'.format(hostname, reason)
         )
     return sock
 
 
-def _clear_redundant(txt, command):
+def _clean_output_info(txt, command):
     """
     Clear the redundant information.
     - Welcome info      ex)Welcome to Ubuntu...
     - Last login info   ex)Last login...
     - Path info         ex)[root@localhost ~]...
     - Command info      ex)ls -l
 
@@ -305,75 +320,7 @@
 
 
 def _remove_end_slash(path):
     """Remove ending slash """
     if path[-1] == '/':
         return path[0:-1]
     return path
-
-
-if __name__ == '__main__':
-    servers = [
-        {  # C9300
-            'host': '10.75.37.165',
-            'username': 'admin',
-            'password': 'Cisco123',
-            'secondary_password': 'Cisco123',
-            'recv_endswith': ['# ', '$ ', ': ', '? ', '#'],
-            'commands': ['enable', 'show udp | in ( 514 )']
-            # 'commands': ['show run']
-        },
-        # {  # C9300
-        #     'host': '10.75.37.165',
-        #     'username': 'admin',
-        #     'password': 'Cisco123',
-        #     # 'secondary_password': 'Cisco123',
-        #     'recv_endswith': ['# ', '$ ', ': ', '? ', '#'],
-        #     'commands': ['enable', 'Cisco123', {'command': 'show run', 'wait': False}]
-        #     # 'commands': ['show run']
-        # },
-        # {  # Centos
-        #     'host': '10.124.4.21',
-        #     'username': 'admin1',
-        #     'password': 'Cisco@123',
-        #     'commands': ['show int eth3/1']
-        # },
-        # {  # Centos
-        #     'host': '10.124.5.222',
-        #     'username': 'root',
-        #     'password': 'cisco123',
-        #     'commands': ['ls -l', 'cd ../opt', '\cp a.txt b.txt']
-        # },
-        # {  # Ubuntu
-        #     'host': '10.124.5.198',
-        #     'username': 'root',
-        #     'password': 'Cisco@123',
-        #     'commands': ['ls -l']
-        # },
-        # {  # Ubuntu, test input password
-        #     'host': '10.124.5.216',
-        #     'username': 'cisco',
-        #     'password': 'cisco123',
-        #     'secondary_password': 'cisco123',
-        #     'commands': ['sudo ls -l']
-        # },
-        # {  # NX-OS
-        #     'host': '10.124.11.134',
-        #     'username': 'admin',
-        #     'password': 'Cisco@123',
-        #     'commands': ['show version', 'show running-config']
-        # },
-        # {  # NX-OS
-        #     'host': '10.66.94.62',
-        #     'username': 'admin',
-        #     'password': 'cisco!123',
-        #     'commands': ['show version', 'show running-config']
-        # }
-    ]
-    for item in servers:
-        print((item.get('host') + ' : ' + str(item.get('commands'))).center(100, '*'))
-        with ssh_session(item.get('host'), item.get('username'), item.get('password'), timeout=10, recv_endswith=item.get('recv_endswith'),
-                         secondary_password=item.get('secondary_password')) as ssh:
-            print(ssh.run_command_list(item.get('commands'), True))
-
-    # ssh.sftp_get_dir('/usr/projects/git/srte/src/', '/Users/taozh/Work/Codes/ssh_test/sftp')
-    print('\n', 'end'.center(100, '-'))
```

### Comparing `flaskz-1.6.2/src/flaskz/log/__init__.py` & `flaskz-1.6.3rc1/src/flaskz/log/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/models/__init__.py` & `flaskz-1.6.3rc1/src/flaskz/models/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/models/_base.py` & `flaskz-1.6.3rc1/src/flaskz/models/_base.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/models/_model.py` & `flaskz-1.6.3rc1/src/flaskz/models/_model.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/models/_query_util.py` & `flaskz-1.6.3rc1/src/flaskz/models/_query_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,17 @@
             TemplateModel, {   # FROM templates
                 "search": {                         # WHERE
                     "like": "t",                    # name like '%t%' OR description like '%t%' (TemplateModel.like_columns = ['name', description])
                     "age": {                        # AND (age>1 AND age<20)
                         ">": 1,                     # operator:value, operators)'='/'>'/'<'/'>='/'<='/'BETWEEN'/'LIKE'/'IN'
                         "<": 20
                     },
+                   "city": {                        # AND (city IN ('Paris','London'))
+                        "in": ['Paris' ,'London'],
+                    },
                     "email": "taozh@focus-ui.com",  # AND (email='taozh@focus-ui.com')
                     "_ors": {                       # AND (country='America' OR country='Canada')
                         "country": "America||Canada"
                     },
                     "_ands": {                      # AND (grade>1 AND grade<5)
                         "grade": {
                             ">": 1,
```

### Comparing `flaskz-1.6.2/src/flaskz/models/_util.py` & `flaskz-1.6.3rc1/src/flaskz/models/_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/res_status_codes.py` & `flaskz-1.6.3rc1/src/flaskz/res_status_codes.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/rest/__init__.py` & `flaskz-1.6.3rc1/src/flaskz/rest/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,35 +108,36 @@
     if 'pss' in types:
         register_model_query_pss_route(app, model, rule, module, to_json_option=to_json_option, strict_slash=strict_slash)
     if multi_models and ('multi' in types or 'multiple' in types):
         register_models_query_route(app, multi_models, rule, module)
     return app
 
 
-def register_model_add_route(app, model, rule, module=None, action='add', methods=None, to_json_option=None, strict_slash=True):
+def register_model_add_route(app, model, rule, module=None, action='add', methods=None, to_json_option=None, strict_slash=True, endpoint=None):
     """
     Register a add type URL rule for the specified model class to the application/blueprint.
 
     Examples:
         register_model_add_route(api_blueprint, User, 'users', 'users')
 
     :param app: Flask application / Blueprints instance
     :param model: The DB model class, ex)User
     :param rule: The URL rule string, ex)/users
     :param module: The module name for permission check, ex)users
     :param action: The action of the module for permission check, ex)add
     :param methods: The methods of the route, default is ['POST']
     :param to_json_option: The option to return the json, ex){'cascade': 1}
     :param strict_slash: If not false, the rule url will end with slash
+    :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
     :return:
     """
     methods = methods or ['POST']
     rule, did_rule = _get_route_rule(rule, strict_slash)
 
-    @app.route(rule, methods=methods)
+    @app.route(rule, methods=methods, endpoint=endpoint)
     @rest_permission_required(module, action)
     @gen_route_method('add', rule)
     def add():
         request_json = request.json
         req_log_data = json.dumps(request_json)
 
         success, data = model.add(request_json)
@@ -145,49 +146,50 @@
         res_log_data = get_log_data(res_data)
         log_operation(module, 'add', success, req_log_data, res_log_data)
         flaskz_logger.info(get_rest_log_msg('Add {} data'.format(model.get_class_name()), req_log_data, success, res_log_data))
 
         return create_response(success, res_data)
 
 
-def register_model_delete_route(app, model, rule, module=None, action='delete', methods=None, to_json_option=None, strict_slash=True):
+def register_model_delete_route(app, model, rule, module=None, action='delete', methods=None, to_json_option=None, strict_slash=True, endpoint=None):
     """
     Register a delete type URL rule for the specified model class to the application/blueprint.
 
     Examples:
         register_model_delete_route(api_blueprint, User, 'users', 'users')
 
     :param app: Flask application / Blueprints instance
     :param model: The DB model class, ex)User
     :param rule: The URL rule string, ex)/users
     :param module: The module name for permission check, ex)users
     :param action: The action of the module for permission check, ex)delete
     :param methods: The methods of the route, default is ['DELETE']
     :param to_json_option: The option to return the json, ex){'cascade': 1}
     :param strict_slash: If not false, the rule url will end with slash
+    :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
     :return:
     """
     methods = methods or ['DELETE']
     rule, did_rule = _get_route_rule(rule, strict_slash)
 
-    @app.route(did_rule, methods=methods)
+    @app.route(did_rule, methods=methods, endpoint=endpoint)
     @rest_permission_required(module, action)
     @gen_route_method('delete', rule)
     def delete(did):
         success, data = model.delete(did)
         res_data = model_to_dict(data, to_json_option)
 
         res_log_data = get_log_data(res_data)
         log_operation(module, 'delete', success, did, res_log_data)
         flaskz_logger.info(get_rest_log_msg('Delete {} data'.format(model.get_class_name()), did, success, res_log_data))
 
         return create_response(success, res_data)
 
 
-def register_model_update_route(app, model, rule, module=None, action='update', methods=None, to_json_option=None, strict_slash=True):
+def register_model_update_route(app, model, rule, module=None, action='update', methods=None, to_json_option=None, strict_slash=True, endpoint=None):
     """
     Register update type URL rule for the specified model class to the application/blueprint.
     The priority of the primary key in the url is higher than that in the body.
 
     Examples:
         register_model_update_route(api_blueprint, User, 'users', 'users')
 
@@ -195,21 +197,22 @@
     :param model: The DB model class, ex)User
     :param rule: The URL rule string, ex)/users
     :param module: The module name for permission check, ex)users
     :param action: The action of the module for permission check, ex)update
     :param methods: The methods of the route, default is ['PATCH']
     :param to_json_option: The option to return the json, ex){'cascade': 1}
     :param strict_slash: If not false, the rule url will end with slash
+    :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
     :return:
     """
     methods = methods or ['PATCH']
     rule, did_rule = _get_route_rule(rule, strict_slash)
 
-    @app.route(rule, methods=methods)
-    @app.route(did_rule, methods=methods)
+    @app.route(rule, methods=methods, endpoint=endpoint)
+    @app.route(did_rule, methods=methods, endpoint=endpoint)
     @rest_permission_required(module, action)
     @gen_route_method('update', rule)
     def update(did=None):
         request_json = request.json
         if did is not None:
             request_json[model.get_primary_field()] = did  # use pk in url
         req_log_data = json.dumps(request_json)
@@ -220,15 +223,15 @@
         res_log_data = get_log_data(res_data)
         log_operation(module, 'update', success, req_log_data, res_log_data)
         flaskz_logger.info(get_rest_log_msg('Update {} data'.format(model.get_class_name()), req_log_data, success, res_log_data))
 
         return create_response(success, res_data)
 
 
-def register_model_upsert_route(app, model, rule, module=None, action='upsert', methods=None, to_json_option=None, strict_slash=True, rule_suffix='upsert'):
+def register_model_upsert_route(app, model, rule, module=None, action='upsert', methods=None, to_json_option=None, strict_slash=True, rule_suffix='upsert', endpoint=None):
     """
     Register a upsert type URL rule for the specified model class to the application/blueprint.
     If primary key value is in json, perform an update action, otherwise perform an add action.
 
     Examples:
         register_model_upsert_route(api_blueprint, User, 'users', 'users')
 
@@ -237,19 +240,20 @@
     :param rule: The URL rule string, ex)/users
     :param module: The module name for permission check, ex)users
     :param action: The action of the module for permission check, ex)update
     :param methods: The methods of the route, default is ['PATCH']
     :param to_json_option: The option to return the json, ex){'cascade': 1}
     :param strict_slash: If not false, the rule url will end with slash
     :param rule_suffix: The upsert suffix, default is 'upsert'
+    :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
     """
     methods = methods or ['POST']
     rule, upsert_rule = _get_route_rule(rule, strict_slash, rule_suffix)
 
-    @app.route(upsert_rule, methods=methods)
+    @app.route(upsert_rule, methods=methods, endpoint=endpoint)
     @rest_permission_required(module, action)
     @gen_route_method('upsert', rule)
     def upsert():
         request_json = request.json
         req_log_data = json.dumps(request_json)
 
         if request_json.get(model.get_primary_field()):
@@ -263,36 +267,37 @@
         res_log_data = get_log_data(res_data)
         log_operation(module, upsert_action, success, req_log_data, res_log_data)
         flaskz_logger.info(get_rest_log_msg('Upsert {} data'.format(model.get_class_name()), req_log_data, success, res_log_data))
 
         return create_response(success, res_data)
 
 
-def register_model_query_route(app, model, rule, module=None, action=None, methods=None, to_json_option=None, strict_slash=True):
+def register_model_query_route(app, model, rule, module=None, action=None, methods=None, to_json_option=None, strict_slash=True, endpoint=None):
     """
     Register query type URL rule for the specified model class to the application/blueprint.
 
     Examples:
         register_model_query_route(api_blueprint, User, 'users', 'users')
 
     :param app: Flask application / Blueprints instance
     :param model: The DB model class, ex)User
     :param rule: The URL rule string, ex)/users
     :param module: The module name for permission check, ex)users
     :param action: The action of the module for permission check, default is None(only check module permission)
     :param methods: The methods of the route, default is ['GET']
     :param to_json_option: The option to return the json, ex){'cascade': 1}
     :param strict_slash: If not false, the rule url will end with slash
+    :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
     :return:
     """
     methods = methods or ['GET']
     rule, did_rule = _get_route_rule(rule, strict_slash)
 
-    @app.route(rule, methods=methods)
-    @app.route(did_rule, methods=methods)
+    @app.route(rule, methods=methods, endpoint=endpoint)
+    @app.route(did_rule, methods=methods, endpoint=endpoint)
     @rest_permission_required(module, action)
     @gen_route_method('query', rule)
     def query(did=None):
         if did is None:
             success, data = model.query_all()
         else:
             try:
@@ -306,15 +311,15 @@
                 success, data = False, res_status_codes.db_query_err
 
         res_data = model_to_dict(data, to_json_option)
         flaskz_logger.debug(get_rest_log_msg('Query {} data'.format(model.get_class_name()), did, success, res_data))
         return create_response(success, res_data)
 
 
-def register_model_query_pss_route(app, model, rule, module=None, action=None, methods=None, to_json_option=None, strict_slash=True, rule_suffix='pss'):
+def register_model_query_pss_route(app, model, rule, module=None, action=None, methods=None, to_json_option=None, strict_slash=True, rule_suffix='pss', endpoint=None):
     """
     Register pss query URL rule for the specified model class to the application/blueprint.
     pss = paging + search + sort
 
     Examples:
         register_model_query_pss_route(api_blueprint, User, 'users', 'users')
 
@@ -323,35 +328,36 @@
     :param rule: The URL rule string, ex)/users
     :param module: The module name for permission check, ex)users
     :param action: The action of the module for permission check, default is None(only check module permission)
     :param methods: The methods of the route, default is ['GET', 'POST']
     :param to_json_option: The option to return the json, ex){'cascade': 1}
     :param strict_slash: If not false, the rule url will end with slash
     :param rule_suffix: The pss suffix, default is 'query_pss'
+    :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
     :return:
     """
     methods = methods or ['GET', 'POST']
     rule, pss_rule = _get_route_rule(rule, strict_slash, rule_suffix)
 
-    @app.route(pss_rule, methods=methods)
+    @app.route(pss_rule, methods=methods, endpoint=endpoint)
     @rest_permission_required(module, action)
     @gen_route_method('query_pss', rule)
     def query_pss():
         request_json = get_request_json({})  # @2023-06-15, request.json --> get_request_json({})
         req_log_data = json.dumps(request_json)
 
         success, data = model.query_pss(parse_pss(model, request_json))
         if success is True:
             data['data'] = model_to_dict(data.get('data', []), to_json_option)
 
         flaskz_logger.debug(get_rest_log_msg('Query pss {} data'.format(model.get_class_name()), req_log_data, success, data))
         return create_response(success, data)
 
 
-def register_models_query_route(app, models, rule, module=None, action=None, methods=None, strict_slash=True, rule_suffix='multi'):
+def register_models_query_route(app, models, rule, module=None, action=None, methods=None, strict_slash=True, rule_suffix='multi', endpoint=None):
     """
     Register query multi models URL rule to the application/blueprint.
     pss = paging + search + sort
 
     Examples:
         register_models_query_route(api_blueprint,
                                  {
@@ -369,27 +375,22 @@
     :param models: The multiple DB model classes,
     :param rule: The URL rule string, ex)/users
     :param module: The module name for permission check, ex)users
     :param action: The action of the module for permission check, default is None(only check module permission)
     :param methods: The methods of the route, default is ['GET', 'POST']
     :param strict_slash: If not false, the rule url will end with slash
     :param rule_suffix: The pss suffix, default is 'multi'
+    :param endpoint: The name of the route endpoint, default is None(use view function name as endpoint name)
 
-    :param rule:
-    :param module:
-    :param action:
-    :param methods:
-    :param strict_slash:
-    :param rule_suffix:
     :return:
     """
     methods = methods or ['GET']
     rule, multi_rule = _get_route_rule(rule, strict_slash, rule_suffix)
 
-    @app.route(multi_rule, methods=methods)
+    @app.route(multi_rule, methods=methods, endpoint=endpoint)
     @rest_permission_required(module, action)
     @gen_route_method('query_multi', rule)
     def query_multi():
         model_cls_list = []
         multi_list = []
         for key in models:
             item = models[key]
```

### Comparing `flaskz-1.6.2/src/flaskz/rest/_mgmt.py` & `flaskz-1.6.3rc1/src/flaskz/rest/_mgmt.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/rest/_util.py` & `flaskz-1.6.3rc1/src/flaskz/rest/_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,26 +113,30 @@
     :return:
     """
     logging_callback = get_current_model_rest_manager_callback('logging_callback')
     if logging_callback:
         logging_callback(*args, **kwargs)
 
 
-def gen_route_method(method, url_prefix):
+def gen_route_method(method, url_prefix, view_func_name=None):
     """
     Generate endpoint unique function name.
     :param method:
     :param url_prefix:
+    :param view_func_name:
     :return:
     """
 
     def decorator(f):
         def wrap(*args, **kwargs):
             return f(*args, **kwargs)
 
-        methods = url_prefix.split('/')
-        methods.append(method)
-        methods.insert(0, 'model_route')
-        wrap.__name__ = '_'.join(filter_list(methods, lambda item: item != '')).replace('-', '_')
+        if view_func_name is None:
+            methods = url_prefix.split('/')
+            methods.append(method)
+            methods.insert(0, 'model_route')
+            wrap.__name__ = '_'.join(filter_list(methods, lambda item: item != '')).replace('-', '_')
+        else:
+            wrap.__name__ = view_func_name
         return wrap
 
     return decorator
```

### Comparing `flaskz-1.6.2/src/flaskz/utils/_app.py` & `flaskz-1.6.3rc1/src/flaskz/utils/_app.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/utils/_cache.py` & `flaskz-1.6.3rc1/src/flaskz/utils/_cache.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/utils/_cls.py` & `flaskz-1.6.3rc1/src/flaskz/utils/_cls.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/utils/_common.py` & `flaskz-1.6.3rc1/src/flaskz/utils/_common.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/utils/_func.py` & `flaskz-1.6.3rc1/src/flaskz/utils/_func.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/utils/_magic.py` & `flaskz-1.6.3rc1/src/flaskz/utils/_magic.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/utils/_request_api.py` & `flaskz-1.6.3rc1/src/flaskz/utils/_request_api.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/utils/_request_args.py` & `flaskz-1.6.3rc1/src/flaskz/utils/_request_args.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/utils/_response.py` & `flaskz-1.6.3rc1/src/flaskz/utils/_response.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz/utils/_timer.py` & `flaskz-1.6.3rc1/src/flaskz/utils/_timer.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.2/src/flaskz.egg-info/PKG-INFO` & `flaskz-1.6.3rc1/src/flaskz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.6.2
+Version: 1.6.3rc1
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,14 +25,16 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.6.3rc1** `2023/08/03`
+    - [A] `flaskz.rest.register_model_*`路由生成函数添加路由`endpoint`参数
 - **1.6.2** `2023/07/06`
     - [F] 修复`flaskz.utils._request_args.py`中`import parse_pss as get_pss`的导入问题
 - **1.6.1** `2023/07/01`
     - [C] `flaskz.utils.get_pss`(`flaskz.models.parse_pss`)函数返回项由SQL字符串拼接改为参数化模式以预防SQL注入
     - [A] 添加`flaskz.utils.run_at`函数用于执行定时函数
 - **1.6** `2023/06/16`
     - [A] `BaseModelMixin`添加`count`方法, 用于数量查询(全量/条件)
```

### Comparing `flaskz-1.6.2/src/flaskz.egg-info/SOURCES.txt` & `flaskz-1.6.3rc1/src/flaskz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

