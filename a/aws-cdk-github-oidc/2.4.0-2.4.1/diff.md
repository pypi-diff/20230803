# Comparing `tmp/aws-cdk-github-oidc-2.4.0.tar.gz` & `tmp/aws-cdk-github-oidc-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cdk-github-oidc-2.4.0.tar", last modified: Wed Aug  2 23:48:17 2023, max compression
+gzip compressed data, was "aws-cdk-github-oidc-2.4.1.tar", last modified: Wed Aug  2 23:55:26 2023, max compression
```

## Comparing `aws-cdk-github-oidc-2.4.0.tar` & `aws-cdk-github-oidc-2.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:48:17.264299 aws-cdk-github-oidc-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-02 23:48:17.260299 aws-cdk-github-oidc-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 23:48:17.264299 aws-cdk-github-oidc-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:48:17.260299 aws-cdk-github-oidc-2.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:48:17.260299 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    56368 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:48:17.260299 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72070 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc/_jsii/aws-cdk-github-oidc@2.4.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:48:04.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:48:17.260299 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-02 23:48:17.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-02 23:48:17.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:48:17.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 23:48:17.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 23:48:17.000000 aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:55:26.090714 aws-cdk-github-oidc-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 23:55:13.000000 aws-cdk-github-oidc-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 23:55:13.000000 aws-cdk-github-oidc-2.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-08-02 23:55:26.090714 aws-cdk-github-oidc-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-08-02 23:55:13.000000 aws-cdk-github-oidc-2.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 23:55:13.000000 aws-cdk-github-oidc-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 23:55:26.090714 aws-cdk-github-oidc-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-02 23:55:13.000000 aws-cdk-github-oidc-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:55:26.086714 aws-cdk-github-oidc-2.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:55:26.090714 aws-cdk-github-oidc-2.4.1/src/aws_cdk_github_oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    55572 2023-08-02 23:55:13.000000 aws-cdk-github-oidc-2.4.1/src/aws_cdk_github_oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:55:26.090714 aws-cdk-github-oidc-2.4.1/src/aws_cdk_github_oidc/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-02 23:55:13.000000 aws-cdk-github-oidc-2.4.1/src/aws_cdk_github_oidc/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71391 2023-08-02 23:55:13.000000 aws-cdk-github-oidc-2.4.1/src/aws_cdk_github_oidc/_jsii/aws-cdk-github-oidc@2.4.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:55:13.000000 aws-cdk-github-oidc-2.4.1/src/aws_cdk_github_oidc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:55:26.090714 aws-cdk-github-oidc-2.4.1/src/aws_cdk_github_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-08-02 23:55:26.000000 aws-cdk-github-oidc-2.4.1/src/aws_cdk_github_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-02 23:55:26.000000 aws-cdk-github-oidc-2.4.1/src/aws_cdk_github_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:55:26.000000 aws-cdk-github-oidc-2.4.1/src/aws_cdk_github_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 23:55:26.000000 aws-cdk-github-oidc-2.4.1/src/aws_cdk_github_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 23:55:26.000000 aws-cdk-github-oidc-2.4.1/src/aws_cdk_github_oidc.egg-info/top_level.txt
```

### Comparing `aws-cdk-github-oidc-2.4.0/LICENSE` & `aws-cdk-github-oidc-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk-github-oidc-2.4.0/PKG-INFO` & `aws-cdk-github-oidc-2.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-github-oidc
-Version: 2.4.0
+Version: 2.4.1
 Summary: CDK constructs to use OpenID Connect for authenticating your Github Action workflow with AWS IAM
 Home-page: https://github.com/aripalo/aws-cdk-github-oidc.git
 Author: Ari Palo<opensource@aripalo.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aripalo/aws-cdk-github-oidc.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -164,15 +164,7 @@
 
       - name: Sync files to S3
         run: |
           aws s3 sync . s3://my-example-bucket
 ```
 
 <br/>
-
-### Development Status
-
-These constructs are fresh out from the oven, since [Github just announced](https://github.blog/changelog/2021-10-27-github-actions-secure-cloud-deployments-with-openid-connect/) the OpenID Connect feature as generally available. I've been playing around with the feature for some time, but the construct itself haven't yet been widely used.
-
-These constructs will stay in `v0.x.x` for a while, to allow easier bug fixing & breaking changes *if absolutely needed*. Once bugs are fixed (if any), the constructs will be published with `v1` major version and will be marked as stable.
-
-Currently only TypeScript, Python and Go versions provided, but before going to stable, I'll probably others (supported by JSII) depending on the amount of work required - so no promises!
```

### Comparing `aws-cdk-github-oidc-2.4.0/README.md` & `aws-cdk-github-oidc-2.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -140,15 +140,7 @@
 
       - name: Sync files to S3
         run: |
           aws s3 sync . s3://my-example-bucket
 ```
 
 <br/>
-
-### Development Status
-
-These constructs are fresh out from the oven, since [Github just announced](https://github.blog/changelog/2021-10-27-github-actions-secure-cloud-deployments-with-openid-connect/) the OpenID Connect feature as generally available. I've been playing around with the feature for some time, but the construct itself haven't yet been widely used.
-
-These constructs will stay in `v0.x.x` for a while, to allow easier bug fixing & breaking changes *if absolutely needed*. Once bugs are fixed (if any), the constructs will be published with `v1` major version and will be marked as stable.
-
-Currently only TypeScript, Python and Go versions provided, but before going to stable, I'll probably others (supported by JSII) depending on the amount of work required - so no promises!
```

### Comparing `aws-cdk-github-oidc-2.4.0/setup.py` & `aws-cdk-github-oidc-2.4.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk-github-oidc",
-    "version": "2.4.0",
+    "version": "2.4.1",
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
-            "aws-cdk-github-oidc@2.4.0.jsii.tgz"
+            "aws-cdk-github-oidc@2.4.1.jsii.tgz"
         ],
         "aws_cdk_github_oidc": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc/__init__.py` & `aws-cdk-github-oidc-2.4.1/src/aws_cdk_github_oidc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,22 +141,14 @@
 
       - name: Sync files to S3
         run: |
           aws s3 sync . s3://my-example-bucket
 ```
 
 <br/>
-
-### Development Status
-
-These constructs are fresh out from the oven, since [Github just announced](https://github.blog/changelog/2021-10-27-github-actions-secure-cloud-deployments-with-openid-connect/) the OpenID Connect feature as generally available. I've been playing around with the feature for some time, but the construct itself haven't yet been widely used.
-
-These constructs will stay in `v0.x.x` for a while, to allow easier bug fixing & breaking changes *if absolutely needed*. Once bugs are fixed (if any), the constructs will be published with `v1` major version and will be marked as stable.
-
-Currently only TypeScript, Python and Go versions provided, but before going to stable, I'll probably others (supported by JSII) depending on the amount of work required - so no promises!
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
```

### Comparing `aws-cdk-github-oidc-2.4.0/src/aws_cdk_github_oidc.egg-info/PKG-INFO` & `aws-cdk-github-oidc-2.4.1/src/aws_cdk_github_oidc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-github-oidc
-Version: 2.4.0
+Version: 2.4.1
 Summary: CDK constructs to use OpenID Connect for authenticating your Github Action workflow with AWS IAM
 Home-page: https://github.com/aripalo/aws-cdk-github-oidc.git
 Author: Ari Palo<opensource@aripalo.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aripalo/aws-cdk-github-oidc.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -164,15 +164,7 @@
 
       - name: Sync files to S3
         run: |
           aws s3 sync . s3://my-example-bucket
 ```
 
 <br/>
-
-### Development Status
-
-These constructs are fresh out from the oven, since [Github just announced](https://github.blog/changelog/2021-10-27-github-actions-secure-cloud-deployments-with-openid-connect/) the OpenID Connect feature as generally available. I've been playing around with the feature for some time, but the construct itself haven't yet been widely used.
-
-These constructs will stay in `v0.x.x` for a while, to allow easier bug fixing & breaking changes *if absolutely needed*. Once bugs are fixed (if any), the constructs will be published with `v1` major version and will be marked as stable.
-
-Currently only TypeScript, Python and Go versions provided, but before going to stable, I'll probably others (supported by JSII) depending on the amount of work required - so no promises!
```

