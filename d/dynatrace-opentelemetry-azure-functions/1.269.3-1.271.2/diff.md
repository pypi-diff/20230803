# Comparing `tmp/dynatrace_opentelemetry_azure_functions-1.269.3-py3-none-any.whl.zip` & `tmp/dynatrace_opentelemetry_azure_functions-1.271.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15110 bytes, number of entries: 11
+Zip file size: 15230 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      687 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/__init__.py
 -rw-r--r--  2.0 unx     3948 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/_bindings.py
 -rw-r--r--  2.0 unx     3563 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/_resource.py
--rw-r--r--  2.0 unx     6768 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/_triggers.py
+-rw-r--r--  2.0 unx     7350 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/_triggers.py
 -rw-r--r--  2.0 unx     8183 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/_wrapper.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/py.typed
 -rw-r--r--  2.0 unx       24 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/version.py
-?rw-r--r--  2.0 unx     1222 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1189 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/RECORD
-11 files, 37013 bytes uncompressed, 13006 bytes compressed:  64.9%
+?rw-r--r--  2.0 unx     1222 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.271.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.271.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.271.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1189 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.271.2.dist-info/RECORD
+11 files, 37595 bytes uncompressed, 13126 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: dynatrace/opentelemetry/azure/functions/py.typed
 Comment: 
 
 Filename: dynatrace/opentelemetry/azure/functions/version.py
 Comment: 
 
-Filename: dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/METADATA
+Filename: dynatrace_opentelemetry_azure_functions-1.271.2.dist-info/METADATA
 Comment: 
 
-Filename: dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/WHEEL
+Filename: dynatrace_opentelemetry_azure_functions-1.271.2.dist-info/WHEEL
 Comment: 
 
-Filename: dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/licenses/LICENSE
+Filename: dynatrace_opentelemetry_azure_functions-1.271.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/RECORD
+Filename: dynatrace_opentelemetry_azure_functions-1.271.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dynatrace/opentelemetry/azure/functions/_triggers.py

```diff
@@ -25,14 +25,17 @@
 from opentelemetry.trace.span import Span
 from opentelemetry.trace.status import Status, StatusCode
 from opentelemetry.util.types import AttributeValue
 
 from dynatrace.odin.semconv import v1 as semconv
 from dynatrace.opentelemetry.azure.functions._bindings import InvocationArgs
 from dynatrace.opentelemetry.azure.functions._resource import detect_resource
+from dynatrace.opentelemetry.tracing._util.context import (
+    propagate_resource_attributes,
+)
 from dynatrace.opentelemetry.tracing._util.exceptions import record_exception
 
 _INSTRUMENTATION_LIBRARY_NAME = "dynatrace.opentelemetry.azure.functions"
 _UNKNOWN_BINDING = object()
 
 
 class Trigger(abc.ABC):
@@ -45,30 +48,36 @@
         self.args = invoke_args.args
         self.kwargs = invoke_args.kwargs
 
     @contextlib.contextmanager
     def start_as_current_span(self) -> Iterator[Span]:
         tracer = self._get_tracer()
         attributes = detect_resource(self._invoke_args.context)
-        parent_context = self._add_start_attributes(attributes)
+        parent_context = self._extract_parent()
 
-        with tracer.start_as_current_span(
-            self._get_function_name(),
-            parent_context,
-            SpanKind.SERVER,
-            attributes=attributes,
-            record_exception=False,
-            set_status_on_exception=False,
-            end_on_exit=True,
-        ) as span:
-            try:
-                yield span
-            except BaseException as ex:
-                self._on_exception(span, ex)
-                raise ex
+        # Set context as active as workaround for: https://github.com/open-telemetry/opentelemetry-python/issues/3350
+        with propagate_resource_attributes(
+            attributes, parent_context
+        ) as parent_context:
+            self._add_start_attributes(attributes)
+
+            with tracer.start_as_current_span(
+                self._get_function_name(),
+                parent_context,
+                SpanKind.SERVER,
+                attributes=attributes,
+                record_exception=False,
+                set_status_on_exception=False,
+                end_on_exit=True,
+            ) as span:
+                try:
+                    yield span
+                except BaseException as ex:
+                    self._on_exception(span, ex)
+                    raise ex
 
     def _get_tracer(self) -> Tracer:
         tracer = Trigger._TRACER
         if tracer is not None:
             return tracer
 
         with self._TRACER_LOCK:
@@ -82,58 +91,60 @@
 
     def _get_function_name(self) -> str:
         if self._invoke_args.context is not None:
             return self._invoke_args.context.function_name
         return "invoke"
 
     @abc.abstractmethod
-    def _add_start_attributes(
-        self, attrs: Dict[str, AttributeValue]
-    ) -> Context:
+    def _extract_parent(self) -> Context:
+        pass
+
+    @abc.abstractmethod
+    def _add_start_attributes(self, attrs: Dict[str, AttributeValue]) -> None:
         pass
 
     def _on_exception(  # pylint:disable=no-self-use
         self, span: Span, exception: BaseException
     ) -> None:
         if span.is_recording():
             record_exception(span, exception)
             span.set_status(Status(StatusCode.ERROR))
 
     def set_exit_attributes(self, span: Span, result: Any) -> None:
         pass
 
 
 class GenericTrigger(Trigger):
-    def _add_start_attributes(
-        self, attrs: Dict[str, AttributeValue]
-    ) -> Context:
-        attrs[semconv.FAAS_TRIGGER] = semconv.FaasTriggerValues.OTHER.value
+    def _extract_parent(self) -> Context:
         return Context()
 
+    def _add_start_attributes(self, attrs: Dict[str, AttributeValue]) -> None:
+        attrs[semconv.FAAS_TRIGGER] = semconv.FaasTriggerValues.OTHER.value
+
 
 class HttpTrigger(Trigger):
     _RESPONSE_TYPES = (func.HttpResponse, str, type(None))
     _CAPTURE_HEADERS = {
         "user-agent": semconv.HTTP_USER_AGENT,
         "referer": semconv.DT_HTTP_REQUEST_HEADER_REFERER,
     }
 
-    def _add_start_attributes(
-        self, attrs: Dict[str, AttributeValue]
-    ) -> Context:
+    def _extract_parent(self):
+        req = self._trigger_param  # type: func.HttpRequest
+        return extract(req.headers, Context())
+
+    def _add_start_attributes(self, attrs: Dict[str, AttributeValue]) -> None:
         req = self._trigger_param  # type: func.HttpRequest
 
         attrs[semconv.FAAS_TRIGGER] = semconv.FaasTriggerValues.HTTP.value
         attrs[semconv.HTTP_METHOD] = req.method or "GET"
         attrs[semconv.HTTP_URL] = req.url
 
         self._capture_http_headers(attrs, req)
 
-        return extract(req.headers, Context())
-
     def _capture_http_headers(
         self, attributes: Dict[str, AttributeValue], req: func.HttpRequest
     ) -> None:
         for header_name, semconv_key in self._CAPTURE_HEADERS.items():
             header_value = req.headers.get(header_name)
             if header_value is not None:
                 attributes[semconv_key] = header_value
```

## dynatrace/opentelemetry/azure/functions/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.269.3"
+__version__ = "1.271.2"
```

## Comparing `dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/METADATA` & `dynatrace_opentelemetry_azure_functions-1.271.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynatrace-opentelemetry-azure-functions
-Version: 1.269.3
+Version: 1.271.2
 Summary: Dynatrace OpenTelemetry package for Azure Functions
 Project-URL: Homepage, https://www.dynatrace.com/technologies/python-monitoring/
 Author: Dynatrace
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: azure-functions>=1.0
-Requires-Dist: dynatrace-opentelemetry-core==1.269.3
+Requires-Dist: dynatrace-opentelemetry-core==1.271.2
 Requires-Dist: opentelemetry-api~=1.3
 Requires-Dist: wrapt<2,>=1.10
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 # Dynatrace OpenTelemetry Tracing API For Python Azure Functions
```

## Comparing `dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/licenses/LICENSE` & `dynatrace_opentelemetry_azure_functions-1.271.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

