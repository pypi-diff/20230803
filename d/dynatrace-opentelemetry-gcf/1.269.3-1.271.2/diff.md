# Comparing `tmp/dynatrace_opentelemetry_gcf-1.269.3-py3-none-any.whl.zip` & `tmp/dynatrace_opentelemetry_gcf-1.271.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12133 bytes, number of entries: 10
+Zip file size: 12264 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/__init__.py
 -rw-r--r--  2.0 unx     4834 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/_resource.py
--rw-r--r--  2.0 unx     6846 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/_trigger.py
+-rw-r--r--  2.0 unx     7304 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/_trigger.py
 -rw-r--r--  2.0 unx     1938 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/_wrapper.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/py.typed
 -rw-r--r--  2.0 unx       24 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/version.py
-?rw-r--r--  2.0 unx     1189 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.269.3.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.269.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.269.3.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      959 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.269.3.dist-info/RECORD
-10 files, 27894 bytes uncompressed, 10451 bytes compressed:  62.5%
+?rw-r--r--  2.0 unx     1189 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.271.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.271.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.271.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      959 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.271.2.dist-info/RECORD
+10 files, 28352 bytes uncompressed, 10582 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: dynatrace/opentelemetry/gcf/py.typed
 Comment: 
 
 Filename: dynatrace/opentelemetry/gcf/version.py
 Comment: 
 
-Filename: dynatrace_opentelemetry_gcf-1.269.3.dist-info/METADATA
+Filename: dynatrace_opentelemetry_gcf-1.271.2.dist-info/METADATA
 Comment: 
 
-Filename: dynatrace_opentelemetry_gcf-1.269.3.dist-info/WHEEL
+Filename: dynatrace_opentelemetry_gcf-1.271.2.dist-info/WHEEL
 Comment: 
 
-Filename: dynatrace_opentelemetry_gcf-1.269.3.dist-info/licenses/LICENSE
+Filename: dynatrace_opentelemetry_gcf-1.271.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: dynatrace_opentelemetry_gcf-1.269.3.dist-info/RECORD
+Filename: dynatrace_opentelemetry_gcf-1.271.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dynatrace/opentelemetry/gcf/_trigger.py

```diff
@@ -11,30 +11,35 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import abc
 import contextlib
 import threading
-from typing import Any, Dict, Iterator, NamedTuple, Optional
+from types import MappingProxyType
+from typing import Any, Callable, Dict, Iterator, NamedTuple, Optional
 
 import flask
 from opentelemetry import trace as api_trace
+from opentelemetry.context import attach, detach
 from opentelemetry.context.context import Context
 from opentelemetry.propagate import extract
 from opentelemetry.trace.span import Span
 from opentelemetry.trace.status import Status, StatusCode
 from opentelemetry.util.types import AttributeValue
 
 from dynatrace.odin.semconv import v1 as semconv
 from dynatrace.opentelemetry.gcf._resource import (
     detect_resource,
     get_function_name,
 )
 from dynatrace.opentelemetry.tracing._logging.loggers import gcf_logger
+from dynatrace.opentelemetry.tracing._util.context import (
+    set_propagated_resource_attributes,
+)
 from dynatrace.opentelemetry.tracing._util.exceptions import record_exception
 
 _INSTRUMENTATION_LIBRARY_NAME = "dynatrace.opentelemetry.gcf"
 _FLUSH_TIMEOUT_MILLIS = 6000
 
 
 class _TriggerGlobals(NamedTuple):
@@ -53,26 +58,41 @@
 
         with Trigger._TRIGGER_GLOBALS_LOCK:
             if Trigger._TRIGGER_GLOBALS is not None:
                 return Trigger._TRIGGER_GLOBALS
 
             Trigger._TRIGGER_GLOBALS = _TriggerGlobals(
                 tracer=api_trace.get_tracer(_INSTRUMENTATION_LIBRARY_NAME),
-                resource_attrs=detect_resource(),
+                resource_attrs=MappingProxyType(detect_resource()),
             )
 
             return Trigger._TRIGGER_GLOBALS
 
     @contextlib.contextmanager
     def start_as_current_span(self, flush_on_exit: bool) -> Iterator[Span]:
         _globals = self._get_or_prepare_globals()
         parent_context = self._extract_parent()
-        attrs = {**_globals.resource_attrs}
-        self._add_start_attributes(attrs)
 
+        attrs = _globals.resource_attrs.copy()
+        parent_context = set_propagated_resource_attributes(
+            attrs, parent_context
+        )
+        # Set context as active as workaround for: https://github.com/open-telemetry/opentelemetry-python/issues/3350
+        ot_context_token = attach(parent_context)
+
+        def _exit_callback():
+            try:
+                activation.__exit__(None, None, None)
+            finally:
+                detach(ot_context_token)
+
+            if flush_on_exit:
+                _flush_spans()
+
+        self._add_start_attributes(attrs)
         activation = _globals.tracer.start_as_current_span(
             get_function_name() or "invoke",
             parent_context,
             api_trace.SpanKind.SERVER,
             attributes=attrs,
             record_exception=False,
             set_status_on_exception=False,
@@ -82,32 +102,29 @@
         try:
             yield span
         except Exception as ex:  # pylint:disable=broad-except
             record_exception(span, ex)
             span.set_status(Status(StatusCode.ERROR))
             raise ex
         finally:
-            self._on_exit(activation, span, flush_on_exit)
+            self._on_exit(span, _exit_callback)
 
     def _extract_parent(self) -> Context:  # pylint:disable=no-self-use
         return Context()
 
-    @abc.abstractmethod
     def _add_start_attributes(self, attrs: Dict[str, AttributeValue]) -> None:
         pass
 
     def set_exit_attributes(self, span: Span, result: Any) -> None:
         pass
 
     def _on_exit(
-        self, activation: Iterator[Span], span: Span, flush_on_exit: bool
+        self, span: Span, exit_callback: Callable[[], None]
     ):  # pylint:disable=no-self-use
-        activation.__exit__(None, None, None)
-        if flush_on_exit:
-            _flush_spans()
+        exit_callback()
 
 
 class GenericTrigger(Trigger):
     def _add_start_attributes(self, attrs: Dict[str, AttributeValue]) -> None:
         attrs[semconv.FAAS_TRIGGER] = semconv.FaasTriggerValues.OTHER.value
 
 
@@ -150,34 +167,30 @@
 
     def set_exit_attributes(self, span: Span, result: Any) -> None:
         if isinstance(result, flask.Response):
             span.set_attribute(semconv.HTTP_STATUS_CODE, result.status_code)
             if result.status_code >= 500:
                 span.set_status(Status(StatusCode.ERROR))
 
-    def _on_exit(
-        self, activation: Iterator[Span], span: Span, flush_on_exit: bool
-    ):
-        _super_on_exit = super()._on_exit
-
+    def _on_exit(self, span: Span, exit_callback: Callable[[], None]):
         def _after_request(response: flask.Response) -> flask.Response:
             self.set_exit_attributes(span, response)
-            _super_on_exit(activation, span, flush_on_exit)
+            exit_callback()
 
             return response
 
         try:
             # defer span end until the current flask request is finished
             flask.after_this_request(_after_request)
         except Exception as ex:  # pylint: disable=broad-except
             gcf_logger.warning(
                 "Error when registering 'flask.after_this_request' callback: %s",
                 ex,
             )
-            _super_on_exit(activation, span, flush_on_exit)
+            exit_callback()
 
 
 def _flush_spans() -> None:
     tracer_provider = api_trace.get_tracer_provider()
     if hasattr(tracer_provider, "force_flush"):
         tracer_provider.force_flush(_FLUSH_TIMEOUT_MILLIS)
```

## dynatrace/opentelemetry/gcf/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.269.3"
+__version__ = "1.271.2"
```

## Comparing `dynatrace_opentelemetry_gcf-1.269.3.dist-info/METADATA` & `dynatrace_opentelemetry_gcf-1.271.2.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynatrace-opentelemetry-gcf
-Version: 1.269.3
+Version: 1.271.2
 Summary: Dynatrace OpenTelemetry package for Google Cloud Functions
 Project-URL: Homepage, https://www.dynatrace.com/technologies/python-monitoring/
 Author: Dynatrace
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
-Requires-Dist: dynatrace-opentelemetry-core==1.269.3
+Requires-Dist: dynatrace-opentelemetry-core==1.271.2
 Requires-Dist: flask<3.0,>=1.0
 Requires-Dist: opentelemetry-api~=1.3
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 # Dynatrace OpenTelemetry Tracing API For Python Google Cloud Functions
```

## Comparing `dynatrace_opentelemetry_gcf-1.269.3.dist-info/licenses/LICENSE` & `dynatrace_opentelemetry_gcf-1.271.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `dynatrace_opentelemetry_gcf-1.269.3.dist-info/RECORD` & `dynatrace_opentelemetry_gcf-1.271.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dynatrace/opentelemetry/gcf/__init__.py,sha256=pVCQ15ocBp7DACT2JC5wmLkyVRbeSqpF5nWkbypokL8,675
 dynatrace/opentelemetry/gcf/_resource.py,sha256=u2eY520ADxlgDir0OoapHkIf1Y9HdR-qSxxkcPkIV4I,4834
-dynatrace/opentelemetry/gcf/_trigger.py,sha256=uDAF-PMwrexrfHGsM3v4yRMaj5OZRb5ClRzZ61f39AQ,6846
+dynatrace/opentelemetry/gcf/_trigger.py,sha256=llD8GhUVbrHd8bj6_yat0I_iMB7Quqd9WFLrD22N_Uc,7304
 dynatrace/opentelemetry/gcf/_wrapper.py,sha256=aigZlgBBlF2Sxsd04xmzSr5nm3-rM61B0y4ttk_3r0c,1938
 dynatrace/opentelemetry/gcf/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dynatrace/opentelemetry/gcf/version.py,sha256=Iv8aaQDjoT0tZwDpNHehTNAt5kMZ3ZmEP8YNNJg71fA,24
-dynatrace_opentelemetry_gcf-1.269.3.dist-info/METADATA,sha256=O-4QzFXRAyt6OkCU79H-e1RNABVqUpgOtK7Zyv76Uf0,1189
-dynatrace_opentelemetry_gcf-1.269.3.dist-info/WHEEL,sha256=KGYbc1zXlYddvwxnNty23BeaKzh7YuoSIvIMO4jEhvw,87
-dynatrace_opentelemetry_gcf-1.269.3.dist-info/licenses/LICENSE,sha256=OUyLShRPZFGLXlxbnRr7Of_8mNYYQ_qda632uhGSIaY,11342
-dynatrace_opentelemetry_gcf-1.269.3.dist-info/RECORD,,
+dynatrace/opentelemetry/gcf/version.py,sha256=EYvGjX0vWkDeibiD0nZANl8LE-NQ5ZG1kY3dQde17dQ,24
+dynatrace_opentelemetry_gcf-1.271.2.dist-info/METADATA,sha256=8F-InG9KpUyHg-ov6IK-B_ELnrbnu8yS2mVRTbGPyZg,1189
+dynatrace_opentelemetry_gcf-1.271.2.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+dynatrace_opentelemetry_gcf-1.271.2.dist-info/licenses/LICENSE,sha256=OUyLShRPZFGLXlxbnRr7Of_8mNYYQ_qda632uhGSIaY,11342
+dynatrace_opentelemetry_gcf-1.271.2.dist-info/RECORD,,
```

