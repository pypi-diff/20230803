# Comparing `tmp/scale_sensor_fusion_io-0.3.0.tar.gz` & `tmp/scale_sensor_fusion_io-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_sensor_fusion_io-0.3.0.tar", max compression
+gzip compressed data, was "scale_sensor_fusion_io-0.3.2.tar", max compression
```

## Comparing `scale_sensor_fusion_io-0.3.0.tar` & `scale_sensor_fusion_io-0.3.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     2945 2023-05-25 18:02:56.996415 scale_sensor_fusion_io-0.3.0/docs/README.md
--rw-r--r--   0        0        0     1045 2023-07-06 20:12:32.471813 scale_sensor_fusion_io-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       98 2023-05-25 18:02:56.996415 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/__init__.py
--rw-r--r--   0        0        0       52 2023-04-21 17:25:32.493004 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/loaders/__init__.py
--rw-r--r--   0        0        0     2716 2023-05-04 20:10:30.275131 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/loaders/bs5_loader.py
--rw-r--r--   0        0        0     3088 2023-05-25 18:02:56.996415 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/loaders/sfs_loader.py
--rw-r--r--   0        0        0       19 2023-05-25 18:02:56.996415 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/model_converters/__init__.py
--rw-r--r--   0        0        0     8163 2023-06-02 18:09:01.052673 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/model_converters/sfs.py
--rw-r--r--   0        0        0     3349 2023-06-13 19:55:58.611076 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/Pose.py
--rw-r--r--   0        0        0       96 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/__init__.py
--rw-r--r--   0        0        0      456 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/__init__.py
--rw-r--r--   0        0        0      512 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/attributes.py
--rw-r--r--   0        0        0      626 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/box_2d.py
--rw-r--r--   0        0        0     1129 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/cuboid.py
--rw-r--r--   0        0        0      520 2023-05-05 15:35:42.316417 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/event.py
--rw-r--r--   0        0        0      690 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/labeled_points.py
--rw-r--r--   0        0        0      924 2023-05-09 02:31:38.889679 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/localization_adjustment.py
--rw-r--r--   0        0        0      425 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/object.py
--rw-r--r--   0        0        0      638 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/polygon.py
--rw-r--r--   0        0        0      509 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/common.py
--rw-r--r--   0        0        0      109 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/paths/__init__.py
--rw-r--r--   0        0        0      291 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/paths/attribute_path.py
--rw-r--r--   0        0        0     5350 2023-05-01 16:05:39.349378 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/paths/cuboid_path.py
--rw-r--r--   0        0        0    16186 2023-06-14 08:40:18.734552 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/paths/pose_path.py
--rw-r--r--   0        0        0      577 2023-05-25 18:02:56.996415 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/scene.py
--rw-r--r--   0        0        0      253 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/sensors/__init__.py
--rw-r--r--   0        0        0       94 2023-04-19 22:28:02.352690 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/sensors/camera/__init__.py
--rw-r--r--   0        0        0     6801 2023-07-06 20:12:32.471813 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py
--rw-r--r--   0        0        0      310 2023-05-09 20:54:40.857630 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/sensors/camera/camera_intrinsics.py
--rw-r--r--   0        0        0      896 2023-05-09 20:55:12.405738 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py
--rw-r--r--   0        0        0       27 2023-04-19 22:28:02.352690 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/sensors/lidar/__init__.py
--rw-r--r--   0        0        0      931 2023-05-05 15:35:42.316417 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py
--rw-r--r--   0        0        0       28 2023-04-19 22:28:02.352690 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/sensors/radar/__init__.py
--rw-r--r--   0        0        0      825 2023-05-09 21:28:41.008175 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py
--rw-r--r--   0        0        0        0 2023-03-31 01:21:32.524089 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/py.typed
--rw-r--r--   0        0        0       91 2023-05-04 20:10:30.275131 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/spec/__init__.py
--rw-r--r--   0        0        0       21 2023-04-21 17:25:32.513004 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/spec/sfs/__init__.py
--rw-r--r--   0        0        0     9688 2023-06-21 00:38:30.739386 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/spec/sfs/types.py
--rw-r--r--   0        0        0       21 2023-04-21 17:25:32.513004 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/spec/v5/__init__.py
--rw-r--r--   0        0        0     3605 2023-06-14 08:41:24.950160 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/spec/v5/types.py
--rw-r--r--   0        0        0        0 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/utils/__init__.py
--rw-r--r--   0        0        0     2005 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/utils/downsample.py
--rw-r--r--   0        0        0     2943 2023-07-06 20:12:32.471813 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/utils/generate_video.py
--rw-r--r--   0        0        0      899 2023-05-25 18:02:56.996415 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/__init__.py
--rw-r--r--   0        0        0     1069 2023-05-25 18:02:56.996415 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/dacite_internal/LICENSE
--rw-r--r--   0        0        0      297 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/dacite_internal/README.md
--rw-r--r--   0        0        0      135 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/dacite_internal/__init__.py
--rw-r--r--   0        0        0      502 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/dacite_internal/config.py
--rw-r--r--   0        0        0     7388 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/dacite_internal/core.py
--rw-r--r--   0        0        0       90 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/dacite_internal/data.py
--rw-r--r--   0        0        0     1121 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py
--rw-r--r--   0        0        0     2949 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py
--rw-r--r--   0        0        0     8189 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/dacite_internal/types.py
--rw-r--r--   0        0        0     2802 2023-06-01 00:34:19.596311 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/error.py
--rw-r--r--   0        0        0      965 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/helpers.py
--rw-r--r--   0        0        0       19 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/parser/__init__.py
--rw-r--r--   0        0        0     7530 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/parser/sfs.py
--rw-r--r--   0        0        0     9584 2023-06-05 17:16:28.436716 scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/validate.py
--rw-r--r--   0        0        0     4023 1970-01-01 00:00:00.000000 scale_sensor_fusion_io-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3072 2023-08-01 23:14:45.423354 scale_sensor_fusion_io-0.3.2/docs/README.md
+-rw-r--r--   0        0        0     1045 2023-08-02 00:18:46.454315 scale_sensor_fusion_io-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-25 07:12:37.457890 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/loaders/__init__.py
+-rw-r--r--   0        0        0     2716 2023-05-22 20:30:40.190095 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/loaders/bs5_loader.py
+-rw-r--r--   0        0        0     3088 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/loaders/sfs_loader.py
+-rw-r--r--   0        0        0       19 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/model_converters/__init__.py
+-rw-r--r--   0        0        0     8163 2023-06-13 16:18:43.797315 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/model_converters/sfs.py
+-rw-r--r--   0        0        0     3349 2023-06-14 02:05:19.522216 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/Pose.py
+-rw-r--r--   0        0        0       96 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/__init__.py
+-rw-r--r--   0        0        0      456 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/__init__.py
+-rw-r--r--   0        0        0      512 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/attributes.py
+-rw-r--r--   0        0        0      626 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/box_2d.py
+-rw-r--r--   0        0        0     1129 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/cuboid.py
+-rw-r--r--   0        0        0      520 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/event.py
+-rw-r--r--   0        0        0      690 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/labeled_points.py
+-rw-r--r--   0        0        0      924 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/localization_adjustment.py
+-rw-r--r--   0        0        0      425 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/object.py
+-rw-r--r--   0        0        0      638 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/polygon.py
+-rw-r--r--   0        0        0      509 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/common.py
+-rw-r--r--   0        0        0      109 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/paths/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/paths/attribute_path.py
+-rw-r--r--   0        0        0     5350 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/paths/cuboid_path.py
+-rw-r--r--   0        0        0    16186 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/paths/pose_path.py
+-rw-r--r--   0        0        0      577 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/scene.py
+-rw-r--r--   0        0        0      253 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/sensors/__init__.py
+-rw-r--r--   0        0        0       94 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/sensors/camera/__init__.py
+-rw-r--r--   0        0        0     6801 2023-07-03 23:35:23.070551 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py
+-rw-r--r--   0        0        0      310 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/sensors/camera/camera_intrinsics.py
+-rw-r--r--   0        0        0      896 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py
+-rw-r--r--   0        0        0       27 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/sensors/lidar/__init__.py
+-rw-r--r--   0        0        0      931 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py
+-rw-r--r--   0        0        0       28 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/sensors/radar/__init__.py
+-rw-r--r--   0        0        0      825 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py
+-rw-r--r--   0        0        0        0 2023-03-29 20:56:32.935581 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/py.typed
+-rw-r--r--   0        0        0       91 2023-05-22 20:08:31.172592 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/spec/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/spec/sfs/__init__.py
+-rw-r--r--   0        0        0     9688 2023-07-03 23:35:23.070551 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/spec/sfs/types.py
+-rw-r--r--   0        0        0       21 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/spec/v5/__init__.py
+-rw-r--r--   0        0        0     3605 2023-06-14 02:05:19.526217 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/spec/v5/types.py
+-rw-r--r--   0        0        0        0 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/utils/__init__.py
+-rw-r--r--   0        0        0     2005 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/utils/downsample.py
+-rw-r--r--   0        0        0     2943 2023-07-03 23:35:23.070551 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/utils/generate_video.py
+-rw-r--r--   0        0        0      899 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/__init__.py
+-rw-r--r--   0        0        0     1069 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/dacite_internal/LICENSE
+-rw-r--r--   0        0        0      297 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/dacite_internal/README.md
+-rw-r--r--   0        0        0      135 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/dacite_internal/__init__.py
+-rw-r--r--   0        0        0      502 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/dacite_internal/config.py
+-rw-r--r--   0        0        0     7388 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/dacite_internal/core.py
+-rw-r--r--   0        0        0       90 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/dacite_internal/data.py
+-rw-r--r--   0        0        0     1121 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py
+-rw-r--r--   0        0        0     2949 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py
+-rw-r--r--   0        0        0     8189 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/dacite_internal/types.py
+-rw-r--r--   0        0        0     2802 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/error.py
+-rw-r--r--   0        0        0      955 2023-07-13 18:49:50.122338 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/helpers.py
+-rw-r--r--   0        0        0       19 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/parser/__init__.py
+-rw-r--r--   0        0        0     7525 2023-07-13 18:49:50.122338 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/parser/sfs.py
+-rw-r--r--   0        0        0     9574 2023-07-13 18:49:50.122338 scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/validate.py
+-rw-r--r--   0        0        0     4150 1970-01-01 00:00:00.000000 scale_sensor_fusion_io-0.3.2/PKG-INFO
```

### Comparing `scale_sensor_fusion_io-0.3.0/docs/README.md` & `scale_sensor_fusion_io-0.3.2/docs/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 
 ## Requirements
 
 Minimum Python version supported is 3.8.
 
 # Code samples
 
+## End-to-End Example From PandaSet
+
+[Here](examples/pandas_to_sfs_conversion.ipynb) is a link to a Jupyter notebook example.
+
 ## Constructing an SFS scene
 
 ### PosePath Dataframe
 
 ## Encoding a SFS scene
 
 ```
```

### Comparing `scale_sensor_fusion_io-0.3.0/pyproject.toml` & `scale_sensor_fusion_io-0.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scale_sensor_fusion_io"
-version = "0.3.0"
+version = "0.3.2"
 description = "Library for working with timestamp-based sensor fusion scenes"
 authors = [
     "Michael Choi <michael.choi@scale.com>",
     "Rodrigo Belfiore <rodrigo.belfiore@scale.com>"
 ]
 readme = ["docs/README.md"]
```

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/loaders/bs5_loader.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/loaders/bs5_loader.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/loaders/sfs_loader.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/loaders/sfs_loader.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/model_converters/sfs.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/model_converters/sfs.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/Pose.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/Pose.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/attributes.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/attributes.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/box_2d.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/box_2d.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/cuboid.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/cuboid.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/event.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/event.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/labeled_points.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/labeled_points.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/localization_adjustment.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/localization_adjustment.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/annotations/polygon.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/annotations/polygon.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/paths/cuboid_path.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/paths/cuboid_path.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/paths/pose_path.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/paths/pose_path.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/scene.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/scene.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/spec/sfs/types.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/spec/sfs/types.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/spec/v5/types.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/spec/v5/types.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/utils/downsample.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/utils/downsample.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/utils/generate_video.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/utils/generate_video.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/__init__.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/dacite_internal/LICENSE` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/dacite_internal/LICENSE`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/dacite_internal/core.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/dacite_internal/core.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/dacite_internal/types.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/dacite_internal/types.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/error.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/error.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/helpers.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,10 +26,10 @@
     except dacite.AggregatedError as e:
         error_details.extend([convert_error(err) for err in e.errors])
     except dacite.DaciteFieldError as e:
         error_details.append(convert_error(e))
     return None
 
 
-def is_monotonically_increasing(ts: List[int]) -> bool:
-    """Check if a list of timestamps is monotonically increasing"""
-    return all(ts[i] <= ts[i + 1] for i in range(len(ts) - 1))
+def is_strictly_increasing(ts: List[int]) -> bool:
+    """Check if a list of timestamps is strictly increasing"""
+    return all(ts1 < ts2 for ts1, ts2 in zip(ts[:-1], ts[1:]))
```

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/parser/sfs.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/parser/sfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     ParseSuccess,
     PathField,
     ValidationResult,
 )
 from scale_sensor_fusion_io.validation.helpers import (
     convert_error,
     handle_dacite,
-    is_monotonically_increasing,
+    is_strictly_increasing,
 )
 from typing_extensions import TypeAlias
 
 CFG = _dacite.Config(cast=[Enum, tuple])
 
 _T = TypeVar("_T")
```

### Comparing `scale_sensor_fusion_io-0.3.0/scale_sensor_fusion_io/validation/validate.py` & `scale_sensor_fusion_io-0.3.2/scale_sensor_fusion_io/validation/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from .error import (
     DataValidationError,
     ErrorDetails,
     PathField,
     ValidationResult,
 )
-from .helpers import is_monotonically_increasing
+from .helpers import is_strictly_increasing
 
 MICRO_IN_SEC = 1e6
 MAX_FPS = 100
 MIN_FPS = 1
 
 
 def _handle_result(
@@ -68,15 +68,15 @@
     error_details: List[ErrorDetails] = []
     if any(ts < 0 for ts in timestamps):
         error_details.append(
             ErrorDetails.from_msg(
                 "timestamps must not be negative",
             )
         )
-    if not is_monotonically_increasing(timestamps):
+    if not is_strictly_increasing(timestamps):
         error_details.append(
             ErrorDetails.from_msg(
                 "timestamps be monotonically increasing",
             )
         )
 
     max_ts_diff = MICRO_IN_SEC / MIN_FPS
```

### Comparing `scale_sensor_fusion_io-0.3.0/PKG-INFO` & `scale_sensor_fusion_io-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-sensor-fusion-io
-Version: 0.3.0
+Version: 0.3.2
 Summary: Library for working with timestamp-based sensor fusion scenes
 Author: Michael Choi
 Author-email: michael.choi@scale.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -37,14 +37,18 @@
 
 ## Requirements
 
 Minimum Python version supported is 3.8.
 
 # Code samples
 
+## End-to-End Example From PandaSet
+
+[Here](examples/pandas_to_sfs_conversion.ipynb) is a link to a Jupyter notebook example.
+
 ## Constructing an SFS scene
 
 ### PosePath Dataframe
 
 ## Encoding a SFS scene
 
 ```
```

