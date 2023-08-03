# Comparing `tmp/anatools-3.2.2.tar.gz` & `tmp/anatools-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anatools-3.2.2.tar", last modified: Wed Jul 19 16:28:55 2023, max compression
+gzip compressed data, was "anatools-3.3.0.tar", last modified: Thu Aug  3 19:39:48 2023, max compression
```

## Comparing `anatools-3.2.2.tar` & `anatools-3.3.0.tar`

### file list

```diff
@@ -1,106 +1,108 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 16:28:55.461567 anatools-3.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-19 16:28:39.000000 anatools-3.2.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-19 16:28:39.000000 anatools-3.2.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     6975 2023-07-19 16:28:55.461567 anatools-3.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6585 2023-07-19 16:28:39.000000 anatools-3.2.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 16:28:55.449567 anatools-3.2.2/anatools/
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-07-19 16:28:41.000000 anatools-3.2.2/anatools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 16:28:55.449567 anatools-3.2.2/anatools/anaclient/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11517 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/anaclient.py
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/analytics.py
--rw-rw-rw-   0 root         (0) root         (0)    11005 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/annotations.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 16:28:55.453567 anatools-3.2.2/anatools/anaclient/api/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2910 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/analytics.py
--rw-rw-rw-   0 root         (0) root         (0)     9403 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     4510 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/api.py
--rw-rw-rw-   0 root         (0) root         (0)    10389 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/channels.py
--rw-rw-rw-   0 root         (0) root         (0)     8002 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)    10116 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/gan.py
--rw-rw-rw-   0 root         (0) root         (0)     4206 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)     1224 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     5334 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/limits.py
--rw-rw-rw-   0 root         (0) root         (0)     3974 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/members.py
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)     2489 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/umap.py
--rw-rw-rw-   0 root         (0) root         (0)     8958 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/volumes.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/api/workspaces.py
--rw-rw-rw-   0 root         (0) root         (0)    18408 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/channels.py
--rw-rw-rw-   0 root         (0) root         (0)     9203 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)     9573 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/gan.py
--rw-rw-rw-   0 root         (0) root         (0)     6300 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)     9386 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)     1936 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/umap.py
--rw-rw-rw-   0 root         (0) root         (0)    17897 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/volumes.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/anaclient/workspaces.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 16:28:55.453567 anatools-3.2.2/anatools/annotations/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/annotations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7460 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/annotations/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     3701 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/annotations/convert_coco.py
--rw-rw-rw-   0 root         (0) root         (0)     7173 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/annotations/convert_kitti.py
--rw-rw-rw-   0 root         (0) root         (0)     3381 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/annotations/convert_pascal.py
--rw-rw-rw-   0 root         (0) root         (0)     4468 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/annotations/convert_sagemaker.py
--rw-rw-rw-   0 root         (0) root         (0)     2727 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/annotations/convert_yolo.py
--rw-rw-rw-   0 root         (0) root         (0)     7548 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/annotations/draw.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 16:28:55.453567 anatools-3.2.2/anatools/bin/
--rw-rw-rw-   0 root         (0) root         (0)     4523 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/bin/ana
--rw-rw-rw-   0 root         (0) root         (0)     9659 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/bin/anadeploy
--rw-rw-rw-   0 root         (0) root         (0)     7692 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/bin/anamount
--rw-rw-rw-   0 root         (0) root         (0)     4559 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/bin/anautils
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 16:28:55.457567 anatools-3.2.2/anatools/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6974 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/ana_object.py
--rw-rw-rw-   0 root         (0) root         (0)     7114 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/bbox.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/blender_main.py
--rw-rw-rw-   0 root         (0) root         (0)     4923 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/camera_checks.py
--rw-rw-rw-   0 root         (0) root         (0)    14524 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/channel.py
--rw-rw-rw-   0 root         (0) root         (0)     1777 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/context.py
--rw-rw-rw-   0 root         (0) root         (0)     1490 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/directory_object.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/download.py
--rw-rw-rw-   0 root         (0) root         (0)     4198 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/file_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     1308 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/file_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/file_object.py
--rw-rw-rw-   0 root         (0) root         (0)     9556 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/generator.py
--rw-rw-rw-   0 root         (0) root         (0)     5670 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/interp.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/load.py
--rw-rw-rw-   0 root         (0) root         (0)    10556 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/node.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/object_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1702 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/package_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/print.py
--rw-rw-rw-   0 root         (0) root         (0)     1918 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/python_main.py
--rw-rw-rw-   0 root         (0) root         (0)     3200 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/rigged_object.py
--rw-rw-rw-   0 root         (0) root         (0)     8111 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/scene.py
--rw-rw-rw-   0 root         (0) root         (0)     3757 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/lib/search_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 16:28:55.461567 anatools-3.2.2/anatools/nodes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/constants.yml
--rw-rw-rw-   0 root         (0) root         (0)     2635 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     2183 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/generators.yml
--rw-rw-rw-   0 root         (0) root         (0)     1592 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/logic.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/logic.yml
--rw-rw-rw-   0 root         (0) root         (0)     5381 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/random_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     8429 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/random_generator.yml
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/sweep_arange.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/sweep_arange.yml
--rw-rw-rw-   0 root         (0) root         (0)     1306 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/sweep_linspace.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/sweep_linspace.yml
--rw-rw-rw-   0 root         (0) root         (0)     1224 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/vectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1922 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/vectors.yml
--rw-rw-rw-   0 root         (0) root         (0)     1246 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/volume_directory.py
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/volume_directory.yml
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/volume_file.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-07-19 16:28:39.000000 anatools-3.2.2/anatools/nodes/volume_file.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 16:28:55.449567 anatools-3.2.2/anatools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6975 2023-07-19 16:28:55.000000 anatools-3.2.2/anatools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2717 2023-07-19 16:28:55.000000 anatools-3.2.2/anatools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-19 16:28:55.000000 anatools-3.2.2/anatools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-19 16:28:55.000000 anatools-3.2.2/anatools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-07-19 16:28:55.000000 anatools-3.2.2/anatools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-19 16:28:39.000000 anatools-3.2.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-19 16:28:39.000000 anatools-3.2.2/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-19 16:28:55.461567 anatools-3.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-07-19 16:28:39.000000 anatools-3.2.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 16:28:55.461567 anatools-3.2.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)      782 2023-07-19 16:28:39.000000 anatools-3.2.2/tests/test_bbox.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 19:39:48.204125 anatools-3.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-08-03 19:39:30.000000 anatools-3.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-08-03 19:39:30.000000 anatools-3.3.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     7863 2023-08-03 19:39:48.200125 anatools-3.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7474 2023-08-03 19:39:30.000000 anatools-3.3.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 19:39:48.188125 anatools-3.3.0/anatools/
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-08-03 19:39:33.000000 anatools-3.3.0/anatools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 19:39:48.192125 anatools-3.3.0/anatools/anaclient/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14766 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/anaclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/analytics.py
+-rw-rw-rw-   0 root         (0) root         (0)    11005 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/annotations.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 19:39:48.196125 anatools-3.3.0/anatools/anaclient/api/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2910 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/analytics.py
+-rw-rw-rw-   0 root         (0) root         (0)     9403 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4612 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     3060 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/api_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    10389 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/channels.py
+-rw-rw-rw-   0 root         (0) root         (0)     8002 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)    10116 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/gan.py
+-rw-rw-rw-   0 root         (0) root         (0)     4206 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5334 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/limits.py
+-rw-rw-rw-   0 root         (0) root         (0)     3974 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/members.py
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2492 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/umap.py
+-rw-rw-rw-   0 root         (0) root         (0)     8958 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/volumes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api/workspaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/api_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    18496 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/channels.py
+-rw-rw-rw-   0 root         (0) root         (0)     9203 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)     9573 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/gan.py
+-rw-rw-rw-   0 root         (0) root         (0)     6300 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)     9639 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/umap.py
+-rw-rw-rw-   0 root         (0) root         (0)    17985 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/volumes.py
+-rw-rw-rw-   0 root         (0) root         (0)     9359 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/anaclient/workspaces.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 19:39:48.196125 anatools-3.3.0/anatools/annotations/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/annotations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7460 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/annotations/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/annotations/convert_coco.py
+-rw-rw-rw-   0 root         (0) root         (0)     7173 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/annotations/convert_kitti.py
+-rw-rw-rw-   0 root         (0) root         (0)     3381 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/annotations/convert_pascal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4468 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/annotations/convert_sagemaker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/annotations/convert_yolo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/annotations/draw.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 19:39:48.196125 anatools-3.3.0/anatools/bin/
+-rw-rw-rw-   0 root         (0) root         (0)     4523 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/bin/ana
+-rw-rw-rw-   0 root         (0) root         (0)     9659 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/bin/anadeploy
+-rw-rw-rw-   0 root         (0) root         (0)     7692 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/bin/anamount
+-rw-rw-rw-   0 root         (0) root         (0)     4559 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/bin/anautils
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 19:39:48.200125 anatools-3.3.0/anatools/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6974 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/ana_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     7114 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/bbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/blender_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     4923 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/camera_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)    14524 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1777 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/directory_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/download.py
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/file_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/file_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/file_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     9556 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5670 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/interp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/load.py
+-rw-rw-rw-   0 root         (0) root         (0)    10556 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/object_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/package_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/print.py
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/python_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3200 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/rigged_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     8111 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/scene.py
+-rw-rw-rw-   0 root         (0) root         (0)     3757 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/lib/search_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 19:39:48.200125 anatools-3.3.0/anatools/nodes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/constants.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2635 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/generators.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/logic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/logic.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5381 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/random_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8429 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/random_generator.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/sweep_arange.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/sweep_arange.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/sweep_linspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/sweep_linspace.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1922 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/vectors.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/volume_directory.py
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/volume_directory.yml
+-rw-rw-rw-   0 root         (0) root         (0)      557 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/volume_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-08-03 19:39:30.000000 anatools-3.3.0/anatools/nodes/volume_file.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 19:39:48.188125 anatools-3.3.0/anatools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     7863 2023-08-03 19:39:48.000000 anatools-3.3.0/anatools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2783 2023-08-03 19:39:48.000000 anatools-3.3.0/anatools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-08-03 19:39:48.000000 anatools-3.3.0/anatools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-08-03 19:39:48.000000 anatools-3.3.0/anatools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-08-03 19:39:48.000000 anatools-3.3.0/anatools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-08-03 19:39:30.000000 anatools-3.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-08-03 19:39:30.000000 anatools-3.3.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-08-03 19:39:48.204125 anatools-3.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-08-03 19:39:30.000000 anatools-3.3.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 19:39:48.200125 anatools-3.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-08-03 19:39:30.000000 anatools-3.3.0/tests/test_bbox.py
```

### Comparing `anatools-3.2.2/LICENSE` & `anatools-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/PKG-INFO` & `anatools-3.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anatools
-Version: 3.2.2
+Version: 3.3.0
 Summary: Tools for development with the Rendered.ai Platform.
 Home-page: https://rendered.ai
 Author: Rendered AI, Inc
 Author-email: support@rendered.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
@@ -58,14 +58,57 @@
 | pyyaml | A python YAML parser and emitter. |
 | requests | A simple HTTP python library. |
 
 If you have any questions or comments, contact Rendered.AI at info@rendered.ai.
 
 <br />
 
+## Multiple ways to login
+
+#### Login with email
+Execute the python command line, create a client and login to Rendered.ai.
+In this example we are instantiating a client with no workspace or environment variables, so it is setting our default workspace.
+To access the tool, you will need to use your email and password for https://deckard.rendered.ai.
+```python
+>>> import anatools
+>>> ana = anatools.client()
+'Enter your credentials for the Rendered.ai Platform.'
+'email:' example@rendered.ai
+'password:' ***************
+```
+
+#### API Keys
+You can generate as many API keys as you desire with custom expiration dates in order to bypass the email login. Create keys via your email login. To do this, run create_api_key and save the resulting output that is your new API Key. This will only be shown once.
+
+```python
+ana.create_api_key(name='name', expires='mm-dd-yyyy', organizationId='OrgId') ​
+'apikey-12345...'
+```
+
+This API Key can be used for future logins as demonstrated in the following two examples.
+
+##### API Key Param
+
+```python
+>>> import anatools
+>>> ana = anatools.client(APIKey='API KEY')
+Using provided APIKey to login
+....
+```
+##### Environment Variable
+
+```python
+export RENDEREDAI_API_KEY=API_KEY
+python
+>>> import anatools
+>>> ana = anatools.client()
+Using environment RENDEREDAI_API_KEY key to login
+....
+```
+
 ## Quickstart Guide
 #### What is the Rendered.ai Platform?
 The Rendered.ai Platform is a synthetic dataset generation tool where graphs describe what and how synthetic datasets are generated.
 
 | Terms | Definitions |
 |-|-|
 | workspace | A workspace is a collection of data used for a particular use-case, for example workspaces can be used to organize data for different projects.
@@ -74,24 +117,15 @@
 | node | A node can be described as an executable block of code, it has inputs and runs some algorithm to generate outputs. |
 | link | A link is used to transfer data from the output of one node, to the input of other nodes. |
 | channel | A channel is a collection of nodes, it is used to limit the scope of what is possible to generate in a dataset (like content from a tv channel). |
 
 #### How do you use the SDK?
 The Rendered.ai Platform creates synthetic datasets by processing a graph, so we will need to create the client to connect to the Platform API, create a graph, then create a dataset.
 
-1. Execute the python command line, create a client and login to Rendered.ai.
-In this example we are instantiating a client with no workspace or environment variables, so it is setting our default workspace.
-To access the tool, you will need to use your email and password for https://deckard.rendered.ai.
-```python
->>> import anatools
->>> ana = anatools.client()
-'Enter your credentials for the Rendered.ai Platform.'
-'email:' example@rendered.ai
-'password:' ***************
-```
+1. Login using email or API Key
 
 2. Create a graph file called `graph.yml` with the code below. 
 We are defining a simplistic graph for this example with multiple children's toys dropped into a container.
 While `YAML` files are used in channel development and for this example, the Platform SDK and API only support `JSON`. Ensure that the `YAML` file is valid in order for the SDK to convert `YAML` to `JSON` for you. Otherwise,  provide a graph in `JSON` format. 
 ```yaml
 version: 2
 nodes:
@@ -179,7 +213,9 @@
 The client will return a `datasetId` that can be used for reference later. You can use this `datasetId` to check the job status and, once the job is complete, download the dataset. You have now generated Synthetic Data!
 
 ``` python
 >>> datasetId = ana.create_dataset(name='testdataset',graphId=graphId,interpretations='10',priority='1',seed='1',description='A simple dataset with cubes in a container.')
 >>> datasetId
 'ce66e81c-23a6-11eb-adc1-0242ac120002'
 ```
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `anatools-3.2.2/README.md` & `anatools-3.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -45,14 +45,57 @@
 | pyyaml | A python YAML parser and emitter. |
 | requests | A simple HTTP python library. |
 
 If you have any questions or comments, contact Rendered.AI at info@rendered.ai.
 
 <br />
 
+## Multiple ways to login
+
+#### Login with email
+Execute the python command line, create a client and login to Rendered.ai.
+In this example we are instantiating a client with no workspace or environment variables, so it is setting our default workspace.
+To access the tool, you will need to use your email and password for https://deckard.rendered.ai.
+```python
+>>> import anatools
+>>> ana = anatools.client()
+'Enter your credentials for the Rendered.ai Platform.'
+'email:' example@rendered.ai
+'password:' ***************
+```
+
+#### API Keys
+You can generate as many API keys as you desire with custom expiration dates in order to bypass the email login. Create keys via your email login. To do this, run create_api_key and save the resulting output that is your new API Key. This will only be shown once.
+
+```python
+ana.create_api_key(name='name', expires='mm-dd-yyyy', organizationId='OrgId') ​
+'apikey-12345...'
+```
+
+This API Key can be used for future logins as demonstrated in the following two examples.
+
+##### API Key Param
+
+```python
+>>> import anatools
+>>> ana = anatools.client(APIKey='API KEY')
+Using provided APIKey to login
+....
+```
+##### Environment Variable
+
+```python
+export RENDEREDAI_API_KEY=API_KEY
+python
+>>> import anatools
+>>> ana = anatools.client()
+Using environment RENDEREDAI_API_KEY key to login
+....
+```
+
 ## Quickstart Guide
 #### What is the Rendered.ai Platform?
 The Rendered.ai Platform is a synthetic dataset generation tool where graphs describe what and how synthetic datasets are generated.
 
 | Terms | Definitions |
 |-|-|
 | workspace | A workspace is a collection of data used for a particular use-case, for example workspaces can be used to organize data for different projects.
@@ -61,24 +104,15 @@
 | node | A node can be described as an executable block of code, it has inputs and runs some algorithm to generate outputs. |
 | link | A link is used to transfer data from the output of one node, to the input of other nodes. |
 | channel | A channel is a collection of nodes, it is used to limit the scope of what is possible to generate in a dataset (like content from a tv channel). |
 
 #### How do you use the SDK?
 The Rendered.ai Platform creates synthetic datasets by processing a graph, so we will need to create the client to connect to the Platform API, create a graph, then create a dataset.
 
-1. Execute the python command line, create a client and login to Rendered.ai.
-In this example we are instantiating a client with no workspace or environment variables, so it is setting our default workspace.
-To access the tool, you will need to use your email and password for https://deckard.rendered.ai.
-```python
->>> import anatools
->>> ana = anatools.client()
-'Enter your credentials for the Rendered.ai Platform.'
-'email:' example@rendered.ai
-'password:' ***************
-```
+1. Login using email or API Key
 
 2. Create a graph file called `graph.yml` with the code below. 
 We are defining a simplistic graph for this example with multiple children's toys dropped into a container.
 While `YAML` files are used in channel development and for this example, the Platform SDK and API only support `JSON`. Ensure that the `YAML` file is valid in order for the SDK to convert `YAML` to `JSON` for you. Otherwise,  provide a graph in `JSON` format. 
 ```yaml
 version: 2
 nodes:
@@ -165,8 +199,10 @@
 
 The client will return a `datasetId` that can be used for reference later. You can use this `datasetId` to check the job status and, once the job is complete, download the dataset. You have now generated Synthetic Data!
 
 ``` python
 >>> datasetId = ana.create_dataset(name='testdataset',graphId=graphId,interpretations='10',priority='1',seed='1',description='A simple dataset with cubes in a container.')
 >>> datasetId
 'ce66e81c-23a6-11eb-adc1-0242ac120002'
-```
+```
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `anatools-3.2.2/anatools/__init__.py` & `anatools-3.3.0/anatools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
         https://support.rendered.ai/gc/Introduction-to-Rendered.ai.1577812005.html
 
 """
 
 from .anaclient.anaclient import client
 from .annotations.annotations import annotations
 
-__version__ = '3.2.2'
+__version__ = '3.3.0'
```

### Comparing `anatools-3.2.2/anatools/anaclient/anaclient.py` & `anatools-3.3.0/anatools/anaclient/anaclient.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         'url':  'https://deckard-infra.web.app',
         'statusAPI': 'https://api.infra.rendered.ai/system',
         'api':  'https://api.infra.rendered.ai/graphql' }
 }
 
 class client:
 
-    def __init__(self, workspaceId=None, environment='prod', email=None, password=None, local=False, interactive=True, verbose=None):
+    def __init__(self, workspaceId=None, environment='prod', email=None, password=None, APIKey=None, local=False, interactive=True, verbose=None):
         import getpass
         import time
         import os
         from anatools.anaclient.api import api
         from anatools.lib.print import print_color
         self.verbose = verbose
         self.interactive = interactive
@@ -39,14 +39,15 @@
             self.__url = 'http://127.0.0.1:3000'
             if interactive: print("Local is set to",self.__url)
         else: self.__url = envs[environment]['api']
         self.__status_url = envs[environment]['statusAPI']
         self.__password = password
         self.__logout = True
         self.__notificationId = None
+        self.__APIKey = None
         self.email = email
         self.user = None
         self.organizations = {}
         self.workspaces ={}
         self.channels = {}
         self.volumes = {}
         self.organization = None
@@ -55,85 +56,145 @@
 
         # fetch system notification
         notification = self.ana_api.getSystemNotifications()
         if notification:
             self.__notificationId = notification['notificationId']
             print_color(notification['message'], 'ffff00')
 
-        if not self.email:
-            print(f'Enter your credentials for the {envs[environment]["name"]}.') 
-            self.email = input('Email: ')
-        if not self.__password:
-            failcount = 1
-            while self.user is None:
-                self.__password = getpass.getpass()
-                self.user = self.ana_api.login(self.email, self.__password)
-        if self.user is None:
-            try: self.user = self.ana_api.login(self.email, self.__password)
-            except: print(f'Failed to login to {envs[environment]["name"]} with email {self.email}.'); return
-        if self.user is False: print(f'Failed to login to {envs[environment]["name"]} with email {self.email}.'); return
-        if self.verbose == 'debug': print(f'{self.user["uid"]}\n{self.user["idtoken"]}')
-        self.__logout = False
-        self.ana_api = api(self.__url, self.__status_url, {'uid':self.user['uid'], 'idtoken':self.user['idtoken']}, self.verbose)
-        self.get_organizations()
-        if len(self.organizations) == 0: print("No organizations available. Contact support@rendered.ai for support or fill out a form at https://rendered.ai/#contact."); return
-        found_valid_org = False
-        for organization in self.organizations:
-            if organization['expired']:
-                print("Warning!!!")
-                print(f"    The subscription has expired for {organization['name']} organization (organizationId {organization['organizationId']}).") 
-                print("    Update the subscription by signing into deckard.rendered.ai or contact sales@rendered.ai.")
+        if(APIKey == None and 'RENDEREDAI_API_KEY' in os.environ and not email): 
+            print_color("Using environment RENDEREDAI_API_KEY key to login", 'ffff00')
+            self.__APIKey = os.environ.get('RENDEREDAI_API_KEY')
+            self.sign_in_apikey(interactive=interactive)
+        
+        elif (APIKey):
+            print_color("Using provided APIKey to login", 'ffff00')
+            self.__APIKey = APIKey
+            self.sign_in_apikey(interactive=interactive)
+
+        else :        
+            if not self.email:
+                print(f'Enter your credentials for the {envs[environment]["name"]}.') 
+                self.email = input('Email: ')
+            if not self.__password:
+                failcount = 1
+                while self.user is None:
+                    self.__password = getpass.getpass()
+                    self.user = self.ana_api.login(self.email, self.__password)
+        
+            if self.user is None:
+                try: self.user = self.ana_api.login(self.email, self.__password)
+                except: print(f'Failed to login to {envs[environment]["name"]} with email {self.email}.'); return
+            if self.user is False: print(f'Failed to login to {envs[environment]["name"]} with email {self.email}.'); return
+            if self.verbose == 'debug': print(f'{self.user["uid"]}\n{self.user["idtoken"]}')
+            self.__logout = False
+            self.ana_api = api(self.__url, self.__status_url, {'uid':self.user['uid'], 'idtoken':self.user['idtoken']}, self.verbose)
+            self.get_organizations()
+            if len(self.organizations) == 0: print("No organizations available. Contact support@rendered.ai for support or fill out a form at https://rendered.ai/#contact."); return
+            found_valid_org = False
+            for organization in self.organizations:
+                if organization['expired']:
+                    print("Warning!!!")
+                    print(f"    The subscription has expired for {organization['name']} organization (organizationId {organization['organizationId']}).") 
+                    print("    Update the subscription by signing into deckard.rendered.ai or contact sales@rendered.ai.")
+                else:
+                    found_valid_org = True
+            if not found_valid_org:
+                print("Error: found no valid workspaces. If you believe this is a mistake, contact Rendered.ai at bugs@rendered.ai.")
+                return
+            self.get_workspaces()
+            if len(self.workspaces) == 0: 
+                self.workspace = None
+                print("No workspaces available. Contact support@rendered.ai for support or fill out a form at https://rendered.ai/#contact."); 
+                return
+            self.get_channels()
+            self.get_volumes()
+            if workspaceId:     
+                self.workspace = workspaceId
+                for workspace in self.workspaces:
+                    if self.workspace == workspace['workspaceId']: self.organization = workspace['organizationId']
+                if self.organization is None:
+                    print("The workspaceId provided is invalid. If you believe this is a mistake, contact support@rendered.ai for support or fill out a form at https://rendered.ai/#contact.")
+                    for workspace in self.workspaces: print(workspace["workspaceId"])
+                    self.workspace = None
+                    return
             else:
-                found_valid_org = True
-        if not found_valid_org:
-            print("Error: found no valid workspaces. If you believe this is a mistake, contact Rendered.ai at bugs@rendered.ai.")
+                self.workspace = self.workspaces[0]['workspaceId']
+                self.organization = self.workspaces[0]['organizationId']
+                if interactive: 
+                    print(f'These are your organizations and workspaces:')
+                    for organization in self.organizations:
+                        print(f"    {organization['name']+' Organization'[:44]:<44}  {organization['organizationId']:<50}")
+                        for workspace in self.workspaces:
+                            if workspace["organizationId"] == organization["organizationId"]:
+                                print(f"\t{workspace['name'][:40]:<40}  {workspace['workspaceId']:<50}")
+            if interactive: 
+                print(f'Signed into {envs[environment]["name"]} with {self.email}')
+                print(f'The current organization is: {self.organization}')
+                print(f'The current workspace is: {self.workspace}')
+
+    def sign_in_apikey(self, interactive):
+        from anatools.anaclient.api import api
+        from anatools.lib.print import print_color
+        from datetime import datetime
+        self.__logout = False
+
+        self.ana_api = api(self.__url, self.__status_url, {'apikey':self.__APIKey}, self.verbose)
+        apikeydata = self.ana_api.getAPIKeyContext(apiKey=self.__APIKey)
+        if not apikeydata:
+            print_color("Invalid API Key", 'ffff00')
+            return
+
+        # check the key is not expired
+        apikey_date = datetime.strptime(apikeydata['expiresAt'], "%Y-%m-%dT%H:%M:%S.%fZ")
+        current_date = datetime.now()
+        if apikey_date < current_date:
+            print_color(f"API Key expired at {apikey_date}", 'ffff00')
             return
-        self.get_workspaces()
+        
+
+        self.organization = apikeydata['organizationId']
+        self.organizations = self.get_organizations(apikeydata['organizationId'])
+
+        # check the organization is not expired
+        if self.organizations[0]['expired']:
+            print("Warning!!!")
+            print(f"    The subscription has expired for {self.organizations[0]['name']} organization (organizationId {self.organizations[0]['organizationId']}).") 
+            print("    Update the subscription by signing into deckard.rendered.ai or contact sales@rendered.ai.")
+
+        self.workspaces = self.get_workspaces(organizationId=self.organization)
         if len(self.workspaces) == 0: 
             self.workspace = None
             print("No workspaces available. Contact support@rendered.ai for support or fill out a form at https://rendered.ai/#contact."); 
             return
-        self.get_channels()
-        self.get_volumes()
-        if workspaceId:     
-            self.workspace = workspaceId
-            for workspace in self.workspaces:
-                if self.workspace == workspace['workspaceId']: self.organization = workspace['organizationId']
-            if self.organization is None:
-                print("The workspaceId provided is invalid. If you believe this is a mistake, contact support@rendered.ai for support or fill out a form at https://rendered.ai/#contact.")
-                for workspace in self.workspaces: print(workspace["workspaceId"])
-                self.workspace = None
-                return
-        else:
-            self.workspace = self.workspaces[0]['workspaceId']
-            self.organization = self.workspaces[0]['organizationId']
-            if interactive: 
-                print(f'These are your organizations and workspaces:')
-                for organization in self.organizations:
-                    print(f"    {organization['name']+' Organization'[:44]:<44}  {organization['organizationId']:<50}")
-                    for workspace in self.workspaces:
-                        if workspace["organizationId"] == organization["organizationId"]:
-                            print(f"\t{workspace['name'][:40]:<40}  {workspace['workspaceId']:<50}")
+
+        self.workspace = self.workspaces[0]['workspaceId']
+        self.get_channels(organizationId=self.organization)
+        self.get_volumes(organizationId=self.organization)
+
         if interactive: 
-            print(f'Signed into {envs[environment]["name"]} with {self.email}')
+            print(f'This is your organization and workspaces:')
+            print(f"    {self.organizations[0]['name']+' Organization'[:44]:<44}  {self.organizations[0]['organizationId']:<50}")
+            for workspace in self.workspaces:
+                print(f"\t{workspace['name'][:40]:<40}  {workspace['workspaceId']:<50}")
+
             print(f'The current organization is: {self.organization}')
             print(f'The current workspace is: {self.workspace}')
 
-
     def refresh_token(self):
         import time
         from anatools.anaclient.api import api
         from anatools.lib.print import print_color
-        if int(time.time()) > int(self.user['expires']):
-            self.user = self.ana_api.login(self.email, self.__password)
-            self.ana_api = api(self.__url, self.__status_url, {'uid': self.user['uid'], 'idtoken': self.user['idtoken']}, self.verbose)
-            notification = self.ana_api.getSystemNotifications()
-            if notification and notification['notificationId'] != self.__notificationId:
-                self.__notificationId = notification['notificationId']
-                print_color(notification['message'], 'ffff00')
+        if self.user:
+            if int(time.time()) > int(self.user['expires']):
+                self.user = self.ana_api.login(self.email, self.__password)
+                self.ana_api = api(self.__url, self.__status_url, {'uid': self.user['uid'], 'idtoken': self.user['idtoken']}, self.verbose)
+                notification = self.ana_api.getSystemNotifications()
+                if notification and notification['notificationId'] != self.__notificationId:
+                    self.__notificationId = notification['notificationId']
+                    print_color(notification['message'], 'ffff00')
 
 
     def check_logout(self):
         if self.__logout: print('You are currently logged out, login to access the Rendered.ai Platform.'); return True
         self.refresh_token()
         return False
 
@@ -200,7 +261,8 @@
     from .datasets      import get_datasets, create_dataset, edit_dataset, delete_dataset, download_dataset, cancel_dataset, upload_dataset, get_dataset_runs, get_dataset_log
     from .channels      import get_channels, get_managed_channels, create_managed_channel, edit_managed_channel, delete_managed_channel, add_channel_access, remove_channel_access, build_managed_channel, deploy_managed_channel, get_deployment_status, get_channel_documentation, upload_channel_documentation
     from .volumes       import get_volumes, get_managed_volumes, create_managed_volume, edit_managed_volume, delete_managed_volume, add_volume_access, remove_volume_access, get_volume_data, download_volume_data, upload_volume_data, delete_volume_data, mount_volumes
     from .analytics     import get_analytics, get_analytics_types, create_analytics, delete_analytics
     from .annotations   import get_annotations, get_annotation_formats, get_annotation_maps, create_annotation, download_annotation, delete_annotation , get_managed_maps, create_managed_map, edit_managed_map, delete_managed_map, add_map_organization, remove_map_organization, download_managed_map
     from .gan           import get_gan_models, get_gan_dataset, create_gan_dataset, delete_gan_dataset, create_managed_gan, delete_gan_model, get_managed_gans, edit_managed_gan, delete_managed_gan, add_gan_organization, remove_gan_organization, download_managed_gan
     from .umap          import get_umap, create_umap, delete_umap
+    from .api_keys      import get_api_keys, create_api_key, delete_api_key, get_api_key_data
```

### Comparing `anatools-3.2.2/anatools/anaclient/analytics.py` & `anatools-3.3.0/anatools/anaclient/analytics.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/annotations.py` & `anatools-3.3.0/anatools/anaclient/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/api/analytics.py` & `anatools-3.3.0/anatools/anaclient/api/analytics.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/api/annotations.py` & `anatools-3.3.0/anatools/anaclient/api/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/api/api.py` & `anatools-3.3.0/anatools/anaclient/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,7 +81,8 @@
     from .graphs        import getGraphs, createGraph, deleteGraph, editGraph, downloadGraph, getDefaultGraph
     from .datasets      import getDatasets, createDataset, deleteDataset, editDataset, downloadDataset, cancelDataset, datasetUpload, getDatasetRuns, getDatasetLog
     from .limits        import getPlatformLimits, setPlatformLimit, getOrganizationLimits, setOrganizationLimit, getWorkspaceLimits, setWorkspaceLimit, getOrganizationUsage
     from .analytics     import getAnalytics, getAnalyticsTypes, createAnalytics, deleteAnalytics
     from .annotations   import getAnnotations, getAnnotationFormats, getAnnotationMaps, createAnnotation, downloadAnnotation, getManagedMaps, createManagedMap, editManagedMap, deleteManagedMap, addMapOrganization, removeMapOrganization, downloadManagedMap
     from .gan           import getGANModels, getGANDataset, createGANDataset, deleteGANDataset, createManagedGAN, deleteGANModel, addGANAccess, removeGANAccess, getManagedGANs, editManagedGAN, deleteManagedGAN, addGANOrganization, removeGANOrganization, downloadManagedGAN
     from .umap          import getUMAP, createUMAP, deleteUMAP
+    from .api_keys      import getAPIKeys, createAPIKey, deleteAPIKey, getAPIKeyData, getAPIKeyContext
```

### Comparing `anatools-3.2.2/anatools/anaclient/api/channels.py` & `anatools-3.3.0/anatools/anaclient/api/channels.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/api/datasets.py` & `anatools-3.3.0/anatools/anaclient/api/datasets.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/api/gan.py` & `anatools-3.3.0/anatools/anaclient/api/gan.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/api/graphs.py` & `anatools-3.3.0/anatools/anaclient/api/graphs.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/api/handlers.py` & `anatools-3.3.0/anatools/anaclient/api/handlers.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/api/limits.py` & `anatools-3.3.0/anatools/anaclient/api/limits.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/api/members.py` & `anatools-3.3.0/anatools/anaclient/api/members.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/api/organizations.py` & `anatools-3.3.0/anatools/anaclient/api/organizations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/api/umap.py` & `anatools-3.3.0/anatools/anaclient/api/umap.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         json = {
             "operationName": "createUMAP",
             "variables": {
                 "workspaceId": workspaceId,
                 "datasetIds": datasetIds,
                 "samples": samples
             },
-            "query": """query 
+            "query": """mutation 
                 createUMAP($workspaceId: String!, $datasetIds: [String]!, $samples: [Int]!) {
                     createUMAP(workspaceId: $workspaceId, datasetIds: $datasetIds, samples: $samples)
                 }"""})
     return self.errorhandler(response, "createUMAP")
 
 
 def deleteUMAP(self, umapId, workspaceId):
```

### Comparing `anatools-3.2.2/anatools/anaclient/api/volumes.py` & `anatools-3.3.0/anatools/anaclient/api/volumes.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/api/workspaces.py` & `anatools-3.3.0/anatools/anaclient/api/workspaces.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/channels.py` & `anatools-3.3.0/anatools/anaclient/channels.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     
     Returns
     -------
     list[dict]
         List of channels associated with user, workspace, organization or channelId.
     """
     if self.check_logout(): return
+    if organizationId is None and self.user is None: organizationId = self.organization
     channels = self.ana_api.getChannels(organizationId=organizationId, workspaceId=workspaceId, channelId=channelId)
     if channels:
         for channel in channels:
             self.channels[channel['channelId']] = channel['name']
     return channels
```

### Comparing `anatools-3.2.2/anatools/anaclient/datasets.py` & `anatools-3.3.0/anatools/anaclient/datasets.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/gan.py` & `anatools-3.3.0/anatools/anaclient/gan.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/graphs.py` & `anatools-3.3.0/anatools/anaclient/graphs.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/organizations.py` & `anatools-3.3.0/anatools/anaclient/organizations.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,19 @@
     Parameters
     ----------
     organizationId : str
         Organization ID for the organization you wish to work in.
     workspaceId : str
         Workspace ID for the workspace you wish to work in. Uses default workspace if this is not set.
     """
+    from anatools.lib.print import print_color
     if self.check_logout(): return
+    if not self.user: 
+        print_color("Cannot change organization while using API Key", 'ffff00')
+        return
     if organizationId is None: raise Exception('OrganizationId must be specified.')
     workspaceSet = False
     self.workspaces = self.ana_api.getWorkspaces()
     if len(self.workspaces) == 0: 
         self.workspace = None
         print("No workspaces available. Contact support@rendered.ai for support or fill out a form at https://rendered.ai/#contact."); 
         return
@@ -51,14 +55,15 @@
     
     Returns
     -------
     list[dict]
         Information about the organizations you belong to. 
     """  
     if self.check_logout(): return
+    if organizationId is None and self.user is None: organizationId = self.organization
     if organizationId is None:
         self.organizations = self.ana_api.getOrganizations(organizationId)
         return self.organizations
     else:
         organizations = self.ana_api.getOrganizations(organizationId)
         return organizations
```

### Comparing `anatools-3.2.2/anatools/anaclient/umap.py` & `anatools-3.3.0/anatools/anaclient/umap.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/anaclient/volumes.py` & `anatools-3.3.0/anatools/anaclient/volumes.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     
     Returns
     -------
     list[dict]
         Volume Info
     """
     if self.check_logout(): return
+    if organizationId is None and self.user is None: organizationId = self.organization
     volumes = self.ana_api.getVolumes(organizationId=organizationId, volumeId=volumeId)
     if volumes:
         for volume in volumes:
             self.volumes[volume['volumeId']] = volume['name']
     return volumes
```

### Comparing `anatools-3.2.2/anatools/anaclient/workspaces.py` & `anatools-3.3.0/anatools/anaclient/workspaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     ----------
     workspaceId : str
         Workspace ID for the workspace you wish to work in.
     """
     if self.check_logout(): return
     if workspaceId is None: raise Exception('WorkspaceId must be specified.')
     workspaceSet = False
-    self.workspaces = self.ana_api.getWorkspaces()
+    if self.user: self.workspaces = self.ana_api.getWorkspaces()
+    else: self.workspaces = self.ana_api.getWorkspaces(organizationId=self.organization)
     for workspace in self.workspaces:
         if workspaceId == workspace['workspaceId']:
             self.workspace = workspace['workspaceId']
             self.organization = workspace['organizationId']
             workspaceSet = True
             break
     if not workspaceSet: raise Exception('Could not find workspace specified.')
@@ -50,14 +51,15 @@
 
     Returns
     -------
     list[dict]
         Workspace data for all workspaces for a user.
     """  
     if self.check_logout(): return
+    if organizationId is None and self.user is None: organizationId = self.organization
     if organizationId is None and workspaceId is None:
         self.workspaces = self.ana_api.getWorkspaces(organizationId, workspaceId)
         return self.workspaces
     else:
         workspaces = self.ana_api.getWorkspaces(organizationId, workspaceId)
         return workspaces
```

### Comparing `anatools-3.2.2/anatools/annotations/annotations.py` & `anatools-3.3.0/anatools/annotations/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/annotations/convert_coco.py` & `anatools-3.3.0/anatools/annotations/convert_coco.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/annotations/convert_kitti.py` & `anatools-3.3.0/anatools/annotations/convert_kitti.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/annotations/convert_pascal.py` & `anatools-3.3.0/anatools/annotations/convert_pascal.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/annotations/convert_sagemaker.py` & `anatools-3.3.0/anatools/annotations/convert_sagemaker.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/annotations/convert_yolo.py` & `anatools-3.3.0/anatools/annotations/convert_yolo.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/annotations/draw.py` & `anatools-3.3.0/anatools/annotations/draw.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/bin/ana` & `anatools-3.3.0/anatools/bin/ana`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/bin/anadeploy` & `anatools-3.3.0/anatools/bin/anadeploy`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/bin/anamount` & `anatools-3.3.0/anatools/bin/anamount`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/bin/anautils` & `anatools-3.3.0/anatools/bin/anautils`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/ana_object.py` & `anatools-3.3.0/anatools/lib/ana_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/bbox.py` & `anatools-3.3.0/anatools/lib/bbox.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/blender_main.py` & `anatools-3.3.0/anatools/lib/blender_main.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/camera_checks.py` & `anatools-3.3.0/anatools/lib/camera_checks.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/channel.py` & `anatools-3.3.0/anatools/lib/channel.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/context.py` & `anatools-3.3.0/anatools/lib/context.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/directory_object.py` & `anatools-3.3.0/anatools/lib/directory_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/file_handlers.py` & `anatools-3.3.0/anatools/lib/file_handlers.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/file_metadata.py` & `anatools-3.3.0/anatools/lib/file_metadata.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/file_object.py` & `anatools-3.3.0/anatools/lib/file_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/generator.py` & `anatools-3.3.0/anatools/lib/generator.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/interp.py` & `anatools-3.3.0/anatools/lib/interp.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/load.py` & `anatools-3.3.0/anatools/lib/load.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/node.py` & `anatools-3.3.0/anatools/lib/node.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/object_utils.py` & `anatools-3.3.0/anatools/lib/object_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/package_utils.py` & `anatools-3.3.0/anatools/lib/package_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/python_main.py` & `anatools-3.3.0/anatools/lib/python_main.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/rigged_object.py` & `anatools-3.3.0/anatools/lib/rigged_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/scene.py` & `anatools-3.3.0/anatools/lib/scene.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/lib/search_utils.py` & `anatools-3.3.0/anatools/lib/search_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/constants.py` & `anatools-3.3.0/anatools/nodes/constants.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/constants.yml` & `anatools-3.3.0/anatools/nodes/constants.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/generators.py` & `anatools-3.3.0/anatools/nodes/generators.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/generators.yml` & `anatools-3.3.0/anatools/nodes/generators.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/logic.py` & `anatools-3.3.0/anatools/nodes/logic.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/logic.yml` & `anatools-3.3.0/anatools/nodes/logic.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/random_generator.py` & `anatools-3.3.0/anatools/nodes/random_generator.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/random_generator.yml` & `anatools-3.3.0/anatools/nodes/random_generator.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/sweep_arange.py` & `anatools-3.3.0/anatools/nodes/sweep_arange.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/sweep_arange.yml` & `anatools-3.3.0/anatools/nodes/sweep_arange.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/sweep_linspace.py` & `anatools-3.3.0/anatools/nodes/sweep_linspace.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/sweep_linspace.yml` & `anatools-3.3.0/anatools/nodes/sweep_linspace.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/vectors.py` & `anatools-3.3.0/anatools/nodes/vectors.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/vectors.yml` & `anatools-3.3.0/anatools/nodes/vectors.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/volume_directory.py` & `anatools-3.3.0/anatools/nodes/volume_directory.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/volume_directory.yml` & `anatools-3.3.0/anatools/nodes/volume_directory.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/volume_file.py` & `anatools-3.3.0/anatools/nodes/volume_file.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools/nodes/volume_file.yml` & `anatools-3.3.0/anatools/nodes/volume_file.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/anatools.egg-info/PKG-INFO` & `anatools-3.3.0/anatools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anatools
-Version: 3.2.2
+Version: 3.3.0
 Summary: Tools for development with the Rendered.ai Platform.
 Home-page: https://rendered.ai
 Author: Rendered AI, Inc
 Author-email: support@rendered.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
@@ -58,14 +58,57 @@
 | pyyaml | A python YAML parser and emitter. |
 | requests | A simple HTTP python library. |
 
 If you have any questions or comments, contact Rendered.AI at info@rendered.ai.
 
 <br />
 
+## Multiple ways to login
+
+#### Login with email
+Execute the python command line, create a client and login to Rendered.ai.
+In this example we are instantiating a client with no workspace or environment variables, so it is setting our default workspace.
+To access the tool, you will need to use your email and password for https://deckard.rendered.ai.
+```python
+>>> import anatools
+>>> ana = anatools.client()
+'Enter your credentials for the Rendered.ai Platform.'
+'email:' example@rendered.ai
+'password:' ***************
+```
+
+#### API Keys
+You can generate as many API keys as you desire with custom expiration dates in order to bypass the email login. Create keys via your email login. To do this, run create_api_key and save the resulting output that is your new API Key. This will only be shown once.
+
+```python
+ana.create_api_key(name='name', expires='mm-dd-yyyy', organizationId='OrgId') ​
+'apikey-12345...'
+```
+
+This API Key can be used for future logins as demonstrated in the following two examples.
+
+##### API Key Param
+
+```python
+>>> import anatools
+>>> ana = anatools.client(APIKey='API KEY')
+Using provided APIKey to login
+....
+```
+##### Environment Variable
+
+```python
+export RENDEREDAI_API_KEY=API_KEY
+python
+>>> import anatools
+>>> ana = anatools.client()
+Using environment RENDEREDAI_API_KEY key to login
+....
+```
+
 ## Quickstart Guide
 #### What is the Rendered.ai Platform?
 The Rendered.ai Platform is a synthetic dataset generation tool where graphs describe what and how synthetic datasets are generated.
 
 | Terms | Definitions |
 |-|-|
 | workspace | A workspace is a collection of data used for a particular use-case, for example workspaces can be used to organize data for different projects.
@@ -74,24 +117,15 @@
 | node | A node can be described as an executable block of code, it has inputs and runs some algorithm to generate outputs. |
 | link | A link is used to transfer data from the output of one node, to the input of other nodes. |
 | channel | A channel is a collection of nodes, it is used to limit the scope of what is possible to generate in a dataset (like content from a tv channel). |
 
 #### How do you use the SDK?
 The Rendered.ai Platform creates synthetic datasets by processing a graph, so we will need to create the client to connect to the Platform API, create a graph, then create a dataset.
 
-1. Execute the python command line, create a client and login to Rendered.ai.
-In this example we are instantiating a client with no workspace or environment variables, so it is setting our default workspace.
-To access the tool, you will need to use your email and password for https://deckard.rendered.ai.
-```python
->>> import anatools
->>> ana = anatools.client()
-'Enter your credentials for the Rendered.ai Platform.'
-'email:' example@rendered.ai
-'password:' ***************
-```
+1. Login using email or API Key
 
 2. Create a graph file called `graph.yml` with the code below. 
 We are defining a simplistic graph for this example with multiple children's toys dropped into a container.
 While `YAML` files are used in channel development and for this example, the Platform SDK and API only support `JSON`. Ensure that the `YAML` file is valid in order for the SDK to convert `YAML` to `JSON` for you. Otherwise,  provide a graph in `JSON` format. 
 ```yaml
 version: 2
 nodes:
@@ -179,7 +213,9 @@
 The client will return a `datasetId` that can be used for reference later. You can use this `datasetId` to check the job status and, once the job is complete, download the dataset. You have now generated Synthetic Data!
 
 ``` python
 >>> datasetId = ana.create_dataset(name='testdataset',graphId=graphId,interpretations='10',priority='1',seed='1',description='A simple dataset with cubes in a container.')
 >>> datasetId
 'ce66e81c-23a6-11eb-adc1-0242ac120002'
 ```
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `anatools-3.2.2/anatools.egg-info/SOURCES.txt` & `anatools-3.3.0/anatools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,26 +10,28 @@
 anatools.egg-info/dependency_links.txt
 anatools.egg-info/requires.txt
 anatools.egg-info/top_level.txt
 anatools/anaclient/__init__.py
 anatools/anaclient/anaclient.py
 anatools/anaclient/analytics.py
 anatools/anaclient/annotations.py
+anatools/anaclient/api_keys.py
 anatools/anaclient/channels.py
 anatools/anaclient/datasets.py
 anatools/anaclient/gan.py
 anatools/anaclient/graphs.py
 anatools/anaclient/organizations.py
 anatools/anaclient/umap.py
 anatools/anaclient/volumes.py
 anatools/anaclient/workspaces.py
 anatools/anaclient/api/__init__.py
 anatools/anaclient/api/analytics.py
 anatools/anaclient/api/annotations.py
 anatools/anaclient/api/api.py
+anatools/anaclient/api/api_keys.py
 anatools/anaclient/api/channels.py
 anatools/anaclient/api/datasets.py
 anatools/anaclient/api/gan.py
 anatools/anaclient/api/graphs.py
 anatools/anaclient/api/handlers.py
 anatools/anaclient/api/limits.py
 anatools/anaclient/api/members.py
```

### Comparing `anatools-3.2.2/setup.py` & `anatools-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `anatools-3.2.2/tests/test_bbox.py` & `anatools-3.3.0/tests/test_bbox.py`

 * *Files identical despite different names*

