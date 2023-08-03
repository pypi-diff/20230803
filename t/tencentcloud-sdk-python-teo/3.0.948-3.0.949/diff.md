# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.948.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.949.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.948.tar", last modified: Wed Aug  2 00:39:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.949.tar", last modified: Thu Aug  3 00:36:03 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.948.tar` & `tencentcloud-sdk-python-teo-3.0.949.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60588 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)    24008 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   605317 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5399 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    38737 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      653 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud_sdk_python_teo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:39:03.000000 tencentcloud-sdk-python-teo-3.0.948/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60588 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)    24008 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   605326 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5399 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    38737 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      653 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud_sdk_python_teo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 00:36:03.000000 tencentcloud-sdk-python-teo-3.0.949/tencentcloud_sdk_python_teo.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-teo-3.0.948/setup.py` & `tencentcloud-sdk-python-teo-3.0.949/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-teo',
-    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.949"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Teo SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-teo-3.0.948/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.949/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220901/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2709,17 +2709,17 @@
 class CheckCnameStatusRequest(AbstractModel):
     """CheckCnameStatus请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _ZoneId: 站点ID。
+        :param _ZoneId: 站点 ID。
         :type ZoneId: str
-        :param _RecordNames: 记录名称列表。
+        :param _RecordNames: 加速域名列表。
         :type RecordNames: list of str
         """
         self._ZoneId = None
         self._RecordNames = None
 
     @property
     def ZoneId(self):
@@ -2754,15 +2754,15 @@
 class CheckCnameStatusResponse(AbstractModel):
     """CheckCnameStatus返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _CnameStatus: 域名Cname状态信息列表。
+        :param _CnameStatus: 加速域名 CNAME 状态信息列表。
         :type CnameStatus: list of CnameStatus
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._CnameStatus = None
         self._RequestId = None
```

### Comparing `tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.948/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.949/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.948/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.949/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.948/README.rst` & `tencentcloud-sdk-python-teo-3.0.949/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.948/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.949/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.948/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.949/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

