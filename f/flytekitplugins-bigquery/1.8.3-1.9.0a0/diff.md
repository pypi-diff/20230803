# Comparing `tmp/flytekitplugins-bigquery-1.8.3.tar.gz` & `tmp/flytekitplugins-bigquery-1.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-bigquery-1.8.3.tar", last modified: Thu Aug  3 17:08:09 2023, max compression
+gzip compressed data, was "flytekitplugins-bigquery-1.9.0a0.tar", last modified: Thu Jul 20 18:58:14 2023, max compression
```

## Comparing `flytekitplugins-bigquery-1.8.3.tar` & `flytekitplugins-bigquery-1.9.0a0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:09.836229 flytekitplugins-bigquery-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-03 17:08:09.836229 flytekitplugins-bigquery-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-03 17:07:50.000000 flytekitplugins-bigquery-1.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:09.836229 flytekitplugins-bigquery-1.8.3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:09.836229 flytekitplugins-bigquery-1.8.3/flytekitplugins/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-03 17:07:50.000000 flytekitplugins-bigquery-1.8.3/flytekitplugins/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-03 17:07:50.000000 flytekitplugins-bigquery-1.8.3/flytekitplugins/bigquery/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-08-03 17:07:50.000000 flytekitplugins-bigquery-1.8.3/flytekitplugins/bigquery/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:09.836229 flytekitplugins-bigquery-1.8.3/flytekitplugins_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-03 17:08:09.000000 flytekitplugins-bigquery-1.8.3/flytekitplugins_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-03 17:08:09.000000 flytekitplugins-bigquery-1.8.3/flytekitplugins_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:08:09.000000 flytekitplugins-bigquery-1.8.3/flytekitplugins_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-03 17:08:09.000000 flytekitplugins-bigquery-1.8.3/flytekitplugins_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 17:08:09.000000 flytekitplugins-bigquery-1.8.3/flytekitplugins_bigquery.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-03 17:08:09.000000 flytekitplugins-bigquery-1.8.3/flytekitplugins_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 17:08:09.000000 flytekitplugins-bigquery-1.8.3/flytekitplugins_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:08:09.836229 flytekitplugins-bigquery-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-03 17:08:08.000000 flytekitplugins-bigquery-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:14.872624 flytekitplugins-bigquery-1.9.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-20 18:58:14.872624 flytekitplugins-bigquery-1.9.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-20 18:57:54.000000 flytekitplugins-bigquery-1.9.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:14.868624 flytekitplugins-bigquery-1.9.0a0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:14.872624 flytekitplugins-bigquery-1.9.0a0/flytekitplugins/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 18:57:54.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-20 18:57:54.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins/bigquery/backend_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-20 18:57:54.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins/bigquery/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:14.872624 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-20 18:58:14.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-20 18:58:14.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:14.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-20 18:58:14.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:14.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 18:58:14.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:14.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:14.872624 flytekitplugins-bigquery-1.9.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-20 18:58:12.000000 flytekitplugins-bigquery-1.9.0a0/setup.py
```

### Comparing `flytekitplugins-bigquery-1.8.3/PKG-INFO` & `flytekitplugins-bigquery-1.9.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.8.3
+Version: 1.9.0a0
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.8.3/README.md` & `flytekitplugins-bigquery-1.9.0a0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.8.3/flytekitplugins/bigquery/agent.py` & `flytekitplugins-bigquery-1.9.0a0/flytekitplugins/bigquery/backend_plugin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import datetime
-import json
-from dataclasses import asdict, dataclass
 from typing import Dict, Optional
 
 import grpc
-from flyteidl.admin.agent_pb2 import (
-    PERMANENT_FAILURE,
+from flyteidl.service.external_plugin_service_pb2 import (
     SUCCEEDED,
-    CreateTaskResponse,
-    DeleteTaskResponse,
-    GetTaskResponse,
-    Resource,
+    TaskCreateResponse,
+    TaskDeleteResponse,
+    TaskGetResponse,
 )
 from google.cloud import bigquery
 
 from flytekit import FlyteContextManager, StructuredDataset, logger
 from flytekit.core.type_engine import TypeEngine
-from flytekit.extend.backend.base_agent import AgentBase, AgentRegistry, convert_to_flyte_state
+from flytekit.extend.backend.base_plugin import BackendPluginBase, BackendPluginRegistry, convert_to_flyte_state
 from flytekit.models import literals
 from flytekit.models.literals import LiteralMap
 from flytekit.models.task import TaskTemplate
 from flytekit.models.types import LiteralType, StructuredDatasetType
 
 pythonTypeToBigQueryType: Dict[type, str] = {
     # https://cloud.google.com/bigquery/docs/reference/standard-sql/data-types#data_type_sizes
@@ -30,88 +26,69 @@
     datetime.datetime: "DATETIME",
     float: "FLOAT64",
     int: "INT64",
     str: "STRING",
 }
 
 
-@dataclass
-class Metadata:
-    job_id: str
-    project: str
-    location: str
-
-
-class BigQueryAgent(AgentBase):
+class BigQueryPlugin(BackendPluginBase):
     def __init__(self):
         super().__init__(task_type="bigquery_query_job_task")
 
     def create(
         self,
         context: grpc.ServicerContext,
         output_prefix: str,
         task_template: TaskTemplate,
         inputs: Optional[LiteralMap] = None,
-    ) -> CreateTaskResponse:
+    ) -> TaskCreateResponse:
         job_config = None
         if inputs:
             ctx = FlyteContextManager.current_context()
             python_interface_inputs = {
                 name: TypeEngine.guess_python_type(lt.type) for name, lt in task_template.interface.inputs.items()
             }
             native_inputs = TypeEngine.literal_map_to_kwargs(ctx, inputs, python_interface_inputs)
+
             logger.info(f"Create BigQuery job config with inputs: {native_inputs}")
             job_config = bigquery.QueryJobConfig(
                 query_parameters=[
                     bigquery.ScalarQueryParameter(name, pythonTypeToBigQueryType[python_interface_inputs[name]], val)
                     for name, val in native_inputs.items()
                 ]
             )
 
         custom = task_template.custom
-        project = custom["ProjectID"]
-        location = custom["Location"]
-        client = bigquery.Client(project=project, location=location)
+        client = bigquery.Client(project=custom["ProjectID"], location=custom["Location"])
         query_job = client.query(task_template.sql.statement, job_config=job_config)
-        metadata = Metadata(job_id=str(query_job.job_id), location=location, project=project)
 
-        return CreateTaskResponse(resource_meta=json.dumps(asdict(metadata)).encode("utf-8"))
+        return TaskCreateResponse(job_id=str(query_job.job_id))
 
-    def get(self, context: grpc.ServicerContext, resource_meta: bytes) -> GetTaskResponse:
+    def get(self, context: grpc.ServicerContext, job_id: str) -> TaskGetResponse:
         client = bigquery.Client()
-        metadata = Metadata(**json.loads(resource_meta.decode("utf-8")))
-        job = client.get_job(metadata.job_id, metadata.project, metadata.location)
-        if job.errors:
-            logger.error(job.errors.__str__())
-            context.set_code(grpc.StatusCode.INTERNAL)
-            context.set_details(job.errors.__str__())
-            return GetTaskResponse(resource=Resource(state=PERMANENT_FAILURE))
+        job = client.get_job(job_id)
         cur_state = convert_to_flyte_state(str(job.state))
         res = None
 
         if cur_state == SUCCEEDED:
             ctx = FlyteContextManager.current_context()
-            if job.destination:
-                output_location = (
-                    f"bq://{job.destination.project}:{job.destination.dataset_id}.{job.destination.table_id}"
-                )
-                res = literals.LiteralMap(
-                    {
-                        "results": TypeEngine.to_literal(
-                            ctx,
-                            StructuredDataset(uri=output_location),
-                            StructuredDataset,
-                            LiteralType(structured_dataset_type=StructuredDatasetType(format="")),
-                        )
-                    }
-                ).to_flyte_idl()
+            output_location = f"bq://{job.destination.project}:{job.destination.dataset_id}.{job.destination.table_id}"
+            res = literals.LiteralMap(
+                {
+                    "results": TypeEngine.to_literal(
+                        ctx,
+                        StructuredDataset(uri=output_location),
+                        StructuredDataset,
+                        LiteralType(structured_dataset_type=StructuredDatasetType(format="")),
+                    )
+                }
+            )
 
-        return GetTaskResponse(resource=Resource(state=cur_state, outputs=res))
+        return TaskGetResponse(state=cur_state, outputs=res.to_flyte_idl())
 
-    def delete(self, context: grpc.ServicerContext, resource_meta: bytes) -> DeleteTaskResponse:
+    def delete(self, context: grpc.ServicerContext, job_id: str) -> TaskDeleteResponse:
         client = bigquery.Client()
-        metadata = Metadata(**json.loads(resource_meta.decode("utf-8")))
-        client.cancel_job(metadata.job_id, metadata.project, metadata.location)
-        return DeleteTaskResponse()
+        client.cancel_job(job_id)
+        return TaskDeleteResponse()
 
 
-AgentRegistry.register(BigQueryAgent())
+BackendPluginRegistry.register(BigQueryPlugin())
```

### Comparing `flytekitplugins-bigquery-1.8.3/flytekitplugins/bigquery/task.py` & `flytekitplugins-bigquery-1.9.0a0/flytekitplugins/bigquery/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from google.cloud import bigquery
 from google.protobuf import json_format
 from google.protobuf.struct_pb2 import Struct
 
 from flytekit.configuration import SerializationSettings
 from flytekit.extend import SQLTask
-from flytekit.extend.backend.base_agent import AsyncAgentExecutorMixin
 from flytekit.models import task as _task_model
 from flytekit.types.structured import StructuredDataset
 
 
 @dataclass
 class BigQueryConfig(object):
     """
@@ -19,15 +18,15 @@
     """
 
     ProjectID: str
     Location: Optional[str] = None
     QueryJobConfig: Optional[bigquery.QueryJobConfig] = None
 
 
-class BigQueryTask(AsyncAgentExecutorMixin, SQLTask[BigQueryConfig]):
+class BigQueryTask(SQLTask[BigQueryConfig]):
     """
     This is the simplest form of a BigQuery Task, that can be used even for tasks that do not produce any output.
     """
 
     # This task is executed using the BigQuery handler in the backend.
     # https://github.com/flyteorg/flyteplugins/blob/43623826fb189fa64dc4cb53e7025b517d911f22/go/tasks/plugins/webapi/bigquery/plugin.go#L34
     _TASK_TYPE = "bigquery_query_job_task"
@@ -41,15 +40,16 @@
         output_structured_dataset_type: Optional[Type[StructuredDataset]] = None,
         **kwargs,
     ):
         """
         To be used to query BigQuery Tables.
 
         :param name: Name of this task, should be unique in the project
-        :param query_template: The actual query to run. We use Flyte's Golang templating format for Query templating. Refer to the templating documentation
+        :param query_template: The actual query to run. We use Flyte's Golang templating format for Query templating.
+          Refer to the templating documentation
         :param task_config: BigQueryConfig object
         :param inputs: Name and type of inputs specified as an ordered dictionary
         :param output_structured_dataset_type: If some data is produced by this query, then you can specify the output StructuredDataset type
         :param kwargs: All other args required by Parent type - SQLTask
         """
         outputs = None
         if output_structured_dataset_type is not None:
@@ -77,7 +77,10 @@
         s = Struct()
         s.update(config)
         return json_format.MessageToDict(s)
 
     def get_sql(self, settings: SerializationSettings) -> Optional[_task_model.Sql]:
         sql = _task_model.Sql(statement=self.query_template, dialect=_task_model.Sql.Dialect.ANSI)
         return sql
+
+    def execute(self, **kwargs) -> Any:
+        raise Exception("Cannot run a SQL Task natively, please mock.")
```

### Comparing `flytekitplugins-bigquery-1.8.3/flytekitplugins_bigquery.egg-info/PKG-INFO` & `flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.8.3
+Version: 1.9.0a0
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.8.3/setup.py` & `flytekitplugins-bigquery-1.9.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "bigquery"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "google-cloud-bigquery"]
 
-__version__ = "1.8.3"
+__version__ = "1.9.0a0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Bigquery plugins for flytekit",
```

