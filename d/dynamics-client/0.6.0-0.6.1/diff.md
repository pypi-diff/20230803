# Comparing `tmp/dynamics_client-0.6.0.tar.gz` & `tmp/dynamics_client-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamics_client-0.6.0.tar", max compression
+gzip compressed data, was "dynamics_client-0.6.1.tar", max compression
```

## Comparing `dynamics_client-0.6.0.tar` & `dynamics_client-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/LICENSE
--rw-r--r--   0        0        0     4799 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/README.md
--rw-r--r--   0        0        0      192 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/dynamics/__init__.py
--rw-r--r--   0        0        0     9458 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/dynamics/api_actions.py
--rw-r--r--   0        0        0     7284 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/dynamics/api_functions.py
--rw-r--r--   0        0        0     1989 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/dynamics/apply_functions.py
--rw-r--r--   0        0        0    34661 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/dynamics/client.py
--rw-r--r--   0        0        0     4199 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/dynamics/enums.py
--rw-r--r--   0        0        0     4194 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/dynamics/exceptions.py
--rw-r--r--   0        0        0    33474 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/fetchxml.py
--rw-r--r--   0        0        0     1479 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/normalizers.py
--rw-r--r--   0        0        0        0 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/py.typed
--rw-r--r--   0        0        0    36471 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/query_functions.py
--rw-r--r--   0        0        0     1910 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/status.py
--rw-r--r--   0        0        0     9650 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/test.py
--rw-r--r--   0        0        0     6060 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/typing.py
--rw-r--r--   0        0        0     8532 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/utils.py
--rw-r--r--   0        0        0     3076 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6484 1970-01-01 00:00:00.000000 dynamics_client-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-03 17:05:20.845075 dynamics_client-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4965 2023-08-03 17:05:20.845075 dynamics_client-0.6.1/README.md
+-rw-r--r--   0        0        0      192 2023-08-03 17:05:20.845075 dynamics_client-0.6.1/dynamics/__init__.py
+-rw-r--r--   0        0        0     9458 2023-08-03 17:05:20.845075 dynamics_client-0.6.1/dynamics/api_actions.py
+-rw-r--r--   0        0        0     7284 2023-08-03 17:05:20.845075 dynamics_client-0.6.1/dynamics/api_functions.py
+-rw-r--r--   0        0        0     1989 2023-08-03 17:05:20.845075 dynamics_client-0.6.1/dynamics/apply_functions.py
+-rw-r--r--   0        0        0    34661 2023-08-03 17:05:20.845075 dynamics_client-0.6.1/dynamics/client.py
+-rw-r--r--   0        0        0     4199 2023-08-03 17:05:20.845075 dynamics_client-0.6.1/dynamics/enums.py
+-rw-r--r--   0        0        0     4194 2023-08-03 17:05:20.845075 dynamics_client-0.6.1/dynamics/exceptions.py
+-rw-r--r--   0        0        0    33474 2023-08-03 17:05:20.845075 dynamics_client-0.6.1/dynamics/fetchxml.py
+-rw-r--r--   0        0        0     1479 2023-08-03 17:05:20.845075 dynamics_client-0.6.1/dynamics/normalizers.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:05:20.845075 dynamics_client-0.6.1/dynamics/py.typed
+-rw-r--r--   0        0        0    36471 2023-08-03 17:05:20.849076 dynamics_client-0.6.1/dynamics/query_functions.py
+-rw-r--r--   0        0        0     1910 2023-08-03 17:05:20.849076 dynamics_client-0.6.1/dynamics/status.py
+-rw-r--r--   0        0        0     9650 2023-08-03 17:05:20.849076 dynamics_client-0.6.1/dynamics/test.py
+-rw-r--r--   0        0        0     6060 2023-08-03 17:05:20.849076 dynamics_client-0.6.1/dynamics/typing.py
+-rw-r--r--   0        0        0     8532 2023-08-03 17:05:20.849076 dynamics_client-0.6.1/dynamics/utils.py
+-rw-r--r--   0        0        0     3057 2023-08-03 17:05:20.849076 dynamics_client-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6402 1970-01-01 00:00:00.000000 dynamics_client-0.6.1/PKG-INFO
```

### Comparing `dynamics_client-0.6.0/LICENSE` & `dynamics_client-0.6.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Matti Lamppu
+Copyright (c) 2023 Matti Lamppu
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dynamics_client-0.6.0/README.md` & `dynamics_client-0.6.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 ---
 
 **Documentation**: [https://mrthearman.github.io/dynamics-client/](https://mrthearman.github.io/dynamics-client/)
 
 **Source Code**: [https://github.com/MrThearMan/dynamics-client/](https://github.com/MrThearMan/dynamics-client/)
 
+**Contributing**: [https://github.com/MrThearMan/dynamics-client/blob/main/CONTRIBUTING.md](https://github.com/MrThearMan/dynamics-client/blob/main/CONTRIBUTING.md)
+
 ---
 
 Client for making Web API request from a Microsoft Dynamics 365 Database.
 
 You should also read the [Dynamics Web API Reference Docs][ref-docs]:
```

### Comparing `dynamics_client-0.6.0/dynamics/api_actions.py` & `dynamics_client-0.6.1/dynamics/api_actions.py`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.6.0/dynamics/api_functions.py` & `dynamics_client-0.6.1/dynamics/api_functions.py`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.6.0/dynamics/apply_functions.py` & `dynamics_client-0.6.1/dynamics/apply_functions.py`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.6.0/dynamics/client.py` & `dynamics_client-0.6.1/dynamics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,15 +456,15 @@
         self.request_counter += 1
 
         if query is None:
             query = self.current_query
 
         response = self._oauth_client.post(
             url=query,
-            data=data,
+            json=data,
             headers={**self.default_headers("post"), **self.headers},
         )
 
         if response.status_code == status.HTTP_204_NO_CONTENT:
             return {}
 
         try:
@@ -501,15 +501,15 @@
         self.request_counter += 1
 
         if query is None:
             query = self.current_query
 
         response = self._oauth_client.patch(
             url=query,
-            data=data,
+            json=data,
             headers={**self.default_headers("patch"), **self.headers},
         )
 
         if response.status_code == status.HTTP_204_NO_CONTENT:
             return {}
 
         try:
```

### Comparing `dynamics_client-0.6.0/dynamics/enums.py` & `dynamics_client-0.6.1/dynamics/enums.py`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.6.0/dynamics/exceptions.py` & `dynamics_client-0.6.1/dynamics/exceptions.py`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.6.0/dynamics/fetchxml.py` & `dynamics_client-0.6.1/dynamics/fetchxml.py`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.6.0/dynamics/normalizers.py` & `dynamics_client-0.6.1/dynamics/normalizers.py`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.6.0/dynamics/query_functions.py` & `dynamics_client-0.6.1/dynamics/query_functions.py`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.6.0/dynamics/status.py` & `dynamics_client-0.6.1/dynamics/status.py`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.6.0/dynamics/test.py` & `dynamics_client-0.6.1/dynamics/test.py`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.6.0/dynamics/typing.py` & `dynamics_client-0.6.1/dynamics/typing.py`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.6.0/dynamics/utils.py` & `dynamics_client-0.6.1/dynamics/utils.py`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.6.0/pyproject.toml` & `dynamics_client-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dynamics-client"
-version = "0.6.0"
+version = "0.6.1"
 description = "Client for making Web API request from a Microsoft Dynamics 365 Database."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "dynamics" },
 ]
@@ -42,34 +42,33 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 httpx = ">=0.23.3"
 authlib = ">=1.2.0"
 tzdata = ">=2021.5"
 "backports.zoneinfo" = { version = ">=0.2.1", python = "<3.9" }
-typing-extensions = { version = ">=4.5", python = "<3.11" }
+typing-extensions = { version = ">=4.7.1", python = "<3.11" }
 Django = { version = ">=3.2", optional = true }
 djangorestframework = { version = ">=3.12", optional = true }
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.3.0"
-coverage = "6.5.0"
-pytest-asyncio = "0.21.0"
-pre-commit = "3.2.2"
-tox = "4.4.11"
-tox-gh-actions = "3.1.0"
-coveralls = "3.3.1"
+pytest = "7.4.0"
+coverage = "7.2.7"
+pytest-asyncio = "0.21.1"
+pre-commit = "3.3.3"
+tox = "4.6.4"
+tox-gh-actions = "3.1.3"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.4.2"
-pymdown-extensions = "9.11"
-mkdocs-mermaid2-plugin = "0.6.0"
+mkdocs = "1.4.3"
+pymdown-extensions = "10.1"
+mkdocs-mermaid2-plugin = "1.0.1"
 
 [tool.poetry.group.lint.dependencies]
-mypy = "1.2.0"
+mypy = "1.4.1"
 
 [tool.poetry.extras]
 django = ["Django", "djangorestframework"]
 
 [tool.black]
 line-length = 120
```

### Comparing `dynamics_client-0.6.0/PKG-INFO` & `dynamics_client-0.6.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamics-client
-Version: 0.6.0
+Version: 0.6.1
 Summary: Client for making Web API request from a Microsoft Dynamics 365 Database.
 Home-page: https://github.com/MrThearMan/dynamics-client/
 License: MIT
 Keywords: Microsoft,Dynamics,client
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.8,<4
@@ -14,27 +14,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: django
 Requires-Dist: Django (>=3.2) ; extra == "django"
 Requires-Dist: authlib (>=1.2.0)
 Requires-Dist: backports.zoneinfo (>=0.2.1) ; python_version < "3.9"
 Requires-Dist: djangorestframework (>=3.12) ; extra == "django"
 Requires-Dist: httpx (>=0.23.3)
-Requires-Dist: typing-extensions (>=4.5) ; python_version < "3.11"
+Requires-Dist: typing-extensions (>=4.7.1) ; python_version < "3.11"
 Requires-Dist: tzdata (>=2021.5)
 Project-URL: Bug Tracker, https://github.com/MrThearMan/dynamics-client/issues
 Project-URL: Repository, https://github.com/MrThearMan/dynamics-client/
 Description-Content-Type: text/markdown
 
 # Dynamics Web API Client
 
@@ -53,14 +48,16 @@
 
 ---
 
 **Documentation**: [https://mrthearman.github.io/dynamics-client/](https://mrthearman.github.io/dynamics-client/)
 
 **Source Code**: [https://github.com/MrThearMan/dynamics-client/](https://github.com/MrThearMan/dynamics-client/)
 
+**Contributing**: [https://github.com/MrThearMan/dynamics-client/blob/main/CONTRIBUTING.md](https://github.com/MrThearMan/dynamics-client/blob/main/CONTRIBUTING.md)
+
 ---
 
 Client for making Web API request from a Microsoft Dynamics 365 Database.
 
 You should also read the [Dynamics Web API Reference Docs][ref-docs]:
```

