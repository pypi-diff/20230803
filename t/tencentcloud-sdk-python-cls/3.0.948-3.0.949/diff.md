# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.948.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.949.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.948.tar", last modified: Wed Aug  2 00:26:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.949.tar", last modified: Thu Aug  3 00:23:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.948.tar` & `tencentcloud-sdk-python-cls-3.0.949.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)    84575 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9142 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   509932 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud_sdk_python_cls.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-02 00:26:47.000000 tencentcloud-sdk-python-cls-3.0.948/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:23:11.000000 tencentcloud-sdk-python-cls-3.0.949/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-03 00:23:10.000000 tencentcloud-sdk-python-cls-3.0.949/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:23:11.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:23:11.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:23:11.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)    84575 2023-08-03 00:23:10.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:23:10.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9142 2023-08-03 00:23:10.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   511117 2023-08-03 00:23:10.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:23:10.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-03 00:23:10.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-03 00:23:11.000000 tencentcloud-sdk-python-cls-3.0.949/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:23:11.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:23:11.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-03 00:23:11.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-03 00:23:11.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud_sdk_python_cls.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:23:11.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 00:23:11.000000 tencentcloud-sdk-python-cls-3.0.949/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:23:11.000000 tencentcloud-sdk-python-cls-3.0.949/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-03 00:23:10.000000 tencentcloud-sdk-python-cls-3.0.949/README.rst
```

### Comparing `tencentcloud-sdk-python-cls-3.0.948/setup.py` & `tencentcloud-sdk-python-cls-3.0.949/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cls',
-    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.949"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cls SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-cls-3.0.948/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.949/tencentcloud/cls/v20201016/cls_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.948/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.949/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.948/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.949/tencentcloud/cls/v20201016/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -8314,20 +8314,23 @@
         r"""
         :param _Status: Kafka协议消费是否打开
         :type Status: bool
         :param _TopicID: KafkaConsumer 消费时使用的Topic参数
         :type TopicID: str
         :param _Compression: 压缩方式[0:NONE；2:SNAPPY；3:LZ4]
         :type Compression: int
+        :param _ConsumerContent: kafka协议消费数据格式
+        :type ConsumerContent: :class:`tencentcloud.cls.v20201016.models.KafkaConsumerContent`
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Status = None
         self._TopicID = None
         self._Compression = None
+        self._ConsumerContent = None
         self._RequestId = None
 
     @property
     def Status(self):
         return self._Status
 
     @Status.setter
@@ -8347,26 +8350,37 @@
         return self._Compression
 
     @Compression.setter
     def Compression(self, Compression):
         self._Compression = Compression
 
     @property
+    def ConsumerContent(self):
+        return self._ConsumerContent
+
+    @ConsumerContent.setter
+    def ConsumerContent(self, ConsumerContent):
+        self._ConsumerContent = ConsumerContent
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._Status = params.get("Status")
         self._TopicID = params.get("TopicID")
         self._Compression = params.get("Compression")
+        if params.get("ConsumerContent") is not None:
+            self._ConsumerContent = KafkaConsumerContent()
+            self._ConsumerContent._deserialize(params.get("ConsumerContent"))
         self._RequestId = params.get("RequestId")
 
 
 class DescribeKafkaRechargesRequest(AbstractModel):
     """DescribeKafkaRecharges请求参数结构体
 
     """
@@ -13886,17 +13900,20 @@
 
     def __init__(self):
         r"""
         :param _FromTopicId: 日志主题ID
         :type FromTopicId: str
         :param _Compression: 压缩方式[0:NONE；2:SNAPPY；3:LZ4]
         :type Compression: int
+        :param _ConsumerContent: kafka协议消费数据格式
+        :type ConsumerContent: :class:`tencentcloud.cls.v20201016.models.KafkaConsumerContent`
         """
         self._FromTopicId = None
         self._Compression = None
+        self._ConsumerContent = None
 
     @property
     def FromTopicId(self):
         return self._FromTopicId
 
     @FromTopicId.setter
     def FromTopicId(self, FromTopicId):
@@ -13906,18 +13923,29 @@
     def Compression(self):
         return self._Compression
 
     @Compression.setter
     def Compression(self, Compression):
         self._Compression = Compression
 
+    @property
+    def ConsumerContent(self):
+        return self._ConsumerContent
+
+    @ConsumerContent.setter
+    def ConsumerContent(self, ConsumerContent):
+        self._ConsumerContent = ConsumerContent
+
 
     def _deserialize(self, params):
         self._FromTopicId = params.get("FromTopicId")
         self._Compression = params.get("Compression")
+        if params.get("ConsumerContent") is not None:
+            self._ConsumerContent = KafkaConsumerContent()
+            self._ConsumerContent._deserialize(params.get("ConsumerContent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -15972,15 +16000,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _TopicId: 目标主题id
         :type TopicId: str
-        :param _Region: 主题的的地域信息
+        :param _Region: 主题的地域信息
         :type Region: str
         :param _BizType: 主题类型：0为日志主题，1为指标主题
         :type BizType: int
         :param _MetricName: 指标名称
         :type MetricName: str
         """
         self._TopicId = None
```

### Comparing `tencentcloud-sdk-python-cls-3.0.948/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.949/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.948/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.949/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.948/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.949/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.948/README.rst` & `tencentcloud-sdk-python-cls-3.0.949/README.rst`

 * *Files identical despite different names*

