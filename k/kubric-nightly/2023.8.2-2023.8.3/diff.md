# Comparing `tmp/kubric-nightly-2023.8.2.tar.gz` & `tmp/kubric-nightly-2023.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kubric-nightly-2023.8.2.tar", last modified: Wed Aug  2 00:34:40 2023, max compression
+gzip compressed data, was "dist/kubric-nightly-2023.8.3.tar", last modified: Thu Aug  3 00:47:51 2023, max compression
```

## Comparing `kubric-nightly-2023.8.2.tar` & `kubric-nightly-2023.8.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:34:40.000000 kubric-nightly-2023.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-02 00:34:40.000000 kubric-nightly-2023.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:34:39.000000 kubric-nightly-2023.8.2/kubric/
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-02 00:34:39.000000 kubric-nightly-2023.8.2/kubric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:34:39.000000 kubric-nightly-2023.8.2/kubric/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/assets/asset_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/assets/asset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/assets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:34:40.000000 kubric-nightly-2023.8.2/kubric/core/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/core/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/core/cameras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/core/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/core/lights.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/core/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/core/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/core/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/core/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/core/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:34:40.000000 kubric-nightly-2023.8.2/kubric/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/datasets/movid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/kubric_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/randomness.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/redirect_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:34:40.000000 kubric-nightly-2023.8.2/kubric/renderer/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36278 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/renderer/blender.py
--rw-r--r--   0 runner    (1001) docker     (123)    18525 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/renderer/blender_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:34:40.000000 kubric-nightly-2023.8.2/kubric/safeimport/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/safeimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/safeimport/bpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:34:40.000000 kubric-nightly-2023.8.2/kubric/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/simulator/pybullet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:34:40.000000 kubric-nightly-2023.8.2/kubric/sunds/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/sunds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/sunds/kubric_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/sunds/kubric_builder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/sunds/render_mock_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/kubric/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:34:40.000000 kubric-nightly-2023.8.2/kubric_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-02 00:34:39.000000 kubric-nightly-2023.8.2/kubric_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-02 00:34:39.000000 kubric-nightly-2023.8.2/kubric_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:34:39.000000 kubric-nightly-2023.8.2/kubric_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-02 00:34:39.000000 kubric-nightly-2023.8.2/kubric_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 00:34:39.000000 kubric-nightly-2023.8.2/kubric_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:34:40.000000 kubric-nightly-2023.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:34:40.000000 kubric-nightly-2023.8.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/test/test_blender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/test/test_cameras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/test/test_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/test/test_fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/test/test_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/test/test_pybullet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/test/test_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-08-02 00:34:21.000000 kubric-nightly-2023.8.2/test/test_traits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric/
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/assets/asset_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/assets/asset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/assets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/core/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/core/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/core/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/core/lights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/core/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/core/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/core/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/core/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/core/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/datasets/movid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/kubric_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/randomness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/redirect_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric/renderer/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36278 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/renderer/blender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18525 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/renderer/blender_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric/safeimport/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/safeimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/safeimport/bpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/simulator/pybullet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric/sunds/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/sunds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/sunds/kubric_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/sunds/kubric_builder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/sunds/render_mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/kubric/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/kubric_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:47:51.000000 kubric-nightly-2023.8.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/test/test_blender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/test/test_cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/test/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/test/test_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/test/test_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/test/test_pybullet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/test/test_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-08-03 00:47:29.000000 kubric-nightly-2023.8.3/test/test_traits.py
```

### Comparing `kubric-nightly-2023.8.2/LICENSE` & `kubric-nightly-2023.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/PKG-INFO` & `kubric-nightly-2023.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubric-nightly
-Version: 2023.8.2
+Version: 2023.8.3
 Summary: A data generation pipeline for creating semi-realistic synthetic multi-object videos with rich annotations such as instance segmentation, depth maps, and optical flow.
 Home-page: https://github.com/google-research/kubric
 Author: Kubric team
 Author-email: kubric+dev@google.com
 License: Apache 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kubric-nightly-2023.8.2/README.md` & `kubric-nightly-2023.8.3/README.md`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/__init__.py` & `kubric-nightly-2023.8.3/kubric/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Root of the kubric module."""
 
 # --- auto-computed by setup.py, source version is always at HEAD
-__version__ = "2023.8.2"
+__version__ = "2023.8.3"
 
 # --- basic kubric types
 from pyquaternion import Quaternion
 
 from kubric.core.scene import Scene
 
 from kubric.core.assets import Asset
```

### Comparing `kubric-nightly-2023.8.2/kubric/assets/__init__.py` & `kubric-nightly-2023.8.3/kubric/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/assets/asset_preprocessing.py` & `kubric-nightly-2023.8.3/kubric/assets/asset_preprocessing.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/assets/asset_source.py` & `kubric-nightly-2023.8.3/kubric/assets/asset_source.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/assets/utils.py` & `kubric-nightly-2023.8.3/kubric/assets/utils.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/core/__init__.py` & `kubric-nightly-2023.8.3/kubric/core/__init__.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/core/assets.py` & `kubric-nightly-2023.8.3/kubric/core/assets.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/core/cameras.py` & `kubric-nightly-2023.8.3/kubric/core/cameras.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/core/color.py` & `kubric-nightly-2023.8.3/kubric/core/color.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/core/lights.py` & `kubric-nightly-2023.8.3/kubric/core/lights.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/core/materials.py` & `kubric-nightly-2023.8.3/kubric/core/materials.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/core/objects.py` & `kubric-nightly-2023.8.3/kubric/core/objects.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/core/scene.py` & `kubric-nightly-2023.8.3/kubric/core/scene.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/core/traits.py` & `kubric-nightly-2023.8.3/kubric/core/traits.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/core/view.py` & `kubric-nightly-2023.8.3/kubric/core/view.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/datasets/__init__.py` & `kubric-nightly-2023.8.3/kubric/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/datasets/utils.py` & `kubric-nightly-2023.8.3/kubric/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/file_io.py` & `kubric-nightly-2023.8.3/kubric/file_io.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/kubric_typing.py` & `kubric-nightly-2023.8.3/kubric/kubric_typing.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/plotting.py` & `kubric-nightly-2023.8.3/kubric/plotting.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/post_processing.py` & `kubric-nightly-2023.8.3/kubric/post_processing.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/randomness.py` & `kubric-nightly-2023.8.3/kubric/randomness.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/redirect_io.py` & `kubric-nightly-2023.8.3/kubric/redirect_io.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/renderer/__init__.py` & `kubric-nightly-2023.8.3/kubric/renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/renderer/blender.py` & `kubric-nightly-2023.8.3/kubric/renderer/blender.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/renderer/blender_utils.py` & `kubric-nightly-2023.8.3/kubric/renderer/blender_utils.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/safeimport/__init__.py` & `kubric-nightly-2023.8.3/kubric/safeimport/__init__.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/safeimport/bpy.py` & `kubric-nightly-2023.8.3/kubric/safeimport/bpy.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/simulator/__init__.py` & `kubric-nightly-2023.8.3/kubric/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/simulator/pybullet.py` & `kubric-nightly-2023.8.3/kubric/simulator/pybullet.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/sunds/__init__.py` & `kubric-nightly-2023.8.3/kubric/sunds/__init__.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/sunds/kubric_builder.py` & `kubric-nightly-2023.8.3/kubric/sunds/kubric_builder.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/sunds/kubric_builder_test.py` & `kubric-nightly-2023.8.3/kubric/sunds/kubric_builder_test.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/sunds/render_mock_utils.py` & `kubric-nightly-2023.8.3/kubric/sunds/render_mock_utils.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric/utils.py` & `kubric-nightly-2023.8.3/kubric/utils.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/kubric_nightly.egg-info/PKG-INFO` & `kubric-nightly-2023.8.3/kubric_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubric-nightly
-Version: 2023.8.2
+Version: 2023.8.3
 Summary: A data generation pipeline for creating semi-realistic synthetic multi-object videos with rich annotations such as instance segmentation, depth maps, and optical flow.
 Home-page: https://github.com/google-research/kubric
 Author: Kubric team
 Author-email: kubric+dev@google.com
 License: Apache 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kubric-nightly-2023.8.2/kubric_nightly.egg-info/SOURCES.txt` & `kubric-nightly-2023.8.3/kubric_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/setup.py` & `kubric-nightly-2023.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/test/__init__.py` & `kubric-nightly-2023.8.3/test/__init__.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/test/test_blender.py` & `kubric-nightly-2023.8.3/test/test_blender.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/test/test_cameras.py` & `kubric-nightly-2023.8.3/test/test_cameras.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/test/test_color.py` & `kubric-nightly-2023.8.3/test/test_color.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/test/test_core.py` & `kubric-nightly-2023.8.3/test/test_core.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/test/test_fileio.py` & `kubric-nightly-2023.8.3/test/test_fileio.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/test/test_postprocessing.py` & `kubric-nightly-2023.8.3/test/test_postprocessing.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/test/test_pybullet.py` & `kubric-nightly-2023.8.3/test/test_pybullet.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/test/test_scene.py` & `kubric-nightly-2023.8.3/test/test_scene.py`

 * *Files identical despite different names*

### Comparing `kubric-nightly-2023.8.2/test/test_traits.py` & `kubric-nightly-2023.8.3/test/test_traits.py`

 * *Files identical despite different names*

