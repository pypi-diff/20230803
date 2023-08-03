# Comparing `tmp/tencentcloud-sdk-python-tiw-3.0.948.tar.gz` & `tmp/tencentcloud-sdk-python-tiw-3.0.949.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tiw-3.0.948.tar", last modified: Wed Aug  2 00:39:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tiw-3.0.949.tar", last modified: Thu Aug  3 00:36:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tiw-3.0.948.tar` & `tencentcloud-sdk-python-tiw-3.0.949.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud_sdk_python_tiw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud_sdk_python_tiw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud_sdk_python_tiw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud_sdk_python_tiw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud_sdk_python_tiw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud/tiw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud/tiw/v20190919/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud/tiw/v20190919/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6089 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud/tiw/v20190919/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    61449 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud/tiw/v20190919/tiw_client.py
--rw-r--r--   0 root         (0) root         (0)   284659 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud/tiw/v20190919/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud/tiw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-02 00:39:49.000000 tencentcloud-sdk-python-tiw-3.0.948/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud_sdk_python_tiw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud_sdk_python_tiw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud_sdk_python_tiw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud_sdk_python_tiw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud_sdk_python_tiw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud/tiw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud/tiw/v20190919/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud/tiw/v20190919/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6092 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud/tiw/v20190919/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    61455 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud/tiw/v20190919/tiw_client.py
+-rw-r--r--   0 root         (0) root         (0)   284659 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud/tiw/v20190919/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud/tiw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-03 00:36:50.000000 tencentcloud-sdk-python-tiw-3.0.949/README.rst
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.948/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tiw-3.0.949/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiw
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Tiw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.948/setup.py` & `tencentcloud-sdk-python-tiw-3.0.949/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-tiw',
-    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.949"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Tiw SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.948/tencentcloud/tiw/v20190919/errorcodes.py` & `tencentcloud-sdk-python-tiw-3.0.949/tencentcloud/tiw/v20190919/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,12 +139,12 @@
 
 # 未知参数错误。
 UNKNOWNPARAMETER = 'UnknownParameter'
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
 
-# 当前未完成的任务不能此状态下执行指定操作，例如对正在录制的任务执行恢复录制等。
+# 当前未完成的任务不能在此状态下执行指定操作，例如对正在录制的任务执行恢复录制等。
 UNSUPPORTEDOPERATION_INVALIDTASKSTATUS = 'UnsupportedOperation.InvalidTaskStatus'
 
 # 任务结束，不能执行指定操作。
 UNSUPPORTEDOPERATION_TASKHASALREADYSTOPPED = 'UnsupportedOperation.TaskHasAlreadyStopped'
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.948/tencentcloud/tiw/v20190919/tiw_client.py` & `tencentcloud-sdk-python-tiw-3.0.949/tencentcloud/tiw/v20190919/tiw_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,15 +648,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTranscodeByUrl(self, request):
-        """通过文档URL查询转码任务，返回最近的一次转码结果
+        """通过文档URL查询转码任务，返回最近一次的转码任务状态
 
         :param request: Request instance for DescribeTranscodeByUrl.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeTranscodeByUrlRequest`
         :rtype: :class:`tencentcloud.tiw.v20190919.models.DescribeTranscodeByUrlResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.948/tencentcloud/tiw/v20190919/models.py` & `tencentcloud-sdk-python-tiw-3.0.949/tencentcloud/tiw/v20190919/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7575,15 +7575,15 @@
 class SnapshotCOS(AbstractModel):
     """板书文件存储cos参数
 
     """
 
     def __init__(self):
         r"""
-        :param _Uin: cos所在腾讯云帐号uin
+        :param _Uin: cos所在腾讯云账号uin
         :type Uin: int
         :param _Region: cos所在地区
         :type Region: str
         :param _Bucket: cos存储桶名称
         :type Bucket: str
         :param _TargetDir: 板书文件存储根目录
         :type TargetDir: str
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.948/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tiw-3.0.949/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tiw-3.0.948/PKG-INFO` & `tencentcloud-sdk-python-tiw-3.0.949/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiw
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Tiw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.948/README.rst` & `tencentcloud-sdk-python-tiw-3.0.949/README.rst`

 * *Files identical despite different names*

