# Comparing `tmp/bmt-1.1.0.tar.gz` & `tmp/bmt-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmt-1.1.0.tar", max compression
+gzip compressed data, was "bmt-1.1.1.tar", max compression
```

## Comparing `bmt-1.1.0.tar` & `bmt-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1544 2023-06-30 23:39:14.959893 bmt-1.1.0/LICENSE
--rw-r--r--   0        0        0     1110 2023-06-30 23:39:14.959893 bmt-1.1.0/README.md
--rw-r--r--   0        0        0       31 2023-06-30 23:39:14.959893 bmt-1.1.0/bmt/__init__.py
--rw-r--r--   0        0        0    57582 2023-06-30 23:39:14.959893 bmt-1.1.0/bmt/toolkit.py
--rw-r--r--   0        0        0     3843 2023-06-30 23:39:14.959893 bmt-1.1.0/bmt/utils.py
--rw-r--r--   0        0        0     1585 2023-06-30 23:39:34.332389 bmt-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2493 1970-01-01 00:00:00.000000 bmt-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1544 2023-08-03 00:47:04.278358 bmt-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1110 2023-08-03 00:47:04.278358 bmt-1.1.1/README.md
+-rw-r--r--   0        0        0       31 2023-08-03 00:47:04.278358 bmt-1.1.1/bmt/__init__.py
+-rw-r--r--   0        0        0    67422 2023-08-03 00:47:04.282358 bmt-1.1.1/bmt/toolkit.py
+-rw-r--r--   0        0        0     3843 2023-08-03 00:47:04.282358 bmt-1.1.1/bmt/utils.py
+-rw-r--r--   0        0        0     1585 2023-08-03 00:47:29.402673 bmt-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2493 1970-01-01 00:00:00.000000 bmt-1.1.1/PKG-INFO
```

### Comparing `bmt-1.1.0/LICENSE` & `bmt-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bmt-1.1.0/README.md` & `bmt-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bmt-1.1.0/bmt/toolkit.py` & `bmt-1.1.1/bmt/toolkit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import yaml
 import csv
 import deprecation
 import requests
 from functools import lru_cache, reduce
 
-from typing import List, Union, TextIO, Optional, Dict
+from typing import List, Union, TextIO, Optional, Dict, Set
 from linkml_runtime.utils.schemaview import SchemaView, Namespaces
 from linkml_runtime.linkml_model.meta import (
     SchemaDefinition,
     Element,
     ElementName,
     Definition,
     ClassDefinition,
@@ -17,16 +17,16 @@
 )
 from pprint import pprint
 from bmt.utils import format_element, parse_name
 
 Url = str
 Path = str
 
-REMOTE_PATH = "https://raw.githubusercontent.com/biolink/biolink-model/v3.5.0/biolink-model.yaml"
-PREDICATE_MAP = 'https://raw.githubusercontent.com/biolink/biolink-model/v3.5.0/predicate_mapping.yaml'
+REMOTE_PATH = "https://raw.githubusercontent.com/biolink/biolink-model/v3.5.3/biolink-model.yaml"
+PREDICATE_MAP = 'https://raw.githubusercontent.com/biolink/biolink-model/v3.5.3/predicate_mapping.yaml'
 
 
 NODE_PROPERTY = "node property"
 ASSOCIATION_SLOT = "association slot"
 RELATED_TO = "related to"
 
 CACHE_SIZE = 1024
@@ -175,30 +175,208 @@
         return self._format_all_elements(elements, formatted)
 
     @lru_cache(CACHE_SIZE)
     def get_all_associations(self, formatted: bool = False) -> List[str]:
         """
         Get all associations from Biolink Model.
 
-        This method returns a list containing all the classes
-        that are descendants of the class ``association``.
+        This method returns a list of names or (optionally) curies
+        designating classes that are descendants of the class ``association``.
 
         Parameters
         ----------
         formatted: bool
             Whether to format element names as CURIEs
 
         Returns
         -------
         List[str]
             A list of elements
 
         """
+        return self.get_descendants("association", formatted=formatted)
+
+    @lru_cache(CACHE_SIZE)
+    def get_all_descendants(self, name: str, formatted: bool = False) -> List[str]:
+        """
+        Gets all descendants of a given element by name,
+        including those found by following associated element mixins.
+
+        Parameters
+        ----------
+        name: str
+            String name of root element whose descendants are to be retrieved.
+        formatted: bool
+            Whether to format element names as CURIEs.
+
+        Returns
+        -------
+        List[str]
+            A list of elements
+
+        """
+        element: Element = self.get_element(name)
+        all_descendants: Set[str] = set()
+        for mixin in element.mixins:
+            all_descendants.update(self.get_descendants(mixin, formatted=formatted))
+        all_descendants.update(self.get_descendants(element.name, formatted=formatted))
+        return list(all_descendants)
+
+    def filter_values_on_slot(
+            self,
+            slot_values: List[str],
+            definition: SlotDefinition,
+            field: str
+    ) -> bool:
+        """
+
+        Parameters
+        ----------
+        slot_values: List[str]
+            List of slot values to be matched against target slot field values.
+        definition: SlotDefinition
+            Slot definition containing the embedded target field.
+        field: str
+            Name of embedded (slot) field rooting the tree of elements
+            against which the slot_values are to be matched.
+
+        Returns
+        -------
+        bool
+           Returns 'True' if any match is found for at least
+           one entry in the slot_values, against the target field values.
+
+        """
+        if field in definition:
+            value = definition[field]
+            if value:
+                value_set = self.get_all_descendants(value, formatted=True)
+                return any([entry in slot_values for entry in value_set])
+        return False
+
+    def match_slot_usage(self, element, slot: str, slot_values: List[str]) -> bool:
+        """
+        Match slot_values against expected slot_usage for
+        specified slot in specified (association) element.
+
+        Parameters
+        ----------
+        element: Element
+            Target element against which slot_usage is being assessed.
+        slot: str
+            Name of target slot in given element, against which slot_usage is being assessed.
+        slot_values: List[str]
+            List of slot value (strings) e.g. categories, predicates, etc. - being assessed against slot_usage
+
+        Returns
+        -------
+        bool
+            Returns 'True' if slot_values are compatible with slot usage within given element
+
+        """
+        # scope of method sanity check for now
+        assert slot in ["subject", "object", "predicate"]
+
+        slot_definition: Optional[SlotDefinition] = None
+
+        if "slot_usage" in element:
+            slot_usage = element["slot_usage"]
+            if slot_usage and slot in slot_usage:
+                slot_definition: SlotDefinition = slot_usage[slot]
+            elif "mixins" in element and element["mixins"]:
+                # 'slot_usage' for some fields may be inherited
+                # from the association mixins. For example:
+                #
+                #     druggable gene to disease association
+                #         mixins:
+                #         - entity to disease association mixin
+                #         - gene to entity association mixin
+                #
+                # the mixins would have a 'subject' slot_usage
+                # for Gene and 'object' usage for Disease
+                #
+                for mixin in element["mixins"]:
+                    mixin_element: Element = self.get_element(mixin)
+                    if "slot_usage" in mixin_element:
+                        slot_usage = mixin_element["slot_usage"]
+                        if slot_usage and slot in slot_usage:
+                            slot_definition: SlotDefinition = slot_usage[slot]
+                            break  # only need first one seen?
+
+        # assess "slot_values" for "subject", "object"
+        # or "predicate" against stipulated constraints
+        if slot_definition:
+            if slot == "predicate":
+                return self.filter_values_on_slot(slot_values, slot_definition, "subproperty_of")
+            else:  # filter on "subject" or "object" category
+                return self.filter_values_on_slot(slot_values, slot_definition, "range")
+
+        return False
+
+    def get_associations(
+            self,
+            subject_categories: Optional[List[str]] = None,
+            predicates: Optional[List[str]] = None,
+            object_categories: Optional[List[str]] = None,
+            formatted: bool = False
+    ) -> List[str]:
+        """
+        Get associations from Biolink Model constrained by
+        subject categories, predicates and/or object categories.
+
+        This method returns a list of names or (optionally) curies
+        designating classes that are descendants of the class ``association``.
+
+        Parameters
+        ----------
+        subject_categories: Optional[List[str]]
+            List of node categories (as CURIES) that the associations must match for the subject node; default: None
+        predicates: Optional[List[str]]
+            List of edge predicates (as CURIES) that the associations allowed for matching associations; default: None
+        object_categories: Optional[List[str]]
+            List of node categories (as CURIES) that the associations must match for the object node; default: None
+        formatted: bool
+            Whether to format element names as CURIEs; default: False
+
+        Returns
+        -------
+        List[str]
+            A list of elements
+
+        """
         elements = self.get_descendants("association")
-        return self._format_all_elements(elements, formatted)
+        filtered_elements: List[str] = list()
+        if subject_categories or predicates or object_categories:
+            # This feels like a bit of a brute force approach as an implementation,
+            # but we just use the list of all association names to retrieve each
+            # association record for filtering against the constraints?
+            for name in elements:
+                association: Optional[Element] = self.get_element(name)
+
+                # sanity checks, probably not necessary
+                # assert association, f"'{name}' not a Biolink Element?"
+                # assert isinstance(association, ClassDefinition), f"'{name}' not a ClassDefinition?"
+
+                if subject_categories:
+                    if not self.match_slot_usage(association, "subject", subject_categories):
+                        continue
+                if predicates:
+                    if not self.match_slot_usage(association, "predicate", predicates):
+                        continue
+                if object_categories:
+                    if not self.match_slot_usage(association, "object", object_categories):
+                        continue
+
+                # this association is assumed to pass stipulated constraints
+                filtered_elements.append(association.name)
+        else:
+            # no filtering equivalent to get_all_associations()
+            filtered_elements = elements
+
+        return self._format_all_elements(filtered_elements, formatted)
 
     @lru_cache(CACHE_SIZE)
     def get_all_node_properties(self, formatted: bool = False) -> List[str]:
         """
         Get all node properties from Biolink Model.
 
         This method returns a list containing all the slots
@@ -413,19 +591,19 @@
         Gets a list of names of descendants.
 
         Parameters
         ----------
         name: str
             The name of an element in the Biolink Model
         reflexive: bool
-            Whether to include the query element in the list of ancestors
+            Whether to include the query element in the list of descendants
         formatted: bool
             Whether to format element names as CURIEs
         mixin: bool
-            If True, then that means we want to find mixin ancestors as well as is_a ancestors
+            If True, then that means we want to find mixin descendants as well as is_a ancestors
 
         Returns
         -------
         List[str]
             The names of the given element's descendants
 
         """
@@ -699,45 +877,100 @@
                     if subject_in_domain and object_in_range:
                         return True
                 else:
                     return False
 
         return False
 
-    def validate_qualifier(self, qualifier_type_id: str, qualifier_value: str) -> bool:
+    def is_subproperty_of(self, predicate: str, name: str, formatted: bool = False) -> bool:
+        """
+        Checks if a given name is a 'subproperty_of' a given predicate.
+        Note: unsure if this method yet captures the full subtlety of 'subproperty_of'.
+
+        Parameters
+        ----------
+        predicate: str
+            Target predicate against which a given name is to be searched as a subproperty
+        name: str
+            Name to be searched
+        formatted: bool = False
+            Input name assumed to be a CURIE
+
+        Returns
+        -------
+            True if the name is observed to be equivalent to,
+            or a 'subproperty' descendant of, the given predicate.
+
+        """
+        return name in self.get_descendants(predicate, formatted=formatted)
+
+    def validate_qualifier(
+            self,
+            qualifier_type_id: str,
+            qualifier_value: str,
+            associations: Optional[List[str]] = None
+    ) -> bool:
         """
         Validates a qualifier.
 
         Parameters
         ----------
         qualifier_type_id: str
             The name or alias of a qualifier in the Biolink Model
         qualifier_value: str
             The value of the qualifier
+        associations: Optional[List[str]] = None
+            Optional list of possible biolink:Association subclass (CURIEs)
+            which could resolve the context for qualifier_value validation.
 
         Returns
         -------
         bool
             Whether or not the given qualifier is valid
 
         """
         if qualifier_type_id and qualifier_value and self.is_qualifier(qualifier_type_id):
+            qualifier_type_name = parse_name(qualifier_type_id)
             qualifier_slot = self.view.get_slot(parse_name(qualifier_type_id))
-            # slot may just be missing from the model or
-            # the range will be None for abstract/mixin qualifiers,
-            # or the range may be just plain missing from the model
-            if qualifier_slot and qualifier_slot.range is not None:
-                if self.is_enum(qualifier_slot.range):
-                    enum = self.view.get_enum(qualifier_slot.range)
-                    if self.is_permissible_value_of_enum(enum.name, qualifier_value):
-                        return True
-                else:  # possible Biolink categorical qualifier
-                    categories = self.get_element_by_prefix(qualifier_value)
-                    if categories and qualifier_slot.range in categories:
-                        return True
+            # qualifier slot may be undefined in the current model
+            if qualifier_slot:
+                value_range: Optional[str] = None
+                if "range" in qualifier_slot and qualifier_slot.range:
+                    value_range = qualifier_slot.range
+
+                # Perhaps the qualifier value range is defined
+                # within a biolink:Association subclass?
+                elif associations:
+                    for association in associations:
+                        association_element = self.get_element(association)
+                        if "slot_usage" in association_element and \
+                                qualifier_type_name in association_element["slot_usage"]:
+                            qualifier_type = association_element["slot_usage"][qualifier_type_name]
+                            if qualifier_type_name == "qualified predicate" and \
+                                    "subproperty_of" in qualifier_type and qualifier_type.subproperty_of:
+                                value_range = qualifier_type.subproperty_of
+
+                            elif "range" in qualifier_type and qualifier_type.range:
+                                value_range = qualifier_type.range
+                                break
+
+                # Else: the range may be missing from a particular model
+                # or the range will be None for abstract/mixin qualifiers?
+
+                if value_range:
+                    if qualifier_type_name == "qualified predicate":
+                        return self.is_subproperty_of(predicate=value_range, name=qualifier_value)
+                    elif self.is_enum(value_range):
+                        enum = self.view.get_enum(value_range)
+                        return self.is_permissible_value_of_enum(enum.name, qualifier_value)
+                    else:
+                        # The value range possibly may be a Biolink categorical qualifier
+                        categories = self.get_element_by_prefix(qualifier_value)
+                        return bool(categories and value_range in categories)
+
         return False
 
     def get_all_slots_with_class_domain(
             self,
             class_name,
             check_ancestors: bool = False,
             formatted: bool = False,
@@ -1553,14 +1786,15 @@
                 if mapping_index.get(identifier)[0] == 'related' and mapping_index.get(identifier)[1] == element:
                     formatted_element = format_element(element)
                     return [formatted_element]
                 else:
                     return []
         else:
             return []
+
     @lru_cache(CACHE_SIZE)
     def get_element_by_narrow_mapping(
             self, identifier: str, formatted: bool = False
     ) -> List[str]:
         """
         Given an identifier as IRI/CURIE, find a Biolink element that corresponds
         to the given identifier as part of its narrow_mappings.
```

### Comparing `bmt-1.1.0/bmt/utils.py` & `bmt-1.1.1/bmt/utils.py`

 * *Files identical despite different names*

### Comparing `bmt-1.1.0/pyproject.toml` & `bmt-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmt"
-version = "1.1.0"
+version = "1.1.1"
 description = "Biolink Model Toolkit: A Python API for working with the Biolink Model"
 authors = ["Sierra Taylor Moxon <sierra.taylor@gmail.com>"]
 license = "BSD"
 
 readme = "README.md"
 repository = "https://github.com/biolink/biolink-model-toolkit"
 documentation = "https://biolink.github.io/biolink-model-toolkit/"
```

### Comparing `bmt-1.1.0/PKG-INFO` & `bmt-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmt
-Version: 1.1.0
+Version: 1.1.1
 Summary: Biolink Model Toolkit: A Python API for working with the Biolink Model
 Home-page: https://github.com/biolink/biolink-model-toolkit
 License: BSD
 Keywords: schema,linked data,data modeling,biolink,api
 Author: Sierra Taylor Moxon
 Author-email: sierra.taylor@gmail.com
 Requires-Python: >=3.9,<4.0
```

