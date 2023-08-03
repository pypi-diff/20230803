# Comparing `tmp/tomodachi_testcontainers-0.2.3.tar.gz` & `tmp/tomodachi_testcontainers-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomodachi_testcontainers-0.2.3.tar", max compression
+gzip compressed data, was "tomodachi_testcontainers-0.3.0.tar", max compression
```

## Comparing `tomodachi_testcontainers-0.2.3.tar` & `tomodachi_testcontainers-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.2.3/LICENSE
--rw-r--r--   0        0        0    26880 2023-07-31 18:13:07.890597 tomodachi_testcontainers-0.2.3/README.md
--rw-r--r--   0        0        0     3996 2023-07-31 18:51:23.321971 tomodachi_testcontainers-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/clients/__init__.py
--rw-r--r--   0        0        0     3487 2023-07-31 18:13:07.895096 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/clients/snssqs_client.py
--rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/__init__.py
--rw-r--r--   0        0        0     3944 2023-07-31 18:13:07.895679 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/common.py
--rw-r--r--   0        0        0     1739 2023-07-31 18:13:07.895948 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/localstack.py
--rw-r--r--   0        0        0     2335 2023-07-31 18:50:45.229403 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/moto.py
--rw-r--r--   0        0        0     3129 2023-07-27 14:17:21.583523 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/sftp.py
--rw-r--r--   0        0        0      930 2023-07-27 14:17:21.583737 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/tomodachi.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/py.typed
--rw-r--r--   0        0        0     1394 2023-07-31 18:13:07.896643 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/__init__.py
--rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/assertions.py
--rw-r--r--   0        0        0     2312 2023-07-31 18:13:07.897004 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
--rw-r--r--   0        0        0     2126 2023-07-31 18:13:07.897240 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/moto_fixtures.py
--rw-r--r--   0        0        0     1594 2023-07-31 12:23:17.273453 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
--rw-r--r--   0        0        0      609 2023-07-29 08:49:13.269030 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
--rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/utils.py
--rw-r--r--   0        0        0    28069 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.3.0/LICENSE
+-rw-r--r--   0        0        0    26880 2023-07-31 18:13:07.890597 tomodachi_testcontainers-0.3.0/README.md
+-rw-r--r--   0        0        0     3997 2023-08-03 07:36:53.880150 tomodachi_testcontainers-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/clients/__init__.py
+-rw-r--r--   0        0        0     3487 2023-07-31 18:13:07.895096 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/clients/snssqs_client.py
+-rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/__init__.py
+-rw-r--r--   0        0        0     3944 2023-07-31 18:13:07.895679 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/common.py
+-rw-r--r--   0        0        0     1942 2023-08-03 07:36:44.798845 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/localstack.py
+-rw-r--r--   0        0        0     2345 2023-08-03 07:36:44.799109 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/moto.py
+-rw-r--r--   0        0        0     3129 2023-07-27 14:17:21.583523 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/sftp.py
+-rw-r--r--   0        0        0      930 2023-07-27 14:17:21.583737 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/tomodachi.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/py.typed
+-rw-r--r--   0        0        0     1394 2023-07-31 18:13:07.896643 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/__init__.py
+-rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/assertions.py
+-rw-r--r--   0        0        0     1121 2023-08-03 07:36:44.799354 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/async_probes.py
+-rw-r--r--   0        0        0     2312 2023-07-31 18:13:07.897004 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
+-rw-r--r--   0        0        0     2126 2023-08-02 12:29:30.549037 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/moto_fixtures.py
+-rw-r--r--   0        0        0     1594 2023-07-31 12:23:17.273453 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
+-rw-r--r--   0        0        0      609 2023-07-29 08:49:13.269030 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
+-rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/utils.py
+-rw-r--r--   0        0        0    28110 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.3.0/PKG-INFO
```

### Comparing `tomodachi_testcontainers-0.2.3/LICENSE` & `tomodachi_testcontainers-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.3/README.md` & `tomodachi_testcontainers-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.3/pyproject.toml` & `tomodachi_testcontainers-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "tomodachi-testcontainers"
-version = "0.2.3"
+version = "0.3.0"
 description = "Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing."
 authors = ["Filips Nastins <nastinsfilips@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/filipsnastins/tomodachi-testcontainers"
 repository = "https://github.com/filipsnastins/tomodachi-testcontainers"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 aiobotocore = "^2.5.2"
 asyncssh = { version = "^2.13.2", optional = true }
 pytest = "^7.1.2"
 pytest-asyncio = "^0.21.1"
+tenacity = "^8.2.2"
 testcontainers = "^3.7.1"
 types-aiobotocore = { extras = [
     "dynamodb",
     "s3",
     "sns",
     "sqs",
     "ssm",
 ], version = "^2.5.2" }
 
 [tool.poetry.group.dev.dependencies]
 autoflake = "^2.2.0"
 bandit = "^1.7.5"
 black = "^23.7.0"
-busypie = "^0.5.1"
 colorama = "^0.4.6"
 flake8 = "^6.0.0"
 flake8-annotations = "^3.0.1"
 flake8-black = "^0.3.6"
 flake8-bugbear = "^23.5.9"
 flake8-executable = "^2.1.3"
 flake8-isort = "^6.0.0"
```

### Comparing `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/clients/snssqs_client.py` & `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/clients/snssqs_client.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/__init__.py` & `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/common.py` & `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/common.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/localstack.py` & `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/localstack.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 
         self.region_name = region_name or os.environ.get("AWS_DEFAULT_REGION") or "us-east-1"
         self.aws_access_key_id = os.environ.get("AWS_ACCESS_KEY_ID") or "testing"  # nosec: B105
         self.aws_secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY") or "testing"  # nosec: B105
 
         self.with_bind_ports(self.internal_port, self.edge_port)
 
+        # Docker is needed for running AWS Lambda container
+        self.with_env("LAMBDA_DOCKER_NETWORK", self.network)
+        self.with_volume_mapping("/var/run/docker.sock", "/var/run/docker.sock")
+
     def get_internal_url(self) -> str:
         ip = self.get_container_internal_ip()
         return f"http://{ip}:{self.internal_port}"
 
     def get_external_url(self) -> str:
         host = self.get_container_host_ip()
         return f"http://{host}:{self.edge_port}"
```

### Comparing `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/moto.py` & `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/moto.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.with_bind_ports(self.internal_port, self.edge_port)
         self.with_env("AWS_DEFAULT_REGION", self.region_name)
         self.with_env("AWS_ACCESS_KEY_ID", self.aws_access_key_id)
         self.with_env("AWS_SECRET_ACCESS_KEY", self.aws_secret_access_key)
 
         self.with_env("MOTO_PORT", str(self.internal_port))
 
-        # Docker is needed for Lambda
+        # Docker is needed for running AWS Lambda container
         self.with_env("MOTO_DOCKER_NETWORK_NAME", self.network)
         self.with_volume_mapping("/var/run/docker.sock", "/var/run/docker.sock")
 
     def get_internal_url(self) -> str:
         ip = self.get_container_internal_ip()
         return f"http://{ip}:{self.internal_port}"
 
@@ -53,8 +53,8 @@
 
     def start(self, timeout: float = 10) -> "MotoContainer":
         super().start()
         wait_for_logs(self, "Running on all addresses", timeout=timeout)
         return self
 
     def reset_moto(self) -> None:
-        self.exec(["sh", "-c", "curl", "-X", "POST", f"http://localhost:{self.internal_port}/moto-api/reset"])
+        self.exec(["curl", "-X", "POST", f"http://localhost:{self.internal_port}/moto-api/reset"])
```

### Comparing `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/sftp.py` & `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/sftp.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/tomodachi.py` & `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/tomodachi.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/__init__.py` & `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/localstack_fixtures.py` & `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/localstack_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/moto_fixtures.py` & `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/moto_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/sftp_fixtures.py` & `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/sftp_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py` & `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.3/PKG-INFO` & `tomodachi_testcontainers-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomodachi-testcontainers
-Version: 0.2.3
+Version: 0.3.0
 Summary: Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing.
 Home-page: https://github.com/filipsnastins/tomodachi-testcontainers
 License: MIT
 Author: Filips Nastins
 Author-email: nastinsfilips@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: sftp
 Requires-Dist: aiobotocore (>=2.5.2,<3.0.0)
 Requires-Dist: asyncssh (>=2.13.2,<3.0.0) ; extra == "sftp"
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.21.1,<0.22.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: testcontainers (>=3.7.1,<4.0.0)
 Requires-Dist: types-aiobotocore[dynamodb,s3,sns,sqs,ssm] (>=2.5.2,<3.0.0)
 Project-URL: Repository, https://github.com/filipsnastins/tomodachi-testcontainers
 Description-Content-Type: text/markdown
 
 # tomodachi-testcontainers
```

