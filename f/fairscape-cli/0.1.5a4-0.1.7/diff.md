# Comparing `tmp/fairscape_cli-0.1.5a4.tar.gz` & `tmp/fairscape_cli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairscape_cli-0.1.5a4.tar", max compression
+gzip compressed data, was "fairscape_cli-0.1.7.tar", max compression
```

## Comparing `fairscape_cli-0.1.5a4.tar` & `fairscape_cli-0.1.7.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1066 2023-01-06 17:27:00.899279 fairscape_cli-0.1.5a4/LICENSE
--rw-r--r--   0        0        0     4058 2023-08-03 18:11:08.295777 fairscape_cli-0.1.5a4/README.md
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a4/fairscape_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a4/fairscape_cli/apps/__init__.py
--rw-r--r--   0        0        0      274 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a4/fairscape_cli/apps/cache.py
--rw-r--r--   0        0        0      510 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a4/fairscape_cli/apps/describe.py
--rw-r--r--   0        0        0      764 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a4/fairscape_cli/apps/fairscape.py
--rw-r--r--   0        0        0       89 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a4/fairscape_cli/apps/list.py
--rw-r--r--   0        0        0      173 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a4/fairscape_cli/apps/models/__init__.py
--rw-r--r--   0        0        0      340 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a4/fairscape_cli/apps/models/computation.py
--rw-r--r--   0        0        0     2559 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a4/fairscape_cli/apps/models/dataset.py
--rw-r--r--   0        0        0     1890 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a4/fairscape_cli/apps/models/software.py
--rw-r--r--   0        0        0     8135 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a4/fairscape_cli/apps/objects.py
--rw-r--r--   0        0        0     3369 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a4/fairscape_cli/apps/rocrate.py
--rw-r--r--   0        0        0     2276 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a4/fairscape_cli/apps/utils.py
--rw-r--r--   0        0        0     2677 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a4/fairscape_cli/apps/validator.py
--rw-r--r--   0        0        0      397 2023-05-30 16:31:53.800262 fairscape_cli-0.1.5a4/fairscape_cli/main.py
--rw-r--r--   0        0        0      339 2023-08-03 18:11:08.295777 fairscape_cli-0.1.5a4/fairscape_cli/models/__init__.py
--rw-r--r--   0        0        0     1395 2023-08-03 18:11:08.295777 fairscape_cli-0.1.5a4/fairscape_cli/models/base.py
--rw-r--r--   0        0        0      707 2023-08-03 18:11:08.295777 fairscape_cli-0.1.5a4/fairscape_cli/models/computation.py
--rw-r--r--   0        0        0     1340 2023-08-03 18:11:08.295777 fairscape_cli-0.1.5a4/fairscape_cli/models/dataset.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a4/fairscape_cli/models/models.py
--rw-r--r--   0        0        0     7869 2023-08-03 18:11:08.295777 fairscape_cli-0.1.5a4/fairscape_cli/models/rocrate.py
--rw-r--r--   0        0        0    13054 2023-08-02 16:41:43.014515 fairscape_cli-0.1.5a4/fairscape_cli/models/schema.py
--rw-r--r--   0        0        0      758 2023-08-03 18:11:08.295777 fairscape_cli-0.1.5a4/fairscape_cli/models/software.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a4/fairscape_cli/rocrate/__init__.py
--rw-r--r--   0        0        0    20849 2023-08-03 18:11:08.295777 fairscape_cli-0.1.5a4/fairscape_cli/rocrate/rocrate.py
--rw-r--r--   0        0        0     1326 2023-05-30 16:31:53.800262 fairscape_cli-0.1.5a4/fairscape_cli/rocrate/utils.py
--rw-r--r--   0        0        0        0 2023-05-30 16:31:53.800262 fairscape_cli-0.1.5a4/fairscape_cli/schema/__init__.py
--rw-r--r--   0        0        0      338 2023-05-30 16:31:53.800262 fairscape_cli-0.1.5a4/fairscape_cli/schema/schema.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a4/fairscape_cli/validate/__init__.py
--rw-r--r--   0        0        0     1365 2023-08-03 18:11:08.295777 fairscape_cli-0.1.5a4/fairscape_cli/validate/validate_json.py
--rw-r--r--   0        0        0     1533 2023-08-03 18:15:02.105731 fairscape_cli-0.1.5a4/pyproject.toml
--rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 fairscape_cli-0.1.5a4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-01-06 17:27:00.899279 fairscape_cli-0.1.7/LICENSE
+-rw-r--r--   0        0        0      201 2023-08-01 17:14:09.131383 fairscape_cli-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.7/fairscape_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.7/fairscape_cli/apps/__init__.py
+-rw-r--r--   0        0        0      274 2023-03-27 17:08:49.098247 fairscape_cli-0.1.7/fairscape_cli/apps/cache.py
+-rw-r--r--   0        0        0      510 2023-03-27 17:08:49.098247 fairscape_cli-0.1.7/fairscape_cli/apps/describe.py
+-rw-r--r--   0        0        0      764 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7/fairscape_cli/apps/fairscape.py
+-rw-r--r--   0        0        0       89 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7/fairscape_cli/apps/list.py
+-rw-r--r--   0        0        0      173 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7/fairscape_cli/apps/models/__init__.py
+-rw-r--r--   0        0        0      340 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7/fairscape_cli/apps/models/computation.py
+-rw-r--r--   0        0        0     2559 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7/fairscape_cli/apps/models/dataset.py
+-rw-r--r--   0        0        0     1890 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7/fairscape_cli/apps/models/software.py
+-rw-r--r--   0        0        0     8135 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7/fairscape_cli/apps/objects.py
+-rw-r--r--   0        0        0     3369 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7/fairscape_cli/apps/rocrate.py
+-rw-r--r--   0        0        0     2276 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7/fairscape_cli/apps/utils.py
+-rw-r--r--   0        0        0     2677 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7/fairscape_cli/apps/validator.py
+-rw-r--r--   0        0        0      397 2023-05-30 16:31:53.800262 fairscape_cli-0.1.7/fairscape_cli/main.py
+-rw-r--r--   0        0        0      397 2023-08-02 16:41:48.664514 fairscape_cli-0.1.7/fairscape_cli/models/__init__.py
+-rw-r--r--   0        0        0     8833 2023-08-02 16:41:47.624514 fairscape_cli-0.1.7/fairscape_cli/models/bagit.py
+-rw-r--r--   0        0        0     1022 2023-08-02 18:23:15.733983 fairscape_cli-0.1.7/fairscape_cli/models/base.py
+-rw-r--r--   0        0        0      761 2023-08-02 18:35:08.013921 fairscape_cli-0.1.7/fairscape_cli/models/computation.py
+-rw-r--r--   0        0        0     1371 2023-08-02 18:57:29.183804 fairscape_cli-0.1.7/fairscape_cli/models/dataset.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7/fairscape_cli/models/models.py
+-rw-r--r--   0        0        0     8472 2023-08-02 16:34:25.854552 fairscape_cli-0.1.7/fairscape_cli/models/rocrate.py
+-rw-r--r--   0        0        0    13054 2023-08-02 16:41:43.014515 fairscape_cli-0.1.7/fairscape_cli/models/schema.py
+-rw-r--r--   0        0        0      710 2023-08-02 16:34:25.854552 fairscape_cli-0.1.7/fairscape_cli/models/software.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7/fairscape_cli/rocrate/__init__.py
+-rw-r--r--   0        0        0    25851 2023-08-02 16:34:25.854552 fairscape_cli-0.1.7/fairscape_cli/rocrate/rocrate.py
+-rw-r--r--   0        0        0     1326 2023-05-30 16:31:53.800262 fairscape_cli-0.1.7/fairscape_cli/rocrate/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 16:31:53.800262 fairscape_cli-0.1.7/fairscape_cli/schema/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-30 16:31:53.800262 fairscape_cli-0.1.7/fairscape_cli/schema/schema.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7/fairscape_cli/validate/__init__.py
+-rw-r--r--   0        0        0     1422 2023-08-02 18:19:09.424004 fairscape_cli-0.1.7/fairscape_cli/validate/validate_json.py
+-rw-r--r--   0        0        0     1539 2023-08-03 13:23:21.749160 fairscape_cli-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1062 1970-01-01 00:00:00.000000 fairscape_cli-0.1.7/PKG-INFO
```

### Comparing `fairscape_cli-0.1.5a4/LICENSE` & `fairscape_cli-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/apps/fairscape.py` & `fairscape_cli-0.1.7/fairscape_cli/apps/fairscape.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/apps/models/dataset.py` & `fairscape_cli-0.1.7/fairscape_cli/apps/models/dataset.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/apps/models/software.py` & `fairscape_cli-0.1.7/fairscape_cli/apps/models/software.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/apps/objects.py` & `fairscape_cli-0.1.7/fairscape_cli/apps/objects.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/apps/rocrate.py` & `fairscape_cli-0.1.7/fairscape_cli/apps/rocrate.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/apps/utils.py` & `fairscape_cli-0.1.7/fairscape_cli/apps/utils.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/apps/validator.py` & `fairscape_cli-0.1.7/fairscape_cli/apps/validator.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/models/computation.py` & `fairscape_cli-0.1.7/fairscape_cli/models/computation.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from typing import (
     Optional,
     List,
     Union,
     Dict,
 )
 from pydantic import (
-    constr,
+    Field,
     AnyUrl
 )
 import re
+from datetime import datetime
 
 
 class Computation(FairscapeBaseModel):
-    metadataType: Optional[str] = "https://w3id.org/EVI#Computation"
+    metadataType: str = Field(default="https://w3id.org/EVI#Computation")
     runBy: str
-    dateCreated: str
-    description: constr(min_length=10, max_length=2056)
-    associatedPublication: Optional[Union[str, AnyUrl]]
-    additionalDocumentation: Optional[Union[str, AnyUrl]]
+    dateCreated: str 
+    description: str = Field(min_length=10, max_length=2056)
+    associatedPublication: Optional[str] = Field(default=None)
+    additionalDocumentation: Optional[str] = Field(default=None)
     command: Optional[Union[List[str], str]] 
     usedSoftware: Optional[List[str]]
     calledBy: Optional[str]
     usedDataset: Optional[Union[List[str], str]]
     generated: Optional[Union[str,List[str]]]
```

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/models/dataset.py` & `fairscape_cli-0.1.7/fairscape_cli/models/dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,47 +9,39 @@
     Union,
     Dict
 )
 
 from pydantic import (
     BaseModel,
     constr,
+    Field,
     AnyUrl
 )
+from datetime import datetime
 
 
 class Dataset(FairscapeBaseModel):
-    metadataType: Optional[str] = "https://w3id.org/EVI#Dataset"
-    author: constr(max_length=64)
-    datePublished: str
+    metadataType: Optional[str] = Field(default="https://w3id.org/EVI#Dataset")
+    author: str = Field(max_length=64)
+    datePublished: str = Field(...)
     version: str
-    description: constr(min_length=10)
-    associatedPublication: Optional[str]
-    additionalDocumentation: Optional[str]
-    fileFormat: str
-    dataSchema: Optional[Union[str, dict]]
+    description: str = Field(min_length=10)
+    keywords: List[str] = Field(...)
+    associatedPublication: Optional[str] = None
+    additionalDocumentation: Optional[str] = None
+    fileFormat: str = Field(alias="format")
+    dataSchema: Optional[Union[str, dict]] = Field(alias="schema")
     generatedBy: Optional[List[Union[str, Identifier]]]
     derivedFrom: Optional[List[Union[str, Identifier]]]
     usedBy: Optional[List[Union[str, Identifier]]]
-    contentUrl: Optional[str]
-
-    class Config:
-        fields={
-            "fileFormat": {
-                "title": "fileFormat",
-                "alias": "format"
-            },
-            "dataSchema": {
-                "title": "dataSchema",
-                "alias": "schema"
-            }
-        }
+    contentUrl: Optional[str] = None
 
 
 class DatasetContainer(FairscapeBaseModel): 
-    guid: str
-    metadataType: Optional[str] = "https://w3id.org/EVI#Dataset"
+    guid: str = Field(alias="@id")
+    metadataType: Optional[str] = Field(default="https://w3id.org/EVI#Dataset", alias="@type")
     name: str
-    description: constr(min_length=10)
-    hasPart: Optional[List[Union[str, Identifier]]] = []
-    isPartOf: Optional[List[Union[str, Identifier]]] = []
+    description: str = Field(min_length=10)
+    keywords: List[str] = Field(...)
+    hasPart: Optional[List[Union[str, Identifier]]] = Field(default=[])
+    isPartOf: Optional[List[Union[str, Identifier]]] = Field(default=[])
```

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/models/rocrate.py` & `fairscape_cli-0.1.7/fairscape_cli/models/rocrate.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,44 @@
 from fairscape_cli.models import (
     Software,
     Dataset,
     Computation,
     DatasetContainer
 )
 from prettytable import PrettyTable
-from pydantic import BaseModel
+from pydantic import (
+    BaseModel,
+    computed_field,
+    Field,
+)
 from typing import (
     Optional,
     Union,
     List
 )
 
 
 class ROCrate(BaseModel):
-    guid: Optional[str] = ""
-    metadataType: str = "https://schema.org/Dataset"
-    name: Optional[str]
+    guid: Optional[str] = Field(default="")
+    metadataType: str = Field(default="https://schema.org/Dataset")
+    name: str = Field(min_length=10)
+    description: str = Field(min_length=10)
+    keywords: List[str] = Field(...)
     projectName: Optional[str]
     organizationName: Optional[str]
     path: pathlib.Path
     metadataGraph: Optional[List[Union[Dataset,Software, Computation]]]
 
+    # Computed Field implementation for guid generation
+    #@computed_field
+    #def guid(self) -> str:
+    #    organization_guid = f"ark:/{self.organizationName.replace(' ', '_')}"
+    #    project_guid = organization_guid + f"/{self.projectName.replace(' ', '_')}"
+    #    return project_guid + f"/{self.name.replace(' ', '_')}"
+
     def createCrateFolder(self):
         self.path.mkdir(exist_ok=False)
         
 
     def initCrate(self):
         """Create an rocrate at the current working directory, initilize the ro-crate-metadata.json
 
@@ -49,14 +62,16 @@
             "@id": self.guid,
             "@context": {
                 "EVI": "https://w3id.org/EVI#",
                 "@vocab": "https://schema.org/"
             },
             "@type": "Dataset",
             "name": self.name,
+            "description": self.description,
+            "keywords": self.keywords,
             "isPartOf": [
                 {
                     "@id": organization_guid,
                     "@type": "Organization",
                     "name": self.organizationName
                 },
                 {
@@ -112,21 +127,21 @@
     def registerObject(self, model: Union[Dataset, Software, Computation, DatasetContainer]):
         ''' Add a specified peice of metadata to the graph of an ROCrate
 
         Marshals a given model into JSON-LD, opens the ro-crate-metadata.json,
         appends the new metadata to the @graph, and overwrites the ro-crate-metadata.json
         '''
 
-        metadata_path = self.path
+        metadata_path = pathlib.Path(self.path)
 
         with metadata_path.open("r+") as rocrate_metadata_file:
             rocrate_metadata = json.load(rocrate_metadata_file)
             
             # add to the @graph
-            rocrate_metadata['@graph'].append(model.dict(by_alias=True))
+            rocrate_metadata['@graph'].append(model.model_dump(by_alias=True))
             rocrate_metadata_file.seek(0)
             json.dump(rocrate_metadata, rocrate_metadata_file, indent=2)
 
 
     def registerDataset(self, Dataset):
         self.registerObject(model=Dataset)
```

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/models/schema.py` & `fairscape_cli-0.1.7/fairscape_cli/models/schema.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/models/software.py` & `fairscape_cli-0.1.7/fairscape_cli/models/software.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 from fairscape_cli.models.base import FairscapeBaseModel
 from pydantic import (
-    constr,
-    AnyUrl
+    Field,
+    AnyUrl,
+    ConfigDict
 )
 from datetime import datetime
 from typing import (
     Optional,
     Union,
     Dict,
     List 
 )
 
 
 class Software(FairscapeBaseModel): 
     metadataType: str = "https://w3id.org/EVI#Software"
-    author: constr(max_length=64)
+    author: str = Field(min_length=4, max_length=64)
     dateModified: str
     version: str
-    description: constr(min_length=10)
+    description: str =  Field(min_length=10)
+    keywords: List[str] = Field(...)
     associatedPublication: Optional[str]
     additionalDocumentation: Optional[str]
-    fileFormat: str
+    fileFormat: str = Field(title="fileFormat", alias="format")
     usedByComputation: Optional[List[str]]
     contentUrl: Optional[str]
-
-    class Config:
-       fields={
-        "fileFormat":
-            {
-                "title": "fileFormat",
-                "alias": "format"
-            }
-        }
```

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/rocrate/rocrate.py` & `fairscape_cli-0.1.7/fairscape_cli/rocrate/rocrate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import click
 import pathlib
 import shutil
 import json
 from pydantic import ValidationError
+from datetime import datetime
 
 from fairscape_cli.models import (
     Dataset,
     Software,
     Computation,
     DatasetContainer,
-    ROCrate
+    ROCrate,
+    BagIt
 )
 
 from fairscape_cli.rocrate.utils import (
     generate_id,
     inside_crate 
 )
 
@@ -39,31 +41,38 @@
 def validate():
     pass
 
 @rocrate.command('zip')
 def zip():
     pass
 
+
 @rocrate.command('init')
 @click.option('--guid', required=False, type=str, default="", show_default=False)
 @click.option('--name', required=True, type=str, prompt = "ROCrate Name (e.g. B2AI_ROCRATE)")
 @click.option('--organization-name', required=True, type=str, prompt = "Organization Name")
 @click.option('--project-name', required=True, type=str, prompt = "Project Name")
+@click.option('--description', required=True, type=str)
+@click.option('--keywords', required=True, multiple=True, type=str)
 def init(
-    guid: str,
-    name: str,
-    organization_name: str,
-    project_name: str
+    guid,
+    name,
+    organization_name,
+    project_name,
+    description,
+    keywords
 ):
 
     passed_crate =ROCrate(
         guid=guid,
         name=name,
         organizationName = organization_name,
         projectName = project_name,
+        description = description,
+        keywords = keywords,
         path = pathlib.Path.cwd(), 
         metadataGraph = []
     )
 
     try:
         passed_crate.initCrate()
     except Exception as e:
@@ -71,39 +80,45 @@
     
 
 @rocrate.command('create')
 @click.option('--guid', required=False, type=str, default="", show_default=False)
 @click.option('--name', required=True, type=str, prompt = "ROCrate Name (e.g. B2AI_ROCRATE)")
 @click.option('--organization-name', required=True, type=str, prompt = "Organization Name")
 @click.option('--project-name', required=True, type=str, prompt = "Project Name")
-@click.argument('crate-path', type=click.Path(exists=False, path_type=pathlib.Path))
+@click.option('--description', required=True, type=str)
+@click.option('--keywords', required=True, multiple=True, type=str)
+@click.argument('rocrate-path', type=click.Path(exists=False, path_type=pathlib.Path))
 def create(
-    guid: str,
-    name: str,
-    organization_name: str,
-    project_name: str,
-    crate_path: pathlib.Path, 
+    guid,
+    name,
+    organization_name,
+    project_name,
+    description,
+    keywords,
+    rocrate_path, 
 ): 
-    '''Create an ROCrate in a new path specified by the crate-path argument
+    '''Create an ROCrate in a new path specified by the rocrate-path argument
     '''
     
-    organization_guid = f"ark:/{organization_name.replace(' ', '_')}"
+    organization_guid = f"ark:5982/{organization_name.replace(' ', '_')}"
     project_guid = organization_guid + f"/{project_name.replace(' ', '_')}"
 
     if guid != "":
         crate_guid = guid
     else:
         crate_guid = project_guid + f"/{name.replace(' ', '_')}"
 
     passed_crate = ROCrate(
         guid=crate_guid,
         name=name,
         organizationName = organization_name,
         projectName = project_name,
-        path = crate_path, 
+        description = description,
+        keywords = keywords,
+        path = rocrate_path, 
         metadataGraph = []
     )
     
     passed_crate.createCrateFolder()
     passed_crate.initCrate()
 
     click.echo(crate_guid)
@@ -129,111 +144,116 @@
 @register.command('software')
 @click.argument('rocrate-path', type=click.Path(exists=True, path_type=pathlib.Path))
 @click.option('--guid', required=False, type=str, default="", show_default=False)
 @click.option('--name',    required=True, prompt = "Software Name")
 @click.option('--author',  required=True, prompt = "Author Name")
 @click.option('--version', required=True, prompt = "Software Version")
 @click.option('--description', required = True, prompt = "Software Description")
+@click.option('--keywords', required=True, multiple=True)
 @click.option('--file-format', required = True, prompt = "File Format of Software")
 @click.option('--url',     required = False)
 @click.option('--date-modified', required=False)
 @click.option('--filepath', required=False)
 @click.option('--used-by-computation', required=False, multiple=True)
 @click.option('--associated-publication', required=False)
 @click.option('--additional-documentation', required=False)
 def registerSoftware(
     rocrate_path: pathlib.Path,
-    guid: str,
-    name: str,
-    author: str,
-    version: str,
-    description: str, 
-    file_format: str,
-    url: str,
-    date_modified: str,
-    filepath: str,
-    used_by_computation: Optional[List[str]],
-    associated_publication: Optional[str],
-    additional_documentation: Optional[str]
+    guid,
+    name,
+    author,
+    version,
+    description, 
+    keywords,
+    file_format,
+    url,
+    date_modified,
+    filepath,
+    used_by_computation,
+    associated_publication,
+    additional_documentation
     ):
     
     metadata_path = rocrate_path / "ro-crate-metadata.json"
 
     # check if you are in the rocrate path
     # ro-crate-metadata.json should be a local file
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
-    crate = ROCrate(path=metadata_path)
+    crate = ROCrate.model_construct(
+        _fields_set={"path"}, 
+        **{"path":"metadata_path"}
+    ) 
 
 
     software_metadata = {
             "@id": guid,
             "@type": "https://w3id.org/EVI#Software",
             "url": url,
             "name": name,
             "author": author,
             "dateModified": date_modified,
             "description": description,
+            "keywords": keywords,
             "version": version,
             "associatedPublication": associated_publication,
             "additionalDocumentation": additional_documentation,
             "format": file_format,
             # sanitize new line characters for multiple inputs
             "usedByComputation": [
                 computation.strip("\n") for computation in used_by_computation
             ],
         }
 
     if filepath != "" and filepath is not None:
-            software_metadata["contentUrl"] = f"file://{str(filepath)}" 
-    else:
-        # if filepath is null and url is null
-        # raise an error
-        if url == "" or url is None:
-            click.echo("Software Validation Error: url and filepath cannot both be null")
-            click.Abort()
+            # TODO if URL just set
+            software_metadata["contentUrl"] = filepath 
+
+            # TODO if pathlike object
 
     try:
         software_model = Software(**software_metadata)
+        crate.registerSoftware(software_model)
 
     except ValidationError as e:
         click.echo("Software Validation Error")
         click.echo(e)
         click.Abort()
         
-    crate.registerSoftware(software_model)
  
     click.echo(guid)
 
 
 
 @register.command('dataset')
 @click.argument('rocrate-path', type=click.Path(exists=True, path_type=pathlib.Path))
 @click.option('--guid', required=False, default="", type=str)
 @click.option('--name', required=True, prompt="Dataset Name")
 @click.option('--url', required=False)
 @click.option('--author', required=True, prompt="Dataset Author")
 @click.option('--version', required=True, prompt="Dataset Version")
 @click.option('--date-published', required=True, prompt="Date Published")
 @click.option('--description', required=True, prompt="Dataset Description")
+@click.option('--keywords', required=True, multiple=True)
 @click.option('--data-format', required=True, prompt="Data Format i.e. (csv, tsv)")
 @click.option('--filepath', required=True)
 @click.option('--used-by', required=False, multiple=True)
 @click.option('--derived-from', required=False, multiple=True)
 @click.option('--associated-publication', required=False)
 @click.option('--additional-documentation', required=False)
 def registerDataset(
     rocrate_path: pathlib.Path,
     guid: str,
     name: str,
     url: str,
     author: str,
     description: str,
+    keywords: List[str],
     date_published: str,
     version: str,
     associated_publication: Optional[str],
     additional_documentation: Optional[List[str]],
     data_format: str,
     filepath: str,
     derived_from: Optional[List[str]],
@@ -244,23 +264,27 @@
 
     # check if you are in the rocrate path
     # ro-crate-metadata.json should be a local file
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
-    crate = ROCrate(path=metadata_path)
+    crate = ROCrate.model_construct(
+        _fields_set={"path"}, 
+        **{"path":"metadata_path"}
+    ) 
 
     dataset_metadata = {
             "@id": guid,
             "@type": "https://w3id.org/EVI#Dataset",
             "url": url,
             "author": author,
             "name": name,
             "description": description,
+            "keywords": keywords,
             "datePublished": date_published,
             "version": version,
             "associatedPublication": associated_publication,
             "additionalDocumentation": additional_documentation,
             "format": data_format,
 
             # sanitize input lists of newline breaks
@@ -274,137 +298,152 @@
 
     if filepath != "" and filepath is not None:
         dataset_metadata["contentUrl"] = f"file://{str(filepath)}" 
 
 
     try:
         dataset_model = Dataset(**dataset_metadata)
+        crate.registerDataset(dataset_model)
 
     except ValidationError as e:
         click.echo("Dataset Validation Error")
         click.echo(e)
         click.Abort()
     
-    crate.registerDataset(dataset_model)
  
     click.echo(guid)
 
 
 @register.command('computation')
 @click.argument('rocrate-path', type=click.Path(exists=True, path_type=pathlib.Path))
 @click.option('--guid', required=False, default="", type=str, show_default=False)
 @click.option('--name', required=True, prompt="Computation Name")
 @click.option('--run-by', required=True, prompt="Computation Run By")
-@click.option('--command', required=False, prompt="Command")
+@click.option('--command', required=False, prompt="Enter the command", prompt_required=False)
 @click.option('--date-created', required=True, prompt="Date Created")
 @click.option('--description', required=True, prompt="Computation Description")
+@click.option('--keywords', required=True, multiple=True)
 @click.option('--used-software', required=False, multiple=True)
 @click.option('--used-dataset', required=False, multiple=True)
 @click.option('--generated', required=False, multiple=True)
 def computation(
     rocrate_path: pathlib.Path,
     guid: str,
     name: str,
     run_by: str,
     command: Optional[Union[str, List[str]]],
     date_created: str,
     description: str,
+    keywords: List[str],
     used_software,
     used_dataset,
     generated
 ):
 
     
     # check if you are in the rocrate path
     # ro-crate-metadata.json should be a local file
     metadata_path = rocrate_path / "ro-crate-metadata.json"
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
-    crate = ROCrate(path=metadata_path)
+    crate = ROCrate.model_construct(
+        _fields_set={"path"}, 
+        **{"path":"metadata_path"}
+    ) 
 
     if guid == "":
         guid = generate_id(metadata_path, name, "Computation")
 
     # initilize the model with the required properties
     try:
 
         computation_model = Computation(   
             **{
             "@id": guid,
             "@type": "https://w3id.org/EVI#Computation",
             "name": name,
+            "description": description,
+            "keywords": keywords,
             "runBy": run_by,
+            "command": command,
             "dateCreated": date_created,
             "description": description,
             # sanitize input lists of newline breaks
             "usedSoftware": [
                 software.strip("\n") for software in used_software
             ],
             "usedDataset": [
                 dataset.strip("\n") for dataset in used_dataset 
             ],
             "generated": [
                 output.strip("\n") for output in generated
             ],
             }
         )
+        crate.registerComputation(computation_model)
+
     except ValidationError as e:
         click.echo("Computation Validation Error")
         click.echo(e)
         click.Abort()
 
-    crate.registerComputation(computation_model)
     
     click.echo(guid)
         #click.echo("Added Computation")
         #click.echo(
         #    json.dumps(computation_model.dict(by_alias=True), indent=2)
         #)
 
 
 
 @register.command('dataset-container')
 @click.argument('rocrate-path', type=click.Path(exists=True, path_type=pathlib.Path))
 @click.option('--guid', required=False, default="", type=str, show_default=False)
 @click.option('--name', required=True, prompt="DatasetContainer Name")
 @click.option('--description', required=True)
+@click.option('--keywords', required=True, multiple=True)
 @click.option('--has-part', required=False, multiple=True)
 @click.option('--is-part-of', required=False, multiple=True)
 def registerDatasetContainer(
     rocrate_path, 
     guid, 
     name, 
     description, 
+    keywords,
     has_part, 
     is_part_of
 ):
     '''Add a DatasetContainer to the ROCrate.
 
     A Dataset Container is used for grouping sets of datasets. Only Datasets may be added to the dataset container hasPart property.
     '''
    
     # check that crate exists 
     metadata_path = rocrate_path / "ro-crate-metadata.json"
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
-    crate = ROCrate(path=metadata_path)
+    crate = ROCrate.model_construct(
+        _fields_set={"path"}, 
+        **{"path":"metadata_path"}
+    ) 
 
     if guid == "":
         guid = generate_id(metadata_path, name, "Dataset")
 
     # validate the provided metadata
     try: 
         dscontainer = DatasetContainer(**{
             "guid": guid,
             "name": name,
             "description": description,
+            "keywords": keywords,
             "hasPart": has_part,
             "isPartOf": is_part_of
         })
 
         crate.registerObject(dscontainer) 
         click.echo(guid)
 
@@ -433,15 +472,18 @@
     """
     # check that crate exists 
     metadata_path = rocrate_path / "ro-crate-metadata.json"
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
-    crate = ROCrate(path=metadata_path)
+    crate = ROCrate.model_construct(
+        _fields_set={"path"}, 
+        **{"path":"metadata_path"}
+    ) 
 
     # TODO check that dataset container is guid
 
     # TODO check that dataset guid is guid
 
     try:
         crate.popDatasetContainer(dataset_container, dataset_guid)
@@ -461,15 +503,18 @@
 
     # check that crate exists 
     metadata_path = rocrate_path / "ro-crate-metadata.json"
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
-    crate = ROCrate(path=metadata_path)
+    crate = ROCrate.model_construct(
+        _fields_set={"path"}, 
+        **{"path":"metadata_path"}
+    ) 
 
     # TODO check that dataset container is guid
 
     # TODO check that dataset guid is guid
 
     try:
         crate.pushDatasetContainer(dataset_container, dataset_guid)
@@ -490,89 +535,93 @@
 @add.command('software')
 @click.argument('rocrate-path', type=click.Path(exists=True, path_type=pathlib.Path))
 @click.option('--guid', required=False, type=str, default="", show_default=False)
 @click.option('--name',    required=True, prompt = "Software Name")
 @click.option('--author',  required=True, prompt = "Author Name")
 @click.option('--version', required=True, prompt = "Software Version")
 @click.option('--description', required = True, prompt = "Software Description")
+@click.option('--keywords', required=True, multiple=True)
 @click.option('--file-format', required = True, prompt = "File Format of Software")
 @click.option('--url',     required = False)
 @click.option('--source-filepath', required=True)
 @click.option('--destination-filepath', required=True)
-@click.option('--date-modified', required=False)
+@click.option('--date-modified', required=True)
 @click.option('--used-by-computation', required=False, multiple=True)
 @click.option('--associated-publication', required=False)
 @click.option('--additional-documentation', required=False)
 def software(
-    rocrate_path: pathlib.Path,
-    guid: str,
-    name: str,
-    author: str,
-    version: str,
-    description: str, 
-    file_format: str,
-    url: str,
-    source_filepath: str,
-    destination_filepath: str,
-    date_modified: str,
-    used_by_computation: Optional[List[str]],
-    associated_publication: Optional[str],
-    additional_documentation: Optional[str]
+    rocrate_path,
+    guid,
+    name,
+    author,
+    version,
+    description, 
+    keywords,
+    file_format,
+    url,
+    source_filepath,
+    destination_filepath,
+    date_modified,
+    used_by_computation,
+    associated_publication,
+    additional_documentation
 ):
-
-    source_path = pathlib.Path(source_filepath)
-    destination_path = pathlib.Path(destination_filepath)
-    
+ 
     metadata_path = rocrate_path / "ro-crate-metadata.json"
 
     # check if you are in the rocrate path
     # ro-crate-metadata.json should be a local file
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
     if guid == "":
         guid = generate_id(metadata_path, name, "Software")
 
     
-    crate = ROCrate(path=metadata_path)
+    crate = ROCrate.model_construct(
+        _fields_set={"path"}, 
+        **{"path": metadata_path}
+    ) 
 
 
     try:
         software_model = Software(   
             **{
             "@id": guid,
             "@type": "https://w3id.org/EVI#Software",
             "url": url,
             "name": name,
             "author": author,
             "dateModified": date_modified,
             "description": description,
+            "keywords": keywords,
             "version": version,
             "associatedPublication": associated_publication,
             "additionalDocumentation": additional_documentation,
             "format": file_format,
             # sanitize multiple inputs
             "usedByComputation": [
                 computation.strip("\n") for computation in used_by_computation
             ],
-            "contentUrl": "file://" + str(destination_path)
+            "contentUrl": "file://" + str(pathlib.Path(destination_filepath))
             }
         )
+        crate.registerSoftware(software_model)
 
     except ValidationError as e:
         click.echo("Software Validation Error")
         click.echo(e)
         click.Abort()
 
-    crate.registerSoftware(software_model)
 
     try:
         crate.copyObject(source_filepath, destination_filepath)
-    except:
+
+    except Exception as e:
         click.echo("Failed to Copy Software")
         click.echo(e)
         click.Abort()
 
     click.echo(guid)
 
     # TODO add to cache
@@ -583,28 +632,30 @@
 @click.option('--guid', required=False, default="", type=str)
 @click.option('--name', required=True, prompt="Dataset Name")
 @click.option('--url', required=False)
 @click.option('--author', required=True, prompt="Dataset Author")
 @click.option('--version', required=True, prompt="Dataset Version")
 @click.option('--date-published', required=True, prompt="Date Published")
 @click.option('--description', required=True, prompt="Dataset Description")
+@click.option('--keywords', required=True, multiple=True)
 @click.option('--data-format', required=True, prompt="Data Format i.e. (csv, tsv)")
-@click.option('--source-filepath', required=False)
-@click.option('--destination-filepath', required=False)
+@click.option('--source-filepath', required=True)
+@click.option('--destination-filepath', required=True)
 @click.option('--used-by', required=False, multiple=True)
 @click.option('--derived-from', required=False, multiple=True)
 @click.option('--associated-publication', required=False)
 @click.option('--additional-documentation', required=False)
 def dataset(
     rocrate_path: pathlib.Path,
     guid: str,
     name: str,
     url: str,
     author: str,
     description: str,
+    keywords: List[str],
     date_published: str,
     version: str,
     associated_publication: Optional[str],
     additional_documentation: Optional[List[str]],
     data_format: str,
     source_filepath: str,
     destination_filepath: str,
@@ -624,25 +675,29 @@
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
     if guid == "":
         guid = generate_id(metadata_path, name, "Dataset")
 
 
-    crate = ROCrate(path=metadata_path)
+    crate = ROCrate.model_construct(
+        _fields_set={"path"}, 
+        **{"path":"metadata_path"}
+    ) 
     
     try:
         dataset_model = Dataset(   
             **{
             "@id": guid,
             "@type": "https://w3id.org/EVI#Dataset",
             "url": url,
             "author": author,
             "name": name,
             "description": description,
+            "keywords": keywords,
             "datePublished": date_published,
             "version": version,
             "associatedPublication": associated_publication,
             "additionalDocumentation": additional_documentation,
             "format": data_format,
             "derivedFrom": [
                 derived.strip("\n") for derived in derived_from
@@ -650,23 +705,116 @@
             "usedBy": [
                 used.strip("\n") for used in used_by 
             ],
             "contentUrl": "file://" + str(destination_path)
             }
         )
 
+        crate.registerDataset(dataset_model)
+        crate.copyObject(source_filepath, destination_filepath)
+
     except ValidationError as e:
         click.echo("Software Validation Error")
         click.echo(e)
         click.Abort()
 
-    crate.registerDataset(dataset_model)
-    crate.copyObject(source_filepath, destination_filepath)
 
     click.echo(guid) 
 
     # TODO add to cache
     
 
 
 
+@rocrate.group('package')
+def package():
+    pass
+
+@package.command('bagit')
+@click.argument('rocrate-path', type=click.Path(exists=True, path_type=pathlib.Path))
+@click.argument('bagit-path', type=click.Path(exists=False, path_type=pathlib.Path))
+@click.option('--Source-Organization', required=True, prompt="Source-Organization")
+@click.option('--Organization-Address', required=True, prompt="Organization-Address")
+@click.option('--Contact-Name', required=True, prompt="Contact-Name")
+@click.option('--Contact-Phone', required=True, prompt="Contact-Phone")
+@click.option('--Contact-Email', required=True, prompt="Contact-Email")
+@click.option('--External-Description', required=True, prompt="External-Description")
+#@click.option('--Bagging-Date', required=False)
+#@click.option('--External-Identifier', required=False, prompt="External-Identifier")
+#@click.option('--Payload-Oxum', required=False, prompt="Payload-Oxum")
+#@click.option('--Bag-Group-Identifier', required=False, prompt="Bag-Group-Identifier")
+#@click.option('--Bag-Count', required=False, prompt="Bag-Count")
+#@click.option('--Internal-Sender-Identifier', required=False, prompt="Internal-Sender-Identifier")
+#@click.option('--Internal-Sender-Description', required=False, prompt="Internal-Sender-Description")
+def bagit(
+    rocrate_path: pathlib.Path,
+    bagit_path: pathlib.Path,
+    source_organization: str,
+    organization_address: str,
+    contact_name: str,
+    contact_phone: str,
+    contact_email: str,
+    external_description: str
+):
+    bagit = BagIt(
+        **{    
+            "rocrate_path": rocrate_path,
+            "bagit_path": bagit_path,
+            "source_organization": source_organization,
+            "organization_address": organization_address,
+            "contact_name": contact_name,
+            "contact_phone": contact_phone,
+            "contact_email": contact_email,
+            "external_description": external_description,
+            "bagging_date": datetime.now().strftime("%m/%d/%Y")
+        }
+    )
+    
+    
+    
+    click.echo(click.style("BagIt path", fg="green") + f": {bagit_path}")
+
+    bagit.create_bagit_directory()
+    
+    # Create bag.txt
+    bagit.create_bagit_declaration()
+    click.echo(click.style("Bag Declaration", fg="green") + f": {bagit_path}/bag.txt")
+    
+    # Populate /data/ directory 
+    bagit.create_payload_directory()
+    click.echo(click.style("Payload Directory", fg="green") + f": {bagit_path}/data/")
+
+
+    # Create bag-info.txt
+    bagit.create_bagit_metadata()
+    click.echo(click.style("Bag Metadata", fg="green") + f": {bagit_path}/bag-info.txt")
+    
+    # Create manifest-sha256.txt
+    bagit.create_payload_manifest_sha256()
+    click.echo(click.style("Payload Manifest", fg="green") + f": {bagit_path}/manifest-sha256.txt")
+    # Create tagmanifest-sha256.txt
+    bagit.create_tag_manifest_sha256()
+    click.echo(click.style("Tag Manifest", fg="green") + f": {bagit_path}/tagmanifest-sha256.txt")
+    
+    # Create manifest-sha512.txt
+    bagit.create_payload_manifest_sha512()
+    click.echo(click.style("Payload Manifest", fg="green") + f": {bagit_path}/manifest-sha512.txt")
+    # Create tagmanifest-sha512.txt
+    bagit.create_tag_manifest_sha512()
+    click.echo(click.style("Tag Manifest", fg="green") + f": {bagit_path}/tagmanifest-sha512.txt")
+    
+    # Create manifest-md5.txt
+    bagit.create_payload_manifest_md5()
+    click.echo(click.style("Payload Manifest", fg="green") + f": {bagit_path}/manifest-md5.txt")
+    # Create tagmanifest-md5.txt
+    bagit.create_tag_manifest_md5()
+    click.echo(click.style("Tag Manifest", fg="green") + f": {bagit_path}/tagmanifest-md5.txt")
+
+    
+    
+
+
+    
+
+
+
```

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/rocrate/utils.py` & `fairscape_cli-0.1.7/fairscape_cli/rocrate/utils.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a4/fairscape_cli/validate/validate_json.py` & `fairscape_cli-0.1.7/fairscape_cli/validate/validate_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from fairscape_cli.models import (
     Dataset,
     Computation,
     Software
 )
 import click
 from pydantic import ValidationError
+from pathlib import Path
+import json
 
 
-def validate_model(path: str):
+def validate_model(path: str, model):
     json_path = Path(path)
     
     with open(json_path, "r") as json_file:
         metadata = json.load(json_file)
-        instance_model = model(**metadata)
+        instance_model = model.model_validate(metadata)
         return instance_model
 
 
 @click.group('validate')
 def validate():
     pass
```

### Comparing `fairscape_cli-0.1.5a4/pyproject.toml` & `fairscape_cli-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -22,35 +22,35 @@
 
 [project.urls]
 Homepage = "https://github.com/fairscape/fairscape-cli"
 
 
 [tool.poetry]
 name = "fairscape-cli"
-version = "0.1.5a4"
+version = "0.1.7"
 description = "A cli for validating metadata, packaging ROCrates, and interacting with the FAIRSCAPE API"
 authors = [
         "Max Levinson",
-        "Sadnan Al Manir",
+        "Sadnan Al Manir", 
         "Tim Clark"
 ]
 license = "LICENSE"
 readme = "README.md"
 packages = [{include = "fairscape_cli"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = "^1.10.7"
 pyld = "^2.0.3"
 click = "^8.1.3"
 fairscape-models = "^0.1.2"
 imageio = "^2.27.0"
 pandas = "^2.0.0"
 prettytable = "^3.7.0"
+mkdocs-material = "^9.1.18"
 
 
 [tool.poetry.scripts]
 fairscape-cli = "fairscape_cli.main:cli"
 
 [build-system]
 requires = ["poetry-core"]
```

