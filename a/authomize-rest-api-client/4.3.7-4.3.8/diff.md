# Comparing `tmp/authomize-rest-api-client-4.3.7.tar.gz` & `tmp/authomize-rest-api-client-4.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.3.7.tar", last modified: Sun Jul 30 08:58:28 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.3.8.tar", last modified: Thu Aug  3 13:10:38 2023, max compression
```

## Comparing `authomize-rest-api-client-4.3.7.tar` & `authomize-rest-api-client-4.3.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.419365 authomize-rest-api-client-4.3.7/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-07-30 08:58:28.419365 authomize-rest-api-client-4.3.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2201 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85173 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49496 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201078 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.419365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   115488 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.419365 authomize-rest-api-client-4.3.7/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-07-30 08:58:28.000000 authomize-rest-api-client-4.3.7/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-07-30 08:58:28.000000 authomize-rest-api-client-4.3.7/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 08:58:28.000000 authomize-rest-api-client-4.3.7/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-30 08:58:28.000000 authomize-rest-api-client-4.3.7/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-30 08:58:28.000000 authomize-rest-api-client-4.3.7/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-07-30 08:58:28.419365 authomize-rest-api-client-4.3.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1117 2023-07-30 08:58:12.000000 authomize-rest-api-client-4.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90538 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49496 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   210449 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   115488 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-08-03 13:10:19.000000 authomize-rest-api-client-4.3.8/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-08-03 13:10:38.000000 authomize-rest-api-client-4.3.8/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-08-03 13:10:38.000000 authomize-rest-api-client-4.3.8/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 13:10:38.000000 authomize-rest-api-client-4.3.8/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-08-03 13:10:38.000000 authomize-rest-api-client-4.3.8/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-03 13:10:38.000000 authomize-rest-api-client-4.3.8/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-08-03 13:10:38.459387 authomize-rest-api-client-4.3.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-08-03 13:10:22.000000 authomize-rest-api-client-4.3.8/setup.py
```

### Comparing `authomize-rest-api-client-4.3.7/LICENSE.txt` & `authomize-rest-api-client-4.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.7/README.md` & `authomize-rest-api-client-4.3.8/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.7/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.3.8/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.3.8/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-07-27T10:34:52+00:00
+#   timestamp: 2023-08-03T13:06:54+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
@@ -431,14 +431,120 @@
     invalidOwnerIds: List[str] = Field(
         ...,
         description='List of **invalid** owner (user) ids.',
         title='Invalidownerids',
     )
 
 
+class Type(Enum):
+    GitRepository = 'GitRepository'
+
+
+class NewGitRepoRequestSchema(BaseModel):
+    uniqueId: constr(min_length=1) = Field(
+        ..., description='Asset ID. **Mandatory, must be unique.**\n', title='Uniqueid'
+    )
+    originId: Optional[constr(min_length=1)] = Field(
+        default=None,
+        description="The asset ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
+        title='Originid',
+    )
+    name: constr(min_length=1) = Field(
+        ...,
+        description='The name of the asset. The default is the Asset ID. **Mandatory**\n',
+        title='Name',
+    )
+    type: Optional[Type] = Field(default='GitRepository', title='Type')
+    alternativeName: Optional[str] = Field(
+        default=None,
+        description='Any alternative name for the resource, or any other representation of the resource, if it exists.\nThe default is `null`.\n',
+        title='Alternativename',
+    )
+    originType: Optional[str] = Field(
+        default=None,
+        description='The asset type in the source system.\nThe default is the canonical type (if not mentioned).\n',
+        title='Origintype',
+    )
+    createdAt: Optional[datetime] = Field(
+        default=None,
+        description='The date (in ISO 8601 format) that the asset was created.\nThe default is `null`.\n',
+        title='Createdat',
+    )
+    lastUsedAt: Optional[datetime] = Field(
+        default=None,
+        description='The date (in ISO 8601 format) of the last time that the asset was in use.\nThe default is `null`.\n',
+        title='Lastusedat',
+    )
+    description: Optional[str] = Field(
+        default=None,
+        description='A description of the asset (up to 512 characters).\n',
+        title='Description',
+    )
+    href: Optional[str] = Field(
+        default=None,
+        description='A link to the asset in the source system.\n',
+        title='Href',
+    )
+    owner: Optional[str] = Field(
+        default=None, description='The owner ID', title='Owner'
+    )
+    tags: Optional[List[constr(min_length=1)]] = Field(
+        default=None, description='Tags associated with the asset.\n', title='Tags'
+    )
+    isPrivate: Optional[bool] = Field(
+        default=False, description='Is Repo Private', title='Isprivate'
+    )
+    isArchived: Optional[bool] = Field(
+        default=False, description='Is Repo Archived', title='Isarchived'
+    )
+    hasProtectionRules: Optional[bool] = Field(
+        default=False,
+        description='Does the Repo have protection rules',
+        title='Hasprotectionrules',
+    )
+    mainBranchProtectionRules: Optional[List[str]] = Field(
+        default=[],
+        description='Protection Rules for main branch',
+        title='Mainbranchprotectionrules',
+    )
+    developBranchProtectionRules: Optional[List[str]] = Field(
+        default=[],
+        description='Protection Rules for develop branch',
+        title='Developbranchprotectionrules',
+    )
+    vulnerabilityAlertsEnabled: Optional[bool] = Field(
+        default=False,
+        description='Are alerts for vulnerability enabled or not',
+        title='Vulnerabilityalertsenabled',
+    )
+
+
+class NewGitRepoResponseSchema(BaseModel):
+    acceptedTimestamp: Optional[datetime] = Field(
+        default=None,
+        description='**The accepted time of the request**',
+        title='Acceptedtimestamp',
+    )
+    requestId: str = Field(..., description='**Request id**', title='Requestid')
+    numberOfAcceptedEntities: int = Field(
+        ...,
+        description='**The number of entities that pass validation and uploaded**',
+        title='Numberofacceptedentities',
+    )
+    data: Optional[Any] = Field(default={}, description='Response data.', title='Data')
+    validOwnerIds: List[str] = Field(
+        ..., description='List of **valid** owner (user) ids.', title='Validownerids'
+    )
+    invalidOwnerIds: List[str] = Field(
+        ...,
+        description='List of **invalid** owner (user) ids.',
+        title='Invalidownerids',
+    )
+
+
 class NewGroupingRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ...,
         description='\nGrouping ID. **Mandatory, must be unique.**\n',
         title='Uniqueid',
     )
     originId: Optional[constr(min_length=1)] = Field(
@@ -1147,14 +1253,15 @@
     tags: Optional[List[constr(min_length=1)]] = Field(
         default=None, description='Tags associated with the asset.\n', title='Tags'
     )
 
 
 class BundleTransactionSchema(BaseModel):
     connectorId: str = Field(..., title='Connectorid')
+    executionId: Optional[str] = Field(default=None, title='Executionid')
     transactionCreatedAt: Optional[datetime] = Field(
         default=None, title='Transactioncreatedat'
     )
     warnings: Optional[List[str]] = Field(default=None, title='Warnings')
     validations: Optional[Dict[str, Any]] = Field(default=None, title='Validations')
     id: str = Field(..., title='Id')
     state: TransactionStateType
@@ -1330,14 +1437,30 @@
     )
     inheritanceAssets: Optional[List[AssetsInheritance]] = Field(
         default=None, title='Inheritanceassets'
     )
     access: Optional[List[AccessDescription]] = Field(default=None, title='Access')
 
 
+class NewGitRepoListRequestSchema(BaseModel):
+    executionId: Optional[str] = Field(
+        default=None,
+        description='The `executionId` parameter can be used to allow an app to run as a set of multiple, different executions with different configurations.\n\nOnce the data was uploaded using a certain `executionId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `executionId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n',
+        title='Executionid',
+    )
+    data: List[NewGitRepoRequestSchema] = Field(
+        ..., description='New Git Repos', max_items=10000, min_items=1, title='Data'
+    )
+    validateOnly: Optional[bool] = Field(
+        default=False,
+        description='Validate the request without uploading the data into the system.',
+        title='Validateonly',
+    )
+
+
 class NewIdentityRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ..., description='Identity ID **Mandatory**\n', title='Uniqueid'
     )
     originId: Optional[constr(min_length=1)] = Field(
         default=None,
         description="The identity ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
@@ -1616,18 +1739,18 @@
         default=None,
         description='The privilege name in the source system.',
         title='Originname',
     )
 
 
 class RequestsBundleSchema(BaseModel):
-    execution_id: Optional[str] = Field(
+    executionId: Optional[str] = Field(
         default=None,
         description='The `executionId` parameter can be used to allow an app to run as a set of multiple, different executions with different configurations.\n\nOnce the data was uploaded using a certain `executionId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `executionId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n',
-        title='Execution Id',
+        title='Executionid',
     )
     delete_app_data: Optional[bool] = Field(
         default=False,
         description='The Delete Application Data API is used to delete app data by `{appId}`.',
         title='Delete App Data',
     )
     createdAt: Optional[datetime] = Field(default=None, title='Createdat')
@@ -1671,14 +1794,19 @@
         title='New Groupings Association',
     )
     new_assets: Optional[List[NewAssetRequestSchema]] = Field(
         default=None,
         description='The Create Assets API creates assets (including asset data).',
         title='New Assets',
     )
+    new_git_repos: Optional[List[NewGitRepoRequestSchema]] = Field(
+        default=None,
+        description='Creates a Git Repository Asset',
+        title='New Git Repos',
+    )
     new_assets_inheritance: Optional[List[NewAssetInheritanceRequestSchema]] = Field(
         default=None,
         description='The Create Assets Inheritence API enables you to create a connection between different assets (for example, a folder that contains multiple files).\n',
         title='New Assets Inheritance',
     )
     new_identities: Optional[List[NewIdentityRequestSchema]] = Field(
         default=None,
@@ -1953,14 +2081,19 @@
         title='New Groupings Association',
     )
     new_assets: Optional[List[NewAssetRequestSchema]] = Field(
         default=None,
         description='The Create Assets API creates assets (including asset data).',
         title='New Assets',
     )
+    new_git_repos: Optional[List[NewGitRepoRequestSchema]] = Field(
+        default=None,
+        description='Creates a Git Repository Asset',
+        title='New Git Repos',
+    )
     new_assets_inheritance: Optional[List[NewAssetInheritanceRequestSchema]] = Field(
         default=None,
         description='The Create Assets Inheritence API enables you to create a connection between different assets (for example, a folder that contains multiple files).\n',
         title='New Assets Inheritance',
     )
     new_identities: Optional[List[NewIdentityRequestSchema]] = Field(
         default=None,
```

### Comparing `authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.3.8/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9830661629153383%*

 * *Differences: {"'components'": "{'schemas': {'BundleTransactionSchema': {'properties': {'executionId': "*

 * *                 "OrderedDict([('title', 'Executionid'), ('type', 'string')])}}, "*

 * *                 "'IngestionDataBundleSchema': {'properties': {'new_git_repos': "*

 * *                 "OrderedDict([('title', 'New Git Repos'), ('type', 'array'), ('items', "*

 * *                 "OrderedDict([('$ref', '#/components/schemas/NewGitRepoRequestSchema')])), "*

 * *                 "('description', 'Creates a Git Repository Asset')])}}, […]*

```diff
@@ -364,14 +364,18 @@
             "BundleTransactionSchema": {
                 "description": "API response schema",
                 "properties": {
                     "connectorId": {
                         "title": "Connectorid",
                         "type": "string"
                     },
+                    "executionId": {
+                        "title": "Executionid",
+                        "type": "string"
+                    },
                     "id": {
                         "title": "Id",
                         "type": "string"
                     },
                     "state": {
                         "$ref": "#/components/schemas/TransactionStateType"
                     },
@@ -865,14 +869,22 @@
                         "description": "The Create Assets Inheritence API enables you to create a connection between different assets (for example, a folder that contains multiple files).\n",
                         "items": {
                             "$ref": "#/components/schemas/NewAssetInheritanceRequestSchema"
                         },
                         "title": "New Assets Inheritance",
                         "type": "array"
                     },
+                    "new_git_repos": {
+                        "description": "Creates a Git Repository Asset",
+                        "items": {
+                            "$ref": "#/components/schemas/NewGitRepoRequestSchema"
+                        },
+                        "title": "New Git Repos",
+                        "type": "array"
+                    },
                     "new_groupings": {
                         "description": "The Create Groupings API is used to create groups that have access to a particular app.",
                         "items": {
                             "$ref": "#/components/schemas/NewGroupingRequestSchema"
                         },
                         "title": "New Groupings",
                         "type": "array"
@@ -1450,14 +1462,220 @@
                     "numberOfAcceptedEntities",
                     "validOwnerIds",
                     "invalidOwnerIds"
                 ],
                 "title": "NewAssetsResponseSchema",
                 "type": "object"
             },
+            "NewGitRepoListRequestSchema": {
+                "description": "List request schema",
+                "properties": {
+                    "data": {
+                        "description": "New Git Repos",
+                        "items": {
+                            "$ref": "#/components/schemas/NewGitRepoRequestSchema"
+                        },
+                        "maxItems": 10000,
+                        "minItems": 1,
+                        "title": "Data",
+                        "type": "array"
+                    },
+                    "executionId": {
+                        "description": "The `executionId` parameter can be used to allow an app to run as a set of multiple, different executions with different configurations.\n\nOnce the data was uploaded using a certain `executionId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `executionId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n",
+                        "title": "Executionid",
+                        "type": "string"
+                    },
+                    "validateOnly": {
+                        "default": false,
+                        "description": "Validate the request without uploading the data into the system.",
+                        "title": "Validateonly",
+                        "type": "boolean"
+                    }
+                },
+                "required": [
+                    "data"
+                ],
+                "title": "NewGitRepoListRequestSchema",
+                "type": "object"
+            },
+            "NewGitRepoRequestSchema": {
+                "description": "New Git Repo request schema",
+                "properties": {
+                    "alternativeName": {
+                        "description": "Any alternative name for the resource, or any other representation of the resource, if it exists.\nThe default is `null`.\n",
+                        "title": "Alternativename",
+                        "type": "string"
+                    },
+                    "createdAt": {
+                        "description": "The date (in ISO 8601 format) that the asset was created.\nThe default is `null`.\n",
+                        "format": "date-time",
+                        "title": "Createdat",
+                        "type": "string"
+                    },
+                    "description": {
+                        "description": "A description of the asset (up to 512 characters).\n",
+                        "title": "Description",
+                        "type": "string"
+                    },
+                    "developBranchProtectionRules": {
+                        "default": [],
+                        "description": "Protection Rules for develop branch",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "Developbranchprotectionrules",
+                        "type": "array"
+                    },
+                    "hasProtectionRules": {
+                        "default": false,
+                        "description": "Does the Repo have protection rules",
+                        "title": "Hasprotectionrules",
+                        "type": "boolean"
+                    },
+                    "href": {
+                        "description": "A link to the asset in the source system.\n",
+                        "title": "Href",
+                        "type": "string"
+                    },
+                    "isArchived": {
+                        "default": false,
+                        "description": "Is Repo Archived",
+                        "title": "Isarchived",
+                        "type": "boolean"
+                    },
+                    "isPrivate": {
+                        "default": false,
+                        "description": "Is Repo Private",
+                        "title": "Isprivate",
+                        "type": "boolean"
+                    },
+                    "lastUsedAt": {
+                        "description": "The date (in ISO 8601 format) of the last time that the asset was in use.\nThe default is `null`.\n",
+                        "format": "date-time",
+                        "title": "Lastusedat",
+                        "type": "string"
+                    },
+                    "mainBranchProtectionRules": {
+                        "default": [],
+                        "description": "Protection Rules for main branch",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "Mainbranchprotectionrules",
+                        "type": "array"
+                    },
+                    "name": {
+                        "description": "The name of the asset. The default is the Asset ID. **Mandatory**\n",
+                        "minLength": 1,
+                        "title": "Name",
+                        "type": "string"
+                    },
+                    "originId": {
+                        "description": "The asset ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
+                        "minLength": 1,
+                        "title": "Originid",
+                        "type": "string"
+                    },
+                    "originType": {
+                        "description": "The asset type in the source system.\nThe default is the canonical type (if not mentioned).\n",
+                        "title": "Origintype",
+                        "type": "string"
+                    },
+                    "owner": {
+                        "description": "The owner ID",
+                        "title": "Owner",
+                        "type": "string"
+                    },
+                    "tags": {
+                        "description": "Tags associated with the asset.\n",
+                        "items": {
+                            "minLength": 1,
+                            "type": "string"
+                        },
+                        "title": "Tags",
+                        "type": "array"
+                    },
+                    "type": {
+                        "default": "GitRepository",
+                        "enum": [
+                            "GitRepository"
+                        ],
+                        "title": "Type",
+                        "type": "string"
+                    },
+                    "uniqueId": {
+                        "description": "Asset ID. **Mandatory, must be unique.**\n",
+                        "minLength": 1,
+                        "title": "Uniqueid",
+                        "type": "string"
+                    },
+                    "vulnerabilityAlertsEnabled": {
+                        "default": false,
+                        "description": "Are alerts for vulnerability enabled or not",
+                        "title": "Vulnerabilityalertsenabled",
+                        "type": "boolean"
+                    }
+                },
+                "required": [
+                    "uniqueId",
+                    "name"
+                ],
+                "title": "NewGitRepoRequestSchema",
+                "type": "object"
+            },
+            "NewGitRepoResponseSchema": {
+                "description": "New Git repo response schema",
+                "properties": {
+                    "acceptedTimestamp": {
+                        "description": "**The accepted time of the request**",
+                        "format": "date-time",
+                        "title": "Acceptedtimestamp",
+                        "type": "string"
+                    },
+                    "data": {
+                        "default": {},
+                        "description": "Response data.",
+                        "title": "Data"
+                    },
+                    "invalidOwnerIds": {
+                        "description": "List of **invalid** owner (user) ids.",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "Invalidownerids",
+                        "type": "array"
+                    },
+                    "numberOfAcceptedEntities": {
+                        "description": "**The number of entities that pass validation and uploaded**",
+                        "title": "Numberofacceptedentities",
+                        "type": "integer"
+                    },
+                    "requestId": {
+                        "description": "**Request id**",
+                        "title": "Requestid",
+                        "type": "string"
+                    },
+                    "validOwnerIds": {
+                        "description": "List of **valid** owner (user) ids.",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "Validownerids",
+                        "type": "array"
+                    }
+                },
+                "required": [
+                    "requestId",
+                    "numberOfAcceptedEntities",
+                    "validOwnerIds",
+                    "invalidOwnerIds"
+                ],
+                "title": "NewGitRepoResponseSchema",
+                "type": "object"
+            },
             "NewGroupingRequestSchema": {
                 "description": "New group request schema",
                 "properties": {
                     "alternativeName": {
                         "description": "Alias of the grouping.",
                         "maxLength": 256,
                         "title": "Alternativename",
@@ -2748,17 +2966,17 @@
                     },
                     "delete_app_data": {
                         "default": false,
                         "description": "The Delete Application Data API is used to delete app data by `{appId}`.",
                         "title": "Delete App Data",
                         "type": "boolean"
                     },
-                    "execution_id": {
+                    "executionId": {
                         "description": "The `executionId` parameter can be used to allow an app to run as a set of multiple, different executions with different configurations.\n\nOnce the data was uploaded using a certain `executionId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `executionId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n",
-                        "title": "Execution Id",
+                        "title": "Executionid",
                         "type": "string"
                     },
                     "new_accounts_association": {
                         "description": "The Create Accounts Association API creates account associations between user accounts and groups.",
                         "items": {
                             "$ref": "#/components/schemas/NewAccountsAssociationRequestSchema"
                         },
@@ -2777,14 +2995,22 @@
                         "description": "The Create Assets Inheritence API enables you to create a connection between different assets (for example, a folder that contains multiple files).\n",
                         "items": {
                             "$ref": "#/components/schemas/NewAssetInheritanceRequestSchema"
                         },
                         "title": "New Assets Inheritance",
                         "type": "array"
                     },
+                    "new_git_repos": {
+                        "description": "Creates a Git Repository Asset",
+                        "items": {
+                            "$ref": "#/components/schemas/NewGitRepoRequestSchema"
+                        },
+                        "title": "New Git Repos",
+                        "type": "array"
+                    },
                     "new_groupings": {
                         "description": "The Create Groupings API is used to create groups that have access to a particular app.",
                         "items": {
                             "$ref": "#/components/schemas/NewGroupingRequestSchema"
                         },
                         "title": "New Groupings",
                         "type": "array"
@@ -3868,15 +4094,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "4.3.4",
+        "version": "4.3.7",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
@@ -5328,14 +5554,72 @@
                 ],
                 "summary": "Create Assets",
                 "tags": [
                     "Assets"
                 ]
             }
         },
+        "/v2/apps/{appId}/assets/git-repository": {
+            "post": {
+                "description": "Creates a Git Repository Asset",
+                "operationId": "create_git_repo_v2_apps__appId__assets_git_repository_post",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "appId",
+                        "required": true,
+                        "schema": {
+                            "title": "Appid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "$ref": "#/components/schemas/NewGitRepoListRequestSchema"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/NewGitRepoResponseSchema"
+                                }
+                            }
+                        },
+                        "description": "Successful Response"
+                    },
+                    "422": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/HTTPValidationError"
+                                }
+                            }
+                        },
+                        "description": "Validation Error"
+                    }
+                },
+                "security": [
+                    {
+                        "APIKeyHeader": []
+                    }
+                ],
+                "summary": "Create Git Repo",
+                "tags": [
+                    "Assets"
+                ]
+            }
+        },
         "/v2/apps/{appId}/assets/inheritance": {
             "get": {
                 "description": "The Search Assets Inheritance API gets all the assets related to the source asset (for examples, all files in a folder).",
                 "operationId": "search_assets_inheritance_v2_apps__appId__assets_inheritance_get",
                 "parameters": [
                     {
                         "in": "path",
@@ -5703,15 +5987,15 @@
                             "description": "The `executionId` parameter can be used to allow an app to run as a set of multiple, different executions with different configurations.\n\nOnce the data was uploaded using a certain `executionId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `executionId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n",
                             "title": "Executionid",
                             "type": "string"
                         }
                     },
                     {
                         "description": "Delete all the app data lastly updated before the given date.",
-                        "example": "2023-07-02T08:30:55.198087+00:00",
+                        "example": "2023-08-03T09:27:54.562402+00:00",
                         "in": "query",
                         "name": "modifiedBefore",
                         "required": false,
                         "schema": {
                             "description": "Delete all the app data lastly updated before the given date.",
                             "format": "date-time",
                             "title": "Modifiedbefore",
```

### Comparing `authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.3.8/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.7/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.3.8/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.7/setup.py` & `authomize-rest-api-client-4.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.3.7',
+        version='4.3.8',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

