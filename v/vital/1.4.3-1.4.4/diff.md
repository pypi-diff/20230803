# Comparing `tmp/vital-1.4.3.tar.gz` & `tmp/vital-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-1.4.3.tar", max compression
+gzip compressed data, was "vital-1.4.4.tar", max compression
```

## Comparing `vital-1.4.3.tar` & `vital-1.4.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      388 2023-08-01 23:30:56.806006 vital-1.4.3/README.md
--rw-r--r--   0        0        0     1123 2023-08-01 23:30:56.806006 vital-1.4.3/pyproject.toml
--rw-r--r--   0        0        0      107 2023-08-01 23:30:56.810006 vital-1.4.3/vital/__init__.py
--rw-r--r--   0        0        0      702 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/__init__.py
--rw-r--r--   0        0        0     1531 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/activity.py
--rw-r--r--   0        0        0      142 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/api.py
--rw-r--r--   0        0        0     2904 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/athome_phlebotomy.py
--rw-r--r--   0        0        0     1515 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/body.py
--rw-r--r--   0        0        0      598 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/devices.py
--rw-r--r--   0        0        0     3306 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/labtests.py
--rw-r--r--   0        0        0     3093 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/link.py
--rw-r--r--   0        0        0      823 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/meals.py
--rw-r--r--   0        0        0      820 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/profile.py
--rw-r--r--   0        0        0        0 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/schema/__init__.py
--rw-r--r--   0        0        0     1719 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/schema/athome_phlebotomy.py
--rw-r--r--   0        0        0     2259 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/sleep.py
--rw-r--r--   0        0        0     2287 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/user.py
--rw-r--r--   0        0        0     3866 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/vitals.py
--rw-r--r--   0        0        0      632 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/webhooks.py
--rw-r--r--   0        0        0     1318 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/workouts.py
--rw-r--r--   0        0        0     5888 2023-08-01 23:30:56.810006 vital-1.4.3/vital/client.py
--rw-r--r--   0        0        0     3118 2023-08-01 23:30:56.810006 vital-1.4.3/vital/errors.py
--rw-r--r--   0        0        0        0 2023-08-01 23:30:56.810006 vital-1.4.3/vital/internal/__init__.py
--rw-r--r--   0        0        0     2363 2023-08-01 23:30:56.810006 vital-1.4.3/vital/internal/requester.py
--rw-r--r--   0        0        0       80 2023-08-01 23:30:56.810006 vital-1.4.3/vital/internal/utils.py
--rw-r--r--   0        0        0     2762 2023-08-01 23:30:56.810006 vital-1.4.3/vital/internal/webhook.py
--rw-r--r--   0        0        0      359 2023-08-01 23:30:56.810006 vital-1.4.3/vital/types.py
--rw-r--r--   0        0        0      239 2023-08-01 23:30:56.810006 vital-1.4.3/vital/version.py
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 vital-1.4.3/setup.py
--rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 vital-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0      388 2023-08-03 18:40:14.650615 vital-1.4.4/README.md
+-rw-r--r--   0        0        0     1123 2023-08-03 18:40:14.650615 vital-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-08-03 18:40:14.650615 vital-1.4.4/vital/__init__.py
+-rw-r--r--   0        0        0      702 2023-08-03 18:40:14.650615 vital-1.4.4/vital/api/__init__.py
+-rw-r--r--   0        0        0     1531 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/activity.py
+-rw-r--r--   0        0        0      142 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/api.py
+-rw-r--r--   0        0        0     2904 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/athome_phlebotomy.py
+-rw-r--r--   0        0        0     1515 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/body.py
+-rw-r--r--   0        0        0      598 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/devices.py
+-rw-r--r--   0        0        0     3870 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/labtests.py
+-rw-r--r--   0        0        0     3093 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/link.py
+-rw-r--r--   0        0        0      823 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/meals.py
+-rw-r--r--   0        0        0      820 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/profile.py
+-rw-r--r--   0        0        0        0 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/schema/__init__.py
+-rw-r--r--   0        0        0     1719 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/schema/athome_phlebotomy.py
+-rw-r--r--   0        0        0     2259 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/sleep.py
+-rw-r--r--   0        0        0     2287 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/user.py
+-rw-r--r--   0        0        0     3866 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/vitals.py
+-rw-r--r--   0        0        0      632 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/webhooks.py
+-rw-r--r--   0        0        0     1318 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/workouts.py
+-rw-r--r--   0        0        0     5888 2023-08-03 18:40:14.654615 vital-1.4.4/vital/client.py
+-rw-r--r--   0        0        0     3118 2023-08-03 18:40:14.654615 vital-1.4.4/vital/errors.py
+-rw-r--r--   0        0        0        0 2023-08-03 18:40:14.654615 vital-1.4.4/vital/internal/__init__.py
+-rw-r--r--   0        0        0     2363 2023-08-03 18:40:14.654615 vital-1.4.4/vital/internal/requester.py
+-rw-r--r--   0        0        0       80 2023-08-03 18:40:14.654615 vital-1.4.4/vital/internal/utils.py
+-rw-r--r--   0        0        0     2762 2023-08-03 18:40:14.654615 vital-1.4.4/vital/internal/webhook.py
+-rw-r--r--   0        0        0      359 2023-08-03 18:40:14.654615 vital-1.4.4/vital/types.py
+-rw-r--r--   0        0        0      239 2023-08-03 18:40:14.654615 vital-1.4.4/vital/version.py
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 vital-1.4.4/setup.py
+-rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 vital-1.4.4/PKG-INFO
```

### Comparing `vital-1.4.3/pyproject.toml` & `vital-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vital"
-version = "1.4.3"
+version = "1.4.4"
 description = ""
 authors = ["maitham <maitham@tryvital.io>"]
 license = "GNU"
 readme = "README.md"
 homepage = "https://github.com/adeptlabs/vital-python"
 repository = "https://github.com/adeptlabs/vital-python"
 keywords = ["vital", "tryvital", "python"]
```

### Comparing `vital-1.4.3/vital/api/__init__.py` & `vital-1.4.4/vital/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/api/activity.py` & `vital-1.4.4/vital/api/activity.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/api/athome_phlebotomy.py` & `vital-1.4.4/vital/api/athome_phlebotomy.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/api/body.py` & `vital-1.4.4/vital/api/body.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/api/devices.py` & `vital-1.4.4/vital/api/devices.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/api/labtests.py` & `vital-1.4.4/vital/api/labtests.py`

 * *Files 13% similar despite different names*

```diff
@@ -70,19 +70,32 @@
     def cancel_order(self, order_id: str) -> Mapping[str, str]:
         """
         Cancel order.
         :param str user_id: The order_id.
         """
         return self.client.post(f"/order/{order_id}/cancel", api_version="v3")
 
+    def search_payor(self, insurance_name: str, insurance_state: Optional[str] = None) -> Mapping[str, str]:
+        params = {
+            "insurance_name": insurance_name
+        }
+
+        if insurance_state:
+            params["insurance_state"] = insurance_state
+
+        return self.client.post("/insurance/search/payor", params, api_version="v3")
+
+    def search_diagnosis(self, diagnosis_query: str) -> Mapping[str, str]:
+        return self.client.get(f"/insurance/search/diagnosis?diagnosis_query={diagnosis_query}", api_version="v3")
+
     def get_tests(self) -> Mapping[str, str]:
         """
         GET all lab tests the team has access to.
         """
-        return self.client.get("/lab_tests")
+        return self.client.get("/lab_tests", api_version="v3")
 
     def get_results(self, order_id: str) -> Mapping[str, str]:
         """
         GET both metadata and raw json test data.
         """
         return self.client.get(f"/order/{order_id}/result", api_version="v3")
```

### Comparing `vital-1.4.3/vital/api/link.py` & `vital-1.4.4/vital/api/link.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/api/meals.py` & `vital-1.4.4/vital/api/meals.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/api/profile.py` & `vital-1.4.4/vital/api/profile.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/api/schema/athome_phlebotomy.py` & `vital-1.4.4/vital/api/schema/athome_phlebotomy.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/api/sleep.py` & `vital-1.4.4/vital/api/sleep.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/api/user.py` & `vital-1.4.4/vital/api/user.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/api/vitals.py` & `vital-1.4.4/vital/api/vitals.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/api/webhooks.py` & `vital-1.4.4/vital/api/webhooks.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/api/workouts.py` & `vital-1.4.4/vital/api/workouts.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/client.py` & `vital-1.4.4/vital/client.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/errors.py` & `vital-1.4.4/vital/errors.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/internal/requester.py` & `vital-1.4.4/vital/internal/requester.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/vital/internal/webhook.py` & `vital-1.4.4/vital/internal/webhook.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.3/setup.py` & `vital-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pydantic>=1.10.7,<2.0.0',
  'requests',
  'svix>=0.41.2,<0.42.0',
  'typed-ast>=1.5.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'vital',
-    'version': '1.4.3',
+    'version': '1.4.4',
     'description': '',
     'long_description': "# vital-python\n\nThe official Python Library for [Vital API](https://docs.tryvital.io)\n\n# Install\n\n```\npip install vital\n```\n\n# Installing locally\n\n```\npoetry build --format sdist\ntar -xvf dist/*-`poetry version -s`.tar.gz -O '*/setup.py' > setup.py\n```\n\n## Documentation\n\nPlease refer to the official [Vital docs](https://docs.tryvital.io) provide a full reference on using this library.\n",
     'author': 'maitham',
     'author_email': 'maitham@tryvital.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/adeptlabs/vital-python',
```

### Comparing `vital-1.4.3/PKG-INFO` & `vital-1.4.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vital
-Version: 1.4.3
+Version: 1.4.4
 Summary: 
 Home-page: https://github.com/adeptlabs/vital-python
 License: GNU
 Keywords: vital,tryvital,python
 Author: maitham
 Author-email: maitham@tryvital.io
 Requires-Python: >=3.8,<4.0
```

