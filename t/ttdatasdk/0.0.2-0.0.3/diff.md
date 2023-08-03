# Comparing `tmp/ttdatasdk-0.0.2.tar.gz` & `tmp/ttdatasdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttdatasdk-0.0.2.tar", last modified: Sat Jul 29 03:09:11 2023, max compression
+gzip compressed data, was "ttdatasdk-0.0.3.tar", last modified: Thu Aug  3 02:55:52 2023, max compression
```

## Comparing `ttdatasdk-0.0.2.tar` & `ttdatasdk-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 03:09:11.709060 ttdatasdk-0.0.2/
--rw-rw-rw-   0        0        0    11558 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3389 2023-07-29 03:09:11.709060 ttdatasdk-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2650 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-29 03:09:11.709060 ttdatasdk-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2004 2023-07-29 03:08:45.000000 ttdatasdk-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:09:11.695061 ttdatasdk-0.0.2/tests/
--rw-rw-rw-   0        0        0      573 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/tests/test_requirements.py
--rw-rw-rw-   0        0        0     2086 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/tests/test_thrift_client.py
--rw-rw-rw-   0        0        0     1820 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/tests/test_ttdatasdk.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:09:11.699060 ttdatasdk-0.0.2/ttdatasdk/
--rw-rw-rw-   0        0        0     1128 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/ttdatasdk/__init__.py
--rw-rw-rw-   0        0        0     5390 2023-07-29 01:45:45.000000 ttdatasdk-0.0.2/ttdatasdk/api.py
--rw-rw-rw-   0        0        0     9944 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/ttdatasdk/client.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:09:11.708060 ttdatasdk-0.0.2/ttdatasdk/compat/
--rw-rw-rw-   0        0        0        0 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/ttdatasdk/compat/__init__.py
--rw-rw-rw-   0        0        0     2187 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/ttdatasdk/compat/pickle_compat.py
--rw-rw-rw-   0        0        0      175 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/ttdatasdk/exceptions.py
--rw-rw-rw-   0        0        0      793 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/ttdatasdk/thrift_client.py
--rw-rw-rw-   0        0        0      587 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/ttdatasdk/utils.py
--rw-rw-rw-   0        0        0      437 2023-07-29 03:08:45.000000 ttdatasdk-0.0.2/ttdatasdk/version.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:09:11.707061 ttdatasdk-0.0.2/ttdatasdk.egg-info/
--rw-rw-rw-   0        0        0     3389 2023-07-29 03:09:11.000000 ttdatasdk-0.0.2/ttdatasdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2023-07-29 03:09:11.000000 ttdatasdk-0.0.2/ttdatasdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 03:09:11.000000 ttdatasdk-0.0.2/ttdatasdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 03:09:11.000000 ttdatasdk-0.0.2/ttdatasdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      118 2023-07-29 03:09:11.000000 ttdatasdk-0.0.2/ttdatasdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 03:09:11.000000 ttdatasdk-0.0.2/ttdatasdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 02:55:52.138834 ttdatasdk-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-07-09 16:17:28.000000 ttdatasdk-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3485 2023-08-03 02:55:52.137833 ttdatasdk-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2743 2023-07-29 03:19:16.000000 ttdatasdk-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 02:55:52.138834 ttdatasdk-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2004 2023-08-03 02:52:30.000000 ttdatasdk-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 02:55:52.126833 ttdatasdk-0.0.3/tests/
+-rw-rw-rw-   0        0        0      464 2023-08-03 02:44:09.000000 ttdatasdk-0.0.3/tests/test_get_index_market_data.py
+-rw-rw-rw-   0        0        0      573 2023-07-09 16:17:28.000000 ttdatasdk-0.0.3/tests/test_requirements.py
+-rw-rw-rw-   0        0        0     2086 2023-07-09 16:17:28.000000 ttdatasdk-0.0.3/tests/test_thrift_client.py
+-rw-rw-rw-   0        0        0     2037 2023-08-02 12:17:33.000000 ttdatasdk-0.0.3/tests/test_ttdatasdk.py
+drwxrwxrwx   0        0        0        0 2023-08-03 02:55:52.130833 ttdatasdk-0.0.3/ttdatasdk/
+-rw-rw-rw-   0        0        0     1128 2023-07-09 16:17:28.000000 ttdatasdk-0.0.3/ttdatasdk/__init__.py
+-rw-rw-rw-   0        0        0    10456 2023-08-02 12:17:00.000000 ttdatasdk-0.0.3/ttdatasdk/api.py
+-rw-rw-rw-   0        0        0     9944 2023-07-09 16:17:28.000000 ttdatasdk-0.0.3/ttdatasdk/client.py
+drwxrwxrwx   0        0        0        0 2023-08-03 02:55:52.137833 ttdatasdk-0.0.3/ttdatasdk/compat/
+-rw-rw-rw-   0        0        0        0 2023-07-09 16:17:28.000000 ttdatasdk-0.0.3/ttdatasdk/compat/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-07-09 16:17:28.000000 ttdatasdk-0.0.3/ttdatasdk/compat/pickle_compat.py
+-rw-rw-rw-   0        0        0      175 2023-07-09 16:17:28.000000 ttdatasdk-0.0.3/ttdatasdk/exceptions.py
+-rw-rw-rw-   0        0        0      793 2023-07-09 16:17:28.000000 ttdatasdk-0.0.3/ttdatasdk/thrift_client.py
+-rw-rw-rw-   0        0        0      587 2023-07-09 16:17:28.000000 ttdatasdk-0.0.3/ttdatasdk/utils.py
+-rw-rw-rw-   0        0        0      437 2023-08-03 02:52:30.000000 ttdatasdk-0.0.3/ttdatasdk/version.py
+drwxrwxrwx   0        0        0        0 2023-08-03 02:55:52.136833 ttdatasdk-0.0.3/ttdatasdk.egg-info/
+-rw-rw-rw-   0        0        0     3485 2023-08-03 02:55:52.000000 ttdatasdk-0.0.3/ttdatasdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-08-03 02:55:52.000000 ttdatasdk-0.0.3/ttdatasdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 02:55:52.000000 ttdatasdk-0.0.3/ttdatasdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-03 02:55:52.000000 ttdatasdk-0.0.3/ttdatasdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      118 2023-08-03 02:55:52.000000 ttdatasdk-0.0.3/ttdatasdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-03 02:55:52.000000 ttdatasdk-0.0.3/ttdatasdk.egg-info/top_level.txt
```

### Comparing `ttdatasdk-0.0.2/LICENSE` & `ttdatasdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.2/PKG-INFO` & `ttdatasdk-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttdatasdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Ticker Trading Factors data access, Backtest and Trading.
 Home-page: https://www.tickertrading.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 License: Apache License v2
@@ -37,14 +37,17 @@
 ttdatasdk==0.0.1
 
 # 在命令行执行：
 pip install -r requirements.txt
 # 如果安装失败，请指定官方镜像源
 pip install -r requirements.txt -i https://pypi.org/simple
 
+# 安装指定的版本： pip install ttdatasdk==<version>
+pip install ttdatasdk==0.0.2
+
 # 升级版本
 pip install -U ttdatasdk
 # 如果安装失败，请指定官方镜像源
 pip install -U ttdatasdk -i https://pypi.org/simple
 ```
```

### Comparing `ttdatasdk-0.0.2/README.md` & `ttdatasdk-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 ttdatasdk==0.0.1
 
 # 在命令行执行：
 pip install -r requirements.txt
 # 如果安装失败，请指定官方镜像源
 pip install -r requirements.txt -i https://pypi.org/simple
 
+# 安装指定的版本： pip install ttdatasdk==<version>
+pip install ttdatasdk==0.0.2
+
 # 升级版本
 pip install -U ttdatasdk
 # 如果安装失败，请指定官方镜像源
 pip install -U ttdatasdk -i https://pypi.org/simple
 ```
```

### Comparing `ttdatasdk-0.0.2/setup.py` & `ttdatasdk-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 
 THIS_FOLDER = os.path.dirname(os.path.abspath(__file__))
 
 
 def get_version():
     scope = {}
-    version = '0.0.2'
+    version = '0.0.3'
     version_file = os.path.join(THIS_FOLDER, "ttdatasdk", "version.py")
     if os.path.exists(version_file):
         with open(version_file) as fp:
             exec(fp.read(), scope)
-        version = scope.get('__version__', '0.0.2')
+        version = scope.get('__version__', '0.0.3')
     return version
 
 
 def get_long_description():
     with open(os.path.join(THIS_FOLDER, 'README.md'), 'rb') as f:
         long_description = f.read().decode('utf-8')
     return long_description
```

### Comparing `ttdatasdk-0.0.2/tests/test_requirements.py` & `ttdatasdk-0.0.3/tests/test_requirements.py`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.2/tests/test_thrift_client.py` & `ttdatasdk-0.0.3/tests/test_thrift_client.py`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.2/tests/test_ttdatasdk.py` & `ttdatasdk-0.0.3/tests/test_ttdatasdk.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,7 +38,12 @@
 
 
 # 获取历史数据，可查询单个标的多个数据字段
 sec_code = '000001.SZ'
 end_datetime = (current_dt + datetime.timedelta(minutes=-1)).strftime('%Y-%m-%d %H:%M:%S')
 df = ttdatasdk.get_attribute_history(security=sec_code, count=5, unit='1m', end_datetime=end_datetime, fields=['open', 'close'])
 print(df)
+
+# 沪深300分钟行情数据
+factor_list = ['open', 'high', 'low', 'close', 'volume']
+df = ttdatasdk.get_factor(sec_code_list=['000300.SH'], unit='1m', trade_date='2022-12-19', factor_list=factor_list)
+print(df)
```

### Comparing `ttdatasdk-0.0.2/ttdatasdk/__init__.py` & `ttdatasdk-0.0.3/ttdatasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.2/ttdatasdk/client.py` & `ttdatasdk-0.0.3/ttdatasdk/client.py`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.2/ttdatasdk/compat/pickle_compat.py` & `ttdatasdk-0.0.3/ttdatasdk/compat/pickle_compat.py`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.2/ttdatasdk/thrift_client.py` & `ttdatasdk-0.0.3/ttdatasdk/thrift_client.py`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.2/ttdatasdk/utils.py` & `ttdatasdk-0.0.3/ttdatasdk/utils.py`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.2/ttdatasdk.egg-info/PKG-INFO` & `ttdatasdk-0.0.3/ttdatasdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttdatasdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Ticker Trading Factors data access, Backtest and Trading.
 Home-page: https://www.tickertrading.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 License: Apache License v2
@@ -37,14 +37,17 @@
 ttdatasdk==0.0.1
 
 # 在命令行执行：
 pip install -r requirements.txt
 # 如果安装失败，请指定官方镜像源
 pip install -r requirements.txt -i https://pypi.org/simple
 
+# 安装指定的版本： pip install ttdatasdk==<version>
+pip install ttdatasdk==0.0.2
+
 # 升级版本
 pip install -U ttdatasdk
 # 如果安装失败，请指定官方镜像源
 pip install -U ttdatasdk -i https://pypi.org/simple
 ```
```

### Comparing `ttdatasdk-0.0.2/ttdatasdk.egg-info/SOURCES.txt` & `ttdatasdk-0.0.3/ttdatasdk.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 setup.py
+tests/test_get_index_market_data.py
 tests/test_requirements.py
 tests/test_thrift_client.py
 tests/test_ttdatasdk.py
 ttdatasdk/__init__.py
 ttdatasdk/api.py
 ttdatasdk/client.py
 ttdatasdk/exceptions.py
```

