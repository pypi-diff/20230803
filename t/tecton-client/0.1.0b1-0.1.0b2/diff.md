# Comparing `tmp/tecton_client-0.1.0b1.tar.gz` & `tmp/tecton_client-0.1.0b2.tar.gz`

## Comparing `tecton_client-0.1.0b1.tar` & `tecton_client-0.1.0b2.tar`

### file list

```diff
@@ -1,42 +1,44 @@
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/requirements.txt
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/.github/pull_request_template.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/.github/workflows/testing.yml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/__init__.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/client_options.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/constants.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/data_types.py
--rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/exceptions.py
--rw-r--r--   0        0        0     9201 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/http_client.py
--rw-r--r--   0        0        0    21998 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/requests.py
--rw-r--r--   0        0        0    25179 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/responses.py
--rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/tecton_client.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tecton_client/utils.py
--rw-r--r--   0        0        0     7864 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/data_types_test.py
--rw-r--r--   0        0        0    10133 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/http_client_test.py
--rw-r--r--   0        0        0    18904 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/requests_test.py
--rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/responses_test.py
--rw-r--r--   0        0        0    15031 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/tecton_client_test.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_utils.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/batch/batch_expected_request_1.json
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/batch/batch_expected_request_2.json
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/batch/batch_expected_request_3.json
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/batch/batch_expected_request_4.json
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/batch/sample_batch_response.json
--rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/batch/sample_batch_response_long_slo.json
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/batch/sample_batch_response_slo.json
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response.json
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response_list.json
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response_long.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response_metadata.json
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response_mixed.json
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response_null.json
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response_slo.json
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/tests/test_data/single/sample_response_struct.json
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/.gitignore
--rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/LICENSE.md
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/README.md
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 tecton_client-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/requirements.txt
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/.github/pull_request_template.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/.github/workflows/testing.yml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tecton_client/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tecton_client/__init__.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tecton_client/client_options.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tecton_client/constants.py
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tecton_client/data_types.py
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tecton_client/exceptions.py
+-rw-r--r--   0        0        0     9201 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tecton_client/http_client.py
+-rw-r--r--   0        0        0    22817 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tecton_client/requests.py
+-rw-r--r--   0        0        0    28219 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tecton_client/responses.py
+-rw-r--r--   0        0        0    17149 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tecton_client/tecton_client.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tecton_client/utils.py
+-rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/data_types_test.py
+-rw-r--r--   0        0        0    10133 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/http_client_test.py
+-rw-r--r--   0        0        0    18314 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/requests_test.py
+-rw-r--r--   0        0        0    19649 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/responses_test.py
+-rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/tecton_client_test.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_utils.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/sample_metadata_response.json
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/sample_metadata_response_long.json
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/batch/batch_expected_request_1.json
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/batch/batch_expected_request_2.json
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/batch/batch_expected_request_3.json
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/batch/batch_expected_request_4.json
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/batch/sample_batch_response.json
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/batch/sample_batch_response_long_slo.json
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/batch/sample_batch_response_slo.json
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/single/sample_response.json
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/single/sample_response_list.json
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/single/sample_response_long.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/single/sample_response_metadata.json
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/single/sample_response_mixed.json
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/single/sample_response_null.json
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/single/sample_response_slo.json
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/tests/test_data/single/sample_response_struct.json
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/.gitignore
+-rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/LICENSE.md
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/README.md
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 tecton_client-0.1.0b2/PKG-INFO
```

### Comparing `tecton_client-0.1.0b1/.pre-commit-config.yaml` & `tecton_client-0.1.0b2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/.github/workflows/testing.yml` & `tecton_client-0.1.0b2/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tecton_client/client_options.py` & `tecton_client-0.1.0b2/tecton_client/client_options.py`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tecton_client/data_types.py` & `tecton_client-0.1.0b2/tecton_client/data_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import abc
+from dataclasses import dataclass
 from typing import List
 from typing import Optional
 
 from tecton_client.exceptions import TectonClientError
 
 
 class DataType(abc.ABC):
@@ -95,15 +96,15 @@
 
     @property
     def data_type(self) -> DataType:
         """Return the :class:`DataType` of the field."""
         return self._data_type
 
     def __str__(self) -> str:
-        return f"Field({self._name}, {self._data_type})"
+        return f'Field("{self._name}", {self._data_type})'
 
 
 class StructType(DataType):
     """Class to represent datatype Struct.
 
     A :class:`StructType` object represents a struct datatype, consisting of multiple fields.
 
@@ -191,7 +192,15 @@
             raise TectonClientError(message)
     else:
         message = (
             f"Received unknown data type {data_type} in the response."
             f"If problem persists, please contact Tecton Support for assistance."
         )
         raise TectonClientError(message)
+
+
+@dataclass
+class NameAndType:
+    """Class to represent a name and data type pair."""
+
+    name: str
+    data_type: DataType
```

### Comparing `tecton_client-0.1.0b1/tecton_client/exceptions.py` & `tecton_client-0.1.0b2/tecton_client/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -110,70 +110,49 @@
         return (
             f"{map_type} values can only be of types {allowed_types}. "
             f"Given value for {map_type} is {value} of type {type(value)}"
         )
 
 
 class BadRequestError(TectonServerException):
-    """Raised when the Tecton API returns a 400 Bad Request error.
-
-    Please refer to the message for more details on the error.
-    """
+    """Raised when the Tecton API returns a 400 Bad Request error."""
 
     STATUS_CODE = 400
 
 
 class UnauthorizedError(TectonServerException):
-    """Raised when the Tecton API returns a 401 Unauthorized error.
-
-    Please refer to the message for more details on the error.
-    """
+    """Raised when the Tecton API returns a 401 Unauthorized error."""
 
     STATUS_CODE = 401
 
 
 class ForbiddenError(TectonServerException):
-    """Raised when the Tecton API returns a 403 Forbidden error.
-
-    Please refer to the message for more details on the error.
-    """
+    """Raised when the Tecton API returns a 403 Forbidden error."""
 
     STATUS_CODE = 403
 
 
 class NotFoundError(TectonServerException):
-    """Raised when the Tecton API returns a 404 Not Found error.
-
-    Please refer to the message for more details on the error.
-    """
+    """Raised when the Tecton API returns a 404 Not Found error."""
 
     STATUS_CODE = 404
 
 
-class ResourcesExhaustedError(TectonServerException):
-    """Raised when the Tecton API returns a 429 Resources Exhausted error.
-
-    Please refer to the message for more details on the error.
-    """
+class ResourceExhaustedError(TectonServerException):
+    """Raised when the Tecton API returns a 429 Resources Exhausted error."""
 
     STATUS_CODE = 429
 
 
 class ServiceUnavailableError(TectonServerException):
-    """Raised when the Tecton API returns a 503 Service Unavailable error.
-
-    Please refer to the message for more details on the error.
-    """
+    """Raised when the Tecton API returns a 503 Service Unavailable error."""
 
     STATUS_CODE = 503
 
 
 class GatewayTimeoutError(TectonServerException):
-    """Raised when the Tecton API returns a 504 Gateway Timeout error.
-
-    Please refer to the message for more details on the error.
-    """
+    """Raised when the Tecton API returns a 504 Gateway Timeout error."""
 
     STATUS_CODE = 504
 
 
 SERVER_ERRORS: dict = {error.STATUS_CODE: error for error in TectonServerException.__subclasses__()}
```

### Comparing `tecton_client-0.1.0b1/tecton_client/http_client.py` & `tecton_client-0.1.0b2/tecton_client/http_client.py`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tecton_client/requests.py` & `tecton_client-0.1.0b2/tecton_client/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Final
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Union
 
 from tecton_client.constants import DEFAULT_MICRO_BATCH_SIZE
-from tecton_client.constants import DEFAULT_WORKSPACE_NAME
 from tecton_client.constants import MAX_MICRO_BATCH_SIZE
 from tecton_client.constants import MIN_MICRO_BATCH_SIZE
 from tecton_client.constants import SUPPORTED_JOIN_KEY_VALUE_TYPES
 from tecton_client.constants import SUPPORTED_REQUEST_CONTEXT_MAP_TYPES
 from tecton_client.exceptions import EMPTY_KEY_VALUE
 from tecton_client.exceptions import INVALID_TYPE_KEY_VALUE
 from tecton_client.exceptions import InvalidMicroBatchSizeError
@@ -33,15 +32,15 @@
     EFFECTIVE_TIME = "include_effective_times"
     """Include the timestamp of the most recent feature value that was written to the online store"""
 
     DATA_TYPE = "include_data_types"
     """Include the data types of each feature in the vector"""
 
     SLO_INFO = "include_slo_info"
-    """Include information about the server response time"""
+    """Include SLO information in the response"""
 
     FEATURE_STATUS = "include_serving_status"
     """Include feature serving status information of the feature"""
 
 
 def _defaults() -> Set[MetadataOptions]:
     """Set the default options to include names and data types.
@@ -65,14 +64,19 @@
                     For int keys, the value should be a string of the decimal representation of the integer.
         request_context_map (Optional[Dict[str, Union[int, str, float]]]):
             Request context used for OnDemand FeatureViews.
             The Request Context values can be of type (int, str, float) and are encoded as follows:
                     For string values, the value should be a string.
                     For int values, the value should be a string of the decimal representation of the integer.
                     For float values, the value should be a number.
+
+    Examples:
+        >>> join_key_map = {"sample_key": "sample_value"}
+        >>> request_context_map = {"example_key_1": "example_value_1", "example_key_2": "example_value_2"}
+        >>> data = GetFeaturesRequestData(join_key_map=join_key_map, request_context_map=request_context_map)
     """
 
     def __init__(
         self,
         join_key_map: Optional[Dict[str, Union[int, str, type(None)]]] = None,
         request_context_map: Optional[Dict[str, Union[int, str, float]]] = None,
     ) -> None:
@@ -107,14 +111,18 @@
             self._get_processed_map(
                 request_context_map, False, SUPPORTED_REQUEST_CONTEXT_MAP_TYPES, map_type="Request Context Map"
             )
             if request_context_map
             else None
         )
 
+    def __str__(self) -> str:
+        """Returns a string representation of the request data."""
+        return f"GetFeaturesRequestData({vars(self)})"
+
     @staticmethod
     def _get_processed_map(request_map: dict, allow_none: bool, allowed_types: set, map_type: str) -> dict:
         """Validates the parameters of the request.
 
         Args:
             request_map (dict): The map to validate.
             allow_none (bool): Whether the map allows None values or not.
@@ -206,44 +214,43 @@
                 values. Defaults to the default set of metadata options.
 
         """
         super().__init__(workspace_name, feature_service_name)
         self.metadata_options = metadata_options.union(_defaults())
 
 
-def _request_to_json(request: TectonRequest, fields_to_remove: List[str], request_type: str) -> dict:
+def _request_to_json(request: TectonRequest, fields_to_remove: List[str]) -> dict:
     """Returns a JSON representation of any :class:`TectonRequest` object as a dictionary.
 
     Args:
         request (TectonRequest): The :class:`TectonRequest` object to be converted to JSON.
         fields_to_remove (List[str]): List of fields to be removed from the JSON representation of the object.
-        request_type (str): Whether the request is a single get-features request, batch request or metadata request.
 
     Returns:
         dict: The JSON representation of the :class:`AbstractGetFeaturesRequest` object.
 
     """
     self_dict = {key: value for key, value in vars(request).items() if key not in fields_to_remove}
 
-    if request_type != "metadata":
+    if isinstance(request, AbstractGetFeaturesRequest):
         self_dict["metadata_options"] = (
             {option.value: True for option in sorted(request.metadata_options, key=lambda x: x.value)}
             if request.metadata_options
             else {}
         )
-        if request_type == "batch":
-            self_dict["request_data"] = [
-                {k: v for k, v in vars(request_data).items() if v} for request_data in request.request_data
-            ]
-        elif request_type == "single":
+        if isinstance(request, GetFeaturesRequest):
             if request.request_data.join_key_map:
                 self_dict["join_key_map"] = request.request_data.join_key_map
             if request.request_data.request_context_map:
                 self_dict["request_context_map"] = request.request_data.request_context_map
 
+        elif isinstance(request, GetFeaturesMicroBatchRequest):
+            self_dict["request_data"] = [
+                {k: v for k, v in vars(request_data).items() if v} for request_data in request.request_data
+            ]
     return {"params": self_dict}
 
 
 @dataclass
 class GetFeaturesRequest(AbstractGetFeaturesRequest):
     """Class representing a request to the /get-features endpoint.
 
@@ -276,19 +283,29 @@
             feature_service_name (str): Name of the Feature Service for which the feature vector is being requested.
             request_data (GetFeaturesRequestData): Request parameters for the query.
             metadata_options (Set[MetadataOptions]): Options for retrieving additional metadata about feature
                 values.
 
         """
         super().__init__(workspace_name, feature_service_name, metadata_options)
-        self.request_data = request_data
+        if request_data:
+            self.request_data = request_data
+        else:
+            message = "Request Data cannot be empty or None."
+            raise InvalidParameterError(message)
 
     def to_json(self) -> dict:
         """Returns a JSON representation of the :class:`GetFeaturesRequest` object as a dictionary."""
-        return _request_to_json(self, fields_to_remove=["ENDPOINT", "request_data"], request_type="single")
+        return _request_to_json(self, fields_to_remove=["ENDPOINT", "request_data"])
+
+    def __str__(self) -> str:
+        """Returns a string representation of the :class:`GetFeaturesRequest` object."""
+        string_representation = vars(self)
+        string_representation["request_data"] = self.request_data.__str__()
+        return f"GetFeaturesRequest({string_representation})"
 
 
 @dataclass
 class GetFeaturesMicroBatchRequest(AbstractGetFeaturesRequest):
     """Class representing a micro-batch request sent to the /get-features-batch endpoint.
 
     Attributes:
@@ -317,15 +334,15 @@
 
         """
         super().__init__(workspace_name, feature_service_name, metadata_options)
         self.request_data = request_data_list
 
     def to_json(self) -> dict:
         """Returns a JSON representation of the :class:`GetFeaturesMicroBatchRequest` object as a dictionary."""
-        return _request_to_json(self, fields_to_remove=["ENDPOINT"], request_type="batch")
+        return _request_to_json(self, fields_to_remove=["ENDPOINT"])
 
 
 @dataclass
 class GetFeaturesBatchRequest(AbstractGetFeaturesRequest):
     """A class that represents a batch request to retrieve a list of feature vectors from the feature server.
 
     The class can be used to make parallel requests to retrieve multiple feature vectors from the feature server API.
@@ -345,17 +362,16 @@
     of `k` where `k` is in the range [|MIN_MICRO_BATCH_SIZE|, |MAX_MICRO_BATCH_SIZE|], the client enqueues
     math.ceil(n/k) microbatch requests to be sent parallelly to the /get-features-batch endpoint, waits until all
     microbatch requests are complete or a specific time has elapsed and returns a List of :class:`GetFeaturesResponse`
     objects of size `n`.
 
 
     Attributes:
-        request_list (List[Union[GetFeaturesRequest, GetFeaturesMicroBatchRequest]]): List of
-            :class:`GetFeaturesRequest` objects or :class:`GetFeaturesMicroBatchRequest` objects, based on the
-            `micro_batch_size` configuration.
+        request_list (List[AbstractGetFeaturesRequest]): List of
+            :class:`AbstractGetFeaturesRequest` objects, based on the `micro_batch_size` configuration.
         ENDPOINT (str): Endpoint string for the get-features-batch API.
 
     Examples:
         >>> request_data = GetFeaturesRequestData(join_key_map={"user_id": 1234})
         >>> request = GetFeaturesBatchRequest(
         ...      workspace_name="my_workspace",
         ...      feature_service_name="my_feature_service",
@@ -442,35 +458,39 @@
         if micro_batch_size < MIN_MICRO_BATCH_SIZE or micro_batch_size > MAX_MICRO_BATCH_SIZE:
             raise InvalidMicroBatchSizeError
 
     def to_json_list(self) -> List[dict]:
         """Returns a list of JSON representations for requests in the object as a list of dictionaries."""
         return [request.to_json() for request in self.request_list]
 
+    def __str__(self) -> str:
+        """Returns a string representation of the :class:`GetFeaturesBatchRequest` object."""
+        string_representation = vars(self)
+        string_representation["request_list"] = [str(request) for request in self.request_list]
+        return f"GetFeaturesBatchRequest({string_representation})"
+
 
 @dataclass
 class GetFeatureServiceMetadataRequest(TectonRequest):
     """Class representing a request to the /feature-service-metadata endpoint.
 
     Attributes:
         ENDPOINT (str): Endpoint string for the feature-service/metadata API.
 
     """
 
     ENDPOINT: Final[str] = "/api/v1/feature-service/metadata"
 
-    def __init__(self, feature_service_name: str, workspace_name: str = DEFAULT_WORKSPACE_NAME) -> None:
+    def __init__(self, feature_service_name: str, workspace_name: str) -> None:
         """Initializing the :class:`GetFeatureServiceMetadataRequest` object with the given parameters.
 
         Args:
-            feature_service_name (str): Name of the Feature Service for which the feature vector is being requested.
+            feature_service_name (str): Name of the Feature Service for which the metadata is being requested.
             workspace_name (str): Name of the workspace in which the Feature Service is defined,
                 defaults to {DEFAULT_WORKSPACE_NAME}.
 
         """
-        if not workspace_name:
-            workspace_name = DEFAULT_WORKSPACE_NAME
         super().__init__(workspace_name=workspace_name, feature_service_name=feature_service_name)
 
     def to_json(self) -> dict:
         """Returns a JSON representation of the :class:`GetFeatureServiceMetadataRequest` object as a dictionary."""
-        return _request_to_json(self, fields_to_remove=["ENDPOINT"], request_type="metadata")
+        return _request_to_json(self, fields_to_remove=["ENDPOINT"])
```

### Comparing `tecton_client-0.1.0b1/tecton_client/responses.py` & `tecton_client-0.1.0b2/tecton_client/responses.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from tecton_client.constants import MAX_MICRO_BATCH_SIZE
 from tecton_client.data_types import ArrayType
 from tecton_client.data_types import BoolType
 from tecton_client.data_types import DataType
 from tecton_client.data_types import FloatType
 from tecton_client.data_types import get_data_type
 from tecton_client.data_types import IntType
+from tecton_client.data_types import NameAndType
 from tecton_client.data_types import StringType
 from tecton_client.data_types import StructType
 from tecton_client.exceptions import InvalidMicroBatchSizeError
 from tecton_client.exceptions import TectonClientError
 from tecton_client.http_client import HTTPResponse
 from tecton_client.utils import parse_string_to_isotime
 
@@ -163,14 +164,18 @@
         if effective_time and not self.effective_time:
             message = f"Invalid datetime string: {effective_time}. Please contact Tecton Support for assistance."
             raise TectonClientError(message)
 
         self.data_type = get_data_type(data_type, element_type, fields)
         self.feature_value = Value(self.data_type, feature_value).value
 
+    def __str__(self) -> str:
+        """Return a string representation of the FeatureValue object."""
+        return f"{self.feature_namespace}.{self.feature_name}: {self.feature_value}"
+
 
 class SloIneligibilityReason(str, Enum):
     """Reasons due to which the Feature Serving Response may be ineligible for SLO."""
 
     UNKNOWN = "UNKNOWN"
     """Reason is unknown."""
 
@@ -516,7 +521,72 @@
                 "sloEligible": is_slo_eligible_batch,
                 "sloServerTimeSeconds": max_slo_server_time_seconds,
                 "storeMaxLatency": max_store_max_latency,
                 "serverTimeSeconds": max_server_time_seconds,
                 "sloIneligibilityReasons": batch_slo_ineligibility_reasons,
             }
         )
+
+
+def _parse_metadata_to_name_type_dict(response_dict: dict) -> Dict[str, NameAndType]:
+    """Parse the returned metadata information to a list of :class:`NameAndType` objects.
+
+    Args:
+        response_dict (dict): The response dictionary returned from the server containing metadata information.
+
+    Returns:
+        Dict[str, NameAndType]: Dictionary of names mapping to :class:`NameAndType` objects.
+
+    """
+    return {
+        key["name"]: NameAndType(
+            name=key.get("name"),
+            data_type=get_data_type(
+                data_type=key["dataType"].get("type"),
+                element_type=key["dataType"].get("elementType"),
+                fields=key["dataType"].get("fields"),
+            ),
+        )
+        for key in response_dict
+    }
+
+
+class FeatureServiceType(str, Enum):
+    """Enum to represent the type of the feature service."""
+
+    DEFAULT = "DEFAULT"
+    """The feature service is a default feature service."""
+
+    WILDCARD = "WILDCARD"
+    """The feature service is a wildcard feature service."""
+
+
+class GetFeatureServiceMetadataResponse:
+    """Response object for GetFeatureServiceMetadata API call.
+
+    Attributes:
+        feature_service_type (FeatureServiceType): The type of the feature service.
+        input_join_keys (Dict[str, NameAndType]): Dictionary of names mapping to :class:`NameAndType` objects
+            representing the input join keys.
+        input_request_context_keys (Dict[str, NameAndType]): Dictionary of names mapping to :class:`NameAndType` objects
+            representing the input request context keys.
+        feature_values (Dict[str, NameAndType]): Dictionary of names mapping to :class:`NameAndType` objects
+            representing the feature values.
+        output_join_keys (Dict[str, NameAndType]): Dictionary of names mapping to :class:`NameAndType` objects
+            representing the output join keys.
+    """
+
+    def __init__(self, http_response: HTTPResponse) -> None:
+        """Initializes the object with data from the response.
+
+        Args:
+            http_response (HTTPResponse): The HTTP response object returned from the GetFeatureServiceMetadata API call.
+
+        """
+        response = http_response.result
+        self.feature_service_type = (
+            FeatureServiceType(response["featureServiceType"]) if response.get("featureServiceType") else None
+        )
+        self.input_join_keys = _parse_metadata_to_name_type_dict(response.get("inputJoinKeys", {}))
+        self.input_request_context_keys = _parse_metadata_to_name_type_dict(response.get("inputRequestContextKeys", {}))
+        self.feature_values = _parse_metadata_to_name_type_dict(response.get("featureValues", {}))
+        self.output_join_keys = _parse_metadata_to_name_type_dict(response.get("outputJoinKeys", {}))
```

### Comparing `tecton_client-0.1.0b1/tecton_client/tecton_client.py` & `tecton_client-0.1.0b2/tecton_client/tecton_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 
 from tecton_client.client_options import TectonClientOptions
 from tecton_client.exceptions import InvalidParameterError
 from tecton_client.exceptions import InvalidParameterMessage
 from tecton_client.http_client import HTTPRequest
 from tecton_client.http_client import TectonHttpClient
 from tecton_client.requests import GetFeaturesBatchRequest
+from tecton_client.requests import GetFeatureServiceMetadataRequest
 from tecton_client.requests import GetFeaturesRequest
 from tecton_client.responses import GetFeaturesBatchResponse
+from tecton_client.responses import GetFeatureServiceMetadataResponse
 from tecton_client.responses import GetFeaturesResponse
 from tecton_client.utils import asyncio_run
 
 
 class TectonClient:
     """Class to represent a Tecton Client.
 
@@ -110,15 +112,15 @@
             ForbiddenError: If the response returned from the Tecton Server is 403 Forbidden, it could be because the
                 Service Account associated with your API Key does not have the necessary permissions to query
                 the feature service. Please refer to the `Tecton Documentation <https://docs.tecton.ai/docs/beta/\
                 reading-feature-data/reading-feature-data-for-inference/reading-online-features-for-inference-using-\
                 the-http-api#creating-an-api-key-to-authenticate-to-the-http-api>`_ for more information.
             NotFoundError: If the response returned from the Tecton Server is 404 Not Found. Please check the exception
                 message for detailed information.
-            ResourcesExhaustedError: If the response returned from the Tecton Server is 429 Resources Exhausted. Some
+            ResourceExhaustedError: If the response returned from the Tecton Server is 429 Resources Exhausted. Some
                 of the possible reasons for the error are:
                 1. GetFeatures exceeded the concurrent request limit, please retry later
                 2. DynamoDB throttled the request. The request rate exceeds the AWS account's throughput limit, or
                     you may be requesting a hot key
             ServiceUnavailableError: If the response returned from the Tecton Server is 503 Service Unavailable, it
                 could be because Tecton is currently unable to process your request. Please retry later.
             GatewayTimeoutError: If the response returned from the Tecton Server is 504 Gateway Timeout, it indicates
@@ -142,28 +144,30 @@
         Returns:
             GetFeaturesBatchResponse: The :class:`GetFeaturesBatchResponse` object representing the response from the
                 HTTP API, with the list of feature vectors and metadata (if requested).
 
         Example:
             >>> tecton_client = TectonClient(url, api_key)
             >>> join_key_map = {"example_join_key": "example_join_value"}
-            >>> request_context_map = {"example_request_context": "example_string_value"}
-            >>> request_data = GetFeaturesRequestData(join_key_map, request_context_map)
+            >>> request_context_map_1 = {"example_request_context1": "example_string_value1"}
+            >>> request_context_map_2 = {"example_request_context2": "example_string_value2"}
+            >>> request_data_1 = GetFeaturesRequestData(join_key_map, request_context_map_1)
+            >>> request_data_2 = GetFeaturesRequestData(join_key_map, request_context_map_2)
             >>> batch_request = GetFeaturesBatchRequest(
             ...     feature_service_name="example_feature_service",
-            ...     request_data_list=[request_data, request_data],
+            ...     request_data_list=[request_data_1, request_data_2],
             ...     workspace_name="example_workspace",
-            ...     micro_batch_size=2
+            ...     micro_batch_size=1
             ... )
             >>> batch_response = tecton_client.get_features_batch(batch_request)
             `batch_response.response_list` returns a list of :class:`GetFeaturesResponse` objects representing a
             response for each request in the :class:`GetFeaturesBatchRequest` object.
             Each :class:`GetFeaturesResponse` object contains a dictionary of {feature_name: `FeatureValue`} pairs,
             which can be accessed using:
-            >>> for response in batch_response.response_list:
+            >>> for response in batch_response.batch_response_list:
             >>>     print([feature.feature_value for feature in response.feature_values.values()])
 
         Raises:
             TectonClientError: If the client encounters an error while making the request.
             BadRequestError: If the response returned from the Tecton Server is 400 Bad Request. Please
                 check the exception message for detailed information.
             UnauthorizedError: If the response returned from the Tecton Server is 401 Unauthorized, it could be because
@@ -174,15 +178,15 @@
             ForbiddenError: If the response returned from the Tecton Server is 403 Forbidden, it could be because the
                 Service Account associated with your API Key does not have the necessary permissions to query
                 the feature service. Please refer to the `Tecton Documentation <https://docs.tecton.ai/docs/beta/\
                 reading-feature-data/reading-feature-data-for-inference/reading-online-features-for-inference-using-\
                 the-http-api#creating-an-api-key-to-authenticate-to-the-http-api>`_ for more information.
             NotFoundError: If the response returned from the Tecton Server is 404 Not Found. Please check the exception
                 message for detailed information.
-            ResourcesExhaustedError: If the response returned from the Tecton Server is 429 Resources Exhausted. Please
+            ResourceExhaustedError: If the response returned from the Tecton Server is 429 Resources Exhausted. Please
                 check the exception message for detailed information.
             ServiceUnavailableError: If the response returned from the Tecton Server is 503 Service Unavailable, it
                 could be because Tecton is currently unable to process your request. Please retry later.
             GatewayTimeoutError: If the response returned from the Tecton Server is 504 Gateway Timeout, it indicates
                 that processing the request exceeded the 2 seconds timeout limit set by Tecton.
 
                 For more detailed information on the errors, please refer to the error responses `here
@@ -194,14 +198,70 @@
                 endpoint=request.ENDPOINT, request_bodies=request.to_json_list(), timeout=request.timeout
             )
         )
         return GetFeaturesBatchResponse(
             responses_list=results, request_latency=latency, micro_batch_size=request.micro_batch_size
         )
 
+    def get_feature_service_metadata(
+        self, request: GetFeatureServiceMetadataRequest
+    ) -> GetFeatureServiceMetadataResponse:
+        """Makes a request to the /metadata endpoint and returns the response in the form of a
+        :class:`GetFeatureServiceMetadataResponse` object.
+
+        Args:
+            request (GetFeatureServiceMetadataRequest): The :class:`GetFeatureServiceMetadataRequest` object
+                with the request parameters.
+
+        Returns:
+            GetFeatureServiceMetadataResponse: The :class:`GetFeatureServiceMetadataResponse` object representing the
+                response from the HTTP API with the requested information.
+
+        Example:
+            >>> tecton_client = TectonClient(url, api_key)
+            >>> metadata_request = GetFeatureServiceMetadataRequest(
+            ...     feature_service_name="example_feature_service",
+            ...     workspace_name="example_workspace",
+            ... )
+            >>> metadata_response = tecton_client.get_feature_service_metadata(metadata_request)
+            The `metadata_response` object contains the metadata information requested as different
+            fields of the object.
+
+            >>> print(metadata_response.feature_values)
+            >>> print(metadata_response.input_join_keys)
+
+        Raises:
+            TectonClientError: If the client encounters an error while making the request.
+            UnauthorizedError: If the response returned from the Tecton Server is 401 Unauthorized, it could be because
+                Tecton does not recognize the API Key in your request. Please refer to the `API Key Documentation
+                <https://docs.tecton.ai/docs/beta/reading-feature-data/reading-feature-data-for-inference/\
+                reading-online-features-for-inference-using-the-http-api#creating-an-api-key-to-authenticate-\
+                to-the-http-api>`_ for more information on how to create a Service Account with an API Key
+            ForbiddenError: If the response returned from the Tecton Server is 403 Forbidden, it could be because the
+                Service Account associated with your API Key does not have the necessary permissions to query
+                the feature service. Please refer to the `Tecton Documentation <https://docs.tecton.ai/docs/beta/\
+                reading-feature-data/reading-feature-data-for-inference/reading-online-features-for-inference-using-\
+                the-http-api#creating-an-api-key-to-authenticate-to-the-http-api>`_ for more information.
+            NotFoundError: If the response returned from the Tecton Server is 404 Not Found. Please check the exception
+                message for detailed information.
+            ResourcesExhaustedError: If the response returned from the Tecton Server is 429 Resources Exhausted. Please
+                check the exception message for detailed information.
+            ServiceUnavailableError: If the response returned from the Tecton Server is 503 Service Unavailable, it
+                could be because Tecton is currently unable to process your request. Please retry later.
+            GatewayTimeoutError: If the response returned from the Tecton Server is 504 Gateway Timeout, it indicates
+                that processing the request exceeded the 2 seconds timeout limit set by Tecton.
+
+                For more detailed information on the errors, please refer to the error responses `here
+                <https://docs.tecton.ai/http-api#operation/GetFeaturesBatch>`_.
+
+        """
+        http_request = HTTPRequest(endpoint=request.ENDPOINT, request_body=request.to_json())
+        http_response = asyncio_run(self._tecton_http_client.execute_request(request=http_request))
+        return GetFeatureServiceMetadataResponse(http_response=http_response)
+
     @property
     def is_closed(self) -> bool:
         """Returns True if the client has been closed, False otherwise."""
         return self._tecton_http_client.is_closed
 
     def close(self) -> None:
         """Closes the client, releasing allocated resources and allowing connection reuse.
```

### Comparing `tecton_client-0.1.0b1/tecton_client/utils.py` & `tecton_client-0.1.0b2/tecton_client/utils.py`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/data_types_test.py` & `tecton_client-0.1.0b2/tests/data_types_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pytest
 
 from tecton_client.data_types import ArrayType
 from tecton_client.data_types import BoolType
 from tecton_client.data_types import DataType
 from tecton_client.data_types import FloatType
 from tecton_client.data_types import IntType
+from tecton_client.data_types import NameAndType
 from tecton_client.data_types import StringType
 from tecton_client.data_types import StructField
 from tecton_client.data_types import StructType
 from tecton_client.exceptions import TectonClientError
 from tecton_client.responses import FeatureValue
 from tecton_client.responses import Value
 from tests.test_utils import dict_equals
@@ -186,7 +187,23 @@
         with pytest.raises(TectonClientError):
             FeatureValue(
                 name="test.test_feature",
                 data_type="array",
                 feature_value=feature_value,
                 element_type=fields[0]["dataType"]["elementType"],
             )
+
+    @pytest.mark.parametrize(
+        "data_type",
+        [
+            BoolType(),
+            IntType(),
+            FloatType(),
+            StringType(),
+            ArrayType(IntType()),
+            StructType([StructField("field1", StringType()), StructField("field2", IntType())]),
+        ],
+    )
+    def test_name_and_type(self, data_type: DataType) -> None:
+        name_and_type_var = NameAndType(name="test", data_type=data_type)
+        assert name_and_type_var.name == "test"
+        assert type(name_and_type_var.data_type) == type(data_type)
```

### Comparing `tecton_client-0.1.0b1/tests/http_client_test.py` & `tecton_client-0.1.0b2/tests/http_client_test.py`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/requests_test.py` & `tecton_client-0.1.0b2/tests/requests_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import os
 from typing import List
 from typing import Union
 
 import pytest
 
-from tecton_client.constants import DEFAULT_WORKSPACE_NAME
 from tecton_client.exceptions import InvalidMicroBatchSizeError
 from tecton_client.exceptions import InvalidParameterError
 from tecton_client.exceptions import UnsupportedTypeError
 from tecton_client.requests import GetFeaturesBatchRequest
 from tecton_client.requests import GetFeatureServiceMetadataRequest
 from tecton_client.requests import GetFeaturesMicroBatchRequest
 from tecton_client.requests import GetFeaturesRequest
@@ -393,44 +392,26 @@
         [
             (
                 TEST_WORKSPACE_NAME,
                 {
                     "feature_service_name": "test_feature_service_name",
                     "workspace_name": "test_workspace_name",
                 },
-            ),
-            (
-                None,
-                {
-                    "feature_service_name": "test_feature_service_name",
-                    "workspace_name": "prod",
-                },
-            ),
-            (
-                "",
-                {
-                    "feature_service_name": "test_feature_service_name",
-                    "workspace_name": "prod",
-                },
-            ),
+            )
         ],
     )
     def test_metadata_request(self, workspace_name: str, expected_response: dict) -> None:
         request = GetFeatureServiceMetadataRequest(
             feature_service_name=self.TEST_FEATURE_SERVICE_NAME, workspace_name=workspace_name
         )
-        if workspace_name:
-            assert request.workspace_name == workspace_name
-        else:
-            assert request.workspace_name == DEFAULT_WORKSPACE_NAME
 
         assert request.feature_service_name == self.TEST_FEATURE_SERVICE_NAME
         assert request.ENDPOINT == GetFeatureServiceMetadataRequest.ENDPOINT
 
         assert request.to_json() == {"params": expected_response}
 
-    @pytest.mark.parametrize("feature_service", ["", None])
-    def test_error_feature_service_name_metadata(self, feature_service: str) -> None:
+    @pytest.mark.parametrize(
+        "feature_service, workspace_name", [("test", ""), ("test", None), (None, "test"), ("", "test")]
+    )
+    def test_error_parameters_metadata(self, feature_service: str, workspace_name: str) -> None:
         with pytest.raises(InvalidParameterError):
-            GetFeatureServiceMetadataRequest(
-                workspace_name=self.TEST_WORKSPACE_NAME, feature_service_name=feature_service
-            )
+            GetFeatureServiceMetadataRequest(workspace_name=workspace_name, feature_service_name=feature_service)
```

### Comparing `tecton_client-0.1.0b1/tests/responses_test.py` & `tecton_client-0.1.0b2/tests/responses_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 
 import pytest
 
 from tecton_client.data_types import ArrayType
 from tecton_client.data_types import BoolType
 from tecton_client.data_types import FloatType
 from tecton_client.data_types import IntType
+from tecton_client.data_types import StringType
 from tecton_client.data_types import StructType
+from tecton_client.responses import FeatureServiceType
 from tecton_client.responses import FeatureStatus
 from tecton_client.responses import GetFeaturesBatchResponse
+from tecton_client.responses import GetFeatureServiceMetadataResponse
 from tecton_client.responses import GetFeaturesResponse
 from tecton_client.responses import HTTPResponse
 from tecton_client.responses import SloIneligibilityReason
 from tecton_client.utils import parse_string_to_isotime
 from tests.test_utils import dict_equals
 
 
@@ -353,7 +356,70 @@
         )
 
         # Test that the order of responses is retained by comparing a random feature within each response
         assert all(
             response.feature_values[feature_name].feature_value == order_of_responses.pop(0)
             for response in batch_response.batch_response_list
         )
+
+    def assert_name_and_type_match(self, input_dict: dict, response_dict: dict) -> None:
+        assert len(input_dict) == len(response_dict)
+        for key, value in input_dict.items():
+            assert key in response_dict
+            assert isinstance(response_dict[key].data_type, value)
+
+    @pytest.mark.parametrize(
+        "file_name, feature_service_type, input_join_keys, input_rc_keys, feature_values, output_join_keys",
+        [
+            (
+                "sample_metadata_response.json",
+                FeatureServiceType.DEFAULT,
+                {"longitude": FloatType, "latitude": FloatType},
+                {},
+                {
+                    "average_rain.average_temperate_6hrs": ArrayType,
+                    "average_rain.precipitation_higher_than_average": BoolType,
+                },
+                {},
+            ),
+            (
+                "sample_metadata_response_long.json",
+                FeatureServiceType.DEFAULT,
+                {"user_id": StringType, "merchant": StringType},
+                {"amt": FloatType},
+                {
+                    "transaction_amount_is_higher_than_average.transaction_amount_is_higher_than_average": BoolType,
+                    "merchant_fraud_rate.is_fraud_mean_1d_1d": FloatType,
+                    "merchant_fraud_rate.is_fraud_mean_30d_1d": FloatType,
+                    "merchant_fraud_rate.is_fraud_mean_90d_1d": FloatType,
+                    "user_distinct_merchant_transaction_count_30d.distinct_merchant_transaction_count_30d": IntType,
+                    "user_transaction_amount_metrics.amt_mean_1d_10m": FloatType,
+                    "user_transaction_amount_metrics.amt_mean_1h_10m": FloatType,
+                    "user_transaction_amount_metrics.amt_mean_3d_10m": FloatType,
+                    "user_transaction_amount_metrics.amt_sum_1d_10m": FloatType,
+                    "user_transaction_amount_metrics.amt_sum_1h_10m": FloatType,
+                    "user_transaction_amount_metrics.amt_sum_3d_10m": FloatType,
+                    "user_transaction_counts.transaction_id_last_3_1d_1d": ArrayType,
+                },
+                {},
+            ),
+        ],
+    )
+    def test_feature_service_metadata_response(
+        self,
+        file_name: str,
+        feature_service_type: FeatureServiceType,
+        input_join_keys: dict,
+        input_rc_keys: dict,
+        feature_values: dict,
+        output_join_keys: dict,
+    ) -> None:
+        with open(os.path.join(TestResponse.TEST_DATA_ROOT, file_name)) as json_file:
+            json_dict = json.load(json_file)
+            http_response = HTTPResponse(result=json_dict, latency=timedelta(milliseconds=10))
+            response = GetFeatureServiceMetadataResponse(http_response=http_response)
+
+            assert response.feature_service_type == feature_service_type
+            self.assert_name_and_type_match(input_join_keys, response.input_join_keys)
+            self.assert_name_and_type_match(input_rc_keys, response.input_request_context_keys)
+            self.assert_name_and_type_match(feature_values, response.feature_values)
+            self.assert_name_and_type_match(output_join_keys, response.output_join_keys)
```

### Comparing `tecton_client-0.1.0b1/tests/tecton_client_test.py` & `tecton_client-0.1.0b2/tests/tecton_client_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 from tecton_client.data_types import FloatType
 from tecton_client.data_types import IntType
 from tecton_client.exceptions import BadRequestError
 from tecton_client.exceptions import ForbiddenError
 from tecton_client.exceptions import GatewayTimeoutError
 from tecton_client.exceptions import InvalidParameterError
 from tecton_client.exceptions import NotFoundError
-from tecton_client.exceptions import ResourcesExhaustedError
+from tecton_client.exceptions import ResourceExhaustedError
 from tecton_client.exceptions import ServiceUnavailableError
 from tecton_client.exceptions import TectonServerException
 from tecton_client.exceptions import UnauthorizedError
 from tecton_client.requests import GetFeaturesBatchRequest
+from tecton_client.requests import GetFeatureServiceMetadataRequest
 from tecton_client.requests import GetFeaturesRequest
 from tecton_client.requests import GetFeaturesRequestData
 from tecton_client.requests import MetadataOptions
+from tecton_client.responses import FeatureServiceType
 from tecton_client.responses import FeatureStatus
 from tecton_client.tecton_client import TectonClient
 from tecton_client.tecton_client import TectonClientOptions
 from tests.test_utils import dict_equals
 
 
 @pytest.fixture
@@ -39,14 +41,15 @@
 
 class TestTectonClient:
     api_key: Final[str] = "1234"
     url: Final[str] = "https://thisisaurl.ai"
 
     final_url: Final[str] = urljoin(url, "api/v1/feature-service/get-features")
     batch_url: Final[str] = urljoin(url, "api/v1/feature-service/get-features-batch")
+    metadata_url: Final[str] = urljoin(url, "api/v1/feature-service/metadata")
 
     TEST_DATA_ROOT: Final[str] = "tests/test_data/"
     TEST_DATA_REL_PATH_SINGLE: Final[str] = os.path.join(TEST_DATA_ROOT, "single/")
     TEST_DATA_REL_PATH_BATCH: Final[str] = os.path.join(TEST_DATA_ROOT, "batch/")
 
     expected_response_mixed = {
         "test.output_struct1": None,
@@ -124,14 +127,18 @@
     test_request_batch = GetFeaturesBatchRequest(
         feature_service_name="test_feature_service",
         request_data_list=[GetFeaturesRequestData(join_key_map, request_context_map)] * 10,
         workspace_name="test-workspace",
         metadata_options={MetadataOptions.SLO_INFO, MetadataOptions.FEATURE_STATUS, MetadataOptions.EFFECTIVE_TIME},
         micro_batch_size=5,
     )
+    test_request_fs_metadata = GetFeatureServiceMetadataRequest(
+        feature_service_name="test_feature_service",
+        workspace_name="test-workspace",
+    )
 
     tecton_client = TectonClient(url=url, api_key=api_key)
 
     @pytest.mark.parametrize(
         "file_name, expected_response",
         [
             ("sample_response_mixed.json", expected_response_mixed),
@@ -208,15 +215,15 @@
                     "message": "Unable to query FeatureService `fs` for workspace `ws`. Newly created feature "
                     "services may take up to 60 seconds to query. Also, ensure that the workspace "
                     "is a live workspace.",
                     "code": 5,
                 },
             ),
             (
-                ResourcesExhaustedError,
+                ResourceExhaustedError,
                 429,
                 {
                     "error": "GetFeatures exceeded the concurrent request limit, please retry later",
                     "message": "GetFeatures exceeded the concurrent request limit, please retry later",
                     "code": 8,
                 },
             ),
@@ -334,9 +341,31 @@
 
             # Test that the order of responses is retained by comparing a random feature within each response
             assert all(
                 response.feature_values[feature_name].feature_value == order_of_responses.pop(0)
                 for response in batch_response.batch_response_list
             )
 
+    @pytest.mark.parametrize(
+        "file_name, feature_service_type",
+        [
+            ("sample_metadata_response.json", FeatureServiceType.DEFAULT),
+            ("sample_metadata_response_long.json", FeatureServiceType.DEFAULT),
+        ],
+    )
+    def test_get_metadata(self, mocked: aioresponses, file_name: str, feature_service_type: FeatureServiceType) -> None:
+        with open(os.path.join(TestTectonClient.TEST_DATA_ROOT, file_name)) as json_file:
+            json_request = json.load(json_file)
+            mocked.post(url=self.metadata_url, payload=json_request)
+            response = self.tecton_client.get_feature_service_metadata(self.test_request_fs_metadata)
+
+            print(json_request)
+
+            assert response is not None
+            assert response.feature_service_type == feature_service_type
+            assert len(response.input_join_keys) == len(json_request.get("inputJoinKeys", []))
+            assert len(response.input_request_context_keys) == len(json_request.get("inputRequestContextKeys", []))
+            assert len(response.feature_values) == len(json_request.get("featureValues", []))
+            assert len(response.output_join_keys) == len(json_request.get("outputJoinKeys", []))
+
     def pytest_sessionfinish(self) -> None:
         self.tecton_client.close()
```

### Comparing `tecton_client-0.1.0b1/tests/test_utils.py` & `tecton_client-0.1.0b2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/batch/batch_expected_request_1.json` & `tecton_client-0.1.0b2/tests/test_data/batch/batch_expected_request_1.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/batch/batch_expected_request_2.json` & `tecton_client-0.1.0b2/tests/test_data/batch/batch_expected_request_2.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/batch/batch_expected_request_3.json` & `tecton_client-0.1.0b2/tests/test_data/batch/batch_expected_request_3.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/batch/batch_expected_request_4.json` & `tecton_client-0.1.0b2/tests/test_data/batch/batch_expected_request_4.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/batch/sample_batch_response.json` & `tecton_client-0.1.0b2/tests/test_data/batch/sample_batch_response.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/batch/sample_batch_response_long_slo.json` & `tecton_client-0.1.0b2/tests/test_data/batch/sample_batch_response_long_slo.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/batch/sample_batch_response_slo.json` & `tecton_client-0.1.0b2/tests/test_data/batch/sample_batch_response_slo.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/single/sample_response.json` & `tecton_client-0.1.0b2/tests/test_data/single/sample_response.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/single/sample_response_list.json` & `tecton_client-0.1.0b2/tests/test_data/single/sample_response_list.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/single/sample_response_long.json` & `tecton_client-0.1.0b2/tests/test_data/single/sample_response_long.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/single/sample_response_metadata.json` & `tecton_client-0.1.0b2/tests/test_data/single/sample_response_metadata.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/single/sample_response_mixed.json` & `tecton_client-0.1.0b2/tests/test_data/single/sample_response_mixed.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/single/sample_response_null.json` & `tecton_client-0.1.0b2/tests/test_data/single/sample_response_null.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/single/sample_response_slo.json` & `tecton_client-0.1.0b2/tests/test_data/single/sample_response_slo.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/tests/test_data/single/sample_response_struct.json` & `tecton_client-0.1.0b2/tests/test_data/single/sample_response_struct.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/LICENSE.md` & `tecton_client-0.1.0b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b1/pyproject.toml` & `tecton_client-0.1.0b2/pyproject.toml`

 * *Files identical despite different names*

