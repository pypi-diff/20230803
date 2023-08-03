# Comparing `tmp/reasoner-pydantic-4.1.2.tar.gz` & `tmp/reasoner-pydantic-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-pydantic-4.1.2.tar", last modified: Wed Jul 26 18:23:14 2023, max compression
+gzip compressed data, was "reasoner-pydantic-4.1.3.tar", last modified: Thu Aug  3 16:00:53 2023, max compression
```

## Comparing `reasoner-pydantic-4.1.2.tar` & `reasoner-pydantic-4.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:23:14.831385 reasoner-pydantic-4.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-26 18:23:14.831385 reasoner-pydantic-4.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-26 18:23:11.000000 reasoner-pydantic-4.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:23:14.831385 reasoner-pydantic-4.1.2/reasoner_pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-26 18:23:11.000000 reasoner-pydantic-4.1.2/reasoner_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-26 18:23:11.000000 reasoner-pydantic-4.1.2/reasoner_pydantic/auxgraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-26 18:23:11.000000 reasoner-pydantic-4.1.2/reasoner_pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-07-26 18:23:11.000000 reasoner-pydantic-4.1.2/reasoner_pydantic/kgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-07-26 18:23:11.000000 reasoner-pydantic-4.1.2/reasoner_pydantic/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-26 18:23:11.000000 reasoner-pydantic-4.1.2/reasoner_pydantic/metakg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-26 18:23:11.000000 reasoner-pydantic-4.1.2/reasoner_pydantic/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-26 18:23:11.000000 reasoner-pydantic-4.1.2/reasoner_pydantic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-26 18:23:11.000000 reasoner-pydantic-4.1.2/reasoner_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-26 18:23:11.000000 reasoner-pydantic-4.1.2/reasoner_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-07-26 18:23:11.000000 reasoner-pydantic-4.1.2/reasoner_pydantic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:23:14.831385 reasoner-pydantic-4.1.2/reasoner_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-26 18:23:14.000000 reasoner-pydantic-4.1.2/reasoner_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-26 18:23:14.000000 reasoner-pydantic-4.1.2/reasoner_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:23:14.000000 reasoner-pydantic-4.1.2/reasoner_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:23:14.000000 reasoner-pydantic-4.1.2/reasoner_pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 18:23:14.000000 reasoner-pydantic-4.1.2/reasoner_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 18:23:14.000000 reasoner-pydantic-4.1.2/reasoner_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 18:23:14.831385 reasoner-pydantic-4.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-26 18:23:11.000000 reasoner-pydantic-4.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:00:53.056341 reasoner-pydantic-4.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-03 16:00:53.056341 reasoner-pydantic-4.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-08-03 16:00:49.000000 reasoner-pydantic-4.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:00:53.052341 reasoner-pydantic-4.1.3/reasoner_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-03 16:00:49.000000 reasoner-pydantic-4.1.3/reasoner_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-08-03 16:00:49.000000 reasoner-pydantic-4.1.3/reasoner_pydantic/auxgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-03 16:00:49.000000 reasoner-pydantic-4.1.3/reasoner_pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-08-03 16:00:49.000000 reasoner-pydantic-4.1.3/reasoner_pydantic/kgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-08-03 16:00:49.000000 reasoner-pydantic-4.1.3/reasoner_pydantic/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-03 16:00:49.000000 reasoner-pydantic-4.1.3/reasoner_pydantic/metakg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-03 16:00:49.000000 reasoner-pydantic-4.1.3/reasoner_pydantic/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-08-03 16:00:49.000000 reasoner-pydantic-4.1.3/reasoner_pydantic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-08-03 16:00:49.000000 reasoner-pydantic-4.1.3/reasoner_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-08-03 16:00:49.000000 reasoner-pydantic-4.1.3/reasoner_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-08-03 16:00:49.000000 reasoner-pydantic-4.1.3/reasoner_pydantic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:00:53.056341 reasoner-pydantic-4.1.3/reasoner_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-03 16:00:53.000000 reasoner-pydantic-4.1.3/reasoner_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-03 16:00:53.000000 reasoner-pydantic-4.1.3/reasoner_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:00:53.000000 reasoner-pydantic-4.1.3/reasoner_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:00:53.000000 reasoner-pydantic-4.1.3/reasoner_pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 16:00:53.000000 reasoner-pydantic-4.1.3/reasoner_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 16:00:53.000000 reasoner-pydantic-4.1.3/reasoner_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:00:53.056341 reasoner-pydantic-4.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-03 16:00:49.000000 reasoner-pydantic-4.1.3/setup.py
```

### Comparing `reasoner-pydantic-4.1.2/PKG-INFO` & `reasoner-pydantic-4.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.1.2
+Version: 4.1.3
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Abrar Mesbah
 Author-email: amesbah@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.1.2/README.md` & `reasoner-pydantic-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.2/reasoner_pydantic/__init__.py` & `reasoner-pydantic-4.1.3/reasoner_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.2/reasoner_pydantic/auxgraphs.py` & `reasoner-pydantic-4.1.3/reasoner_pydantic/auxgraphs.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.2/reasoner_pydantic/base_model.py` & `reasoner-pydantic-4.1.3/reasoner_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.2/reasoner_pydantic/kgraph.py` & `reasoner-pydantic-4.1.3/reasoner_pydantic/kgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.2/reasoner_pydantic/message.py` & `reasoner-pydantic-4.1.3/reasoner_pydantic/message.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.2/reasoner_pydantic/metakg.py` & `reasoner-pydantic-4.1.3/reasoner_pydantic/metakg.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.2/reasoner_pydantic/qgraph.py` & `reasoner-pydantic-4.1.3/reasoner_pydantic/qgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.2/reasoner_pydantic/results.py` & `reasoner-pydantic-4.1.3/reasoner_pydantic/results.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.2/reasoner_pydantic/shared.py` & `reasoner-pydantic-4.1.3/reasoner_pydantic/shared.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.2/reasoner_pydantic/utils.py` & `reasoner-pydantic-4.1.3/reasoner_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.2/reasoner_pydantic/workflow.py` & `reasoner-pydantic-4.1.3/reasoner_pydantic/workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,22 @@
     """Generate a static enum."""
     return Enum(value=s, names={s: s}, type=str)
 
 
 class RunnerAllowList(BaseModel):
     allowlist: Optional[HashableSequence[str]]
     timeout: Optional[float]
-    _nonzero_allowlist = validator("allowlist", allow_reuse=True)(nonzero_validator)
 
     class Config:
         extra = "forbid"
 
 
 class RunnerDenyList(BaseModel):
     denylist: Optional[HashableSequence[str]]
     timeout: Optional[float]
-    _nonzero_denylist = validator("denylist", allow_reuse=True)(nonzero_validator)
 
     class Config:
         extra = "forbid"
 
 
 class RunnerTimeout(BaseModel):
     timeout: Optional[float]
@@ -110,24 +108,22 @@
     class Config:
         extra = "forbid"
 
 
 class FillAllowParameters(BaseModel):
     allowlist: Optional[HashableSequence[str]]
     qedge_keys: Optional[HashableSequence[str]]
-    _nonzero_allowlist = validator("allowlist", allow_reuse=True)(nonzero_validator)
 
     class Config:
         extra = "forbid"
 
 
 class FillDenyParameters(BaseModel):
     denylist: Optional[HashableSequence[str]]
     qedge_keys: Optional[HashableSequence[str]]
-    _nonzero_denylist = validator("denylist", allow_reuse=True)(nonzero_validator)
 
     class Config:
         extra = "forbid"
 
 
 class FillParameters(BaseModel):
     __root__: Union[FillAllowParameters, FillDenyParameters]
```

### Comparing `reasoner-pydantic-4.1.2/reasoner_pydantic.egg-info/PKG-INFO` & `reasoner-pydantic-4.1.3/reasoner_pydantic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.1.2
+Version: 4.1.3
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Abrar Mesbah
 Author-email: amesbah@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.1.2/reasoner_pydantic.egg-info/SOURCES.txt` & `reasoner-pydantic-4.1.3/reasoner_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.1.2/setup.py` & `reasoner-pydantic-4.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="reasoner-pydantic",
-    version="4.1.2",
+    version="4.1.3",
     author="Abrar Mesbah",
     author_email="amesbah@covar.com",
     url="https://github.com/TranslatorSRI/reasoner-pydantic",
     description="Pydantic models for the Reasoner API data formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["reasoner_pydantic"],
```

