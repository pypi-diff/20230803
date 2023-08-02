# Comparing `tmp/aws-cdk-github-oidc-2.3.3.tar.gz` & `tmp/aws-cdk-github-oidc-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cdk-github-oidc-2.3.3.tar", last modified: Wed Aug  2 23:01:08 2023, max compression
+gzip compressed data, was "aws-cdk-github-oidc-2.3.4.tar", last modified: Wed Aug  2 23:31:27 2023, max compression
```

## Comparing `aws-cdk-github-oidc-2.3.3.tar` & `aws-cdk-github-oidc-2.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:01:08.417246 aws-cdk-github-oidc-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 23:00:56.000000 aws-cdk-github-oidc-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 23:00:56.000000 aws-cdk-github-oidc-2.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-08-02 23:01:08.417246 aws-cdk-github-oidc-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-08-02 23:00:56.000000 aws-cdk-github-oidc-2.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 23:00:56.000000 aws-cdk-github-oidc-2.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 23:01:08.417246 aws-cdk-github-oidc-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-02 23:00:56.000000 aws-cdk-github-oidc-2.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:01:08.417246 aws-cdk-github-oidc-2.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:01:08.417246 aws-cdk-github-oidc-2.3.3/src/aws_cdk_github_oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    56711 2023-08-02 23:00:56.000000 aws-cdk-github-oidc-2.3.3/src/aws_cdk_github_oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:01:08.417246 aws-cdk-github-oidc-2.3.3/src/aws_cdk_github_oidc/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-02 23:00:56.000000 aws-cdk-github-oidc-2.3.3/src/aws_cdk_github_oidc/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72704 2023-08-02 23:00:56.000000 aws-cdk-github-oidc-2.3.3/src/aws_cdk_github_oidc/_jsii/aws-cdk-github-oidc@2.3.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:00:56.000000 aws-cdk-github-oidc-2.3.3/src/aws_cdk_github_oidc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:01:08.417246 aws-cdk-github-oidc-2.3.3/src/aws_cdk_github_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-08-02 23:01:08.000000 aws-cdk-github-oidc-2.3.3/src/aws_cdk_github_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-02 23:01:08.000000 aws-cdk-github-oidc-2.3.3/src/aws_cdk_github_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:01:08.000000 aws-cdk-github-oidc-2.3.3/src/aws_cdk_github_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 23:01:08.000000 aws-cdk-github-oidc-2.3.3/src/aws_cdk_github_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 23:01:08.000000 aws-cdk-github-oidc-2.3.3/src/aws_cdk_github_oidc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:27.675873 aws-cdk-github-oidc-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 23:31:16.000000 aws-cdk-github-oidc-2.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 23:31:16.000000 aws-cdk-github-oidc-2.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-02 23:31:27.675873 aws-cdk-github-oidc-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-08-02 23:31:16.000000 aws-cdk-github-oidc-2.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 23:31:16.000000 aws-cdk-github-oidc-2.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 23:31:27.675873 aws-cdk-github-oidc-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-02 23:31:16.000000 aws-cdk-github-oidc-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:27.675873 aws-cdk-github-oidc-2.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:27.675873 aws-cdk-github-oidc-2.3.4/src/aws_cdk_github_oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    56368 2023-08-02 23:31:16.000000 aws-cdk-github-oidc-2.3.4/src/aws_cdk_github_oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:27.675873 aws-cdk-github-oidc-2.3.4/src/aws_cdk_github_oidc/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-02 23:31:16.000000 aws-cdk-github-oidc-2.3.4/src/aws_cdk_github_oidc/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72346 2023-08-02 23:31:16.000000 aws-cdk-github-oidc-2.3.4/src/aws_cdk_github_oidc/_jsii/aws-cdk-github-oidc@2.3.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:31:16.000000 aws-cdk-github-oidc-2.3.4/src/aws_cdk_github_oidc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:27.675873 aws-cdk-github-oidc-2.3.4/src/aws_cdk_github_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-02 23:31:27.000000 aws-cdk-github-oidc-2.3.4/src/aws_cdk_github_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-02 23:31:27.000000 aws-cdk-github-oidc-2.3.4/src/aws_cdk_github_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:31:27.000000 aws-cdk-github-oidc-2.3.4/src/aws_cdk_github_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 23:31:27.000000 aws-cdk-github-oidc-2.3.4/src/aws_cdk_github_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 23:31:27.000000 aws-cdk-github-oidc-2.3.4/src/aws_cdk_github_oidc.egg-info/top_level.txt
```

### Comparing `aws-cdk-github-oidc-2.3.3/LICENSE` & `aws-cdk-github-oidc-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk-github-oidc-2.3.3/PKG-INFO` & `aws-cdk-github-oidc-2.3.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-github-oidc
-Version: 2.3.3
+Version: 2.3.4
 Summary: CDK constructs to use OpenID Connect for authenticating your Github Action workflow with AWS IAM
 Home-page: https://github.com/aripalo/aws-cdk-github-oidc.git
 Author: Ari Palo<opensource@aripalo.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aripalo/aws-cdk-github-oidc.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -59,75 +59,80 @@
 <br/>
 
 ### OpenID Connect Identity Provider trust for AWS IAM
 
 To create a new Github OIDC provider configuration into AWS IAM:
 
 ```python
-import { GithubActionsIdentityProvider } from 'aws-cdk-github-oidc';
+import { GithubActionsIdentityProvider } from "aws-cdk-github-oidc";
 
-const provider = new GithubActionsIdentityProvider(scope, 'GithubProvider');
+const provider = new GithubActionsIdentityProvider(scope, "GithubProvider");
 ```
 
-In the background this creates an OIDC provider trust configuration into AWS IAM with an [issuer URL of `https://token.actions.githubusercontent.com`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws), audiences (client IDs) configured as `['sts.amazonaws.com']` (which matches the [`aws-actions/configure-aws-credentials`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws) implementation) and the thumbprint as Github's `a031c46782e6e6c662c2c87c76da9aa62ccabd8e`
+In the background this creates an OIDC provider trust configuration into AWS IAM with an [issuer URL of `https://token.actions.githubusercontent.com`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws) and audiences (client IDs) configured as `['sts.amazonaws.com']` (which matches the [`aws-actions/configure-aws-credentials`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws) implementation).
 
 <br/>
 
 ### Retrieving a reference to an existing Github OIDC provider configuration
 
 Remember, **there can be only one (Github OIDC provider per AWS Account)**, so to retrieve a reference to existing Github OIDC provider use `fromAccount` static method:
 
 ```python
-import { GithubActionsIdentityProvider } from 'aws-cdk-github-oidc';
+import { GithubActionsIdentityProvider } from "aws-cdk-github-oidc";
 
-const provider = GithubActionsIdentityProvider.fromAccount(scope, 'GithubProvider');
+const provider = GithubActionsIdentityProvider.fromAccount(
+  scope,
+  "GithubProvider"
+);
 ```
 
 <br/>
 
 ### Defining a role for Github Actions workflow to assume
 
 ```python
-import { GithubActionsRole } from 'aws-cdk-github-oidc';
+import { GithubActionsRole } from "aws-cdk-github-oidc";
 
-const uploadRole = new GithubActionsRole(scope, 'UploadRole', {
-  provider: provider,           // reference into the OIDC provider
-  owner: 'octo-org',            // your repository owner (organization or user) name
-  repo: 'octo-repo',            // your repository name (without the owner name)
-  filter: 'ref:refs/tags/v*',   // JWT sub suffix filter, defaults to '*'
+const uploadRole = new GithubActionsRole(scope, "UploadRole", {
+  provider: provider, // reference into the OIDC provider
+  owner: "octo-org", // your repository owner (organization or user) name
+  repo: "octo-repo", // your repository name (without the owner name)
+  filter: "ref:refs/tags/v*", // JWT sub suffix filter, defaults to '*'
 });
 
 // use it like any other role, for example grant S3 bucket write access:
 myBucket.grantWrite(uploadRole);
 ```
 
 You may pass in any `iam.RoleProps` into the construct's props, except `assumedBy` which will be defined by this construct (CDK will fail if you do):
 
 ```python
-const deployRole = new GithubActionsRole(scope, 'DeployRole', {
+const deployRole = new GithubActionsRole(scope, "DeployRole", {
   provider: provider,
-  owner: 'octo-org',
-  repo: 'octo-repo',
-  roleName: 'MyDeployRole',
-  description: 'This role deploys stuff to AWS',
+  owner: "octo-org",
+  repo: "octo-repo",
+  roleName: "MyDeployRole",
+  description: "This role deploys stuff to AWS",
   maxSessionDuration: cdk.Duration.hours(2),
 });
 
 // You may also use various "add*" policy methods!
 // "AdministratorAccess" not really a good idea, just for an example here:
-deployRole.addManagedPolicy(iam.ManagedPolicy.fromAwsManagedPolicyName('AdministratorAccess'));
+deployRole.addManagedPolicy(
+  iam.ManagedPolicy.fromAwsManagedPolicyName("AdministratorAccess")
+);
 ```
 
 <br/>
 
 #### Subject Filter
 
 By default the value of `filter` property will be `'*'` which means any workflow (from given repository) from any branch, tag, environment or pull request can assume this role. To further stricten the OIDC trust policy on the role, you may adjust the subject filter as seen on the [examples in Github Docs](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/about-security-hardening-with-openid-connect#configuring-the-oidc-trust-with-the-cloud); For example:
 
-|         `filter` value         |                Descrition                |
+| `filter` value                 | Descrition                               |
 | :----------------------------- | :--------------------------------------- |
 | `'ref:refs/tags/v*'`           | Allow only tags with prefix of `v`       |
 | `'ref:refs/heads/demo-branch'` | Allow only from branch `demo-branch`     |
 | `'pull_request'`               | Allow only from pull request             |
 | `'environment:Production'`     | Allow only from `Production` environment |
 
 <br/>
@@ -143,27 +148,27 @@
   deploy:
     name: Upload to Amazon S3
     runs-on: ubuntu-latest
     permissions:
       id-token: write # needed to interact with GitHub's OIDC Token endpoint.
       contents: read
     steps:
-    - name: Checkout
-      uses: actions/checkout@v2
+      - name: Checkout
+        uses: actions/checkout@v2
 
-    - name: Configure AWS credentials
-      uses: aws-actions/configure-aws-credentials@master
-      with:
-        role-to-assume: arn:aws:iam::123456789012:role/MyUploadRole
-        #role-session-name: MySessionName # Optional
-        aws-region: us-east-1
-
-    - name: Sync files to S3
-      run: |
-        aws s3 sync . s3://my-example-bucket
+      - name: Configure AWS credentials
+        uses: aws-actions/configure-aws-credentials@master
+        with:
+          role-to-assume: arn:aws:iam::123456789012:role/MyUploadRole
+          #role-session-name: MySessionName # Optional
+          aws-region: us-east-1
+
+      - name: Sync files to S3
+        run: |
+          aws s3 sync . s3://my-example-bucket
 ```
 
 <br/>
 
 ### Development Status
 
 These constructs are fresh out from the oven, since [Github just announced](https://github.blog/changelog/2021-10-27-github-actions-secure-cloud-deployments-with-openid-connect/) the OpenID Connect feature as generally available. I've been playing around with the feature for some time, but the construct itself haven't yet been widely used.
```

### Comparing `aws-cdk-github-oidc-2.3.3/README.md` & `aws-cdk-github-oidc-2.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,75 +35,80 @@
 <br/>
 
 ### OpenID Connect Identity Provider trust for AWS IAM
 
 To create a new Github OIDC provider configuration into AWS IAM:
 
 ```python
-import { GithubActionsIdentityProvider } from 'aws-cdk-github-oidc';
+import { GithubActionsIdentityProvider } from "aws-cdk-github-oidc";
 
-const provider = new GithubActionsIdentityProvider(scope, 'GithubProvider');
+const provider = new GithubActionsIdentityProvider(scope, "GithubProvider");
 ```
 
-In the background this creates an OIDC provider trust configuration into AWS IAM with an [issuer URL of `https://token.actions.githubusercontent.com`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws), audiences (client IDs) configured as `['sts.amazonaws.com']` (which matches the [`aws-actions/configure-aws-credentials`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws) implementation) and the thumbprint as Github's `a031c46782e6e6c662c2c87c76da9aa62ccabd8e`
+In the background this creates an OIDC provider trust configuration into AWS IAM with an [issuer URL of `https://token.actions.githubusercontent.com`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws) and audiences (client IDs) configured as `['sts.amazonaws.com']` (which matches the [`aws-actions/configure-aws-credentials`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws) implementation).
 
 <br/>
 
 ### Retrieving a reference to an existing Github OIDC provider configuration
 
 Remember, **there can be only one (Github OIDC provider per AWS Account)**, so to retrieve a reference to existing Github OIDC provider use `fromAccount` static method:
 
 ```python
-import { GithubActionsIdentityProvider } from 'aws-cdk-github-oidc';
+import { GithubActionsIdentityProvider } from "aws-cdk-github-oidc";
 
-const provider = GithubActionsIdentityProvider.fromAccount(scope, 'GithubProvider');
+const provider = GithubActionsIdentityProvider.fromAccount(
+  scope,
+  "GithubProvider"
+);
 ```
 
 <br/>
 
 ### Defining a role for Github Actions workflow to assume
 
 ```python
-import { GithubActionsRole } from 'aws-cdk-github-oidc';
+import { GithubActionsRole } from "aws-cdk-github-oidc";
 
-const uploadRole = new GithubActionsRole(scope, 'UploadRole', {
-  provider: provider,           // reference into the OIDC provider
-  owner: 'octo-org',            // your repository owner (organization or user) name
-  repo: 'octo-repo',            // your repository name (without the owner name)
-  filter: 'ref:refs/tags/v*',   // JWT sub suffix filter, defaults to '*'
+const uploadRole = new GithubActionsRole(scope, "UploadRole", {
+  provider: provider, // reference into the OIDC provider
+  owner: "octo-org", // your repository owner (organization or user) name
+  repo: "octo-repo", // your repository name (without the owner name)
+  filter: "ref:refs/tags/v*", // JWT sub suffix filter, defaults to '*'
 });
 
 // use it like any other role, for example grant S3 bucket write access:
 myBucket.grantWrite(uploadRole);
 ```
 
 You may pass in any `iam.RoleProps` into the construct's props, except `assumedBy` which will be defined by this construct (CDK will fail if you do):
 
 ```python
-const deployRole = new GithubActionsRole(scope, 'DeployRole', {
+const deployRole = new GithubActionsRole(scope, "DeployRole", {
   provider: provider,
-  owner: 'octo-org',
-  repo: 'octo-repo',
-  roleName: 'MyDeployRole',
-  description: 'This role deploys stuff to AWS',
+  owner: "octo-org",
+  repo: "octo-repo",
+  roleName: "MyDeployRole",
+  description: "This role deploys stuff to AWS",
   maxSessionDuration: cdk.Duration.hours(2),
 });
 
 // You may also use various "add*" policy methods!
 // "AdministratorAccess" not really a good idea, just for an example here:
-deployRole.addManagedPolicy(iam.ManagedPolicy.fromAwsManagedPolicyName('AdministratorAccess'));
+deployRole.addManagedPolicy(
+  iam.ManagedPolicy.fromAwsManagedPolicyName("AdministratorAccess")
+);
 ```
 
 <br/>
 
 #### Subject Filter
 
 By default the value of `filter` property will be `'*'` which means any workflow (from given repository) from any branch, tag, environment or pull request can assume this role. To further stricten the OIDC trust policy on the role, you may adjust the subject filter as seen on the [examples in Github Docs](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/about-security-hardening-with-openid-connect#configuring-the-oidc-trust-with-the-cloud); For example:
 
-|         `filter` value         |                Descrition                |
+| `filter` value                 | Descrition                               |
 | :----------------------------- | :--------------------------------------- |
 | `'ref:refs/tags/v*'`           | Allow only tags with prefix of `v`       |
 | `'ref:refs/heads/demo-branch'` | Allow only from branch `demo-branch`     |
 | `'pull_request'`               | Allow only from pull request             |
 | `'environment:Production'`     | Allow only from `Production` environment |
 
 <br/>
@@ -119,27 +124,27 @@
   deploy:
     name: Upload to Amazon S3
     runs-on: ubuntu-latest
     permissions:
       id-token: write # needed to interact with GitHub's OIDC Token endpoint.
       contents: read
     steps:
-    - name: Checkout
-      uses: actions/checkout@v2
+      - name: Checkout
+        uses: actions/checkout@v2
 
-    - name: Configure AWS credentials
-      uses: aws-actions/configure-aws-credentials@master
-      with:
-        role-to-assume: arn:aws:iam::123456789012:role/MyUploadRole
-        #role-session-name: MySessionName # Optional
-        aws-region: us-east-1
-
-    - name: Sync files to S3
-      run: |
-        aws s3 sync . s3://my-example-bucket
+      - name: Configure AWS credentials
+        uses: aws-actions/configure-aws-credentials@master
+        with:
+          role-to-assume: arn:aws:iam::123456789012:role/MyUploadRole
+          #role-session-name: MySessionName # Optional
+          aws-region: us-east-1
+
+      - name: Sync files to S3
+        run: |
+          aws s3 sync . s3://my-example-bucket
 ```
 
 <br/>
 
 ### Development Status
 
 These constructs are fresh out from the oven, since [Github just announced](https://github.blog/changelog/2021-10-27-github-actions-secure-cloud-deployments-with-openid-connect/) the OpenID Connect feature as generally available. I've been playing around with the feature for some time, but the construct itself haven't yet been widely used.
```

### Comparing `aws-cdk-github-oidc-2.3.3/setup.py` & `aws-cdk-github-oidc-2.3.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk-github-oidc",
-    "version": "2.3.3",
+    "version": "2.3.4",
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
-            "aws-cdk-github-oidc@2.3.3.jsii.tgz"
+            "aws-cdk-github-oidc@2.3.4.jsii.tgz"
         ],
         "aws_cdk_github_oidc": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-cdk-github-oidc-2.3.3/src/aws_cdk_github_oidc/__init__.py` & `aws-cdk-github-oidc-2.3.4/src/aws_cdk_github_oidc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,75 +36,80 @@
 <br/>
 
 ### OpenID Connect Identity Provider trust for AWS IAM
 
 To create a new Github OIDC provider configuration into AWS IAM:
 
 ```python
-import { GithubActionsIdentityProvider } from 'aws-cdk-github-oidc';
+import { GithubActionsIdentityProvider } from "aws-cdk-github-oidc";
 
-const provider = new GithubActionsIdentityProvider(scope, 'GithubProvider');
+const provider = new GithubActionsIdentityProvider(scope, "GithubProvider");
 ```
 
-In the background this creates an OIDC provider trust configuration into AWS IAM with an [issuer URL of `https://token.actions.githubusercontent.com`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws), audiences (client IDs) configured as `['sts.amazonaws.com']` (which matches the [`aws-actions/configure-aws-credentials`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws) implementation) and the thumbprint as Github's `a031c46782e6e6c662c2c87c76da9aa62ccabd8e`
+In the background this creates an OIDC provider trust configuration into AWS IAM with an [issuer URL of `https://token.actions.githubusercontent.com`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws) and audiences (client IDs) configured as `['sts.amazonaws.com']` (which matches the [`aws-actions/configure-aws-credentials`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws) implementation).
 
 <br/>
 
 ### Retrieving a reference to an existing Github OIDC provider configuration
 
 Remember, **there can be only one (Github OIDC provider per AWS Account)**, so to retrieve a reference to existing Github OIDC provider use `fromAccount` static method:
 
 ```python
-import { GithubActionsIdentityProvider } from 'aws-cdk-github-oidc';
+import { GithubActionsIdentityProvider } from "aws-cdk-github-oidc";
 
-const provider = GithubActionsIdentityProvider.fromAccount(scope, 'GithubProvider');
+const provider = GithubActionsIdentityProvider.fromAccount(
+  scope,
+  "GithubProvider"
+);
 ```
 
 <br/>
 
 ### Defining a role for Github Actions workflow to assume
 
 ```python
-import { GithubActionsRole } from 'aws-cdk-github-oidc';
+import { GithubActionsRole } from "aws-cdk-github-oidc";
 
-const uploadRole = new GithubActionsRole(scope, 'UploadRole', {
-  provider: provider,           // reference into the OIDC provider
-  owner: 'octo-org',            // your repository owner (organization or user) name
-  repo: 'octo-repo',            // your repository name (without the owner name)
-  filter: 'ref:refs/tags/v*',   // JWT sub suffix filter, defaults to '*'
+const uploadRole = new GithubActionsRole(scope, "UploadRole", {
+  provider: provider, // reference into the OIDC provider
+  owner: "octo-org", // your repository owner (organization or user) name
+  repo: "octo-repo", // your repository name (without the owner name)
+  filter: "ref:refs/tags/v*", // JWT sub suffix filter, defaults to '*'
 });
 
 // use it like any other role, for example grant S3 bucket write access:
 myBucket.grantWrite(uploadRole);
 ```
 
 You may pass in any `iam.RoleProps` into the construct's props, except `assumedBy` which will be defined by this construct (CDK will fail if you do):
 
 ```python
-const deployRole = new GithubActionsRole(scope, 'DeployRole', {
+const deployRole = new GithubActionsRole(scope, "DeployRole", {
   provider: provider,
-  owner: 'octo-org',
-  repo: 'octo-repo',
-  roleName: 'MyDeployRole',
-  description: 'This role deploys stuff to AWS',
+  owner: "octo-org",
+  repo: "octo-repo",
+  roleName: "MyDeployRole",
+  description: "This role deploys stuff to AWS",
   maxSessionDuration: cdk.Duration.hours(2),
 });
 
 // You may also use various "add*" policy methods!
 // "AdministratorAccess" not really a good idea, just for an example here:
-deployRole.addManagedPolicy(iam.ManagedPolicy.fromAwsManagedPolicyName('AdministratorAccess'));
+deployRole.addManagedPolicy(
+  iam.ManagedPolicy.fromAwsManagedPolicyName("AdministratorAccess")
+);
 ```
 
 <br/>
 
 #### Subject Filter
 
 By default the value of `filter` property will be `'*'` which means any workflow (from given repository) from any branch, tag, environment or pull request can assume this role. To further stricten the OIDC trust policy on the role, you may adjust the subject filter as seen on the [examples in Github Docs](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/about-security-hardening-with-openid-connect#configuring-the-oidc-trust-with-the-cloud); For example:
 
-|         `filter` value         |                Descrition                |
+| `filter` value                 | Descrition                               |
 | :----------------------------- | :--------------------------------------- |
 | `'ref:refs/tags/v*'`           | Allow only tags with prefix of `v`       |
 | `'ref:refs/heads/demo-branch'` | Allow only from branch `demo-branch`     |
 | `'pull_request'`               | Allow only from pull request             |
 | `'environment:Production'`     | Allow only from `Production` environment |
 
 <br/>
@@ -120,27 +125,27 @@
   deploy:
     name: Upload to Amazon S3
     runs-on: ubuntu-latest
     permissions:
       id-token: write # needed to interact with GitHub's OIDC Token endpoint.
       contents: read
     steps:
-    - name: Checkout
-      uses: actions/checkout@v2
+      - name: Checkout
+        uses: actions/checkout@v2
 
-    - name: Configure AWS credentials
-      uses: aws-actions/configure-aws-credentials@master
-      with:
-        role-to-assume: arn:aws:iam::123456789012:role/MyUploadRole
-        #role-session-name: MySessionName # Optional
-        aws-region: us-east-1
-
-    - name: Sync files to S3
-      run: |
-        aws s3 sync . s3://my-example-bucket
+      - name: Configure AWS credentials
+        uses: aws-actions/configure-aws-credentials@master
+        with:
+          role-to-assume: arn:aws:iam::123456789012:role/MyUploadRole
+          #role-session-name: MySessionName # Optional
+          aws-region: us-east-1
+
+      - name: Sync files to S3
+        run: |
+          aws s3 sync . s3://my-example-bucket
 ```
 
 <br/>
 
 ### Development Status
 
 These constructs are fresh out from the oven, since [Github just announced](https://github.blog/changelog/2021-10-27-github-actions-secure-cloud-deployments-with-openid-connect/) the OpenID Connect feature as generally available. I've been playing around with the feature for some time, but the construct itself haven't yet been widely used.
@@ -696,22 +701,14 @@
     @jsii.member(jsii_name="issuer")
     def ISSUER(cls) -> builtins.str:
         '''
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.sget(cls, "issuer"))
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="thumbprints")
-    def THUMBPRINTS(cls) -> typing.List[builtins.str]:
-        '''
-        :stability: experimental
-        '''
-        return typing.cast(typing.List[builtins.str], jsii.sget(cls, "thumbprints"))
-
 
 @jsii.data_type(
     jsii_type="aws-cdk-github-oidc.GithubActionsRoleProps",
     jsii_struct_bases=[GithubConfiguration, RoleProps],
     name_mapping={
         "owner": "owner",
         "provider": "provider",
```

### Comparing `aws-cdk-github-oidc-2.3.3/src/aws_cdk_github_oidc.egg-info/PKG-INFO` & `aws-cdk-github-oidc-2.3.4/src/aws_cdk_github_oidc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-github-oidc
-Version: 2.3.3
+Version: 2.3.4
 Summary: CDK constructs to use OpenID Connect for authenticating your Github Action workflow with AWS IAM
 Home-page: https://github.com/aripalo/aws-cdk-github-oidc.git
 Author: Ari Palo<opensource@aripalo.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aripalo/aws-cdk-github-oidc.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -59,75 +59,80 @@
 <br/>
 
 ### OpenID Connect Identity Provider trust for AWS IAM
 
 To create a new Github OIDC provider configuration into AWS IAM:
 
 ```python
-import { GithubActionsIdentityProvider } from 'aws-cdk-github-oidc';
+import { GithubActionsIdentityProvider } from "aws-cdk-github-oidc";
 
-const provider = new GithubActionsIdentityProvider(scope, 'GithubProvider');
+const provider = new GithubActionsIdentityProvider(scope, "GithubProvider");
 ```
 
-In the background this creates an OIDC provider trust configuration into AWS IAM with an [issuer URL of `https://token.actions.githubusercontent.com`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws), audiences (client IDs) configured as `['sts.amazonaws.com']` (which matches the [`aws-actions/configure-aws-credentials`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws) implementation) and the thumbprint as Github's `a031c46782e6e6c662c2c87c76da9aa62ccabd8e`
+In the background this creates an OIDC provider trust configuration into AWS IAM with an [issuer URL of `https://token.actions.githubusercontent.com`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws) and audiences (client IDs) configured as `['sts.amazonaws.com']` (which matches the [`aws-actions/configure-aws-credentials`](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#adding-the-identity-provider-to-aws) implementation).
 
 <br/>
 
 ### Retrieving a reference to an existing Github OIDC provider configuration
 
 Remember, **there can be only one (Github OIDC provider per AWS Account)**, so to retrieve a reference to existing Github OIDC provider use `fromAccount` static method:
 
 ```python
-import { GithubActionsIdentityProvider } from 'aws-cdk-github-oidc';
+import { GithubActionsIdentityProvider } from "aws-cdk-github-oidc";
 
-const provider = GithubActionsIdentityProvider.fromAccount(scope, 'GithubProvider');
+const provider = GithubActionsIdentityProvider.fromAccount(
+  scope,
+  "GithubProvider"
+);
 ```
 
 <br/>
 
 ### Defining a role for Github Actions workflow to assume
 
 ```python
-import { GithubActionsRole } from 'aws-cdk-github-oidc';
+import { GithubActionsRole } from "aws-cdk-github-oidc";
 
-const uploadRole = new GithubActionsRole(scope, 'UploadRole', {
-  provider: provider,           // reference into the OIDC provider
-  owner: 'octo-org',            // your repository owner (organization or user) name
-  repo: 'octo-repo',            // your repository name (without the owner name)
-  filter: 'ref:refs/tags/v*',   // JWT sub suffix filter, defaults to '*'
+const uploadRole = new GithubActionsRole(scope, "UploadRole", {
+  provider: provider, // reference into the OIDC provider
+  owner: "octo-org", // your repository owner (organization or user) name
+  repo: "octo-repo", // your repository name (without the owner name)
+  filter: "ref:refs/tags/v*", // JWT sub suffix filter, defaults to '*'
 });
 
 // use it like any other role, for example grant S3 bucket write access:
 myBucket.grantWrite(uploadRole);
 ```
 
 You may pass in any `iam.RoleProps` into the construct's props, except `assumedBy` which will be defined by this construct (CDK will fail if you do):
 
 ```python
-const deployRole = new GithubActionsRole(scope, 'DeployRole', {
+const deployRole = new GithubActionsRole(scope, "DeployRole", {
   provider: provider,
-  owner: 'octo-org',
-  repo: 'octo-repo',
-  roleName: 'MyDeployRole',
-  description: 'This role deploys stuff to AWS',
+  owner: "octo-org",
+  repo: "octo-repo",
+  roleName: "MyDeployRole",
+  description: "This role deploys stuff to AWS",
   maxSessionDuration: cdk.Duration.hours(2),
 });
 
 // You may also use various "add*" policy methods!
 // "AdministratorAccess" not really a good idea, just for an example here:
-deployRole.addManagedPolicy(iam.ManagedPolicy.fromAwsManagedPolicyName('AdministratorAccess'));
+deployRole.addManagedPolicy(
+  iam.ManagedPolicy.fromAwsManagedPolicyName("AdministratorAccess")
+);
 ```
 
 <br/>
 
 #### Subject Filter
 
 By default the value of `filter` property will be `'*'` which means any workflow (from given repository) from any branch, tag, environment or pull request can assume this role. To further stricten the OIDC trust policy on the role, you may adjust the subject filter as seen on the [examples in Github Docs](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/about-security-hardening-with-openid-connect#configuring-the-oidc-trust-with-the-cloud); For example:
 
-|         `filter` value         |                Descrition                |
+| `filter` value                 | Descrition                               |
 | :----------------------------- | :--------------------------------------- |
 | `'ref:refs/tags/v*'`           | Allow only tags with prefix of `v`       |
 | `'ref:refs/heads/demo-branch'` | Allow only from branch `demo-branch`     |
 | `'pull_request'`               | Allow only from pull request             |
 | `'environment:Production'`     | Allow only from `Production` environment |
 
 <br/>
@@ -143,27 +148,27 @@
   deploy:
     name: Upload to Amazon S3
     runs-on: ubuntu-latest
     permissions:
       id-token: write # needed to interact with GitHub's OIDC Token endpoint.
       contents: read
     steps:
-    - name: Checkout
-      uses: actions/checkout@v2
+      - name: Checkout
+        uses: actions/checkout@v2
 
-    - name: Configure AWS credentials
-      uses: aws-actions/configure-aws-credentials@master
-      with:
-        role-to-assume: arn:aws:iam::123456789012:role/MyUploadRole
-        #role-session-name: MySessionName # Optional
-        aws-region: us-east-1
-
-    - name: Sync files to S3
-      run: |
-        aws s3 sync . s3://my-example-bucket
+      - name: Configure AWS credentials
+        uses: aws-actions/configure-aws-credentials@master
+        with:
+          role-to-assume: arn:aws:iam::123456789012:role/MyUploadRole
+          #role-session-name: MySessionName # Optional
+          aws-region: us-east-1
+
+      - name: Sync files to S3
+        run: |
+          aws s3 sync . s3://my-example-bucket
 ```
 
 <br/>
 
 ### Development Status
 
 These constructs are fresh out from the oven, since [Github just announced](https://github.blog/changelog/2021-10-27-github-actions-secure-cloud-deployments-with-openid-connect/) the OpenID Connect feature as generally available. I've been playing around with the feature for some time, but the construct itself haven't yet been widely used.
```

