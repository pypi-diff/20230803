# Comparing `tmp/ibm_data_engine-0.1.1.tar.gz` & `tmp/ibm_data_engine-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm_data_engine-0.1.1.tar", max compression
+gzip compressed data, was "ibm_data_engine-0.1.2.tar", max compression
```

## Comparing `ibm_data_engine-0.1.1.tar` & `ibm_data_engine-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11358 2023-01-10 18:48:48.587858 ibm_data_engine-0.1.1/LICENSE
--rw-r--r--   0        0        0     2757 2023-01-10 18:48:48.587858 ibm_data_engine-0.1.1/README.md
--rw-r--r--   0        0        0      906 2023-01-10 18:48:48.587858 ibm_data_engine-0.1.1/ibm_data_engine/__init__.py
--rw-r--r--   0        0        0    28894 2023-01-10 18:48:48.587858 ibm_data_engine-0.1.1/ibm_data_engine/data_engine_offline_store.py
--rw-r--r--   0        0        0     1502 2023-01-10 18:48:48.587858 ibm_data_engine-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 ibm_data_engine-0.1.1/setup.py
--rw-r--r--   0        0        0     4000 1970-01-01 00:00:00.000000 ibm_data_engine-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-01-04 14:27:30.628584 ibm_data_engine-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2757 2023-01-04 14:27:30.628584 ibm_data_engine-0.1.2/README.md
+-rw-r--r--   0        0        0      906 2023-01-04 15:05:40.002084 ibm_data_engine-0.1.2/ibm_data_engine/__init__.py
+-rw-r--r--   0        0        0    28894 2023-01-05 14:41:43.460407 ibm_data_engine-0.1.2/ibm_data_engine/data_engine_offline_store.py
+-rw-r--r--   0        0        0     1502 2023-08-03 14:59:27.177599 ibm_data_engine-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4000 1970-01-01 00:00:00.000000 ibm_data_engine-0.1.2/PKG-INFO
```

### Comparing `ibm_data_engine-0.1.1/LICENSE` & `ibm_data_engine-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm_data_engine-0.1.1/README.md` & `ibm_data_engine-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ibm_data_engine-0.1.1/ibm_data_engine/__init__.py` & `ibm_data_engine-0.1.2/ibm_data_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_data_engine-0.1.1/ibm_data_engine/data_engine_offline_store.py` & `ibm_data_engine-0.1.2/ibm_data_engine/data_engine_offline_store.py`

 * *Files identical despite different names*

### Comparing `ibm_data_engine-0.1.1/pyproject.toml` & `ibm_data_engine-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ibm-data-engine"
-version = "0.1.1"
+version = "0.1.2"
 description = "Feast offline feature store implementation backed by the IBM Cloud Data Engine"
 license = "Apache-2.0"
 authors = [
     "Michal Siedlaczek <michal.siedlaczek@ibm.com>",
     "Abhay Ratnaparkhi <abhay.ratnaparkhi1@ibm.com>",
     "Jay Hou <jhou@us.ibm.com>",
 ]
@@ -27,25 +27,25 @@
     "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 # We current have issues installing dependencies for 3.11. We will remove <3.11 constraint as soon
 # as the problem gets resolved.
 python = "^3.8,<3.11"
-feast = "^0.25.0"
+feast = "^0.26.0"
 ibmcloudsql = "^0.5.11"
 
 [tool.poetry.dev-dependencies]
 black = "^22.10"
 diff-cover = "^7"
 freezegun = "^1"
 hypothesis = "^6"
 isort = "^5"
 pylint = "^2"
-pytest = "^6"
+pytest = "^7"
 pytest-cov = "^4"
 testfixtures = "^7.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ibm_data_engine-0.1.1/setup.py` & `ibm_data_engine-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,138 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ibm-data-engine
+Version: 0.1.2
+Summary: Feast offline feature store implementation backed by the IBM Cloud Data Engine
+Home-page: https://github.com/IBM/feast-ibm
+License: Apache-2.0
+Author: Michal Siedlaczek
+Author-email: michal.siedlaczek@ibm.com
+Maintainer: Michal Siedlaczek
+Maintainer-email: michal.siedlaczek@ibm.com
+Requires-Python: >=3.8,<3.11
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Environment :: Plugins
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: feast (>=0.26.0,<0.27.0)
+Requires-Dist: ibmcloudsql (>=0.5.11,<0.6.0)
+Project-URL: Repository, https://github.com/IBM/feast-ibm
+Description-Content-Type: text/markdown
+
+[Feast](https://feast.dev/) plugin for IBM Cloud.  
+This plugin implements Feast's offline store backed using [IBM Cloud Data Engine](https://www.ibm.com/cloud/data-engine) and [IBM Cloud Object Storage](https://www.ibm.com/cloud/object-storage)
+
+# Installation
+
+Project dependencies can be installed in a dedicated virtual environment
+by running the following command:
+
+```bash
+poetry install
+```
+
+# Testing and Linting
+
+```bash
+poetry run pytest tests/
+poetry run pylint ibm_data_engine
+```
+
+# Test with Feast
+
+You use it with [Feast](https://feast.dev/) by defining your offline store and data sources.
+The instructions below illustrate how it can be used in
+[feast-ibm-quickstart](https://github.com/IBM/feast-ibm-quickstart).
+
+## Define dependency
+
+This library is currently not published in [PyPI](https://pypi.org/); you will have to
+point to the repository directly. The easiest way to do it is to clone
+the repository, and define the dependency as a path in `feast-ibm-quickstart`.
+
+```toml
+ibm-data-engine = { path = "/path/to/ibm-data-engine" }
+```
+
+After running `poetry update`, you should be able to use the IBM Cloud
+Data Engine offline store.
+
+## Define data source
+
+You can modify the `src/feature_repo/example_repo.py` file to use the new data
+source. Below is the minimal example of the file:
+
+```python
+from ibm_data_engine import DataEngineDataSource
+driver_stats_source = DataEngineDataSource(
+    name="driver_hourly_stats_source",
+    table="driver_stats_demo",
+    timestamp_field="event_timestamp",
+)
+```
+
+## Define offline store
+
+Then, `feature_repo/feature_store.yaml` must configure the offline store.
+
+```yaml
+project: test_plugin
+entity_key_serialization_version: 2
+registry: data/registry.db
+provider: local
+online_store:
+    type: redis
+    connection_string: ${REDIS_HOST}:${REDIS_PORT},username=${REDIS_USERNAME},password=${REDIS_PASSWORD},ssl=true,ssl_ca_certs=${REDIS_CERT_PATH},db=0
+
+offline_store:
+    type: ibm_data_engine.DataEngineOfflineStore
+    api_key: ${DATA_ENGINE_API_KEY}
+    instance_crn: ${DATA_ENGINE_INSTANCE_CRN}
+    target_cos_url: ${IBM_CLOUD_OBJECT_STORE_URL}
+```
+
+Notice that you must define the environment variables:
+ * `IBM_CLOUD_OBJECT_STORE_URL`
+ * `REDIS_HOST`
+ * `REDIS_PORT`
+ * `REDIS_PASSWORD`
+ * `REDIS_CERT_PATH`
+ * `DATA_ENGINE_API_KEY`
+ * `DATA_ENGINE_INSTANCE_CRN`
+
+## Apply
+
+To apply the definitions to the registry, run:
+
+```
+poetry run feast -c ./feature_repo apply
+```
+
+## Training
+
+Run training by retrieving historical feature information from feature store
+```
+poetry run python training.py
+```
+## Materialize
+
+To materialize to Redis, run:
+
+```
+poetry run feast -c ./ materialize '<START_TIMESTAMP>'  '<END_TIMESTAMP>'
+```
+## Inference
+
+```
+poetry run python inference.py
+```
 
-packages = \
-['ibm_data_engine']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['feast>=0.25.0,<0.26.0', 'ibmcloudsql>=0.5.11,<0.6.0']
-
-setup_kwargs = {
-    'name': 'ibm-data-engine',
-    'version': '0.1.1',
-    'description': 'Feast offline feature store implementation backed by the IBM Cloud Data Engine',
-    'long_description': '[Feast](https://feast.dev/) plugin for IBM Cloud.  \nThis plugin implements Feast\'s offline store backed using [IBM Cloud Data Engine](https://www.ibm.com/cloud/data-engine) and [IBM Cloud Object Storage](https://www.ibm.com/cloud/object-storage)\n\n# Installation\n\nProject dependencies can be installed in a dedicated virtual environment\nby running the following command:\n\n```bash\npoetry install\n```\n\n# Testing and Linting\n\n```bash\npoetry run pytest tests/\npoetry run pylint ibm_data_engine\n```\n\n# Test with Feast\n\nYou use it with [Feast](https://feast.dev/) by defining your offline store and data sources.\nThe instructions below illustrate how it can be used in\n[feast-ibm-quickstart](https://github.com/IBM/feast-ibm-quickstart).\n\n## Define dependency\n\nThis library is currently not published in [PyPI](https://pypi.org/); you will have to\npoint to the repository directly. The easiest way to do it is to clone\nthe repository, and define the dependency as a path in `feast-ibm-quickstart`.\n\n```toml\nibm-data-engine = { path = "/path/to/ibm-data-engine" }\n```\n\nAfter running `poetry update`, you should be able to use the IBM Cloud\nData Engine offline store.\n\n## Define data source\n\nYou can modify the `src/feature_repo/example_repo.py` file to use the new data\nsource. Below is the minimal example of the file:\n\n```python\nfrom ibm_data_engine import DataEngineDataSource\ndriver_stats_source = DataEngineDataSource(\n    name="driver_hourly_stats_source",\n    table="driver_stats_demo",\n    timestamp_field="event_timestamp",\n)\n```\n\n## Define offline store\n\nThen, `feature_repo/feature_store.yaml` must configure the offline store.\n\n```yaml\nproject: test_plugin\nentity_key_serialization_version: 2\nregistry: data/registry.db\nprovider: local\nonline_store:\n    type: redis\n    connection_string: ${REDIS_HOST}:${REDIS_PORT},username=${REDIS_USERNAME},password=${REDIS_PASSWORD},ssl=true,ssl_ca_certs=${REDIS_CERT_PATH},db=0\n\noffline_store:\n    type: ibm_data_engine.DataEngineOfflineStore\n    api_key: ${DATA_ENGINE_API_KEY}\n    instance_crn: ${DATA_ENGINE_INSTANCE_CRN}\n    target_cos_url: ${IBM_CLOUD_OBJECT_STORE_URL}\n```\n\nNotice that you must define the environment variables:\n * `IBM_CLOUD_OBJECT_STORE_URL`\n * `REDIS_HOST`\n * `REDIS_PORT`\n * `REDIS_PASSWORD`\n * `REDIS_CERT_PATH`\n * `DATA_ENGINE_API_KEY`\n * `DATA_ENGINE_INSTANCE_CRN`\n\n## Apply\n\nTo apply the definitions to the registry, run:\n\n```\npoetry run feast -c ./feature_repo apply\n```\n\n## Training\n\nRun training by retrieving historical feature information from feature store\n```\npoetry run python training.py\n```\n## Materialize\n\nTo materialize to Redis, run:\n\n```\npoetry run feast -c ./ materialize \'<START_TIMESTAMP>\'  \'<END_TIMESTAMP>\'\n```\n## Inference\n\n```\npoetry run python inference.py\n```\n',
-    'author': 'Michal Siedlaczek',
-    'author_email': 'michal.siedlaczek@ibm.com',
-    'maintainer': 'Michal Siedlaczek',
-    'maintainer_email': 'michal.siedlaczek@ibm.com',
-    'url': 'https://github.com/IBM/feast-ibm',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
-
-
-setup(**setup_kwargs)
```

