# Comparing `tmp/dcicutils-7.6.0.2b9.tar.gz` & `tmp/dcicutils-7.7.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.6.0.2b9.tar", max compression
+gzip compressed data, was "dcicutils-7.7.0.1b1.tar", max compression
```

## Comparing `dcicutils-7.6.0.2b9.tar` & `dcicutils-7.7.0.1b1.tar`

### file list

```diff
@@ -1,54 +1,53 @@
--rw-r--r--   0        0        0     1102 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/README.rst
--rw-r--r--   0        0        0        0 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3763 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68885 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27797 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    38905 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    30631 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20511 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   156269 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    13576 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     4387 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/pyproject.toml
--rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b9/setup.py
--rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b9/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/README.rst
+-rw-r--r--   0        0        0        0 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3763 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/common.py
+-rw-r--r--   0        0        0    11113 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68885 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-08-03 19:43:26.307244 dcicutils-7.7.0.1b1/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0     6881 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/item_model_utils.py
+-rw-r--r--   0        0        0    11502 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27661 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    30631 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20234 2023-08-03 19:43:26.311245 dcicutils-7.7.0.1b1/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   156269 2023-08-03 19:43:26.315245 dcicutils-7.7.0.1b1/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-08-03 19:43:26.315245 dcicutils-7.7.0.1b1/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-08-03 19:43:26.315245 dcicutils-7.7.0.1b1/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-08-03 19:43:26.315245 dcicutils-7.7.0.1b1/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    13576 2023-08-03 19:43:26.315245 dcicutils-7.7.0.1b1/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-08-03 19:43:26.315245 dcicutils-7.7.0.1b1/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-08-03 19:43:26.315245 dcicutils-7.7.0.1b1/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-08-03 19:43:26.315245 dcicutils-7.7.0.1b1/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-08-03 19:43:26.315245 dcicutils-7.7.0.1b1/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1174 2023-08-03 19:43:26.315245 dcicutils-7.7.0.1b1/dcicutils/testing_utils.py
+-rw-r--r--   0        0        0     1769 2023-08-03 19:43:26.315245 dcicutils-7.7.0.1b1/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3948 2023-08-03 19:43:26.315245 dcicutils-7.7.0.1b1/pyproject.toml
+-rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 dcicutils-7.7.0.1b1/setup.py
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.7.0.1b1/PKG-INFO
```

### Comparing `dcicutils-7.6.0.2b9/LICENSE.txt` & `dcicutils-7.7.0.1b1/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License
 
-Copyright 2017-2023 President and Fellows of Harvard College
+Copyright 2017 President and Fellows of Harvard College.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dcicutils-7.6.0.2b9/README.rst` & `dcicutils-7.7.0.1b1/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/base.py` & `dcicutils-7.7.0.1b1/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/beanstalk_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/cloudformation_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/codebuild_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/command_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/common.py` & `dcicutils-7.7.0.1b1/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/creds_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/data_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/deployment_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/diff_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/docker_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/ecr_scripts.py` & `dcicutils-7.7.0.1b1/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/ecr_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/ecs_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/env_base.py` & `dcicutils-7.7.0.1b1/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/env_manager.py` & `dcicutils-7.7.0.1b1/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/env_scripts.py` & `dcicutils-7.7.0.1b1/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/env_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/env_utils_legacy.py` & `dcicutils-7.7.0.1b1/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/es_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/exceptions.py` & `dcicutils-7.7.0.1b1/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/ff_mocks.py` & `dcicutils-7.7.0.1b1/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/ff_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/function_cache_decorator.py` & `dcicutils-7.7.0.1b1/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/glacier_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/jh_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/kibana/dashboards.json` & `dcicutils-7.7.0.1b1/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/kibana/readme.md` & `dcicutils-7.7.0.1b1/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/lang_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/lang_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,21 +194,21 @@
             return result + qualifier_suffix
 
     _USE_AN = {}
 
     _PREFIX_PATTERN_FOR_A = re.compile("^(%s)" % "|".join({
         "[^aeioux]",  # Consonants other than x need 'a' (bicycle, dog, etc.)
         "x[aeiouy]",  # x followed by any vowel makes it pronounceable like a consonant (xylophone), so needs 'a'
-        "uni([^aeiuym]|[aeiuy][^aeiy])",  # things starting with "uni" are pronounced like "yuni", so need "a"
+        "uni([^aeiuym]|[aeiuy][^aeiy])",  # things starting with with "uni" are pronounced like "yuni", so need "a"
     }), flags=re.IGNORECASE)
 
     @classmethod
     def select_a_or_an(cls, word):
         """
-        Uses a heuristic to try to select the appropriate article ("a" or "an") for a given English noun.
+        Uses a heuristic to try to select the appropriate article ('a' or 'an') for a given English noun.
         select_a_or_an("gene") => 'a'
         select_a_or_an("accession") => 'an'
         """
 
         return "a" if cls._PREFIX_PATTERN_FOR_A.match(word) else "an"
 
     @classmethod
@@ -274,15 +274,15 @@
         "The only possible option is foo."
         >>> must_be_one_of(['foo', 'bar'])
         "Possible options are foo and bar."
         >>> must_be_one_of(['foo', 'bar', 'baz'])
         "Possible options are foo, bar and baz."
 
         :param items: the items to enumerate
-        :param possible: whether to use the word 'possible' before the given kind (default True), or a string to use
+        :param possible: whether to use the word 'possible' before the given kind (default True), or an string to use
         :param kind: the kind of items being enumerated (default "option")
         :param quote: whether to put quotes around each option
         :param capitalize: whether to capitalize the first letter of the sentence (default True)
         :param joiner: the joining function to join the items (default if None is just a commas-separated list)
         :param joiner_options: additional (keyword) options to be used with a joiner function if one is supplied
         """
 
@@ -347,30 +347,29 @@
                                  f" ({cls.disjoined_list(sorted(list(cls._BE_TENSES.keys())))})"
                                  f" nor a modal ({cls.disjoined_list(sorted(list(cls._MODALS)))}).")
         return is_or_are  # possibly in some other tense. :)
 
     @classmethod
     def there_are(cls, items, *, kind: str = "thing", count: Optional[int] = None, there: str = "there",
                   capitalize=True, joiner=None, zero: object = "no", punctuate=None, punctuate_none=None,
-                  use_article=False, show=True, context=None, tense='present', punctuation_mark: str = ".",
+                  use_article=False, show=True, context=None, tense='present',
                   **joiner_options) -> str:
         """
         Constructs a sentence that enumerates a set of things.
 
         :param items: the items to enumerate
         :param kind: the kind of items being enumerated (default "thing")
         :param count: the number of items (defaults to the result of 'len(items)')
         :param there: the demonstrative or noun phrase that starts the sentence (default "there")
         :param capitalize: whether to capitalize the first letter of the sentence (default True)
         :param joiner: the joining function to join the items (default if None is just a commas-separated list)
         :param zero: the value to print instead of a numeric zero (default "no")
         :param punctuate: in the case of one or more values (not zero), whether to end with a period (default False)
         :param punctuate_none: in the case of no values or not showing values, whether to end with a period
                (default True if show is True, and otherwise is the same as the value of punctuate)
-        :param punctuation_mark: if specified, something to use at the end if punctuating
         :param use_article: whether to put 'a' or 'an' in front of each option (default False)
         :param joiner_options: additional (keyword) options to be used with a joiner function if one is supplied
         :param show: whether to show the items if there are any (default True)
         :param context: an optional prepositional phrase indicating the context of the item(s) (default None)
         :param tense: one of 'past', 'present', 'future', 'conditional', or 'hypothetical' for the verbs used
 
         By far the most common uses are likely to be:
@@ -403,26 +402,26 @@
         n = len(items) if count is None else count
         # If the items is not in the tenses table, it's assumed to be a modal like 'might', 'may', 'must', 'can' etc.
         is_or_are = cls._conjugate_be(count=n, tense=tense)
         part1 = f"{there} {is_or_are} {n_of(n, kind, num_format=lambda n, thing: zero if n == 0 else None)}"
         if context:
             part1 += f" {context}"
         if n == 0 or not show:
-            punctuation = punctuation_mark if punctuate_none else ""
+            punctuation = "." if punctuate_none else ""
             return part1 + punctuation
         else:
             if use_article:
                 items = [a_or_an(str(item)) for item in items]
             else:
                 items = [str(item) for item in items]
             if joiner is None:
                 joined = ", ".join(items)
             else:
                 joined = joiner(items, **joiner_options)
-            punctuation = punctuation_mark if punctuate else ""
+            punctuation = "." if punctuate else ""
             return f"{part1}: {joined}{punctuation}"
 
     @classmethod
     def _time_count_formatter(cls, n, unit):
         ignored(unit)
         if isinstance(n, float):
             return ("%.6f" % n).rstrip('0').rstrip('.')
@@ -469,15 +468,15 @@
     def parse_relative_time_string(cls, s):
         parts = [x for x in s.split(' ') if x != '']
         if len(parts) % 2 != 0:
             raise ValueError(f"Relative time strings are an even number of tokens"
                              f" of the form '<n1> <unit1> <n2> <unit2>...': {s!r}")
         kwargs = {}
         for i in range(len(parts) // 2):
-            # Canonicalize "1 week" or "1 weeks" to "weeks": 1.0 for inclusion as kwarg to timedelta
+            # Canonicalize "1 week" or "1 weeks" to "weeks": 1.0 for inclusion as kwarg to to timedelta
             # Uses specialized knowledge that all time units don't end in "s" but pluralize with "+s"
             value = float(parts[2 * i])
             units = parts[2 * i + 1].rstrip(',s') + "s"
             kwargs[units] = value
         try:
             return datetime.timedelta(**kwargs)
         except Exception:
```

### Comparing `dcicutils-7.6.0.2b9/dcicutils/log_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/misc_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/obfuscation_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/opensearch_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/project_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/qa_checkers.py` & `dcicutils-7.7.0.1b1/dcicutils/qa_checkers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import re
 import toml
 import warnings
 
 from collections import defaultdict
 from typing import Optional, List, Dict, Type
 from typing_extensions import Literal
-from .contribution_utils import Contributions
 from .lang_utils import conjoined_list, n_of, there_are
 from .misc_utils import PRINT, remove_prefix, remove_suffix, getattr_customized, CustomizableProperty
 
 
 QA_EXCEPTION_PATTERN = re.compile(r"[#].*\b[N][O][Q][A]\b", re.IGNORECASE)
 
 
@@ -433,15 +432,7 @@
         detail = ""
         n = 0
         for file, matches in uses.items():
             n += len(matches)
             detail += f"\n In {file}, {summarize(matches)}."
         message = f"{n_of(n, 'problem')} detected:" + detail
         raise AssertionError(message)
-
-
-class ContributionsChecker:
-
-    @classmethod
-    def validate(cls):
-        contributions = Contributions()  # no repo specified, so use current directory
-        contributions.show_repo_contributors(error_class=AssertionError)
```

### Comparing `dcicutils-7.6.0.2b9/dcicutils/qa_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/redis_tools.py` & `dcicutils-7.7.0.1b1/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/redis_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/s3_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.7.0.1b1/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/secrets_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/snapshot_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/task_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/dcicutils/trace_utils.py` & `dcicutils-7.7.0.1b1/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b9/pyproject.toml` & `dcicutils-7.7.0.1b1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.6.0.2b9"
+version = "7.7.0.1b1"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
@@ -66,36 +66,30 @@
 boto3-stubs = "1.18.23"
 coverage = ">=7.2.3"
 # Loaded manually in GA workflow for coverage because a dependency on 2to3
 # in its docopts dependency makes a problem for laoding it here in poetry. -kmp 7-Apr-2023
 # coveralls = ">=3.3.1"
 flake8 = ">=3.9.2"
 flaky = ">=3.7.0"
-pip-licenses = "^3.5.5"
 pytest = ">=4.5.0"
 pytest-cov = ">=2.7.1"
 pytest-mock = ">=1.11.0"
 pytest-redis = "^2.0.0"
 pytest-runner = ">=5.1"
 
 
 [tool.poetry.scripts]
 publish-to-pypi = "dcicutils.scripts.publish_to_pypi:main"
-show-contributors = "dcicutils.contribution_scripts:show_contributors_main"
+
 
 [tool.pytest.ini_options]
 addopts = "--basetemp=/tmp/pytest"
 redis_exec = "/usr/local/bin/redis-server"
 filterwarnings = [
-    # TODO: These next two are about use of the Version class:
-    "ignore:distutils Version classes are deprecated. Use packaging.version instead.:DeprecationWarning",
-    "ignore:Setuptools is replacing distutils.:UserWarning",
-    # This is a pip-licenses problem (still present in 3.5.5):
-    "ignore:pkg_resources is deprecated as an API:DeprecationWarning",
-    "ignore:Boto3 will no longer support Python 3.7 starting December 13, 2023.*:",
+    "ignore::DeprecationWarning: distutils Version classes are deprecated. Use packaging.version instead.",
 ]
 markers = [
     "working: test should work",
     "integrated: an integration test",
     "integratedx: an excludable integration test, redundantly testing functionality also covered by a unit test",
     "unit: a proper unit test",
     "file_operation: a test that utilizes files",
```

### Comparing `dcicutils-7.6.0.2b9/setup.py` & `dcicutils-7.7.0.1b1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,21 +29,20 @@
  'toml>=0.10.1,<1',
  'tqdm>=4.65.0,<5.0.0',
  'typing-extensions>=3.8',
  'urllib3>=1.26.6,<2.0.0',
  'webtest>=2.0.34,<3.0.0']
 
 entry_points = \
-{'console_scripts': ['publish-to-pypi = dcicutils.scripts.publish_to_pypi:main',
-                     'show-contributors = '
-                     'dcicutils.contribution_scripts:show_contributors_main']}
+{'console_scripts': ['publish-to-pypi = '
+                     'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.6.0.2b9',
+    'version': '7.7.0.1b1',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.6.0.2b9/PKG-INFO` & `dcicutils-7.7.0.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.6.0.2b9
+Version: 7.7.0.1b1
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

