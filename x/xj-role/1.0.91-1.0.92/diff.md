# Comparing `tmp/xj_role-1.0.91.tar.gz` & `tmp/xj_role-1.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xj_role-1.0.91.tar", last modified: Wed Aug  2 08:20:59 2023, max compression
+gzip compressed data, was "xj_role-1.0.92.tar", last modified: Thu Aug  3 08:26:08 2023, max compression
```

## Comparing `xj_role-1.0.91.tar` & `xj_role-1.0.92.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 08:20:59.994717 xj_role-1.0.91/
--rw-rw-rw-   0        0        0      354 2023-08-02 08:20:59.993716 xj_role-1.0.91/PKG-INFO
--rw-rw-rw-   0        0        0      212 2022-09-02 08:12:19.000000 xj_role-1.0.91/README.md
--rw-rw-rw-   0        0        0       42 2023-08-02 08:20:59.994717 xj_role-1.0.91/setup.cfg
--rw-rw-rw-   0        0        0     1956 2023-08-02 08:15:16.000000 xj_role-1.0.91/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:20:59.839302 xj_role-1.0.91/xj_role/
--rw-rw-rw-   0        0        0        0 2022-09-02 08:12:19.000000 xj_role-1.0.91/xj_role/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/admin.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:20:59.876149 xj_role-1.0.91/xj_role/apis/
--rw-rw-rw-   0        0        0        0 2022-09-02 08:12:19.000000 xj_role-1.0.91/xj_role/apis/__init__.py
--rw-rw-rw-   0        0        0     7074 2023-07-20 02:20:21.000000 xj_role-1.0.91/xj_role/apis/group_api.py
--rw-rw-rw-   0        0        0     3879 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/apis/permission_api.py
--rw-rw-rw-   0        0        0     4549 2023-07-20 02:20:21.000000 xj_role-1.0.91/xj_role/apis/role_api.py
--rw-rw-rw-   0        0        0     3638 2023-07-13 00:57:44.000000 xj_role-1.0.91/xj_role/apis/role_menu_apis.py
--rw-rw-rw-   0        0        0     2162 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/apis/role_system_apis.py
--rw-rw-rw-   0        0        0      202 2022-09-06 08:07:54.000000 xj_role-1.0.91/xj_role/apps.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:20:59.891863 xj_role-1.0.91/xj_role/library/
--rw-rw-rw-   0        0        0      149 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/library/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:20:59.901375 xj_role-1.0.91/xj_role/library/api_interrupter/
--rw-rw-rw-   0        0        0      158 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/library/api_interrupter/__init__.py
--rw-rw-rw-   0        0        0     5573 2023-07-20 02:20:21.000000 xj_role-1.0.91/xj_role/library/api_interrupter/api_interrupter.py
--rw-rw-rw-   0        0        0      973 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/library/api_interrupter/api_interrupter_middleware.py
--rw-rw-rw-   0        0        0     4659 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/library/get_system_apis.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:20:59.906903 xj_role-1.0.91/xj_role/library/permission_execute/
--rw-rw-rw-   0        0        0      238 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/library/permission_execute/__init__.py
--rw-rw-rw-   0        0        0      292 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/library/permission_execute/permission_base.py
--rw-rw-rw-   0        0        0      280 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/library/permission_execute/permission_executor.py
--rw-rw-rw-   0        0        0    10442 2023-08-02 08:00:30.000000 xj_role-1.0.91/xj_role/models.py
--rw-rw-rw-   0        0        0     1091 2023-05-12 03:24:05.000000 xj_role-1.0.91/xj_role/service_register.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:20:59.926651 xj_role-1.0.91/xj_role/services/
--rw-rw-rw-   0        0        0        0 2022-09-02 08:12:19.000000 xj_role-1.0.91/xj_role/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:20:59.967210 xj_role-1.0.91/xj_role/services/abstract/
--rw-rw-rw-   0        0        0      168 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/services/abstract/__init__.py
--rw-rw-rw-   0        0        0      767 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/services/abstract/observer_subject.py
--rw-rw-rw-   0        0        0     6264 2022-10-18 05:55:19.000000 xj_role-1.0.91/xj_role/services/auto_permission_service.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:20:59.969208 xj_role-1.0.91/xj_role/services/observer/
--rw-rw-rw-   0        0        0      321 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/services/observer/__init__.py
--rw-rw-rw-   0        0        0    17658 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/services/permission_service.py
--rw-rw-rw-   0        0        0     6454 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/services/role_apis_services.py
--rw-rw-rw-   0        0        0    10049 2023-07-27 01:05:50.000000 xj_role-1.0.91/xj_role/services/role_nemus_services.py
--rw-rw-rw-   0        0        0    23254 2023-07-20 02:20:21.000000 xj_role-1.0.91/xj_role/services/role_service.py
--rw-rw-rw-   0        0        0    12667 2022-10-10 01:30:46.000000 xj_role-1.0.91/xj_role/services/user_group_service [backup].py
--rw-rw-rw-   0        0        0    24336 2023-08-02 08:14:38.000000 xj_role-1.0.91/xj_role/services/user_group_service.py
--rw-rw-rw-   0        0        0     3634 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/urls.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:20:59.989727 xj_role-1.0.91/xj_role/utils/
--rw-rw-rw-   0        0        0        0 2022-09-02 08:12:19.000000 xj_role-1.0.91/xj_role/utils/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/utils/api_interrupter_wrapper.py
--rw-rw-rw-   0        0        0     1082 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/utils/custom_authorization.py
--rw-rw-rw-   0        0        0     4618 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/utils/custom_response.py
--rw-rw-rw-   0        0        0    39226 2023-07-20 02:20:21.000000 xj_role-1.0.91/xj_role/utils/custom_tool.py
--rw-rw-rw-   0        0        0      958 2022-10-17 09:29:18.000000 xj_role-1.0.91/xj_role/utils/j_dict.py
--rw-rw-rw-   0        0        0    10256 2023-07-20 02:20:21.000000 xj_role-1.0.91/xj_role/utils/j_recur.py
--rw-rw-rw-   0        0        0      660 2023-05-12 03:24:05.000000 xj_role-1.0.91/xj_role/utils/join_list.py
--rw-rw-rw-   0        0        0     2691 2023-07-12 06:37:35.000000 xj_role-1.0.91/xj_role/utils/omnipotence_wrapper.py
--rw-rw-rw-   0        0        0     5867 2023-07-20 02:20:21.000000 xj_role-1.0.91/xj_role/utils/user_wrapper.py
--rw-rw-rw-   0        0        0     2682 2022-09-02 08:12:19.000000 xj_role-1.0.91/xj_role/utils/validator.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:20:59.849062 xj_role-1.0.91/xj_role.egg-info/
--rw-rw-rw-   0        0        0      354 2023-08-02 08:20:59.000000 xj_role-1.0.91/xj_role.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1577 2023-08-02 08:20:59.000000 xj_role-1.0.91/xj_role.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 08:20:59.000000 xj_role-1.0.91/xj_role.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 08:20:59.000000 xj_role-1.0.91/xj_role.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.162714 xj_role-1.0.92/
+-rw-rw-rw-   0        0        0      354 2023-08-03 08:26:08.161716 xj_role-1.0.92/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2022-09-02 08:12:19.000000 xj_role-1.0.92/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 08:26:08.162714 xj_role-1.0.92/setup.cfg
+-rw-rw-rw-   0        0        0     1956 2023-08-03 08:25:02.000000 xj_role-1.0.92/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.098468 xj_role-1.0.92/xj_role/
+-rw-rw-rw-   0        0        0        0 2022-09-02 08:12:19.000000 xj_role-1.0.92/xj_role/__init__.py
+-rw-rw-rw-   0        0        0     2912 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/admin.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.111954 xj_role-1.0.92/xj_role/apis/
+-rw-rw-rw-   0        0        0        0 2022-09-02 08:12:19.000000 xj_role-1.0.92/xj_role/apis/__init__.py
+-rw-rw-rw-   0        0        0     7074 2023-07-20 02:20:21.000000 xj_role-1.0.92/xj_role/apis/group_api.py
+-rw-rw-rw-   0        0        0     3879 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/apis/permission_api.py
+-rw-rw-rw-   0        0        0     4549 2023-07-20 02:20:21.000000 xj_role-1.0.92/xj_role/apis/role_api.py
+-rw-rw-rw-   0        0        0     3638 2023-07-13 00:57:44.000000 xj_role-1.0.92/xj_role/apis/role_menu_apis.py
+-rw-rw-rw-   0        0        0     2162 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/apis/role_system_apis.py
+-rw-rw-rw-   0        0        0      202 2022-09-06 08:07:54.000000 xj_role-1.0.92/xj_role/apps.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.115574 xj_role-1.0.92/xj_role/library/
+-rw-rw-rw-   0        0        0      149 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/library/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.120549 xj_role-1.0.92/xj_role/library/api_interrupter/
+-rw-rw-rw-   0        0        0      158 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/library/api_interrupter/__init__.py
+-rw-rw-rw-   0        0        0     5573 2023-07-20 02:20:21.000000 xj_role-1.0.92/xj_role/library/api_interrupter/api_interrupter.py
+-rw-rw-rw-   0        0        0      973 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/library/api_interrupter/api_interrupter_middleware.py
+-rw-rw-rw-   0        0        0     4659 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/library/get_system_apis.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.124807 xj_role-1.0.92/xj_role/library/permission_execute/
+-rw-rw-rw-   0        0        0      238 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/library/permission_execute/__init__.py
+-rw-rw-rw-   0        0        0      292 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/library/permission_execute/permission_base.py
+-rw-rw-rw-   0        0        0      280 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/library/permission_execute/permission_executor.py
+-rw-rw-rw-   0        0        0    10442 2023-08-02 08:00:30.000000 xj_role-1.0.92/xj_role/models.py
+-rw-rw-rw-   0        0        0     1091 2023-05-12 03:24:05.000000 xj_role-1.0.92/xj_role/service_register.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.136802 xj_role-1.0.92/xj_role/services/
+-rw-rw-rw-   0        0        0        0 2022-09-02 08:12:19.000000 xj_role-1.0.92/xj_role/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.139820 xj_role-1.0.92/xj_role/services/abstract/
+-rw-rw-rw-   0        0        0      168 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/services/abstract/__init__.py
+-rw-rw-rw-   0        0        0      767 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/services/abstract/observer_subject.py
+-rw-rw-rw-   0        0        0     6264 2022-10-18 05:55:19.000000 xj_role-1.0.92/xj_role/services/auto_permission_service.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.140817 xj_role-1.0.92/xj_role/services/observer/
+-rw-rw-rw-   0        0        0      321 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/services/observer/__init__.py
+-rw-rw-rw-   0        0        0    17658 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/services/permission_service.py
+-rw-rw-rw-   0        0        0     6454 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/services/role_apis_services.py
+-rw-rw-rw-   0        0        0    10049 2023-07-27 01:05:50.000000 xj_role-1.0.92/xj_role/services/role_nemus_services.py
+-rw-rw-rw-   0        0        0    23254 2023-07-20 02:20:21.000000 xj_role-1.0.92/xj_role/services/role_service.py
+-rw-rw-rw-   0        0        0    12667 2022-10-10 01:30:46.000000 xj_role-1.0.92/xj_role/services/user_group_service [backup].py
+-rw-rw-rw-   0        0        0    24433 2023-08-03 08:23:47.000000 xj_role-1.0.92/xj_role/services/user_group_service.py
+-rw-rw-rw-   0        0        0     3634 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/urls.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.159721 xj_role-1.0.92/xj_role/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-02 08:12:19.000000 xj_role-1.0.92/xj_role/utils/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/utils/api_interrupter_wrapper.py
+-rw-rw-rw-   0        0        0     1082 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/utils/custom_authorization.py
+-rw-rw-rw-   0        0        0     4618 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/utils/custom_response.py
+-rw-rw-rw-   0        0        0    39226 2023-07-20 02:20:21.000000 xj_role-1.0.92/xj_role/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      958 2022-10-17 09:29:18.000000 xj_role-1.0.92/xj_role/utils/j_dict.py
+-rw-rw-rw-   0        0        0    10256 2023-07-20 02:20:21.000000 xj_role-1.0.92/xj_role/utils/j_recur.py
+-rw-rw-rw-   0        0        0      660 2023-05-12 03:24:05.000000 xj_role-1.0.92/xj_role/utils/join_list.py
+-rw-rw-rw-   0        0        0     2691 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/utils/omnipotence_wrapper.py
+-rw-rw-rw-   0        0        0     5867 2023-07-20 02:20:21.000000 xj_role-1.0.92/xj_role/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     2682 2022-09-02 08:12:19.000000 xj_role-1.0.92/xj_role/utils/validator.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.103595 xj_role-1.0.92/xj_role.egg-info/
+-rw-rw-rw-   0        0        0      354 2023-08-03 08:26:07.000000 xj_role-1.0.92/xj_role.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1577 2023-08-03 08:26:08.000000 xj_role-1.0.92/xj_role.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 08:26:07.000000 xj_role-1.0.92/xj_role.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-03 08:26:07.000000 xj_role-1.0.92/xj_role.egg-info/top_level.txt
```

### Comparing `xj_role-1.0.91/setup.py` & `xj_role-1.0.92/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_role',  # 模块名称
-    version='1.0.91',  # 模块版本
+    version='1.0.92',  # 模块版本
     description='权限模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     # author='sieyoo',
     # author_email='sieyoo@163.com',
     packages=find_packages(),  # 系统自动从当前目录开始找包
     # packages=['xj_user'],  # 系指定安装模块
```

### Comparing `xj_role-1.0.91/xj_role/admin.py` & `xj_role-1.0.92/xj_role/admin.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/apis/group_api.py` & `xj_role-1.0.92/xj_role/apis/group_api.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/apis/permission_api.py` & `xj_role-1.0.92/xj_role/apis/permission_api.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/apis/role_api.py` & `xj_role-1.0.92/xj_role/apis/role_api.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/apis/role_menu_apis.py` & `xj_role-1.0.92/xj_role/apis/role_menu_apis.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/apis/role_system_apis.py` & `xj_role-1.0.92/xj_role/apis/role_system_apis.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/library/api_interrupter/api_interrupter.py` & `xj_role-1.0.92/xj_role/library/api_interrupter/api_interrupter.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/library/api_interrupter/api_interrupter_middleware.py` & `xj_role-1.0.92/xj_role/library/api_interrupter/api_interrupter_middleware.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/library/get_system_apis.py` & `xj_role-1.0.92/xj_role/library/get_system_apis.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/models.py` & `xj_role-1.0.92/xj_role/models.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/service_register.py` & `xj_role-1.0.92/xj_role/service_register.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/services/abstract/observer_subject.py` & `xj_role-1.0.92/xj_role/services/abstract/observer_subject.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/services/auto_permission_service.py` & `xj_role-1.0.92/xj_role/services/auto_permission_service.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/services/permission_service.py` & `xj_role-1.0.92/xj_role/services/permission_service.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/services/role_apis_services.py` & `xj_role-1.0.92/xj_role/services/role_apis_services.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/services/role_nemus_services.py` & `xj_role-1.0.92/xj_role/services/role_nemus_services.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/services/role_service.py` & `xj_role-1.0.92/xj_role/services/role_service.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/services/user_group_service [backup].py` & `xj_role-1.0.92/xj_role/services/user_group_service [backup].py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/services/user_group_service.py` & `xj_role-1.0.92/xj_role/services/user_group_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,16 +79,18 @@
         params = format_params_handle(
             param_dict=params,
             filter_filed_list=["id", "group", "group_name", "parent_group_id", "description"]
         )
         id = params.pop("id", None)
         if not id:
             return None, "ID 不可以为空"
-        instance = RoleUserGroup.objects.filter(id=id).first().to_json()
-
+        instance = RoleUserGroup.objects.filter(id=id).first()
+        if not instance:
+            return None, "分组不存在"
+        instance = instance.to_json()
         return instance, None
 
     @staticmethod
     def del_group(id: int):
         """
         删除用户的分组
         :param id: 分组的主键ID
```

### Comparing `xj_role-1.0.91/xj_role/urls.py` & `xj_role-1.0.92/xj_role/urls.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/utils/api_interrupter_wrapper.py` & `xj_role-1.0.92/xj_role/utils/api_interrupter_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/utils/custom_authorization.py` & `xj_role-1.0.92/xj_role/utils/custom_authorization.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/utils/custom_response.py` & `xj_role-1.0.92/xj_role/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/utils/custom_tool.py` & `xj_role-1.0.92/xj_role/utils/custom_tool.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/utils/j_dict.py` & `xj_role-1.0.92/xj_role/utils/j_dict.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/utils/j_recur.py` & `xj_role-1.0.92/xj_role/utils/j_recur.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/utils/join_list.py` & `xj_role-1.0.92/xj_role/utils/join_list.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/utils/omnipotence_wrapper.py` & `xj_role-1.0.92/xj_role/utils/omnipotence_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/utils/user_wrapper.py` & `xj_role-1.0.92/xj_role/utils/user_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role/utils/validator.py` & `xj_role-1.0.92/xj_role/utils/validator.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.91/xj_role.egg-info/SOURCES.txt` & `xj_role-1.0.92/xj_role.egg-info/SOURCES.txt`

 * *Files identical despite different names*

