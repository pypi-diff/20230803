# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.948.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.949.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.948.tar", last modified: Wed Aug  2 00:34:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.949.tar", last modified: Thu Aug  3 00:30:41 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.948.tar` & `tencentcloud-sdk-python-ocr-3.0.949.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5802 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   113546 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)   807406 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud_sdk_python_ocr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud/ocr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud/ocr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5802 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   113621 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)   807406 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud/ocr/v20181119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud_sdk_python_ocr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-03 00:30:41.000000 tencentcloud-sdk-python-ocr-3.0.949/README.rst
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.948/setup.py` & `tencentcloud-sdk-python-ocr-3.0.949/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-ocr',
-    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.949"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Ocr SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.949/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.949/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.949/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BusinessCardOCR(self, request):
-        """本接口支持名片各字段的自动定位与识别，包含姓名、电话、手机号、邮箱、公司、部门、职位、网址、地址、QQ、微信、MSN等。
+        """本接口支持中英文名片各字段的自动定位与识别，包含姓名、电话、手机号、邮箱、公司、部门、职位、网址、地址、QQ、微信、MSN等。
 
         默认接口请求频率限制：10次/秒。
 
         :param request: Request instance for BusinessCardOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.BusinessCardOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.BusinessCardOCRResponse`
 
@@ -931,15 +931,17 @@
                   <td>身份证照片裁剪（去掉证件外多余的边缘、自动矫正拍摄角度）</td>
                 </tr>
                 <tr>
                   <td>人像照片裁剪（自动抠取身份证头像区域）</td>
                 </tr>
                 <tr>
                   <td rowspan="9">告警功能</td>
-                  <td>身份证有效日期不合法告警</td>
+                  <td>身份证有效日期不合法，即有效日期不符合5年、10年、20年、长期期限
+
+        </td>
                 </tr>
                 <tr>
                   <td>身份证边框不完整告警</td>
                 </tr>
                 <tr>
                   <td>身份证复印件告警</td>
                 </tr>
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.949/tencentcloud/ocr/v20181119/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.948/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.949/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.948/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.949/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.948/README.rst` & `tencentcloud-sdk-python-ocr-3.0.949/README.rst`

 * *Files identical despite different names*

