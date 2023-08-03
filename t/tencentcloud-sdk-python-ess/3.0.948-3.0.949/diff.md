# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.948.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.949.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.948.tar", last modified: Wed Aug  2 00:29:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.949.tar", last modified: Thu Aug  3 00:26:09 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.948.tar` & `tencentcloud-sdk-python-ess-3.0.949.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    67109 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25058 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   477099 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud_sdk_python_ess.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    67169 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25058 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   478193 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud_sdk_python_ess.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-03 00:26:09.000000 tencentcloud-sdk-python-ess-3.0.949/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.948/setup.py` & `tencentcloud-sdk-python-ess-3.0.949/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-ess',
-    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.949"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Ess SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-ess-3.0.948/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.949/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.949/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -961,15 +961,15 @@
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowBriefs(self, request):
         """查询流程基础信息
         适用场景：可用于主动查询某个合同流程的签署状态信息。可以配合回调通知使用。
-        每个企业限制日调用量限制：10W,  当当日超过此限制后再调用接口返回错误
+        每个企业限制日调用量限制：10W，当日超过此限制后再调用接口返回错误
 
         :param request: Request instance for DescribeFlowBriefs.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeFlowBriefsRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeFlowBriefsResponse`
 
         """
         try:
@@ -1007,15 +1007,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowEvidenceReport(self, request):
-        """查询出证报告，返回报告 URL。
+        """查询出证报告，返回报告 URL。出证报告编号通过CreateFlowEvidenceReport接口获取。
 
         :param request: Request instance for DescribeFlowEvidenceReport.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeFlowEvidenceReportRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeFlowEvidenceReportResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.949/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.949/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,28 +557,28 @@
 
     def __init__(self):
         r"""
         :param _UserInfo: 自动签开通个人用户的三要素
         :type UserInfo: :class:`tencentcloud.ess.v20201111.models.UserThreeFactor`
         :param _CallbackUrl: 接受回调URL地址。支持http://或者https://协议
 
-Post数据到此地址后后返回httpcode200表示接受回调成功, 返回其他httpcode表示接受回调失败
+Post数据到此地址后返回httpcode200表示接受回调成功, 返回其他httpcode表示接受回调失败
         :type CallbackUrl: str
         :param _CertInfoCallback: 是否回调证书信息
 false-不需要 (默认值)
 true-需要
         :type CertInfoCallback: bool
         :param _UserDefineSeal: 是否支持用户自定义签名印章
 false-不需要(默认)
 true-需要
         :type UserDefineSeal: bool
         :param _SealImgCallback: 是否需要回调的时候返回印章(签名) 图片的 base64
 
 false-不需要(默认)
-true-需要(
+true-需要
         :type SealImgCallback: bool
         :param _VerifyChannels: 开通时候的验证方式, 分布为
 
 WEIXINAPP : 微信人脸识别
 INSIGHT : 慧眼人脸认别
 TELECOM : 运营商三要素验证
 
@@ -2325,23 +2325,29 @@
     """
 
     def __init__(self):
         r"""
         :param _Operator: 操作者信息
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _EmbedType: WEB嵌入资源类型。
-<br/>CREATE_SEAL: 创建印章
-<br/>PREVIEW_SEAL_LIST：预览印章列表
-<br/>PREVIEW_SEAL_DETAIL：预览印章详情
-<br/>EXTEND_SERVICE：拓展服务
-<br/>PREVIEW_FLOW：预览合同
-<br/>PREVIEW_FLOW_DETAIL：查看合同详情
+<br/>CREATE_SEAL: 生成创建印章的嵌入页面
+<br/>CREATE_TEMPLATE：生成创建模板的嵌入页面
+<br/>MODIFY_TEMPLATE：生成编辑模板的嵌入页面
+<br/>PREVIEW_TEMPLATE：生成预览模板的嵌入页面
+<br/>PREVIEW_SEAL_LIST：生成预览印章列表的嵌入页面
+<br/>PREVIEW_SEAL_DETAIL：生成预览印章详情的嵌入页面
+<br/>EXTEND_SERVICE：生成拓展服务的嵌入页面
+<br/>PREVIEW_FLOW：生成预览合同的嵌入页面
+<br/>PREVIEW_FLOW_DETAIL：生成查看合同详情的嵌入页面
+
         :type EmbedType: str
         :param _BusinessId: WEB嵌入的业务资源ID
 <br/>PREVIEW_SEAL_DETAIL，必填，取值为印章id
+<br/>MODIFY_TEMPLATE，PREVIEW_TEMPLATE，必填，取值为模版id
+<br/>PREVIEW_FLOW，PREVIEW_FLOW_DETAIL，必填，取值为合同id
         :type BusinessId: str
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param _Reviewer: 抄送方信息
         :type Reviewer: :class:`tencentcloud.ess.v20201111.models.ReviewerInfo`
         :param _Option: 个性化参数
         :type Option: :class:`tencentcloud.ess.v20201111.models.EmbedUrlOption`
@@ -3361,18 +3367,18 @@
     """
 
     def __init__(self):
         r"""
         :param _CanEditFlow: 是否允许修改发起合同时确认弹窗的合同信息（合同名称、合同类型、签署截止时间），若不允许编辑，则表单字段将被禁止输入。
 <br/>true：允许编辑（默认），<br/>false：不允许编辑<br/>默认：false：不允许编辑
         :type CanEditFlow: bool
-        :param _CanEditFormField: 是否允许编辑模版控件
-<br/>true:允许编辑模版控件信息
-<br/>false:不允许编辑模版控件信息
-<br/>默认false:不允许编辑模版控件信息
+        :param _CanEditFormField: 是否允许编辑模板控件
+<br/>true:允许编辑模板控件信息
+<br/>false:不允许编辑模板控件信息
+<br/>默认false:不允许编辑模板控件信息
         :type CanEditFormField: bool
         :param _HideShowFlowName: 发起页面隐藏合同名称展示
 <br/>true:发起页面隐藏合同名称展示
 <br/>false:发起页面不隐藏合同名称展示
 <br/>默认false:发起页面不隐藏合同名称展示
         :type HideShowFlowName: bool
         :param _HideShowFlowType: 发起页面隐藏合同类型展示
@@ -7807,15 +7813,15 @@
         :param _ReportUrl: 出证报告PDF的下载 URL
 注意：此字段可能返回 null，表示取不到有效值。
         :type ReportUrl: str
         :param _Status: 出证任务执行的状态, 分布表示下面的含义
 
 EvidenceStatusExecuting  出证任务在执行中
 EvidenceStatusSuccess  出证任务执行成功
-EvidenceStatusFailed  出征任务执行失败
+EvidenceStatusFailed  出证任务执行失败
         :type Status: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._ReportUrl = None
         self._Status = None
         self._RequestId = None
@@ -8868,31 +8874,35 @@
         r"""
         :param _Total: 查询到的符合条件的成员企业总数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type Total: int
         :param _JoinedTotal: 已授权待激活的企业数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type JoinedTotal: int
-        :param _ActivedTotal: 已加入的企业数量
+        :param _ActivedTotal: 已加入的企业数量(废弃,请使用ActivatedTotal)
 注意：此字段可能返回 null，表示取不到有效值。
         :type ActivedTotal: int
         :param _ExportUrl: 导出文件的url
 注意：此字段可能返回 null，表示取不到有效值。
         :type ExportUrl: str
         :param _List: 成员企业信息列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type List: list of GroupOrganization
+        :param _ActivatedTotal: 已加入的企业数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ActivatedTotal: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Total = None
         self._JoinedTotal = None
         self._ActivedTotal = None
         self._ExportUrl = None
         self._List = None
+        self._ActivatedTotal = None
         self._RequestId = None
 
     @property
     def Total(self):
         return self._Total
 
     @Total.setter
@@ -8905,18 +8915,22 @@
 
     @JoinedTotal.setter
     def JoinedTotal(self, JoinedTotal):
         self._JoinedTotal = JoinedTotal
 
     @property
     def ActivedTotal(self):
+        warnings.warn("parameter `ActivedTotal` is deprecated", DeprecationWarning) 
+
         return self._ActivedTotal
 
     @ActivedTotal.setter
     def ActivedTotal(self, ActivedTotal):
+        warnings.warn("parameter `ActivedTotal` is deprecated", DeprecationWarning) 
+
         self._ActivedTotal = ActivedTotal
 
     @property
     def ExportUrl(self):
         return self._ExportUrl
 
     @ExportUrl.setter
@@ -8928,14 +8942,22 @@
         return self._List
 
     @List.setter
     def List(self, List):
         self._List = List
 
     @property
+    def ActivatedTotal(self):
+        return self._ActivatedTotal
+
+    @ActivatedTotal.setter
+    def ActivatedTotal(self, ActivatedTotal):
+        self._ActivatedTotal = ActivatedTotal
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -8947,14 +8969,15 @@
         self._ExportUrl = params.get("ExportUrl")
         if params.get("List") is not None:
             self._List = []
             for item in params.get("List"):
                 obj = GroupOrganization()
                 obj._deserialize(item)
                 self._List.append(obj)
+        self._ActivatedTotal = params.get("ActivatedTotal")
         self._RequestId = params.get("RequestId")
 
 
 class DescribeOrganizationSealsRequest(AbstractModel):
     """DescribeOrganizationSeals请求参数结构体
 
     """
@@ -9470,18 +9493,18 @@
     def __init__(self):
         r"""
         :param _ShowFlowDetailComponent: 合同详情预览，允许展示控件信息
 <br/>true：允许在合同详情页展示控件
 <br/>false：不允许在合同详情页展示控件
 <br/>默认false，合同详情页不展示控件
         :type ShowFlowDetailComponent: bool
-        :param _ShowTemplateComponent: 模版预览，允许展示模版控件信息
-<br/>true：允许在模版预览页展示控件
-<br/>false：不允许在模版预览页展示控件
-<br/>默认false，模版预览页不展示控件
+        :param _ShowTemplateComponent: 模板预览，允许展示模板控件信息
+<br/>true：允许在模板预览页展示控件
+<br/>false：不允许在模板预览页展示控件
+<br/>默认false，模板预览页不展示控件
         :type ShowTemplateComponent: bool
         """
         self._ShowFlowDetailComponent = None
         self._ShowTemplateComponent = None
 
     @property
     def ShowFlowDetailComponent(self):
@@ -10685,15 +10708,15 @@
         :param _ApproverIdCardType: 签署方经办人证件类型ID_CARD 身份证
 HONGKONG_AND_MACAO 港澳居民来往内地通行证
 HONGKONG_MACAO_AND_TAIWAN 港澳台居民居住证(格式同居民身份证)
         :type ApproverIdCardType: str
         :param _ApproverIdCardNumber: 签署方经办人证件号码
         :type ApproverIdCardNumber: str
         :param _RecipientId: 签署方经办人在模板中的参与方ID
-<br/>模版发起合同时，该参数为必填项
+<br/>模板发起合同时，该参数为必填项
 <br/>文件发起合同是，该参数无序传值
 
         :type RecipientId: str
         :param _VerifyChannel: 签署意愿确认渠道,WEIXINAPP:人脸识别
         :type VerifyChannel: list of str
         :param _NotifyType: 是否发送短信
 <br/>sms--短信通知
@@ -13318,15 +13341,15 @@
 ORGANIZATION-企业
 ENTERPRISESERVER-企业静默签
         :type ApproverType: str
         :param _ApproverSignComponentType: 签署控件类型，支持自定义企业签署方的签署控件为“印章”或“签名”
 - SIGN_SEAL-默认为印章控件类型
 - SIGN_SIGNATURE-手写签名控件类型
         :type ApproverSignComponentType: str
-        :param _ApproverSignRole: 参与方在合同中的角色是按照创建合同的时候来排序的; 解除协议会将第一个参与人叫甲方, 第二个叫乙方,第三个叫丙方, 依次类推.  如果想改动参与人的角色名字, 可以设置此签署方自定义控件别名字段，最大20个字符
+        :param _ApproverSignRole: 参与方在合同中的角色是按照创建合同的时候来排序的; 解除协议会将第一个参与人叫甲方, 第二个叫乙方,第三个叫丙方，以此类推。  如果想改动参与人的角色名字, 可以设置此签署方自定义控件别名字段，最大20个字符
         :type ApproverSignRole: str
         """
         self._Name = None
         self._Mobile = None
         self._RelievedApproverReceiptId = None
         self._ApproverType = None
         self._ApproverSignComponentType = None
```

### Comparing `tencentcloud-sdk-python-ess-3.0.948/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.949/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.948/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.949/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.948
+Version: 3.0.949
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.948/README.rst` & `tencentcloud-sdk-python-ess-3.0.949/README.rst`

 * *Files identical despite different names*

