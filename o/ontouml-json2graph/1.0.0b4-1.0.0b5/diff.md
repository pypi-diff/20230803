# Comparing `tmp/ontouml_json2graph-1.0.0b4.tar.gz` & `tmp/ontouml_json2graph-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontouml_json2graph-1.0.0b4.tar", max compression
+gzip compressed data, was "ontouml_json2graph-1.0.0b5.tar", max compression
```

## Comparing `ontouml_json2graph-1.0.0b4.tar` & `ontouml_json2graph-1.0.0b5.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0    11558 2023-08-01 15:24:11.470721 ontouml_json2graph-1.0.0b4/LICENSE
--rw-r--r--   0        0        0      788 2023-08-01 18:58:30.114670 ontouml_json2graph-1.0.0b4/pyproject.toml
--rw-r--r--   0        0        0     7227 2023-08-01 15:24:11.505323 ontouml_json2graph-1.0.0b4/README.md
--rw-r--r--   0        0        0        0 2023-08-01 18:18:42.034762 ontouml_json2graph-1.0.0b4/src/__init__.py
--rw-r--r--   0        0        0     4536 2023-08-01 18:04:39.977624 ontouml_json2graph-1.0.0b4/src/main.py
--rw-r--r--   0        0        0        0 2023-08-01 15:24:11.472722 ontouml_json2graph-1.0.0b4/src/modules/__init__.py
--rw-r--r--   0        0        0     4134 2023-08-01 15:24:11.474722 ontouml_json2graph-1.0.0b4/src/modules/arguments.py
--rw-r--r--   0        0        0        0 2023-08-01 15:24:11.473968 ontouml_json2graph-1.0.0b4/src/modules/decoder/__init__.py
--rw-r--r--   0        0        0     9184 2023-08-01 15:24:11.477723 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_general.py
--rw-r--r--   0        0        0     9616 2023-08-01 15:24:11.478723 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_main.py
--rw-r--r--   0        0        0    20148 2023-08-01 15:24:11.480722 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_class.py
--rw-r--r--   0        0        0     3844 2023-08-01 15:24:11.482721 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_diagram.py
--rw-r--r--   0        0        0     4473 2023-08-01 15:24:11.484866 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_elementview.py
--rw-r--r--   0        0        0     2750 2023-08-01 15:24:11.483723 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_generalization.py
--rw-r--r--   0        0        0     4661 2023-08-01 15:24:11.486723 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_generalizationset.py
--rw-r--r--   0        0        0     4502 2023-08-01 15:24:11.482721 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_package.py
--rw-r--r--   0        0        0     2593 2023-08-01 15:24:11.484721 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_path.py
--rw-r--r--   0        0        0     5467 2023-08-01 15:24:11.484866 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_project.py
--rw-r--r--   0        0        0    14058 2023-08-01 15:24:11.485722 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_property.py
--rw-r--r--   0        0        0     3223 2023-08-01 15:24:11.490848 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_rectangularshape.py
--rw-r--r--   0        0        0     6594 2023-08-01 15:24:11.488721 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_relation.py
--rw-r--r--   0        0        0     2955 2023-08-01 15:24:11.484866 ontouml_json2graph-1.0.0b4/src/modules/errors.py
--rw-r--r--   0        0        0      701 2023-08-01 15:24:11.485722 ontouml_json2graph-1.0.0b4/src/modules/globals.py
--rw-r--r--   0        0        0     3476 2023-08-01 15:24:11.490848 ontouml_json2graph-1.0.0b4/src/modules/input_output.py
--rw-r--r--   0        0        0     2642 2023-08-01 15:24:11.490848 ontouml_json2graph-1.0.0b4/src/modules/logger.py
--rw-r--r--   0        0        0     7258 2023-08-01 15:24:11.495722 ontouml_json2graph-1.0.0b4/src/modules/messages.py
--rw-r--r--   0        0        0      878 2023-08-01 15:24:11.492800 ontouml_json2graph-1.0.0b4/src/modules/sparql_queries.py
--rw-r--r--   0        0        0     1486 2023-08-01 15:24:11.494722 ontouml_json2graph-1.0.0b4/src/modules/utils_general.py
--rw-r--r--   0        0        0     3688 2023-08-01 15:24:11.495722 ontouml_json2graph-1.0.0b4/src/modules/utils_graph.py
--rw-r--r--   0        0        0    84660 2023-08-01 15:24:11.505721 ontouml_json2graph-1.0.0b4/src/resources/logo-json2graph.png
--rw-r--r--   0        0        0    18036 2023-08-01 15:24:11.506917 ontouml_json2graph-1.0.0b4/src/resources/ontouml_v100.ttl
--rw-r--r--   0        0        0    78196 2023-08-01 15:24:11.507721 ontouml_json2graph-1.0.0b4/src/resources/ontouml_v110.ttl
--rw-r--r--   0        0        0     8257 1970-01-01 00:00:00.000000 ontouml_json2graph-1.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-02 10:46:56.176418 ontouml_json2graph-1.0.0b5/json2graph/__init__.py
+-rw-r--r--   0        0        0      613 2023-08-03 06:42:17.177350 ontouml_json2graph-1.0.0b5/json2graph/__main__.py
+-rw-r--r--   0        0        0     4190 2023-08-02 10:46:56.178418 ontouml_json2graph-1.0.0b5/json2graph/main_decode.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:46:56.178418 ontouml_json2graph-1.0.0b5/json2graph/modules/__init__.py
+-rw-r--r--   0        0        0     4318 2023-08-02 10:46:56.179420 ontouml_json2graph-1.0.0b5/json2graph/modules/arguments.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:46:56.179420 ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/__init__.py
+-rw-r--r--   0        0        0     9182 2023-08-02 10:46:56.180421 ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_general.py
+-rw-r--r--   0        0        0     9614 2023-08-02 10:46:56.181420 ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_main.py
+-rw-r--r--   0        0        0    20146 2023-08-02 10:46:56.182418 ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_class.py
+-rw-r--r--   0        0        0     3842 2023-08-02 10:46:56.182418 ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_diagram.py
+-rw-r--r--   0        0        0     4471 2023-08-02 10:46:56.183418 ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_elementview.py
+-rw-r--r--   0        0        0     2748 2023-08-02 10:46:56.184419 ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_generalization.py
+-rw-r--r--   0        0        0     4659 2023-08-02 10:46:56.184419 ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_generalizationset.py
+-rw-r--r--   0        0        0     4500 2023-08-02 10:46:56.185420 ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_package.py
+-rw-r--r--   0        0        0     2591 2023-08-02 10:46:56.186428 ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_path.py
+-rw-r--r--   0        0        0     5465 2023-08-02 10:46:56.187421 ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_project.py
+-rw-r--r--   0        0        0    14056 2023-08-02 10:46:56.188419 ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_property.py
+-rw-r--r--   0        0        0     3221 2023-08-02 10:46:56.188419 ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_rectangularshape.py
+-rw-r--r--   0        0        0     6592 2023-08-02 10:46:56.190419 ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_relation.py
+-rw-r--r--   0        0        0     2955 2023-08-02 10:46:56.190419 ontouml_json2graph-1.0.0b5/json2graph/modules/errors.py
+-rw-r--r--   0        0        0      764 2023-08-03 06:42:03.802409 ontouml_json2graph-1.0.0b5/json2graph/modules/globals.py
+-rw-r--r--   0        0        0     3474 2023-08-02 10:46:56.192419 ontouml_json2graph-1.0.0b5/json2graph/modules/input_output.py
+-rw-r--r--   0        0        0     2642 2023-08-02 10:46:56.193417 ontouml_json2graph-1.0.0b5/json2graph/modules/logger.py
+-rw-r--r--   0        0        0     7258 2023-08-02 10:46:56.193417 ontouml_json2graph-1.0.0b5/json2graph/modules/messages.py
+-rw-r--r--   0        0        0      878 2023-08-02 10:46:56.194418 ontouml_json2graph-1.0.0b5/json2graph/modules/sparql_queries.py
+-rw-r--r--   0        0        0     1486 2023-08-02 10:46:56.195420 ontouml_json2graph-1.0.0b5/json2graph/modules/utils_general.py
+-rw-r--r--   0        0        0     3686 2023-08-02 10:46:56.195420 ontouml_json2graph-1.0.0b5/json2graph/modules/utils_graph.py
+-rw-r--r--   0        0        0    84660 2023-08-02 10:46:56.196419 ontouml_json2graph-1.0.0b5/json2graph/resources/logo-json2graph.png
+-rw-r--r--   0        0        0    18036 2023-08-02 10:46:56.198417 ontouml_json2graph-1.0.0b5/json2graph/resources/ontouml_v100.ttl
+-rw-r--r--   0        0        0    78196 2023-08-02 10:46:56.199418 ontouml_json2graph-1.0.0b5/json2graph/resources/ontouml_v110.ttl
+-rw-r--r--   0        0        0    11558 2023-08-01 15:24:11.470721 ontouml_json2graph-1.0.0b5/LICENSE
+-rw-r--r--   0        0        0      800 2023-08-03 06:36:11.241747 ontouml_json2graph-1.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0     7362 2023-08-02 10:46:56.105432 ontouml_json2graph-1.0.0b5/README.md
+-rw-r--r--   0        0        0     8396 1970-01-01 00:00:00.000000 ontouml_json2graph-1.0.0b5/PKG-INFO
```

### Comparing `ontouml_json2graph-1.0.0b4/LICENSE` & `ontouml_json2graph-1.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b4/pyproject.toml` & `ontouml_json2graph-1.0.0b5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "ontouml-json2graph"
+version = "1.0.0b5"
 description = "OntoUML JSON2Graph Decoder"
-version = "v1.0.0b4"
-authors = ["Pedro Paulo F. Barcelos <pedropaulofb@gmail.com>"]
 license = "Apache-2.0"
-keywords = ["semantic-web", "knowledge-graph", "ontouml", "ontology-driven-development", "ontouml-schema",
-    "ontouml-vocabulary", "ontouml-metamodel"]
-
+authors = ["Pedro Paulo F. Barcelos <p.p.favatobarcelos@utwente.nl>"]
+readme = "README.md"
 homepage = "https://w3id.org/ontouml/json2graph"
 repository = "https://w3id.org/ontouml/json2graph"
 documentation = "https://w3id.org/ontouml/json2graph/docs"
-readme = "README.md"
+keywords = ["semantic-web", "knowledge-graph", "ontouml", "ontology-driven-development", "ontouml-schema", "ontouml-vocabulary", "ontouml-metamodel"]
+packages = [{include = "json2graph"}]
 
-#conformsTo = "https://w3id.org/ontouml"
-#conformsToVersion = "v1.1.0"
-
-packages =  [   { include = "src" },
-                { include = "src/main.py"} ]
+[extras]
+conformsTo = "https://w3id.org/ontouml"
+conformsToBase = "https://w3id.org/ontouml#"
+conformsToVersion = "v1.1.0"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
+
+
```

### Comparing `ontouml_json2graph-1.0.0b4/README.md` & `ontouml_json2graph-1.0.0b5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,23 +27,26 @@
 
 You need to [download and install Python](https://www.python.org/downloads/) to execute the ontouml-json2graph transformation tool. To install all necessary dependencies, run the following command on the terminal inside the project's folder:
 
 ```text
 pip install -r requirements.txt
 ```
 
-For executing the software, run the following command on the terminal inside the project's folder, where path_to_json must be substituted for the location of the catalog's directory on your computer:
+For executing the software, run the following command on the terminal inside the project's folder: 
 
 ```text
-python main.py path_to_json [ARGUMENTS]
+python json2graph [path_to_json] [OTHER ARGUMENTS]
 ```
 
+The only mandatory argument is `path_to_json`, which must be substituted for the input file's location on your computer. 
+Other arguments provide additional features and are presented in the next section.
+
 ## Arguments
 
-All available ontouml-models-tools arguments can be observed below.
+All available ontouml-json2graph arguments can be observed below.
 
 ```text
 usage: ontouml-json2graph [-h]
                           [-f {turtle,ttl,turtle2,xml,pretty-xml,json-ld,ntriples,nt,nt11,n3,trig,trix,nquads}]
                           [-l LANGUAGE] [-c] [-s] [-u BASE_URI] [-m] [-v]
                           json_file
 
@@ -86,16 +89,16 @@
     - Sets Class stereotype as 'event' when it is originally 'null' and the class is related to a Property with stereotype.
 
 ## Permanent URLs and Identifiers
 
 - Repository: https://w3id.org/ontouml/json2graph
 - Documentation: https://w3id.org/ontouml/json2graph/docs
 - Releases:
-    - Latest: https://w3id.org/ontouml/json2graph/latest
-    - Version: https://w3id.org/ontouml/json2graph/v<n>, where \<n\> is a version number (e.g., '1.0.0')
+    - Latest version: https://w3id.org/ontouml/json2graph/latest
+    - Specific version: https://w3id.org/ontouml/json2graph/v<n>, where \<n\> is a version number (e.g., '1.0.0')
 
 ## Related Projects
 
 - **[OntoUML Metamodel](https://w3id.org/ontouml/metamodel)
   **: Implementation-independent OntoUML Metamodel. Unlike the UML profile, this version is independent of UML and presents only the concepts officially supported in the language. This metamodel covers the abstract and concrete syntaxes of the language and serves as the reference for all projects in the [OntoUML as a Service (OaaS)](https://ceur-ws.org/Vol-2969/paper29-FOMI.pdf) ecosystem, including its different model serializations.
```

### Comparing `ontouml_json2graph-1.0.0b4/src/main.py` & `ontouml_json2graph-1.0.0b5/json2graph/main_decode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-""" Main file for ontouml-json2graph.
-
-It provides a convenient interface for converting OntoUML JSON files into knowledge graphs,
+""" It provides a convenient interface for converting OntoUML JSON files into knowledge graphs,
 with the flexibility to customize the output and control the execution mode for different use cases.
 """
 
 import time
 
 from rdflib import RDF
 
@@ -34,14 +32,15 @@
 
     logger = initialize_logger(execution_mode)
 
     model_elements = ["Class", "Property", "Generalization", "GeneralizationSet", "Relation", "Cardinality"]
 
     # Setting tests' arguments
     if execution_mode == "test":
+        args.initialize_arguments(execution_mode)
         args.ARGUMENTS["correct"] = True
         args.ARGUMENTS["silent"] = True
         args.ARGUMENTS["base_uri"] = 'https://example.org#'
         args.ARGUMENTS["model_only"] = False
 
     if execution_mode == "production" and not args.ARGUMENTS["silent"]:
         # Initial time information
@@ -86,19 +85,7 @@
         logger.info(f"Decoding concluded on {end_date_time}. Total execution time: {elapsed_time} seconds.")
 
     # Save graph as specified format
     output_file_path = write_graph_file(ontouml_graph, json_path, graph_format)
     logger.info(f"Output graph file successfully saved at {output_file_path}.")
 
     return output_file_path
-
-
-if __name__ == '__main__':
-    # Treat and publish user's arguments
-    args.publish_user_arguments()
-
-    json_path = args.ARGUMENTS["json_path"]
-    graph_format = args.ARGUMENTS["format"]
-    language = args.ARGUMENTS["language"]
-
-    # Execute the transformation
-    decode_ontouml_json2graph(json_path, graph_format, language, "production")
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/arguments.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/arguments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """ Argument Treatments """
 
 import argparse
 
 import validators as validators
 
-from modules.globals import METADATA
-from modules.logger import initialize_logger
+from .globals import METADATA
+from .logger import initialize_logger
 
-LOGGER = initialize_logger()
 ARGUMENTS = {}
 
+LOGGER = initialize_logger()
+
 
 def treat_user_arguments() -> dict:
     """ Treat arguments provided by the user when starting software execution.
 
     :return: Dictionary with json path (key 'json_path') and final file format (key 'format').
     :rtype: dict
     :raises OSError: If provided input is not of JSON type.
@@ -79,11 +80,18 @@
         arguments_dictionary["base_uri"] += '#'
 
     LOGGER.debug(f"Arguments parsed. Obtained values are: {arguments_dictionary}.")
 
     return arguments_dictionary
 
 
-def publish_user_arguments():
-    arguments_dictionary = treat_user_arguments()
+def initialize_arguments(execution_mode: str = "production"):
+    """
+
+    :param execution_mode: Information about execution mode. Valid values are 'production' (default) and 'test'.
+    :type execution_mode: str
+    """
+
     global ARGUMENTS
-    ARGUMENTS = arguments_dictionary
+
+    if execution_mode == "production":
+        ARGUMENTS = treat_user_arguments()
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_general.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_general.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """ General decoding functions. """
 
-from rdflib import Graph, URIRef, Literal, RDF
-
 import modules.arguments as args
 from modules.logger import initialize_logger
 from modules.sparql_queries import GET_ELEMENT_AND_TYPE
 from modules.utils_graph import load_ontouml_vocabulary, ontouml_ref
+from rdflib import Graph, URIRef, Literal, RDF
 
 LOGGER = initialize_logger()
 
 
 def create_point(point_id: str, x_coord: int, y_coord: int, ontouml_graph: Graph) -> None:
     """ Creates a new instance of ontouml:Point with its ontouml:xCoordinate, and ontouml:yCoordinate properties.
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_main.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """ JSON decode functions."""
 
-from rdflib import Graph, URIRef, Literal, RDF, XSD, OWL, RDFS
-
 import modules.arguments as args
 from modules.decoder.decode_general import clean_null_data, count_elements_graph
 from modules.decoder.decode_obj_class import create_class_properties
 from modules.decoder.decode_obj_diagram import create_diagram_properties
 from modules.decoder.decode_obj_elementview import create_elementview_properties
 from modules.decoder.decode_obj_generalization import create_generalization_properties
 from modules.decoder.decode_obj_generalizationset import create_generalizationset_properties
@@ -15,14 +13,15 @@
 from modules.decoder.decode_obj_property import create_property_properties
 from modules.decoder.decode_obj_rectangularshape import create_rectangularshape_properties
 from modules.decoder.decode_obj_relation import create_relation_properties
 from modules.globals import URI_ONTOUML, ELEMENT_VIEW_TYPES, METADATA
 from modules.logger import initialize_logger
 from modules.utils_general import get_date_time
 from modules.utils_graph import ontouml_ref
+from rdflib import Graph, URIRef, Literal, RDF, XSD, OWL, RDFS
 
 LOGGER = initialize_logger()
 
 
 def add_metadata(ontouml_graph: Graph) -> None:
     """ Adds basic metadata to the generated graph when not in test mode. The metadata added are:
         - dct:conformsTo URI_ONTOUML
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_class.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,20 @@
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
 """
 
 import inspect
 
-from rdflib import Graph, URIRef, XSD, Literal
-
 import modules.arguments as args
 from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, get_stereotype
 from modules.errors import report_error_end_of_switch
 from modules.messages import print_decode_log_message
 from modules.utils_graph import ontouml_ref
+from rdflib import Graph, URIRef, XSD, Literal
 
 
 def validate_class_attribute_constraints(class_dict: dict) -> None:
     """ Verifies all Class dictionaries and check if the constraints related to classes were correctly considered and
     fixes them when they are not.
 
     The pair of attribute/stereotype: isExtensional/collective and isPowertype/type checked constraints are:
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_diagram.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_diagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,19 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-from rdflib import Graph, URIRef
-
 import modules.arguments as args
 from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
 from modules.globals import ELEMENT_VIEW_TYPES
 from modules.utils_graph import ontouml_ref
+from rdflib import Graph, URIRef
 
 
 def set_diagram_owner_modelelement(diagram_dict: dict, ontouml_graph: Graph) -> None:
     """ Set the ontouml:owner property between an ontouml:Diagram and its related ontouml:Package.
 
     :param diagram_dict: Diagram object loaded as a dictionary.
     :type diagram_dict: dict
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_elementview.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_elementview.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,20 @@
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 import inspect
 
-from rdflib import Graph, URIRef
-
 import modules.arguments as args
 from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
 from modules.errors import report_error_end_of_switch
 from modules.globals import ELEMENT_VIEW_TYPES
 from modules.utils_graph import ontouml_ref
+from rdflib import Graph, URIRef
 
 
 def set_elementview_relations(elementview_dict: dict, ontouml_graph: Graph) -> None:
     """ Set an ontouml:ElementView's ontouml:shape and ontouml:isViewOf object properties in the resulting graph.
 
     :param elementview_dict: ElementView object loaded as a dictionary.
     :type elementview_dict: dict
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_generalization.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_generalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,18 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-from rdflib import Graph, URIRef
-
 import modules.arguments as args
 from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
 from modules.utils_graph import ontouml_ref
+from rdflib import Graph, URIRef
 
 
 def set_generalization_relations(generalization_dict: dict, ontouml_graph: Graph) -> None:
     """ Set the ontouml:general and ontouml:specific properties in the resulting graph.
 
     :param generalization_dict: Generalization object loaded as a dictionary.
     :type generalization_dict: dict
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_generalizationset.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_generalizationset.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,19 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-from rdflib import Graph, URIRef, Literal, XSD
-
 import modules.arguments as args
 from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
 from modules.messages import print_decode_log_message
 from modules.utils_graph import ontouml_ref
+from rdflib import Graph, URIRef, Literal, XSD
 
 
 def set_generalizationset_defaults(generalizationset_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets the default values to ontouml:generalizationSets to the resulting graph.
 
     - Default isDisjoint: If isDisjoint is null, set as False.
     - Default isComplete: If isComplete is null, set as False.
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_package.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_package.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,18 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-from rdflib import Graph, URIRef
-
 import modules.arguments as args
 from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
 from modules.utils_graph import ontouml_ref
+from rdflib import Graph, URIRef
 
 
 def get_package_contents(package_dict: dict, package_id: str, list_contents: list = []) -> list[dict]:
     """ Receives the dictionary with all loaded JSON data and returns the value of the 'contents' field for a given
     object (defined by the received value of its ID).
 
     :param package_dict: Package's data to have its fields decoded.
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_path.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,18 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-from rdflib import Graph, URIRef
-
 import modules.arguments as args
 from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, create_point
 from modules.utils_graph import ontouml_ref
+from rdflib import Graph, URIRef
 
 
 def set_path_path_point(path_dict: dict, ontouml_graph: Graph) -> None:
     """ Creates an ontouml:Point, their properties and the ontouml:point of an ontouml:Path.
 
     :param path_dict: Path object loaded as a dictionary.
     :type path_dict: dict
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_project.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,18 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-from rdflib import Graph, URIRef
-
 import modules.arguments as args
 from modules.decoder.decode_general import get_all_ids_of_specific_type, get_list_subdictionaries_for_specific_type
 from modules.utils_graph import ontouml_ref
+from rdflib import Graph, URIRef
 
 
 def set_ontoumlelement_project_project(project_dict: dict, ontouml_graph: Graph, element_counting: dict) -> None:
     """ Sets the ontouml:project object property between an ontouml:Project (obj) and all its related entities (subj).
 
     :param project_dict: Project's data to have its fields decoded.
     :type project_dict: dict
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_property.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,21 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-from rdflib import Graph, URIRef, RDF, Literal, XSD
-
 import modules.arguments as args
 from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
 from modules.logger import initialize_logger
 from modules.messages import print_decode_log_message
 from modules.sparql_queries import GET_CLASS_STEREOTYPE_ATTRIBUTE_STEREOTYPE
 from modules.utils_graph import load_ontouml_vocabulary, ontouml_ref
+from rdflib import Graph, URIRef, RDF, Literal, XSD
 
 LOGGER = initialize_logger()
 
 
 def validate_property_stereotype(ontouml_graph: Graph) -> None:
     """ Performs syntactical and semantic validations on an ontouml:Property's stereotype.
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_rectangularshape.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_rectangularshape.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,18 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-from rdflib import Graph, URIRef
-
 import modules.arguments as args
 from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, create_point
 from modules.utils_graph import ontouml_ref
+from rdflib import Graph, URIRef
 
 
 def set_rectangularshape_coordinates(rectangularshape_dict: dict, ontouml_graph: Graph) -> None:
     """ Creates an ontouml:Point, their properties and the ontouml:topLeftPosition of an ontouml:RectangularShape.
 
     :param rectangularshape_dict: RectangularShape object loaded as a dictionary.
     :type rectangularshape_dict: dict
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_relation.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/decoder/decode_obj_relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,19 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-from rdflib import Graph, URIRef, Literal, XSD
-
 import modules.arguments as args
 from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, get_stereotype
 from modules.messages import print_decode_log_message
 from modules.utils_graph import ontouml_ref
+from rdflib import Graph, URIRef, Literal, XSD
 
 
 def set_relation_defaults(relation_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets the following attribute's default values for ontouml:Relation:
 
     DRA1) ontouml:isDerived default value = False
     DRA2) ontouml:isAbstract default value = False
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/errors.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/errors.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/globals.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/globals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """ Global variables definitions. """
 from os.path import exists
+from pprint import pprint
 
 import toml as toml
 
 # Software's metadata got from pyproject.toml config file
 global METADATA
 
 pyproject_file = "pyproject.toml"
 pyproject_path_prod = "./" + pyproject_file
 pyproject_path_test = "../" + pyproject_file
 pyproject_path = pyproject_path_prod if exists(pyproject_file) else pyproject_path_test
 
 metadata_project = toml.load(pyproject_path)
-METADATA = metadata_project["project"]
+METADATA = metadata_project["tool"]["poetry"] | metadata_project["extras"]
 
 # URIs
 URI_ONTOUML = "https://w3id.org/ontouml#"
 
 # GROUPS OF CONCEPTS
 
 ELEMENT_VIEW_TYPES = ["ClassView", "PackageView", "GeneralizationSetView", "RelationView", "GeneralizationView",
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/input_output.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/input_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """ IO functions used in diverse occasions. """
 
 import json
 import os
 from pathlib import Path
 
-from rdflib import Graph
-
 from modules.errors import report_error_io_read, report_error_io_write
 from modules.logger import initialize_logger
+from rdflib import Graph
 
 LOGGER = initialize_logger()
 
 
 def create_directory_if_not_exists(directory_path: str, file_description: str) -> None:
     """ Checks if the directory that has the path received as argument exists.
     If it does, do nothing. If it does not, create it.
```

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/logger.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/logger.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/messages.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/messages.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/sparql_queries.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/sparql_queries.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/utils_general.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/utils_general.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b4/src/modules/utils_graph.py` & `ontouml_json2graph-1.0.0b5/json2graph/modules/utils_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """ Util functions related to graphs. """
 
-from rdflib import Graph, URIRef, RDF
-
 from modules.errors import report_error_io_read
 from modules.globals import METADATA
 from modules.logger import initialize_logger
+from rdflib import Graph, URIRef, RDF
 
 LOGGER = initialize_logger()
 
 
 def ontouml_ref(entity: str) -> URIRef:
     """ Receives the name of the OntoUML Vocabulary's entity as a string and returns the corresponding URIRef.
```

### Comparing `ontouml_json2graph-1.0.0b4/src/resources/logo-json2graph.png` & `ontouml_json2graph-1.0.0b5/json2graph/resources/logo-json2graph.png`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b4/src/resources/ontouml_v100.ttl` & `ontouml_json2graph-1.0.0b5/json2graph/resources/ontouml_v100.ttl`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b4/src/resources/ontouml_v110.ttl` & `ontouml_json2graph-1.0.0b5/json2graph/resources/ontouml_v110.ttl`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b4/PKG-INFO` & `ontouml_json2graph-1.0.0b5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ontouml-json2graph
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: OntoUML JSON2Graph Decoder
 Home-page: https://w3id.org/ontouml/json2graph
 License: Apache-2.0
 Keywords: semantic-web,knowledge-graph,ontouml,ontology-driven-development,ontouml-schema,ontouml-vocabulary,ontouml-metamodel
 Author: Pedro Paulo F. Barcelos
-Author-email: pedropaulofb@gmail.com
+Author-email: p.p.favatobarcelos@utwente.nl
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -52,23 +52,26 @@
 
 You need to [download and install Python](https://www.python.org/downloads/) to execute the ontouml-json2graph transformation tool. To install all necessary dependencies, run the following command on the terminal inside the project's folder:
 
 ```text
 pip install -r requirements.txt
 ```
 
-For executing the software, run the following command on the terminal inside the project's folder, where path_to_json must be substituted for the location of the catalog's directory on your computer:
+For executing the software, run the following command on the terminal inside the project's folder: 
 
 ```text
-python main.py path_to_json [ARGUMENTS]
+python json2graph [path_to_json] [OTHER ARGUMENTS]
 ```
 
+The only mandatory argument is `path_to_json`, which must be substituted for the input file's location on your computer. 
+Other arguments provide additional features and are presented in the next section.
+
 ## Arguments
 
-All available ontouml-models-tools arguments can be observed below.
+All available ontouml-json2graph arguments can be observed below.
 
 ```text
 usage: ontouml-json2graph [-h]
                           [-f {turtle,ttl,turtle2,xml,pretty-xml,json-ld,ntriples,nt,nt11,n3,trig,trix,nquads}]
                           [-l LANGUAGE] [-c] [-s] [-u BASE_URI] [-m] [-v]
                           json_file
 
@@ -111,16 +114,16 @@
     - Sets Class stereotype as 'event' when it is originally 'null' and the class is related to a Property with stereotype.
 
 ## Permanent URLs and Identifiers
 
 - Repository: https://w3id.org/ontouml/json2graph
 - Documentation: https://w3id.org/ontouml/json2graph/docs
 - Releases:
-    - Latest: https://w3id.org/ontouml/json2graph/latest
-    - Version: https://w3id.org/ontouml/json2graph/v<n>, where \<n\> is a version number (e.g., '1.0.0')
+    - Latest version: https://w3id.org/ontouml/json2graph/latest
+    - Specific version: https://w3id.org/ontouml/json2graph/v<n>, where \<n\> is a version number (e.g., '1.0.0')
 
 ## Related Projects
 
 - **[OntoUML Metamodel](https://w3id.org/ontouml/metamodel)
   **: Implementation-independent OntoUML Metamodel. Unlike the UML profile, this version is independent of UML and presents only the concepts officially supported in the language. This metamodel covers the abstract and concrete syntaxes of the language and serves as the reference for all projects in the [OntoUML as a Service (OaaS)](https://ceur-ws.org/Vol-2969/paper29-FOMI.pdf) ecosystem, including its different model serializations.
```

