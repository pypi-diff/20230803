# Comparing `tmp/ontouml_json2graph-1.0.0b6.tar.gz` & `tmp/ontouml_json2graph-1.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontouml_json2graph-1.0.0b6.tar", max compression
+gzip compressed data, was "ontouml_json2graph-1.0.0b7.tar", max compression
```

## Comparing `ontouml_json2graph-1.0.0b6.tar` & `ontouml_json2graph-1.0.0b7.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0        0 2023-08-02 10:46:56.176418 ontouml_json2graph-1.0.0b6/json2graph/__init__.py
--rw-r--r--   0        0        0      613 2023-08-03 06:42:17.177350 ontouml_json2graph-1.0.0b6/json2graph/__main__.py
--rw-r--r--   0        0        0     4190 2023-08-02 10:46:56.178418 ontouml_json2graph-1.0.0b6/json2graph/main_decode.py
--rw-r--r--   0        0        0        0 2023-08-02 10:46:56.178418 ontouml_json2graph-1.0.0b6/json2graph/modules/__init__.py
--rw-r--r--   0        0        0     4318 2023-08-02 10:46:56.179420 ontouml_json2graph-1.0.0b6/json2graph/modules/arguments.py
--rw-r--r--   0        0        0        0 2023-08-02 10:46:56.179420 ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/__init__.py
--rw-r--r--   0        0        0     9182 2023-08-02 10:46:56.180421 ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_general.py
--rw-r--r--   0        0        0     9631 2023-08-03 06:47:54.786096 ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_main.py
--rw-r--r--   0        0        0    20146 2023-08-02 10:46:56.182418 ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_class.py
--rw-r--r--   0        0        0     3842 2023-08-02 10:46:56.182418 ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_diagram.py
--rw-r--r--   0        0        0     4471 2023-08-02 10:46:56.183418 ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_elementview.py
--rw-r--r--   0        0        0     2748 2023-08-02 10:46:56.184419 ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_generalization.py
--rw-r--r--   0        0        0     4659 2023-08-02 10:46:56.184419 ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_generalizationset.py
--rw-r--r--   0        0        0     4500 2023-08-02 10:46:56.185420 ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_package.py
--rw-r--r--   0        0        0     2591 2023-08-02 10:46:56.186428 ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_path.py
--rw-r--r--   0        0        0     5465 2023-08-02 10:46:56.187421 ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_project.py
--rw-r--r--   0        0        0    14056 2023-08-02 10:46:56.188419 ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_property.py
--rw-r--r--   0        0        0     3221 2023-08-02 10:46:56.188419 ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_rectangularshape.py
--rw-r--r--   0        0        0     6592 2023-08-02 10:46:56.190419 ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_relation.py
--rw-r--r--   0        0        0     2955 2023-08-02 10:46:56.190419 ontouml_json2graph-1.0.0b6/json2graph/modules/errors.py
--rw-r--r--   0        0        0      711 2023-08-03 06:48:14.947600 ontouml_json2graph-1.0.0b6/json2graph/modules/globals.py
--rw-r--r--   0        0        0     3474 2023-08-02 10:46:56.192419 ontouml_json2graph-1.0.0b6/json2graph/modules/input_output.py
--rw-r--r--   0        0        0     2642 2023-08-02 10:46:56.193417 ontouml_json2graph-1.0.0b6/json2graph/modules/logger.py
--rw-r--r--   0        0        0     7258 2023-08-02 10:46:56.193417 ontouml_json2graph-1.0.0b6/json2graph/modules/messages.py
--rw-r--r--   0        0        0      878 2023-08-02 10:46:56.194418 ontouml_json2graph-1.0.0b6/json2graph/modules/sparql_queries.py
--rw-r--r--   0        0        0     1486 2023-08-02 10:46:56.195420 ontouml_json2graph-1.0.0b6/json2graph/modules/utils_general.py
--rw-r--r--   0        0        0     3686 2023-08-02 10:46:56.195420 ontouml_json2graph-1.0.0b6/json2graph/modules/utils_graph.py
--rw-r--r--   0        0        0    84660 2023-08-02 10:46:56.196419 ontouml_json2graph-1.0.0b6/json2graph/resources/logo-json2graph.png
--rw-r--r--   0        0        0    18036 2023-08-02 10:46:56.198417 ontouml_json2graph-1.0.0b6/json2graph/resources/ontouml_v100.ttl
--rw-r--r--   0        0        0    78196 2023-08-02 10:46:56.199418 ontouml_json2graph-1.0.0b6/json2graph/resources/ontouml_v110.ttl
--rw-r--r--   0        0        0    11558 2023-08-01 15:24:11.470721 ontouml_json2graph-1.0.0b6/LICENSE
--rw-r--r--   0        0        0      800 2023-08-03 06:50:29.399611 ontouml_json2graph-1.0.0b6/pyproject.toml
--rw-r--r--   0        0        0     7362 2023-08-02 10:46:56.105432 ontouml_json2graph-1.0.0b6/README.md
--rw-r--r--   0        0        0     8396 1970-01-01 00:00:00.000000 ontouml_json2graph-1.0.0b6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-02 10:46:56.176418 ontouml_json2graph-1.0.0b7/json2graph/__init__.py
+-rw-r--r--   0        0        0      613 2023-08-03 06:42:17.177350 ontouml_json2graph-1.0.0b7/json2graph/__main__.py
+-rw-r--r--   0        0        0     4190 2023-08-02 10:46:56.178418 ontouml_json2graph-1.0.0b7/json2graph/main_decode.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:46:56.178418 ontouml_json2graph-1.0.0b7/json2graph/modules/__init__.py
+-rw-r--r--   0        0        0     4318 2023-08-02 10:46:56.179420 ontouml_json2graph-1.0.0b7/json2graph/modules/arguments.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:46:56.179420 ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/__init__.py
+-rw-r--r--   0        0        0     9182 2023-08-02 10:46:56.180421 ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_general.py
+-rw-r--r--   0        0        0     9631 2023-08-03 06:47:54.786096 ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_main.py
+-rw-r--r--   0        0        0    20146 2023-08-02 10:46:56.182418 ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_class.py
+-rw-r--r--   0        0        0     3842 2023-08-02 10:46:56.182418 ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_diagram.py
+-rw-r--r--   0        0        0     4471 2023-08-02 10:46:56.183418 ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_elementview.py
+-rw-r--r--   0        0        0     2748 2023-08-02 10:46:56.184419 ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_generalization.py
+-rw-r--r--   0        0        0     4659 2023-08-02 10:46:56.184419 ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_generalizationset.py
+-rw-r--r--   0        0        0     4500 2023-08-02 10:46:56.185420 ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_package.py
+-rw-r--r--   0        0        0     2591 2023-08-02 10:46:56.186428 ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_path.py
+-rw-r--r--   0        0        0     5465 2023-08-02 10:46:56.187421 ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_project.py
+-rw-r--r--   0        0        0    14056 2023-08-02 10:46:56.188419 ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_property.py
+-rw-r--r--   0        0        0     3221 2023-08-02 10:46:56.188419 ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_rectangularshape.py
+-rw-r--r--   0        0        0     6592 2023-08-02 10:46:56.190419 ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_relation.py
+-rw-r--r--   0        0        0     2955 2023-08-02 10:46:56.190419 ontouml_json2graph-1.0.0b7/json2graph/modules/errors.py
+-rw-r--r--   0        0        0      711 2023-08-03 06:48:14.947600 ontouml_json2graph-1.0.0b7/json2graph/modules/globals.py
+-rw-r--r--   0        0        0     3474 2023-08-02 10:46:56.192419 ontouml_json2graph-1.0.0b7/json2graph/modules/input_output.py
+-rw-r--r--   0        0        0     2642 2023-08-02 10:46:56.193417 ontouml_json2graph-1.0.0b7/json2graph/modules/logger.py
+-rw-r--r--   0        0        0     7258 2023-08-02 10:46:56.193417 ontouml_json2graph-1.0.0b7/json2graph/modules/messages.py
+-rw-r--r--   0        0        0      878 2023-08-02 10:46:56.194418 ontouml_json2graph-1.0.0b7/json2graph/modules/sparql_queries.py
+-rw-r--r--   0        0        0     1486 2023-08-02 10:46:56.195420 ontouml_json2graph-1.0.0b7/json2graph/modules/utils_general.py
+-rw-r--r--   0        0        0     3686 2023-08-02 10:46:56.195420 ontouml_json2graph-1.0.0b7/json2graph/modules/utils_graph.py
+-rw-r--r--   0        0        0       49 2023-08-03 06:59:49.504172 ontouml_json2graph-1.0.0b7/json2graph/requirements.txt
+-rw-r--r--   0        0        0    84660 2023-08-02 10:46:56.196419 ontouml_json2graph-1.0.0b7/json2graph/resources/logo-json2graph.png
+-rw-r--r--   0        0        0    18036 2023-08-02 10:46:56.198417 ontouml_json2graph-1.0.0b7/json2graph/resources/ontouml_v100.ttl
+-rw-r--r--   0        0        0    78196 2023-08-02 10:46:56.199418 ontouml_json2graph-1.0.0b7/json2graph/resources/ontouml_v110.ttl
+-rw-r--r--   0        0        0    11558 2023-08-01 15:24:11.470721 ontouml_json2graph-1.0.0b7/LICENSE
+-rw-r--r--   0        0        0      800 2023-08-03 07:02:00.356450 ontouml_json2graph-1.0.0b7/pyproject.toml
+-rw-r--r--   0        0        0     7362 2023-08-02 10:46:56.105432 ontouml_json2graph-1.0.0b7/README.md
+-rw-r--r--   0        0        0     8396 1970-01-01 00:00:00.000000 ontouml_json2graph-1.0.0b7/PKG-INFO
```

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/__main__.py` & `ontouml_json2graph-1.0.0b7/json2graph/__main__.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/main_decode.py` & `ontouml_json2graph-1.0.0b7/json2graph/main_decode.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/arguments.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/arguments.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_general.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_general.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_main.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_main.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_class.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_class.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_diagram.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_diagram.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_elementview.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_elementview.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_generalization.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_generalization.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_generalizationset.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_generalizationset.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_package.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_package.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_path.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_path.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_project.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_project.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_property.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_property.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_rectangularshape.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_rectangularshape.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/decoder/decode_obj_relation.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/decoder/decode_obj_relation.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/errors.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/errors.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/globals.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/globals.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/input_output.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/input_output.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/logger.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/logger.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/messages.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/messages.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/sparql_queries.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/sparql_queries.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/utils_general.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/utils_general.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/modules/utils_graph.py` & `ontouml_json2graph-1.0.0b7/json2graph/modules/utils_graph.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/resources/logo-json2graph.png` & `ontouml_json2graph-1.0.0b7/json2graph/resources/logo-json2graph.png`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/resources/ontouml_v100.ttl` & `ontouml_json2graph-1.0.0b7/json2graph/resources/ontouml_v100.ttl`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/json2graph/resources/ontouml_v110.ttl` & `ontouml_json2graph-1.0.0b7/json2graph/resources/ontouml_v110.ttl`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/LICENSE` & `ontouml_json2graph-1.0.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/pyproject.toml` & `ontouml_json2graph-1.0.0b7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ontouml-json2graph"
-version = "1.0.0b6"
+version = "1.0.0b7"
 description = "OntoUML JSON2Graph Decoder"
 license = "Apache-2.0"
 authors = ["Pedro Paulo F. Barcelos <p.p.favatobarcelos@utwente.nl>"]
 readme = "README.md"
 homepage = "https://w3id.org/ontouml/json2graph"
 repository = "https://w3id.org/ontouml/json2graph"
 documentation = "https://w3id.org/ontouml/json2graph/docs"
```

### Comparing `ontouml_json2graph-1.0.0b6/README.md` & `ontouml_json2graph-1.0.0b7/README.md`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b6/PKG-INFO` & `ontouml_json2graph-1.0.0b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontouml-json2graph
-Version: 1.0.0b6
+Version: 1.0.0b7
 Summary: OntoUML JSON2Graph Decoder
 Home-page: https://w3id.org/ontouml/json2graph
 License: Apache-2.0
 Keywords: semantic-web,knowledge-graph,ontouml,ontology-driven-development,ontouml-schema,ontouml-vocabulary,ontouml-metamodel
 Author: Pedro Paulo F. Barcelos
 Author-email: p.p.favatobarcelos@utwente.nl
 Classifier: License :: OSI Approved :: Apache Software License
```

