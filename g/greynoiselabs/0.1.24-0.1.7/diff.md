# Comparing `tmp/greynoiselabs-0.1.24.tar.gz` & `tmp/greynoiselabs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greynoiselabs-0.1.24.tar", max compression
+gzip compressed data, was "greynoiselabs-0.1.7.tar", last modified: Thu Jul 27 18:38:35 2023, max compression
```

## Comparing `greynoiselabs-0.1.24.tar` & `greynoiselabs-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,41 @@
--rw-r--r--   0        0        0     1079 2023-08-03 19:33:57.044632 greynoiselabs-0.1.24/LICENSE
--rw-r--r--   0        0        0     6300 2023-08-03 19:33:57.044632 greynoiselabs-0.1.24/README.rst
--rw-r--r--   0        0        0     1698 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/__init__.py
--rw-r--r--   0        0        0     1809 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/__init__.py
--rw-r--r--   0        0        0     7371 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/async_base_client.py
--rw-r--r--   0        0        0     1951 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/base_model.py
--rw-r--r--   0        0        0     4982 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/client.py
--rw-r--r--   0        0        0       84 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/enums.py
--rw-r--r--   0        0        0     2366 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/exceptions.py
--rw-r--r--   0        0        0      461 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/generate_g_n_q_l.py
--rw-r--r--   0        0        0      593 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/get_c2s.py
--rw-r--r--   0        0        0      698 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/get_i_ps.py
--rw-r--r--   0        0        0      775 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/get_knocks.py
--rw-r--r--   0        0        0      689 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/get_noise_ranks.py
--rw-r--r--   0        0        0      683 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/get_payloads.py
--rw-r--r--   0        0        0      755 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/get_requests.py
--rw-r--r--   0        0        0      221 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/input_types.py
--rw-r--r--   0        0        0      220 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/api/scalars.py
--rw-r--r--   0        0        0        0 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/cli/__init__.py
--rwxr-xr-x   0        0        0     5840 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/cli/auth.py
--rw-r--r--   0        0        0    12117 2023-08-03 19:33:57.048632 greynoiselabs-0.1.24/src/greynoiselabs/cli/main.py
--rw-r--r--   0        0        0     7800 1970-01-01 00:00:00.000000 greynoiselabs-0.1.24/PKG-INFO
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.736639 greynoiselabs-0.1.7/
+-rw-r--r--   0 matt       (502) staff       (20)     1079 2023-06-16 04:21:17.000000 greynoiselabs-0.1.7/LICENSE
+-rw-r--r--   0 matt       (502) staff       (20)     2005 2023-07-27 18:38:35.736729 greynoiselabs-0.1.7/PKG-INFO
+-rw-r--r--   0 matt       (502) staff       (20)      960 2023-07-27 16:38:11.000000 greynoiselabs-0.1.7/README.rst
+-rw-r--r--   0 matt       (502) staff       (20)      281 2023-07-27 18:38:35.737016 greynoiselabs-0.1.7/setup.cfg
+-rw-r--r--   0 matt       (502) staff       (20)     1698 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/setup.py
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.729256 greynoiselabs-0.1.7/src/
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.730993 greynoiselabs-0.1.7/src/greynoiselabs/
+-rw-r--r--   0 matt       (502) staff       (20)        0 2023-07-27 04:05:43.000000 greynoiselabs-0.1.7/src/greynoiselabs/__init__.py
+-rw-r--r--   0 matt       (502) staff       (20)      254 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/__version__.py
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.736050 greynoiselabs-0.1.7/src/greynoiselabs/api/
+-rw-r--r--   0 matt       (502) staff       (20)     1611 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/__init__.py
+-rw-r--r--   0 matt       (502) staff       (20)     7371 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/async_base_client.py
+-rw-r--r--   0 matt       (502) staff       (20)     1951 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/base_model.py
+-rw-r--r--   0 matt       (502) staff       (20)     4181 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/client.py
+-rw-r--r--   0 matt       (502) staff       (20)       84 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/enums.py
+-rw-r--r--   0 matt       (502) staff       (20)     2366 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/exceptions.py
+-rw-r--r--   0 matt       (502) staff       (20)      461 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/generate_g_n_q_l.py
+-rw-r--r--   0 matt       (502) staff       (20)      593 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_c2s.py
+-rw-r--r--   0 matt       (502) staff       (20)      614 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_i_ps.py
+-rw-r--r--   0 matt       (502) staff       (20)      775 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_knocks.py
+-rw-r--r--   0 matt       (502) staff       (20)      689 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_noise_ranks.py
+-rw-r--r--   0 matt       (502) staff       (20)      755 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_requests.py
+-rw-r--r--   0 matt       (502) staff       (20)      221 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/input_types.py
+-rw-r--r--   0 matt       (502) staff       (20)      942 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/noise_rank.py
+-rw-r--r--   0 matt       (502) staff       (20)      220 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/scalars.py
+-rw-r--r--   0 matt       (502) staff       (20)     1138 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/top_h_t_t_p_requests.py
+-rw-r--r--   0 matt       (502) staff       (20)     1060 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/top_knocks.py
+-rw-r--r--   0 matt       (502) staff       (20)      993 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/top_popular_i_ps.py
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.736481 greynoiselabs-0.1.7/src/greynoiselabs/cli/
+-rw-r--r--   0 matt       (502) staff       (20)        0 2023-07-27 03:55:22.000000 greynoiselabs-0.1.7/src/greynoiselabs/cli/__init__.py
+-rwxr-xr-x   0 matt       (502) staff       (20)     5763 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/cli/auth.py
+-rw-r--r--   0 matt       (502) staff       (20)     4985 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/cli/main.py
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.732309 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/
+-rw-r--r--   0 matt       (502) staff       (20)     2005 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (502) staff       (20)     1148 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (502) staff       (20)        1 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (502) staff       (20)       61 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/entry_points.txt
+-rw-r--r--   0 matt       (502) staff       (20)        1 2023-07-27 03:56:32.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/not-zip-safe
+-rw-r--r--   0 matt       (502) staff       (20)      246 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/requires.txt
+-rw-r--r--   0 matt       (502) staff       (20)       14 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/top_level.txt
```

### Comparing `greynoiselabs-0.1.24/LICENSE` & `greynoiselabs-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `greynoiselabs-0.1.24/pyproject.toml` & `greynoiselabs-0.1.7/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,45 @@
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+#!/usr/bin/env python
+"""GreyNoise Labs API client package."""
+import os
 
-[tool.poetry]
-name = "greynoiselabs"
-version = "0.1.24"
-description = "Abstraction to interact with GreyNoise Labs GraphQL API."
-authors = ["GreyNoise Intelligence <labs@greynoise.io>"]
-license = "MIT"
-readme = "README.rst"
-homepage = "https://api.labs.greynoise.io/"
-repository = "https://github.com/GreyNoise-Intelligence/greynoiselabs"
-documentation = "https://api.labs.greynoise.io/"
-keywords = ["internet", "scanning", "threat intelligence", "security"]
-classifiers = [
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Natural Language :: English",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Topic :: Software Development :: Libraries",
-]
+from setuptools import find_packages, setup
 
-[tool.poetry.scripts]
-greynoiselabs = "greynoiselabs.cli.main:app"
 
-[tool.poetry.dev-dependencies]
-ariadne-codegen = "0.7.1"
-pre-commit = "3.3.3"
-tox = "4.6.4"
-wheel = "0.41.0"
-black = "^23.1.0"
-ruff = "0.0.280"
-isort = "^5.12.0"
-mock = "^5.0.1"
-pylint = "^2.17.4"
-pytest-cov = "^4.0.0"
-pytest = "^7.3.0"
-restructuredtext-lint = "^1.4.0"
-yamllint = "^1.29.0"
+def read(fname):
+    """Read file and return its contents."""
+    with open(os.path.join(os.path.dirname(__file__), fname)) as input_file:
+        return input_file.read()
 
-[tool.poetry.dependencies]
-python = ">=3.9,<4"
-Click = "8.1.6"
-pydantic = "1.10.9"
-httpx = "0.24.1"
-websockets = "11.0.3"
-auth0-python = "4.4.0"
-typer = "0.9.0"
-PyJWT = "2.8.0"
-requests = "2.31.0"
-rich = "13.4.2"
-urllib3 = "2.0.4"
-colorama = "0.4.6"
-jsonlines = "3.1.0"
-requests_oauthlib = "1.3.1"
-platformdirs = "3.9.1"
-merge_args = "0.1.5"
+
+setup(
+    name="greynoiselabs",
+    version="0.1.7",
+    description="Abstraction to interact with GreyNoise Labs GraphQL API.",
+    url="https://api.labs.greynoise.io/",
+    author="GreyNoise Intelligence",
+    author_email="labs@greynoise.io",
+    license="MIT",
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
+    install_requires=read("requirements/common.txt").split("\n"),
+    long_description=read("README.rst") + "\n\n" + read("CHANGELOG.md"),
+    python_requires=">=3.0, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*",
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Software Development :: Libraries",
+    ],
+    entry_points={"console_scripts": ["greynoiselabs = greynoiselabs.cli.main:app"]},
+    zip_safe=False,
+    keywords=["internet", "scanning", "threat intelligence", "security"],
+    download_url="https://github.com/GreyNoise-Intelligence/greynoiselabs",
+)
```

### Comparing `greynoiselabs-0.1.24/src/greynoiselabs/api/__init__.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 15:11
+# Generated by ariadne-codegen on 2023-07-27 18:00
 
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel
 from .client import Client
 from .exceptions import (
     GraphQLClientError,
     GraphQLClientGraphQLError,
@@ -15,19 +15,14 @@
 from .get_i_ps import GetIPs, GetIPsTopPopularIPs, GetIPsTopPopularIPsPopularIPs
 from .get_knocks import GetKnocks, GetKnocksTopKnocks, GetKnocksTopKnocksKnock
 from .get_noise_ranks import (
     GetNoiseRanks,
     GetNoiseRanksNoiseRank,
     GetNoiseRanksNoiseRankIps,
 )
-from .get_payloads import (
-    GetPayloads,
-    GetPayloadsTopPayloads,
-    GetPayloadsTopPayloadsPayloads,
-)
 from .get_requests import (
     GetRequests,
     GetRequestsTopHTTPRequests,
     GetRequestsTopHTTPRequestsHttpRequests,
 )
 from .input_types import SpectaQLOption
 
@@ -45,17 +40,14 @@
     "GetIPsTopPopularIPsPopularIPs",
     "GetKnocks",
     "GetKnocksTopKnocks",
     "GetKnocksTopKnocksKnock",
     "GetNoiseRanks",
     "GetNoiseRanksNoiseRank",
     "GetNoiseRanksNoiseRankIps",
-    "GetPayloads",
-    "GetPayloadsTopPayloads",
-    "GetPayloadsTopPayloadsPayloads",
     "GetRequests",
     "GetRequestsTopHTTPRequests",
     "GetRequestsTopHTTPRequestsHttpRequests",
     "GraphQLClientError",
     "GraphQLClientGraphQLError",
     "GraphQLClientGraphQLMultiError",
     "GraphQLClientHttpError",
```

### Comparing `greynoiselabs-0.1.24/src/greynoiselabs/api/async_base_client.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 15:11
+# Generated by ariadne-codegen on 2023-07-27 18:00
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `greynoiselabs-0.1.24/src/greynoiselabs/api/base_model.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 15:11
+# Generated by ariadne-codegen on 2023-07-27 18:00
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `greynoiselabs-0.1.24/src/greynoiselabs/api/client.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# Generated by ariadne-codegen on 2023-08-03 15:11
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from .async_base_client import AsyncBaseClient
 from .generate_g_n_q_l import GenerateGNQL
 from .get_c2s import GetC2s
 from .get_i_ps import GetIPs
 from .get_knocks import GetKnocks
 from .get_noise_ranks import GetNoiseRanks
-from .get_payloads import GetPayloads
 from .get_requests import GetRequests
 
 
 def gql(q: str) -> str:
     return q
 
 
@@ -85,26 +84,26 @@
             """
         )
         variables: dict[str, object] = {"ip": ip}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetKnocks.parse_obj(data)
 
-    async def generate_g_n_q_l(self, input_text: str) -> GenerateGNQL:
+    async def generate_g_n_q_l(self, input: str) -> GenerateGNQL:
         query = gql(
             """
-            query generateGNQL($input_text: String!) {
-              generateGNQL(input_text: $input_text) {
+            query generateGNQL($input: String!) {
+              generateGNQL(input: $input) {
                 input_text
                 queries
               }
             }
             """
         )
-        variables: dict[str, object] = {"input_text": input_text}
+        variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GenerateGNQL.parse_obj(data)
 
     async def get_noise_ranks(self, ip: str) -> GetNoiseRanks:
         query = gql(
             """
@@ -124,49 +123,23 @@
             """
         )
         variables: dict[str, object] = {"ip": ip}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetNoiseRanks.parse_obj(data)
 
-    async def get_payloads(self) -> GetPayloads:
-        query = gql(
-            """
-            query getPayloads {
-              topPayloads {
-                payloads {
-                  protocol
-                  size
-                  payload
-                  payload_b64
-                  request_count
-                  source_ip_count
-                  pervasiveness
-                }
-              }
-            }
-            """
-        )
-        variables: dict[str, object] = {}
-        response = await self.execute(query=query, variables=variables)
-        data = self.get_data(response)
-        return GetPayloads.parse_obj(data)
-
     async def get_i_ps(self) -> GetIPs:
         query = gql(
             """
             query getIPs {
               topPopularIPs {
                 popularIPs {
                   ip
                   request_count
                   users_count
-                  last_requested
-                  noise
-                  last_seen
                 }
               }
             }
             """
         )
         variables: dict[str, object] = {}
         response = await self.execute(query=query, variables=variables)
```

### Comparing `greynoiselabs-0.1.24/src/greynoiselabs/api/exceptions.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 15:11
+# Generated by ariadne-codegen on 2023-07-27 18:00
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `greynoiselabs-0.1.24/src/greynoiselabs/api/get_c2s.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/get_c2s.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 15:11
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.24/src/greynoiselabs/api/get_i_ps.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/get_i_ps.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Generated by ariadne-codegen on 2023-08-03 15:11
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
-from typing import Any, List, Optional
+from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
 
 
 class GetIPs(BaseModel):
@@ -16,15 +16,12 @@
     popular_i_ps: List["GetIPsTopPopularIPsPopularIPs"] = Field(alias="popularIPs")
 
 
 class GetIPsTopPopularIPsPopularIPs(BaseModel):
     ip: str
     request_count: int
     users_count: int
-    last_requested: Any
-    noise: bool
-    last_seen: Optional[Any]
 
 
 GetIPs.update_forward_refs()
 GetIPsTopPopularIPs.update_forward_refs()
 GetIPsTopPopularIPsPopularIPs.update_forward_refs()
```

### Comparing `greynoiselabs-0.1.24/src/greynoiselabs/api/get_knocks.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/get_knocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 15:11
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from typing import Any, List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.24/src/greynoiselabs/api/get_noise_ranks.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/get_noise_ranks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 15:11
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.24/src/greynoiselabs/api/get_requests.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/get_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-03 15:11
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.24/src/greynoiselabs/cli/auth.py` & `greynoiselabs-0.1.7/src/greynoiselabs/cli/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 #!/usr/bin/env python3
 
+import time
 import json
 import os
-import time
-
-import jwt
-import requests
-import typer
+from requests_oauthlib import OAuth2Session
 from auth0.authentication.token_verifier import (
-    AsymmetricSignatureVerifier,
     TokenVerifier,
+    AsymmetricSignatureVerifier,
 )
-from requests_oauthlib import OAuth2Session
+import jwt
+import requests
+import typer
 
 AUTH0_DOMAIN = "greynoise2.auth0.com"
 AUTH0_CLIENT_ID = "IM8Old6x7WCr2wqVI0Cz3I0c4JPSR1gn"
 TOKEN_URL = f"https://{AUTH0_DOMAIN}/oauth/token"
 JWKS_URL = f"https://{AUTH0_DOMAIN}/.well-known/jwks.json"
 ISSUER_URL = f"https://{AUTH0_DOMAIN}/"
 ALGORITHMS = ["RS256"]
 
 
-def get_token_from_file(token_filename: str):
+def get_token_from_file(token_filename):
     """
     Gets the token from a file
     """
     try:
         fp = os.path.expanduser(token_filename)
         with open(fp, "r") as f:
             token_data = json.load(f)
             return token_data
-    except Exception:
+    except Exception as ex:
+        print(f"Unable to load token from {token_filename}, {ex}")
         return None
 
 
-def token_saver(token_filename: str, token_data: any):
+def token_saver(token_filename, token_data):
     """
     Saves the token to a file
     """
     try:
         fp = os.path.expanduser(token_filename)
         os.makedirs(os.path.dirname(fp), exist_ok=True)
         with open(fp, "w+") as f:
             json.dump(token_data, f)
-        print(f"Token saved to {token_filename}.")
     except Exception as ex:
         print(f"Unable to save token to {token_filename}, {ex}")
         raise typer.Abort()
 
 
-def token_refresh(token_filename: str, token_data_in: any):
+def token_refresh(token_filename, token_data_in):
     """
     Refreshes the token
     """
     extra = {
         "client_id": AUTH0_CLIENT_ID,
     }
     try:
@@ -62,28 +61,29 @@
         token_saver(token_filename, token_data)
         return token_data
     except Exception as ex:
         print(f"Unable to refresh token {ex}.")
         return None
 
 
-def validate_token(id_token: any):
+def validate_token(id_token):
     """
     Verify the token and its precedence
 
     :param id_token:
     """
     sv = AsymmetricSignatureVerifier(JWKS_URL)
     tv = TokenVerifier(
         signature_verifier=sv, issuer=ISSUER_URL, audience=AUTH0_CLIENT_ID
     )
     try:
         tv.verify(id_token)
         return True
-    except Exception:
+    except Exception as ex:
+        print(f"Unable to validate token {ex}.")
         return False
 
 
 def init_device_flow():
     """
     Initiate Oauth 2.0 Device Authorization Flow with Auth0
     """
@@ -126,22 +126,21 @@
             print(token_data["error_description"])
             raise typer.Exit(code=1)
         else:
             time.sleep(device_code_data["interval"])
     return token_data, current_user
 
 
-def authenticate(config_dir: str):
+def authenticate(token_filename):
     """
     Checks for local token and validates it, if invalid, attempts to refresh it.
     """
     global token_data
     global current_user
     validated = False
-    token_filename = os.path.join(config_dir, "token.json")
 
     token_data = get_token_from_file(token_filename)
     if token_data:
         validated = validate_token(token_data["id_token"])
         if validated:
             current_user = jwt.decode(
                 token_data["id_token"],
@@ -161,24 +160,22 @@
                     options={"verify_signature": False},
                 )
                 return token_data, current_user
     else:
         return None, None
 
 
-def login(config_dir: str):
+def login(token_filename):
     """
     Runs the device authorization flow and stores the user object in memory
     """
 
     global token_data
     global current_user
     validated = False
-    token_filename = os.path.join(config_dir, "token.json")
-
     token_data, current_user = init_device_flow()
     token_saver(token_filename, token_data)
     validated = validate_token(token_data["id_token"])
     if validated:
         current_user = jwt.decode(
             token_data["id_token"],
             algorithms=ALGORITHMS,
```

