# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.948.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.949.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.948.tar", last modified: Wed Aug  2 00:29:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.949.tar", last modified: Thu Aug  3 00:26:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.948.tar` & `tencentcloud-sdk-python-essbasic-3.0.949.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    56676 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   393412 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54057 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      733 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    57594 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   393411 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54057 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      733 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud_sdk_python_essbasic.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 00:26:14.000000 tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.948/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.949/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-essbasic',
-    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.949"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Essbasic SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1080,19 +1080,31 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OperateChannelTemplate(self, request):
-        """此接口（OperateChannelTemplate）用于针对第三方应用平台模板库中的模板对子客企业可见性的查询和设置，不会直接分配第三方应用平台模板给子客企业。
-        1、OperateType=select时：
-        查询第三方应用平台模板库
-        2、OperateType=update或者delete时：
-        对子客企业进行模板库中模板可见性的修改、删除操作。
+        """此接口（OperateChannelTemplate）用于针对第三方应用平台模板库中的模板对子客企业可见性的查询和设置。
+
+        > **使用场景**
+        >
+        >  1：查询 OperateType=SELECT
+        > - 查询第三方应用平台模板库的可见性以及授权的子客列表。
+        >
+        >  2：修改部分子客授权 OperateType=UPDATE
+        > - 对子客企业进行模板库中模板可见性的进行修改操作。
+        >- 当模板未发布时，可以修改可见性AuthTag（part/all），当模板发布后，不可做此修改
+        > - 若模板已发布且可见性AuthTag是part，可以通过ProxyOrganizationOpenIds增加子客的授权范围。如果是自动领取的模板，增加授权范围后会自动下发。
+        >
+        >  3：取消部分子客授权 OperateType=DELETE
+        > - 对子客企业进行模板库中模板可见性的进行删除操作。
+        > - 主要对于手动领取的模板，去除授权后子客在在模板库中看不到，就无法再领取了。但是已经领取过成为自有模板的不会同步删除。
+        > - 对于自动领取的模板，由于已经下发，更改授权不会影响。
+        > - 如果要同步删除子客自有模板库中的模板，请使用OperateType=UPDATE+Available参数处理。
 
         :param request: Request instance for OperateChannelTemplate.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.OperateChannelTemplateRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.OperateChannelTemplateResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -9482,15 +9482,15 @@
         :param _ProxyOrganizationOpenIds: 合作企业方第三方机构唯一标识数据.
 支持多个， 用","进行分隔
         :type ProxyOrganizationOpenIds: str
         :param _AuthTag: 模板可见性, 
 全部可见-"all",
  部分可见-"part"
         :type AuthTag: str
-        :param _Available: 当OperateType=UPADATE时，可以通过设置此字段对模板启停用状态进行操作。
+        :param _Available: 当OperateType=UPDATE时，可以通过设置此字段对模板启停用状态进行操作。
 若此字段值为0，则不会修改模板Available，
 1为启用模板，
 2为停用模板。
 启用后模板可以正常领取。停用后，推送方式为【自动推送】的模板则无法被子客使用，推送方式为【手动领取】的模板则无法出现被模板库被子客领用。如果Available更新失败，会直接返回错误。
         :type Available: int
         :param _Operator: 暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.948/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.949/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.948/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.949/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.949/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

