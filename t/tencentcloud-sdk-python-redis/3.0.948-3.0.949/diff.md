# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.948.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.949.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.948.tar", last modified: Wed Aug  2 00:35:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.949.tar", last modified: Thu Aug  3 00:31:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.948.tar` & `tencentcloud-sdk-python-redis-3.0.949.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/
--rw-r--r--   0 root         (0) root         (0)     1076 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      517 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud_sdk_python_redis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud_sdk_python_redis.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud/redis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)    87721 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   467524 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-08-02 00:35:40.000000 tencentcloud-sdk-python-redis-3.0.948/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:31:50.000000 tencentcloud-sdk-python-redis-3.0.949/
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-08-03 00:31:46.000000 tencentcloud-sdk-python-redis-3.0.949/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:31:50.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:31:49.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      517 2023-08-03 00:31:49.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-03 00:31:49.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud_sdk_python_redis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-08-03 00:31:49.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 00:31:49.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:31:50.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-03 00:31:46.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:31:50.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:31:46.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud/redis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:31:50.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:31:46.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    87874 2023-08-03 00:31:46.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-08-03 00:31:46.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   467550 2023-08-03 00:31:46.000000 tencentcloud-sdk-python-redis-3.0.949/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-03 00:31:50.000000 tencentcloud-sdk-python-redis-3.0.949/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-08-03 00:31:50.000000 tencentcloud-sdk-python-redis-3.0.949/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-08-03 00:31:46.000000 tencentcloud-sdk-python-redis-3.0.949/README.rst
```

### Comparing `tencentcloud-sdk-python-redis-3.0.948/setup.py` & `tencentcloud-sdk-python-redis-3.0.949/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-redis',
-    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.949"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Redis SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-redis-3.0.948/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-redis-3.0.949/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.948/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.949/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.948/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.949/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.948'
+__version__ = '3.0.949'
```

### Comparing `tencentcloud-sdk-python-redis-3.0.948/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.949/tencentcloud/redis/v20180412/redis_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -759,15 +759,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceMonitorSIP(self, request):
-        """查询实例访问来源信息
+        """该接口已下线，请使用数据库智能管家 DBbrain 接口 [DescribeProxyProcessStatistics] (https://cloud.tencent.com/document/product/1130/84544) 获取实例访问来源。
 
         :param request: Request instance for DescribeInstanceMonitorSIP.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceMonitorSIPRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceMonitorSIPResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-redis-3.0.948/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.949/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.948/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.949/tencentcloud/redis/v20180412/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -14881,17 +14881,17 @@
 class SourceInfo(AbstractModel):
     """访问来源信息
 
     """
 
     def __init__(self):
         r"""
-        :param _Ip: 来源IP
+        :param _Ip: 来源 IP 地址。
         :type Ip: str
-        :param _Conn: 连接数
+        :param _Conn: 客户端连接数量。
         :type Conn: int
         :param _Cmd: 命令
         :type Cmd: int
         """
         self._Ip = None
         self._Conn = None
         self._Cmd = None
```

### Comparing `tencentcloud-sdk-python-redis-3.0.948/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.949/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.948/README.rst` & `tencentcloud-sdk-python-redis-3.0.949/README.rst`

 * *Files identical despite different names*

