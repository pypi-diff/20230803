# Comparing `tmp/pip-setting-1.0.0.tar.gz` & `tmp/pip-setting-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-setting-1.0.0.tar", last modified: Wed May 17 13:25:07 2023, max compression
+gzip compressed data, was "pip-setting-1.0.1.tar", last modified: Thu Aug  3 08:23:45 2023, max compression
```

## Comparing `pip-setting-1.0.0.tar` & `pip-setting-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 qiujiajin   (501) staff       (20)        0 2023-05-17 13:25:07.046181 pip-setting-1.0.0/
--rw-r--r--   0 qiujiajin   (501) staff       (20)     1061 2023-05-17 13:21:18.000000 pip-setting-1.0.0/LICENSE
--rw-r--r--   0 qiujiajin   (501) staff       (20)      810 2023-05-17 13:25:07.045975 pip-setting-1.0.0/PKG-INFO
--rw-r--r--   0 qiujiajin   (501) staff       (20)      399 2023-05-17 13:23:12.000000 pip-setting-1.0.0/README.md
-drwxr-xr-x   0 qiujiajin   (501) staff       (20)        0 2023-05-17 13:25:07.044472 pip-setting-1.0.0/pip_setting/
--rw-r--r--   0 qiujiajin   (501) staff       (20)     1540 2023-05-17 13:21:18.000000 pip-setting-1.0.0/pip_setting/__init__.py
--rw-r--r--   0 qiujiajin   (501) staff       (20)      775 2023-05-17 13:21:18.000000 pip-setting-1.0.0/pip_setting/mirrors.json
-drwxr-xr-x   0 qiujiajin   (501) staff       (20)        0 2023-05-17 13:25:07.045570 pip-setting-1.0.0/pip_setting.egg-info/
--rw-r--r--   0 qiujiajin   (501) staff       (20)      810 2023-05-17 13:25:07.000000 pip-setting-1.0.0/pip_setting.egg-info/PKG-INFO
--rw-r--r--   0 qiujiajin   (501) staff       (20)      253 2023-05-17 13:25:07.000000 pip-setting-1.0.0/pip_setting.egg-info/SOURCES.txt
--rw-r--r--   0 qiujiajin   (501) staff       (20)        1 2023-05-17 13:25:07.000000 pip-setting-1.0.0/pip_setting.egg-info/dependency_links.txt
--rw-r--r--   0 qiujiajin   (501) staff       (20)       78 2023-05-17 13:25:07.000000 pip-setting-1.0.0/pip_setting.egg-info/entry_points.txt
--rw-r--r--   0 qiujiajin   (501) staff       (20)       12 2023-05-17 13:25:07.000000 pip-setting-1.0.0/pip_setting.egg-info/top_level.txt
--rw-r--r--   0 qiujiajin   (501) staff       (20)       38 2023-05-17 13:25:07.046276 pip-setting-1.0.0/setup.cfg
--rw-r--r--   0 qiujiajin   (501) staff       (20)      926 2023-05-17 13:23:26.000000 pip-setting-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:23:45.765025 pip-setting-1.0.1/
+-rw-rw-rw-   0        0        0     1082 2023-08-03 07:57:28.000000 pip-setting-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      832 2023-08-03 08:23:45.764022 pip-setting-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-08-03 07:57:28.000000 pip-setting-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 08:23:45.739522 pip-setting-1.0.1/pip_setting/
+-rw-rw-rw-   0        0        0     1526 2023-08-03 08:00:22.000000 pip-setting-1.0.1/pip_setting/__init__.py
+-rw-rw-rw-   0        0        0      955 2023-08-03 08:20:18.000000 pip-setting-1.0.1/pip_setting/mirrors.json
+drwxrwxrwx   0        0        0        0 2023-08-03 08:23:45.760004 pip-setting-1.0.1/pip_setting.egg-info/
+-rw-rw-rw-   0        0        0      832 2023-08-03 08:23:45.000000 pip-setting-1.0.1/pip_setting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-08-03 08:23:45.000000 pip-setting-1.0.1/pip_setting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 08:23:45.000000 pip-setting-1.0.1/pip_setting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-08-03 08:23:45.000000 pip-setting-1.0.1/pip_setting.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2023-08-03 08:23:45.000000 pip-setting-1.0.1/pip_setting.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 08:23:45.765025 pip-setting-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      896 2023-08-03 08:00:25.000000 pip-setting-1.0.1/setup.py
```

### Comparing `pip-setting-1.0.0/PKG-INFO` & `pip-setting-1.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1
-Name: pip-setting
-Version: 1.0.0
-Summary: 快速设置pip镜像源的工具
-Home-page: https://github.com/13528080556/pip_setting
-Author: 丘家劲
-Author-email: 609799548@qq.com
-License: MIT Licence
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# 设置 pip 镜像源
-
-这是设置国内镜像源的工具，可以使用它快速切换镜像源地址。
-目前支持
-- 官方源
-- 阿里云源
-- 清华源
-- 豆瓣源
-- 腾讯云源
-- 上海交大
-
-#### 方式 1
-```
-命令行直接输入: pip-setting , 根据提示继续操作
-```
-
-#### 方式 2
-命令行输入
-- pip-setting -s 阿里云
-- pip-setting --source 阿里云
+Metadata-Version: 2.1
+Name: pip-setting
+Version: 1.0.1
+Summary: 快速设置pip镜像源的工具
+Home-page: https://github.com/qq1u/pip_setting
+Author: Hugh
+Author-email: 609799548@qq.com
+License: MIT Licence
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# 设置 pip 镜像源
+
+这是设置国内镜像源的工具，可以使用它快速切换镜像源地址。
+目前支持
+- 官方源
+- 阿里云源
+- 清华源
+- 豆瓣源
+- 腾讯云源
+- 上海交大
+
+#### 方式 1
+```
+命令行直接输入: pip-setting , 根据提示继续操作
+```
+
+#### 方式 2
+命令行输入
+- pip-setting -s 阿里云
+- pip-setting --source 阿里云
```

### Comparing `pip-setting-1.0.0/pip_setting/mirrors.json` & `pip-setting-1.0.1/pip_setting/mirrors.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7291666666666666%*

 * *Differences: {"'上海交大'": "{'global': 'index-url=https://mirror.sjtu.edu.cn/pypi/web/simple'}",*

 * * "'华为云'": "OrderedDict([('global', "*

 * *          "'index-url=https://repo.huaweicloud.com/repository/pypi/simple'), ('install', "*

 * *          "'trusted-host=repo.huaweicloud.com')])",*

 * * "'清华'": "{'global': 'index-url=https://pypi.tuna.tsinghua.edu.cn/simple'}",*

 * * "'腾讯云'": "{'global': 'index-url=https://mirrors.cloud.tencent.com/pypi/simple'}",*

 * * "'豆瓣'": "{'global': 'index-url=https://pypi.doubanio.com/simple'}",*

 * * "'阿里云'": "{'global':  […]*

```diff
@@ -1,22 +1,26 @@
 {
     "\u4e0a\u6d77\u4ea4\u5927": {
-        "global": "index-url = https://mirror.sjtu.edu.cn/pypi/web/simple",
+        "global": "index-url=https://mirror.sjtu.edu.cn/pypi/web/simple",
         "install": "trusted-host=mirror.sjtu.edu.cn"
     },
+    "\u534e\u4e3a\u4e91": {
+        "global": "index-url=https://repo.huaweicloud.com/repository/pypi/simple",
+        "install": "trusted-host=repo.huaweicloud.com"
+    },
     "\u6e05\u534e": {
-        "global": "index-url = https://pypi.tuna.tsinghua.edu.cn/simple",
+        "global": "index-url=https://pypi.tuna.tsinghua.edu.cn/simple",
         "install": "trusted-host=pypi.tuna.tsinghua.edu.cn"
     },
     "\u817e\u8baf\u4e91": {
-        "global": "index-url = https://mirrors.cloud.tencent.com/pypi/simple",
+        "global": "index-url=https://mirrors.cloud.tencent.com/pypi/simple",
         "install": "trusted-host=mirrors.cloud.tencent.com"
     },
     "\u8c46\u74e3": {
-        "global": "index-url = https://pypi.doubanio.com/simple",
+        "global": "index-url=https://pypi.doubanio.com/simple",
         "install": "trusted-host=pypi.doubanio.com"
     },
     "\u963f\u91cc\u4e91": {
-        "global": "index-url = https://mirrors.aliyun.com/pypi/simple",
+        "global": "index-url=https://mirrors.aliyun.com/pypi/simple",
         "install": "trusted-host=mirrors.aliyun.com"
     }
 }
```

### Comparing `pip-setting-1.0.0/pip_setting.egg-info/PKG-INFO` & `pip-setting-1.0.1/pip_setting.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1
-Name: pip-setting
-Version: 1.0.0
-Summary: 快速设置pip镜像源的工具
-Home-page: https://github.com/13528080556/pip_setting
-Author: 丘家劲
-Author-email: 609799548@qq.com
-License: MIT Licence
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# 设置 pip 镜像源
-
-这是设置国内镜像源的工具，可以使用它快速切换镜像源地址。
-目前支持
-- 官方源
-- 阿里云源
-- 清华源
-- 豆瓣源
-- 腾讯云源
-- 上海交大
-
-#### 方式 1
-```
-命令行直接输入: pip-setting , 根据提示继续操作
-```
-
-#### 方式 2
-命令行输入
-- pip-setting -s 阿里云
-- pip-setting --source 阿里云
+Metadata-Version: 2.1
+Name: pip-setting
+Version: 1.0.1
+Summary: 快速设置pip镜像源的工具
+Home-page: https://github.com/qq1u/pip_setting
+Author: Hugh
+Author-email: 609799548@qq.com
+License: MIT Licence
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# 设置 pip 镜像源
+
+这是设置国内镜像源的工具，可以使用它快速切换镜像源地址。
+目前支持
+- 官方源
+- 阿里云源
+- 清华源
+- 豆瓣源
+- 腾讯云源
+- 上海交大
+
+#### 方式 1
+```
+命令行直接输入: pip-setting , 根据提示继续操作
+```
+
+#### 方式 2
+命令行输入
+- pip-setting -s 阿里云
+- pip-setting --source 阿里云
```

