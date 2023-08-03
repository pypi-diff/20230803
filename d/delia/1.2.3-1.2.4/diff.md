# Comparing `tmp/delia-1.2.3.tar.gz` & `tmp/delia-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delia-1.2.3.tar", last modified: Wed Jul 12 22:16:11 2023, max compression
+gzip compressed data, was "delia-1.2.4.tar", last modified: Thu Aug  3 13:46:09 2023, max compression
```

## Comparing `delia-1.2.3.tar` & `delia-1.2.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.780358 delia-1.2.3/
--rw-rw-rw-   0        0        0    11549 2022-03-24 18:12:27.000000 delia-1.2.3/LICENSE
--rw-rw-rw-   0        0        0    15339 2023-07-12 22:16:11.779315 delia-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    14707 2023-06-20 15:23:09.000000 delia-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.680908 delia-1.2.3/delia/
--rw-rw-rw-   0        0        0      583 2023-07-12 22:15:09.000000 delia-1.2.3/delia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.688985 delia-1.2.3/delia/databases/
--rw-rw-rw-   0        0        0       49 2022-11-08 03:00:14.000000 delia-1.2.3/delia/databases/__init__.py
--rw-rw-rw-   0        0        0    13553 2023-07-12 22:13:37.000000 delia-1.2.3/delia/databases/patients_database.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.689989 delia-1.2.3/delia/extractors/
--rw-rw-rw-   0        0        0      187 2023-05-04 17:50:19.000000 delia-1.2.3/delia/extractors/__init__.py
--rw-rw-rw-   0        0        0    14578 2023-06-20 15:23:09.000000 delia-1.2.3/delia/extractors/patients_data_extractor.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.694117 delia-1.2.3/delia/radiomics/
--rw-rw-rw-   0        0        0      158 2023-05-04 17:50:19.000000 delia-1.2.3/delia/radiomics/__init__.py
--rw-rw-rw-   0        0        0    12188 2023-07-03 19:53:42.000000 delia-1.2.3/delia/radiomics/radiomics_dataset.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.695159 delia-1.2.3/delia/readers/
--rw-rw-rw-   0        0        0       65 2022-11-08 03:03:57.000000 delia-1.2.3/delia/readers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.698676 delia-1.2.3/delia/readers/image/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.3/delia/readers/image/__init__.py
--rw-rw-rw-   0        0        0    11258 2023-06-20 15:23:09.000000 delia-1.2.3/delia/readers/image/dicom_reader.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.705211 delia-1.2.3/delia/readers/patient_data/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.3/delia/readers/patient_data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.710472 delia-1.2.3/delia/readers/patient_data/factories/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.3/delia/readers/patient_data/factories/__init__.py
--rw-rw-rw-   0        0        0     5110 2023-06-20 15:23:09.000000 delia-1.2.3/delia/readers/patient_data/factories/base_patient_data_factory.py
--rw-rw-rw-   0        0        0     8114 2023-06-20 15:23:09.000000 delia-1.2.3/delia/readers/patient_data/factories/patient_data_factories.py
--rw-rw-rw-   0        0        0     3974 2023-06-20 15:23:09.000000 delia-1.2.3/delia/readers/patient_data/patient_data_query_context.py
--rw-rw-rw-   0        0        0      943 2023-06-20 15:23:09.000000 delia-1.2.3/delia/readers/patient_data/patient_data_query_strategy.py
--rw-rw-rw-   0        0        0    10030 2023-06-20 15:23:09.000000 delia-1.2.3/delia/readers/patient_data/patient_data_reader.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.716936 delia-1.2.3/delia/readers/segmentation/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.3/delia/readers/segmentation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.726100 delia-1.2.3/delia/readers/segmentation/factories/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.3/delia/readers/segmentation/factories/__init__.py
--rw-rw-rw-   0        0        0     2042 2022-11-08 03:20:33.000000 delia-1.2.3/delia/readers/segmentation/factories/base_segmentation_factory.py
--rw-rw-rw-   0        0        0     6278 2022-11-08 03:20:33.000000 delia-1.2.3/delia/readers/segmentation/factories/dicom_segmentation_factories.py
--rw-rw-rw-   0        0        0     1260 2022-07-27 14:35:42.000000 delia-1.2.3/delia/readers/segmentation/factories/segment.py
--rw-rw-rw-   0        0        0     2830 2022-02-08 18:32:16.000000 delia-1.2.3/delia/readers/segmentation/factories/segmentation.py
--rw-rw-rw-   0        0        0     4772 2023-05-05 16:07:22.000000 delia-1.2.3/delia/readers/segmentation/segmentation_context.py
--rw-rw-rw-   0        0        0     2801 2023-03-16 14:44:58.000000 delia-1.2.3/delia/readers/segmentation/segmentation_reader.py
--rw-rw-rw-   0        0        0     2217 2023-05-05 16:07:22.000000 delia-1.2.3/delia/readers/segmentation/segmentation_strategy.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.733406 delia-1.2.3/delia/transforms/
--rw-rw-rw-   0        0        0      120 2023-03-16 15:36:25.000000 delia-1.2.3/delia/transforms/__init__.py
--rw-rw-rw-   0        0        0    13141 2023-06-20 15:23:09.000000 delia-1.2.3/delia/transforms/applications.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.743532 delia-1.2.3/delia/transforms/array_space/
--rw-rw-rw-   0        0        0      293 2023-03-16 15:36:25.000000 delia-1.2.3/delia/transforms/array_space/__init__.py
--rw-rw-rw-   0        0        0     5085 2023-06-20 15:23:09.000000 delia-1.2.3/delia/transforms/array_space/matching_centroid_spatial_crop.py
--rw-rw-rw-   0        0        0     3096 2023-06-20 15:23:09.000000 delia-1.2.3/delia/transforms/array_space/matching_crop_foreground.py
--rw-rw-rw-   0        0        0     1043 2023-03-16 16:39:24.000000 delia-1.2.3/delia/transforms/array_space/tools.py
--rw-rw-rw-   0        0        0     2544 2023-06-20 15:23:09.000000 delia-1.2.3/delia/transforms/array_space/transform.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.749212 delia-1.2.3/delia/transforms/data/
--rw-rw-rw-   0        0        0      115 2023-03-16 15:36:25.000000 delia-1.2.3/delia/transforms/data/__init__.py
--rw-rw-rw-   0        0        0     4558 2023-06-20 15:23:09.000000 delia-1.2.3/delia/transforms/data/copy_segmentations.py
--rw-rw-rw-   0        0        0     1864 2023-06-20 15:23:09.000000 delia-1.2.3/delia/transforms/data/transform.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.759073 delia-1.2.3/delia/transforms/physical_space/
--rw-rw-rw-   0        0        0      269 2023-03-27 00:27:35.000000 delia-1.2.3/delia/transforms/physical_space/__init__.py
--rw-rw-rw-   0        0        0     3360 2023-06-20 15:23:09.000000 delia-1.2.3/delia/transforms/physical_space/matching_resample.py
--rw-rw-rw-   0        0        0     9808 2023-06-20 15:23:09.000000 delia-1.2.3/delia/transforms/physical_space/pet_to_suv.py
--rw-rw-rw-   0        0        0     3694 2023-06-20 15:23:09.000000 delia-1.2.3/delia/transforms/physical_space/resample.py
--rw-rw-rw-   0        0        0     2992 2023-06-20 15:23:09.000000 delia-1.2.3/delia/transforms/physical_space/transform.py
--rw-rw-rw-   0        0        0     2403 2023-06-20 15:23:09.000000 delia-1.2.3/delia/transforms/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.767432 delia-1.2.3/delia/utils/
--rw-rw-rw-   0        0        0       42 2022-11-08 03:52:44.000000 delia-1.2.3/delia/utils/__init__.py
--rw-rw-rw-   0        0        0     4101 2023-03-16 14:44:58.000000 delia-1.2.3/delia/utils/data_model.py
--rw-rw-rw-   0        0        0     1329 2022-03-25 22:07:08.000000 delia-1.2.3/delia/utils/tools.py
--rw-rw-rw-   0        0        0     2131 2022-11-08 03:00:14.000000 delia-1.2.3/delia/utils/transforms_history.py
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.685921 delia-1.2.3/delia.egg-info/
--rw-rw-rw-   0        0        0    15339 2023-07-12 22:16:11.000000 delia-1.2.3/delia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2252 2023-07-12 22:16:11.000000 delia-1.2.3/delia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 22:16:11.000000 delia-1.2.3/delia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-07-12 22:16:11.000000 delia-1.2.3/delia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-12 22:16:11.000000 delia-1.2.3/delia.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 22:16:11.778387 delia-1.2.3/examples/
--rw-rw-rw-   0        0        0       38 2022-03-26 17:30:16.000000 delia-1.2.3/examples/__init__.py
--rw-rw-rw-   0        0        0      712 2022-03-29 17:53:18.000000 delia-1.2.3/examples/env_examples.py
--rw-rw-rw-   0        0        0     3440 2023-06-20 15:23:09.000000 delia-1.2.3/examples/ex01.py
--rw-rw-rw-   0        0        0     3085 2023-06-20 15:23:09.000000 delia-1.2.3/examples/ex02.py
--rw-rw-rw-   0        0        0     2726 2023-06-20 15:23:09.000000 delia-1.2.3/examples/ex03.py
--rw-rw-rw-   0        0        0     5348 2023-06-20 15:23:09.000000 delia-1.2.3/examples/ex04.py
--rw-rw-rw-   0        0        0      108 2022-01-10 21:30:41.000000 delia-1.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 22:16:11.780358 delia-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-07-12 22:15:09.000000 delia-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.351452 delia-1.2.4/
+-rw-rw-rw-   0        0        0    11549 2022-03-24 18:12:27.000000 delia-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0    15339 2023-08-03 13:46:09.350405 delia-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    14707 2023-06-20 15:23:09.000000 delia-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.251046 delia-1.2.4/delia/
+-rw-rw-rw-   0        0        0      583 2023-08-03 13:45:17.000000 delia-1.2.4/delia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.256597 delia-1.2.4/delia/databases/
+-rw-rw-rw-   0        0        0       49 2022-11-08 03:00:14.000000 delia-1.2.4/delia/databases/__init__.py
+-rw-rw-rw-   0        0        0    13553 2023-07-12 22:13:37.000000 delia-1.2.4/delia/databases/patients_database.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.257602 delia-1.2.4/delia/extractors/
+-rw-rw-rw-   0        0        0      187 2023-05-04 17:50:19.000000 delia-1.2.4/delia/extractors/__init__.py
+-rw-rw-rw-   0        0        0    14538 2023-08-03 13:41:17.000000 delia-1.2.4/delia/extractors/patients_data_extractor.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.262036 delia-1.2.4/delia/radiomics/
+-rw-rw-rw-   0        0        0      158 2023-05-04 17:50:19.000000 delia-1.2.4/delia/radiomics/__init__.py
+-rw-rw-rw-   0        0        0    12188 2023-07-03 19:53:42.000000 delia-1.2.4/delia/radiomics/radiomics_dataset.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.263053 delia-1.2.4/delia/readers/
+-rw-rw-rw-   0        0        0       65 2022-11-08 03:03:57.000000 delia-1.2.4/delia/readers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.266046 delia-1.2.4/delia/readers/image/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.4/delia/readers/image/__init__.py
+-rw-rw-rw-   0        0        0    11258 2023-06-20 15:23:09.000000 delia-1.2.4/delia/readers/image/dicom_reader.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.273198 delia-1.2.4/delia/readers/patient_data/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.4/delia/readers/patient_data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.277198 delia-1.2.4/delia/readers/patient_data/factories/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.4/delia/readers/patient_data/factories/__init__.py
+-rw-rw-rw-   0        0        0     5110 2023-06-20 15:23:09.000000 delia-1.2.4/delia/readers/patient_data/factories/base_patient_data_factory.py
+-rw-rw-rw-   0        0        0     8102 2023-08-03 13:41:17.000000 delia-1.2.4/delia/readers/patient_data/factories/patient_data_factories.py
+-rw-rw-rw-   0        0        0     3974 2023-06-20 15:23:09.000000 delia-1.2.4/delia/readers/patient_data/patient_data_query_context.py
+-rw-rw-rw-   0        0        0      931 2023-08-03 13:41:17.000000 delia-1.2.4/delia/readers/patient_data/patient_data_query_strategy.py
+-rw-rw-rw-   0        0        0    10030 2023-06-20 15:23:09.000000 delia-1.2.4/delia/readers/patient_data/patient_data_reader.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.285437 delia-1.2.4/delia/readers/segmentation/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.4/delia/readers/segmentation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.295377 delia-1.2.4/delia/readers/segmentation/factories/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.2.4/delia/readers/segmentation/factories/__init__.py
+-rw-rw-rw-   0        0        0     2042 2022-11-08 03:20:33.000000 delia-1.2.4/delia/readers/segmentation/factories/base_segmentation_factory.py
+-rw-rw-rw-   0        0        0     6278 2022-11-08 03:20:33.000000 delia-1.2.4/delia/readers/segmentation/factories/dicom_segmentation_factories.py
+-rw-rw-rw-   0        0        0     1260 2022-07-27 14:35:42.000000 delia-1.2.4/delia/readers/segmentation/factories/segment.py
+-rw-rw-rw-   0        0        0     2830 2022-02-08 18:32:16.000000 delia-1.2.4/delia/readers/segmentation/factories/segmentation.py
+-rw-rw-rw-   0        0        0     4772 2023-05-05 16:07:22.000000 delia-1.2.4/delia/readers/segmentation/segmentation_context.py
+-rw-rw-rw-   0        0        0     2801 2023-03-16 14:44:58.000000 delia-1.2.4/delia/readers/segmentation/segmentation_reader.py
+-rw-rw-rw-   0        0        0     2217 2023-05-05 16:07:22.000000 delia-1.2.4/delia/readers/segmentation/segmentation_strategy.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.302329 delia-1.2.4/delia/transforms/
+-rw-rw-rw-   0        0        0      120 2023-03-16 15:36:25.000000 delia-1.2.4/delia/transforms/__init__.py
+-rw-rw-rw-   0        0        0    13141 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/applications.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.311428 delia-1.2.4/delia/transforms/array_space/
+-rw-rw-rw-   0        0        0      293 2023-03-16 15:36:25.000000 delia-1.2.4/delia/transforms/array_space/__init__.py
+-rw-rw-rw-   0        0        0     5085 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/array_space/matching_centroid_spatial_crop.py
+-rw-rw-rw-   0        0        0     3096 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/array_space/matching_crop_foreground.py
+-rw-rw-rw-   0        0        0     1043 2023-03-16 16:39:24.000000 delia-1.2.4/delia/transforms/array_space/tools.py
+-rw-rw-rw-   0        0        0     2544 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/array_space/transform.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.318737 delia-1.2.4/delia/transforms/data/
+-rw-rw-rw-   0        0        0      115 2023-03-16 15:36:25.000000 delia-1.2.4/delia/transforms/data/__init__.py
+-rw-rw-rw-   0        0        0     4558 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/data/copy_segmentations.py
+-rw-rw-rw-   0        0        0     1864 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/data/transform.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.328653 delia-1.2.4/delia/transforms/physical_space/
+-rw-rw-rw-   0        0        0      269 2023-03-27 00:27:35.000000 delia-1.2.4/delia/transforms/physical_space/__init__.py
+-rw-rw-rw-   0        0        0     3360 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/physical_space/matching_resample.py
+-rw-rw-rw-   0        0        0     9808 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/physical_space/pet_to_suv.py
+-rw-rw-rw-   0        0        0     3694 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/physical_space/resample.py
+-rw-rw-rw-   0        0        0     2992 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/physical_space/transform.py
+-rw-rw-rw-   0        0        0     2403 2023-06-20 15:23:09.000000 delia-1.2.4/delia/transforms/tools.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.338445 delia-1.2.4/delia/utils/
+-rw-rw-rw-   0        0        0       42 2022-11-08 03:52:44.000000 delia-1.2.4/delia/utils/__init__.py
+-rw-rw-rw-   0        0        0     4101 2023-03-16 14:44:58.000000 delia-1.2.4/delia/utils/data_model.py
+-rw-rw-rw-   0        0        0     1329 2022-03-25 22:07:08.000000 delia-1.2.4/delia/utils/tools.py
+-rw-rw-rw-   0        0        0     2131 2022-11-08 03:00:14.000000 delia-1.2.4/delia/utils/transforms_history.py
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.255356 delia-1.2.4/delia.egg-info/
+-rw-rw-rw-   0        0        0    15339 2023-08-03 13:46:09.000000 delia-1.2.4/delia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2252 2023-08-03 13:46:09.000000 delia-1.2.4/delia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 13:46:09.000000 delia-1.2.4/delia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-08-03 13:46:09.000000 delia-1.2.4/delia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-03 13:46:09.000000 delia-1.2.4/delia.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 13:46:09.349277 delia-1.2.4/examples/
+-rw-rw-rw-   0        0        0       38 2022-03-26 17:30:16.000000 delia-1.2.4/examples/__init__.py
+-rw-rw-rw-   0        0        0      712 2022-03-29 17:53:18.000000 delia-1.2.4/examples/env_examples.py
+-rw-rw-rw-   0        0        0     3474 2023-08-03 13:41:17.000000 delia-1.2.4/examples/ex01.py
+-rw-rw-rw-   0        0        0     3119 2023-08-03 13:41:17.000000 delia-1.2.4/examples/ex02.py
+-rw-rw-rw-   0        0        0     2760 2023-08-03 13:41:17.000000 delia-1.2.4/examples/ex03.py
+-rw-rw-rw-   0        0        0     5382 2023-08-03 13:41:17.000000 delia-1.2.4/examples/ex04.py
+-rw-rw-rw-   0        0        0      108 2022-01-10 21:30:41.000000 delia-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 13:46:09.351452 delia-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2023-08-03 13:45:17.000000 delia-1.2.4/setup.py
```

### Comparing `delia-1.2.3/LICENSE` & `delia-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/PKG-INFO` & `delia-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delia
-Version: 1.2.3
+Version: 1.2.4
 Summary: DICOM Extraction for Large-scale Image Analysis (DELIA).
 Home-page: https://github.com/MaxenceLarose/delia
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: dicom hdf5 medical image segmentation pre-processing python3 radiomics deep-learning dicom-seg rt-struct
 Classifier: Programming Language :: Python :: 3
```

### Comparing `delia-1.2.3/README.md` & `delia-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/__init__.py` & `delia-1.2.4/delia/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 from .utils import PatientDataModel
 
 stream_handler = logging.StreamHandler()
 stream_handler.setLevel(logging.WARNING)
 logging.getLogger(__name__).addHandler(stream_handler)
 
 __author__ = "Maxence Larose"
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 __copyright__ = "Copyright 2022, Maxence Larose"
 __credits__ = ["Maxence Larose"]
 __license__ = "Apache License 2.0"
 __maintainer__ = "Maxence Larose"
 __email__ = "maxence.larose.1@ulaval.ca"
 __status__ = "Production"
```

### Comparing `delia-1.2.3/delia/databases/patients_database.py` & `delia-1.2.4/delia/databases/patients_database.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/extractors/patients_data_extractor.py` & `delia-1.2.4/delia/extractors/patients_data_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,30 +39,29 @@
     A class used to iterate on multiple patients' dicom files and segmentation files using the PatientDataReader to
     obtain all patients' data. The PatientsDataGenerator inherits from the Generator abstract class.
     """
 
     def __init__(
             self,
             path_to_patients_folder: str,
-            tag: Union[str, Tuple[int, int]] = "SeriesDescription",
+            tag: Union[str, Tuple[int, int]] = "Modality",
             tag_values: Optional[Union[str, Dict[str, List[str]]]] = None,
             transforms: Optional[Union[Compose, DataTransform, MonaiMapTransform, PhysicalSpaceTransform]] = None,
             erase_unused_dicom_files: bool = False
     ) -> None:
         """
         Used to get the paths to the images and segmentations folders. Also used to check if either the tag values or
         the path to the tag value json dictionary is None.
 
         Parameters
         ----------
         path_to_patients_folder : str
             The path to the folder that contains all the patients' folders.
-        tag : Union[str, Tuple[int, int]] = "SeriesDescription"
-            Keyword or tuple of the DICOM tag to use while selecting which files to extract. Uses SeriesDescription
-            as a default.
+        tag : Union[str, Tuple[int, int]] = "Modality"
+            Keyword or tuple of the DICOM tag to use while selecting which files to extract. Uses Modality as a default.
         tag_values : Optional[Union[str, Dict[str, List[str]]]], default = None.
             A dictionary that contains the desired tag's values for the images that absolutely needs to be extracted
             from the patient's file. Keys are arbitrary names given to the images we want to add and values are lists of
             values associated with the specified tag. The images associated with these values do not need to have a
             corresponding segmentation. Note that it can be specified as a path to a json dictionary that contains the
             desired values for the tag.
         transforms : Union[Compose, DataTransform, MonaiMapTransform, PhysicalSpaceTransform]
```

### Comparing `delia-1.2.3/delia/radiomics/radiomics_dataset.py` & `delia-1.2.4/delia/radiomics/radiomics_dataset.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/readers/image/dicom_reader.py` & `delia-1.2.4/delia/readers/image/dicom_reader.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/readers/patient_data/factories/base_patient_data_factory.py` & `delia-1.2.4/delia/readers/patient_data/factories/base_patient_data_factory.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/readers/patient_data/factories/patient_data_factories.py` & `delia-1.2.4/delia/readers/patient_data/factories/patient_data_factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,30 +93,30 @@
         patient_data = PatientDataModel(
             patient_id=self.patient_id,
             data=data
         )
         return patient_data
 
 
-class SeriesDescriptionPatientDataFactory(BasePatientDataFactory):
+class SpecificTagPatientDataFactory(BasePatientDataFactory):
     """
     Class that defines the methods that are used to get the patient data. The tag value patient data factory
     consists in obtaining only the images that have the given tag's desired value and their corresponding segmentations.
     """
 
     def __init__(
             self,
             path_to_patient_folder: str,
             paths_to_segmentations: Optional[List[str]],
             tag_values: Optional[Dict[str, List[str]]],
             tag: Union[str, Tuple[int, int]],
             erase_unused_dicom_files: bool = False
     ):
         """
-        Constructor of the class SeriesDescriptionPatientDataFactory.
+        Constructor of the class SpecificTagPatientDataFactory.
 
         Parameters
         ----------
         path_to_patient_folder : str
             Path to the folder containing the patient's image files.
         paths_to_segmentations : Optional[List[str]]
             List of paths to the patient's segmentation files.
```

### Comparing `delia-1.2.3/delia/readers/patient_data/patient_data_query_context.py` & `delia-1.2.4/delia/readers/patient_data/patient_data_query_context.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/readers/patient_data/patient_data_query_strategy.py` & `delia-1.2.4/delia/readers/patient_data/patient_data_query_strategy.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     @Description:       This file contains the class PatientDataQueryStrategies that enumerates the available categories
                         for the queries a user can make to obtain a patient's data.
 """
 
 from enum import Enum
 from typing import NamedTuple, Callable
 
-from .factories.patient_data_factories import DefaultPatientDataFactory, SeriesDescriptionPatientDataFactory
+from .factories.patient_data_factories import DefaultPatientDataFactory, SpecificTagPatientDataFactory
 
 
 class PatientDataQueryStrategy(NamedTuple):
     name: str
     factory: Callable
 
 
@@ -25,9 +25,9 @@
     DEFAULT = PatientDataQueryStrategy(
         name="Default",
         factory=DefaultPatientDataFactory
     )
 
     TAG_VALUE = PatientDataQueryStrategy(
         name="Tag value",
-        factory=SeriesDescriptionPatientDataFactory
+        factory=SpecificTagPatientDataFactory
     )
```

### Comparing `delia-1.2.3/delia/readers/patient_data/patient_data_reader.py` & `delia-1.2.4/delia/readers/patient_data/patient_data_reader.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/readers/segmentation/factories/base_segmentation_factory.py` & `delia-1.2.4/delia/readers/segmentation/factories/base_segmentation_factory.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/readers/segmentation/factories/dicom_segmentation_factories.py` & `delia-1.2.4/delia/readers/segmentation/factories/dicom_segmentation_factories.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/readers/segmentation/factories/segment.py` & `delia-1.2.4/delia/readers/segmentation/factories/segment.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/readers/segmentation/factories/segmentation.py` & `delia-1.2.4/delia/readers/segmentation/factories/segmentation.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/readers/segmentation/segmentation_context.py` & `delia-1.2.4/delia/readers/segmentation/segmentation_context.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/readers/segmentation/segmentation_reader.py` & `delia-1.2.4/delia/readers/segmentation/segmentation_reader.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/readers/segmentation/segmentation_strategy.py` & `delia-1.2.4/delia/readers/segmentation/segmentation_strategy.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/transforms/applications.py` & `delia-1.2.4/delia/transforms/applications.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/transforms/array_space/matching_centroid_spatial_crop.py` & `delia-1.2.4/delia/transforms/array_space/matching_centroid_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/transforms/array_space/matching_crop_foreground.py` & `delia-1.2.4/delia/transforms/array_space/matching_crop_foreground.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/transforms/array_space/tools.py` & `delia-1.2.4/delia/transforms/array_space/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/transforms/array_space/transform.py` & `delia-1.2.4/delia/transforms/array_space/transform.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/transforms/data/copy_segmentations.py` & `delia-1.2.4/delia/transforms/data/copy_segmentations.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/transforms/data/transform.py` & `delia-1.2.4/delia/transforms/data/transform.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/transforms/physical_space/matching_resample.py` & `delia-1.2.4/delia/transforms/physical_space/matching_resample.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/transforms/physical_space/pet_to_suv.py` & `delia-1.2.4/delia/transforms/physical_space/pet_to_suv.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/transforms/physical_space/resample.py` & `delia-1.2.4/delia/transforms/physical_space/resample.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/transforms/physical_space/transform.py` & `delia-1.2.4/delia/transforms/physical_space/transform.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/transforms/tools.py` & `delia-1.2.4/delia/transforms/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/utils/data_model.py` & `delia-1.2.4/delia/utils/data_model.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/utils/tools.py` & `delia-1.2.4/delia/utils/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia/utils/transforms_history.py` & `delia-1.2.4/delia/utils/transforms_history.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/delia.egg-info/PKG-INFO` & `delia-1.2.4/delia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delia
-Version: 1.2.3
+Version: 1.2.4
 Summary: DICOM Extraction for Large-scale Image Analysis (DELIA).
 Home-page: https://github.com/MaxenceLarose/delia
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: dicom hdf5 medical image segmentation pre-processing python3 radiomics deep-learning dicom-seg rt-struct
 Classifier: Programming Language :: Python :: 3
```

### Comparing `delia-1.2.3/delia.egg-info/SOURCES.txt` & `delia-1.2.4/delia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/examples/env_examples.py` & `delia-1.2.4/examples/env_examples.py`

 * *Files identical despite different names*

### Comparing `delia-1.2.3/examples/ex01.py` & `delia-1.2.4/examples/ex01.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     env_examples.configure_logging("logging_conf.yaml")
 
     # ----------------------------------------------------------------------------------------------------------- #
     #                                      Create patients data extractor                                         #
     # ----------------------------------------------------------------------------------------------------------- #
     patients_data_extractor = PatientsDataExtractor(
         path_to_patients_folder="data/patients",
+        tag="SeriesDescription",
         tag_values="data/tag_values.json",
         transforms=Compose(
             [
                 ResampleD(keys=["CT_THORAX", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
                 MatchingCentroidSpatialCropD(
                     segmentation_key="Heart",
                     matching_keys=["CT_THORAX"],
```

### Comparing `delia-1.2.3/examples/ex02.py` & `delia-1.2.4/examples/ex02.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     env_examples.configure_logging("logging_conf.yaml")
 
     # ----------------------------------------------------------------------------------------------------------- #
     #                                      Create patients data extractor                                         #
     # ----------------------------------------------------------------------------------------------------------- #
     patients_data_extractor = PatientsDataExtractor(
         path_to_patients_folder="data/patients",
+        tag="SeriesDescription",
         tag_values="data/radiomics_tag_values.json",
         transforms=Compose(
             [
                 PETtoSUVD(keys=["PT"]),
                 CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="PT")
             ]
         )
```

### Comparing `delia-1.2.3/examples/ex03.py` & `delia-1.2.4/examples/ex03.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     env_examples.configure_logging("logging_conf.yaml")
 
     # ----------------------------------------------------------------------------------------------------------- #
     #                                      Create patients data extractor                                         #
     # ----------------------------------------------------------------------------------------------------------- #
     patients_data_extractor = PatientsDataExtractor(
         path_to_patients_folder="data/patients",
+        tag="SeriesDescription",
         tag_values="data/tag_values.json",
         transforms=Compose(
             [
                 ResampleD(keys=["CT_THORAX", "PT", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
                 MatchingResampleD(reference_image_key="CT_THORAX", matching_keys=["PT", "Heart"]),
                 CenterSpatialCropD(keys=["CT_THORAX", "PT", "Heart"], roi_size=(1000, 160, 160)),
                 ScaleIntensityRangeD(keys=["CT_THORAX"], a_min=-250, a_max=500, b_min=0, b_max=1, clip=True),
```

### Comparing `delia-1.2.3/examples/ex04.py` & `delia-1.2.4/examples/ex04.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 if __name__ == "__main__":
     # ----------------------------------------------------------------------------------------------------------- #
     #     Create database (some images of some patients might fail to be added to the database due to the         #
     #                               absence of the tag value in the patient record)                               #
     # ----------------------------------------------------------------------------------------------------------- #
     patients_data_extractor = PatientsDataExtractor(
         path_to_patients_folder="data/patients",
+        tag="SeriesDescription",
         tag_values="data/incorrect_tag_values.json"
     )
 
     database = PatientsDatabase(path_to_database="data/patients_database.h5")
 
     patients_who_failed = database.create(
         patients_data_extractor=patients_data_extractor,
```

### Comparing `delia-1.2.3/setup.py` & `delia-1.2.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="delia",
-    version="1.2.3",
+    version="1.2.4",
     author="Maxence Larose",
     author_email="maxence.larose.1@ulaval.ca",
     description="DICOM Extraction for Large-scale Image Analysis (DELIA).",
     long_description=open('README.md', "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/MaxenceLarose/delia",
     license="Apache License 2.0",
```

