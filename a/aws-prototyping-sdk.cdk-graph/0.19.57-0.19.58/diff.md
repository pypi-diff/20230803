# Comparing `tmp/aws_prototyping_sdk.cdk_graph-0.19.57.tar.gz` & `tmp/aws_prototyping_sdk.cdk_graph-0.19.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.cdk_graph-0.19.57.tar", last modified: Wed Aug  2 02:51:01 2023, max compression
+gzip compressed data, was "aws_prototyping_sdk.cdk_graph-0.19.58.tar", last modified: Wed Aug  2 06:29:36 2023, max compression
```

## Comparing `aws_prototyping_sdk.cdk_graph-0.19.57.tar` & `aws_prototyping_sdk.cdk_graph-0.19.58.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:51:01.937218 aws_prototyping_sdk.cdk_graph-0.19.57/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 02:50:51.000000 aws_prototyping_sdk.cdk_graph-0.19.57/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 02:50:51.000000 aws_prototyping_sdk.cdk_graph-0.19.57/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-08-02 02:51:01.937218 aws_prototyping_sdk.cdk_graph-0.19.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-08-02 02:50:51.000000 aws_prototyping_sdk.cdk_graph-0.19.57/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 02:50:51.000000 aws_prototyping_sdk.cdk_graph-0.19.57/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 02:51:01.937218 aws_prototyping_sdk.cdk_graph-0.19.57/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-08-02 02:50:51.000000 aws_prototyping_sdk.cdk_graph-0.19.57/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:51:01.929217 aws_prototyping_sdk.cdk_graph-0.19.57/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:51:01.933218 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:51:01.933218 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk/cdk_graph/
--rw-r--r--   0 runner    (1001) docker     (123)    83028 2023-08-02 02:50:51.000000 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk/cdk_graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:51:01.933218 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk/cdk_graph/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-02 02:50:51.000000 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk/cdk_graph/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   626368 2023-08-02 02:50:51.000000 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk/cdk_graph/_jsii/cdk-graph@0.19.57.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:51:01.937218 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk/cdk_graph/graph/
--rw-r--r--   0 runner    (1001) docker     (123)   193146 2023-08-02 02:50:51.000000 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk/cdk_graph/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 02:50:51.000000 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk/cdk_graph/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:51:01.937218 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk/cdk_graph/serialized_graph/
--rw-r--r--   0 runner    (1001) docker     (123)    35320 2023-08-02 02:50:51.000000 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk/cdk_graph/serialized_graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:51:01.933218 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk.cdk_graph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-08-02 02:51:01.000000 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk.cdk_graph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 02:51:01.000000 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk.cdk_graph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 02:51:01.000000 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk.cdk_graph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 02:51:01.000000 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk.cdk_graph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 02:51:01.000000 aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk.cdk_graph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:29:36.402761 aws_prototyping_sdk.cdk_graph-0.19.58/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 06:29:26.000000 aws_prototyping_sdk.cdk_graph-0.19.58/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 06:29:26.000000 aws_prototyping_sdk.cdk_graph-0.19.58/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-08-02 06:29:36.402761 aws_prototyping_sdk.cdk_graph-0.19.58/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-08-02 06:29:26.000000 aws_prototyping_sdk.cdk_graph-0.19.58/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 06:29:26.000000 aws_prototyping_sdk.cdk_graph-0.19.58/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 06:29:36.402761 aws_prototyping_sdk.cdk_graph-0.19.58/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-08-02 06:29:26.000000 aws_prototyping_sdk.cdk_graph-0.19.58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:29:36.398761 aws_prototyping_sdk.cdk_graph-0.19.58/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:29:36.398761 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:29:36.398761 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk/cdk_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    83028 2023-08-02 06:29:26.000000 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk/cdk_graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:29:36.398761 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk/cdk_graph/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-02 06:29:26.000000 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk/cdk_graph/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   626374 2023-08-02 06:29:26.000000 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk/cdk_graph/_jsii/cdk-graph@0.19.58.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:29:36.402761 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk/cdk_graph/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)   193146 2023-08-02 06:29:26.000000 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk/cdk_graph/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 06:29:26.000000 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk/cdk_graph/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:29:36.402761 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk/cdk_graph/serialized_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    35320 2023-08-02 06:29:26.000000 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk/cdk_graph/serialized_graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:29:36.398761 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk.cdk_graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-08-02 06:29:36.000000 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk.cdk_graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 06:29:36.000000 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk.cdk_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 06:29:36.000000 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk.cdk_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 06:29:36.000000 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk.cdk_graph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 06:29:36.000000 aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk.cdk_graph.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.cdk_graph-0.19.57/LICENSE` & `aws_prototyping_sdk.cdk_graph-0.19.58/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.cdk_graph-0.19.57/PKG-INFO` & `aws_prototyping_sdk.cdk_graph-0.19.58/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_prototyping_sdk.cdk_graph
-Version: 0.19.57
+Version: 0.19.58
 Summary: @aws-prototyping-sdk/cdk-graph
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws_prototyping_sdk.cdk_graph-0.19.57/README.md` & `aws_prototyping_sdk.cdk_graph-0.19.58/README.md`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.cdk_graph-0.19.57/setup.py` & `aws_prototyping_sdk.cdk_graph-0.19.58/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.cdk_graph",
-    "version": "0.19.57",
+    "version": "0.19.58",
     "description": "@aws-prototyping-sdk/cdk-graph",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-prototyping-sdk",
     "long_description_content_type": "text/markdown",
     "author": "AWS APJ COPE<apj-cope@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -24,15 +24,15 @@
         "aws_prototyping_sdk.cdk_graph",
         "aws_prototyping_sdk.cdk_graph._jsii",
         "aws_prototyping_sdk.cdk_graph.graph",
         "aws_prototyping_sdk.cdk_graph.serialized_graph"
     ],
     "package_data": {
         "aws_prototyping_sdk.cdk_graph._jsii": [
-            "cdk-graph@0.19.57.jsii.tgz"
+            "cdk-graph@0.19.58.jsii.tgz"
         ],
         "aws_prototyping_sdk.cdk_graph": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk/cdk_graph/__init__.py` & `aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk/cdk_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk/cdk_graph/graph/__init__.py` & `aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk/cdk_graph/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk/cdk_graph/serialized_graph/__init__.py` & `aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk/cdk_graph/serialized_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk.cdk_graph.egg-info/PKG-INFO` & `aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk.cdk_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-prototyping-sdk.cdk-graph
-Version: 0.19.57
+Version: 0.19.58
 Summary: @aws-prototyping-sdk/cdk-graph
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws_prototyping_sdk.cdk_graph-0.19.57/src/aws_prototyping_sdk.cdk_graph.egg-info/SOURCES.txt` & `aws_prototyping_sdk.cdk_graph-0.19.58/src/aws_prototyping_sdk.cdk_graph.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 src/aws_prototyping_sdk.cdk_graph.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.cdk_graph.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.cdk_graph.egg-info/requires.txt
 src/aws_prototyping_sdk.cdk_graph.egg-info/top_level.txt
 src/aws_prototyping_sdk/cdk_graph/__init__.py
 src/aws_prototyping_sdk/cdk_graph/py.typed
 src/aws_prototyping_sdk/cdk_graph/_jsii/__init__.py
-src/aws_prototyping_sdk/cdk_graph/_jsii/cdk-graph@0.19.57.jsii.tgz
+src/aws_prototyping_sdk/cdk_graph/_jsii/cdk-graph@0.19.58.jsii.tgz
 src/aws_prototyping_sdk/cdk_graph/graph/__init__.py
 src/aws_prototyping_sdk/cdk_graph/serialized_graph/__init__.py
```

