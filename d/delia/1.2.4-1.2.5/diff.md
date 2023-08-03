# Comparing `tmp/delia-1.2.4.tar.gz` & `tmp/delia-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delia-1.2.4.tar", last modified: Thu Aug  3 13:46:09 2023, max compression
+gzip compressed data, was "delia-1.2.5.tar", last modified: Thu Aug  3 15:09:10 2023, max compression
```

## Comparing `delia-1.2.4.tar` & `delia-1.2.5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.351452 delia-1.2.4/
--rw-rw-rw-   0        0        0    11549 2022-03-24 18:12:27.000000 delia-1.2.4/LICENSE
--rw-rw-rw-   0        0        0    15339 2023-08-03 13:46:09.350405 delia-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    14707 2023-06-20 15:23:09.000000 delia-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.251046 delia-1.2.4/delia/
--rw-rw-rw-   0        0        0      583 2023-08-03 13:45:17.000000 delia-1.2.4/delia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.256597 delia-1.2.4/delia/databases/
--rw-rw-rw-   0        0        0       49 2022-11-08 03:00:14.000000 delia-1.2.4/delia/databases/__init__.py
--rw-rw-rw-   0        0        0    13553 2023-07-12 22:13:37.000000 delia-1.2.4/delia/databases/patients_database.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.257602 delia-1.2.4/delia/extractors/
--rw-rw-rw-   0        0        0      187 2023-05-04 17:50:19.000000 delia-1.2.4/delia/extractors/__init__.py
--rw-rw-rw-   0        0        0    14538 2023-08-03 13:41:17.000000 delia-1.2.4/delia/extractors/patients_data_extractor.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.262036 delia-1.2.4/delia/radiomics/
--rw-rw-rw-   0        0        0      158 2023-05-04 17:50:19.000000 delia-1.2.4/delia/radiomics/__init__.py
--rw-rw-rw-   0        0        0    12188 2023-07-03 19:53:42.000000 delia-1.2.4/delia/radiomics/radiomics_dataset.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.263053 delia-1.2.4/delia/readers/
--rw-rw-rw-   0        0        0       65 2022-11-08 03:03:57.000000 delia-1.2.4/delia/readers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.266046 delia-1.2.4/delia/readers/image/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.4/delia/readers/image/__init__.py
--rw-rw-rw-   0        0        0    11258 2023-06-20 15:23:09.000000 delia-1.2.4/delia/readers/image/dicom_reader.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.273198 delia-1.2.4/delia/readers/patient_data/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.4/delia/readers/patient_data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.277198 delia-1.2.4/delia/readers/patient_data/factories/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.4/delia/readers/patient_data/factories/__init__.py
--rw-rw-rw-   0        0        0     5110 2023-06-20 15:23:09.000000 delia-1.2.4/delia/readers/patient_data/factories/base_patient_data_factory.py
--rw-rw-rw-   0        0        0     8102 2023-08-03 13:41:17.000000 delia-1.2.4/delia/readers/patient_data/factories/patient_data_factories.py
--rw-rw-rw-   0        0        0     3974 2023-06-20 15:23:09.000000 delia-1.2.4/delia/readers/patient_data/patient_data_query_context.py
--rw-rw-rw-   0        0        0      931 2023-08-03 13:41:17.000000 delia-1.2.4/delia/readers/patient_data/patient_data_query_strategy.py
--rw-rw-rw-   0        0        0    10030 2023-06-20 15:23:09.000000 delia-1.2.4/delia/readers/patient_data/patient_data_reader.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.285437 delia-1.2.4/delia/readers/segmentation/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.4/delia/readers/segmentation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.295377 delia-1.2.4/delia/readers/segmentation/factories/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.4/delia/readers/segmentation/factories/__init__.py
--rw-rw-rw-   0        0        0     2042 2022-11-08 03:20:33.000000 delia-1.2.4/delia/readers/segmentation/factories/base_segmentation_factory.py
--rw-rw-rw-   0        0        0     6278 2022-11-08 03:20:33.000000 delia-1.2.4/delia/readers/segmentation/factories/dicom_segmentation_factories.py
--rw-rw-rw-   0        0        0     1260 2022-07-27 14:35:42.000000 delia-1.2.4/delia/readers/segmentation/factories/segment.py
--rw-rw-rw-   0        0        0     2830 2022-02-08 18:32:16.000000 delia-1.2.4/delia/readers/segmentation/factories/segmentation.py
--rw-rw-rw-   0        0        0     4772 2023-05-05 16:07:22.000000 delia-1.2.4/delia/readers/segmentation/segmentation_context.py
--rw-rw-rw-   0        0        0     2801 2023-03-16 14:44:58.000000 delia-1.2.4/delia/readers/segmentation/segmentation_reader.py
--rw-rw-rw-   0        0        0     2217 2023-05-05 16:07:22.000000 delia-1.2.4/delia/readers/segmentation/segmentation_strategy.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.302329 delia-1.2.4/delia/transforms/
--rw-rw-rw-   0        0        0      120 2023-03-16 15:36:25.000000 delia-1.2.4/delia/transforms/__init__.py
--rw-rw-rw-   0        0        0    13141 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/applications.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.311428 delia-1.2.4/delia/transforms/array_space/
--rw-rw-rw-   0        0        0      293 2023-03-16 15:36:25.000000 delia-1.2.4/delia/transforms/array_space/__init__.py
--rw-rw-rw-   0        0        0     5085 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/array_space/matching_centroid_spatial_crop.py
--rw-rw-rw-   0        0        0     3096 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/array_space/matching_crop_foreground.py
--rw-rw-rw-   0        0        0     1043 2023-03-16 16:39:24.000000 delia-1.2.4/delia/transforms/array_space/tools.py
--rw-rw-rw-   0        0        0     2544 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/array_space/transform.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.318737 delia-1.2.4/delia/transforms/data/
--rw-rw-rw-   0        0        0      115 2023-03-16 15:36:25.000000 delia-1.2.4/delia/transforms/data/__init__.py
--rw-rw-rw-   0        0        0     4558 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/data/copy_segmentations.py
--rw-rw-rw-   0        0        0     1864 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/data/transform.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.328653 delia-1.2.4/delia/transforms/physical_space/
--rw-rw-rw-   0        0        0      269 2023-03-27 00:27:35.000000 delia-1.2.4/delia/transforms/physical_space/__init__.py
--rw-rw-rw-   0        0        0     3360 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/physical_space/matching_resample.py
--rw-rw-rw-   0        0        0     9808 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/physical_space/pet_to_suv.py
--rw-rw-rw-   0        0        0     3694 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/physical_space/resample.py
--rw-rw-rw-   0        0        0     2992 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/physical_space/transform.py
--rw-rw-rw-   0        0        0     2403 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/tools.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.338445 delia-1.2.4/delia/utils/
--rw-rw-rw-   0        0        0       42 2022-11-08 03:52:44.000000 delia-1.2.4/delia/utils/__init__.py
--rw-rw-rw-   0        0        0     4101 2023-03-16 14:44:58.000000 delia-1.2.4/delia/utils/data_model.py
--rw-rw-rw-   0        0        0     1329 2022-03-25 22:07:08.000000 delia-1.2.4/delia/utils/tools.py
--rw-rw-rw-   0        0        0     2131 2022-11-08 03:00:14.000000 delia-1.2.4/delia/utils/transforms_history.py
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.255356 delia-1.2.4/delia.egg-info/
--rw-rw-rw-   0        0        0    15339 2023-08-03 13:46:09.000000 delia-1.2.4/delia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2252 2023-08-03 13:46:09.000000 delia-1.2.4/delia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 13:46:09.000000 delia-1.2.4/delia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-08-03 13:46:09.000000 delia-1.2.4/delia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-08-03 13:46:09.000000 delia-1.2.4/delia.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.349277 delia-1.2.4/examples/
--rw-rw-rw-   0        0        0       38 2022-03-26 17:30:16.000000 delia-1.2.4/examples/__init__.py
--rw-rw-rw-   0        0        0      712 2022-03-29 17:53:18.000000 delia-1.2.4/examples/env_examples.py
--rw-rw-rw-   0        0        0     3474 2023-08-03 13:41:17.000000 delia-1.2.4/examples/ex01.py
--rw-rw-rw-   0        0        0     3119 2023-08-03 13:41:17.000000 delia-1.2.4/examples/ex02.py
--rw-rw-rw-   0        0        0     2760 2023-08-03 13:41:17.000000 delia-1.2.4/examples/ex03.py
--rw-rw-rw-   0        0        0     5382 2023-08-03 13:41:17.000000 delia-1.2.4/examples/ex04.py
--rw-rw-rw-   0        0        0      108 2022-01-10 21:30:41.000000 delia-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-03 13:46:09.351452 delia-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-08-03 13:45:17.000000 delia-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.781733 delia-1.2.5/
+-rw-rw-rw-   0        0        0    11549 2022-03-24 18:12:27.000000 delia-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0    15339 2023-08-03 15:09:10.781733 delia-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    14707 2023-06-20 15:23:09.000000 delia-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.718182 delia-1.2.5/delia/
+-rw-rw-rw-   0        0        0      583 2023-08-03 15:08:01.000000 delia-1.2.5/delia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.723411 delia-1.2.5/delia/databases/
+-rw-rw-rw-   0        0        0       49 2022-11-08 03:00:14.000000 delia-1.2.5/delia/databases/__init__.py
+-rw-rw-rw-   0        0        0    13553 2023-07-12 22:13:37.000000 delia-1.2.5/delia/databases/patients_database.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.726961 delia-1.2.5/delia/extractors/
+-rw-rw-rw-   0        0        0      187 2023-05-04 17:50:19.000000 delia-1.2.5/delia/extractors/__init__.py
+-rw-rw-rw-   0        0        0    15024 2023-08-03 15:01:33.000000 delia-1.2.5/delia/extractors/patients_data_extractor.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.727970 delia-1.2.5/delia/radiomics/
+-rw-rw-rw-   0        0        0      158 2023-05-04 17:50:19.000000 delia-1.2.5/delia/radiomics/__init__.py
+-rw-rw-rw-   0        0        0    12188 2023-07-03 19:53:42.000000 delia-1.2.5/delia/radiomics/radiomics_dataset.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.728967 delia-1.2.5/delia/readers/
+-rw-rw-rw-   0        0        0       65 2022-11-08 03:03:57.000000 delia-1.2.5/delia/readers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.731383 delia-1.2.5/delia/readers/image/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.5/delia/readers/image/__init__.py
+-rw-rw-rw-   0        0        0    11505 2023-08-03 14:57:28.000000 delia-1.2.5/delia/readers/image/dicom_reader.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.738492 delia-1.2.5/delia/readers/patient_data/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.5/delia/readers/patient_data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.743497 delia-1.2.5/delia/readers/patient_data/factories/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.5/delia/readers/patient_data/factories/__init__.py
+-rw-rw-rw-   0        0        0     5270 2023-08-03 14:57:28.000000 delia-1.2.5/delia/readers/patient_data/factories/base_patient_data_factory.py
+-rw-rw-rw-   0        0        0     8522 2023-08-03 14:58:43.000000 delia-1.2.5/delia/readers/patient_data/factories/patient_data_factories.py
+-rw-rw-rw-   0        0        0     4168 2023-08-03 14:57:28.000000 delia-1.2.5/delia/readers/patient_data/patient_data_query_context.py
+-rw-rw-rw-   0        0        0      931 2023-08-03 13:41:17.000000 delia-1.2.5/delia/readers/patient_data/patient_data_query_strategy.py
+-rw-rw-rw-   0        0        0    10470 2023-08-03 14:57:28.000000 delia-1.2.5/delia/readers/patient_data/patient_data_reader.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.749742 delia-1.2.5/delia/readers/segmentation/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.5/delia/readers/segmentation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.756863 delia-1.2.5/delia/readers/segmentation/factories/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.5/delia/readers/segmentation/factories/__init__.py
+-rw-rw-rw-   0        0        0     2209 2023-08-03 14:57:28.000000 delia-1.2.5/delia/readers/segmentation/factories/base_segmentation_factory.py
+-rw-rw-rw-   0        0        0     7023 2023-08-03 14:57:28.000000 delia-1.2.5/delia/readers/segmentation/factories/dicom_segmentation_factories.py
+-rw-rw-rw-   0        0        0     1260 2022-07-27 14:35:42.000000 delia-1.2.5/delia/readers/segmentation/factories/segment.py
+-rw-rw-rw-   0        0        0     2830 2022-02-08 18:32:16.000000 delia-1.2.5/delia/readers/segmentation/factories/segmentation.py
+-rw-rw-rw-   0        0        0     5006 2023-08-03 14:57:28.000000 delia-1.2.5/delia/readers/segmentation/segmentation_context.py
+-rw-rw-rw-   0        0        0     3034 2023-08-03 14:57:28.000000 delia-1.2.5/delia/readers/segmentation/segmentation_reader.py
+-rw-rw-rw-   0        0        0     2217 2023-05-05 16:07:22.000000 delia-1.2.5/delia/readers/segmentation/segmentation_strategy.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.760222 delia-1.2.5/delia/transforms/
+-rw-rw-rw-   0        0        0      120 2023-03-16 15:36:25.000000 delia-1.2.5/delia/transforms/__init__.py
+-rw-rw-rw-   0        0        0    13141 2023-06-20 15:23:09.000000 delia-1.2.5/delia/transforms/applications.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.763447 delia-1.2.5/delia/transforms/array_space/
+-rw-rw-rw-   0        0        0      293 2023-03-16 15:36:25.000000 delia-1.2.5/delia/transforms/array_space/__init__.py
+-rw-rw-rw-   0        0        0     5085 2023-06-20 15:23:09.000000 delia-1.2.5/delia/transforms/array_space/matching_centroid_spatial_crop.py
+-rw-rw-rw-   0        0        0     3096 2023-06-20 15:23:09.000000 delia-1.2.5/delia/transforms/array_space/matching_crop_foreground.py
+-rw-rw-rw-   0        0        0     1043 2023-03-16 16:39:24.000000 delia-1.2.5/delia/transforms/array_space/tools.py
+-rw-rw-rw-   0        0        0     2544 2023-06-20 15:23:09.000000 delia-1.2.5/delia/transforms/array_space/transform.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.765518 delia-1.2.5/delia/transforms/data/
+-rw-rw-rw-   0        0        0      115 2023-03-16 15:36:25.000000 delia-1.2.5/delia/transforms/data/__init__.py
+-rw-rw-rw-   0        0        0     4558 2023-06-20 15:23:09.000000 delia-1.2.5/delia/transforms/data/copy_segmentations.py
+-rw-rw-rw-   0        0        0     1864 2023-06-20 15:23:09.000000 delia-1.2.5/delia/transforms/data/transform.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.771080 delia-1.2.5/delia/transforms/physical_space/
+-rw-rw-rw-   0        0        0      269 2023-03-27 00:27:35.000000 delia-1.2.5/delia/transforms/physical_space/__init__.py
+-rw-rw-rw-   0        0        0     3360 2023-06-20 15:23:09.000000 delia-1.2.5/delia/transforms/physical_space/matching_resample.py
+-rw-rw-rw-   0        0        0     9808 2023-06-20 15:23:09.000000 delia-1.2.5/delia/transforms/physical_space/pet_to_suv.py
+-rw-rw-rw-   0        0        0     3694 2023-06-20 15:23:09.000000 delia-1.2.5/delia/transforms/physical_space/resample.py
+-rw-rw-rw-   0        0        0     2992 2023-06-20 15:23:09.000000 delia-1.2.5/delia/transforms/physical_space/transform.py
+-rw-rw-rw-   0        0        0     2403 2023-06-20 15:23:09.000000 delia-1.2.5/delia/transforms/tools.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.774115 delia-1.2.5/delia/utils/
+-rw-rw-rw-   0        0        0       42 2022-11-08 03:52:44.000000 delia-1.2.5/delia/utils/__init__.py
+-rw-rw-rw-   0        0        0     4101 2023-03-16 14:44:58.000000 delia-1.2.5/delia/utils/data_model.py
+-rw-rw-rw-   0        0        0     1329 2022-03-25 22:07:08.000000 delia-1.2.5/delia/utils/tools.py
+-rw-rw-rw-   0        0        0     2131 2022-11-08 03:00:14.000000 delia-1.2.5/delia/utils/transforms_history.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.722313 delia-1.2.5/delia.egg-info/
+-rw-rw-rw-   0        0        0    15339 2023-08-03 15:09:10.000000 delia-1.2.5/delia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2252 2023-08-03 15:09:10.000000 delia-1.2.5/delia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 15:09:10.000000 delia-1.2.5/delia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-08-03 15:09:10.000000 delia-1.2.5/delia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-03 15:09:10.000000 delia-1.2.5/delia.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 15:09:10.780571 delia-1.2.5/examples/
+-rw-rw-rw-   0        0        0       38 2022-03-26 17:30:16.000000 delia-1.2.5/examples/__init__.py
+-rw-rw-rw-   0        0        0      712 2022-03-29 17:53:18.000000 delia-1.2.5/examples/env_examples.py
+-rw-rw-rw-   0        0        0     3474 2023-08-03 15:03:38.000000 delia-1.2.5/examples/ex01.py
+-rw-rw-rw-   0        0        0     3119 2023-08-03 13:41:17.000000 delia-1.2.5/examples/ex02.py
+-rw-rw-rw-   0        0        0     2760 2023-08-03 13:41:17.000000 delia-1.2.5/examples/ex03.py
+-rw-rw-rw-   0        0        0     5382 2023-08-03 13:41:17.000000 delia-1.2.5/examples/ex04.py
+-rw-rw-rw-   0        0        0      108 2022-01-10 21:30:41.000000 delia-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 15:09:10.781733 delia-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2023-08-03 15:08:01.000000 delia-1.2.5/setup.py
```

### Comparing `delia-1.2.4/LICENSE` & `delia-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/PKG-INFO` & `delia-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delia
-Version: 1.2.4
+Version: 1.2.5
 Summary: DICOM Extraction for Large-scale Image Analysis (DELIA).
 Home-page: https://github.com/MaxenceLarose/delia
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: dicom hdf5 medical image segmentation pre-processing python3 radiomics deep-learning dicom-seg rt-struct
 Classifier: Programming Language :: Python :: 3
```

### Comparing `delia-1.2.4/README.md` & `delia-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/__init__.py` & `delia-1.2.5/delia/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 from .utils import PatientDataModel
 
 stream_handler = logging.StreamHandler()
 stream_handler.setLevel(logging.WARNING)
 logging.getLogger(__name__).addHandler(stream_handler)
 
 __author__ = "Maxence Larose"
-__version__ = "1.2.4"
+__version__ = "1.2.5"
 __copyright__ = "Copyright 2022, Maxence Larose"
 __credits__ = ["Maxence Larose"]
 __license__ = "Apache License 2.0"
 __maintainer__ = "Maxence Larose"
 __email__ = "maxence.larose.1@ulaval.ca"
 __status__ = "Production"
```

### Comparing `delia-1.2.4/delia/databases/patients_database.py` & `delia-1.2.5/delia/databases/patients_database.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/extractors/patients_data_extractor.py` & `delia-1.2.5/delia/extractors/patients_data_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
     """
 
     def __init__(
             self,
             path_to_patients_folder: str,
             tag: Union[str, Tuple[int, int]] = "Modality",
             tag_values: Optional[Union[str, Dict[str, List[str]]]] = None,
+            load_segmentations: bool = True,
+            organs: Optional[List[str]] = None,
             transforms: Optional[Union[Compose, DataTransform, MonaiMapTransform, PhysicalSpaceTransform]] = None,
             erase_unused_dicom_files: bool = False
     ) -> None:
         """
         Used to get the paths to the images and segmentations folders. Also used to check if either the tag values or
         the path to the tag value json dictionary is None.
 
@@ -60,26 +62,32 @@
             Keyword or tuple of the DICOM tag to use while selecting which files to extract. Uses Modality as a default.
         tag_values : Optional[Union[str, Dict[str, List[str]]]], default = None.
             A dictionary that contains the desired tag's values for the images that absolutely needs to be extracted
             from the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
             values associated with the specified tag. The images associated with these values do not need to have a
             corresponding segmentation. Note that it can be specified as a path to a json dictionary that contains the
             desired values for the tag.
+        load_segmentations : bool = True
+            Whether to load the segmentations or not.
+        organs : Optional[List[str]] = None
+            A list of organs to load. If None, all organs are loaded.
         transforms : Union[Compose, DataTransform, MonaiMapTransform, PhysicalSpaceTransform]
             A sequence of transformations to apply. PhysicalSpaceTransform are applied in the physical space, i.e on
             the SimpleITK image, while MonaiMapTransform are applied in the array space, i.e on the numpy array that
             represents the image. DataTransform transforms the data using other a patient's other images or
             segmentations. The keys for images are assumed to be the arbitrary series key set in 'tag_values'.
             For segmentation, keys are organ names. Note that if 'tag_values' is None, the keys for images are
             assumed to be modalities.
         erase_unused_dicom_files: bool = False
             Whether to delete unused DICOM files or not. Use with EXTREME caution!
         """
         self._path_to_patients_folder = path_to_patients_folder
         self._erase_unused_dicom_files = erase_unused_dicom_files
+        self._load_segmentations = load_segmentations
+        self._organs = organs
         self._transforms = self._validate_transforms(transforms)
         self.tag = tag
 
         if isinstance(tag_values, str):
             self.path_to_tag_value_json = tag_values
         elif isinstance(tag_values, dict):
             self.tag_values = tag_values
@@ -293,14 +301,16 @@
         _logger.info(f"Downloading Patient {self._current_index + 1}/{len(self)}")
         _logger.info(f"Path to patient folder : {self.paths_to_patients_folders[self._current_index]}")
 
         patient_data_reader = PatientDataReader(
             path_to_patient_folder=self.paths_to_patients_folders[self._current_index],
             tag_values=self.tag_values,
             tag=self.tag,
+            load_segmentations=self._load_segmentations,
+            organs=self._organs,
             erase_unused_dicom_files=self._erase_unused_dicom_files
         )
 
         if self._tag_values is not None:
             self.tag_values = patient_data_reader.tag_values
         if self.path_to_tag_value_json:
             self.save_tag_values_to_json(path=self._path_to_tag_value_json)
```

### Comparing `delia-1.2.4/delia/radiomics/radiomics_dataset.py` & `delia-1.2.5/delia/radiomics/radiomics_dataset.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/readers/image/dicom_reader.py` & `delia-1.2.5/delia/readers/image/dicom_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                         folder.
 """
 
 from collections import defaultdict
 from glob import glob
 import logging
 import os
-from typing import Dict, List, NamedTuple, Set, Tuple, Union
+from typing import Dict, List, NamedTuple, Optional, Set, Tuple, Union
 
 import pydicom
 import SimpleITK as sitk
 
 from delia.utils.data_model import ImageDataModel
 from delia.readers.segmentation.segmentation_strategy import SegmentationStrategies
 from delia.utils.tools import is_path_valid
@@ -39,30 +39,34 @@
         tag_value: str
         paths_to_dicoms_from_series: List[str]
         dicom_header: pydicom.dataset.FileDataset
 
     def __init__(
             self,
             path_to_patient_folder: str,
-            tag: Union[str, Tuple[int, int]]
+            tag: Union[str, Tuple[int, int]],
+            load_segmentations: bool = True
     ):
         """
         Constructor of the class DicomReader.
 
         Parameters
         ----------
         path_to_patient_folder : str
             Path to the folder containing the patient DICOM files.
         tag : Union[str, Tuple[int, int]]
             Keyword or tuple of the DICOM tag to use while selecting which files to extract.
+        load_segmentations : bool
+            Whether to load segmentations or not.
         """
         super(DicomReader, self).__init__()
 
         is_path_valid(path=path_to_patient_folder)
         self._path_to_patient_folder = path_to_patient_folder
+        self._load_segmentations = load_segmentations
         self.tag = tag
 
         self._images_series_data_dict = {}
         self._segmentations_series_data_dict = {}
         self.__series_data_dict = self.__get_series_data_dict()
 
     @staticmethod
@@ -186,15 +190,16 @@
         elif len(all_patient_ids) > 1:
             raise AssertionError(f"All DICOM files in the same folder must belong to the same patient. This is not "
                                  f"the case for the patient whose data is currently being downloaded since the "
                                  f"identifiers {all_patient_ids} are found in their folder.")
 
         for series_id, series_data in series_data_dict.items():
             if series_data.dicom_header.Modality in SegmentationStrategies.get_available_modalities():
-                self._segmentations_series_data_dict[series_id] = series_data
+                if self._load_segmentations:
+                    self._segmentations_series_data_dict[series_id] = series_data
             else:
                 self._images_series_data_dict[series_id] = series_data
 
         return series_data_dict
 
     @staticmethod
     def __get_3d_sitk_image_from_dicom_series(
```

### Comparing `delia-1.2.4/delia/readers/patient_data/factories/base_patient_data_factory.py` & `delia-1.2.5/delia/readers/patient_data/factories/base_patient_data_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
     def __init__(
             self,
             path_to_patient_folder: str,
             paths_to_segmentations: Optional[List[str]],
             tag_values: Optional[Dict[str, List[str]]],
             tag: Union[str, Tuple[int, int]],
+            organs: Optional[List[str]] = None,
             erase_unused_dicom_files: bool = False
     ):
         """
         Constructor of the class BasePatientDataFactory.
 
         Parameters
         ----------
@@ -43,20 +44,23 @@
             List of paths to the patient's segmentation files.
         tag_values : Optional[Dict[str, List[str]]]
             A dictionary that contains the desired tag's values for the images that absolutely needs to be extracted
             from the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
             values associated with the specified tag.
         tag : Union[str, Tuple[int, int]]
             Keyword or tuple of the DICOM tag to use while selecting which files to extract.
+        organs : Optional[List[str]]
+            A set of the organs to save.
         erase_unused_dicom_files: bool = False
             Whether to delete unused DICOM files or not. Use with caution.
         """
         self._path_to_patient_folder = path_to_patient_folder
         self._paths_to_segmentations = paths_to_segmentations
         self._tag_values = tag_values
+        self._organs = organs
         self._erase_unused_dicom_files = erase_unused_dicom_files
         self.tag = tag
 
         dicom_reader = DicomReader(path_to_patient_folder=self._path_to_patient_folder, tag=self.tag)
         self._images_data = dicom_reader.get_images_data(remove_segmentations=True)
 
     @property
```

### Comparing `delia-1.2.4/delia/readers/patient_data/factories/patient_data_factories.py` & `delia-1.2.5/delia/readers/patient_data/factories/patient_data_factories.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     def __init__(
             self,
             path_to_patient_folder: str,
             paths_to_segmentations: Optional[List[str]],
             tag_values: Optional[Dict[str, List[str]]],
             tag: Union[str, Tuple[int, int]],
+            organs: Optional[List[str]] = None,
             erase_unused_dicom_files: bool = False
     ):
         """
         Constructor of the class DefaultPatientDataFactory.
 
         Parameters
         ----------
@@ -41,22 +42,25 @@
             List of paths to the patient's segmentation files.
         tag_values : Optional[Dict[str, List[str]]]
             A dictionary that contains the desired tag's values for the images that absolutely needs to be extracted
             from the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
             values associated with the specified tag.
         tag : Union[str, Tuple[int, int]]
             Keyword or tuple of the DICOM tag to use while selecting which files to extract.
+        organs : Optional[List[str]]
+            A set of the organs to segment.
         erase_unused_dicom_files: bool = False
             Whether to delete unused DICOM files or not. Use with caution.
         """
         super().__init__(
             path_to_patient_folder=path_to_patient_folder,
             paths_to_segmentations=paths_to_segmentations,
             tag_values=tag_values,
             tag=tag,
+            organs=organs,
             erase_unused_dicom_files=erase_unused_dicom_files
         )
 
     def create_patient_data(self) -> PatientDataModel:
         """
         Creates a tuple containing all the patient's data.
 
@@ -71,15 +75,16 @@
             for path_to_segmentation in self._paths_to_segmentations:
                 seg_header = DicomReader.get_dicom_header(path_to_dicom=path_to_segmentation)
                 reference_uid = self.get_segmentation_reference_uid(seg_header)
 
                 if image.dicom_header.SeriesInstanceUID == reference_uid:
                     segmentation_reader = SegmentationReader(
                         image=image,
-                        path_to_segmentation=path_to_segmentation
+                        path_to_segmentation=path_to_segmentation,
+                        organs=self._organs
                     )
 
                     segmentations.append(segmentation_reader.get_segmentation_data())
 
             if segmentations:
                 image_and_segmentation_data = ImageAndSegmentationDataModel(
                     image=image,
@@ -105,14 +110,15 @@
 
     def __init__(
             self,
             path_to_patient_folder: str,
             paths_to_segmentations: Optional[List[str]],
             tag_values: Optional[Dict[str, List[str]]],
             tag: Union[str, Tuple[int, int]],
+            organs: Optional[List[str]] = None,
             erase_unused_dicom_files: bool = False
     ):
         """
         Constructor of the class SpecificTagPatientDataFactory.
 
         Parameters
         ----------
@@ -122,22 +128,25 @@
             List of paths to the patient's segmentation files.
         tag_values : Optional[Dict[str, List[str]]]
             A dictionary that contains the desired tag's values for the images that absolutely needs to be extracted
             from the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
             values associated with the specified tag.
         tag : Union[str, Tuple[int, int]]
             Keyword or tuple of the DICOM tag to use while selecting which files to extract.
+        organs : Optional[List[str]]
+            A set of the organs to segment.
         erase_unused_dicom_files: bool = False
             Whether to delete unused DICOM files or not. Use with caution.
         """
         super().__init__(
             path_to_patient_folder=path_to_patient_folder,
             paths_to_segmentations=paths_to_segmentations,
             tag_values=tag_values,
             tag=tag,
+            organs=organs,
             erase_unused_dicom_files=erase_unused_dicom_files
         )
 
     def create_patient_data(self) -> PatientDataModel:
         """
         Creates a tuple containing all the patient's data.
 
@@ -161,15 +170,16 @@
                     for path_to_segmentation in self._paths_to_segmentations:
                         seg_header = DicomReader.get_dicom_header(path_to_dicom=path_to_segmentation)
                         reference_uid = self.get_segmentation_reference_uid(seg_header)
 
                         if image.dicom_header.SeriesInstanceUID == reference_uid:
                             segmentation_reader = SegmentationReader(
                                 image=image,
-                                path_to_segmentation=path_to_segmentation
+                                path_to_segmentation=path_to_segmentation,
+                                organs=self._organs
                             )
 
                             segmentations.append(segmentation_reader.get_segmentation_data())
 
                     if segmentations:
                         image_and_segmentation_data = ImageAndSegmentationDataModel(
                             image=image,
```

### Comparing `delia-1.2.4/delia/readers/patient_data/patient_data_query_context.py` & `delia-1.2.5/delia/readers/patient_data/patient_data_query_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
     def __init__(
             self,
             path_to_patient_folder: str,
             paths_to_segmentations: Optional[List[str]],
             tag_values: Dict[str, List[str]],
             tag: Union[str, Tuple[int, int]],
+            organs: Optional[List[str]] = None,
             erase_unused_dicom_files: bool = False
     ):
         """
         Constructor of the PatientDataQueryContext class.
 
         Parameters
         ----------
@@ -40,20 +41,23 @@
             List of paths to the patient's segmentation files.
         tag_values : Dict[str, List[str]]
             A dictionary that contains the desired tag's values for the images that absolutely needs to be extracted
             from the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
             values associated with the specified tag.
         tag : Union[str, Tuple[int, int]]
             Keyword or tuple of the DICOM tag to use while selecting which files to extract.
+        organs : Optional[List[str]]
+            A set of the organs to save.
         erase_unused_dicom_files: bool = False
             Whether to delete unused DICOM files or not. Use with caution.
         """
         self._path_to_patient_folder = path_to_patient_folder
         self._paths_to_segmentations = paths_to_segmentations
         self._tag_values = tag_values
+        self._organs = organs
         self._erase_unused_dicom_files = erase_unused_dicom_files
         self.tag = tag
 
     @property
     def patient_data_query_strategy(self) -> PatientDataQueryStrategy:
         """
         Patient data query strategy corresponding to the given tag values configuration.
@@ -79,14 +83,15 @@
             Factory class instance used to get a patient's data.
         """
         patient_data_factory_instance = self.patient_data_query_strategy.factory(
             path_to_patient_folder=self._path_to_patient_folder,
             paths_to_segmentations=self._paths_to_segmentations,
             tag_values=self._tag_values,
             tag=self.tag,
+            organs=self._organs,
             erase_unused_dicom_files=self._erase_unused_dicom_files
         )
 
         return patient_data_factory_instance
 
     def create_patient_data(self) -> PatientDataModel:
         """
```

### Comparing `delia-1.2.4/delia/readers/patient_data/patient_data_query_strategy.py` & `delia-1.2.5/delia/readers/patient_data/patient_data_query_strategy.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/readers/patient_data/patient_data_reader.py` & `delia-1.2.5/delia/readers/patient_data/patient_data_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     """
 
     def __init__(
             self,
             path_to_patient_folder: str,
             tag_values: Optional[Dict[str, List[str]]],
             tag: Union[str, Tuple[int, int]],
+            load_segmentations: bool = True,
+            organs: Optional[List[str]] = None,
             erase_unused_dicom_files: bool = False
     ):
         """
         Used to check availability of given series' uid and tag values in the patient's dicom files.
 
         Parameters
         ----------
@@ -47,23 +49,31 @@
             Path to the folder containing the patient's files.
         tag_values : Dict[str, List[str]]
             A dictionary that contains the desired tag's values for the images that absolutely needs to be extracted
             from the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
             values associated with the specified tag.
         tag : Union[str, Tuple[int, int]]
             Keyword or tuple of the DICOM tag to use while selecting which files to extract.
+        load_segmentations : bool = True
+            Whether to load the segmentation files or not.
+        organs : Optional[List[str]] = None
+            List of organs to load. If None, all organs will be loaded.
         erase_unused_dicom_files: bool = False
             Whether to delete unused DICOM files or not. Use with caution.
         """
-        self.tag = tag
-        super().__init__(path_to_patient_folder=path_to_patient_folder, tag=self.tag)
+        super().__init__(
+            path_to_patient_folder=path_to_patient_folder,
+            tag=tag,
+            load_segmentations=load_segmentations
+        )
 
         self._images_dicom_headers = self.get_dicom_headers(remove_segmentations=True)
         self._tag_values = tag_values
         self._erase_unused_dicom_files = erase_unused_dicom_files
+        self._organs = organs
 
         self.failed_images = []
         if tag_values is not None:
             self.check_availability_of_given_tag_value()
 
     @property
     def patient_id(self) -> str:
@@ -202,14 +212,15 @@
             segmentation data extracted from the segmentation files.
         """
         patient_data_context = PatientDataQueryContext(
             path_to_patient_folder=self._path_to_patient_folder,
             paths_to_segmentations=self.paths_to_segmentations,
             tag_values=self._tag_values,
             tag=self.tag,
+            organs=self._organs,
             erase_unused_dicom_files=self._erase_unused_dicom_files
         )
         patient_dataset = patient_data_context.create_patient_data()
 
         if transforms:
             apply_transforms(patient_dataset=patient_dataset, transforms=transforms)
```

### Comparing `delia-1.2.4/delia/readers/segmentation/factories/base_segmentation_factory.py` & `delia-1.2.5/delia/readers/segmentation/factories/base_segmentation_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     @Description:       This file contains the class SegmentationFactory that is used as an abstract class used as a
                         reference for all other segmentation classes that read data and build a Segmentation object
                         from it.
 """
 
 from abc import ABC, abstractmethod
-from typing import List
+from typing import List, Optional
 
 from ....utils.data_model import ImageDataModel
 from .segment import Segment
 from .segmentation import Segmentation
 
 
 class BaseSegmentationFactory(ABC):
@@ -24,28 +24,32 @@
     Segmentation object from it.
     """
 
     def __init__(
             self,
             image: ImageDataModel,
             path_to_segmentation: str,
+            organs: Optional[List[str]] = None
     ):
         """
         Used to load the segmentation data from the path to segmentation.
 
         Parameters
         ----------
         image : ImageDataModel
             A named tuple grouping the patient's dicom header, its medical image as a simpleITK image and a sequence of
             the paths to each dicom contained in the series.
         path_to_segmentation : str
             The path to the segmentation file.
+        organs : Optional[List[str]]
+            The set of organs to save.
         """
         self._image = image
         self._path_to_segmentation = path_to_segmentation
+        self._organs = organs
 
     @property
     @abstractmethod
     def segments(self) -> List[Segment]:
         """
         Abstract segments property.
```

### Comparing `delia-1.2.4/delia/readers/segmentation/factories/dicom_segmentation_factories.py` & `delia-1.2.5/delia/readers/segmentation/factories/dicom_segmentation_factories.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     @Last modification: 03/2022
 
     @Description:       This file contains the abstract class BaseDicomSegmentationFactory and all factories that
                         inherit from this class.
 """
 
 from abc import abstractmethod
-from typing import List
+from typing import List, Optional
 
 import numpy as np
 import pydicom
 import pydicom_seg
 from rt_utils import RTStruct
 import SimpleITK as sitk
 
@@ -29,30 +29,34 @@
     classes differ by the type of segmentation they are able to read. Indeed, the format of the segmentations may be
     different even if the file extension is the same, because there is multiple ways of representing a segment.
     """
 
     def __init__(
             self,
             image: ImageDataModel,
-            path_to_segmentation: str
+            path_to_segmentation: str,
+            organs: Optional[List[str]] = None
     ):
         """
         Used to load the segmentation data from the path to segmentation.
 
         Parameters
         ----------
         image : ImageDataModel
             A named tuple grouping the patient's dicom header, its medical image as a simpleITK image and a sequence of
             the paths to each dicom contained in the series.
         path_to_segmentation : str
             The path to the segmentation file.
+        organs : Optional[List[str]]
+            The set of organs to save.
         """
         super().__init__(
             image=image,
-            path_to_segmentation=path_to_segmentation
+            path_to_segmentation=path_to_segmentation,
+            organs=organs
         )
 
         self._dicom: pydicom.FileDataset = pydicom.dcmread(path_to_segmentation)
 
     @abstractmethod
     def segments(self) -> List[Segment]:
         """
@@ -70,30 +74,34 @@
     """
     Class that defined the methods that are used to get the segments for the DICOM-SEG type of segmentation.
     """
 
     def __init__(
             self,
             image: ImageDataModel,
-            path_to_segmentation: str
+            path_to_segmentation: str,
+            organs: Optional[List[str]] = None
     ):
         """
         Used to load the segmentation data from the path to segmentation.
 
         Parameters
         ----------
         image : ImageDataModel
             A named tuple grouping the patient's dicom header, its medical image as a simpleITK image and a sequence of
             the paths to each dicom contained in the series.
         path_to_segmentation : str
             The path to the segmentation file.
+        organs : Optional[List[str]]
+            The set of organs to save.
         """
         super().__init__(
             image=image,
-            path_to_segmentation=path_to_segmentation
+            path_to_segmentation=path_to_segmentation,
+            organs=organs
         )
 
     @property
     def _reader(self) -> pydicom_seg.SegmentReader:
         """
         Reader property.
 
@@ -119,45 +127,50 @@
         segments = []
         for segment_number, dicom_header in result.segment_infos.items():
             if dicom_header.__contains__("SegmentLabel"):
                 organ_name = dicom_header.SegmentLabel
             else:
                 organ_name = dicom_header.SegmentDescription
 
-            simple_itk_label_map = result.segment_image(segment_number)
-
-            segments.append(Segment(name=organ_name, simple_itk_label_map=simple_itk_label_map))
+            load_organ = True if self._organs is None else organ_name in self._organs
+            if load_organ:
+                simple_itk_label_map = result.segment_image(segment_number)
+                segments.append(Segment(name=organ_name, simple_itk_label_map=simple_itk_label_map))
 
         return segments
 
 
 class RTStructSegmentationFactory(BaseDicomSegmentationFactory):
     """
     Class that defined the methods that are used to get the segments for the RT Struct type of segmentation.
     """
 
     def __init__(
             self,
             image: ImageDataModel,
-            path_to_segmentation: str
+            path_to_segmentation: str,
+            organs: Optional[List[str]] = None
     ):
         """
         Used to load the segmentation data from the path to segmentation.
 
         Parameters
         ----------
         image : ImageDataModel
             A named tuple grouping the patient's dicom header, its medical image as a simpleITK image and a sequence of
             the paths to each dicom contained in the series.
         path_to_segmentation : str
             The path to the segmentation file.
+        organs : Optional[List[str]]
+            The set of organs to save.
         """
         super().__init__(
             image=image,
-            path_to_segmentation=path_to_segmentation
+            path_to_segmentation=path_to_segmentation,
+            organs=organs
         )
 
     @property
     def _reader(self) -> RTStruct:
         """
         Reader property.
 
@@ -181,19 +194,22 @@
         segments : List[Segment]
             List of all the segments.
         """
         segment_names = self._reader.get_roi_names()
         segments = []
 
         for organ_name in segment_names:
-            array = self._reader.get_roi_mask_by_name(organ_name)
-            array = np.multiply(array, 1)
-            array = array.transpose(2, 0, 1)
-
-            simple_itk_label_map = sitk.GetImageFromArray(array)
-            simple_itk_label_map.SetOrigin(self._image.simple_itk_image.GetOrigin())
-            simple_itk_label_map.SetSpacing(self._image.simple_itk_image.GetSpacing())
-            simple_itk_label_map.SetDirection(self._image.simple_itk_image.GetDirection())
+            load_organ = True if self._organs is None else organ_name in self._organs
+
+            if load_organ:
+                array = self._reader.get_roi_mask_by_name(organ_name)
+                array = np.multiply(array, 1)
+                array = array.transpose(2, 0, 1)
+
+                simple_itk_label_map = sitk.GetImageFromArray(array)
+                simple_itk_label_map.SetOrigin(self._image.simple_itk_image.GetOrigin())
+                simple_itk_label_map.SetSpacing(self._image.simple_itk_image.GetSpacing())
+                simple_itk_label_map.SetDirection(self._image.simple_itk_image.GetDirection())
 
-            segments.append(Segment(name=organ_name, simple_itk_label_map=simple_itk_label_map))
+                segments.append(Segment(name=organ_name, simple_itk_label_map=simple_itk_label_map))
 
         return segments
```

### Comparing `delia-1.2.4/delia/readers/segmentation/factories/segment.py` & `delia-1.2.5/delia/readers/segmentation/factories/segment.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/readers/segmentation/factories/segmentation.py` & `delia-1.2.5/delia/readers/segmentation/factories/segmentation.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/readers/segmentation/segmentation_context.py` & `delia-1.2.5/delia/readers/segmentation/segmentation_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     @Last modification: 01/2022
 
     @Description:       This file contains the class SegmentationContext that is used as a context class where
                         strategies are types of ways to load the segmentation data, or more precisely, types of
                         segmentation object factory.
 """
 
+from typing import List, Optional
+
 import pydicom
 
 from .segmentation_strategy import SegmentationStrategy, SegmentationStrategies
 from .factories.segmentation import Segmentation
 from ...utils.data_model import ImageDataModel
 
 
@@ -23,29 +25,33 @@
     types of segmentation object factory. Strategies are entirely defined by the extension of the given file and so, by
     the path of the segmentation.
     """
 
     def __init__(
             self,
             image: ImageDataModel,
-            path_to_segmentation: str
+            path_to_segmentation: str,
+            organs: Optional[List[str]] = None
     ):
         """
         Constructor of the SegmentationContext class.
 
         Parameters
         ----------
         image : ImageDataModel
             A named tuple grouping the patient's dicom header, its medical image as a simpleITK image and a sequence of
             the paths to each dicom contained in the series.
         path_to_segmentation : str
             The path to the segmentation file.
+        organs : Optional[List[str]]
+            A set of the organs to segment.
         """
         self._image = image
         self._path_to_segmentation = path_to_segmentation
+        self._organs = organs
 
     @property
     def path_to_segmentation(self) -> str:
         """
         Path to segmentation property.
 
         Returns
@@ -124,15 +130,16 @@
         Returns
         -------
         _segmentation_factory_instance : SegmentationStrategy.factory
             Factory class instance used to get the label maps and the segmentation metadata from a segmentation file.
         """
         return self.segmentation_strategy.factory(
             image=self._image,
-            path_to_segmentation=self.path_to_segmentation
+            path_to_segmentation=self.path_to_segmentation,
+            organs=self._organs
         )
 
     def create_segmentation(self) -> Segmentation:
         """
         Creates a Segmentation object.
 
         Returns
```

### Comparing `delia-1.2.4/delia/readers/segmentation/segmentation_reader.py` & `delia-1.2.5/delia/readers/segmentation/segmentation_reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,16 @@
     @Creation Date:     10/2021
     @Last modification: 01/2022
 
     @Description:       This file contains the SegmentationReader class which is used to read a given segmentation file
                         and transform its contents into the format of the SegmentationDataModel class.
 """
 
+from typing import List, Optional
+
 from .segmentation_context import SegmentationContext
 from .factories.segmentation import Segmentation
 from ...utils.data_model import ImageDataModel, SegmentationDataModel
 
 
 class SegmentationReader:
     """
@@ -20,42 +22,47 @@
     SegmentationDataModel class.
     """
 
     def __init__(
             self,
             image: ImageDataModel,
             path_to_segmentation: str,
+            organs: Optional[List[str]] = None
     ):
         """
         Constructor of the class SegmentationReader.
 
         Parameters
         ----------
         image : ImageDataModel
             A named tuple grouping the patient's dicom header, its medical image as a simpleITK image and a sequence of
             the paths to each dicom contained in the series.
         path_to_segmentation : str
             The path to the segmentation file.
+        organs : Optional[List[str]]
+            A set of the organs to segment.
         """
         self._image = image
         self._path_to_segmentation = path_to_segmentation
+        self._organs = organs
 
     @property
     def __segmentation_context_manager(self) -> SegmentationContext:
         """
         Creates a SegmentationContext object.
 
         Returns
         -------
         segmentation_context : SegmentationContext
             Segmentation context manager.
         """
         return SegmentationContext(
             image=self._image,
-            path_to_segmentation=self._path_to_segmentation
+            path_to_segmentation=self._path_to_segmentation,
+            organs=self._organs
         )
 
     @property
     def __segmentation(self) -> Segmentation:
         """
         Creates a Segmentation object.
```

### Comparing `delia-1.2.4/delia/readers/segmentation/segmentation_strategy.py` & `delia-1.2.5/delia/readers/segmentation/segmentation_strategy.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/transforms/applications.py` & `delia-1.2.5/delia/transforms/applications.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/transforms/array_space/matching_centroid_spatial_crop.py` & `delia-1.2.5/delia/transforms/array_space/matching_centroid_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/transforms/array_space/matching_crop_foreground.py` & `delia-1.2.5/delia/transforms/array_space/matching_crop_foreground.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/transforms/array_space/tools.py` & `delia-1.2.5/delia/transforms/array_space/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/transforms/array_space/transform.py` & `delia-1.2.5/delia/transforms/array_space/transform.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/transforms/data/copy_segmentations.py` & `delia-1.2.5/delia/transforms/data/copy_segmentations.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/transforms/data/transform.py` & `delia-1.2.5/delia/transforms/data/transform.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/transforms/physical_space/matching_resample.py` & `delia-1.2.5/delia/transforms/physical_space/matching_resample.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/transforms/physical_space/pet_to_suv.py` & `delia-1.2.5/delia/transforms/physical_space/pet_to_suv.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/transforms/physical_space/resample.py` & `delia-1.2.5/delia/transforms/physical_space/resample.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/transforms/physical_space/transform.py` & `delia-1.2.5/delia/transforms/physical_space/transform.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/transforms/tools.py` & `delia-1.2.5/delia/transforms/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/utils/data_model.py` & `delia-1.2.5/delia/utils/data_model.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/utils/tools.py` & `delia-1.2.5/delia/utils/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia/utils/transforms_history.py` & `delia-1.2.5/delia/utils/transforms_history.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/delia.egg-info/PKG-INFO` & `delia-1.2.5/delia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delia
-Version: 1.2.4
+Version: 1.2.5
 Summary: DICOM Extraction for Large-scale Image Analysis (DELIA).
 Home-page: https://github.com/MaxenceLarose/delia
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: dicom hdf5 medical image segmentation pre-processing python3 radiomics deep-learning dicom-seg rt-struct
 Classifier: Programming Language :: Python :: 3
```

### Comparing `delia-1.2.4/delia.egg-info/SOURCES.txt` & `delia-1.2.5/delia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/examples/env_examples.py` & `delia-1.2.5/examples/env_examples.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/examples/ex01.py` & `delia-1.2.5/examples/ex01.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/examples/ex02.py` & `delia-1.2.5/examples/ex02.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/examples/ex03.py` & `delia-1.2.5/examples/ex03.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/examples/ex04.py` & `delia-1.2.5/examples/ex04.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.4/setup.py` & `delia-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="delia",
-    version="1.2.4",
+    version="1.2.5",
     author="Maxence Larose",
     author_email="maxence.larose.1@ulaval.ca",
     description="DICOM Extraction for Large-scale Image Analysis (DELIA).",
     long_description=open('README.md', "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/MaxenceLarose/delia",
     license="Apache License 2.0",
```

