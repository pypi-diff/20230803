# Comparing `tmp/amazon_sagemaker_jupyter_scheduler-2.1.0.tar.gz` & `tmp/amazon_sagemaker_jupyter_scheduler-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon_sagemaker_jupyter_scheduler-2.1.0.tar", last modified: Thu Jul 13 17:45:27 2023, max compression
+gzip compressed data, was "amazon_sagemaker_jupyter_scheduler-2.2.0.tar", last modified: Tue Aug  1 18:15:48 2023, max compression
```

## Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0.tar` & `amazon_sagemaker_jupyter_scheduler-2.2.0.tar`

### file list

```diff
@@ -1,224 +1,223 @@
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.709317 amazon_sagemaker_jupyter_scheduler-2.1.0/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/.eslintignore
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1026 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/.eslintrc.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1605 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/.gitignore
--rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/.prettierignore
--rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/.prettierrc
--rw-r--r--   0 p4admin  (12569) amazon     (100)      739 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/Config
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2329 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/DEVELOPMENT.md
--rw-r--r--   0 p4admin  (12569) amazon     (100)      686 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/MANIFEST.in
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1174 2023-07-13 17:45:27.709317 amazon_sagemaker_jupyter_scheduler-2.1.0/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)      347 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/README.md
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2046 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/RELEASE.md
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.681318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      806 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      455 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/_version.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.681318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      163 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/base_advanced_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5969 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    13333 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2541 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/app_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      465 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/aws_config.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.669318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/botocore_model/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.669318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.681318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/
--rw-r--r--   0 p4admin  (12569) amazon     (100)  1377688 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/service-2.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)    19161 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/clients.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2538 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/cron_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2060 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/deletable_resource.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1501 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/environment_detector.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5211 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3338 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/error_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      820 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/extension.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5757 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/file_uploader.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6084 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/handlers.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    65897 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1533 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.685318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4948 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/package.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.669318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.669318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.685318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1130 2023-07-13 17:45:16.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4834 2023-07-13 17:45:16.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.689318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1875 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/144.9be27e93647ef0e84863.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   242036 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      166 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)    26299 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)   106222 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      412 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)    13283 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1875 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   209775 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      706 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4059 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)    52588 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/993.84c00bb76b4448d8ce3f.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8346 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.299f9d522c52a504280b.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2023-07-13 17:45:16.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/style.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    66200 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6440 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/logging.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    31271 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/model_converter.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3898 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/models.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.689318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      759 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      528 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/revenue.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9468 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4682 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3788 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/tags.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2930 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      498 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/s3_uri.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    44823 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/scheduler.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.693318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/__init__.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.693318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/helpers/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/helpers/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      913 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.693318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/providers/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/providers/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9555 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8033 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    14065 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3180 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1145 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    17404 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1694 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2149 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1895 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1529 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1512 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6823 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2280 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3519 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5843 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    28697 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2101 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    34195 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      427 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_utils.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2805 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/utils.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.681318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1174 2023-07-13 17:45:27.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9270 2023-07-13 17:45:27.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-07-13 17:45:27.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-07-13 17:45:27.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 p4admin  (12569) amazon     (100)      208 2023-07-13 17:45:27.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/requires.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-13 17:45:27.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/top_level.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)      261 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/babel.config.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)       73 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/custom.d.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      827 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/jest.config.base.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      510 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/jest.config.js
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.693318 amazon_sagemaker_jupyter_scheduler-2.1.0/jupyter-config/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.693318 amazon_sagemaker_jupyter_scheduler-2.1.0/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      109 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/jupyter-config/jupyter_server_config.d/amazon_sagemaker_jupyter_scheduler.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)      306 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/jupyter-config/jupyter_server_config.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)   965893 2023-07-13 17:45:15.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/package-lock.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4834 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/package.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)      127 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/pyproject.toml
--rw-r--r--   0 p4admin  (12569) amazon     (100)      133 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/requirements.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2023-07-13 17:45:27.709317 amazon_sagemaker_jupyter_scheduler-2.1.0/setup.cfg
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3069 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/setup.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.693318 amazon_sagemaker_jupyter_scheduler-2.1.0/src/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.693318 amazon_sagemaker_jupyter_scheduler-2.1.0/src/__mocks__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/__mocks__/fileMock.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)    12302 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/CreateNotebookJobForm.spec.tsx
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)     4348 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/VpcCheckbox.spec.tsx
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)    13449 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/initalValueHelpers.spec.ts
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)    11135 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/validationHelpers.spec.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.669318 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      964 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/Link.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      754 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/RouterLink.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/__test__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1005 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/__test__/Link.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      609 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/__test__/RouterLink.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      184 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/types.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/selectinput/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1583 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/selectinput/SelectInput.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       56 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/selectinput/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      967 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/selectinput/types.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1626 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/TextInput.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1656 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/__tests__/TextInput.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       54 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2932 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      206 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/types.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1348 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/Tooltip.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1040 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/__tests__/Tooltip.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       27 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      553 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/styles.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/constants/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8440 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/constants/common.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       53 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/constants/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       99 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/constants/kernels.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      186 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.701317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/plugins/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3429 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/plugins/ScheduleNotebookDisablerPlugin.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1455 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/plugins/ScheduleNotebookPlugin.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       92 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/plugins/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3328 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/themeProvider.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.701317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/types/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      420 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/types/images.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       82 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/types/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      141 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/types/kernels.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      132 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/types/sagemaker.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.701317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1929 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/PluginEnvironmentProvider.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.701317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1833 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      123 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/common.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1528 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/images.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      108 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1205 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/kernels.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1017 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/rendering.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.701317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4427 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJob.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.705317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.705317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/
--rw-r--r--   0 p4admin  (12569) amazon     (100)    17765 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.705317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3900 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3230 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1094 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.705317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3551 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       55 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      285 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5596 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    14732 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1229 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/InputContainer.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.705317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2737 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      712 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1280 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3138 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1554 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.709317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1613 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6035 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      552 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    12172 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    64113 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      781 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1305 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       41 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8199 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1727 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2216 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/mockResponses.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2815 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9250 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/tsconfig.base.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)      304 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/tsconfig.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.103032 amazon_sagemaker_jupyter_scheduler-2.2.0/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/.eslintignore
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1026 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/.eslintrc.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1605 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/.gitignore
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/.prettierignore
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/.prettierrc
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      739 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/Config
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2329 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/DEVELOPMENT.md
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      686 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/MANIFEST.in
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1174 2023-08-01 18:15:48.103032 amazon_sagemaker_jupyter_scheduler-2.2.0/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      347 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/README.md
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2046 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/RELEASE.md
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.079033 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      806 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      455 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/_version.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.083032 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      163 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/base_advanced_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5969 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    13333 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2541 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/app_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      465 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/aws_config.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.071033 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/botocore_model/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.071033 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.083032 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)  1377688 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/service-2.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    19161 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/clients.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2538 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/cron_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2060 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/deletable_resource.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1501 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/environment_detector.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5211 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3338 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/error_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      716 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/extension.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5757 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/file_uploader.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3670 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/handlers.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    65897 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1533 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.083032 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4948 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/package.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.071033 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.071033 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.083032 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1130 2023-08-01 18:15:38.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4832 2023-08-01 18:15:38.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.087032 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1875 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/144.9be27e93647ef0e84863.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   242036 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      166 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    26299 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    51387 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/315.59fba34ec08e26375d68.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   106222 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      412 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    13283 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1875 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   209775 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      706 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4059 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8282 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.3b333e0e590d8edb68a6.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2023-08-01 18:15:38.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/style.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    66200 2023-08-01 18:15:47.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6440 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/logging.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    31271 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/model_converter.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3898 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/models.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.087032 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/providers/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/providers/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      759 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      528 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/providers/revenue.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9468 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4682 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3788 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/providers/tags.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2930 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      498 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/s3_uri.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    44823 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/scheduler.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.091032 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/__init__.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.091032 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/helpers/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/helpers/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      913 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.091032 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/providers/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/providers/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9555 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8033 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    13934 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3180 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1439 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    17404 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1694 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2149 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1895 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1529 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1512 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6823 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2280 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3519 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5843 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    28697 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2101 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    34195 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      427 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_utils.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2805 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/utils.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.083032 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler.egg-info/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1174 2023-08-01 18:15:48.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9223 2023-08-01 18:15:48.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-08-01 18:15:48.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-08-01 18:15:48.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      208 2023-08-01 18:15:48.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler.egg-info/requires.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-08-01 18:15:48.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      261 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/babel.config.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       73 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/custom.d.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      827 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/jest.config.base.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      510 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/jest.config.js
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.091032 amazon_sagemaker_jupyter_scheduler-2.2.0/jupyter-config/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.091032 amazon_sagemaker_jupyter_scheduler-2.2.0/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      109 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/jupyter-config/jupyter_server_config.d/amazon_sagemaker_jupyter_scheduler.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      306 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/jupyter-config/jupyter_server_config.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   965893 2023-08-01 18:15:37.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/package-lock.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4832 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/package.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      127 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/pyproject.toml
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      133 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/requirements.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2023-08-01 18:15:48.103032 amazon_sagemaker_jupyter_scheduler-2.2.0/setup.cfg
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3069 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/setup.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.091032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.091032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/__mocks__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/__mocks__/fileMock.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.091032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/__tests__/
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)    12302 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/__tests__/CreateNotebookJobForm.spec.tsx
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)     4348 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/__tests__/VpcCheckbox.spec.tsx
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)    13449 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/__tests__/initalValueHelpers.spec.ts
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)    11135 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/__tests__/validationHelpers.spec.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.071033 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.095032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/link/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      964 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/link/Link.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      754 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/link/RouterLink.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.095032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/link/__test__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1005 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/link/__test__/Link.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      609 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/link/__test__/RouterLink.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/link/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/link/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      184 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/link/types.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.095032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/selectinput/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1583 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/selectinput/SelectInput.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       56 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/selectinput/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      967 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/selectinput/types.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.095032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/textinput/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1626 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/textinput/TextInput.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.095032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/textinput/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1656 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/textinput/__tests__/TextInput.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       54 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/textinput/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2932 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/textinput/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      206 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/textinput/types.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.095032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/tooltip/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1348 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/tooltip/Tooltip.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.095032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/tooltip/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1040 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/tooltip/__tests__/Tooltip.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       27 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/tooltip/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      553 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/tooltip/styles.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.095032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/constants/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8364 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/constants/common.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       53 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/constants/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       99 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/constants/kernels.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       94 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.095032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/plugins/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1455 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/plugins/ScheduleNotebookPlugin.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       42 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/plugins/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3328 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/themeProvider.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.095032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/types/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      420 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/types/images.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       82 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/types/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      141 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/types/kernels.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      132 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/types/sagemaker.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.099032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/utils/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1929 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/utils/PluginEnvironmentProvider.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.099032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/utils/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1833 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      123 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/utils/common.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1528 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/utils/images.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      108 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/utils/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1205 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/utils/kernels.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1017 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/utils/rendering.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.099032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4427 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJob.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.099032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.099032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    17765 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.099032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3900 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3230 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1094 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.099032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3551 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       55 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      285 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5596 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    14732 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1229 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/InputContainer.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.099032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/JobEnvironment/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2737 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      712 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/JobEnvironment/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1280 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3138 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1554 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:15:48.103032 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1613 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6035 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      552 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    12172 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    64113 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      781 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1305 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       41 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8199 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1727 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2216 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/mockResponses.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2815 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9250 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/tsconfig.base.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      304 2023-08-01 18:13:40.000000 amazon_sagemaker_jupyter_scheduler-2.2.0/tsconfig.json
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/.eslintrc.js` & `amazon_sagemaker_jupyter_scheduler-2.2.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/.gitignore` & `amazon_sagemaker_jupyter_scheduler-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/Config` & `amazon_sagemaker_jupyter_scheduler-2.2.0/Config`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/DEVELOPMENT.md` & `amazon_sagemaker_jupyter_scheduler-2.2.0/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/MANIFEST.in` & `amazon_sagemaker_jupyter_scheduler-2.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/PKG-INFO` & `amazon_sagemaker_jupyter_scheduler-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_sagemaker_jupyter_scheduler
-Version: 2.1.0
+Version: 2.2.0
 Summary: Amazon SageMaker Jupyter Scheduler based on the https://pypi.org/project/jupyter-scheduler/
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,Scheduling Notebooks,Notebooks,Amazon Sagemaker
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/RELEASE.md` & `amazon_sagemaker_jupyter_scheduler-2.2.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/__init__.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/app_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/app_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/service-2.json` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/service-2.json`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/clients.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/clients.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/cron_util.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/cron_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/deletable_resource.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/deletable_resource.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/environment_detector.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/environment_detector.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/environments.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/error_util.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/error_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/extension.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/extension.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from amazon_sagemaker_jupyter_scheduler.logging import init_api_operation_logger
 from jupyter_server.extension.application import ExtensionApp
 from amazon_sagemaker_jupyter_scheduler.handlers import (
     AdvancedEnvironmentsHandler,
     SageMakerImagesListHandler,
-    ValidateVolumePathHandler,
-    FeatureAccessControlHandler
+    ValidateVolumePathHandler
 )
 
 class SageMakerSchedulingApp(ExtensionApp):
     name = "amazon_sagemaker_jupyter_scheduler"
     handlers = [
         (r"/advanced_environments", AdvancedEnvironmentsHandler),
         (r"/sagemaker_images", SageMakerImagesListHandler),
-        (r"/validate_volume_path", ValidateVolumePathHandler),
-        (r"/sagemaker_feature_enabled", FeatureAccessControlHandler),
+        (r"/validate_volume_path", ValidateVolumePathHandler)
     ]
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         init_api_operation_logger(self.log)
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/file_uploader.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/file_uploader.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/package.json` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9659722222222222%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.3b333e0e590d8edb68a6.js'}}",*

 * * "'version'": "'2.2.0'"}*

```diff
@@ -61,15 +61,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.299f9d522c52a504280b.js"
+            "load": "static/remoteEntry.3b333e0e590d8edb68a6.js"
         },
         "disabledExtensions": [
             "@jupyterlab/scheduler:IAdvancedOptions"
         ],
         "extension": true,
         "outputDir": "amazon_sagemaker_jupyter_scheduler/labextension",
         "schemaDir": "schema",
@@ -110,9 +110,9 @@
         "test": "jest",
         "test:debug": "node --inspect node_modules/.bin/jest --watch --runInBand",
         "test:server-extension": ":",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "2.1.0"
+    "version": "2.2.0"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'2.2.0'"}*

```diff
@@ -106,9 +106,9 @@
         "test": "jest",
         "test:debug": "node --inspect node_modules/.bin/jest --watch --runInBand",
         "test:server-extension": ":",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "2.1.0"
+    "version": "2.2.0"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/144.9be27e93647ef0e84863.js` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/144.9be27e93647ef0e84863.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/993.84c00bb76b4448d8ce3f.js` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/315.59fba34ec08e26375d68.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,19 @@
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyter_scheduler = self.webpackChunk_amzn_sagemaker_jupyter_scheduler || []).push([
-    [993], {
-        7993: (e, t, r) => {
+    [315], {
+        8315: (e, t, r) => {
             r.r(t), r.d(t, {
-                default: () => Rt
+                default: () => Ft
             });
             var n = r(6271),
                 o = r.n(n),
                 a = r(7363),
                 l = r(5015);
-            const i = "nbScheduler",
-                s = {
+            const i = {
                     ScheduleNoteBook: {
                         MainPanel: {
                             AdvancedOptions: {
                                 options: "Advanced Options",
                                 environmentVariables: "Environment variables",
                                 addEnvironmentvariable: "Add Variable",
                                 Key: "Key",
@@ -140,47 +139,47 @@
                             buttons: {
                                 goToIamConsole: "Go to IAM console",
                                 enterKeysInTerminal: "Run `aws configure` in Terminal"
                             }
                         }
                     }
                 },
-                u = {
+                s = {
                     expiredToken: "ExpiredToken",
                     invalidClientTokenId: "InvalidClientTokenId",
                     noCredentials: "NoCredentials"
                 },
-                c = "terminal:create-new";
-            var m, d = r(5185),
-                p = r(5306),
-                v = r(1396),
-                g = r(6247);
+                u = "terminal:create-new";
+            var c, m = r(5185),
+                d = r(5306),
+                p = r(1396),
+                v = r(6247);
             ! function(e) {
                 e.PublicInternetOnly = "PublicInternetOnly", e.VpcOnly = "VpcOnly"
-            }(m || (m = {}));
-            var b, h, f = r(9208),
-                E = r(1982),
-                y = r(9692);
+            }(c || (c = {}));
+            var g, b, h = r(9208),
+                f = r(1982),
+                E = r(9692);
             ! function(e) {
                 e[e.Large = 0] = "Large", e[e.Medium = 1] = "Medium", e[e.Small = 2] = "Small"
-            }(b || (b = {})),
+            }(g || (g = {})),
             function(e) {
                 e.Filled = "filled"
-            }(h || (h = {}));
-            const S = {
-                    [b.Large]: "var(--jp-content-line-height-3)",
-                    [b.Medium]: "var(--jp-content-line-height-2)",
-                    [b.Small]: "var(--jp-content-line-height-1-25)"
+            }(b || (b = {}));
+            const y = {
+                    [g.Large]: "var(--jp-content-line-height-3)",
+                    [g.Medium]: "var(--jp-content-line-height-2)",
+                    [g.Small]: "var(--jp-content-line-height-1-25)"
                 },
-                _ = {
-                    [b.Large]: "1em",
-                    [b.Medium]: "0.5em",
-                    [b.Small]: "0.25em"
+                S = {
+                    [g.Large]: "1em",
+                    [g.Medium]: "0.5em",
+                    [g.Small]: "0.25em"
                 },
-                k = (0, y.Z)((() => ({
+                _ = (0, E.Z)((() => ({
                     root: {
                         background: "var(--jp-input-active-background)",
                         borderTopLeftRadius: "var(--jp-border-radius)",
                         borderTopRightRadius: "var(--jp-border-radius)",
                         fontSize: "var(--jp-ui-font-size2)",
                         "&.Mui-focused": {
                             background: "var(--jp-input-active-background)"
@@ -209,93 +208,93 @@
                         },
                         "&.Mui-error:after": {
                             borderBottom: "var(--jp-border-width) solid"
                         }
                     },
                     input: {
                         color: "var(--jp-ui-font-color0)",
-                        lineHeight: e => S[e.size],
-                        padding: e => `${_[e.size]}`
+                        lineHeight: e => y[e.size],
+                        padding: e => `${S[e.size]}`
                     }
                 }))),
-                x = ((0, y.Z)((() => ({
+                k = ((0, E.Z)((() => ({
                     root: {
                         fontFamily: "var(--jp-cell-prompt-font-family)",
                         color: "var(--jp-input-border-color)",
                         marginBottom: "var(--padding-small)",
                         "&.Mui-error": {
                             fontFamily: "var(--jp-cell-prompt-font-family)",
                             color: "var(--jp-error-color1)"
                         },
                         "&.Mui-disabled": {
                             fontFamily: "var(--jp-cell-prompt-font-family)",
                             color: "var(--jp-error-color1)"
                         }
                     }
-                }))), (0, y.Z)((() => ({
+                }))), (0, E.Z)((() => ({
                     root: {
                         fontSize: "var(--jp-ui-font-size0)",
                         color: "var(--text-input-helper-text)",
                         "&.Mui-error": {
                             color: "var(--jp-error-color1)"
                         },
                         "&.Mui-disabled": {
                             color: "var(--jp-error-color1)"
                         }
                     }
                 })))),
-                w = ({
+                x = ({
                     classes: e,
                     className: t,
                     InputProps: r,
                     FormHelperTextProps: n,
-                    size: a = b.Medium,
+                    size: a = g.Medium,
                     variant: l,
                     ...i
                 }) => {
                     var s, u, c;
-                    const m = (0, E.cx)(E.css`
+                    const m = (0, f.cx)(f.css`
   .MuiFormHelperText-root.Mui-error::before {
     display: inline-block;
     vertical-align: middle;
     background-size: 1rem 1rem;
     height: var(--text-input-error-icon-height);
     width: var(--text-input-error-icon-width);
     background-image: var(--text-input-helper-text-alert-icon);
     background-repeat: no-repeat;
     content: ' ';
   }
 `, t, null == e ? void 0 : e.root);
-                    return o().createElement(p.TextField, {
+                    return o().createElement(d.TextField, {
                         classes: {
                             root: m,
                             ...e
                         },
                         variant: l,
                         InputProps: {
                             ...r,
                             classes: {
-                                root: (0, E.cx)(k({
+                                root: (0, f.cx)(_({
                                     size: a
                                 }).root, null === (s = null == r ? void 0 : r.classes) || void 0 === s ? void 0 : s.root),
-                                input: (0, E.cx)(k({
+                                input: (0, f.cx)(_({
                                     size: a
                                 }).input, null === (u = null == r ? void 0 : r.classes) || void 0 === u ? void 0 : u.input)
                             }
                         },
                         FormHelperTextProps: {
                             ...n,
                             classes: {
-                                root: (0, E.cx)(x().root, null === (c = null == n ? void 0 : n.classes) || void 0 === c ? void 0 : c.root)
+                                root: (0, f.cx)(k().root, null === (c = null == n ? void 0 : n.classes) || void 0 === c ? void 0 : c.root)
                             }
                         },
                         ...i
                     })
                 },
-                M = (0, y.Z)((() => ({
+                w = (0, E.Z)((() => ({
                     popper: {
                         "& .MuiTooltip-tooltip": {
                             backgroundColor: "var(--color-light)",
                             boxShadow: "var(--tooltip-shadow)",
                             color: "var(--tooltip-text-color",
                             padding: "var(--padding-16)",
                             fontSize: "var(--font-size-0)"
@@ -306,138 +305,138 @@
                             color: "var(--tooltip-surface)",
                             "&:before": {
                                 boxShadow: "var(--tooltip-shadow)"
                             }
                         }
                     }
                 })));
-            var P, T = r(30);
+            var M, P = r(30);
             ! function(e) {
                 e.TopStart = "top-start", e.Top = "top", e.TopEnd = "top-end", e.RightStart = "right-start", e.Right = "right", e.RightEnd = "right-end", e.BottomStart = "bottom-start", e.Bottom = "bottom", e.BottomEnd = "bottom-end", e.LeftStart = "left-start", e.Left = "left", e.LeftEnd = "left-end"
-            }(P || (P = {}));
-            const j = ({
+            }(M || (M = {}));
+            const T = ({
                     children: e,
                     classes: t,
                     className: r,
-                    placement: n = P.Right,
+                    placement: n = M.Right,
                     ...a
                 }) => {
-                    const l = (0, E.cx)(r, M().popper, null == t ? void 0 : t.popper);
-                    return o().createElement(T.ZP, {
+                    const l = (0, f.cx)(r, w().popper, null == t ? void 0 : t.popper);
+                    return o().createElement(P.ZP, {
                         ...a,
                         arrow: !0,
                         classes: {
                             popper: l,
-                            tooltip: M().tooltip
+                            tooltip: w().tooltip
                         },
                         placement: n
                     }, e)
                 },
-                C = E.css`
+                j = f.css`
   display: flex;
   flex-direction: column;
 `,
-                I = E.css`
+                I = f.css`
   display: flex;
   flex-direction: column;
 `,
-                N = E.css`
+                C = f.css`
   display: inline-flex;
   svg {
     width: 0.75em;
     height: 0.75em;
     transform: translateY(-2px);
   }
 `,
-                O = E.css`
+                N = f.css`
   svg {
     width: 0.75em;
     height: 0.75em;
     transform: translateY(1px);
   }
 `,
-                V = (e = !1) => E.css`
+                O = (e = !1) => f.css`
   display: flex;
   flex-direction: column;
   ${e?"":"max-width : 500px;"}
   .MuiCheckbox-colorPrimary.Mui-checked {
     color: var(--jp-brand-color1);
   }
   .MuiButton-containedPrimary:hover {
     background-color: var(--jp-brand-color1);
   }
 `,
-                A = E.css`
+                V = f.css`
   font-size: var(--jp-content-font-size1);
 `,
-                F = E.css`
+                A = f.css`
   display: flex;
   justify-content: flex-start;
   align-items: center;
   gap: 0.5rem;
   svg {
     width: var(--jp-ui-font-size1);
     height: var(--jp-ui-font-size1);
     path {
       fill: var(--jp-error-color1);
     }
   }
 `,
-                R = (e = !1) => E.css`
+                F = (e = !1) => f.css`
   color: var(--jp-color-root-light-800);
   font-weight: 400;
   font-size: var(--jp-ui-font-size1);
   line-height: var(--jp-ui-font-size1);
   margin-bottom: var(--jp-ui-font-size1);
   ${e&&"\n    &:after {\n      content: '*';\n      color: var(--jp-error-color1);\n    }\n  "}
 `;
-            var z, K, D = r(6689);
+            var R, z, K = r(6689);
             ! function(e) {
                 e.External = "_blank", e.Content = "_self"
-            }(z || (z = {})),
+            }(R || (R = {})),
             function(e) {
                 e.None = "none", e.Hover = "hover", e.Always = "always"
-            }(K || (K = {}));
-            const L = ({
+            }(z || (z = {}));
+            const D = ({
                 className: e,
                 disabled: t = !1,
                 children: r,
                 onClick: n,
-                target: a = z.Content,
+                target: a = R.Content,
                 ...l
             }) => {
-                const i = a === z.External,
+                const i = a === R.External,
                     s = {
                         ...l,
-                        className: (0, E.cx)(E.css`
+                        className: (0, f.cx)(f.css`
   cursor: pointer;
   text-decoration: none;
   color: var(--jp-brand-color1);
 
   &:hover {
     text-decoration: none;
     color: var(--jp-brand-color1);
   }
 `, e),
                         target: a,
                         onClick: t ? void 0 : n,
                         rel: i ? "noopener noreferrer" : void 0
                     };
-                return o().createElement(D.Z, {
+                return o().createElement(K.Z, {
                     ...s
                 }, r)
             };
             r(78);
-            const J = e => "string" == typeof e && e.length > 0;
-            var B = r(5505),
-                G = r.n(B);
+            const L = e => "string" == typeof e && e.length > 0;
+            var J = r(5505),
+                B = r.n(J);
 
-            function $(e) {
+            function G(e) {
                 try {
-                    if (!G()(e) || 0 === e.length) return {
+                    if (!B()(e) || 0 === e.length) return {
                         kernel: null,
                         arnEnvironment: null,
                         version: null
                     };
                     const t = e.split("__SAGEMAKER_INTERNAL__"),
                         [r, n] = t,
                         o = n && n.split("/"),
@@ -452,260 +451,260 @@
                     return {
                         kernel: null,
                         arnEnvironment: null,
                         version: null
                     }
                 }
             }
-            const q = ({
+            const $ = ({
                 labelInfo: e,
                 required: t,
                 toolTipText: r,
                 errorMessage: n,
                 ...a
             }) => o().createElement("div", {
                 className: I
             }, o().createElement("div", {
-                className: N
+                className: C
             }, o().createElement("label", {
-                className: R(t)
-            }, " ", e, " "), r && !a.readOnly && o().createElement(j, {
+                className: F(t)
+            }, " ", e, " "), r && !a.readOnly && o().createElement(T, {
                 title: r,
-                className: O
-            }, o().createElement(f.Z, null))), o().createElement(w, {
+                className: N
+            }, o().createElement(h.Z, null))), o().createElement(x, {
                 ...a,
-                error: J(n),
+                error: L(n),
                 helperText: n,
                 InputProps: {
                     readOnly: a.readOnly,
                     ...a.InputProps
                 }
             }));
             var Z = r(6433);
-            E.css`
+            f.css`
   box-sizing: border-box;
   width: 100%;
   padding: var(--jp-padding-large);
   flex-direction: column;
   display: flex;
   color: var(--jp-ui-font-color0);
-`, E.css`
+`, f.css`
   width: 100%;
   display: flex;
   flex-flow: row nowrap;
   justify-content: space-between;
   padding-bottom: var(--jp-padding-20);
   color: var(--jp-ui-font-color0);
-`, E.css`
+`, f.css`
   max-width: 525px;
   color: var(--jp-ui-font-color2);
   margin-bottom: var(--jp-padding-medium);
-`, E.css`
+`, f.css`
   display: block;
   margin-bottom: 0.5em;
   overflow-y: scroll;
-`, E.css`
+`, f.css`
   align-items: center;
   display: inline-flex;
   margin-bottom: var(--jp-padding-16);
   margin-left: 1em;
   font-size: var(--jp-ui-font-size3);
   color: var(--jp-ui-font-color0);
 `;
-            const H = E.css`
+            const q = f.css`
   display: flex;
   flex-direction: column;
   font-size: 12px;
   color: var(--jp-ui-font-color0);
   padding: 10px;
   overflow-x: auto;
   overflow-y: hidden;
   gap: 20px;
 `,
-                U = (E.css`
+                H = (f.css`
   display: flex;
   justify-content: space-between;
-`, E.css`
+`, f.css`
   display: flex;
   align-items: center;
-`, E.css`
+`, f.css`
   margin-bottom: var(--jp-padding-medium);
-`, E.css`
+`, f.css`
   width: 50% !important;
   text-align: center;
   height: 30px;
   font-size: 12px !important;
-`, E.css`
+`, f.css`
   display: inline-flex;
   justify-content: right;
-`, E.css`
+`, f.css`
   height: fit-content;
   width: 90px;
   text-align: center;
   margin-right: var(--jp-padding-medium);
-`, E.css`
+`, f.css`
   position: absolute;
   right: 0%;
   bottom: 0%;
   margin-bottom: var(--jp-padding-large);
-`, E.css`
+`, f.css`
   div:nth-child(2) {
     width: 98%;
   }
-`, E.css`
+`, f.css`
   div:nth-child(2) {
     width: 49%;
   }
-`, E.css`
+`, f.css`
   div:nth-child(2) {
     width: 150px;
   }
-`, E.css`
+`, f.css`
   width: 500px;
   margin-bottom: var(--jp-size-4);
 `),
-                Y = E.css`
+                U = f.css`
   display: flex;
   align-items: center;
 `,
-                W = E.css`
+                Y = f.css`
   display: flex;
   align-items: center;
 `,
-                Q = E.css`
+                W = f.css`
   color: var(--jp-brand-color3);
 `,
-                X = E.css`
+                Q = f.css`
   padding: 4px;
 `,
-                ee = E.css`
+                X = f.css`
   color: var(--jp-ui-font-color0);
 `,
-                te = E.css`
+                ee = f.css`
   display: flex;
   flex-direction: column;
   gap: var(--jp-ui-font-size1);
 `,
-                re = E.css`
+                te = f.css`
   color: var(--jp-error-color1);
   padding: 12px;
 `,
-                ne = s.ScheduleNoteBook.MainPanel.ErrorMessages.VPCErrors,
-                oe = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
-                ae = s.ScheduleNoteBook.MainPanel.Tooltips,
-                le = o().createElement("div", null, o().createElement("span", {
-                    className: W
-                }, " ", ae.VPCTooltip, " "), o().createElement(L, {
+                re = i.ScheduleNoteBook.MainPanel.ErrorMessages.VPCErrors,
+                ne = i.ScheduleNoteBook.MainPanel.AdvancedOptions,
+                oe = i.ScheduleNoteBook.MainPanel.Tooltips,
+                ae = o().createElement("div", null, o().createElement("span", {
+                    className: Y
+                }, " ", oe.VPCTooltip, " "), o().createElement(D, {
                     href: "https://docs.aws.amazon.com/sagemaker/latest/dg/create-notebook-auto-execution-advanced.html",
-                    target: z.External
+                    target: R.External
                 }, o().createElement("p", {
-                    className: Q
-                }, s.ScheduleNoteBook.MainPanel.Tooltips.LearnMore))),
-                ie = ({
+                    className: W
+                }, i.ScheduleNoteBook.MainPanel.Tooltips.LearnMore))),
+                le = ({
                     isChecked: e,
                     formState: t,
                     formErrors: r,
                     initialSecurityGroups: n,
                     initialSubnets: a,
                     availableSubnets: l,
                     setFormErrors: i,
                     setChecked: s,
                     setFormState: u,
                     ...c
                 }) => o().createElement("div", {
-                    className: Y
+                    className: U
                 }, o().createElement(Z.Z, {
                     name: "vpc-check-box",
-                    className: X,
+                    className: Q,
                     color: "primary",
                     checked: e,
                     onChange: e => {
                         const o = e.target.checked;
                         if (s(o), o) {
                             if (u({
                                     ...t,
                                     vpc_security_group_ids: n,
                                     vpc_subnets: a
                                 }), 0 === a.length && l.length > 0) return void i({
                                 ...r,
-                                subnetError: `${ne.RequiresPrivateSubnet} ${ne.NoPrivateSubnetsInSageMakerDomain}. ${ne.YouMayChooseOtherSubnets}`
+                                subnetError: `${re.RequiresPrivateSubnet} ${re.NoPrivateSubnetsInSageMakerDomain}. ${re.YouMayChooseOtherSubnets}`
                             });
                             0 === l.length && i({
                                 ...r,
-                                subnetError: `${ne.RequiresPrivateSubnet} ${ne.NoPrivateSubnetsInSageMakerDomain}`
+                                subnetError: `${re.RequiresPrivateSubnet} ${re.NoPrivateSubnetsInSageMakerDomain}`
                             })
                         } else u({
                             ...t,
                             vpc_security_group_ids: [],
                             vpc_subnets: []
                         }), i({
                             ...r,
                             subnetError: "",
                             securityGroupError: ""
                         })
                     },
                     ...c
-                }), o().createElement("label", null, oe.useVPC), o().createElement(j, {
+                }), o().createElement("label", null, ne.useVPC), o().createElement(T, {
                     classes: {
-                        popperInteractive: ee
+                        popperInteractive: X
                     },
-                    title: le,
+                    title: ae,
                     interactive: !0
-                }, o().createElement(f.Z, {
+                }, o().createElement(h.Z, {
                     fontSize: "small"
                 })));
-            var se = r(9419),
-                ue = r(2679),
-                ce = r(4085);
-            const me = E.css`
+            var ie = r(9419),
+                se = r(2679),
+                ue = r(4085);
+            const ce = f.css`
   display: flex;
   align-items: flex-end;
   padding-right: 1em;
   gap: 20px;
 `,
-                de = E.css`
+                me = f.css`
   display: flex;
   flex-direction: column;
 `,
-                pe = E.css`
+                de = f.css`
   width: 170px;
 `,
-                ve = (E.css`
+                pe = (f.css`
   display: flex;
   flex-direction: column;
   margin-bottom: var(--jp-padding-large);
-`, E.css`
+`, f.css`
   display: flex;
   flex-direction: column;
   gap: 16px;
 `),
-                ge = E.css`
+                ve = f.css`
   font-weight: 400;
   font-size: var(--jp-ui-font-size1);
   line-height: var(--jp-ui-font-size1);
 `,
-                be = E.css`
+                ge = f.css`
   background-color: var(--jp-brand-color1);
   font-size: var(--jp-ui-font-size1);
   text-transform: none;
 `,
-                he = E.css`
+                be = f.css`
   display: inline-flex;
   align-items: center;
   gap: 6px;
   svg {
     width: 0.75em;
     height: 0.75em;
   }
 `,
-                fe = new RegExp("[a-zA-Z_][a-zA-Z0-9_]*"),
-                Ee = new RegExp("[\\S\\s]*"),
-                ye = s.ScheduleNoteBook.MainPanel.ErrorMessages.AdvancedOptions,
-                Se = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
-                _e = ({
+                he = new RegExp("[a-zA-Z_][a-zA-Z0-9_]*"),
+                fe = new RegExp("[\\S\\s]*"),
+                Ee = i.ScheduleNoteBook.MainPanel.ErrorMessages.AdvancedOptions,
+                ye = i.ScheduleNoteBook.MainPanel.AdvancedOptions,
+                Se = ({
                     isDisabled: e,
                     environmentParameters: t,
                     setEnvironmentParameters: r,
                     index: n,
                     formErrors: a,
                     setFormErrors: l
                 }) => {
@@ -727,163 +726,163 @@
                         u = () => {
                             const {
                                 key: e,
                                 value: t
                             } = i;
                             e.length < 1 || t.length < 1 ? l({
                                 ...a,
-                                environmentVariablesError: ye.EnvironmentVariableEmptyError
+                                environmentVariablesError: Ee.EnvironmentVariableEmptyError
                             }) : e.length > 512 || t.length > 512 ? l({
                                 ...a,
-                                environmentVariablesError: ye.EnvironmentVariableLengthError
-                            }) : fe.test(e) && Ee.test(t) ? l({
+                                environmentVariablesError: Ee.EnvironmentVariableLengthError
+                            }) : he.test(e) && fe.test(t) ? l({
                                 ...a,
                                 environmentVariablesError: ""
                             }) : l({
                                 ...a,
-                                environmentVariablesError: ye.EnvironmentVariableFormatError
+                                environmentVariablesError: Ee.EnvironmentVariableFormatError
                             })
                         };
                     return o().createElement("div", {
-                        className: me
-                    }, o().createElement(q, {
-                        className: pe,
+                        className: ce
+                    }, o().createElement($, {
+                        className: de,
                         readOnly: e,
                         name: `envKey-${n}`,
-                        labelInfo: Se.Key,
+                        labelInfo: ye.Key,
                         value: t[n].key,
                         onChange: s,
                         onBlur: u
-                    }), o().createElement(q, {
-                        className: pe,
+                    }), o().createElement($, {
+                        className: de,
                         readOnly: e,
                         name: `envValue-${n}`,
-                        labelInfo: Se.Value,
+                        labelInfo: ye.Value,
                         value: t[n].value,
                         onChange: s,
                         onBlur: u
-                    }), o().createElement("div", null, !e && o().createElement(ce.Z, {
+                    }), o().createElement("div", null, !e && o().createElement(ue.Z, {
                         onClick: () => {
                             (e => {
                                 const n = [...t];
                                 n.splice(e, 1), r(n), l({
                                     ...a,
                                     environmentVariablesError: ""
                                 })
                             })(n), l({
                                 ...a,
                                 environmentVariablesError: ""
                             })
                         }
-                    }, o().createElement(ue.Z, null))))
+                    }, o().createElement(se.Z, null))))
                 },
-                ke = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
-                xe = s.ScheduleNoteBook.MainPanel.Tooltips,
-                we = ({
+                _e = i.ScheduleNoteBook.MainPanel.AdvancedOptions,
+                ke = i.ScheduleNoteBook.MainPanel.Tooltips,
+                xe = ({
                     allFieldsDisabled: e,
                     isButtonDisabled: t,
                     environmentVariables: r,
                     setEnvironmentVariables: n,
                     formErrors: a,
                     ...l
                 }) => {
                     const i = !!a.environmentVariablesError,
                         s = o().createElement("div", {
-                            className: F
-                        }, o().createElement(se.Z, {
+                            className: A
+                        }, o().createElement(ie.Z, {
                             severity: "error"
                         }, a.environmentVariablesError));
                     return o().createElement("div", {
-                        className: ve
+                        className: pe
                     }, o().createElement("div", {
-                        className: he
+                        className: be
                     }, o().createElement("label", {
-                        className: ge
-                    }, ke.environmentVariables), e ? null : o().createElement(j, {
-                        title: xe.EnvironmentVariablesTooltip
-                    }, o().createElement(f.Z, null))), e && 0 === r.length ? o().createElement("div", {
-                        className: de
-                    }, o().createElement(w, {
+                        className: ve
+                    }, _e.environmentVariables), e ? null : o().createElement(T, {
+                        title: ke.EnvironmentVariablesTooltip
+                    }, o().createElement(h.Z, null))), e && 0 === r.length ? o().createElement("div", {
+                        className: me
+                    }, o().createElement(x, {
                         InputProps: {
                             readOnly: !0
                         },
-                        placeholder: ke.Placeholders.NoneSelected
-                    })) : o().createElement(o().Fragment, null, r.map(((t, i) => o().createElement(_e, {
+                        placeholder: _e.Placeholders.NoneSelected
+                    })) : o().createElement(o().Fragment, null, r.map(((t, i) => o().createElement(Se, {
                         isDisabled: e,
                         key: i,
                         environmentParameters: r,
                         setEnvironmentParameters: n,
                         index: i,
                         formErrors: a,
                         ...l
-                    })))), i && o().createElement("div", null, s), !e && o().createElement("div", null, o().createElement(p.Button, {
+                    })))), i && o().createElement("div", null, s), !e && o().createElement("div", null, o().createElement(d.Button, {
                         disabled: t,
-                        className: be,
+                        className: ge,
                         variant: "contained",
                         color: "primary",
                         size: "small",
                         onClick: () => {
                             n([...r, {
                                 key: "",
                                 value: ""
                             }])
                         }
-                    }, ke.addEnvironmentvariable)))
+                    }, _e.addEnvironmentvariable)))
                 };
-            var Me = r(1518),
-                Pe = r(5861),
-                Te = r(3640);
-            const je = (0, Me.D)(),
-                Ce = ({
+            var we = r(1518),
+                Me = r(5861),
+                Pe = r(3640);
+            const Te = (0, we.D)(),
+                je = ({
                     label: e,
                     required: t,
                     errorMessage: r,
                     disabled: n,
                     renderInput: a,
                     tooltip: l,
                     disabledTooltip: i,
                     freeSolo: s,
                     options: u,
                     ...c
                 }) => {
                     var m, d;
-                    null != a || (a = t => o().createElement(Te.Z, {
+                    null != a || (a = t => o().createElement(Pe.Z, {
                         ...t,
                         variant: "outlined",
                         size: "small",
                         margin: "dense",
                         placeholder: e
                     }));
-                    const p = n ? i ? o().createElement(j, {
+                    const p = n ? i ? o().createElement(T, {
                             title: i,
-                            className: O
-                        }, o().createElement(f.Z, null)) : o().createElement(o().Fragment, null) : l ? o().createElement(j, {
+                            className: N
+                        }, o().createElement(h.Z, null)) : o().createElement(o().Fragment, null) : l ? o().createElement(T, {
                             title: l,
-                            className: O
-                        }, o().createElement(f.Z, null)) : o().createElement(o().Fragment, null),
+                            className: N
+                        }, o().createElement(h.Z, null)) : o().createElement(o().Fragment, null),
                         v = r ? o().createElement("div", {
-                            className: F
-                        }, o().createElement(se.Z, {
+                            className: A
+                        }, o().createElement(ie.Z, {
                             severity: "error"
                         }, r)) : o().createElement(o().Fragment, null);
                     return o().createElement("div", {
-                        className: C
+                        className: j
                     }, o().createElement("div", {
-                        className: N
+                        className: C
                     }, o().createElement("label", {
-                        className: R(t)
-                    }, e), p), o().createElement(Pe.Z, {
+                        className: F(t)
+                    }, e), p), o().createElement(Me.Z, {
                         ...c,
                         multiple: !0,
                         renderInput: a,
                         freeSolo: s,
                         readOnly: n,
                         options: u,
                         filterOptions: (e, t) => {
-                            const r = je(e, t);
+                            const r = Te(e, t);
                             return "" === t.inputValue || e.includes(t.inputValue) || r.push(t.inputValue), r
                         },
                         renderOption: (e, t, r) => (u.includes(t) || (t = `Add "${t}"`), o().createElement("li", {
                             ...e
                         }, t)),
                         componentsProps: {
                             ...c.componentsProps,
@@ -895,457 +894,457 @@
                                 ...null === (d = c.componentsProps) || void 0 === d ? void 0 : d.clearIndicator,
                                 size: "small"
                             }
                         }
                     }), v)
                 },
                 Ie = new RegExp("^(https|s3)://([^/]+)/?(.*)$"),
-                Ne = new RegExp("[-0-9a-zA-Z]+"),
-                Oe = new RegExp("^arn:aws[a-z\\-]*:iam::\\d{12}:role/?[a-zA-Z_0-9+=,.@\\-_/]+$"),
-                Ve = new RegExp("^arn:aws:kms:\\w+(?:-\\w+)+:\\d{12}:key\\/[A-Za-z0-9]+(?:-[A-Za-z0-9]+)+$"),
-                Ae = new RegExp("^[0-9a-z]{8}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12}$"),
-                Fe = s.ScheduleNoteBook.MainPanel.ErrorMessages,
-                Re = Fe.VPCErrors,
-                ze = e => e.length < 20 || e.length > 2048 ? Fe.AdvancedOptions.RoleArnLengthError : Oe.test(e) ? "" : Fe.AdvancedOptions.RoleArnFormatError,
-                Ke = e => 0 === e.trim().length ? Fe.AdvancedOptions.S3LengthError : Ie.test(e) ? "" : Fe.AdvancedOptions.S3FormatError,
-                De = e => 0 === e.length || Ve.test(e) || Ae.test(e) ? "" : Fe.AdvancedOptions.KMSKeyError;
-            var Le;
+                Ce = new RegExp("[-0-9a-zA-Z]+"),
+                Ne = new RegExp("^arn:aws[a-z\\-]*:iam::\\d{12}:role/?[a-zA-Z_0-9+=,.@\\-_/]+$"),
+                Oe = new RegExp("^arn:aws:kms:\\w+(?:-\\w+)+:\\d{12}:key\\/[A-Za-z0-9]+(?:-[A-Za-z0-9]+)+$"),
+                Ve = new RegExp("^[0-9a-z]{8}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12}$"),
+                Ae = i.ScheduleNoteBook.MainPanel.ErrorMessages,
+                Fe = Ae.VPCErrors,
+                Re = e => e.length < 20 || e.length > 2048 ? Ae.AdvancedOptions.RoleArnLengthError : Ne.test(e) ? "" : Ae.AdvancedOptions.RoleArnFormatError,
+                ze = e => 0 === e.trim().length ? Ae.AdvancedOptions.S3LengthError : Ie.test(e) ? "" : Ae.AdvancedOptions.S3FormatError,
+                Ke = e => 0 === e.length || Oe.test(e) || Ve.test(e) ? "" : Ae.AdvancedOptions.KMSKeyError;
+            var De;
             ! function(e) {
                 e.LocalJL = "local-jupyter-lab", e.Studio = "studio"
-            }(Le || (Le = {}));
-            class Je {
+            }(De || (De = {}));
+            class Le {
                 get isStudio() {
-                    return this.type === Le.Studio
+                    return this.type === De.Studio
                 }
                 get isLocalJL() {
-                    return this.type === Le.LocalJL
+                    return this.type === De.LocalJL
                 }
                 constructor(e) {
                     this.type = e
                 }
             }
-            const Be = (0, n.createContext)(void 0);
+            const Je = (0, n.createContext)(void 0);
 
-            function Ge({
+            function Be({
                 app: e,
                 children: t
             }) {
                 const [r, a] = (0, n.useState)((() => function(e) {
-                    return e.hasPlugin("@amzn/sagemaker-ui:project") ? new Je(Le.Studio) : new Je(Le.LocalJL)
+                    return e.hasPlugin("@amzn/sagemaker-ui:project") ? new Le(De.Studio) : new Le(De.LocalJL)
                 }(e))), l = {
                     pluginEnvironment: r,
                     setPluginEnvironment: a
                 };
-                return o().createElement(Be.Provider, {
+                return o().createElement(Je.Provider, {
                     value: l
                 }, t)
             }
 
-            function $e() {
-                const e = (0, n.useContext)(Be);
+            function Ge() {
+                const e = (0, n.useContext)(Je);
                 if (void 0 === e) throw new Error("usePluginEnvironment must be used within a PluginEnvironmentProvider");
                 return e
             }
-            var qe = r(8202),
+            var $e = r(8202),
                 Ze = r(3274),
-                He = r(8102);
-            const Ue = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
-                Ye = s.ScheduleNoteBook.MainPanel.Tooltips,
-                We = s.ScheduleNoteBook.MainPanel.StudioTooltips,
-                Qe = s.ScheduleNoteBook.MainPanel.ErrorMessages,
-                Xe = o().createElement("div", null, o().createElement("span", {
-                    className: W
-                }, Ye.kmsKeyTooltip), o().createElement(L, {
+                qe = r(8102);
+            const He = i.ScheduleNoteBook.MainPanel.AdvancedOptions,
+                Ue = i.ScheduleNoteBook.MainPanel.Tooltips,
+                Ye = i.ScheduleNoteBook.MainPanel.StudioTooltips,
+                We = i.ScheduleNoteBook.MainPanel.ErrorMessages,
+                Qe = o().createElement("div", null, o().createElement("span", {
+                    className: Y
+                }, Ue.kmsKeyTooltip), o().createElement(D, {
                     href: "https://docs.aws.amazon.com/sagemaker/latest/dg/create-notebook-auto-execution-advanced.html",
-                    target: z.External
+                    target: R.External
                 }, o().createElement("p", {
-                    className: Q
-                }, Ye.LearnMore))),
-                et = o().createElement("div", null, o().createElement("span", {
                     className: W
-                }, Ye.LCCScriptTooltipText), o().createElement(L, {
+                }, Ue.LearnMore))),
+                Xe = o().createElement("div", null, o().createElement("span", {
+                    className: Y
+                }, Ue.LCCScriptTooltipText), o().createElement(D, {
                     href: "https://aws.amazon.com/blogs/machine-learning/customize-amazon-sagemaker-studio-using-lifecycle-configurations/",
-                    target: z.External
+                    target: R.External
                 }, o().createElement("p", {
-                    className: Q
-                }, Ye.LearnMore))),
-                tt = ({
+                    className: W
+                }, Ue.LearnMore))),
+                et = ({
                     isDisabled: e,
                     formState: t,
                     formErrors: r,
                     environmentVariables: a,
                     setEnvironmentVariables: l,
                     lccOptions: i,
                     availableSecurityGroups: s,
                     availableSubnets: u,
                     initialSubnets: c,
                     initialSecurityGroups: m,
-                    isVPCDomain: d,
+                    isVPCDomain: g,
                     requestClient: b,
-                    enableVPCSetting: h,
+                    enableVPCSetting: f,
                     userDefaultValues: E,
                     setFormState: y,
                     handleChange: S,
                     handleNumberValueChange: _,
                     setSubnets: k,
                     setSecurityGroups: x,
                     onSelectLCCScript: w,
                     setFormValidationErrors: M,
                     setEnableVPCSetting: P,
-                    setRoleArn: T
+                    setRoleArn: j
                 }) => {
                     const {
-                        pluginEnvironment: C
-                    } = $e(), [I, N] = (0, n.useState)(!1), [O, V] = (0, n.useState)(!1), A = e => {
+                        pluginEnvironment: I
+                    } = Ge(), [C, N] = (0, n.useState)(!1), [O, V] = (0, n.useState)(!1), A = e => {
                         const t = e.target.name,
-                            n = Ke(e.target.value);
+                            n = ze(e.target.value);
                         M({
                             ...r,
                             ["s3_input" === t ? "s3InputFolderError" : "s3OutputFolderError"]: n
                         })
                     }, F = e => {
                         const t = e.target.name,
-                            n = De(e.target.value);
+                            n = Ke(e.target.value);
                         M({
                             ...r,
                             ["sm_output_kms_key" === t ? "outputKMSError" : "ebsKMSError"]: n
                         })
                     };
                     return o().createElement("div", {
-                        className: H
-                    }, o().createElement(q, {
+                        className: q
+                    }, o().createElement($, {
                         "aria-label": "role_arn",
                         name: "role_arn",
                         disabled: O,
                         readOnly: e,
                         required: !0,
-                        labelInfo: Ue.RoleArn,
+                        labelInfo: He.RoleArn,
                         errorMessage: r.roleError,
-                        placeholder: Ue.Placeholders.RolePlaceHolder,
+                        placeholder: He.Placeholders.RolePlaceHolder,
                         onChange: S,
                         value: t.role_arn,
                         onBlur: e => {
                             const {
                                 value: t
-                            } = e.target, n = ze(t);
-                            T(t), M({
+                            } = e.target, n = Re(t);
+                            j(t), M({
                                 ...r,
                                 roleError: n
                             })
                         },
-                        toolTipText: C.isStudio ? We.RoleArnTooltip : Ye.RoleArnTooltip
-                    }), o().createElement(q, {
+                        toolTipText: I.isStudio ? Ye.RoleArnTooltip : Ue.RoleArnTooltip
+                    }), o().createElement($, {
                         name: "s3_input",
                         onChange: S,
                         required: !0,
                         disabled: O,
                         readOnly: e,
                         value: t.s3_input,
-                        placeholder: Ue.Placeholders.S3BucketPlaceHolder,
-                        labelInfo: Ue.s3InputFolder,
+                        placeholder: He.Placeholders.S3BucketPlaceHolder,
+                        labelInfo: He.s3InputFolder,
                         errorMessage: r.s3InputFolderError,
                         onBlur: A,
-                        toolTipText: C.isStudio ? We.InputFolderTooltip : Ye.InputFolderTooltip
-                    }), o().createElement(q, {
+                        toolTipText: I.isStudio ? Ye.InputFolderTooltip : Ue.InputFolderTooltip
+                    }), o().createElement($, {
                         name: "s3_output",
                         onChange: S,
                         required: !0,
                         disabled: O,
                         readOnly: e,
                         value: t.s3_output,
-                        placeholder: Ue.Placeholders.S3BucketPlaceHolder,
-                        labelInfo: Ue.s3OutputFolder,
+                        placeholder: He.Placeholders.S3BucketPlaceHolder,
+                        labelInfo: He.s3OutputFolder,
                         errorMessage: r.s3OutputFolderError,
                         onBlur: A,
-                        toolTipText: C.isStudio ? We.OutputFolderTooltip : Ye.OutputFolderTooltip
+                        toolTipText: I.isStudio ? Ye.OutputFolderTooltip : Ue.OutputFolderTooltip
                     }), !e && o().createElement("div", {
-                        className: Y
-                    }, o().createElement(p.Checkbox, {
+                        className: U
+                    }, o().createElement(d.Checkbox, {
                         "data-testid": "kms_checkbox",
                         name: "kms_checkbox",
-                        className: X,
+                        className: Q,
                         color: "primary",
-                        checked: I,
+                        checked: C,
                         onChange: e => {
                             const n = e.target.checked;
                             N(n);
                             const o = n ? E.sm_output_kms_key : "",
                                 a = n ? E.sm_volume_kms_key : "";
                             y({
                                 ...t,
                                 sm_output_kms_key: o,
                                 sm_volume_kms_key: a
                             }), M({
                                 ...r,
-                                outputKMSError: De(o),
-                                ebsKMSError: De(a)
+                                outputKMSError: Ke(o),
+                                ebsKMSError: Ke(a)
                             })
                         }
-                    }), o().createElement("label", null, Ue.enableEncryption), o().createElement(j, {
+                    }), o().createElement("label", null, He.enableEncryption), o().createElement(T, {
                         classes: {
-                            popperInteractive: ee
+                            popperInteractive: X
                         },
-                        title: Xe,
+                        title: Qe,
                         interactive: !0
-                    }, o().createElement(f.Z, {
+                    }, o().createElement(h.Z, {
                         fontSize: "small"
-                    }))), (e || I) && o().createElement(o().Fragment, null, o().createElement(q, {
+                    }))), (e || C) && o().createElement(o().Fragment, null, o().createElement($, {
                         name: "sm_output_kms_key",
                         onChange: S,
                         required: !1,
                         readOnly: e,
                         disabled: O,
                         value: t.sm_output_kms_key,
-                        placeholder: e ? Ue.Placeholders.NoneSelected : Ue.enterKMSArnOrID,
-                        labelInfo: Ue.kmsKey,
+                        placeholder: e ? He.Placeholders.NoneSelected : He.enterKMSArnOrID,
+                        labelInfo: He.kmsKey,
                         errorMessage: r.outputKMSError,
                         onBlur: F,
-                        toolTipText: e ? void 0 : Ye.kmsKeyTooltip
-                    }), o().createElement(q, {
+                        toolTipText: e ? void 0 : Ue.kmsKeyTooltip
+                    }), o().createElement($, {
                         name: "sm_volume_kms_key",
                         onChange: S,
                         required: !1,
                         readOnly: e,
                         disabled: O,
                         value: t.sm_volume_kms_key,
-                        placeholder: e ? Ue.Placeholders.NoneSelected : Ue.enterKMSArnOrID,
-                        labelInfo: Ue.ebsKey,
+                        placeholder: e ? He.Placeholders.NoneSelected : He.enterKMSArnOrID,
+                        labelInfo: He.ebsKey,
                         errorMessage: r.ebsKMSError,
                         onBlur: F,
-                        toolTipText: e ? void 0 : Ye.ebsKeyTooltip
-                    })), d && !e && o().createElement(ie, {
-                        isChecked: h,
+                        toolTipText: e ? void 0 : Ue.ebsKeyTooltip
+                    })), g && !e && o().createElement(le, {
+                        isChecked: f,
                         setChecked: P,
                         initialSecurityGroups: m,
                         initialSubnets: c,
                         availableSubnets: u,
                         formState: t,
                         formErrors: r,
                         setFormErrors: M,
                         setFormState: y,
                         "data-testid": "vpc-checkbox"
-                    }), (d && h || e) && o().createElement(o().Fragment, null, o().createElement(Ce, {
+                    }), (g && f || e) && o().createElement(o().Fragment, null, o().createElement(je, {
                         required: !0,
                         name: "vpc_subnets",
                         disabled: e || 0 === u.length,
-                        label: Ue.subnet,
+                        label: He.subnet,
                         options: u,
                         value: t.vpc_subnets,
                         onChange: (e, n, o) => {
                             const [a, l] = ((e, t) => {
-                                if (0 === e.length) return 0 === t.length ? ["", ""] : [Fe.AdvancedOptions.SubnetMinError, void 0];
+                                if (0 === e.length) return 0 === t.length ? ["", ""] : [Ae.AdvancedOptions.SubnetMinError, void 0];
                                 if (e && e.length > 0) {
-                                    if (e.length > 16) return [Fe.AdvancedOptions.SubnetsMaxError, void 0];
+                                    if (e.length > 16) return [Ae.AdvancedOptions.SubnetsMaxError, void 0];
                                     for (const t of e) {
-                                        if (t.length > 32) return [Fe.AdvancedOptions.SubnetLengthError, void 0];
-                                        if (!Ne.test(t)) return [Fe.AdvancedOptions.SubnetsFormatError, void 0]
+                                        if (t.length > 32) return [Ae.AdvancedOptions.SubnetLengthError, void 0];
+                                        if (!Ce.test(t)) return [Ae.AdvancedOptions.SubnetsFormatError, void 0]
                                     }
-                                    if (0 === t.length) return ["", Fe.AdvancedOptions.SecurityGroupMinError]
+                                    if (0 === t.length) return ["", Ae.AdvancedOptions.SecurityGroupMinError]
                                 }
                                 return ["", void 0]
                             })(n, t.vpc_security_group_ids);
                             k(n), M({
                                 ...r,
                                 securityGroupError: null != l ? l : r.securityGroupError,
                                 subnetError: null != a ? a : ""
                             })
                         },
                         errorMessage: r.subnetError,
-                        placeholder: `${Ue.Placeholders.SelectPrivateSubnets}`,
-                        tooltip: C.isStudio ? We.SubnetTooltip : Ye.SubnetTooltip,
-                        disabledTooltip: `${Ue.Placeholders.NoPrivateSubnets}`,
+                        placeholder: `${He.Placeholders.SelectPrivateSubnets}`,
+                        tooltip: I.isStudio ? Ye.SubnetTooltip : Ue.SubnetTooltip,
+                        disabledTooltip: `${He.Placeholders.NoPrivateSubnets}`,
                         freeSolo: !0
-                    }), o().createElement(Ce, {
+                    }), o().createElement(je, {
                         required: !0,
                         className: "securityGroupSelector",
                         name: "vpc_security_group_ids",
                         disabled: e || 0 === u.length,
-                        label: Ue.securityGroup,
+                        label: He.securityGroup,
                         options: s,
                         value: t.vpc_security_group_ids,
                         onChange: (e, n, o) => {
                             const [a, l] = ((e, t) => {
-                                if (0 === e.length) return 0 === t.length ? ["", ""] : [Fe.AdvancedOptions.SecurityGroupMinError, void 0];
+                                if (0 === e.length) return 0 === t.length ? ["", ""] : [Ae.AdvancedOptions.SecurityGroupMinError, void 0];
                                 if (e.length > 0) {
-                                    if (e.length > 5) return [Fe.AdvancedOptions.SecurityGroupsMaxError, void 0];
+                                    if (e.length > 5) return [Ae.AdvancedOptions.SecurityGroupsMaxError, void 0];
                                     for (const t of e) {
-                                        if (!t.startsWith("sg-")) return [Fe.AdvancedOptions.SecurityGroupSGError, void 0];
-                                        if (t.length > 32) return [Fe.AdvancedOptions.SecurityGroupLengthError, void 0];
-                                        if (!Ne.test(t)) return [Fe.AdvancedOptions.SecurityGroupFormatError, void 0]
+                                        if (!t.startsWith("sg-")) return [Ae.AdvancedOptions.SecurityGroupSGError, void 0];
+                                        if (t.length > 32) return [Ae.AdvancedOptions.SecurityGroupLengthError, void 0];
+                                        if (!Ce.test(t)) return [Ae.AdvancedOptions.SecurityGroupFormatError, void 0]
                                     }
-                                    if (0 === t.length) return ["", Fe.AdvancedOptions.SubnetMinError]
+                                    if (0 === t.length) return ["", Ae.AdvancedOptions.SubnetMinError]
                                 }
                                 return ["", void 0]
                             })(n, t.vpc_subnets);
                             x(n), M({
                                 ...r,
                                 securityGroupError: null != a ? a : "",
                                 subnetError: null != l ? l : r.subnetError
                             })
                         },
                         errorMessage: r.securityGroupError,
-                        placeholder: `${Ue.Placeholders.selectOrAdd} ${Ue.securityGroup}`,
-                        tooltip: C.isStudio ? We.SecurityGroupsTooltip : Ye.SecurityGroupsTooltip,
-                        disabledTooltip: `${Ue.Placeholders.No} ${Ue.securityGroup}`,
+                        placeholder: `${He.Placeholders.selectOrAdd} ${He.securityGroup}`,
+                        tooltip: I.isStudio ? Ye.SecurityGroupsTooltip : Ue.SecurityGroupsTooltip,
+                        disabledTooltip: `${He.Placeholders.No} ${He.securityGroup}`,
                         freeSolo: !0
-                    })), C.isStudio && o().createElement("div", {
-                        className: te
-                    }, o().createElement(He.Z, {
+                    })), I.isStudio && o().createElement("div", {
+                        className: ee
+                    }, o().createElement(qe.Z, {
                         id: "startup-script-select-label"
-                    }, Ue.startUpScript, o().createElement(j, {
-                        title: et,
+                    }, He.startUpScript, o().createElement(T, {
+                        title: Xe,
                         interactive: !0
-                    }, o().createElement(f.Z, {
+                    }, o().createElement(h.Z, {
                         fontSize: "small"
-                    }))), o().createElement(qe.Z, {
+                    }))), o().createElement($e.Z, {
                         labelId: "startup-script-select-label",
                         id: "startup-script-select",
                         disabled: O,
                         readOnly: e,
                         value: t.sm_lcc_init_script_arn,
                         onChange: e => w(e.target.value)
                     }, i && i.map((e => o().createElement(Ze.Z, {
                         key: e,
                         value: e
-                    }, e))))), o().createElement(we, {
+                    }, e))))), o().createElement(xe, {
                         isButtonDisabled: e || a.length >= 48 || !!r.environmentVariablesError,
                         allFieldsDisabled: e,
                         environmentVariables: a,
                         setEnvironmentVariables: l,
                         formErrors: r,
                         setFormErrors: M
-                    }), o().createElement("div", null, o().createElement(q, {
-                        placeholder: e ? Ue.Placeholders.NoneSelected : Ue.efsPlaceholder,
-                        labelInfo: Ue.efsLabel,
+                    }), o().createElement("div", null, o().createElement($, {
+                        placeholder: e ? He.Placeholders.NoneSelected : He.efsPlaceholder,
+                        labelInfo: He.efsLabel,
                         required: !1,
                         value: t.sm_init_script,
                         name: "sm_init_script",
                         readOnly: e,
                         disabled: O,
                         errorMessage: r.efsFilePathError,
                         onChange: S,
                         onBlur: e => {
                             const t = e.target.value;
                             0 === t.trim().length ? M({
                                 ...r,
                                 efsFilePathError: ""
                             }) : (async e => {
-                                const t = v.URLExt.join(b.baseUrl, "/validate_volume_path");
+                                const t = p.URLExt.join(b.baseUrl, "/validate_volume_path");
                                 V(!0);
-                                const n = await g.ServerConnection.makeRequest(t, {
+                                const n = await v.ServerConnection.makeRequest(t, {
                                     method: "POST",
                                     body: JSON.stringify({
                                         file_path: e
                                     })
                                 }, b);
                                 V(!1), 200 !== n.status || !0 === (await n.json()).file_path_exist ? M({
                                     ...r,
                                     efsFilePathError: ""
                                 }) : M({
                                     ...r,
-                                    efsFilePathError: Qe.AdvancedOptions.EFSFilePathError
+                                    efsFilePathError: We.AdvancedOptions.EFSFilePathError
                                 })
                             })(t)
                         },
-                        toolTipText: e ? void 0 : C.isStudio ? We.InitialScriptTooltip : Ye.InitialScriptTooltip
-                    })), o().createElement(q, {
+                        toolTipText: e ? void 0 : I.isStudio ? Ye.InitialScriptTooltip : Ue.InitialScriptTooltip
+                    })), o().createElement($, {
                         name: "max_retry_attempts",
                         type: "number",
                         onChange: _,
                         required: !0,
                         disabled: O,
                         readOnly: e,
                         value: t.max_retry_attempts,
-                        placeholder: Ue.maxRetryAttempts,
-                        labelInfo: Ue.maxRetryAttempts,
+                        placeholder: He.maxRetryAttempts,
+                        labelInfo: He.maxRetryAttempts,
                         errorMessage: r.maxRetryAttemptsError,
                         onBlur: e => {
                             const t = (e => {
                                 const t = parseInt(e);
-                                return isNaN(t) || t < 0 || t > 30 ? Fe.AdvancedOptions.MaxRetryAttemptsError : ""
+                                return isNaN(t) || t < 0 || t > 30 ? Ae.AdvancedOptions.MaxRetryAttemptsError : ""
                             })(e.target.value);
                             M({
                                 ...r,
                                 maxRetryAttemptsError: t
                             })
                         },
-                        toolTipText: Ye.MaxRetryAttempts
-                    }), o().createElement(q, {
+                        toolTipText: Ue.MaxRetryAttempts
+                    }), o().createElement($, {
                         name: "max_run_time_in_seconds",
                         type: "number",
                         onChange: _,
                         required: !0,
                         disabled: O,
                         readOnly: e,
                         value: t.max_run_time_in_seconds,
-                        placeholder: Ue.maxRunTimeInSeconds,
-                        labelInfo: Ue.maxRunTimeInSeconds,
+                        placeholder: He.maxRunTimeInSeconds,
+                        labelInfo: He.maxRunTimeInSeconds,
                         errorMessage: r.maxRunTimeInSecondsError,
                         onBlur: e => {
                             const t = (e => {
                                 const t = parseInt(e);
-                                return isNaN(t) || t < 0 ? Fe.AdvancedOptions.MaxRunTimeInSecondsError : ""
+                                return isNaN(t) || t < 0 ? Ae.AdvancedOptions.MaxRunTimeInSecondsError : ""
                             })(e.target.value);
                             M({
                                 ...r,
                                 maxRunTimeInSecondsError: t
                             })
                         },
-                        toolTipText: Ye.MaxRunTimeInSeconds
+                        toolTipText: Ue.MaxRunTimeInSeconds
                     }))
                 },
-                rt = "No script",
-                nt = new Set(["sm_kernel", "sm_image", "sm_lcc_init_script_arn", "role_arn", "vpc_security_group_ids", "vpc_subnets", "s3_input", "s3_output", "sm_init_script", "sm_output_kms_key", "sm_volume_kms_key", "max_run_time_in_seconds", "max_retry_attempts"]),
-                ot = (e, t, r, n) => {
+                tt = "No script",
+                rt = new Set(["sm_kernel", "sm_image", "sm_lcc_init_script_arn", "role_arn", "vpc_security_group_ids", "vpc_subnets", "s3_input", "s3_output", "sm_init_script", "sm_output_kms_key", "sm_volume_kms_key", "max_run_time_in_seconds", "max_retry_attempts"]),
+                nt = (e, t, r, n) => {
                     var o, a;
                     if (r === l.JobsView.JobDetail || r === l.JobsView.JobDefinitionDetail) {
                         if (e) return e[n] ? e[n].split(",") : []
                     } else if (r === l.JobsView.CreateForm) {
                         if (e && n in e) {
                             const t = e[n];
                             return t ? t.split(",") : []
                         }
                         const r = null === (o = null == t ? void 0 : t.find((e => e.name === n))) || void 0 === o ? void 0 : o.value;
                         return (null === (a = null == r ? void 0 : r.filter((e => e.is_selected))) || void 0 === a ? void 0 : a.map((e => e.name))) || []
                     }
                     return []
                 },
-                at = (e, t, r, n) => {
+                ot = (e, t, r, n) => {
                     var o;
                     if (r === l.JobsView.JobDetail || r === l.JobsView.JobDefinitionDetail) {
                         if (e) return e[n]
                     } else if (r === l.JobsView.CreateForm) return e && n in e ? e[n] : (null === (o = null == t ? void 0 : t.find((e => e.name === n))) || void 0 === o ? void 0 : o.value) || "";
                     return ""
                 },
-                lt = (e, t, r, n) => {
+                at = (e, t, r, n) => {
                     if (t === l.JobsView.JobDetail || t === l.JobsView.JobDefinitionDetail) {
                         if (e) return e[n]
                     } else if (t === l.JobsView.CreateForm && e && n in e) return e[n];
                     return r
                 },
-                it = (e, t, r) => {
+                lt = (e, t, r) => {
                     if (t === l.JobsView.JobDetail || t === l.JobsView.JobDefinitionDetail) {
                         if (e) return e[r]
                     } else if (t === l.JobsView.CreateForm && e && r in e) return e[r];
                     return ""
                 },
-                st = ({
+                it = ({
                     label: e,
                     value: t,
                     options: r,
                     onChange: n,
                     freeSolo: a,
                     customListItemRender: l,
                     renderInput: i,
                     ...s
                 }) => {
                     var u;
                     const c = Object.fromEntries(r.map((e => [e.value, e])));
                     let m = t;
-                    return !a && "string" == typeof t && t in c && (m = c[t]), o().createElement(o().Fragment, null, o().createElement(Pe.Z, {
+                    return !a && "string" == typeof t && t in c && (m = c[t]), o().createElement(o().Fragment, null, o().createElement(Me.Z, {
                         ...s,
                         id: `${e}-selectinput`,
                         renderOption: (e, t, r) => o().createElement("li", {
                             ...e
                         }, l ? l(t, t.label, r.selected) : t.label),
                         componentsProps: {
                             ...s.componentsProps,
@@ -1355,179 +1354,179 @@
                             }
                         },
                         options: r,
                         onChange: (e, t, r) => {
                             (t && "string" != typeof t || a) && n && n(t || "")
                         },
                         value: m,
-                        renderInput: i || (e => o().createElement(Te.Z, {
+                        renderInput: i || (e => o().createElement(Pe.Z, {
                             ...e,
                             variant: "outlined",
                             size: "small",
                             margin: "dense"
                         }))
                     }))
                 },
-                ut = ({
+                st = ({
                     label: e,
                     required: t = !0,
                     toolTipText: r,
                     toolTipArea: n,
                     errorMessage: a,
                     ...l
                 }) => {
                     const i = n && o().createElement("div", null, o().createElement("span", {
-                        className: W
+                        className: Y
                     }, n.descriptionText), n.toolTipComponent);
                     return o().createElement("div", {
-                        className: C
+                        className: j
                     }, o().createElement("div", {
-                        className: N
+                        className: C
                     }, o().createElement("label", {
-                        className: R(t)
-                    }, e), (r || n) && !l.readOnly && o().createElement(j, {
+                        className: F(t)
+                    }, e), (r || n) && !l.readOnly && o().createElement(T, {
                         title: i || r || "",
-                        className: O,
+                        className: N,
                         interactive: null !== n
-                    }, o().createElement(f.Z, null))), o().createElement(st, {
+                    }, o().createElement(h.Z, null))), o().createElement(it, {
                         label: e,
                         disableClearable: !0,
                         ...l
                     }))
                 },
-                ct = E.css`
+                ut = f.css`
   display: flex;
   flex-direction: column;
   padding: 10px;
 `,
-                mt = E.css`
+                ct = f.css`
   display: flex;
   flex-direction: column;
   gap: 20px;
 `,
-                dt = E.css`
+                mt = f.css`
   display: flex;
   flex-direction: column;
 `,
-                pt = (E.css`
+                dt = (f.css`
   transform: rotate(90deg);
-`, E.css`
+`, f.css`
   display: flex;
   flex-flow: row nowrap;
   justify-content: space-between;
   align-items: center;
   width: 100%;
 `),
-                vt = E.css`
+                pt = f.css`
   font-size: var(--jp-ui-font-size0);
   min-width: max-content;
 `,
-                gt = E.css`
+                vt = f.css`
   font-size: var(--jp-ui-font-size0);
   color: var(--jp-inverse-layout-color4);
   padding-right: 5px;
   text-overflow: ellipsis;
   overflow: hidden;
   white-space: nowrap;
 `,
-                bt = E.css`
+                gt = f.css`
   width: 100%;
 `,
-                ht = E.css`
+                bt = f.css`
   display: flex;
   flex-direction: row;
   justify-content: space-between;
   &[data-selected='true'] {
     background-image: var(--jp-check-icon);
     background-size: 15px;
     background-repeat: no-repeat;
     background-position: 100% center;
   }
   & > p {
     max-width: calc(100% - 10px);
   }
 `,
-                ft = (e, t, r) => o().createElement("span", {
-                    className: bt
+                ht = (e, t, r) => o().createElement("span", {
+                    className: gt
                 }, o().createElement("div", {
-                    className: ht,
+                    className: bt,
                     "data-selected": r
-                }, o().createElement("p", null, t || e.label)), Et(e.optionMetadata && e.optionMetadata.description)),
-                Et = e => {
+                }, o().createElement("p", null, t || e.label)), ft(e.optionMetadata && e.optionMetadata.description)),
+                ft = e => {
                     if (!e) return;
                     const t = e.match(/(((https?:\/\/)|(www\.))[^\s]+)/g);
                     if (t)
                         for (const r of t) e = e.replace(r, " ");
                     const r = e.trim();
                     return o().createElement("div", {
-                        className: pt
+                        className: dt
                     }, o().createElement("span", {
-                        className: gt
-                    }, r), t && t.map((e => o().createElement(L, {
-                        className: vt,
+                        className: vt
+                    }, r), t && t.map((e => o().createElement(D, {
+                        className: pt,
                         key: e,
                         href: e,
-                        target: z.External
-                    }, s.KernelSelector.imageSelectorOption.linkText))))
+                        target: R.External
+                    }, i.KernelSelector.imageSelectorOption.linkText))))
                 };
             r(9850);
-            const yt = ["datascience-1.0", "sagemaker-data-science-38", "1.8.1-cpu-py36", "pytorch-1.8-gpu-py36", "sagemaker-sparkmagic", "tensorflow-2.6-cpu-py38-ubuntu20.04-v1", "tensorflow-2.6-gpu-py38-cu112-ubuntu20.04-v1", "sagemaker-sparkanalytics-v1"];
-            var St;
+            const Et = ["datascience-1.0", "sagemaker-data-science-38", "1.8.1-cpu-py36", "pytorch-1.8-gpu-py36", "sagemaker-sparkmagic", "tensorflow-2.6-cpu-py38-ubuntu20.04-v1", "tensorflow-2.6-gpu-py38-cu112-ubuntu20.04-v1", "sagemaker-sparkanalytics-v1"];
+            var yt;
             ! function(e) {
                 e.Custom = "customImage", e.Sagemaker = "smeImage", e.Session = "session"
-            }(St || (St = {}));
-            const _t = {
+            }(yt || (yt = {}));
+            const St = {
                 smeImage: "Sagemaker Image",
                 customImage: "Custom Image",
                 prefered: "Use image from preferred session",
                 session: "Use image from other session"
             };
 
-            function kt(e, t, r) {
+            function _t(e, t, r) {
                 const n = Object.values(e).filter((e => {
                     const n = e.arnEnvironment.split("/")[1];
-                    return r ? (null == e ? void 0 : e.group) === t && yt.includes(n) : ((null == e ? void 0 : e.group) !== St.Sagemaker || !e.label.includes("Geospatial")) && (null == e ? void 0 : e.group) === t
+                    return r ? (null == e ? void 0 : e.group) === t && Et.includes(n) : ((null == e ? void 0 : e.group) !== yt.Sagemaker || !e.label.includes("Geospatial")) && (null == e ? void 0 : e.group) === t
                 }));
                 return {
-                    label: _t[t],
+                    label: St[t],
                     value: "",
                     options: n.map((e => ({
                         label: e.label,
-                        value: t === St.Session ? e.label : e.arnEnvironment,
-                        group: _t[t],
+                        value: t === yt.Session ? e.label : e.arnEnvironment,
+                        group: St[t],
                         optionMetadata: e,
                         options: e.versionOptions
                     })))
                 }
             }
-            const xt = s.ScheduleNoteBook.MainPanel.Tooltips,
-                wt = s.ScheduleNoteBook.MainPanel.StudioTooltips,
-                Mt = ({
+            const kt = i.ScheduleNoteBook.MainPanel.Tooltips,
+                xt = i.ScheduleNoteBook.MainPanel.StudioTooltips,
+                wt = ({
                     isDisabled: e,
                     formState: t,
                     formErrors: r,
                     setFormState: a,
-                    setFormErrors: i,
+                    setFormErrors: s,
                     model: u,
                     jobsView: c,
                     requestClient: m,
                     contentsManager: d
                 }) => {
-                    var p, b;
+                    var g, b;
                     const {
                         pluginEnvironment: h
-                    } = $e(), [f, E] = (0, n.useState)({
+                    } = Ge(), [f, E] = (0, n.useState)({
                         arnEnvironment: null,
                         kernel: null,
                         version: null
                     }), [y, S] = (0, n.useState)({});
                     (0, n.useEffect)((() => {
                         (async function(e) {
-                            const t = v.URLExt.join(e.baseUrl, "api/kernelspecs"),
-                                r = await g.ServerConnection.makeRequest(t, {}, e);
+                            const t = p.URLExt.join(e.baseUrl, "api/kernelspecs"),
+                                r = await v.ServerConnection.makeRequest(t, {}, e);
                             if (200 === r.status) return await r.json()
                         })(m).then((async e => {
                             var r;
                             e && S(function(e) {
                                 const t = {},
                                     r = e.kernelspecs;
                                 return Object.values(r).forEach((e => {
@@ -1535,15 +1534,15 @@
                                     if (!e) return;
                                     const n = (null === (r = e.spec) || void 0 === r ? void 0 : r.metadata) ? e.spec.metadata.sme_metadata : null,
                                         {
                                             imageName: o,
                                             kernelName: a
                                         } = function(e) {
                                             try {
-                                                if (!G()(e) || 0 === e.length) return {
+                                                if (!B()(e) || 0 === e.length) return {
                                                     imageName: null,
                                                     kernelName: null
                                                 };
                                                 const [t, r] = e.split("(");
                                                 return {
                                                     imageName: r && r.slice(0, -1).split("/")[0],
                                                     kernelName: t && t.slice(0, -1)
@@ -1555,29 +1554,29 @@
                                                 }
                                             }
                                         }(e.spec.display_name),
                                         {
                                             kernel: l,
                                             arnEnvironment: i,
                                             version: s
-                                        } = $(e.name);
+                                        } = G(e.name);
                                     if (!(l && i && o && a)) return;
                                     const u = {
                                         arnEnvironment: i,
                                         kernelOptions: [{
                                             label: a,
                                             value: l
                                         }],
                                         versionOptions: s ? [{
                                             label: `v${s}`,
                                             value: s
                                         }] : void 0,
                                         label: s ? `${o} v${s}` : o,
                                         description: (null == n ? void 0 : n.description) ? n.description : void 0,
-                                        group: n && n.is_template ? St.Sagemaker : St.Custom
+                                        group: n && n.is_template ? yt.Sagemaker : yt.Custom
                                     };
                                     if (t[i]) {
                                         const {
                                             kernelOptions: e
                                         } = t[i];
                                         if (!e.some((e => e.value === l))) {
                                             const r = [...e, {
@@ -1612,77 +1611,77 @@
                             }(u.inputFile, d), o = n in (null !== (r = null == e ? void 0 : e.kernelspecs) && void 0 !== r ? r : {}) ? n : "", i = ((e, t, r) => {
                                 if (r === l.JobsView.JobDetail || r === l.JobsView.JobDefinitionDetail) {
                                     if (e) {
                                         const {
                                             sm_kernel: t,
                                             sm_image: r
                                         } = e;
-                                        return $(`${t}__SAGEMAKER_INTERNAL__${r}`)
+                                        return G(`${t}__SAGEMAKER_INTERNAL__${r}`)
                                     }
                                     return {
                                         kernel: null,
                                         arnEnvironment: null,
                                         version: null
                                     }
                                 }
                                 if (r === l.JobsView.CreateForm) {
                                     if (e && "sm_image" in e) {
                                         const {
                                             sm_kernel: t,
                                             sm_image: r
                                         } = e;
-                                        return $(`${t}__SAGEMAKER_INTERNAL__${r}`)
+                                        return G(`${t}__SAGEMAKER_INTERNAL__${r}`)
                                     }
-                                    return $(t) || {
+                                    return G(t) || {
                                         kernel: null,
                                         arnEnvironment: null,
                                         version: null
                                     }
                                 }
-                                return $(t) || {
+                                return G(t) || {
                                     kernel: null,
                                     arnEnvironment: null,
                                     version: null
                                 }
                             })(u.runtimeEnvironmentParameters, o, c);
                             E(i), a({
                                 ...t,
                                 sm_kernel: i.kernel || "",
                                 sm_image: i.arnEnvironment || ""
                             })
                         }))
                     }), []);
-                    const _ = [...null !== (p = kt(y, St.Sagemaker, !1).options) && void 0 !== p ? p : [], ...null !== (b = kt(y, St.Custom).options) && void 0 !== b ? b : []],
+                    const _ = [...null !== (g = _t(y, yt.Sagemaker, !1).options) && void 0 !== g ? g : [], ...null !== (b = _t(y, yt.Custom).options) && void 0 !== b ? b : []],
                         k = (0, n.useMemo)((() => {
                             var e;
                             return f.arnEnvironment && (null === (e = y[f.arnEnvironment]) || void 0 === e ? void 0 : e.kernelOptions) || []
                         }), [y, f]),
                         x = !!r.jobEnvironmentError,
                         w = o().createElement("div", {
-                            className: F
-                        }, o().createElement(se.Z, {
+                            className: A
+                        }, o().createElement(ie.Z, {
                             severity: "error"
                         }, r.jobEnvironmentError));
                     return (0, n.useEffect)((() => {
-                        f.arnEnvironment && f.kernel && r.jobEnvironmentError && i({
+                        f.arnEnvironment && f.kernel && r.jobEnvironmentError && s({
                             ...r,
                             jobEnvironmentError: ""
                         })
                     }), [f.arnEnvironment, f.kernel]), 0 === Object.keys(y).length ? null : o().createElement("div", {
+                        className: ut
+                    }, o().createElement("div", {
                         className: ct
                     }, o().createElement("div", {
                         className: mt
-                    }, o().createElement("div", {
-                        className: dt
-                    }, o().createElement(ut, {
+                    }, o().createElement(st, {
                         "data-testid": "sm_image_dropdown",
                         options: _,
                         value: f.arnEnvironment,
-                        label: s.ImageSelector.label,
-                        customListItemRender: ft,
+                        label: i.ImageSelector.label,
+                        customListItemRender: ht,
                         onChange: (e, r) => {
                             var n;
                             if (!e || "string" == typeof e) return;
                             const o = (null === (n = e.optionMetadata) || void 0 === n ? void 0 : n.kernelOptions) || [],
                                 l = o.length > 0 ? o[0].value : null,
                                 i = r ? r.value : null;
                             a({
@@ -1696,37 +1695,37 @@
                             })
                         },
                         readOnly: e,
                         groupBy: e => {
                             var t;
                             return null !== (t = e.group) && void 0 !== t ? t : ""
                         },
-                        toolTipText: h.isStudio ? wt.ImageTooltipText : xt.ImageTooltipText
+                        toolTipText: h.isStudio ? xt.ImageTooltipText : kt.ImageTooltipText
                     }), r.jobEnvironmentError && o().createElement("div", {
-                        className: A
-                    }, x && w)), o().createElement(ut, {
+                        className: V
+                    }, x && w)), o().createElement(st, {
                         options: k,
                         value: f.kernel,
-                        label: s.KernelSelector.label,
+                        label: i.KernelSelector.label,
                         onChange: e => {
                             e && "string" != typeof e && e && (a({
                                 ...t,
                                 sm_kernel: e.value
                             }), E({
                                 ...f,
                                 kernel: e.value
                             }))
                         },
                         readOnly: e,
-                        toolTipText: h.isStudio ? wt.KernelTooltipText : xt.KernelTooltipText
+                        toolTipText: h.isStudio ? xt.KernelTooltipText : kt.KernelTooltipText
                     })))
                 },
-                Pt = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
-                Tt = s.ScheduleNoteBook.MainPanel.Tooltips,
-                jt = ({
+                Mt = i.ScheduleNoteBook.MainPanel.AdvancedOptions,
+                Pt = i.ScheduleNoteBook.MainPanel.Tooltips,
+                Tt = ({
                     setFormState: e,
                     formState: t,
                     isDisabled: r,
                     formErrors: a,
                     setFormErrors: l,
                     model: i,
                     executionEnvironments: s
@@ -1734,19 +1733,19 @@
                     const u = (0, n.useMemo)((() => ((e, t) => {
                         var r, n;
                         if (e) {
                             const {
                                 sm_kernel: t,
                                 sm_image: r
                             } = e;
-                            return $(`${t}__SAGEMAKER_INTERNAL__${r}`)
+                            return G(`${t}__SAGEMAKER_INTERNAL__${r}`)
                         }
                         const o = null === (r = null == t ? void 0 : t.find((e => "image" === e.name))) || void 0 === r ? void 0 : r.value,
                             a = null === (n = null == t ? void 0 : t.find((e => "kernel" === e.name))) || void 0 === n ? void 0 : n.value;
-                        return J(o) && J(a) ? $(`${a}__SAGEMAKER_INTERNAL__${o}`) : {
+                        return L(o) && L(a) ? G(`${a}__SAGEMAKER_INTERNAL__${o}`) : {
                             kernel: null,
                             arnEnvironment: null,
                             version: null
                         }
                     })(i.runtimeEnvironmentParameters, null == s ? void 0 : s.auto_detected_config)), []);
                     (0, n.useEffect)((() => {
                         e({
@@ -1760,131 +1759,131 @@
                             o = r.target.value;
                         e({
                             ...t,
                             [n]: o
                         })
                     };
                     return o().createElement("div", {
-                        className: H
-                    }, o().createElement(q, {
+                        className: q
+                    }, o().createElement($, {
                         name: "sm_image",
                         onChange: c,
                         readOnly: r,
                         required: !0,
                         value: t.sm_image,
-                        placeholder: Pt.Placeholders.ImagePlaceHolder,
-                        labelInfo: Pt.Image,
+                        placeholder: Mt.Placeholders.ImagePlaceHolder,
+                        labelInfo: Mt.Image,
                         errorMessage: a.ImageError,
                         onBlur: e => {
                             const {
                                 value: t
-                            } = e.target, r = t.length <= 0 ? Fe.AdvancedOptions.ImageError : "";
+                            } = e.target, r = t.length <= 0 ? Ae.AdvancedOptions.ImageError : "";
                             l({
                                 ...a,
                                 ImageError: r
                             })
                         },
-                        toolTipText: Tt.ImageTooltipText
-                    }), o().createElement(q, {
+                        toolTipText: Pt.ImageTooltipText
+                    }), o().createElement($, {
                         name: "sm_kernel",
                         onChange: c,
                         readOnly: r,
                         required: !0,
                         value: t.sm_kernel,
-                        placeholder: Pt.Placeholders.KernelPlaceHolder,
-                        labelInfo: Pt.Kernel,
+                        placeholder: Mt.Placeholders.KernelPlaceHolder,
+                        labelInfo: Mt.Kernel,
                         errorMessage: a.KernelError,
                         onBlur: e => {
                             const {
                                 value: t
-                            } = e.target, r = t.length <= 0 ? Fe.AdvancedOptions.KernelError : "";
+                            } = e.target, r = t.length <= 0 ? Ae.AdvancedOptions.KernelError : "";
                             l({
                                 ...a,
                                 KernelError: r
                             })
                         },
-                        toolTipText: Tt.KernelTooltipText
+                        toolTipText: Pt.KernelTooltipText
                     }))
                 },
-                Ct = e => {
+                jt = e => {
                     const {
                         pluginEnvironment: t
-                    } = $e();
-                    return o().createElement(o().Fragment, null, t.isStudio && o().createElement(Mt, {
+                    } = Ge();
+                    return o().createElement(o().Fragment, null, t.isStudio && o().createElement(wt, {
                         ...e
-                    }), t.isLocalJL && o().createElement(jt, {
+                    }), t.isLocalJL && o().createElement(Tt, {
                         ...e
                     }))
                 },
                 It = e => {
                     const {
                         executionEnvironments: t,
                         settingRegistry: r,
                         jobsView: a,
                         requestClient: i,
                         errors: s,
                         handleErrorsChange: u,
-                        model: c,
+                        model: m,
                         handleModelChange: d
                     } = e, p = (0, n.useMemo)((() => {
                         return e = null == t ? void 0 : t.auto_detected_config, a === l.JobsView.CreateForm && (null === (r = null == e ? void 0 : e.find((e => "app_network_access_type" === e.name))) || void 0 === r ? void 0 : r.value) || "";
                         var e, r
                     }), []), v = (0, n.useMemo)((() => {
                         var e, r;
                         const n = [],
                             o = (null === (r = null === (e = t.auto_detected_config) || void 0 === e ? void 0 : e.find((e => "lcc_arn" === e.name))) || void 0 === r ? void 0 : r.value) || [];
-                        n.push(rt), n.push(...o);
-                        const i = (s = c.runtimeEnvironmentParameters, ((u = a) === l.JobsView.JobDetail || u === l.JobsView.JobDefinitionDetail) && s && s.sm_lcc_init_script_arn || rt);
+                        n.push(tt), n.push(...o);
+                        const i = (s = m.runtimeEnvironmentParameters, ((u = a) === l.JobsView.JobDetail || u === l.JobsView.JobDefinitionDetail) && s && s.sm_lcc_init_script_arn || tt);
                         var s, u;
-                        return c.runtimeEnvironmentParameters && i !== rt && n.push(i), {
+                        return m.runtimeEnvironmentParameters && i !== tt && n.push(i), {
                             allLCCOptions: n,
                             selectedLccValue: i
                         }
                     }), []), g = (0, n.useMemo)((() => ((e, t, r) => {
                         var n;
                         if (r === l.JobsView.JobDetail || r === l.JobsView.JobDefinitionDetail) {
                             if (e) return e.role_arn
                         } else if (r === l.JobsView.CreateForm) {
                             if (e && "role_arn" in e) return e.role_arn;
                             const r = null === (n = null == t ? void 0 : t.find((e => "role_arn" === e.name))) || void 0 === n ? void 0 : n.value;
                             if ((null == r ? void 0 : r.length) > 0) return r[0]
                         }
                         return ""
-                    })(c.runtimeEnvironmentParameters, t.auto_detected_config, a)), []), b = (0, n.useMemo)((() => at(c.runtimeEnvironmentParameters, t.auto_detected_config, a, "s3_output")), []), h = (0, n.useMemo)((() => at(c.runtimeEnvironmentParameters, t.auto_detected_config, a, "s3_input")), []), f = (0, n.useMemo)((() => lt(c.runtimeEnvironmentParameters, a, 1, "max_retry_attempts")), []), E = (0, n.useMemo)((() => lt(c.runtimeEnvironmentParameters, a, 172800, "max_run_time_in_seconds")), []), y = (0, n.useMemo)((() => {
+                    })(m.runtimeEnvironmentParameters, t.auto_detected_config, a)), []), b = (0, n.useMemo)((() => ot(m.runtimeEnvironmentParameters, t.auto_detected_config, a, "s3_output")), []), h = (0, n.useMemo)((() => ot(m.runtimeEnvironmentParameters, t.auto_detected_config, a, "s3_input")), []), f = (0, n.useMemo)((() => at(m.runtimeEnvironmentParameters, a, 1, "max_retry_attempts")), []), E = (0, n.useMemo)((() => at(m.runtimeEnvironmentParameters, a, 172800, "max_run_time_in_seconds")), []), y = (0, n.useMemo)((() => {
                         var e, r;
                         const n = (null === (r = null === (e = t.auto_detected_config) || void 0 === e ? void 0 : e.find((e => "vpc_security_group_ids" === e.name))) || void 0 === r ? void 0 : r.value) || [];
                         return null == n ? void 0 : n.map((e => e.name))
                     }), []), S = (0, n.useMemo)((() => {
                         var e, r;
                         const n = (null === (r = null === (e = t.auto_detected_config) || void 0 === e ? void 0 : e.find((e => "vpc_subnets" === e.name))) || void 0 === r ? void 0 : r.value) || [];
                         return null == n ? void 0 : n.map((e => e.name))
-                    }), []), _ = (0, n.useMemo)((() => p === m.PublicInternetOnly ? {
+                    }), []), _ = (0, n.useMemo)((() => p === c.PublicInternetOnly ? {
                         securityGroups: [],
                         subnets: []
                     } : {
-                        securityGroups: 0 === S.length && a === l.JobsView.CreateForm ? [] : ot(c.runtimeEnvironmentParameters, t.auto_detected_config, a, "vpc_security_group_ids"),
-                        subnets: ot(c.runtimeEnvironmentParameters, t.auto_detected_config, a, "vpc_subnets")
+                        securityGroups: 0 === S.length && a === l.JobsView.CreateForm ? [] : nt(m.runtimeEnvironmentParameters, t.auto_detected_config, a, "vpc_security_group_ids"),
+                        subnets: nt(m.runtimeEnvironmentParameters, t.auto_detected_config, a, "vpc_subnets")
                     }), []), k = (0, n.useMemo)((() => ((e, t) => {
                         if (t === l.JobsView.JobDetail || t === l.JobsView.JobDefinitionDetail) {
                             if (e) return e.sm_init_script
                         } else if (t === l.JobsView.CreateForm && e && "sm_init_script" in e) return e.sm_init_script;
                         return ""
-                    })(c.runtimeEnvironmentParameters, a)), []), x = (0, n.useMemo)((() => (e => {
+                    })(m.runtimeEnvironmentParameters, a)), []), x = (0, n.useMemo)((() => (e => {
                         const t = [];
                         if (e)
                             for (const r in e)
-                                if (!nt.has(r)) {
+                                if (!rt.has(r)) {
                                     const n = {
                                         key: r,
                                         value: e[r]
                                     };
                                     t.push(n)
                                 } return t
-                    })(c.runtimeEnvironmentParameters)), []), w = (0, n.useMemo)((() => it(c.runtimeEnvironmentParameters, a, "sm_output_kms_key")), []), M = (0, n.useMemo)((() => it(c.runtimeEnvironmentParameters, a, "sm_volume_kms_key")), []), P = (0, n.useMemo)((() => {
-                        if (p === m.PublicInternetOnly) return !1;
+                    })(m.runtimeEnvironmentParameters)), []), w = (0, n.useMemo)((() => lt(m.runtimeEnvironmentParameters, a, "sm_output_kms_key")), []), M = (0, n.useMemo)((() => lt(m.runtimeEnvironmentParameters, a, "sm_volume_kms_key")), []), P = (0, n.useMemo)((() => {
+                        if (p === c.PublicInternetOnly) return !1;
                         const e = _.subnets;
                         return 0 !== S.length && (0 === e.length && S.length, !0)
                     }), []), [T, j] = (0, n.useState)({
                         sm_lcc_init_script_arn: v.selectedLccValue || "",
                         role_arn: g || "",
                         vpc_security_group_ids: _.securityGroups || "",
                         vpc_subnets: _.subnets || "",
@@ -1893,78 +1892,78 @@
                         sm_kernel: "",
                         sm_image: "",
                         sm_init_script: k || "",
                         sm_output_kms_key: w || "",
                         sm_volume_kms_key: M || "",
                         max_retry_attempts: f,
                         max_run_time_in_seconds: E
-                    }), [C, I] = (0, n.useState)({
+                    }), [I, C] = (0, n.useState)({
                         ...T,
                         sm_output_kms_key: "",
                         sm_volume_kms_key: ""
                     });
                     (0, n.useEffect)((() => {
-                        const e = (e => e && 0 === e.length ? `${Re.RequiresPrivateSubnet} ${Re.NoPrivateSubnetsInSageMakerDomain}` : "")(S),
-                            t = (r = _.subnets) && 0 === r.length ? `${Re.RequiresPrivateSubnet} ${Re.NoPrivateSubnetsInSageMakerDomain}. ${Re.YouMayChooseOtherSubnets}` : "";
+                        const e = (e => e && 0 === e.length ? `${Fe.RequiresPrivateSubnet} ${Fe.NoPrivateSubnetsInSageMakerDomain}` : "")(S),
+                            t = (r = _.subnets) && 0 === r.length ? `${Fe.RequiresPrivateSubnet} ${Fe.NoPrivateSubnetsInSageMakerDomain}. ${Fe.YouMayChooseOtherSubnets}` : "";
                         var r;
                         u({
                             ...s,
-                            roleError: ze(g),
-                            s3InputFolderError: Ke(h),
-                            s3OutputFolderError: Ke(b),
+                            roleError: Re(g),
+                            s3InputFolderError: ze(h),
+                            s3OutputFolderError: ze(b),
                             environmentsStillLoading: "",
                             kernelsStillLoading: "",
                             subnetError: P && (e || t) || ""
                         })
                     }), []);
-                    const [N, O] = (0, n.useState)();
+                    const [N, V] = (0, n.useState)();
                     (0, n.useEffect)((() => {
                         (async function(e) {
                             return (await e.get("@amzn/sagemaker-jupyter-scheduler:advanced-options", "advancedOptions")).composite
                         })(r).then((e => {
-                            O(e)
+                            V(e)
                         }))
                     }), []), (0, n.useEffect)((() => {
                         var e, t, r, n;
                         let o = {},
                             a = {},
                             l = {};
                         const i = null !== (e = null == N ? void 0 : N.role_arn) && void 0 !== e ? e : "";
                         i && i !== g && (o = {
                             ...o,
                             role_arn: i
                         }, a = {
                             ...a,
-                            roleError: ze(i)
+                            roleError: Re(i)
                         });
                         const c = null !== (t = null == N ? void 0 : N.s3_input) && void 0 !== t ? t : "";
                         c && c !== h && (o = {
                             ...o,
                             s3_input: c
                         }, a = {
                             ...a,
-                            s3InputFolderError: Ke(c)
+                            s3InputFolderError: ze(c)
                         });
                         const m = null !== (r = null == N ? void 0 : N.s3_output) && void 0 !== r ? r : "";
                         m && m !== b && (o = {
                             ...o,
                             s3_output: m
                         }, a = {
                             ...a,
-                            s3OutputFolderError: Ke(m)
+                            s3OutputFolderError: ze(m)
                         });
                         const d = null !== (n = null == N ? void 0 : N.sm_output_kms_key) && void 0 !== n ? n : "";
                         d && d !== w && (l = {
                             ...l,
                             sm_output_kms_key: d
                         }), l = {
                             ...o,
                             ...l
-                        }, Object.keys(o).length > 0 && I({
-                            ...C,
+                        }, Object.keys(o).length > 0 && C({
+                            ...I,
                             ...o
                         }), Object.keys(l).length > 0 && j({
                             ...T,
                             ...l
                         }), Object.keys(a).length > 0 && u({
                             ...s,
                             ...a
@@ -1978,53 +1977,53 @@
                                 value: n
                             } = t;
                             0 !== r.trim().length && 0 !== n.trim().length && (e[r] = n)
                         })), e
                     }), [A]);
                     (0, n.useEffect)((() => {
                         var e, t;
-                        const r = (null === (e = C.vpc_security_group_ids) || void 0 === e ? void 0 : e.join(",")) || "",
-                            n = (null === (t = C.vpc_subnets) || void 0 === t ? void 0 : t.join(",")) || "";
+                        const r = (null === (e = I.vpc_security_group_ids) || void 0 === e ? void 0 : e.join(",")) || "",
+                            n = (null === (t = I.vpc_subnets) || void 0 === t ? void 0 : t.join(",")) || "";
                         d({
-                            ...c,
+                            ...m,
                             runtimeEnvironmentParameters: {
-                                ...C,
+                                ...I,
                                 vpc_security_group_ids: r,
                                 vpc_subnets: n,
                                 ...K
                             }
                         })
-                    }), [C, K]);
+                    }), [I, K]);
                     const D = a === l.JobsView.JobDefinitionDetail || a === l.JobsView.JobDetail;
                     return o().createElement("div", {
-                        className: V(D)
-                    }, o().createElement(Ct, {
+                        className: O(D)
+                    }, o().createElement(jt, {
                         isDisabled: D,
-                        formState: C,
-                        setFormState: I,
+                        formState: I,
+                        setFormState: C,
                         formErrors: s,
                         setFormErrors: u,
                         ...e
-                    }), o().createElement(tt, {
+                    }), o().createElement(et, {
                         isDisabled: D,
-                        formState: C,
-                        setFormState: I,
+                        formState: I,
+                        setFormState: C,
                         handleChange: e => {
                             const t = e.target.name,
                                 r = e.target.value;
-                            I({
-                                ...C,
+                            C({
+                                ...I,
                                 [t]: r
                             })
                         },
                         handleNumberValueChange: e => {
                             const t = e.target.name,
                                 r = parseInt(e.target.value);
-                            I({
-                                ...C,
+                            C({
+                                ...I,
                                 [t]: isNaN(r) ? "" : r
                             })
                         },
                         requestClient: i,
                         formErrors: s,
                         setFormValidationErrors: u,
                         environmentVariables: A,
@@ -2032,51 +2031,51 @@
                         setEnvironmentVariables: F,
                         lccOptions: v.allLCCOptions,
                         availableSecurityGroups: y,
                         availableSubnets: S,
                         initialSecurityGroups: _.securityGroups,
                         initialSubnets: _.subnets,
                         setSubnets: e => {
-                            I({
-                                ...C,
+                            C({
+                                ...I,
                                 vpc_subnets: e
                             })
                         },
                         setRoleArn: e => {
-                            I({
-                                ...C,
+                            C({
+                                ...I,
                                 role_arn: e
                             })
                         },
                         setSecurityGroups: e => {
-                            I({
-                                ...C,
+                            C({
+                                ...I,
                                 vpc_security_group_ids: e
                             })
                         },
                         onSelectLCCScript: e => {
-                            I({
-                                ...C,
+                            C({
+                                ...I,
                                 sm_lcc_init_script_arn: e
                             })
                         },
-                        isVPCDomain: p === m.VpcOnly,
+                        isVPCDomain: p === c.VpcOnly,
                         enableVPCSetting: R,
                         setEnableVPCSetting: z
                     }))
                 };
-            var Nt = r(2453);
+            var Ct = r(2453);
 
-            function Ot(e) {
+            function Nt(e) {
                 return getComputedStyle(document.body).getPropertyValue(e).trim()
             }
 
-            function Vt() {
+            function Ot() {
                 const e = document.body.getAttribute("data-jp-theme-light");
-                return (0, Nt.Z)({
+                return (0, Ct.Z)({
                     spacing: 4,
                     components: {
                         MuiButton: {
                             defaultProps: {
                                 size: "small"
                             }
                         },
@@ -2159,179 +2158,146 @@
                             defaultProps: {
                                 variant: "dense"
                             }
                         }
                     },
                     palette: {
                         background: {
-                            paper: Ot("--jp-layout-color1"),
-                            default: Ot("--jp-layout-color1")
+                            paper: Nt("--jp-layout-color1"),
+                            default: Nt("--jp-layout-color1")
                         },
                         mode: "true" === e ? "light" : "dark",
                         primary: {
-                            main: Ot("--jp-brand-color1"),
-                            light: Ot("--jp-brand-color2"),
-                            dark: Ot("--jp-brand-color0")
+                            main: Nt("--jp-brand-color1"),
+                            light: Nt("--jp-brand-color2"),
+                            dark: Nt("--jp-brand-color0")
                         },
                         error: {
-                            main: Ot("--jp-error-color1"),
-                            light: Ot("--jp-error-color2"),
-                            dark: Ot("--jp-error-color0")
+                            main: Nt("--jp-error-color1"),
+                            light: Nt("--jp-error-color2"),
+                            dark: Nt("--jp-error-color0")
                         },
                         warning: {
-                            main: Ot("--jp-warn-color1"),
-                            light: Ot("--jp-warn-color2"),
-                            dark: Ot("--jp-warn-color0")
+                            main: Nt("--jp-warn-color1"),
+                            light: Nt("--jp-warn-color2"),
+                            dark: Nt("--jp-warn-color0")
                         },
                         success: {
-                            main: Ot("--jp-success-color1"),
-                            light: Ot("--jp-success-color2"),
-                            dark: Ot("--jp-success-color0")
+                            main: Nt("--jp-success-color1"),
+                            light: Nt("--jp-success-color2"),
+                            dark: Nt("--jp-success-color0")
                         },
                         text: {
-                            primary: Ot("--jp-ui-font-color1"),
-                            secondary: Ot("--jp-ui-font-color2"),
-                            disabled: Ot("--jp-ui-font-color3")
+                            primary: Nt("--jp-ui-font-color1"),
+                            secondary: Nt("--jp-ui-font-color2"),
+                            disabled: Nt("--jp-ui-font-color3")
                         }
                     },
                     shape: {
                         borderRadius: 2
                     },
                     typography: {
-                        fontFamily: Ot("--jp-ui-font-family"),
+                        fontFamily: Nt("--jp-ui-font-family"),
                         fontSize: 12,
                         htmlFontSize: 16,
                         button: {
                             textTransform: "capitalize"
                         }
                     }
                 })
             }
-            var At = r(5395);
-            const Ft = ({
+            var Vt = r(5395);
+            const At = ({
                     requestClient: e,
                     contentsManager: t,
                     commands: r,
                     jobsView: a,
-                    errors: i,
-                    handleErrorsChange: m,
+                    errors: c,
+                    handleErrorsChange: g,
                     ...b
                 }) => {
                     const [h, f] = (0, n.useState)("");
                     (0, n.useEffect)((() => {
                         const t = {
-                            ...i,
+                            ...c,
                             environmentsStillLoading: "EnvironmentsStillLoadingError",
                             kernelsStillLoading: "KernelsStillLoadingError"
                         };
-                        m(t), a === l.JobsView.CreateForm ? (async () => {
-                            const t = v.URLExt.join(e.baseUrl, "/advanced_environments"),
-                                n = await g.ServerConnection.makeRequest(t, {}, e);
+                        g(t), a === l.JobsView.CreateForm ? (async () => {
+                            const t = p.URLExt.join(e.baseUrl, "/advanced_environments"),
+                                n = await v.ServerConnection.makeRequest(t, {}, e);
                             if (200 !== n.status) {
                                 const e = (await n.json()).error_code;
-                                throw Object.values(u).indexOf(e) >= 0 && (async e => {
-                                    const t = o().createElement(o().Fragment, null, s.Dialog.awsCredentialsError.body.text.map(((e, t) => o().createElement("p", {
+                                throw Object.values(s).indexOf(e) >= 0 && (async e => {
+                                    const t = o().createElement(o().Fragment, null, i.Dialog.awsCredentialsError.body.text.map(((e, t) => o().createElement("p", {
                                             key: t,
-                                            className: U
+                                            className: H
                                         }, ((e, t) => {
                                             const r = e.split("%");
                                             return o().createElement(o().Fragment, null, r.map((e => {
                                                 if (e.startsWith("{")) {
                                                     const [r, ...n] = e.replace("{", "").split("}"), a = t[r], l = n.join("");
-                                                    return a ? o().createElement(o().Fragment, null, o().createElement(L, {
+                                                    return a ? o().createElement(o().Fragment, null, o().createElement(D, {
                                                         key: r,
                                                         href: a.linkHref,
-                                                        target: z.External
+                                                        target: R.External
                                                     }, a.linkString), l) : o().createElement(o().Fragment, null, e)
                                                 }
                                                 return o().createElement(o().Fragment, null, e)
                                             })))
-                                        })(e, s.Dialog.awsCredentialsError.body.links))))),
-                                        r = new d.Dialog({
-                                            title: s.Dialog.awsCredentialsError.title,
+                                        })(e, i.Dialog.awsCredentialsError.body.links))))),
+                                        r = new m.Dialog({
+                                            title: i.Dialog.awsCredentialsError.title,
                                             body: t,
-                                            buttons: [d.Dialog.cancelButton(), d.Dialog.okButton({
-                                                label: s.Dialog.awsCredentialsError.buttons.enterKeysInTerminal
+                                            buttons: [m.Dialog.cancelButton(), m.Dialog.okButton({
+                                                label: i.Dialog.awsCredentialsError.buttons.enterKeysInTerminal
                                             })]
                                         });
-                                    (await r.launch()).button.label === s.Dialog.awsCredentialsError.buttons.enterKeysInTerminal && e.execute(c)
+                                    (await r.launch()).button.label === i.Dialog.awsCredentialsError.buttons.enterKeysInTerminal && e.execute(u)
                                 })(r), new Error(n.statusText)
                             }
                             return await n.json()
                         })().then((async e => {
                             _(!1), y(e)
                         })).catch((e => {
                             f(e.message)
                         })) : _(!1)
                     }), [a, b.model.inputFile]);
                     const [E, y] = (0, n.useState)({}), [S, _] = (0, n.useState)(!0);
                     return h ? o().createElement("div", {
-                        className: re
-                    }, h) : S ? null : a !== l.JobsView.CreateForm || (null == E ? void 0 : E.auto_detected_config) ? o().createElement(At.Z, {
-                        theme: Vt()
-                    }, o().createElement(p.StylesProvider, {
+                        className: te
+                    }, h) : S ? null : a !== l.JobsView.CreateForm || (null == E ? void 0 : E.auto_detected_config) ? o().createElement(Vt.Z, {
+                        theme: Ot()
+                    }, o().createElement(d.StylesProvider, {
                         injectFirst: !0
                     }, o().createElement(It, {
                         executionEnvironments: E,
                         requestClient: e,
                         contentsManager: t,
                         jobsView: a,
-                        errors: i,
-                        handleErrorsChange: m,
+                        errors: c,
+                        handleErrorsChange: g,
                         ...b
                     }))) : null
                 },
-                Rt = [{
+                Ft = [{
                     id: "@amzn/sagemaker-scheduler:scheduler",
                     autoStart: !1,
                     requires: [a.ISettingRegistry],
                     provides: l.Scheduler.IAdvancedOptions,
                     activate: (e, t) => r => {
                         const n = e.serviceManager.serverSettings,
                             a = e.serviceManager.contents;
-                        return o().createElement(Ge, {
+                        return o().createElement(Be, {
                             app: e
-                        }, o().createElement(Ft, {
+                        }, o().createElement(At, {
                             requestClient: n,
                             contentsManager: a,
                             settingRegistry: t,
                             commands: e.commands,
                             ...r
                         }))
                     }
-                }, {
-                    id: "@amzn/sagemaker-scheudler:scheduler-disabler",
-                    requires: [r(6753).ILabShell],
-                    autoStart: !0,
-                    activate: (e, t) => {
-                        (async () => {
-                            await e.started, await t.restored;
-                            const r = g.ServerConnection.makeSettings(),
-                                n = v.URLExt.join(r.baseUrl, "/sagemaker_feature_enabled");
-                            let o = Date.now();
-                            const a = await g.ServerConnection.makeRequest(n, {
-                                method: "POST",
-                                body: JSON.stringify({
-                                    feature_name: i
-                                })
-                            }, r);
-                            let l = !1;
-                            try {
-                                const e = await a.json();
-                                e.currentTime && (o = parseInt(e.currentTime)), 200 === a.status && !0 === e.feature_found && !1 === e.feature_enabled && (l = !0)
-                            } catch (e) {}
-                            const s = (() => {
-                                    const e = (document.cookie || "").split(";");
-                                    for (let t = 0; t < e.length; t++) {
-                                        const r = e[t].split("=");
-                                        if ("enabledFeatureFlags" === r[0].trim()) return JSON.parse(decodeURIComponent(r[1]))
-                                    }
-                                    return null
-                                })(),
-                                u = !!s && s.indexOf(i) >= 0;
-                            (o < 1669824e6 || l) && !u && (document.styleSheets[0].insertRule('li[data-command="scheduling:create-from-filebrowser"] { display: none !important; }'), document.styleSheets[0].insertRule('\n          button[title="Create a notebook job"] { display: none !important; }\n        '), document.styleSheets[0].insertRule('\n          div[class="jp-LauncherCard"][title="Notebook Jobs"] { display: none !important; }\n        '))
-                        })()
-                    }
                 }]
         }
     }
 ]);
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.299f9d522c52a504280b.js` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.3b333e0e590d8edb68a6.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, u, l, f, d, s, c, p, h, b, m, v, g = {
-            3194: (e, r, t) => {
+    var e, r, t, a, n, o, i, u, l, f, s, d, c, p, h, b, m, v, g = {
+            3486: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(349), t.e(509), t.e(86), t.e(271), t.e(456), t.e(993)]).then((() => () => t(7993))),
-                        "./extension": () => Promise.all([t.e(349), t.e(509), t.e(86), t.e(271), t.e(456), t.e(993)]).then((() => () => t(7993)))
+                        "./index": () => Promise.all([t.e(349), t.e(509), t.e(86), t.e(271), t.e(456), t.e(315)]).then((() => () => t(8315))),
+                        "./extension": () => Promise.all([t.e(349), t.e(509), t.e(86), t.e(271), t.e(456), t.e(315)]).then((() => () => t(8315)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
                             var a = "default",
@@ -46,62 +46,62 @@
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
         86: "99a29e600153377570fa",
         144: "9be27e93647ef0e84863",
         193: "04adf0a714b67e82f263",
         240: "762850093662386d80d3",
         271: "a546aebb6445a3b38e60",
+        315: "59fba34ec08e26375d68",
         349: "eb375dbeb301592df698",
         456: "f9df645a48dde143e1a9",
         509: "b1db44e3c8c1ddb64444",
         615: "d5639a877b54ff655d41",
-        915: "83ac080d036e9c56d7e0",
-        993: "84c00bb76b4448d8ce3f"
+        915: "83ac080d036e9c56d7e0"
     } [e] + ".js?v=" + {
         86: "99a29e600153377570fa",
         144: "9be27e93647ef0e84863",
         193: "04adf0a714b67e82f263",
         240: "762850093662386d80d3",
         271: "a546aebb6445a3b38e60",
+        315: "59fba34ec08e26375d68",
         349: "eb375dbeb301592df698",
         456: "f9df645a48dde143e1a9",
         509: "b1db44e3c8c1ddb64444",
         615: "d5639a877b54ff655d41",
-        915: "83ac080d036e9c56d7e0",
-        993: "84c00bb76b4448d8ce3f"
+        915: "83ac080d036e9c56d7e0"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amzn/sagemaker-jupyter-scheduler:", w.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var i, u;
             if (void 0 !== n)
                 for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var d = l[f];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
-                        i = d;
+                    var s = l[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
-            var s = (r, a) => {
+            var d = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                c = setTimeout(s.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -123,15 +123,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (u("@amzn/sagemaker-jupyter-scheduler", "2.1.0", (() => Promise.all([w.e(349), w.e(509), w.e(86), w.e(271), w.e(456), w.e(993)]).then((() => () => w(7993))))), u("@emotion/css", "11.10.5", (() => Promise.all([w.e(509), w.e(615)]).then((() => () => w(4615))))), u("@material-ui/core", "4.12.4", (() => Promise.all([w.e(193), w.e(349), w.e(271), w.e(456)]).then((() => () => w(3193))))), u("react-router-dom", "5.3.4", (() => Promise.all([w.e(240), w.e(271), w.e(915)]).then((() => () => w(7240)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@amzn/sagemaker-jupyter-scheduler", "2.2.0", (() => Promise.all([w.e(349), w.e(509), w.e(86), w.e(271), w.e(456), w.e(315)]).then((() => () => w(8315))))), u("@emotion/css", "11.10.5", (() => Promise.all([w.e(509), w.e(615)]).then((() => () => w(4615))))), u("@material-ui/core", "4.12.4", (() => Promise.all([w.e(193), w.e(349), w.e(271), w.e(456)]).then((() => () => w(3193))))), u("react-router-dom", "5.3.4", (() => Promise.all([w.e(240), w.e(271), w.e(915)]).then((() => () => w(7240)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -180,33 +180,33 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > a && !n : "" == s != n);
-                if ("u" == d) {
-                    if (!l || "u" != s) return !1
+                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > a && !n : "" == d != n);
+                if ("u" == s) {
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (s == d)
+                    if (d == s)
                         if (u <= a) {
                             if (f != e[u]) return !1
                         } else {
                             if (n ? f > e[u] : f < e[u]) return !1;
                             f != e[u] && (l = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != d && "n" != d) {
                     if (n || u <= a) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= a || d < s != n) return !1;
+                    if (u <= a || s < d != n) return !1;
                     l = !1
-                } else "s" != s && "n" != s && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
@@ -217,41 +217,40 @@
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
         var n = u(e, t);
-        return o(a, n) || "undefined" != typeof console && console.warn && console.warn(l(e, t, n, a)), s(e[t][n])
-    }, d = (e, r, t) => {
+        return o(a, n) || "undefined" != typeof console && console.warn && console.warn(l(e, t, n, a)), d(e[t][n])
+    }, s = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
-    }, s = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, a, n) {
+    }, d = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, a, n) {
         var o = w.I(r);
         return o && o.then ? o.then(e.bind(e, r, w.S[r], t, a, n)) : e(r, w.S[r], t, a, n)
     })(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), h = c(((e, r, t, a, n) => {
-        var o = r && w.o(r, t) && d(r, t, a);
-        return o ? s(o) : n()
+        var o = r && w.o(r, t) && s(r, t, a);
+        return o ? d(o) : n()
     })), b = {}, m = {
         6271: () => p("default", "react", [1, 17, 0, 1]),
         4456: () => p("default", "react-dom", [1, 17, 0, 1]),
         78: () => h("default", "react-router-dom", [1, 5, 3, 4], (() => w.e(240).then((() => () => w(7240))))),
         1396: () => p("default", "@jupyterlab/coreutils", [1, 5, 1, 11]),
         1982: () => h("default", "@emotion/css", [1, 11, 10, 5], (() => w.e(144).then((() => () => w(4615))))),
         5015: () => p("default", "@jupyterlab/scheduler", [4, 0, 6, 1]),
         5185: () => p("default", "@jupyterlab/apputils", [1, 3, 1, 11]),
         5306: () => h("default", "@material-ui/core", [1, 4, 12, 4], (() => w.e(193).then((() => () => w(3193))))),
         6247: () => p("default", "@jupyterlab/services", [1, 6, 1, 11]),
-        6753: () => p("default", "@jupyterlab/application", [1, 3, 1, 11]),
         7363: () => p("default", "@jupyterlab/settingregistry", [1, 3, 1, 11]),
         9850: () => p("default", "@lumino/algorithm", [1, 1, 3, 3])
     }, v = {
         271: [6271],
-        456: [4456],
-        993: [78, 1396, 1982, 5015, 5185, 5306, 6247, 6753, 7363, 9850]
+        315: [78, 1396, 1982, 5015, 5185, 5306, 6247, 7363, 9850],
+        456: [4456]
     }, w.f.consumes = (e, r) => {
         w.o(v, e) && v[e].forEach((e => {
             if (w.o(b, e)) return r.push(b[e]);
             var t = r => {
                     b[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
@@ -299,10 +298,10 @@
                     u && u(w)
                 }
                 for (r && r(t); l < o.length; l++) n = o[l], w.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyter_scheduler = self.webpackChunk_amzn_sagemaker_jupyter_scheduler || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var j = w(3194);
+    var j = w(3486);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyter-scheduler"] = j
 })();
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/logging.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/logging.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/model_converter.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/model_converter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/models.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/models.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/revenue.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/providers/revenue.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/tags.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/providers/tags.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/scheduler.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,19 +295,14 @@
 @patch("builtins.open", new_callable=mock_open, read_data=MOCK_RESOURCE_METADATA)
 @patch.object(EC2AsyncBotoClient, "list_subnets_by_vpc_id")
 @patch.object(EC2AsyncBotoClient, "list_routetable_by_vpc_id")
 @patch.object(Session, "get_scoped_config")
 @patch.object(Session, "get_partition_for_region")
 @patch.object(STSAsyncBotoClient, "get_caller_identity")
 @patch.object(IAMAsyncBotoClient, "list_role_arns_with_matching_prefix")
-@patch.dict(
-    os.environ,
-    {"AWS_ACCOUNT_ID": TEST_ACCOUNT_ID, "AWS_DEFAULT_REGION": TEST_DEFAULT_REGION},
-    clear=True,
-)
 class TestAdvancedEnvironments:
     @pytest.mark.asyncio
     async def test_auto_detect_happy_path(
         self,
         mock_list_role_arns_with_matching_prefix,
         mock_get_caller_identity,
         mock_get_partition_for_region,
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,23 +7,32 @@
 from amazon_sagemaker_jupyter_scheduler.clients import STSAsyncBotoClient
 
 
 TEST_AWS_ACCOUNT_ID_STUDIO = "898989898989"
 
 
 @pytest.mark.asyncio
-@patch.dict(os.environ, {"AWS_ACCOUNT_ID": TEST_AWS_ACCOUNT_ID_STUDIO}, clear=True)
 async def test_async_cache_studio_base():
-    get_aws_account_id.cache_clear()
-    assert await get_aws_account_id() == TEST_AWS_ACCOUNT_ID_STUDIO
+    # Remember old value
+    old_aws_account_id = os.getenv("AWS_ACCOUNT_ID")
+    # Update environment
+    os.environ["AWS_ACCOUNT_ID"] = TEST_AWS_ACCOUNT_ID_STUDIO
+    try:
+        get_aws_account_id.cache_clear()
+        assert await get_aws_account_id() == TEST_AWS_ACCOUNT_ID_STUDIO
+    finally:
+        # Revert environment back to original state after test
+        if old_aws_account_id is None:
+            del os.environ["AWS_ACCOUNT_ID"]
+        else:
+            os.environ["AWS_ACCOUNT_ID"] = old_aws_account_id
 
 
 @pytest.mark.asyncio
 @patch.object(STSAsyncBotoClient, "get_caller_identity")
-@patch.dict(os.environ, {}, clear=True)
 async def test_async_cache_standalone_multiple_call(mock_sts_identity):
     TEST_ACCOUNT_ID_STANDALONE = 888888888888
     get_aws_account_id.cache_clear()
     mock_sts_identity.return_value = {"Account": TEST_ACCOUNT_ID_STANDALONE}
     assert await get_aws_account_id() == TEST_ACCOUNT_ID_STANDALONE
 
     # future calls should return from cache and not call aws account
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/utils.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-sagemaker-jupyter-scheduler
-Version: 2.1.0
+Version: 2.2.0
 Summary: Amazon SageMaker Jupyter Scheduler based on the https://pypi.org/project/jupyter-scheduler/
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,Scheduling Notebooks,Notebooks,Amazon Sagemaker
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt` & `amazon_sagemaker_jupyter_scheduler-2.2.0/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,24 +56,24 @@
 amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json
 amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig
 amazon_sagemaker_jupyter_scheduler/labextension/static/144.9be27e93647ef0e84863.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js.LICENSE.txt
 amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js.LICENSE.txt
+amazon_sagemaker_jupyter_scheduler/labextension/static/315.59fba34ec08e26375d68.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js.LICENSE.txt
 amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt
 amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js.LICENSE.txt
-amazon_sagemaker_jupyter_scheduler/labextension/static/993.84c00bb76b4448d8ce3f.js
-amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.299f9d522c52a504280b.js
+amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.3b333e0e590d8edb68a6.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/style.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json
 amazon_sagemaker_jupyter_scheduler/providers/__init__.py
 amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py
 amazon_sagemaker_jupyter_scheduler/providers/revenue.py
 amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py
 amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py
@@ -128,15 +128,14 @@
 src/components/tooltip/Tooltip.tsx
 src/components/tooltip/index.ts
 src/components/tooltip/styles.ts
 src/components/tooltip/__tests__/Tooltip.spec.tsx
 src/constants/common.ts
 src/constants/index.ts
 src/constants/kernels.ts
-src/plugins/ScheduleNotebookDisablerPlugin.tsx
 src/plugins/ScheduleNotebookPlugin.tsx
 src/plugins/index.ts
 src/types/images.ts
 src/types/index.ts
 src/types/kernels.ts
 src/types/sagemaker.ts
 src/utils/PluginEnvironmentProvider.tsx
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/jest.config.base.js` & `amazon_sagemaker_jupyter_scheduler-2.2.0/jest.config.base.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/package-lock.json` & `amazon_sagemaker_jupyter_scheduler-2.2.0/package-lock.json`

 * *Files identical despite different names*

#### Pretty-printed

 * *Similarity: 0.916663640764948%*

 * *Differences: {"'packages'": "{'': {'version': '2.2.0'}}", "'version'": "'2.2.0'"}*

```diff
@@ -11856,15 +11856,15 @@
                 "jest": "^27.2.4",
                 "npm-run-all": "^4.1.5",
                 "ts-jest": "^27.0.5",
                 "typescript": "^4.9.5"
             },
             "license": "Apache 2.0",
             "name": "@amzn/sagemaker-jupyter-scheduler",
-            "version": "2.1.0"
+            "version": "2.2.0"
         },
         "node_modules/@adobe/css-tools": {
             "dev": true,
             "integrity": "sha512-E09FiIft46CmH5Qnjb0wsW54/YQd69LsxeKUOWawmws1XWvyFGURnAChH0mlr7YPFR1ofwvUQfcL0J3lMxXqPA==",
             "license": "MIT",
             "version": "4.2.0"
         },
@@ -29020,9 +29020,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "license": "MIT",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "2.1.0"
+    "version": "2.2.0"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/package.json` & `amazon_sagemaker_jupyter_scheduler-2.2.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'2.2.0'"}*

```diff
@@ -106,9 +106,9 @@
         "test": "jest",
         "test:debug": "node --inspect node_modules/.bin/jest --watch --runInBand",
         "test:server-extension": ":",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "2.1.0"
+    "version": "2.2.0"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/setup.py` & `amazon_sagemaker_jupyter_scheduler-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/CreateNotebookJobForm.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/__tests__/CreateNotebookJobForm.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/VpcCheckbox.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/__tests__/VpcCheckbox.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/initalValueHelpers.spec.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/__tests__/initalValueHelpers.spec.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/validationHelpers.spec.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/__tests__/validationHelpers.spec.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/Link.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/link/Link.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/RouterLink.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/link/RouterLink.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/__test__/Link.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/link/__test__/Link.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/__test__/RouterLink.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/link/__test__/RouterLink.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/selectinput/SelectInput.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/selectinput/SelectInput.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/selectinput/types.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/selectinput/types.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/TextInput.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/textinput/TextInput.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/__tests__/TextInput.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/textinput/__tests__/TextInput.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/textinput/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/Tooltip.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/tooltip/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/__tests__/Tooltip.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/tooltip/__tests__/Tooltip.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/components/tooltip/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/constants/common.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/constants/common.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 const pluginIds = {
-  SchedulerPlugin: '@amzn/sagemaker-scheduler:scheduler',
-  SchedulerDisablerPlugin: '@amzn/sagemaker-scheudler:scheduler-disabler',
+  SchedulerPlugin: '@amzn/sagemaker-scheduler:scheduler'
 };
 
 const featureNames = {
   scheduler: 'nbScheduler',
 };
 
 const i18nStrings = {
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/plugins/ScheduleNotebookPlugin.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/plugins/ScheduleNotebookPlugin.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/themeProvider.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/themeProvider.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/PluginEnvironmentProvider.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/utils/PluginEnvironmentProvider.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/images.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/utils/images.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/kernels.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/utils/kernels.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/rendering.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/utils/rendering.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJob.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJob.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/InputContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/InputContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/CreateNotebookJobForm/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/mockResponses.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/mockResponses.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.2.0/src/widgets/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.1.0/tsconfig.base.json` & `amazon_sagemaker_jupyter_scheduler-2.2.0/tsconfig.base.json`

 * *Files identical despite different names*

