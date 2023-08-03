# Comparing `tmp/Colectica_API-0.0.3.tar.gz` & `tmp/Colectica_API-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Colectica_API-0.0.3.tar", last modified: Mon Jul 17 22:18:41 2023, max compression
+gzip compressed data, was "Colectica_API-0.0.4.tar", last modified: Thu Aug  3 06:41:32 2023, max compression
```

## Comparing `Colectica_API-0.0.3.tar` & `Colectica_API-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:41.005998 Colectica_API-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:41.005998 Colectica_API-0.0.3/Colectica_API.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-17 22:18:40.000000 Colectica_API-0.0.3/Colectica_API.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-17 22:18:41.000000 Colectica_API-0.0.3/Colectica_API.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:18:40.000000 Colectica_API-0.0.3/Colectica_API.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 22:18:40.000000 Colectica_API-0.0.3/Colectica_API.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 22:18:40.000000 Colectica_API-0.0.3/Colectica_API.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-17 22:18:26.000000 Colectica_API-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-17 22:18:41.005998 Colectica_API-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-17 22:18:26.000000 Colectica_API-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:41.005998 Colectica_API-0.0.3/colectica_api/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-17 22:18:26.000000 Colectica_API-0.0.3/colectica_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28108 2023-07-17 22:18:26.000000 Colectica_API-0.0.3/colectica_api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55927 2023-07-17 22:18:26.000000 Colectica_API-0.0.3/colectica_api/colectica.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-17 22:18:26.000000 Colectica_API-0.0.3/colectica_api/test_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-17 22:18:26.000000 Colectica_API-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:18:41.005998 Colectica_API-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:41:32.232200 Colectica_API-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:41:32.228200 Colectica_API-0.0.4/Colectica_API.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-08-03 06:41:32.000000 Colectica_API-0.0.4/Colectica_API.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-03 06:41:32.000000 Colectica_API-0.0.4/Colectica_API.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:41:32.000000 Colectica_API-0.0.4/Colectica_API.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 06:41:32.000000 Colectica_API-0.0.4/Colectica_API.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 06:41:32.000000 Colectica_API-0.0.4/Colectica_API.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-03 06:41:22.000000 Colectica_API-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-08-03 06:41:32.232200 Colectica_API-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-03 06:41:22.000000 Colectica_API-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:41:32.232200 Colectica_API-0.0.4/colectica_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-03 06:41:22.000000 Colectica_API-0.0.4/colectica_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28988 2023-08-03 06:41:22.000000 Colectica_API-0.0.4/colectica_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55927 2023-08-03 06:41:22.000000 Colectica_API-0.0.4/colectica_api/colectica.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-03 06:41:22.000000 Colectica_API-0.0.4/colectica_api/test_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-08-03 06:41:22.000000 Colectica_API-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:41:32.232200 Colectica_API-0.0.4/setup.cfg
```

### Comparing `Colectica_API-0.0.3/Colectica_API.egg-info/PKG-INFO` & `Colectica_API-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Colectica-API
-Version: 0.0.3
+Name: Colectica_API
+Version: 0.0.4
 Summary: Python interface to the Colectica API
 Author-email: Jenny Li <jenny.li@ucl.ac.uk>
 Project-URL: Homepage, https://github.com/CLOSER-Cohorts/colectica_api
 Project-URL: Bug Tracker, https://github.com/CLOSER-Cohorts/colectica_api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,49 +25,69 @@
 pip install colectica_api
 ```
 
 ## Basic usage
 
 ```
 from colectica_api import ColecticaObject
-C = ColecticaObject(colectica.example.com, <username>, <password>)
+C = ColecticaObject("colectica.example.com", <username>, <password>)
 C.search_item(...)
 ```
 
 See `example.ipynb` for a more complete example.
 
 
 ## Closer Discovery relationship graph
 
 Work-in-progress!
 
 ```mermaid
 graph LR
-  QG[Question Group] --> Concept
-  QG[Question Group] --> QG[Question Group]
+  VS[Variable Set] --> VG[Variable Group]
+  QGr[Question Group] --> Concept
+  QGr[Question Group] --> QGr[Question Group]
+  VG[Variable Group] --> Variable
   VG[Variable Group] --> Concept
   CS[Concept Set] --> Concept
+  MetP[Metadata Package] --> InS[Instrument Set]
+  MetP[Metadata Package] --> QuS[Question Set]
+  MetP[Metadata Package] --> IIS[Interviewer Instruction Set]
+  MetP[Metadata Package] --> CCS[Control Construct Set]
+  MetP[Metadata Package] --> CaS[Category Set]
+  MetP[Metadata Package] --> CLS[Code List Set]
+  QuS[Question Set] --> Question
+  OrS[Organization Set] -->  Organization
+  UnS[Universe Set] --> Universe
+  UnG[Universe Group] --> Universe
   Project --> Series
   Series --> Organization
   Series --> Universe
   Series --> Study
   Study --> Organization
   Study --> Universe
   Study --> DaC[Data Collection]
   Study --> DaF[Data File]
   DaC[Data Collection] --> Organization
+  UnG[Universe Group] --> Universe
+  InS[Instrument Set] --> Instrument
   Instrument --> Sequence
   Sequence --> Sequence
   Sequence --> Statement
   Sequence --> QA[Question Activity]
   QA[Question Activity] --> Question
+  QG[Question Grid] --> CoS[Code Set]
+  QG[Question Grid] --> II[Interviewer Instruction]
   Question --> CoS[Code Set]
+  CLS[Code List Set] --> CoS[Code Set]
   CoS --> Category
+  CaS[Category Set] --> Category
   CCS[Control Construct Set] --> Sequence
   Conditional --> Sequence
   CCS[Control Construct Set] --> Conditional
   CCS[Control Construct Set] --> Statement
   CCS[Control Construct Set] --> QA[Question Activity]
   DaF[Data file] --> DL[Data Layout]
   DaF[Data file] --> VaS[Variable Statistic]
   VaS[Variable Statistic] --> Variable
+  IIS[Interviewer Instruction Set] --> II[Interviewer Instruction]
+  loop --> Sequence
 ```
```

### Comparing `Colectica_API-0.0.3/LICENSE` & `Colectica_API-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Colectica_API-0.0.3/PKG-INFO` & `Colectica_API-0.0.4/Colectica_API.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Colectica_API
-Version: 0.0.3
+Name: Colectica-API
+Version: 0.0.4
 Summary: Python interface to the Colectica API
 Author-email: Jenny Li <jenny.li@ucl.ac.uk>
 Project-URL: Homepage, https://github.com/CLOSER-Cohorts/colectica_api
 Project-URL: Bug Tracker, https://github.com/CLOSER-Cohorts/colectica_api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,49 +25,69 @@
 pip install colectica_api
 ```
 
 ## Basic usage
 
 ```
 from colectica_api import ColecticaObject
-C = ColecticaObject(colectica.example.com, <username>, <password>)
+C = ColecticaObject("colectica.example.com", <username>, <password>)
 C.search_item(...)
 ```
 
 See `example.ipynb` for a more complete example.
 
 
 ## Closer Discovery relationship graph
 
 Work-in-progress!
 
 ```mermaid
 graph LR
-  QG[Question Group] --> Concept
-  QG[Question Group] --> QG[Question Group]
+  VS[Variable Set] --> VG[Variable Group]
+  QGr[Question Group] --> Concept
+  QGr[Question Group] --> QGr[Question Group]
+  VG[Variable Group] --> Variable
   VG[Variable Group] --> Concept
   CS[Concept Set] --> Concept
+  MetP[Metadata Package] --> InS[Instrument Set]
+  MetP[Metadata Package] --> QuS[Question Set]
+  MetP[Metadata Package] --> IIS[Interviewer Instruction Set]
+  MetP[Metadata Package] --> CCS[Control Construct Set]
+  MetP[Metadata Package] --> CaS[Category Set]
+  MetP[Metadata Package] --> CLS[Code List Set]
+  QuS[Question Set] --> Question
+  OrS[Organization Set] -->  Organization
+  UnS[Universe Set] --> Universe
+  UnG[Universe Group] --> Universe
   Project --> Series
   Series --> Organization
   Series --> Universe
   Series --> Study
   Study --> Organization
   Study --> Universe
   Study --> DaC[Data Collection]
   Study --> DaF[Data File]
   DaC[Data Collection] --> Organization
+  UnG[Universe Group] --> Universe
+  InS[Instrument Set] --> Instrument
   Instrument --> Sequence
   Sequence --> Sequence
   Sequence --> Statement
   Sequence --> QA[Question Activity]
   QA[Question Activity] --> Question
+  QG[Question Grid] --> CoS[Code Set]
+  QG[Question Grid] --> II[Interviewer Instruction]
   Question --> CoS[Code Set]
+  CLS[Code List Set] --> CoS[Code Set]
   CoS --> Category
+  CaS[Category Set] --> Category
   CCS[Control Construct Set] --> Sequence
   Conditional --> Sequence
   CCS[Control Construct Set] --> Conditional
   CCS[Control Construct Set] --> Statement
   CCS[Control Construct Set] --> QA[Question Activity]
   DaF[Data file] --> DL[Data Layout]
   DaF[Data file] --> VaS[Variable Statistic]
   VaS[Variable Statistic] --> Variable
+  IIS[Interviewer Instruction Set] --> II[Interviewer Instruction]
+  loop --> Sequence
 ```
```

### Comparing `Colectica_API-0.0.3/colectica_api/api.py` & `Colectica_API-0.0.4/colectica_api/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 In most cases you'll want to work with :class:`ColecticaObject` instead.
 """
 
 import json
 import os
 
 import requests
+import urllib3
 
 
 # item type dictionary
 #   See Item Type Identifiers for a list of identifiers for all item types.
 #   https://docs.colectica.com/repository/technical/item-type-identifiers/
 item_dict = {
     "Action": "0b70f0ba-602a-4575-a15c-91f0915bae36",
@@ -111,30 +112,32 @@
     "Variable Statistic": "3b438f9f-e039-4eac-a06d-3fa1aedf48bb",
     "While": "0681e606-ba3f-453c-9fdd-10670e8e045c",
 }
 
 item_dict_inv = {v: k for k, v in item_dict.items()}
 
 
-def get_jwtToken(hostname, username, password):
+def get_jwtToken(hostname, username, password, verify_ssl=True):
     """
     First obtain a JWT access token
     documented at https://docs.colectica.com/portal/technical/deployment/local-jwt-provider/#usage
+    
+    Raises:
+        RuntimeError: if cannot get a token, such as invalid login.
     """
     tokenEndpoint = "https://" + hostname + "/token/createtoken"
     response = requests.post(
         tokenEndpoint,
         json={"username": username, "password": password},
         allow_redirects=True,
-        verify=False,
+        verify=verify_ssl,
     )
 
-    if response.ok is not True:
-        print("Could not get token. Status code: ", response.status_code)
-        quit()
+    if not response.ok:
+        raise RuntimeError("Could not get token. Status code: ", response.status_code)
 
     jsonResponse = response.json()
     jwtToken = jsonResponse["access_token"]
     tokenHeader = {"Authorization": "Bearer " + jwtToken}
 
     # get Repository information
     # response = requests.get("https://"+self.host+"/api/v1/repository/info", headers=tokenHeader, verify=False)
@@ -154,24 +157,39 @@
     >>> C = ColecticaBasicAPI(hostname, username, password)
 
     If `hostname`, `username` or `password` are omitted, environment
     variables `COLECTICA_HOSTNAME`, `COLECTICA_USERNAME` and `COLECTICA_PASSWORD`
     will be used, if they are defined.
     """
 
-    def __init__(self, hostname=None, username=None, password=None):
+    def __init__(self, hostname=None, username=None, password=None, *, verify_ssl=True):
         if hostname is None:
             hostname = os.environ.get("COLECTICA_HOSTNAME")
         if username is None:
             username = os.environ.get("COLECTICA_USERNAME")
         if password is None:
             password = os.environ.get("COLECTICA_PASSWORD")
         print(f"Connecting to {hostname} as user {username}")
         self.host = hostname
-        self.token = get_jwtToken(hostname, username, password)
+        self.verify = verify_ssl
+        if not self.verify:
+            print("Disabled SSL verification")
+            self._be_quiet_urllib3()
+        self.token = get_jwtToken(hostname, username, password, verify_ssl=self.verify)
+
+    def _be_quiet_urllib3(self):
+        """Disable a warning when user has explicitly disabled SSL verification.
+        
+        If the server does not have a valid ssl certificate, users can
+        disable SSL verification, but they will still get a warning coming
+        from urllib3 library.  This silences the warning, but only when
+        SSL verification is off.
+        """
+        if not self.verify:
+            urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
     @classmethod
     def item_code(self, item):
         return item_dict[item]
 
     @classmethod
     def item_code_inv(self, item_type_id):
@@ -198,15 +216,15 @@
         Exceptions:
             ValueError: the request did not succeed.
         """
         uri = "https://" + self.host + "/api/v1/item/" + AgencyId + "/" + Identifier
         # use explicit None check so that zero treated
         if version is not None:
             uri += f"/{version}"
-        response = requests.get(uri, headers=self.token, verify=False)
+        response = requests.get(uri, headers=self.token, verify=self.verify)
         if not response.ok:
             raise ValueError(response.text)
         return response.json()
 
     def get_item_json(self, AgencyId, Identifier, *, version=None):
         """Gets an item
 
@@ -230,15 +248,15 @@
             ValueError: the request did not succeed.
         """
 
         uri = "https://" + self.host + "/api/v1/json/" + AgencyId + "/" + Identifier
         # use explicit None check so that zero treated
         if version is not None:
             uri += f"/{version}"
-        response = requests.get(uri, headers=self.token, verify=False)
+        response = requests.get(uri, headers=self.token, verify=self.verify)
         if not response.ok:
             raise ValueError(response.text)
         return response.json()
 
     # backwards compatibility for old calls without a warning
     # get_an_item = get_item_xml
 
@@ -270,15 +288,15 @@
             ValueError: the request did not succeed.
         """
 
         uri = "https://" + self.host + "/api/v1/jsonset/" + AgencyId + "/" + Identifier
         # use explicit None check so that zero treated
         if version is not None:
             uri += f"/{version}"
-        response = requests.get(uri, headers=self.token, verify=False)
+        response = requests.get(uri, headers=self.token, verify=self.verify)
         if not response.ok:
             raise ValueError(response.text)
         return response.json()
 
     def get_item_version_history(self, AgencyId, Identifier):
         """Gets the version history of an item.
 
@@ -293,15 +311,15 @@
         Returns:
             dict:
 
         Exceptions:
             ValueError: the request did not succeed.
         """
         uri = f"https://{self.host}/api/v1/item/{AgencyId}/{Identifier}/history"
-        response = requests.get(uri, headers=self.token, verify=False)
+        response = requests.get(uri, headers=self.token, verify=self.verify)
         if not response.ok:
             raise ValueError(response.text)
         return response.json()
 
     def get_item_description(self, AgencyId, Identifier, Version):
         """Gets a description of a repository item.
 
@@ -331,15 +349,15 @@
             + AgencyId
             + "/"
             + Identifier
             + "/"
             + str(Version)
             + "/description",
             headers=self.token,
-            verify=False,
+            verify=self.verify,
         )
         if not response.ok:
             raise ValueError(response.text)
         return response.json()
 
     def search_item(
         self,
@@ -397,15 +415,15 @@
         if UsePrefixSearch is not None:
             query["UsePrefixSearch"] = UsePrefixSearch
 
         response = requests.post(
             "https://" + self.host + "/api/v1/_query/",
             headers=self.token,
             json=query,
-            verify=False,
+            verify=self.verify,
         )
         if response.ok:
             return response.json()
         raise ValueError(
             f"Server returned {response.status_code} error: {response.content}"
         )
 
@@ -473,15 +491,15 @@
             query["UseDistinctResultItem"] = UseDistinctResultItem
         if UseDistinctTargetItem is not None:
             query["UseDistinctTargetItem"] = UseDistinctTargetItem
 
         url = f"https://{self.host}/api/v1/_query/relationship/bysubject/"
         if Descriptions:
             url += "descriptions"
-        response = requests.post(url, headers=self.token, json=query, verify=False)
+        response = requests.post(url, headers=self.token, json=query, verify=self.verify)
         if response.ok:
             return response.json()
         raise ValueError(
             f"Server returned {response.status_code} error: {response.content}"
         )
 
     def search_relationship_byobject(
@@ -548,15 +566,15 @@
             query["UseDistinctResultItem"] = UseDistinctResultItem
         if UseDistinctTargetItem is not None:
             query["UseDistinctTargetItem"] = UseDistinctTargetItem
 
         url = f"https://{self.host}/api/v1/_query/relationship/byobject/"
         if Descriptions:
             url += "descriptions"
-        response = requests.post(url, headers=self.token, json=query, verify=False)
+        response = requests.post(url, headers=self.token, json=query, verify=self.verify)
         if response.ok:
             return response.json()
         raise ValueError(
             f"Server returned {response.status_code} error: {response.content}"
         )
 
     def search_set(
@@ -598,15 +616,15 @@
                 {"agencyId": AgencyId, "identifier": Identifier, "version": 1}
             ],
         }
         response = requests.post(
             "https://" + self.host + "/api/v1/_query/",
             headers=self.token,
             json=query,
-            verify=False,
+            verify=self.verify,
         )
         if response.ok:
             return response.json()
         raise ValueError(
             f"Server returned {response.status_code} error: {response.content}"
         )
 
@@ -629,15 +647,15 @@
             "Facet": {"Predicate": Predicate, "ReverseTraversal": ReverseTraversal},
         }
 
         response = requests.post(
             "https://" + self.host + "/api/v1/_query/relationship/matrix",
             headers=self.token,
             json=jsonquery,
-            verify=False,
+            verify=self.verify,
         )
         if response.ok:
             if response.json() != []:
                 return response.json()
 
     def relationship_matrix_typed(
         self, AgencyId, Identifier, Version, Predicate, ReverseTraversal=True
@@ -656,15 +674,15 @@
             "Facet": {"Predicate": Predicate, "ReverseTraversal": ReverseTraversal},
         }
 
         response = requests.post(
             "https://" + self.host + "/api/v1/_query/relationship/matrix/typed",
             headers=self.token,
             json=jsonquery,
-            verify=False,
+            verify=self.verify,
         )
         if response.ok:
             if response.json() != []:
                 return response.json()
 
     def get_a_set(self, AgencyId, Identifier, Version):
         """Gets the set of all items under the specified root.
@@ -690,15 +708,15 @@
             + "/api/v1/set/"
             + AgencyId
             + "/"
             + Identifier
             + "/"
             + Version,
             headers=self.token,
-            verify=False,
+            verify=self.verify,
         )
         if response.ok:
             if response.json() != []:
                 return response.json()
 
     def get_a_set_typed(self, AgencyId, Identifier, Version):
         """
@@ -715,15 +733,15 @@
             + AgencyId
             + "/"
             + Identifier
             + "/"
             + Version
             + "/typed",
             headers=self.token,
-            verify=False,
+            verify=self.verify,
         )
         if response.ok:
             if response.json() != []:
                 return response.json()
 
     def get_a_set_lasted(self, AgencyId, Identifier):
         """
@@ -732,15 +750,15 @@
         Request Type: GET
         URL: /api/v1/set/{agency}/{id}
         """
 
         response = requests.get(
             "https://" + self.host + "/api/v1/set/" + AgencyId + "/" + Identifier,
             headers=self.token,
-            verify=False,
+            verify=self.verify,
         )
         if response.ok:
             if response.json() != []:
                 return response.json()
 
 
 if __name__ == "__main__":
```

### Comparing `Colectica_API-0.0.3/colectica_api/colectica.py` & `Colectica_API-0.0.4/colectica_api/colectica.py`

 * *Files identical despite different names*

### Comparing `Colectica_API-0.0.3/pyproject.toml` & `Colectica_API-0.0.4/pyproject.toml`

 * *Files identical despite different names*

