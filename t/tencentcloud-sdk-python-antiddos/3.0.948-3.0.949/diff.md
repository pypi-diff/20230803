# Comparing `tmp/tencentcloud-sdk-python-antiddos-3.0.948.tar.gz` & `tmp/tencentcloud-sdk-python-antiddos-3.0.949.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-antiddos-3.0.948.tar", last modified: Wed Aug  2 00:22:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-antiddos-3.0.949.tar", last modified: Thu Aug  3 00:18:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-antiddos-3.0.948.tar` & `tencentcloud-sdk-python-antiddos-3.0.949.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:22:27.000000 tencentcloud-sdk-python-antiddos-3.0.948/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-08-02 00:22:26.000000 tencentcloud-sdk-python-antiddos-3.0.948/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:22:27.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:22:26.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:22:27.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud/antiddos/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:22:26.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud/antiddos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:22:27.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud/antiddos/v20200309/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:22:26.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud/antiddos/v20200309/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89474 2023-08-02 00:22:26.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud/antiddos/v20200309/antiddos_client.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-08-02 00:22:26.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud/antiddos/v20200309/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   506474 2023-08-02 00:22:26.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud/antiddos/v20200309/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:22:27.000000 tencentcloud-sdk-python-antiddos-3.0.948/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:22:27.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud_sdk_python_antiddos.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:22:27.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud_sdk_python_antiddos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      550 2023-08-02 00:22:27.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud_sdk_python_antiddos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:22:27.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud_sdk_python_antiddos.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-08-02 00:22:27.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:22:27.000000 tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud_sdk_python_antiddos.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-08-02 00:22:27.000000 tencentcloud-sdk-python-antiddos-3.0.948/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-08-02 00:22:26.000000 tencentcloud-sdk-python-antiddos-3.0.948/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud/antiddos/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud/antiddos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud/antiddos/v20200309/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud/antiddos/v20200309/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89474 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud/antiddos/v20200309/antiddos_client.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud/antiddos/v20200309/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   506554 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud/antiddos/v20200309/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud_sdk_python_antiddos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud_sdk_python_antiddos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      550 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud_sdk_python_antiddos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud_sdk_python_antiddos.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud_sdk_python_antiddos.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-08-03 00:18:47.000000 tencentcloud-sdk-python-antiddos-3.0.949/README.rst
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.948/setup.py` & `tencentcloud-sdk-python-antiddos-3.0.949/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-antiddos',
-    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.949"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Antiddos SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud/__init__.py` & `tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud/antiddos/v20200309/antiddos_client.py` & `tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud/antiddos/v20200309/antiddos_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud/antiddos/v20200309/errorcodes.py` & `tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud/antiddos/v20200309/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud/antiddos/v20200309/models.py` & `tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud/antiddos/v20200309/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3035,15 +3035,15 @@
 class CreateBoundIPRequest(AbstractModel):
     """CreateBoundIP请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Business: 大禹子产品代号（bgp表示独享包；bgp-multip表示共享包）
+        :param _Business: DDoS防护子产品代号（bgp表示独享包；bgp-multip表示共享包）
         :type Business: str
         :param _Id: 资源实例ID
         :type Id: str
         :param _BoundDevList: 绑定到资源实例的IP数组，当资源实例为高防包(独享包)时，数组只允许填1个IP；当没有要绑定的IP时可以为空数组；但是BoundDevList和UnBoundDevList至少有一个不为空；
         :type BoundDevList: list of BoundIpInfo
         :param _UnBoundDevList: 与资源实例解绑的IP数组，当资源实例为高防包(独享包)时，数组只允许填1个IP；当没有要解绑的IP时可以为空数组；但是BoundDevList和UnBoundDevList至少有一个不为空；
         :type UnBoundDevList: list of BoundIpInfo
@@ -4256,15 +4256,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Rules: 规则列表
         :type Rules: list of L7RuleEntry
-        :param _Business: 大禹子产品代号（bgpip表示高防IP）
+        :param _Business: DDoS防护子产品代号（bgpip表示高防IP）
         :type Business: str
         :param _IdList: 资源ID列表
         :type IdList: list of str
         :param _VipList: 资源IP列表
         :type VipList: list of str
         """
         self._Rules = None
@@ -6344,15 +6344,15 @@
 class DescribeBgpBizTrendRequest(AbstractModel):
     """DescribeBgpBizTrend请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Business: 大禹子产品代号（bgp-multip表示高防包）
+        :param _Business: DDoS防护子产品代号（bgp-multip表示高防包）
         :type Business: str
         :param _StartTime: 统计开始时间。 例：“2020-09-22 00:00:00”
         :type StartTime: str
         :param _EndTime: 统计结束时间。 例：“2020-09-22 00:00:00”
         :type EndTime: str
         :param _MetricName: 统计纬度，可取值intraffic, outtraffic, inpkg, outpkg
         :type MetricName: str
@@ -6512,15 +6512,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Statistics: 统计方式，仅支持sum
         :type Statistics: str
-        :param _Business: 大禹子产品代号（bgpip表示高防IP）
+        :param _Business: DDoS防护子产品代号（bgpip表示高防IP）
         :type Business: str
         :param _Period: 统计周期，可取值60，300，1800，3600， 21600，86400，单位秒
         :type Period: int
         :param _StartTime: 统计开始时间。 如2020-02-01 12:04:12
         :type StartTime: str
         :param _EndTime: 统计结束时间。如2020-02-03 18:03:23
         :type EndTime: str
@@ -6671,15 +6671,15 @@
 class DescribeBizMonitorTrendRequest(AbstractModel):
     """DescribeBizMonitorTrend请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Business: 大禹子产品代号（bgpip表示高防IP）
+        :param _Business: DDoS防护子产品代号（bgpip表示高防IP）
         :type Business: str
         :param _StartTime: 统计开始时间。 例：“2020-09-22 00:00:00”
         :type StartTime: str
         :param _EndTime: 统计结束时间。 例：“2020-09-22 00:00:00”
         :type EndTime: str
         :param _Id: 资源实例ID
         :type Id: str
@@ -6828,15 +6828,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Statistics: 统计方式，可取值max, min, avg, sum, 如统计纬度是流量速率或包量速率，仅可取值max
         :type Statistics: str
-        :param _Business: 大禹子产品代号（bgpip表示高防IP）
+        :param _Business: DDoS防护子产品代号（bgpip表示高防IP）
         :type Business: str
         :param _Period: 统计周期，可取值60，300，1800，3600，21600，86400，单位秒
         :type Period: int
         :param _StartTime: 统计开始时间。 例：“2020-09-22 00:00:00”
         :type StartTime: str
         :param _EndTime: 统计结束时间。 例：“2020-09-22 00:00:00”
         :type EndTime: str
@@ -7118,15 +7118,15 @@
 class DescribeCCLevelListRequest(AbstractModel):
     """DescribeCCLevelList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Business: 大禹子产品代号（bgp-multip表示高防包）
+        :param _Business: DDoS防护子产品代号（bgp-multip表示高防包）
         :type Business: str
         :param _Offset: 页起始偏移，取值为(页码-1)*一页条数
         :type Offset: int
         :param _Limit: 一页条数
         :type Limit: int
         :param _InstanceId: 指定实例Id
         :type InstanceId: str
@@ -7347,15 +7347,15 @@
 class DescribeCCPrecisionPlyListRequest(AbstractModel):
     """DescribeCCPrecisionPlyList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Business: 大禹子产品代号（bgpip-multip：表示高防包；bgpip：表示高防IP）
+        :param _Business: DDoS防护子产品代号（bgpip-multip：表示高防包；bgpip：表示高防IP）
         :type Business: str
         :param _Offset: 页起始偏移，取值为(页码-1)*一页条数
         :type Offset: int
         :param _Limit: 一页条数
         :type Limit: int
         :param _InstanceId: 指定特定实例Id
         :type InstanceId: str
@@ -7506,15 +7506,15 @@
 class DescribeCCReqLimitPolicyListRequest(AbstractModel):
     """DescribeCCReqLimitPolicyList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Business: 大禹子产品代号（bgp-multip表示高防包，bgpip表示高防IP）
+        :param _Business: DDoS防护子产品代号（bgp-multip表示高防包，bgpip表示高防IP）
         :type Business: str
         :param _Offset: 页起始偏移，取值为(页码-1)*一页条数
         :type Offset: int
         :param _Limit: 一页条数
         :type Limit: int
         :param _InstanceId: 指定实例Id
         :type InstanceId: str
@@ -7665,15 +7665,15 @@
 class DescribeCCThresholdListRequest(AbstractModel):
     """DescribeCCThresholdList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Business: 大禹子产品代号（bgp-multip表示高防包）
+        :param _Business: DDoS防护子产品代号（bgp-multip表示高防包）
         :type Business: str
         :param _Offset: 页起始偏移，取值为(页码-1)*一页条数
         :type Offset: int
         :param _Limit: 一页条数
         :type Limit: int
         :param _InstanceId: 指定实例Id
         :type InstanceId: str
@@ -7788,15 +7788,15 @@
 class DescribeCCTrendRequest(AbstractModel):
     """DescribeCCTrend请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Business: 大禹子产品代号（bgpip表示高防IP；bgp表示独享包；bgp-multip表示共享包；net表示高防IP专业版；basic表示DDoS基础防护）
+        :param _Business: DDoS防护子产品代号（bgpip表示高防IP；bgp表示独享包；bgp-multip表示共享包；net表示高防IP专业版；basic表示DDoS基础防护）
         :type Business: str
         :param _Ip: 资源的IP
         :type Ip: str
         :param _Period: 统计粒度，取值[300(5分钟)，3600(小时)，86400(天)]
         :type Period: int
         :param _StartTime: 统计开始时间
         :type StartTime: str
@@ -8039,15 +8039,15 @@
 class DescribeCcBlackWhiteIpListRequest(AbstractModel):
     """DescribeCcBlackWhiteIpList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Business: 大禹子产品代号（bgp-multip：表示高防包；bgpip：表示高防IP）
+        :param _Business: DDoS防护子产品代号（bgp-multip：表示高防包；bgpip：表示高防IP）
         :type Business: str
         :param _InstanceId: 指定特定实例Id
         :type InstanceId: str
         :param _Offset: 页起始偏移，取值为(页码-1)*一页条数
         :type Offset: int
         :param _Limit: 一页条数
         :type Limit: int
@@ -8222,15 +8222,15 @@
 class DescribeCcGeoIPBlockConfigListRequest(AbstractModel):
     """DescribeCcGeoIPBlockConfigList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Business: 大禹子产品代号（bgpip-multip：表示高防包；bgpip：表示高防IP）
+        :param _Business: DDoS防护子产品代号（bgpip-multip：表示高防包；bgpip：表示高防IP）
         :type Business: str
         :param _Offset: 页起始偏移，取值为(页码-1)*一页条数
         :type Offset: int
         :param _Limit: 一页条数
         :type Limit: int
         :param _InstanceId: 指定特定实例ID
         :type InstanceId: str
@@ -11064,15 +11064,15 @@
 class DescribeNewL7RulesErrHealthRequest(AbstractModel):
     """DescribeNewL7RulesErrHealth请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Business: 大禹子产品代号(bgpip表示高防IP)
+        :param _Business: DDoS防护子产品代号(bgpip表示高防IP)
         :type Business: str
         :param _RuleIdList: 规则Id列表
         :type RuleIdList: list of str
         """
         self._Business = None
         self._RuleIdList = None
 
@@ -11163,15 +11163,15 @@
 class DescribeNewL7RulesRequest(AbstractModel):
     """DescribeNewL7Rules请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Business: 大禹子产品代号（bgpip表示高防IP）
+        :param _Business: DDoS防护子产品代号（bgpip表示高防IP）
         :type Business: str
         :param _StatusList: 状态搜索，选填，取值[0(规则配置成功)，1(规则配置生效中)，2(规则配置失败)，3(规则删除生效中)，5(规则删除失败)，6(规则等待配置)，7(规则等待删除)，8(规则待配置证书)]
         :type StatusList: list of int non-negative
         :param _Domain: 域名搜索，选填，当需要搜索域名请填写
         :type Domain: str
         :param _Ip: IP搜索，选填，当需要搜索IP请填写
         :type Ip: str
@@ -11549,15 +11549,15 @@
         :type Period: int
         :param _StartTime: 统计开始时间
         :type StartTime: str
         :param _EndTime: 统计结束时间
         :type EndTime: str
         :param _MetricName: 指标，取值[inqps(总请求峰值，dropqps(攻击请求峰值))，incount(请求次数), dropcount(攻击次数)]
         :type MetricName: str
-        :param _Business: 大禹子产品代号（bgpip表示高防IP；bgp-multip表示共享包；basic表示DDoS基础防护）
+        :param _Business: DDoS防护子产品代号（bgpip表示高防IP；bgp-multip表示共享包；basic表示DDoS基础防护）
         :type Business: str
         :param _IpList: 资源的IP
         :type IpList: list of str
         :param _Id: 资源实例ID
         :type Id: str
         """
         self._Period = None
@@ -11838,15 +11838,15 @@
         :type Period: int
         :param _StartTime: 统计开始时间
         :type StartTime: str
         :param _EndTime: 统计结束时间
         :type EndTime: str
         :param _MetricName: 指标，取值[bps(攻击流量带宽，pps(攻击包速率))]
         :type MetricName: str
-        :param _Business: 大禹子产品代号（bgpip表示高防IP；bgp-multip表示高防包；basic表示DDoS基础防护）
+        :param _Business: DDoS防护子产品代号（bgpip表示高防IP；bgp-multip表示高防包；basic表示DDoS基础防护）
         :type Business: str
         :param _IpList: 资源实例的IP列表
         :type IpList: list of str
         :param _Id: 资源实例ID
         :type Id: str
         """
         self._Period = None
@@ -14724,15 +14724,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Id: 资源ID
         :type Id: str
-        :param _Business: 大禹子产品代号（bgpip表示高防IP；bgp表示独享包；bgp-multip表示共享包；net表示高防IP专业版）
+        :param _Business: DDoS防护子产品代号（bgpip表示高防IP；bgp表示独享包；bgp-multip表示共享包；net表示高防IP专业版）
         :type Business: str
         :param _Method: =get表示读取防护等级；=set表示修改防护等级
         :type Method: str
         :param _DDoSLevel: 防护等级，取值[low,middle,high]；当Method=set时必填
         :type DDoSLevel: str
         """
         self._Id = None
@@ -14917,15 +14917,15 @@
     def __init__(self):
         r"""
         :param _Threshold: DDoS清洗阈值，取值[0, 60, 80, 100, 150, 200, 250, 300, 400, 500, 700, 1000];
 当设置值为0时，表示采用默认值；
         :type Threshold: int
         :param _Id: 资源ID
         :type Id: str
-        :param _Business: 大禹子产品代号（bgpip表示高防IP；bgp表示独享包；bgp-multip表示共享包；net表示高防IP专业版）
+        :param _Business: DDoS防护子产品代号（bgpip表示高防IP；bgp表示独享包；bgp-multip表示共享包；net表示高防IP专业版）
         :type Business: str
         :param _OtherThresholdFlag: 配置其他阈值标志位，1表示配置其他阈值
         :type OtherThresholdFlag: int
         :param _SynFloodThreshold: SYN FLOOD流量阈值
         :type SynFloodThreshold: int
         :param _SynFloodPktThreshold: SYN FLOOD包量阈值
         :type SynFloodPktThreshold: int
@@ -15211,15 +15211,15 @@
 class ModifyNewDomainRulesRequest(AbstractModel):
     """ModifyNewDomainRules请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Business: 大禹子产品代号（bgpip表示高防IP）
+        :param _Business: DDoS防护子产品代号（bgpip表示高防IP）
         :type Business: str
         :param _Id: 资源ID
         :type Id: str
         :param _Rule: 域名转发规则
         :type Rule: :class:`tencentcloud.antiddos.v20200309.models.NewL7RuleEntry`
         """
         self._Business = None
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud_sdk_python_antiddos.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud_sdk_python_antiddos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.948/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO` & `tencentcloud-sdk-python-antiddos-3.0.949/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-antiddos
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Antiddos SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.948/PKG-INFO` & `tencentcloud-sdk-python-antiddos-3.0.949/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-antiddos
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Antiddos SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.948/README.rst` & `tencentcloud-sdk-python-antiddos-3.0.949/README.rst`

 * *Files identical despite different names*

