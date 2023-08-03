# Comparing `tmp/ontouml_json2graph-1.0.0b8.tar.gz` & `tmp/ontouml_json2graph-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontouml_json2graph-1.0.0b8.tar", max compression
+gzip compressed data, was "ontouml_json2graph-1.0.0b9.tar", max compression
```

## Comparing `ontouml_json2graph-1.0.0b8.tar` & `ontouml_json2graph-1.0.0b9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0        0 2023-08-02 10:46:56.176418 ontouml_json2graph-1.0.0b8/json2graph/__init__.py
--rw-r--r--   0        0        0      613 2023-08-03 06:42:17.177350 ontouml_json2graph-1.0.0b8/json2graph/__main__.py
--rw-r--r--   0        0        0     4238 2023-08-03 07:27:32.062155 ontouml_json2graph-1.0.0b8/json2graph/main_decode.py
--rw-r--r--   0        0        0        0 2023-08-02 10:46:56.178418 ontouml_json2graph-1.0.0b8/json2graph/modules/__init__.py
--rw-r--r--   0        0        0     4318 2023-08-02 10:46:56.179420 ontouml_json2graph-1.0.0b8/json2graph/modules/arguments.py
--rw-r--r--   0        0        0        0 2023-08-02 10:46:56.179420 ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/__init__.py
--rw-r--r--   0        0        0     9182 2023-08-02 10:46:56.180421 ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_general.py
--rw-r--r--   0        0        0     9631 2023-08-03 06:47:54.786096 ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_main.py
--rw-r--r--   0        0        0    20146 2023-08-02 10:46:56.182418 ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_class.py
--rw-r--r--   0        0        0     3842 2023-08-02 10:46:56.182418 ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_diagram.py
--rw-r--r--   0        0        0     4471 2023-08-02 10:46:56.183418 ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_elementview.py
--rw-r--r--   0        0        0     2748 2023-08-02 10:46:56.184419 ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_generalization.py
--rw-r--r--   0        0        0     4659 2023-08-02 10:46:56.184419 ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_generalizationset.py
--rw-r--r--   0        0        0     4500 2023-08-02 10:46:56.185420 ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_package.py
--rw-r--r--   0        0        0     2591 2023-08-02 10:46:56.186428 ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_path.py
--rw-r--r--   0        0        0     5465 2023-08-02 10:46:56.187421 ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_project.py
--rw-r--r--   0        0        0    14056 2023-08-02 10:46:56.188419 ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_property.py
--rw-r--r--   0        0        0     3221 2023-08-02 10:46:56.188419 ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_rectangularshape.py
--rw-r--r--   0        0        0     6592 2023-08-02 10:46:56.190419 ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_relation.py
--rw-r--r--   0        0        0     2955 2023-08-02 10:46:56.190419 ontouml_json2graph-1.0.0b8/json2graph/modules/errors.py
--rw-r--r--   0        0        0      711 2023-08-03 06:48:14.947600 ontouml_json2graph-1.0.0b8/json2graph/modules/globals.py
--rw-r--r--   0        0        0     3474 2023-08-02 10:46:56.192419 ontouml_json2graph-1.0.0b8/json2graph/modules/input_output.py
--rw-r--r--   0        0        0     2642 2023-08-02 10:46:56.193417 ontouml_json2graph-1.0.0b8/json2graph/modules/logger.py
--rw-r--r--   0        0        0     7258 2023-08-02 10:46:56.193417 ontouml_json2graph-1.0.0b8/json2graph/modules/messages.py
--rw-r--r--   0        0        0      878 2023-08-02 10:46:56.194418 ontouml_json2graph-1.0.0b8/json2graph/modules/sparql_queries.py
--rw-r--r--   0        0        0     1486 2023-08-02 10:46:56.195420 ontouml_json2graph-1.0.0b8/json2graph/modules/utils_general.py
--rw-r--r--   0        0        0     3686 2023-08-02 10:46:56.195420 ontouml_json2graph-1.0.0b8/json2graph/modules/utils_graph.py
--rw-r--r--   0        0        0    84660 2023-08-02 10:46:56.196419 ontouml_json2graph-1.0.0b8/json2graph/resources/logo-json2graph.png
--rw-r--r--   0        0        0    18036 2023-08-02 10:46:56.198417 ontouml_json2graph-1.0.0b8/json2graph/resources/ontouml_v100.ttl
--rw-r--r--   0        0        0    78196 2023-08-02 10:46:56.199418 ontouml_json2graph-1.0.0b8/json2graph/resources/ontouml_v110.ttl
--rw-r--r--   0        0        0    11558 2023-08-01 15:24:11.470721 ontouml_json2graph-1.0.0b8/LICENSE
--rw-r--r--   0        0        0      909 2023-08-03 07:42:52.619064 ontouml_json2graph-1.0.0b8/pyproject.toml
--rw-r--r--   0        0        0     7289 2023-08-03 07:26:16.856872 ontouml_json2graph-1.0.0b8/README.md
--rw-r--r--   0        0        0     8028 1970-01-01 00:00:00.000000 ontouml_json2graph-1.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-02 10:46:56.176418 ontouml_json2graph-1.0.0b9/json2graph/__init__.py
+-rw-r--r--   0        0        0      613 2023-08-03 06:42:17.177350 ontouml_json2graph-1.0.0b9/json2graph/__main__.py
+-rw-r--r--   0        0        0     4238 2023-08-03 07:27:32.062155 ontouml_json2graph-1.0.0b9/json2graph/main_decode.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:46:56.178418 ontouml_json2graph-1.0.0b9/json2graph/modules/__init__.py
+-rw-r--r--   0        0        0     4318 2023-08-02 10:46:56.179420 ontouml_json2graph-1.0.0b9/json2graph/modules/arguments.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:46:56.179420 ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/__init__.py
+-rw-r--r--   0        0        0     9166 2023-08-03 07:58:16.925113 ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_general.py
+-rw-r--r--   0        0        0     9537 2023-08-03 07:58:16.987336 ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_main.py
+-rw-r--r--   0        0        0    20124 2023-08-03 07:58:16.863111 ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_class.py
+-rw-r--r--   0        0        0     3826 2023-08-03 07:58:16.797446 ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_diagram.py
+-rw-r--r--   0        0        0     4449 2023-08-03 07:58:16.629112 ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_elementview.py
+-rw-r--r--   0        0        0     2738 2023-08-03 07:58:16.957218 ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_generalization.py
+-rw-r--r--   0        0        0     4643 2023-08-03 07:58:16.769111 ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_generalizationset.py
+-rw-r--r--   0        0        0     4490 2023-08-03 07:58:16.703109 ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_package.py
+-rw-r--r--   0        0        0     2581 2023-08-03 07:58:16.734112 ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_path.py
+-rw-r--r--   0        0        0     5455 2023-08-03 07:58:17.023111 ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_project.py
+-rw-r--r--   0        0        0    14028 2023-08-03 07:58:16.667109 ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_property.py
+-rw-r--r--   0        0        0     3211 2023-08-03 07:58:16.893114 ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_rectangularshape.py
+-rw-r--r--   0        0        0     6576 2023-08-03 07:58:16.832378 ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_relation.py
+-rw-r--r--   0        0        0     2948 2023-08-03 07:49:05.194947 ontouml_json2graph-1.0.0b9/json2graph/modules/errors.py
+-rw-r--r--   0        0        0      684 2023-08-03 07:49:05.267243 ontouml_json2graph-1.0.0b9/json2graph/modules/globals.py
+-rw-r--r--   0        0        0     3462 2023-08-03 07:52:17.471425 ontouml_json2graph-1.0.0b9/json2graph/modules/input_output.py
+-rw-r--r--   0        0        0     2642 2023-08-02 10:46:56.193417 ontouml_json2graph-1.0.0b9/json2graph/modules/logger.py
+-rw-r--r--   0        0        0     7236 2023-08-03 07:50:35.792940 ontouml_json2graph-1.0.0b9/json2graph/modules/messages.py
+-rw-r--r--   0        0        0      878 2023-08-02 10:46:56.194418 ontouml_json2graph-1.0.0b9/json2graph/modules/sparql_queries.py
+-rw-r--r--   0        0        0     1486 2023-08-02 10:46:56.195420 ontouml_json2graph-1.0.0b9/json2graph/modules/utils_general.py
+-rw-r--r--   0        0        0     3667 2023-08-03 07:52:17.535428 ontouml_json2graph-1.0.0b9/json2graph/modules/utils_graph.py
+-rw-r--r--   0        0        0    84660 2023-08-02 10:46:56.196419 ontouml_json2graph-1.0.0b9/json2graph/resources/logo-json2graph.png
+-rw-r--r--   0        0        0    18036 2023-08-02 10:46:56.198417 ontouml_json2graph-1.0.0b9/json2graph/resources/ontouml_v100.ttl
+-rw-r--r--   0        0        0    78196 2023-08-02 10:46:56.199418 ontouml_json2graph-1.0.0b9/json2graph/resources/ontouml_v110.ttl
+-rw-r--r--   0        0        0    11558 2023-08-01 15:24:11.470721 ontouml_json2graph-1.0.0b9/LICENSE
+-rw-r--r--   0        0        0      909 2023-08-03 08:00:53.002856 ontouml_json2graph-1.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0     7289 2023-08-03 07:26:16.856872 ontouml_json2graph-1.0.0b9/README.md
+-rw-r--r--   0        0        0     8028 1970-01-01 00:00:00.000000 ontouml_json2graph-1.0.0b9/PKG-INFO
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/__main__.py` & `ontouml_json2graph-1.0.0b9/json2graph/__main__.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/main_decode.py` & `ontouml_json2graph-1.0.0b9/json2graph/main_decode.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/arguments.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/arguments.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_general.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_general.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ General decoding functions. """
 
-import modules.arguments as args
-from modules.logger import initialize_logger
-from modules.sparql_queries import GET_ELEMENT_AND_TYPE
-from modules.utils_graph import load_ontouml_vocabulary, ontouml_ref
 from rdflib import Graph, URIRef, Literal, RDF
 
+from .. import arguments as args
+from ..logger import initialize_logger
+from ..sparql_queries import GET_ELEMENT_AND_TYPE
+from ..utils_graph import load_ontouml_vocabulary, ontouml_ref
+
 LOGGER = initialize_logger()
 
 
 def create_point(point_id: str, x_coord: int, y_coord: int, ontouml_graph: Graph) -> None:
     """ Creates a new instance of ontouml:Point with its ontouml:xCoordinate, and ontouml:yCoordinate properties.
 
     :param point_id: ID of the new ontouml:Point instance to be created.
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_main.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """ JSON decode functions."""
 
-import modules.arguments as args
-from modules.decoder.decode_general import clean_null_data, count_elements_graph
-from modules.decoder.decode_obj_class import create_class_properties
-from modules.decoder.decode_obj_diagram import create_diagram_properties
-from modules.decoder.decode_obj_elementview import create_elementview_properties
-from modules.decoder.decode_obj_generalization import create_generalization_properties
-from modules.decoder.decode_obj_generalizationset import create_generalizationset_properties
-from modules.decoder.decode_obj_package import create_package_properties
-from modules.decoder.decode_obj_path import create_path_properties
-from modules.decoder.decode_obj_project import create_project_properties
-from modules.decoder.decode_obj_property import create_property_properties
-from modules.decoder.decode_obj_rectangularshape import create_rectangularshape_properties
-from modules.decoder.decode_obj_relation import create_relation_properties
-from modules.globals import METADATA, ELEMENT_VIEW_TYPES
-from modules.logger import initialize_logger
-from modules.utils_general import get_date_time
-from modules.utils_graph import ontouml_ref
 from rdflib import Graph, URIRef, Literal, RDF, XSD, OWL, RDFS
 
+from .. import arguments as args
+from ..decoder.decode_general import clean_null_data, count_elements_graph
+from ..decoder.decode_obj_class import create_class_properties
+from ..decoder.decode_obj_diagram import create_diagram_properties
+from ..decoder.decode_obj_elementview import create_elementview_properties
+from ..decoder.decode_obj_generalization import create_generalization_properties
+from ..decoder.decode_obj_generalizationset import create_generalizationset_properties
+from ..decoder.decode_obj_package import create_package_properties
+from ..decoder.decode_obj_path import create_path_properties
+from ..decoder.decode_obj_project import create_project_properties
+from ..decoder.decode_obj_property import create_property_properties
+from ..decoder.decode_obj_rectangularshape import create_rectangularshape_properties
+from ..decoder.decode_obj_relation import create_relation_properties
+from ..globals import METADATA, ELEMENT_VIEW_TYPES
+from ..logger import initialize_logger
+from ..utils_general import get_date_time
+from ..utils_graph import ontouml_ref
+
 LOGGER = initialize_logger()
 
 
 def add_metadata(ontouml_graph: Graph) -> None:
     """ Adds basic metadata to the generated graph when not in test mode. The metadata added are:
         - dct:conformsTo METADATA["conformsToBase"]
         - dct:created (creation date)
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_class.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,22 @@
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
 """
 
 import inspect
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, get_stereotype
-from modules.errors import report_error_end_of_switch
-from modules.messages import print_decode_log_message
-from modules.utils_graph import ontouml_ref
 from rdflib import Graph, URIRef, XSD, Literal
 
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type, get_stereotype
+from ..errors import report_error_end_of_switch
+from ..messages import print_decode_log_message
+from ..utils_graph import ontouml_ref
+
 
 def validate_class_attribute_constraints(class_dict: dict) -> None:
     """ Verifies all Class dictionaries and check if the constraints related to classes were correctly considered and
     fixes them when they are not.
 
     The pair of attribute/stereotype: isExtensional/collective and isPowertype/type checked constraints are:
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_diagram.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_diagram.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,21 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
-from modules.globals import ELEMENT_VIEW_TYPES
-from modules.utils_graph import ontouml_ref
 from rdflib import Graph, URIRef
 
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
+from ..globals import ELEMENT_VIEW_TYPES
+from ..utils_graph import ontouml_ref
+
 
 def set_diagram_owner_modelelement(diagram_dict: dict, ontouml_graph: Graph) -> None:
     """ Set the ontouml:owner property between an ontouml:Diagram and its related ontouml:Package.
 
     :param diagram_dict: Diagram object loaded as a dictionary.
     :type diagram_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_elementview.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_elementview.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,22 @@
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 import inspect
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
-from modules.errors import report_error_end_of_switch
-from modules.globals import ELEMENT_VIEW_TYPES
-from modules.utils_graph import ontouml_ref
 from rdflib import Graph, URIRef
 
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
+from ..errors import report_error_end_of_switch
+from ..globals import ELEMENT_VIEW_TYPES
+from ..utils_graph import ontouml_ref
+
 
 def set_elementview_relations(elementview_dict: dict, ontouml_graph: Graph) -> None:
     """ Set an ontouml:ElementView's ontouml:shape and ontouml:isViewOf object properties in the resulting graph.
 
     :param elementview_dict: ElementView object loaded as a dictionary.
     :type elementview_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_generalization.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_generalization.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,20 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
-from modules.utils_graph import ontouml_ref
 from rdflib import Graph, URIRef
 
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
+from ..utils_graph import ontouml_ref
+
 
 def set_generalization_relations(generalization_dict: dict, ontouml_graph: Graph) -> None:
     """ Set the ontouml:general and ontouml:specific properties in the resulting graph.
 
     :param generalization_dict: Generalization object loaded as a dictionary.
     :type generalization_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_generalizationset.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_generalizationset.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,21 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
-from modules.messages import print_decode_log_message
-from modules.utils_graph import ontouml_ref
 from rdflib import Graph, URIRef, Literal, XSD
 
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
+from ..messages import print_decode_log_message
+from ..utils_graph import ontouml_ref
+
 
 def set_generalizationset_defaults(generalizationset_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets the default values to ontouml:generalizationSets to the resulting graph.
 
     - Default isDisjoint: If isDisjoint is null, set as False.
     - Default isComplete: If isComplete is null, set as False.
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_package.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_package.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,20 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
-from modules.utils_graph import ontouml_ref
 from rdflib import Graph, URIRef
 
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
+from ..utils_graph import ontouml_ref
+
 
 def get_package_contents(package_dict: dict, package_id: str, list_contents: list = []) -> list[dict]:
     """ Receives the dictionary with all loaded JSON data and returns the value of the 'contents' field for a given
     object (defined by the received value of its ID).
 
     :param package_dict: Package's data to have its fields decoded.
     :type package_dict: dict
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_path.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_path.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,20 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, create_point
-from modules.utils_graph import ontouml_ref
 from rdflib import Graph, URIRef
 
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type, create_point
+from ..utils_graph import ontouml_ref
+
 
 def set_path_path_point(path_dict: dict, ontouml_graph: Graph) -> None:
     """ Creates an ontouml:Point, their properties and the ontouml:point of an ontouml:Path.
 
     :param path_dict: Path object loaded as a dictionary.
     :type path_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_project.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,20 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_all_ids_of_specific_type, get_list_subdictionaries_for_specific_type
-from modules.utils_graph import ontouml_ref
 from rdflib import Graph, URIRef
 
+from .. import arguments as args
+from ..decoder.decode_general import get_all_ids_of_specific_type, get_list_subdictionaries_for_specific_type
+from ..utils_graph import ontouml_ref
+
 
 def set_ontoumlelement_project_project(project_dict: dict, ontouml_graph: Graph, element_counting: dict) -> None:
     """ Sets the ontouml:project object property between an ontouml:Project (obj) and all its related entities (subj).
 
     :param project_dict: Project's data to have its fields decoded.
     :type project_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_property.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_property.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,23 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
-from modules.logger import initialize_logger
-from modules.messages import print_decode_log_message
-from modules.sparql_queries import GET_CLASS_STEREOTYPE_ATTRIBUTE_STEREOTYPE
-from modules.utils_graph import load_ontouml_vocabulary, ontouml_ref
 from rdflib import Graph, URIRef, RDF, Literal, XSD
 
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
+from ..logger import initialize_logger
+from ..messages import print_decode_log_message
+from ..sparql_queries import GET_CLASS_STEREOTYPE_ATTRIBUTE_STEREOTYPE
+from ..utils_graph import load_ontouml_vocabulary, ontouml_ref
+
 LOGGER = initialize_logger()
 
 
 def validate_property_stereotype(ontouml_graph: Graph) -> None:
     """ Performs syntactical and semantic validations on an ontouml:Property's stereotype.
 
     Differently from what is used in the validation of other JSON objects, this function manipulates the graph itself,
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_rectangularshape.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_rectangularshape.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,20 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, create_point
-from modules.utils_graph import ontouml_ref
 from rdflib import Graph, URIRef
 
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type, create_point
+from ..utils_graph import ontouml_ref
+
 
 def set_rectangularshape_coordinates(rectangularshape_dict: dict, ontouml_graph: Graph) -> None:
     """ Creates an ontouml:Point, their properties and the ontouml:topLeftPosition of an ontouml:RectangularShape.
 
     :param rectangularshape_dict: RectangularShape object loaded as a dictionary.
     :type rectangularshape_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/decoder/decode_obj_relation.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/decoder/decode_obj_relation.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,21 @@
     - Functions that set one property are named: set_<subject>_<predicate>_<object>.
     - Functions that set multiple object properties are named: set_<subject>_relations.
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, get_stereotype
-from modules.messages import print_decode_log_message
-from modules.utils_graph import ontouml_ref
 from rdflib import Graph, URIRef, Literal, XSD
 
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type, get_stereotype
+from ..messages import print_decode_log_message
+from ..utils_graph import ontouml_ref
+
 
 def set_relation_defaults(relation_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets the following attribute's default values for ontouml:Relation:
 
     DRA1) ontouml:isDerived default value = False
     DRA2) ontouml:isAbstract default value = False
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/errors.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Functions related to the verification and treatment of identified ERROR cases. """
 
-from modules.logger import initialize_logger
+from .logger import initialize_logger
 
 LOGGER = initialize_logger()
 
 
 def report_error_requirement_not_met(error_message: str) -> None:
     """ Reports the error caused when a requirement is not met. As this is a generic function, the error message
     parameter must be used to identify the error to the user.
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/globals.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/globals.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ Global variables definitions. """
 from os.path import exists
-from pprint import pprint
 
 import toml as toml
 
 # Software's metadata got from pyproject.toml config file
 global METADATA
 
 pyproject_file = "pyproject.toml"
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/input_output.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/input_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """ IO functions used in diverse occasions. """
 
 import json
 import os
 from pathlib import Path
 
-from modules.errors import report_error_io_read, report_error_io_write
-from modules.logger import initialize_logger
 from rdflib import Graph
 
+from .errors import report_error_io_read, report_error_io_write
+from .logger import initialize_logger
+
 LOGGER = initialize_logger()
 
 
 def create_directory_if_not_exists(directory_path: str, file_description: str) -> None:
     """ Checks if the directory that has the path received as argument exists.
     If it does, do nothing. If it does not, create it.
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/logger.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/logger.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/messages.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Decoding messages to be displayed to users must be concentrated in this module whenever possibile. """
 import inspect
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_stereotype
-from modules.errors import report_error_end_of_switch
-from modules.logger import initialize_logger
+from . import arguments as args
+from .decoder.decode_general import get_stereotype
+from .errors import report_error_end_of_switch
+from .logger import initialize_logger
 
 LOGGER = initialize_logger()
 
 
 def get_decode_log_message(object_dict: dict, warning_code: str, property_name: str,
                            att_valid_stereotype: str = "") -> str:
     """ Mounts and returns a warning message according to the information received as parameter.
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/sparql_queries.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/sparql_queries.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/utils_general.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/utils_general.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/modules/utils_graph.py` & `ontouml_json2graph-1.0.0b9/json2graph/modules/utils_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ Util functions related to graphs. """
 
-from modules.errors import report_error_io_read
-from modules.globals import METADATA
-from modules.logger import initialize_logger
 from rdflib import Graph, URIRef, RDF
 
+from .errors import report_error_io_read
+from .globals import METADATA
+from .logger import initialize_logger
+
 LOGGER = initialize_logger()
 
 
 def ontouml_ref(entity: str) -> URIRef:
     """ Receives the name of the OntoUML Vocabulary's entity as a string and returns the corresponding URIRef.
 
     :param entity: OntoUML Vocabulary entity (class, property, or individual) to have its URIRef returned.
```

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/resources/logo-json2graph.png` & `ontouml_json2graph-1.0.0b9/json2graph/resources/logo-json2graph.png`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/resources/ontouml_v100.ttl` & `ontouml_json2graph-1.0.0b9/json2graph/resources/ontouml_v100.ttl`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b8/json2graph/resources/ontouml_v110.ttl` & `ontouml_json2graph-1.0.0b9/json2graph/resources/ontouml_v110.ttl`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b8/LICENSE` & `ontouml_json2graph-1.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b8/pyproject.toml` & `ontouml_json2graph-1.0.0b9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ontouml-json2graph"
-version = "1.0.0b8"
+version = "1.0.0b9"
 description = "OntoUML JSON2Graph Decoder"
 license = "Apache-2.0"
 authors = ["Pedro Paulo F. Barcelos <p.p.favatobarcelos@utwente.nl>"]
 readme = "README.md"
 homepage = "https://w3id.org/ontouml/json2graph"
 repository = "https://w3id.org/ontouml/json2graph"
 documentation = "https://w3id.org/ontouml/json2graph/docs"
```

### Comparing `ontouml_json2graph-1.0.0b8/README.md` & `ontouml_json2graph-1.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b8/PKG-INFO` & `ontouml_json2graph-1.0.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontouml-json2graph
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: OntoUML JSON2Graph Decoder
 Home-page: https://w3id.org/ontouml/json2graph
 License: Apache-2.0
 Keywords: semantic-web,knowledge-graph,ontouml,ontology-driven-development,ontouml-schema,ontouml-vocabulary,ontouml-metamodel
 Author: Pedro Paulo F. Barcelos
 Author-email: p.p.favatobarcelos@utwente.nl
 Requires-Python: >=3.11,<4.0
```

