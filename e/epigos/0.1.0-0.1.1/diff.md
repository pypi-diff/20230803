# Comparing `tmp/epigos-0.1.0.tar.gz` & `tmp/epigos-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epigos-0.1.0.tar", max compression
+gzip compressed data, was "epigos-0.1.1.tar", max compression
```

## Comparing `epigos-0.1.0.tar` & `epigos-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1067 2023-08-03 16:09:32.246115 epigos-0.1.0/LICENSE
--rw-r--r--   0        0        0     1883 2023-08-03 16:09:32.246115 epigos-0.1.0/README.md
--rw-r--r--   0        0        0      192 2023-08-03 16:09:32.246115 epigos-0.1.0/epigos/__init__.py
--rw-r--r--   0        0        0       85 2023-08-03 16:09:32.246115 epigos-0.1.0/epigos/__version__.py
--rw-r--r--   0        0        0     3766 2023-08-03 16:09:32.246115 epigos-0.1.0/epigos/client.py
--rw-r--r--   0        0        0      169 2023-08-03 16:09:32.246115 epigos-0.1.0/epigos/core/__init__.py
--rw-r--r--   0        0        0      706 2023-08-03 16:09:32.246115 epigos-0.1.0/epigos/core/base.py
--rw-r--r--   0        0        0     1496 2023-08-03 16:09:32.246115 epigos-0.1.0/epigos/core/classification.py
--rw-r--r--   0        0        0      831 2023-08-03 16:09:32.246115 epigos-0.1.0/epigos/core/object_detection.py
--rw-r--r--   0        0        0     1163 2023-08-03 16:09:32.246115 epigos-0.1.0/epigos/typings.py
--rw-r--r--   0        0        0        0 2023-08-03 16:09:32.246115 epigos-0.1.0/epigos/utils/__init__.py
--rw-r--r--   0        0        0     1341 2023-08-03 16:09:32.246115 epigos-0.1.0/epigos/utils/image.py
--rw-r--r--   0        0        0      782 2023-08-03 16:09:32.246115 epigos-0.1.0/epigos/utils/prediction.py
--rw-r--r--   0        0        0     1877 2023-08-03 16:09:32.246115 epigos-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2663 1970-01-01 00:00:00.000000 epigos-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-03 17:31:47.715775 epigos-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1885 2023-08-03 17:31:47.719775 epigos-0.1.1/README.md
+-rw-r--r--   0        0        0      192 2023-08-03 17:31:47.719775 epigos-0.1.1/epigos/__init__.py
+-rw-r--r--   0        0        0      115 2023-08-03 17:31:47.719775 epigos-0.1.1/epigos/__version__.py
+-rw-r--r--   0        0        0     3766 2023-08-03 17:31:47.719775 epigos-0.1.1/epigos/client.py
+-rw-r--r--   0        0        0      169 2023-08-03 17:31:47.719775 epigos-0.1.1/epigos/core/__init__.py
+-rw-r--r--   0        0        0      706 2023-08-03 17:31:47.719775 epigos-0.1.1/epigos/core/base.py
+-rw-r--r--   0        0        0     1451 2023-08-03 17:31:47.719775 epigos-0.1.1/epigos/core/classification.py
+-rw-r--r--   0        0        0      831 2023-08-03 17:31:47.719775 epigos-0.1.1/epigos/core/object_detection.py
+-rw-r--r--   0        0        0     1163 2023-08-03 17:31:47.719775 epigos-0.1.1/epigos/typings.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:31:47.719775 epigos-0.1.1/epigos/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2023-08-03 17:31:47.719775 epigos-0.1.1/epigos/utils/image.py
+-rw-r--r--   0        0        0      782 2023-08-03 17:31:47.719775 epigos-0.1.1/epigos/utils/prediction.py
+-rw-r--r--   0        0        0     1828 2023-08-03 17:31:47.719775 epigos-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2605 1970-01-01 00:00:00.000000 epigos-0.1.1/PKG-INFO
```

### Comparing `epigos-0.1.0/LICENSE` & `epigos-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `epigos-0.1.0/README.md` & `epigos-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,18 @@
 
 #### Classification
 
 ```python
 import epigos
 
 client = epigos.Epigos("api_key")
+
 # load classification model
 model = client.classification("model_id")
+
 # make predictions
 results = model.predict("path/to/your/image.jpg")
 print(results.json())
 ```
 
 ## Contributing
```

### Comparing `epigos-0.1.0/epigos/client.py` & `epigos-0.1.1/epigos/client.py`

 * *Files identical despite different names*

### Comparing `epigos-0.1.0/epigos/core/base.py` & `epigos-0.1.1/epigos/core/base.py`

 * *Files identical despite different names*

### Comparing `epigos-0.1.0/epigos/core/classification.py` & `epigos-0.1.1/epigos/core/classification.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import typing
-import urllib.parse
 
 from epigos import typings
 from epigos.core.base import PredictionModel
 from epigos.utils import image as image_utils
 from epigos.utils.prediction import Prediction
 
 
@@ -26,15 +25,15 @@
         :param image_path: Path to image (can be local file or remote url).
         :param confidence: Prediction confidence
         :return: Prediction object
         """
         if image_utils.is_path(image_path):
             image = image_utils.image_to_b64(image_path)
         elif image_utils.is_url(image_path):
-            image = urllib.parse.quote_plus(image_path)
+            image = image_path
         else:
             raise ValueError(f"Image does not exist at {image_path}!")
 
         data = {"image": image, "confidence": confidence}
         url = self._build_url()
         res = self._client.call_api(path=url, method="post", json=data)
```

### Comparing `epigos-0.1.0/epigos/core/object_detection.py` & `epigos-0.1.1/epigos/core/object_detection.py`

 * *Files identical despite different names*

### Comparing `epigos-0.1.0/epigos/typings.py` & `epigos-0.1.1/epigos/typings.py`

 * *Files identical despite different names*

### Comparing `epigos-0.1.0/epigos/utils/image.py` & `epigos-0.1.1/epigos/utils/image.py`

 * *Files identical despite different names*

### Comparing `epigos-0.1.0/epigos/utils/prediction.py` & `epigos-0.1.1/epigos/utils/prediction.py`

 * *Files identical despite different names*

### Comparing `epigos-0.1.0/pyproject.toml` & `epigos-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "epigos"
-version = "0.1.0"
+version = "0.1.1"
 description = "Epigos AI Python SDK"
 authors = ["Philip Adzanoukpe <philip@epigos.ai>"]
 license = "MIT"
 readme = "README.md"
 keywords = []
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", ]
-homepage = "https://docs.epigos.ai/sdks/python"
+homepage = "https://github.com/Epigos-Inc/epigos-python"
 documentation = "https://docs.epigos.ai/sdks/python"
-repository = "https://github.com/Epigos-Inc/epigos-python"
+
 [[tool.poetry.packages]]
 include = "epigos"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 httpx = "^0.24.1"
 typing-extensions = "^4.7.1"
```

### Comparing `epigos-0.1.0/PKG-INFO` & `epigos-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: epigos
-Version: 0.1.0
+Version: 0.1.1
 Summary: Epigos AI Python SDK
-Home-page: https://docs.epigos.ai/sdks/python
+Home-page: https://github.com/Epigos-Inc/epigos-python
 License: MIT
 Author: Philip Adzanoukpe
 Author-email: philip@epigos.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Project-URL: Documentation, https://docs.epigos.ai/sdks/python
-Project-URL: Repository, https://github.com/Epigos-Inc/epigos-python
 Description-Content-Type: text/markdown
 
 # Epigos Python
 
 ![Tests](https://github.com/Epigos-Inc/epigos-python/actions/workflows/tests.yaml/badge.svg)
 
 Epigos provides an end-to-end platform to annotate data, train computer vision AI models,
@@ -65,16 +64,18 @@
 
 #### Classification
 
 ```python
 import epigos
 
 client = epigos.Epigos("api_key")
+
 # load classification model
 model = client.classification("model_id")
+
 # make predictions
 results = model.predict("path/to/your/image.jpg")
 print(results.json())
 ```
 
 ## Contributing
```

