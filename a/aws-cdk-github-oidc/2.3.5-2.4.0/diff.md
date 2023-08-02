# Comparing `tmp/aws-cdk-github-oidc-2.3.5.tar.gz` & `tmp/aws-cdk-github-oidc-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cdk-github-oidc-2.3.5.tar", last modified: Wed Aug  2 23:36:33 2023, max compression
+gzip compressed data, was "aws-cdk-github-oidc-2.4.0.tar", last modified: Wed Aug  2 23:48:17 2023, max compression
```

## Comparing `aws-cdk-github-oidc-2.3.5.tar` & `aws-cdk-github-oidc-2.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:36:33.344106 aws-cdk-github-oidc-2.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 23:36:20.000000 aws-cdk-github-oidc-2.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 23:36:20.000000 aws-cdk-github-oidc-2.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-02 23:36:33.344106 aws-cdk-github-oidc-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-08-02 23:36:20.000000 aws-cdk-github-oidc-2.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 23:36:20.000000 aws-cdk-github-oidc-2.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 23:36:33.344106 aws-cdk-github-oidc-2.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-02 23:36:20.000000 aws-cdk-github-oidc-2.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:36:33.340106 aws-cdk-github-oidc-2.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:36:33.340106 aws-cdk-github-oidc-2.3.5/src/aws_cdk_github_oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    56368 2023-08-02 23:36:20.000000 aws-cdk-github-oidc-2.3.5/src/aws_cdk_github_oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:36:33.344106 aws-cdk-github-oidc-2.3.5/src/aws_cdk_github_oidc/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-02 23:36:20.000000 aws-cdk-github-oidc-2.3.5/src/aws_cdk_github_oidc/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72092 2023-08-02 23:36:20.000000 aws-cdk-github-oidc-2.3.5/src/aws_cdk_github_oidc/_jsii/aws-cdk-github-oidc@2.3.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:36:20.000000 aws-cdk-github-oidc-2.3.5/src/aws_cdk_github_oidc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:36:33.340106 aws-cdk-github-oidc-2.3.5/src/aws_cdk_github_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-02 23:36:33.000000 aws-cdk-github-oidc-2.3.5/src/aws_cdk_github_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-02 23:36:33.000000 aws-cdk-github-oidc-2.3.5/src/aws_cdk_github_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:36:33.000000 aws-cdk-github-oidc-2.3.5/src/aws_cdk_github_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 23:36:33.000000 aws-cdk-github-oidc-2.3.5/src/aws_cdk_github_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 23:36:33.000000 aws-cdk-github-oidc-2.3.5/src/aws_cdk_github_oidc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:48:17.264299 aws-cdk-github-oidc-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-02 23:48:17.260299 aws-cdk-github-oidc-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 23:48:17.264299 aws-cdk-github-oidc-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:48:17.260299 aws-cdk-github-oidc-2.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:48:17.260299 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    56368 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:48:17.260299 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72070 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc/_jsii/aws-cdk-github-oidc@2.4.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:48:17.260299 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-02 23:48:17.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-02 23:48:17.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:48:17.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 23:48:17.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 23:48:17.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc.egg-info/top_level.txt
```

### Comparing `aws-cdk-github-oidc-2.3.5/LICENSE` & `aws-cdk-github-oidc-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk-github-oidc-2.3.5/PKG-INFO` & `aws-cdk-github-oidc-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-github-oidc
-Version: 2.3.5
+Version: 2.4.0
 Summary: CDK constructs to use OpenID Connect for authenticating your Github Action workflow with AWS IAM
 Home-page: https://github.com/aripalo/aws-cdk-github-oidc.git
 Author: Ari Palo<opensource@aripalo.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aripalo/aws-cdk-github-oidc.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk-github-oidc-2.3.5/README.md` & `aws-cdk-github-oidc-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk-github-oidc-2.3.5/setup.py` & `aws-cdk-github-oidc-2.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk-github-oidc",
-    "version": "2.3.5",
+    "version": "2.4.0",
     "description": "CDK constructs to use OpenID Connect for authenticating your Github Action workflow with AWS IAM",
     "license": "Apache-2.0",
     "url": "https://github.com/aripalo/aws-cdk-github-oidc.git",
     "long_description_content_type": "text/markdown",
     "author": "Ari Palo<opensource@aripalo.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_cdk_github_oidc",
         "aws_cdk_github_oidc._jsii"
     ],
     "package_data": {
         "aws_cdk_github_oidc._jsii": [
-            "aws-cdk-github-oidc@2.3.5.jsii.tgz"
+            "aws-cdk-github-oidc@2.4.0.jsii.tgz"
         ],
         "aws_cdk_github_oidc": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-cdk-github-oidc-2.3.5/src/aws_cdk_github_oidc/__init__.py` & `aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-github-oidc-2.3.5/src/aws_cdk_github_oidc.egg-info/PKG-INFO` & `aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-github-oidc
-Version: 2.3.5
+Version: 2.4.0
 Summary: CDK constructs to use OpenID Connect for authenticating your Github Action workflow with AWS IAM
 Home-page: https://github.com/aripalo/aws-cdk-github-oidc.git
 Author: Ari Palo<opensource@aripalo.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aripalo/aws-cdk-github-oidc.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

