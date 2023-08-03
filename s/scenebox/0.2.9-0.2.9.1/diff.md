# Comparing `tmp/scenebox-0.2.9.tar.gz` & `tmp/scenebox-0.2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scenebox-0.2.9.tar", last modified: Sat Jun  4 00:58:17 2022, max compression
+gzip compressed data, was "dist/scenebox-0.2.9.1.tar", last modified: Fri Jun 10 01:22:51 2022, max compression
```

## Comparing `scenebox-0.2.9.tar` & `scenebox-0.2.9.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:17.000000 scenebox-0.2.9/
-drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:17.000000 scenebox-0.2.9/scenebox/
--rw-rw-r--   0 yaser     (1000) yaser     (1000)      492 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/__init__.py
-drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:17.000000 scenebox-0.2.9/scenebox/clients/
--rw-rw-r--   0 yaser     (1000) yaser     (1000)      219 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/clients/__init__.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)    20810 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/clients/job_manager_client.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)   266640 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/clients/scene_engine_client.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)    91011 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/clients/asset_manager_client.py
-drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:17.000000 scenebox-0.2.9/scenebox/models/
--rw-rw-r--   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/__init__.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)    13036 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/assets.py
-drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:17.000000 scenebox-0.2.9/scenebox/models/annotation_transformers/
--rw-rw-r--   0 yaser     (1000) yaser     (1000)       67 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/annotation_transformers/__init__.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)     4883 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/annotation_transformers/coco.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)    14579 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/annotation_transformers/scale.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)     5136 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/annotation_transformers/deepen.py
-drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:17.000000 scenebox-0.2.9/scenebox/models/annotation_transformers/tests/
--rw-rw-r--   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/annotation_transformers/tests/__init__.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)    11985 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/annotation_transformers/tests/test_annotations.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)    11851 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/annotation_transformers/tests/test_scale_annotation.py
-drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:17.000000 scenebox-0.2.9/scenebox/models/annotation_transformers/tests/resources/
--rw-rw-r--   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/annotation_transformers/tests/resources/__init__.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)    11915 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/annotation_transformers/tests/resources/deepen_file_labels.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)     1860 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/udf.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)    46631 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/annotation.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)     2409 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/object_access.py
-drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:17.000000 scenebox-0.2.9/scenebox/models/tests/
--rw-rw-r--   0 yaser     (1000) yaser     (1000)     1184 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/tests/test_object_access.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)       67 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/tests/__init__.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)    14582 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/tests/test_annotations.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)      892 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/models/tests/test_assets.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)    17977 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/constants.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)        5 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/BASE_VERSION
--rw-rw-r--   0 yaser     (1000) yaser     (1000)     2157 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/custom_exceptions.py
-drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:17.000000 scenebox-0.2.9/scenebox/tools/
--rw-rw-r--   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/__init__.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)     6525 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/time_utils.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)      612 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/sampling.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)      610 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/connections.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)     1093 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/video_utils.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)     1860 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/logger.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)     3954 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/image_utils.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)     3711 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/naming.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)     1220 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/asset_utils.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)    10298 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/misc.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)      411 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/threading_utils.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)    18395 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/asset_uploader.py
-drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:17.000000 scenebox-0.2.9/scenebox/tools/tests/
--rw-rw-r--   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/tests/__init__.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)      894 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/tests/test_image_utils.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)      719 2022-06-04 00:58:15.000000 scenebox-0.2.9/scenebox/tools/tests/test_threading_utils.py
--rw-rw-r--   0 yaser     (1000) yaser     (1000)     1121 2021-12-27 01:48:40.000000 scenebox-0.2.9/setup.py
-drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-04 00:58:17.000000 scenebox-0.2.9/scenebox.egg-info/
--rw-rw-r--   0 yaser     (1000) yaser     (1000)     1720 2022-06-04 00:58:16.000000 scenebox-0.2.9/scenebox.egg-info/SOURCES.txt
--rw-rw-r--   0 yaser     (1000) yaser     (1000)      210 2022-06-04 00:58:16.000000 scenebox-0.2.9/scenebox.egg-info/requires.txt
--rw-rw-r--   0 yaser     (1000) yaser     (1000)      755 2022-06-04 00:58:16.000000 scenebox-0.2.9/scenebox.egg-info/PKG-INFO
--rw-rw-r--   0 yaser     (1000) yaser     (1000)        9 2022-06-04 00:58:16.000000 scenebox-0.2.9/scenebox.egg-info/top_level.txt
--rw-rw-r--   0 yaser     (1000) yaser     (1000)        1 2022-06-04 00:58:16.000000 scenebox-0.2.9/scenebox.egg-info/dependency_links.txt
--rw-rw-r--   0 yaser     (1000) yaser     (1000)       38 2022-06-04 00:58:17.000000 scenebox-0.2.9/setup.cfg
--rw-rw-r--   0 yaser     (1000) yaser     (1000)      755 2022-06-04 00:58:17.000000 scenebox-0.2.9/PKG-INFO
--rw-rw-r--   0 yaser     (1000) yaser     (1000)      329 2021-09-03 01:58:14.000000 scenebox-0.2.9/README.md
+drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/
+drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox/
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)      492 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/__init__.py
+drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox/clients/
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)      219 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/clients/__init__.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)    20810 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/clients/job_manager_client.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)   267971 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/clients/scene_engine_client.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)    90999 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/clients/asset_manager_client.py
+drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox/models/
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/__init__.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)    13036 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/assets.py
+drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox/models/annotation_transformers/
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)       67 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/annotation_transformers/__init__.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)     4883 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/annotation_transformers/coco.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)    14579 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/annotation_transformers/scale.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)     5136 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/annotation_transformers/deepen.py
+drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox/models/annotation_transformers/tests/
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/annotation_transformers/tests/__init__.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)    11985 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/annotation_transformers/tests/test_annotations.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)    11851 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/annotation_transformers/tests/test_scale_annotation.py
+drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox/models/annotation_transformers/tests/resources/
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/annotation_transformers/tests/resources/__init__.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)    11915 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/annotation_transformers/tests/resources/deepen_file_labels.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)     1860 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/udf.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)    46641 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/annotation.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)     2409 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/object_access.py
+drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox/models/tests/
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)     1184 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/tests/test_object_access.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)       67 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/tests/__init__.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)    14582 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/tests/test_annotations.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)      892 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/models/tests/test_assets.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)    17977 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/constants.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)        7 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/BASE_VERSION
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)     2157 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/custom_exceptions.py
+drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox/tools/
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/__init__.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)     6525 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/time_utils.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)      612 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/sampling.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)      610 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/connections.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)     1093 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/video_utils.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)     1860 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/logger.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)     3954 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/image_utils.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)     3703 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/naming.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)     1220 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/asset_utils.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)    10397 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/misc.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)      411 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/threading_utils.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)    18465 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/asset_uploader.py
+drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox/tools/tests/
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/tests/__init__.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)      894 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/tests/test_image_utils.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)      719 2022-06-10 01:22:50.000000 scenebox-0.2.9.1/scenebox/tools/tests/test_threading_utils.py
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)     1121 2021-12-27 01:48:40.000000 scenebox-0.2.9.1/setup.py
+drwxrwxr-x   0 yaser     (1000) yaser     (1000)        0 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox.egg-info/
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)     1720 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox.egg-info/SOURCES.txt
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)      210 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox.egg-info/requires.txt
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)      757 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox.egg-info/PKG-INFO
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)        9 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox.egg-info/top_level.txt
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)        1 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/scenebox.egg-info/dependency_links.txt
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)       38 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/setup.cfg
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)      757 2022-06-10 01:22:51.000000 scenebox-0.2.9.1/PKG-INFO
+-rw-rw-r--   0 yaser     (1000) yaser     (1000)      329 2021-09-03 01:58:14.000000 scenebox-0.2.9.1/README.md
```

### Comparing `scenebox-0.2.9/scenebox/clients/job_manager_client.py` & `scenebox-0.2.9.1/scenebox/clients/job_manager_client.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/clients/scene_engine_client.py` & `scenebox-0.2.9.1/scenebox/clients/scene_engine_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -767,14 +767,15 @@
 
         Parameters
         ----------
         name:
             The name to give to the set.
         asset_type:
             The type of assets for the set to contain. e.g. images, videos, LIDARs, etc.
+            To ensure using a valid asset_type, you can import AssetsConstants from scenebox.constants
         origin_set_id:
             Id of the set, the new set is created from. Useful when creating a set by deriving its assets
             from other sets.
         expected_count:
             Estimated count of the number of assets this set is expected to contain.
         tags:
             Labels associated with the set.  Allows for easy set search.
@@ -1821,15 +1822,15 @@
         Set the asset_manager state to access particular assets. This is often used in chaining:
         Eg. client.with_asset_state("images", True).search_files({})
 
         Parameters
         ----------
         asset_type:
             Desired AssetManagerClient asset type.
-
+            To ensure using a valid asset_type, you can import AssetsConstants from scenebox.constants
         Returns
         -------
         AssetManagerClient
             The AssetManagerClient associated with the specified asset.
 
         """
         key = asset_type + (self.auth_token or "")
@@ -1921,15 +1922,15 @@
     def get_searchable_field_statistics(self, asset_type: str) -> dict:
         """Get the metadata searchable field statistics for a certain asset type.
 
         Parameters
         ----------
         asset_type:
             The asset type to receive the searchable field statistics of.
-
+            To ensure using a valid asset_type, you can import AssetsConstants from scenebox.constants
         Returns
         -------
         dict
             Dictionary with keys of the searchable statistics, and values of the
             min/max/count/defaults for that statistic.
 
         """
@@ -1949,14 +1950,15 @@
 
         Parameters
         ----------
         id:
             The ID of the asset to get metadata from.
         asset_type:
             The asset type of the asset to get metadata from.
+            To ensure using a valid asset_type, you can import AssetsConstants from scenebox.constants
         with_session_metadata:
             If True and the asset belongs to a session, also return session entities
 
         Returns
         -------
         dict
             The asset metadata.
@@ -2226,14 +2228,15 @@
                                        asset_ids: List[str],
                                        asset_type: str):
         """Cleanup annotation lists by removing repeated entries in an asset's metadata.
         asset_ids:
             List of asset ids to clean-up.
         asset_type:
             The type of asset.
+            To ensure using a valid asset_type, you can import AssetsConstants from scenebox.constants
         """
         asset_ids_chunked = chunk_list(asset_ids, chunk_size=10000)
         asset_amc = self.get_asset_manager(asset_type=asset_type)
 
         def perform_cleanup(asset_ids_chunk):
             asset_metadata = asset_amc.get_metadata_in_batch(ids=asset_ids_chunk)
 
@@ -2742,14 +2745,15 @@
         ----------
         annotation_sources:
             A list of dictionaries. Each dictionary defines an annotation source with the mandatory
             field: `provider` and optional fields: `version`, `annotation_type`, `annotation_group`.
             Can be collected from the `get_annotation_sources` method.
         asset_type:
             Asset media type for annotations provided by all annotation_sources.
+            To ensure using a valid asset_type, you can import AssetsConstants from scenebox.constants
         asset_filters:
             Query to locate the data subset of interest.  Filters through existing
             assets according to the dictionary passed.
         wait_for_completion:
             If True, polls until job is complete.
             Otherwise, continues execution and does not raise an error if the job does not complete.
             Default is True.
@@ -3885,14 +3889,15 @@
         Returns the top ``size`` matching hits.  If a return of more than 10000 hits is desired, please use
         AssetManagerClient.search_assets_large().
 
         Parameters
         ----------
         asset_type:
             Asset type to filter for in the asset search.
+            To ensure using a valid asset_type, you can import AssetsConstants from scenebox.constants
         search:
             Query to locate the data subset of interest.  Filters through existing
             assets according to the dictionary passed.
         size:
             Specifies the Elasticsearch search size.  The maximum number of hits to return.
             Has no effect if ``scan`` is False.
         offset:
@@ -3945,14 +3950,15 @@
         Returns the top ``size`` matching hits.  If a return of more than 10000 hits is desired, please use
         AssetManagerClient.search_meta_large().
 
         Parameters
         ----------
         asset_type:
             Asset type to filter for in the asset metadata search.
+            To ensure using a valid asset_type, you can import AssetsConstants from scenebox.constants
         query:
             Query to locate the data subset of interest.  Filters through existing
             assets according to the dictionary passed.
         size:
             Specifies the Elasticsearch search size.  The maximum number of hits to return.
             Has no effect if ``scan`` is False.
         offset:
@@ -4001,14 +4007,15 @@
             summary_request: Dict) -> Dict:
         """Retrieve summary of asset metadata with a search query.
 
         Parameters
         ----------
         asset_type:
             Asset type to collect metadata summary for.
+            To ensure using a valid asset_type, you can import AssetsConstants from scenebox.constants
         summary_request:
             Includes:
                 - search: (Dict) to locate the data subset of interest.
                 - dimensions: (List[str]) to collect statistical summary of the desired dimensions
                 - nested_dimensions: (List[str]) to collect statistical summary of the desired nested dimensions
             Example:
                 {
@@ -5834,14 +5841,15 @@
         Extracts inferences such as masks, bounding boxes, objects, and/or embeddings on an asset of choice using a
         model of choice.  Select from Mask RCNN, StarDist, or Image Intensity Histogram.
 
         Parameters
         ----------
         asset_type:
             The type of assets to perform model inference on.
+            To ensure using a valid asset_type, you can import AssetsConstants from scenebox.constants
         ids:
             IDs of the previously uploaded assets on which to perform a model inference.
         search:
             Query to locate the data subset of interest.  Filters through existing
             assets according to the dictionary passed.
         model:
             The model to perform the inference with.  Select from Mask RCNN ('mrcnn'), StarDist ('stardist'), or Image
@@ -5921,15 +5929,16 @@
 
         Enrich image or object assets with classical image properties/features such as brightness or contrast
         and add this as auxiliary metadata for the asset.
 
         Parameters
         ----------
         asset_type:
-            The type of assets to perform model inference on.
+            The type of assets to perform enrichment on.
+            To ensure using a valid asset_type, you can import AssetsConstants from scenebox.constants
         ids:
             IDs of the previously uploaded assets on which to perform a model inference.
         search:
             Query to locate the data subset of interest.  Filters through existing
             assets according to the dictionary passed.
         properties:
             A list of strings for each property to be added to the metadata of the asset.
@@ -6423,14 +6432,15 @@
 
         .. note:: Embeddings must be indexed before this function can be used.
 
         Parameters
         ----------
         asset_type:
             The type of asset to apply UMAP on.
+            To ensure using a valid asset_type, you can import AssetsConstants from scenebox.constants
         index_name:
             index_name of the embeddings.  Used to filter through the embeddings metadata.
         search_dic:
             Query to locate the data subset of interest.  Filters through existing
             assets according to the dictionary passed.
         n_neighbors:
             Controls how UMAP balances local vs. global structure in data.  Low values of ``n_neighbours`` forces UMAP
@@ -6491,14 +6501,15 @@
        ----------
        id:
            asset id.
        similar_asset_count:
            count of similar assets (10 by default)
        asset_type:
            type of assets (Images by default)
+           To ensure using a valid asset_type, you can import AssetsConstants from scenebox.constants
        embedding_space:
            embedding space in which similarity is performed on. Ineffective/optional if there is only one embedding
            space
 
        Returns
        -------
        list
```

### Comparing `scenebox-0.2.9/scenebox/clients/asset_manager_client.py` & `scenebox-0.2.9.1/scenebox/clients/asset_manager_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2007,28 +2007,28 @@
         params = self.add_asset_manager_params()
         resp = requests.post(
             url,
             json=summary_2d_request,
             params=params)
         if not resp.ok:
             raise AssetError(
-                'Could not get the confusion matrix for ::: {} -- {} -- {}'.format(
+                'Could not get the 2d summary for ::: {} -- {} -- {}'.format(
                     summary_2d_request, resp.reason, resp.content))
         return resp.json()
 
     def summary_nd(self, summary_nd_request: dict):
         url = self.get_assets_url('summary_nd/')
         params = self.add_asset_manager_params()
         resp = requests.post(
             url,
             json=summary_nd_request,
             params=params)
         if not resp.ok:
             raise AssetError(
-                'Could not get the confusion matrix for ::: {} -- {} -- {}'.format(
+                'Could not get the nd summary for ::: {} -- {} -- {}'.format(
                     summary_nd_request, resp.reason, resp.content))
         return resp.json()
 
     def api_status(self):
         url = self.get_assets_url('status/')
         params = self.add_asset_manager_params()
         resp = requests.get(url, params=params)
```

### Comparing `scenebox-0.2.9/scenebox/models/assets.py` & `scenebox-0.2.9.1/scenebox/models/assets.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/models/annotation_transformers/coco.py` & `scenebox-0.2.9.1/scenebox/models/annotation_transformers/coco.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/models/annotation_transformers/scale.py` & `scenebox-0.2.9.1/scenebox/models/annotation_transformers/scale.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/models/annotation_transformers/deepen.py` & `scenebox-0.2.9.1/scenebox/models/annotation_transformers/deepen.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/models/annotation_transformers/tests/test_annotations.py` & `scenebox-0.2.9.1/scenebox/models/annotation_transformers/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/models/annotation_transformers/tests/test_scale_annotation.py` & `scenebox-0.2.9.1/scenebox/models/annotation_transformers/tests/test_scale_annotation.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/models/annotation_transformers/tests/resources/deepen_file_labels.py` & `scenebox-0.2.9.1/scenebox/models/annotation_transformers/tests/resources/deepen_file_labels.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/models/udf.py` & `scenebox-0.2.9.1/scenebox/models/udf.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/models/annotation.py` & `scenebox-0.2.9.1/scenebox/models/annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,40 +365,40 @@
             tags: Optional[List[str]]
                 Any tags to associate with the annotation.
             frame: Optional[int]
                 Video frame number associated with the annotation.  Must be specified if annotating video.
             aux: Optional[List[str]]
                 Any auxiliary annotation metadata.
         """
-        self.id: str = standardize_name(kwargs.get("id", misc.get_guid()))
-        self.timestamp: datetime = kwargs.get("timestamp", datetime.utcnow())
+        self.id: str = standardize_name(kwargs.get("id") or misc.get_guid())
+        self.timestamp: datetime = kwargs.get("timestamp") or datetime.utcnow()
 
         self.asset_id: str = kwargs.get("asset_id") or kwargs.get("image_id") or \
                              kwargs.get("video_id") or kwargs.get("lidar_id")
         if not self.asset_id:
             raise InvalidAnnotationError("asset_id (image, video, lidar) should be specified")
 
         # assert_standardized(self.asset_id)  # remove in the future
         self.asset_id = standardize_name(self.asset_id)
 
-        self.media_type: str = kwargs.get("media_type", AssetsConstants.IMAGES_ASSET_ID)
+        self.media_type: str = kwargs.get("media_type") or AssetsConstants.IMAGES_ASSET_ID
         if self.media_type not in AnnotationMediaTypes.VALID_TYPES:
             raise InvalidAnnotationError(
                 "invalid annotation type {}".format(self.media_type)
             )
 
         self.annotation_type: str = kwargs.get("annotation_type")
         if self.annotation_type not in AnnotationTypes.VALID_TYPES:
             raise InvalidAnnotationError(
                 "invalid annotation type {}".format(self.annotation_type)
             )
 
         self.provider: Optional[str] = kwargs.get("provider") or AnnotationProviders.DEFAULT_PROVIDER
-        self.annotation_entities: List[AnnotationEntity] = kwargs.get("annotation_entities", [])
-        self.annotation_meta: Dict = kwargs.get("annotation_meta", {})
+        self.annotation_entities: List[AnnotationEntity] = kwargs.get("annotation_entities") or []
+        self.annotation_meta: Dict = kwargs.get("annotation_meta") or {}
         self.sets: List[str] = kwargs.get("sets", [])
         if "set_id" in kwargs:
             self.sets.append(kwargs.get("set_id"))
         self.session_uid: Optional[str] = kwargs.get("session_uid")
         self.sensor: Optional[str] = kwargs.get("sensor")
         self.version: Optional[str] = kwargs.get("version")
         self.annotation_group: str = kwargs.get("annotation_group", AnnotationGroups.GROUND_TRUTH)
```

### Comparing `scenebox-0.2.9/scenebox/models/object_access.py` & `scenebox-0.2.9.1/scenebox/models/object_access.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/models/tests/test_object_access.py` & `scenebox-0.2.9.1/scenebox/models/tests/test_object_access.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/models/tests/test_annotations.py` & `scenebox-0.2.9.1/scenebox/models/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/models/tests/test_assets.py` & `scenebox-0.2.9.1/scenebox/models/tests/test_assets.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/constants.py` & `scenebox-0.2.9.1/scenebox/constants.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/custom_exceptions.py` & `scenebox-0.2.9.1/scenebox/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/tools/time_utils.py` & `scenebox-0.2.9.1/scenebox/tools/time_utils.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/tools/sampling.py` & `scenebox-0.2.9.1/scenebox/tools/sampling.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/tools/connections.py` & `scenebox-0.2.9.1/scenebox/tools/connections.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/tools/video_utils.py` & `scenebox-0.2.9.1/scenebox/tools/video_utils.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/tools/logger.py` & `scenebox-0.2.9.1/scenebox/tools/logger.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/tools/image_utils.py` & `scenebox-0.2.9.1/scenebox/tools/image_utils.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/tools/naming.py` & `scenebox-0.2.9.1/scenebox/tools/naming.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 def standardize_name(
         name: str,
         replace_symbol: str = '_') -> str:
     if not name:
         raise ValueError(
-            'Session name must be provided, got: `{}`'.format(name))
+            'name must be provided, got: `{}`'.format(name))
 
     if name in standardized_name_cache:
         return standardized_name_cache[name]
     else:
         original_name = name
         for symbol in [",", "*", "\\", "<", "|", ">", "/", "?",
                        ' ', '{', '}', '$', '^', '%', '(', ')', ':', '+', '-']:
```

### Comparing `scenebox-0.2.9/scenebox/tools/asset_utils.py` & `scenebox-0.2.9.1/scenebox/tools/asset_utils.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/tools/misc.py` & `scenebox-0.2.9.1/scenebox/tools/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import platform
 import re
 import time
 import uuid
 import requests
 from concurrent.futures import ThreadPoolExecutor
 from functools import wraps
-from typing import Callable, Dict, Iterable, Optional
+from typing import Callable, Dict, Iterable, Optional, List
 from tqdm import tqdm as tqdm_base
 
 from ..custom_exceptions import ResponseError
 from ..constants import MAX_THREADS
 
 
 def decorate_all_inherited_methods(decorator):
@@ -146,14 +146,18 @@
     return get_md5_from_string(json.dumps(json_object, sort_keys=True))
 
 
 def deduplicate(input_list: list) -> list:
     return list(set(input_list))
 
 
+def flatten(t: List[List]) -> list:
+    return [item for sublist in t for item in sublist]
+
+
 def parse_file_path(input_str: str) \
         -> (str, str, str, str):
     cleaned_str = input_str.replace("\\", "/")
     filename = cleaned_str.split("/")[-1]
     extension = filename.split(".")[-1]
     filename_no_extension = filename.replace("." + extension, "")
     path = cleaned_str.replace(filename, "")
```

### Comparing `scenebox-0.2.9/scenebox/tools/asset_uploader.py` & `scenebox-0.2.9.1/scenebox/tools/asset_uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from .logger import get_logger
 from ..constants import AUXILIARY_KEY, EntityNames, EntityTypes, EntityInfluenceTypes, AssetsConstants
 from ..custom_exceptions import InvalidArgumentsError
 from ..models.assets import UnstructuredInputAsset, Lidar, Image, Video
 from ..models.object_access import ObjectAccess
 from ..tools.asset_utils import get_asset_attributes_filename
-from ..tools.misc import chunk_list, run_threaded, get_guid
+from ..tools.misc import chunk_list, run_threaded, get_guid, flatten
 from ..tools.time_utils import datetime_or_str_to_iso_utc, str_or_datetime_to_datetime
 
 
 logger = get_logger(__name__)
 
 
 class BulkAssetUploader(ABC):
@@ -253,16 +253,17 @@
 
             if add_to_session and asset_id_entity_map:
                 self.sec.add_entities(entity_dicts=list(asset_id_entity_map.values()))
 
             self.post_index_processing(ids=ids)
 
             if self.index_annotations and asset_id_annotations_map:
+                annotations_list = flatten(list(asset_id_annotations_map.values()))
                 self.sec.add_annotations(
-                    annotations=list(asset_id_annotations_map.values()),
+                    annotations=annotations_list,
                     update_asset=False,
                     threading=False,
                     disable_tqdm=True)
 
             chunk_id_added_asset_ids_map[chunk_id] = ids
 
         run_threaded(func=process_asset_chunk_add,
```

### Comparing `scenebox-0.2.9/scenebox/tools/tests/test_image_utils.py` & `scenebox-0.2.9.1/scenebox/tools/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox/tools/tests/test_threading_utils.py` & `scenebox-0.2.9.1/scenebox/tools/tests/test_threading_utils.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/setup.py` & `scenebox-0.2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox.egg-info/SOURCES.txt` & `scenebox-0.2.9.1/scenebox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scenebox-0.2.9/scenebox.egg-info/PKG-INFO` & `scenebox-0.2.9.1/scenebox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenebox
-Version: 0.2.9
+Version: 0.2.9.1
 Summary: Caliber Data Labs Clients package
 Home-page: UNKNOWN
 Author: Caliber Data labs
 Author-email: yaser@caliberdatalabs.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scenebox-0.2.9/PKG-INFO` & `scenebox-0.2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenebox
-Version: 0.2.9
+Version: 0.2.9.1
 Summary: Caliber Data Labs Clients package
 Home-page: UNKNOWN
 Author: Caliber Data labs
 Author-email: yaser@caliberdatalabs.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

