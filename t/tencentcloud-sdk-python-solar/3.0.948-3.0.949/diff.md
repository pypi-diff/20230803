# Comparing `tmp/tencentcloud-sdk-python-solar-3.0.948.tar.gz` & `tmp/tencentcloud-sdk-python-solar-3.0.949.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-solar-3.0.948.tar", last modified: Wed Aug  2 00:36:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-solar-3.0.949.tar", last modified: Thu Aug  3 00:33:43 2023, max compression
```

## Comparing `tencentcloud-sdk-python-solar-3.0.948.tar` & `tencentcloud-sdk-python-solar-3.0.949.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/
--rw-r--r--   0 root         (0) root         (0)     1076 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud_sdk_python_solar.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud_sdk_python_solar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      517 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud_sdk_python_solar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud_sdk_python_solar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud_sdk_python_solar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud_sdk_python_solar.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud/solar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud/solar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud/solar/v20181011/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud/solar/v20181011/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud/solar/v20181011/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    15882 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud/solar/v20181011/solar_client.py
--rw-r--r--   0 root         (0) root         (0)    88391 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/tencentcloud/solar/v20181011/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-08-02 00:36:38.000000 tencentcloud-sdk-python-solar-3.0.948/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud_sdk_python_solar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud_sdk_python_solar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      517 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud_sdk_python_solar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud_sdk_python_solar.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud_sdk_python_solar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud_sdk_python_solar.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud/solar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud/solar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud/solar/v20181011/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud/solar/v20181011/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud/solar/v20181011/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    15882 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud/solar/v20181011/solar_client.py
+-rw-r--r--   0 root         (0) root         (0)    88391 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/tencentcloud/solar/v20181011/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-08-03 00:33:43.000000 tencentcloud-sdk-python-solar-3.0.949/README.rst
```

### Comparing `tencentcloud-sdk-python-solar-3.0.948/setup.py` & `tencentcloud-sdk-python-solar-3.0.949/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-solar',
-    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.949"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Solar SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-solar-3.0.948/tencentcloud_sdk_python_solar.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-solar-3.0.949/tencentcloud_sdk_python_solar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-solar-3.0.948/tencentcloud_sdk_python_solar.egg-info/PKG-INFO` & `tencentcloud-sdk-python-solar-3.0.949/tencentcloud_sdk_python_solar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-solar
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Solar SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-solar-3.0.948/tencentcloud/__init__.py` & `tencentcloud-sdk-python-solar-3.0.949/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-solar-3.0.948/tencentcloud/solar/v20181011/errorcodes.py` & `tencentcloud-sdk-python-solar-3.0.949/tencentcloud/solar/v20181011/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-solar-3.0.948/tencentcloud/solar/v20181011/solar_client.py` & `tencentcloud-sdk-python-solar-3.0.949/tencentcloud/solar/v20181011/solar_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-solar-3.0.948/tencentcloud/solar/v20181011/models.py` & `tencentcloud-sdk-python-solar-3.0.949/tencentcloud/solar/v20181011/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-solar-3.0.948/PKG-INFO` & `tencentcloud-sdk-python-solar-3.0.949/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-solar
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Solar SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-solar-3.0.948/README.rst` & `tencentcloud-sdk-python-solar-3.0.949/README.rst`

 * *Files identical despite different names*

