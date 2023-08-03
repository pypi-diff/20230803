# Comparing `tmp/neulabs-cdk-constructs-0.5.3.tar.gz` & `tmp/neulabs-cdk-constructs-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neulabs-cdk-constructs-0.5.3.tar", last modified: Wed Aug  2 13:09:39 2023, max compression
+gzip compressed data, was "neulabs-cdk-constructs-0.5.4.tar", last modified: Thu Aug  3 13:52:51 2023, max compression
```

## Comparing `neulabs-cdk-constructs-0.5.3.tar` & `neulabs-cdk-constructs-0.5.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.247220 neulabs-cdk-constructs-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   117579 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.5.3.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)   306174 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/aws_lambda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)    49782 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    47689 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/stack/
--rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-08-02 13:09:39.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-02 13:09:39.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:09:39.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-02 13:09:39.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 13:09:39.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:51.984028 neulabs-cdk-constructs-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-03 13:52:38.000000 neulabs-cdk-constructs-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 13:52:38.000000 neulabs-cdk-constructs-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-08-03 13:52:51.984028 neulabs-cdk-constructs-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-08-03 13:52:38.000000 neulabs-cdk-constructs-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-03 13:52:38.000000 neulabs-cdk-constructs-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 13:52:51.984028 neulabs-cdk-constructs-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-03 13:52:38.000000 neulabs-cdk-constructs-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:51.984028 neulabs-cdk-constructs-0.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:51.984028 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-08-03 13:52:38.000000 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:51.984028 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-03 13:52:38.000000 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117663 2023-08-03 13:52:38.000000 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.5.4.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:51.984028 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)   306174 2023-08-03 13:52:38.000000 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/aws_lambda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:51.984028 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)    52606 2023-08-03 13:52:38.000000 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:51.984028 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    47689 2023-08-03 13:52:38.000000 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 13:52:38.000000 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:51.984028 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-08-03 13:52:38.000000 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:51.984028 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-08-03 13:52:38.000000 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:51.984028 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-08-03 13:52:51.000000 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-03 13:52:51.000000 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 13:52:51.000000 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-03 13:52:51.000000 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 13:52:51.000000 neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs.egg-info/top_level.txt
```

### Comparing `neulabs-cdk-constructs-0.5.3/LICENSE` & `neulabs-cdk-constructs-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.3/PKG-INFO` & `neulabs-cdk-constructs-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.5.3
+Version: 0.5.4
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `neulabs-cdk-constructs-0.5.3/README.md` & `neulabs-cdk-constructs-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.3/setup.py` & `neulabs-cdk-constructs-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "neulabs-cdk-constructs",
-    "version": "0.5.3",
+    "version": "0.5.4",
     "description": "neulabs-cdk-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/neulabscom/neulabs-cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Neulabs<tech@neulabs.com>",
     "bdist_wheel": {
         "universal": true
@@ -27,15 +27,15 @@
         "neulabs_cdk_constructs.newrelic",
         "neulabs_cdk_constructs.oidc",
         "neulabs_cdk_constructs.stack",
         "neulabs_cdk_constructs.utils"
     ],
     "package_data": {
         "neulabs_cdk_constructs._jsii": [
-            "neulabs-cdk-constructs@0.5.3.jsii.tgz"
+            "neulabs-cdk-constructs@0.5.4.jsii.tgz"
         ],
         "neulabs_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/__init__.py` & `neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/_jsii/__init__.py` & `neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aws_cdk._jsii
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_apigatewayv2_integrations_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "neulabs-cdk-constructs",
-    "0.5.3",
+    "0.5.4",
     __name__[0:-6],
-    "neulabs-cdk-constructs@0.5.3.jsii.tgz",
+    "neulabs-cdk-constructs@0.5.4.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/aws_lambda/__init__.py` & `neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/aws_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/newrelic/__init__.py` & `neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/newrelic/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,14 +106,15 @@
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         new_relic_account_id: builtins.str,
         new_relic_bucket_name: builtins.str,
         new_relic_license_key: builtins.str,
+        buffery_hints: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream.BufferingHintsProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         cloudwatch_metric_stream_props: typing.Optional[typing.Union[CfnMetricStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
         new_relic_api_url_logs: typing.Optional[EndpointUrlLogs] = None,
         new_relic_api_url_metrics: typing.Optional[EndpointUrlMetrics] = None,
         stage: builtins.str,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
@@ -127,14 +128,15 @@
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param new_relic_account_id: 
         :param new_relic_bucket_name: 
         :param new_relic_license_key: 
+        :param buffery_hints: 
         :param cloudwatch_metric_stream_props: 
         :param new_relic_api_url_logs: 
         :param new_relic_api_url_metrics: 
         :param stage: 
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
@@ -150,14 +152,15 @@
             type_hints = typing.get_type_hints(_typecheckingstub__3d16994fa6098e1a11bee3003bb87e23e040f04cdc0edc42f729eccb764b26ca)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = NewRelicStackProps(
             new_relic_account_id=new_relic_account_id,
             new_relic_bucket_name=new_relic_bucket_name,
             new_relic_license_key=new_relic_license_key,
+            buffery_hints=buffery_hints,
             cloudwatch_metric_stream_props=cloudwatch_metric_stream_props,
             new_relic_api_url_logs=new_relic_api_url_logs,
             new_relic_api_url_metrics=new_relic_api_url_metrics,
             stage=stage,
             analytics_reporting=analytics_reporting,
             cross_region_references=cross_region_references,
             description=description,
@@ -228,30 +231,39 @@
     def create_firehose_stream(
         self,
         new_relic_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
         role: _aws_cdk_aws_iam_ceddda9d.IRole,
         endpoint_type: EndpointType,
         endpoint_url: builtins.str,
         new_relic_license_ley: builtins.str,
+        *,
+        interval_in_seconds: typing.Optional[jsii.Number] = None,
+        size_in_m_bs: typing.Optional[jsii.Number] = None,
     ) -> _aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream:
         '''
         :param new_relic_bucket: -
         :param role: -
         :param endpoint_type: -
         :param endpoint_url: -
         :param new_relic_license_ley: -
+        :param interval_in_seconds: The length of time, in seconds, that Kinesis Data Firehose buffers incoming data before delivering it to the destination. For valid values, see the ``IntervalInSeconds`` content for the `BufferingHints <https://docs.aws.amazon.com/firehose/latest/APIReference/API_BufferingHints.html>`_ data type in the *Amazon Kinesis Data Firehose API Reference* .
+        :param size_in_m_bs: The size of the buffer, in MBs, that Kinesis Data Firehose uses for incoming data before delivering it to the destination. For valid values, see the ``SizeInMBs`` content for the `BufferingHints <https://docs.aws.amazon.com/firehose/latest/APIReference/API_BufferingHints.html>`_ data type in the *Amazon Kinesis Data Firehose API Reference* .
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__29a8c6006513a8211068ba90e3161ed414e09ab40b8b39a6df5b69eda0c7580b)
             check_type(argname="argument new_relic_bucket", value=new_relic_bucket, expected_type=type_hints["new_relic_bucket"])
             check_type(argname="argument role", value=role, expected_type=type_hints["role"])
             check_type(argname="argument endpoint_type", value=endpoint_type, expected_type=type_hints["endpoint_type"])
             check_type(argname="argument endpoint_url", value=endpoint_url, expected_type=type_hints["endpoint_url"])
             check_type(argname="argument new_relic_license_ley", value=new_relic_license_ley, expected_type=type_hints["new_relic_license_ley"])
-        return typing.cast(_aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream, jsii.invoke(self, "createFirehoseStream", [new_relic_bucket, role, endpoint_type, endpoint_url, new_relic_license_ley]))
+        buffering_hints = _aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream.BufferingHintsProperty(
+            interval_in_seconds=interval_in_seconds, size_in_m_bs=size_in_m_bs
+        )
+
+        return typing.cast(_aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream, jsii.invoke(self, "createFirehoseStream", [new_relic_bucket, role, endpoint_type, endpoint_url, new_relic_license_ley, buffering_hints]))
 
     @jsii.member(jsii_name="createNewRelicRole")
     def create_new_relic_role(
         self,
         new_relic_account_id: builtins.str,
     ) -> _aws_cdk_aws_iam_ceddda9d.IRole:
         '''
@@ -398,14 +410,15 @@
         "synthesizer": "synthesizer",
         "tags": "tags",
         "termination_protection": "terminationProtection",
         "stage": "stage",
         "new_relic_account_id": "newRelicAccountId",
         "new_relic_bucket_name": "newRelicBucketName",
         "new_relic_license_key": "newRelicLicenseKey",
+        "buffery_hints": "bufferyHints",
         "cloudwatch_metric_stream_props": "cloudwatchMetricStreamProps",
         "new_relic_api_url_logs": "newRelicApiUrlLogs",
         "new_relic_api_url_metrics": "newRelicApiUrlMetrics",
     },
 )
 class NewRelicStackProps(_BaseStackProps_bfec638c):
     def __init__(
@@ -421,14 +434,15 @@
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
         stage: builtins.str,
         new_relic_account_id: builtins.str,
         new_relic_bucket_name: builtins.str,
         new_relic_license_key: builtins.str,
+        buffery_hints: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream.BufferingHintsProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         cloudwatch_metric_stream_props: typing.Optional[typing.Union[CfnMetricStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
         new_relic_api_url_logs: typing.Optional[EndpointUrlLogs] = None,
         new_relic_api_url_metrics: typing.Optional[EndpointUrlMetrics] = None,
     ) -> None:
         '''
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
@@ -440,20 +454,23 @@
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         :param stage: 
         :param new_relic_account_id: 
         :param new_relic_bucket_name: 
         :param new_relic_license_key: 
+        :param buffery_hints: 
         :param cloudwatch_metric_stream_props: 
         :param new_relic_api_url_logs: 
         :param new_relic_api_url_metrics: 
         '''
         if isinstance(env, dict):
             env = _aws_cdk_ceddda9d.Environment(**env)
+        if isinstance(buffery_hints, dict):
+            buffery_hints = _aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream.BufferingHintsProperty(**buffery_hints)
         if isinstance(cloudwatch_metric_stream_props, dict):
             cloudwatch_metric_stream_props = CfnMetricStreamProps(**cloudwatch_metric_stream_props)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1b73444472d0b16a38d845ab8c4feabeadd9937eadb9c68ca1f7a002e868c7df)
             check_type(argname="argument analytics_reporting", value=analytics_reporting, expected_type=type_hints["analytics_reporting"])
             check_type(argname="argument cross_region_references", value=cross_region_references, expected_type=type_hints["cross_region_references"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
@@ -464,14 +481,15 @@
             check_type(argname="argument synthesizer", value=synthesizer, expected_type=type_hints["synthesizer"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument termination_protection", value=termination_protection, expected_type=type_hints["termination_protection"])
             check_type(argname="argument stage", value=stage, expected_type=type_hints["stage"])
             check_type(argname="argument new_relic_account_id", value=new_relic_account_id, expected_type=type_hints["new_relic_account_id"])
             check_type(argname="argument new_relic_bucket_name", value=new_relic_bucket_name, expected_type=type_hints["new_relic_bucket_name"])
             check_type(argname="argument new_relic_license_key", value=new_relic_license_key, expected_type=type_hints["new_relic_license_key"])
+            check_type(argname="argument buffery_hints", value=buffery_hints, expected_type=type_hints["buffery_hints"])
             check_type(argname="argument cloudwatch_metric_stream_props", value=cloudwatch_metric_stream_props, expected_type=type_hints["cloudwatch_metric_stream_props"])
             check_type(argname="argument new_relic_api_url_logs", value=new_relic_api_url_logs, expected_type=type_hints["new_relic_api_url_logs"])
             check_type(argname="argument new_relic_api_url_metrics", value=new_relic_api_url_metrics, expected_type=type_hints["new_relic_api_url_metrics"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "stage": stage,
             "new_relic_account_id": new_relic_account_id,
             "new_relic_bucket_name": new_relic_bucket_name,
@@ -493,14 +511,16 @@
             self._values["suppress_template_indentation"] = suppress_template_indentation
         if synthesizer is not None:
             self._values["synthesizer"] = synthesizer
         if tags is not None:
             self._values["tags"] = tags
         if termination_protection is not None:
             self._values["termination_protection"] = termination_protection
+        if buffery_hints is not None:
+            self._values["buffery_hints"] = buffery_hints
         if cloudwatch_metric_stream_props is not None:
             self._values["cloudwatch_metric_stream_props"] = cloudwatch_metric_stream_props
         if new_relic_api_url_logs is not None:
             self._values["new_relic_api_url_logs"] = new_relic_api_url_logs
         if new_relic_api_url_metrics is not None:
             self._values["new_relic_api_url_metrics"] = new_relic_api_url_metrics
 
@@ -700,14 +720,21 @@
     @builtins.property
     def new_relic_license_key(self) -> builtins.str:
         result = self._values.get("new_relic_license_key")
         assert result is not None, "Required property 'new_relic_license_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
+    def buffery_hints(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream.BufferingHintsProperty]:
+        result = self._values.get("buffery_hints")
+        return typing.cast(typing.Optional[_aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream.BufferingHintsProperty], result)
+
+    @builtins.property
     def cloudwatch_metric_stream_props(self) -> typing.Optional[CfnMetricStreamProps]:
         result = self._values.get("cloudwatch_metric_stream_props")
         return typing.cast(typing.Optional[CfnMetricStreamProps], result)
 
     @builtins.property
     def new_relic_api_url_logs(self) -> typing.Optional[EndpointUrlLogs]:
         result = self._values.get("new_relic_api_url_logs")
@@ -752,14 +779,15 @@
 def _typecheckingstub__3d16994fa6098e1a11bee3003bb87e23e040f04cdc0edc42f729eccb764b26ca(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     new_relic_account_id: builtins.str,
     new_relic_bucket_name: builtins.str,
     new_relic_license_key: builtins.str,
+    buffery_hints: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream.BufferingHintsProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     cloudwatch_metric_stream_props: typing.Optional[typing.Union[CfnMetricStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
     new_relic_api_url_logs: typing.Optional[EndpointUrlLogs] = None,
     new_relic_api_url_metrics: typing.Optional[EndpointUrlMetrics] = None,
     stage: builtins.str,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
@@ -797,14 +825,17 @@
 
 def _typecheckingstub__29a8c6006513a8211068ba90e3161ed414e09ab40b8b39a6df5b69eda0c7580b(
     new_relic_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
     role: _aws_cdk_aws_iam_ceddda9d.IRole,
     endpoint_type: EndpointType,
     endpoint_url: builtins.str,
     new_relic_license_ley: builtins.str,
+    *,
+    interval_in_seconds: typing.Optional[jsii.Number] = None,
+    size_in_m_bs: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__4d2ce9d7e6b30b79bf03d30143ef0ab44dace126e3cf4fe6416410a87bd7adb9(
     new_relic_account_id: builtins.str,
 ) -> None:
@@ -872,13 +903,14 @@
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
     stage: builtins.str,
     new_relic_account_id: builtins.str,
     new_relic_bucket_name: builtins.str,
     new_relic_license_key: builtins.str,
+    buffery_hints: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_ceddda9d.CfnDeliveryStream.BufferingHintsProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     cloudwatch_metric_stream_props: typing.Optional[typing.Union[CfnMetricStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
     new_relic_api_url_logs: typing.Optional[EndpointUrlLogs] = None,
     new_relic_api_url_metrics: typing.Optional[EndpointUrlMetrics] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/oidc/__init__.py` & `neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/stack/__init__.py` & `neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/utils/__init__.py` & `neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/PKG-INFO` & `neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.5.3
+Version: 0.5.4
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/SOURCES.txt` & `neulabs-cdk-constructs-0.5.4/src/neulabs_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/neulabs_cdk_constructs/py.typed
 src/neulabs_cdk_constructs.egg-info/PKG-INFO
 src/neulabs_cdk_constructs.egg-info/SOURCES.txt
 src/neulabs_cdk_constructs.egg-info/dependency_links.txt
 src/neulabs_cdk_constructs.egg-info/requires.txt
 src/neulabs_cdk_constructs.egg-info/top_level.txt
 src/neulabs_cdk_constructs/_jsii/__init__.py
-src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.5.3.jsii.tgz
+src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.5.4.jsii.tgz
 src/neulabs_cdk_constructs/aws_lambda/__init__.py
 src/neulabs_cdk_constructs/newrelic/__init__.py
 src/neulabs_cdk_constructs/oidc/__init__.py
 src/neulabs_cdk_constructs/stack/__init__.py
 src/neulabs_cdk_constructs/utils/__init__.py
```

