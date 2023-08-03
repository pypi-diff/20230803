# Comparing `tmp/google-cloud-bigquery-connection-1.9.0.tar.gz` & `tmp/google-cloud-bigquery-connection-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-connection-1.9.0.tar", last modified: Tue Jan 10 20:34:06 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-connection-1.9.1.tar", last modified: Mon Jan 23 19:55:18 2023, max compression
```

## Comparing `google-cloud-bigquery-connection-1.9.0.tar` & `google-cloud-bigquery-connection-1.9.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:34:06.875399 google-cloud-bigquery-connection-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4817 2023-01-10 20:34:06.875399 google-cloud-bigquery-connection-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3865 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:34:06.867398 google-cloud-bigquery-connection-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:34:06.867398 google-cloud-bigquery-connection-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:34:06.867398 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection/
--rw-rw-r--   0 root         (0)     1003     1897 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:34:06.871398 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/
--rw-rw-r--   0 root         (0)     1003     1727 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2592 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:34:06.871398 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:34:06.871398 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    54587 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    63008 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/client.py
--rw-rw-r--   0 root         (0)     1003     5913 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:34:06.871398 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/transports/
--rw-rw-r--   0 root         (0)     1003     1220 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10728 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20808 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    21179 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:34:06.871398 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/types/
--rw-rw-r--   0 root         (0)     1003     1423 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    17354 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/types/connection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:34:06.871398 google-cloud-bigquery-connection-1.9.0/google_cloud_bigquery_connection.egg-info/
--rw-r--r--   0 root         (0)     1003     4817 2023-01-10 20:34:06.000000 google-cloud-bigquery-connection-1.9.0/google_cloud_bigquery_connection.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1807 2023-01-10 20:34:06.000000 google-cloud-bigquery-connection-1.9.0/google_cloud_bigquery_connection.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-10 20:34:06.000000 google-cloud-bigquery-connection-1.9.0/google_cloud_bigquery_connection.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-10 20:34:06.000000 google-cloud-bigquery-connection-1.9.0/google_cloud_bigquery_connection.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-10 20:34:06.000000 google-cloud-bigquery-connection-1.9.0/google_cloud_bigquery_connection.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-01-10 20:34:06.000000 google-cloud-bigquery-connection-1.9.0/google_cloud_bigquery_connection.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-10 20:34:06.000000 google-cloud-bigquery-connection-1.9.0/google_cloud_bigquery_connection.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-10 20:34:06.875399 google-cloud-bigquery-connection-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3076 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:34:06.871398 google-cloud-bigquery-connection-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/tests/__init__.py
--rw-rw-r--   0 root         (0)     1003     1011 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/tests/system.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:34:06.875399 google-cloud-bigquery-connection-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:34:06.875399 google-cloud-bigquery-connection-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:34:06.875399 google-cloud-bigquery-connection-1.9.0/tests/unit/gapic/bigquery_connection_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/tests/unit/gapic/bigquery_connection_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   132786 2023-01-10 20:30:43.000000 google-cloud-bigquery-connection-1.9.0/tests/unit/gapic/bigquery_connection_v1/test_connection_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 19:55:18.779945 google-cloud-bigquery-connection-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4817 2023-01-23 19:55:18.779945 google-cloud-bigquery-connection-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3865 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 19:55:18.771947 google-cloud-bigquery-connection-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 19:55:18.771947 google-cloud-bigquery-connection-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 19:55:18.771947 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection/
+-rw-rw-r--   0 root         (0)     1003     1897 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 19:55:18.771947 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/
+-rw-rw-r--   0 root         (0)     1003     1727 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2592 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 19:55:18.771947 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 19:55:18.775946 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    54587 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    63037 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5913 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 19:55:18.775946 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1220 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10728 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20808 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21179 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 19:55:18.775946 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1423 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17594 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/types/connection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 19:55:18.775946 google-cloud-bigquery-connection-1.9.1/google_cloud_bigquery_connection.egg-info/
+-rw-r--r--   0 root         (0)     1003     4817 2023-01-23 19:55:18.000000 google-cloud-bigquery-connection-1.9.1/google_cloud_bigquery_connection.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1807 2023-01-23 19:55:18.000000 google-cloud-bigquery-connection-1.9.1/google_cloud_bigquery_connection.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 19:55:18.000000 google-cloud-bigquery-connection-1.9.1/google_cloud_bigquery_connection.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-01-23 19:55:18.000000 google-cloud-bigquery-connection-1.9.1/google_cloud_bigquery_connection.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 19:55:18.000000 google-cloud-bigquery-connection-1.9.1/google_cloud_bigquery_connection.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-01-23 19:55:18.000000 google-cloud-bigquery-connection-1.9.1/google_cloud_bigquery_connection.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-01-23 19:55:18.000000 google-cloud-bigquery-connection-1.9.1/google_cloud_bigquery_connection.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-01-23 19:55:18.779945 google-cloud-bigquery-connection-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3076 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 19:55:18.775946 google-cloud-bigquery-connection-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/tests/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1011 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/tests/system.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 19:55:18.779945 google-cloud-bigquery-connection-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 19:55:18.779945 google-cloud-bigquery-connection-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 19:55:18.779945 google-cloud-bigquery-connection-1.9.1/tests/unit/gapic/bigquery_connection_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/tests/unit/gapic/bigquery_connection_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   132786 2023-01-23 19:51:48.000000 google-cloud-bigquery-connection-1.9.1/tests/unit/gapic/bigquery_connection_v1/test_connection_service.py
```

### Comparing `google-cloud-bigquery-connection-1.9.0/LICENSE` & `google-cloud-bigquery-connection-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/MANIFEST.in` & `google-cloud-bigquery-connection-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/PKG-INFO` & `google-cloud-bigquery-connection-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-connection
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Bigquery Connection API client library
 Home-page: https://github.com/googleapis/python-bigquery-connection
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-bigquery-connection-1.9.0/README.rst` & `google-cloud-bigquery-connection-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection/__init__.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection/gapic_version.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/__init__.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/gapic_metadata.json` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/gapic_version.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/__init__.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/__init__.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/async_client.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/client.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1453,15 +1453,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "ConnectionServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/pagers.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/transports/__init__.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/transports/base.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/transports/grpc.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/services/connection_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/services/connection_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/types/__init__.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/google/cloud/bigquery_connection_v1/types/connection.py` & `google-cloud-bigquery-connection-1.9.1/google/cloud/bigquery_connection_v1/types/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,24 @@
             operation in BigQuery, this service account will
             serve as identity being used for connecting to
             the CloudSQL instance specified in this
             connection.
     """
 
     class DatabaseType(proto.Enum):
-        r"""Supported Cloud SQL database types."""
+        r"""Supported Cloud SQL database types.
+
+        Values:
+            DATABASE_TYPE_UNSPECIFIED (0):
+                Unspecified database type.
+            POSTGRES (1):
+                Cloud SQL for PostgreSQL.
+            MYSQL (2):
+                Cloud SQL for MySQL.
+        """
         DATABASE_TYPE_UNSPECIFIED = 0
         POSTGRES = 1
         MYSQL = 2
 
     instance_id: str = proto.Field(
         proto.STRING,
         number=1,
```

### Comparing `google-cloud-bigquery-connection-1.9.0/google_cloud_bigquery_connection.egg-info/PKG-INFO` & `google-cloud-bigquery-connection-1.9.1/google_cloud_bigquery_connection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-connection
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Bigquery Connection API client library
 Home-page: https://github.com/googleapis/python-bigquery-connection
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-bigquery-connection-1.9.0/google_cloud_bigquery_connection.egg-info/SOURCES.txt` & `google-cloud-bigquery-connection-1.9.1/google_cloud_bigquery_connection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/setup.py` & `google-cloud-bigquery-connection-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/tests/__init__.py` & `google-cloud-bigquery-connection-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/tests/system.py` & `google-cloud-bigquery-connection-1.9.1/tests/system.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/tests/unit/__init__.py` & `google-cloud-bigquery-connection-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-connection-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/tests/unit/gapic/bigquery_connection_v1/__init__.py` & `google-cloud-bigquery-connection-1.9.1/tests/unit/gapic/bigquery_connection_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-connection-1.9.0/tests/unit/gapic/bigquery_connection_v1/test_connection_service.py` & `google-cloud-bigquery-connection-1.9.1/tests/unit/gapic/bigquery_connection_v1/test_connection_service.py`

 * *Files identical despite different names*

