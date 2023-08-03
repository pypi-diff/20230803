# Comparing `tmp/txrm2tiff-2.0.7.tar.gz` & `tmp/txrm2tiff-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/rky95813/Documents/Eclipse2/txrm2tiff/dist/.tmp-5klfs9y2/txrm2tiff-2.0.7.tar", last modified: Thu Jul 27 14:17:06 2023, max compression
+gzip compressed data, was "/home/rky95813/Documents/Eclipse2/txrm2tiff/dist/.tmp-1h9ljtf7/txrm2tiff-2.0.8.tar", last modified: Thu Aug  3 15:03:58 2023, max compression
```

## Comparing `txrm2tiff-2.0.7.tar` & `txrm2tiff-2.0.8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1290 2023-07-10 08:58:14.000000 txrm2tiff-2.0.7/.gitignore
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/.settings/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       64 2020-03-30 17:10:47.000000 txrm2tiff-2.0.7/.settings/org.eclipse.core.resources.prefs
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/.vscode/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      638 2021-03-02 11:54:13.000000 txrm2tiff-2.0.7/.vscode/launch.json
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      766 2023-07-26 16:51:44.000000 txrm2tiff-2.0.7/.vscode/settings.json
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1533 2020-03-30 17:10:47.000000 txrm2tiff-2.0.7/LICENSE
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7423 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/PKG-INFO
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6945 2023-07-26 16:31:57.000000 txrm2tiff-2.0.7/README.md
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/conda/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1482 2023-07-27 14:15:28.000000 txrm2tiff-2.0.7/conda/meta.yaml
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1544 2023-07-27 14:15:28.000000 txrm2tiff-2.0.7/pyproject.toml
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       38 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/setup.cfg
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      122 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/src/txrm2tiff/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5966 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/src/txrm2tiff/__main__.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff/font/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    42884 2021-02-08 17:40:15.000000 txrm2tiff-2.0.7/src/txrm2tiff/font/CallingCode-Regular.otf
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1554 2021-02-08 17:40:15.000000 txrm2tiff-2.0.7/src/txrm2tiff/font/License.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       89 2023-07-26 16:21:03.000000 txrm2tiff-2.0.7/src/txrm2tiff/info.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6531 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/src/txrm2tiff/inspector.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6992 2023-07-26 16:32:48.000000 txrm2tiff-2.0.7/src/txrm2tiff/main.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       28 2021-12-01 16:06:26.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    18841 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/abstract.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    12885 2023-07-26 17:09:35.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/annot_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1357 2021-12-14 13:07:27.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/main.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     8432 2023-05-30 10:24:41.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/ref_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3086 2023-07-26 16:28:35.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/save_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1623 2021-12-01 16:29:22.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/shifts_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1560 2023-05-30 10:24:37.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/txrm_property.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3158 2023-05-30 10:24:41.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/v3.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2928 2023-05-30 10:24:41.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/v5.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm_functions/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       45 2021-11-26 16:04:02.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm_functions/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4667 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm_functions/general.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2649 2021-12-01 16:08:13.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm_functions/images.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        0 2021-11-26 16:04:02.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4715 2023-07-17 13:59:18.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/file_handler.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      415 2021-11-26 16:04:02.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/functions.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6400 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/image_processing.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      818 2021-11-26 16:04:02.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/logging.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5618 2023-07-07 17:08:26.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/metadata.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2570 2021-11-26 16:04:02.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/shortcut_creation.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/src/txrm2tiff/xradia_properties/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       50 2021-11-26 16:04:02.000000 txrm2tiff-2.0.7/src/txrm2tiff/xradia_properties/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1856 2023-05-30 10:24:41.000000 txrm2tiff-2.0.7/src/txrm2tiff/xradia_properties/enums.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3334 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/src/txrm2tiff/xradia_properties/stream_dtypes.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff.egg-info/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7423 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff.egg-info/PKG-INFO
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1853 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff.egg-info/SOURCES.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        1 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff.egg-info/dependency_links.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       54 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff.egg-info/entry_points.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      178 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff.egg-info/requires.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       10 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff.egg-info/top_level.txt
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/tests/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      193 2021-02-08 17:40:15.000000 txrm2tiff-2.0.7/tests/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    11184 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/tests/test_abstract_txrm.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    10974 2023-07-26 17:15:31.000000 txrm2tiff-2.0.7/tests/test_annotator.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     9650 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/tests/test_commandline_entrypoint.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5721 2023-07-17 13:59:18.000000 txrm2tiff-2.0.7/tests/test_file_handler.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5849 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/tests/test_image_processing.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2777 2021-12-01 16:29:22.000000 txrm2tiff-2.0.7/tests/test_inspector.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    14720 2023-07-26 16:31:57.000000 txrm2tiff-2.0.7/tests/test_main.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4036 2023-05-30 10:24:41.000000 txrm2tiff-2.0.7/tests/test_metadata.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3859 2023-07-26 16:31:57.000000 txrm2tiff-2.0.7/tests/test_referencer.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     9936 2023-05-30 16:23:06.000000 txrm2tiff-2.0.7/tests/test_saver.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1455 2021-12-01 16:07:16.000000 txrm2tiff-2.0.7/tests/test_setup_fuctions.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2246 2021-12-01 16:29:22.000000 txrm2tiff-2.0.7/tests/test_shifts.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5057 2021-12-01 16:07:23.000000 txrm2tiff-2.0.7/tests/test_txrm_functions.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2682 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/tests/test_txrm_property.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3709 2023-05-30 15:25:01.000000 txrm2tiff-2.0.7/tests/test_txrm_v5.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6007 2023-05-30 15:10:23.000000 txrm2tiff-2.0.7/tests/test_txrmv3.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      834 2021-12-01 16:07:35.000000 txrm2tiff-2.0.7/tests/test_util_functions.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7056 2021-12-14 13:07:27.000000 txrm2tiff-2.0.7/tests/test_with_files.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1290 2023-08-02 16:53:33.000000 txrm2tiff-2.0.8/.gitignore
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/.settings/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       64 2020-03-30 17:10:47.000000 txrm2tiff-2.0.8/.settings/org.eclipse.core.resources.prefs
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/.vscode/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      638 2021-03-02 11:54:13.000000 txrm2tiff-2.0.8/.vscode/launch.json
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      766 2023-08-02 16:53:33.000000 txrm2tiff-2.0.8/.vscode/settings.json
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1533 2020-03-30 17:10:47.000000 txrm2tiff-2.0.8/LICENSE
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7423 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/PKG-INFO
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6945 2023-08-02 16:53:33.000000 txrm2tiff-2.0.8/README.md
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/conda/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1482 2023-08-02 16:56:01.000000 txrm2tiff-2.0.8/conda/meta.yaml
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1544 2023-07-27 14:15:28.000000 txrm2tiff-2.0.8/pyproject.toml
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       38 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/setup.cfg
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/src/
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/src/txrm2tiff/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      122 2023-05-30 10:44:58.000000 txrm2tiff-2.0.8/src/txrm2tiff/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5966 2023-05-30 10:44:58.000000 txrm2tiff-2.0.8/src/txrm2tiff/__main__.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/src/txrm2tiff/font/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    42884 2021-02-08 17:40:15.000000 txrm2tiff-2.0.8/src/txrm2tiff/font/CallingCode-Regular.otf
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1554 2021-02-08 17:40:15.000000 txrm2tiff-2.0.8/src/txrm2tiff/font/License.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       89 2023-08-02 16:56:02.000000 txrm2tiff-2.0.8/src/txrm2tiff/info.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6531 2023-05-30 10:44:58.000000 txrm2tiff-2.0.8/src/txrm2tiff/inspector.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6992 2023-07-26 16:32:48.000000 txrm2tiff-2.0.8/src/txrm2tiff/main.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       28 2021-12-01 16:06:26.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    18841 2023-05-30 10:44:58.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm/abstract.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    13229 2023-08-02 16:53:33.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm/annot_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1357 2021-12-14 13:07:27.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm/main.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     8432 2023-05-30 10:24:41.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm/ref_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3086 2023-07-26 16:28:35.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm/save_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1623 2021-12-01 16:29:22.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm/shifts_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1560 2023-05-30 10:24:37.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm/txrm_property.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3158 2023-05-30 10:24:41.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm/v3.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2928 2023-05-30 10:24:41.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm/v5.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm_functions/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       45 2021-11-26 16:04:02.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm_functions/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4667 2023-05-30 10:44:58.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm_functions/general.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2649 2021-12-01 16:08:13.000000 txrm2tiff-2.0.8/src/txrm2tiff/txrm_functions/images.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/src/txrm2tiff/utils/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        0 2021-11-26 16:04:02.000000 txrm2tiff-2.0.8/src/txrm2tiff/utils/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4715 2023-07-17 13:59:18.000000 txrm2tiff-2.0.8/src/txrm2tiff/utils/file_handler.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      415 2021-11-26 16:04:02.000000 txrm2tiff-2.0.8/src/txrm2tiff/utils/functions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6591 2023-08-02 16:53:33.000000 txrm2tiff-2.0.8/src/txrm2tiff/utils/image_processing.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      818 2021-11-26 16:04:02.000000 txrm2tiff-2.0.8/src/txrm2tiff/utils/logging.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5618 2023-07-07 17:08:26.000000 txrm2tiff-2.0.8/src/txrm2tiff/utils/metadata.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2570 2021-11-26 16:04:02.000000 txrm2tiff-2.0.8/src/txrm2tiff/utils/shortcut_creation.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/src/txrm2tiff/xradia_properties/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       50 2021-11-26 16:04:02.000000 txrm2tiff-2.0.8/src/txrm2tiff/xradia_properties/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1856 2023-05-30 10:24:41.000000 txrm2tiff-2.0.8/src/txrm2tiff/xradia_properties/enums.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3334 2023-05-30 10:44:58.000000 txrm2tiff-2.0.8/src/txrm2tiff/xradia_properties/stream_dtypes.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/src/txrm2tiff.egg-info/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7423 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/src/txrm2tiff.egg-info/PKG-INFO
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1853 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/src/txrm2tiff.egg-info/SOURCES.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        1 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/src/txrm2tiff.egg-info/dependency_links.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       54 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/src/txrm2tiff.egg-info/entry_points.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      178 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/src/txrm2tiff.egg-info/requires.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       10 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/src/txrm2tiff.egg-info/top_level.txt
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-08-03 15:03:58.000000 txrm2tiff-2.0.8/tests/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      193 2021-02-08 17:40:15.000000 txrm2tiff-2.0.8/tests/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    11184 2023-05-30 10:44:58.000000 txrm2tiff-2.0.8/tests/test_abstract_txrm.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    11066 2023-08-03 12:43:52.000000 txrm2tiff-2.0.8/tests/test_annotator.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     9650 2023-05-30 10:44:58.000000 txrm2tiff-2.0.8/tests/test_commandline_entrypoint.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5721 2023-07-17 13:59:18.000000 txrm2tiff-2.0.8/tests/test_file_handler.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6878 2023-08-03 12:37:02.000000 txrm2tiff-2.0.8/tests/test_image_processing.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2777 2021-12-01 16:29:22.000000 txrm2tiff-2.0.8/tests/test_inspector.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    14720 2023-07-26 16:31:57.000000 txrm2tiff-2.0.8/tests/test_main.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4036 2023-05-30 10:24:41.000000 txrm2tiff-2.0.8/tests/test_metadata.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3859 2023-07-26 16:31:57.000000 txrm2tiff-2.0.8/tests/test_referencer.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     9936 2023-05-30 16:23:06.000000 txrm2tiff-2.0.8/tests/test_saver.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1455 2021-12-01 16:07:16.000000 txrm2tiff-2.0.8/tests/test_setup_fuctions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2246 2021-12-01 16:29:22.000000 txrm2tiff-2.0.8/tests/test_shifts.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5057 2021-12-01 16:07:23.000000 txrm2tiff-2.0.8/tests/test_txrm_functions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2682 2023-05-30 10:44:58.000000 txrm2tiff-2.0.8/tests/test_txrm_property.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3709 2023-05-30 15:25:01.000000 txrm2tiff-2.0.8/tests/test_txrm_v5.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6007 2023-05-30 15:10:23.000000 txrm2tiff-2.0.8/tests/test_txrmv3.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      834 2021-12-01 16:07:35.000000 txrm2tiff-2.0.8/tests/test_util_functions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7056 2021-12-14 13:07:27.000000 txrm2tiff-2.0.8/tests/test_with_files.py
```

### Comparing `txrm2tiff-2.0.7/.gitignore` & `txrm2tiff-2.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/.vscode/launch.json` & `txrm2tiff-2.0.8/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/.vscode/settings.json` & `txrm2tiff-2.0.8/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/LICENSE` & `txrm2tiff-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/PKG-INFO` & `txrm2tiff-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txrm2tiff
-Version: 2.0.7
+Version: 2.0.8
 Summary: A converter for Zeiss txrm and xrm files, created by & for B24 of Diamond Light Source
 Author-email: Thomas Fish <thomas.fish@diamond.ac.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `txrm2tiff-2.0.7/README.md` & `txrm2tiff-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/conda/meta.yaml` & `txrm2tiff-2.0.8/conda/meta.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% set name = "txrm2tiff" %}
-{% set version = "2.0.7" %}
+{% set version = "2.0.8" %}
 
 package:
   name: {{ name|lower }}
   version: {{ version }}
 
 source:
   path: ../
```

### Comparing `txrm2tiff-2.0.7/pyproject.toml` & `txrm2tiff-2.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/__main__.py` & `txrm2tiff-2.0.8/src/txrm2tiff/__main__.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/font/CallingCode-Regular.otf` & `txrm2tiff-2.0.8/src/txrm2tiff/font/CallingCode-Regular.otf`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/font/License.txt` & `txrm2tiff-2.0.8/src/txrm2tiff/font/License.txt`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/inspector.py` & `txrm2tiff-2.0.8/src/txrm2tiff/inspector.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/main.py` & `txrm2tiff-2.0.8/src/txrm2tiff/main.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/txrm/abstract.py` & `txrm2tiff-2.0.8/src/txrm2tiff/txrm/abstract.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/txrm/annot_mixin.py` & `txrm2tiff-2.0.8/src/txrm2tiff/txrm/annot_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from collections import defaultdict
 from typing import Iterable, Optional, Tuple
 
 import numpy as np
 from PIL import Image, ImageDraw, ImageFont
 from PIL.ImageOps import autocontrast
 
+from ..utils.image_processing import rescale_image
 from ..utils.file_handler import manual_annotation_save
 from ..xradia_properties import AnnotationTypes, XrmDataTypes as XDT
 
 font_path = Path(__file__).parent.parent / "font" / "CallingCode-Regular.otf"
 
 
 class AnnotatorMixin:
@@ -40,15 +41,17 @@
         annotations = self.extract_annotations(scale_bar=scale_bar)
         # Checks if anything has been added
         if annotations is None:
             logging.warning("No annotations to apply")
             self.annotated_image = None
         else:
             # Annotations will be in the wrong place if flipped
-            images = self.get_output(flip=False, clear_images=False)
+            images = rescale_image(
+                self.get_output(flip=False, clear_images=False), 0, 255
+            )
             self.annotated_image = self.apply_annotations(images, annotations)
         return self.annotated_image
 
     @property
     def thickness_modifier(self) -> float:
         """This set a multiplier so that lines are visible when the image is at a sensible size"""
         if not hasattr(self, "output_shape"):
@@ -93,17 +96,21 @@
             RGB numpy array or None: Annotated images, if successfully applied
         """
         try:
             # Create output array with shape of input, plus 3 channels for RGB
             output_images = np.zeros((*images.shape, 3), dtype="uint8")
             for idx, image in enumerate(images, 0):
                 # Make 'L' type PIL image from 2D array, autocontrast, then convert to RGBA
-                image = autocontrast(Image.fromarray(image).convert("L")).convert(
-                    "RGBA"
-                )
+                image = Image.fromarray(image).convert("L")
+                image_auto_contrasted = autocontrast(image)
+                if np.mean(image_auto_contrasted) == np.max(image_auto_contrasted):
+                    image = image_auto_contrasted
+                else:
+                    del image_auto_contrasted
+                image = image.convert("RGBA")
                 # Combine annotations and image by alpha
                 image.alpha_composite(annotations)
                 # Throw away alpha and fill into output array
                 output_images[idx] = image.convert("RGB")
             return output_images
         except Exception:
             logging.error("Failed to apply annotations", exc_info=True)
```

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/txrm/main.py` & `txrm2tiff-2.0.8/src/txrm2tiff/txrm/main.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/txrm/ref_mixin.py` & `txrm2tiff-2.0.8/src/txrm2tiff/txrm/ref_mixin.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/txrm/save_mixin.py` & `txrm2tiff-2.0.8/src/txrm2tiff/txrm/save_mixin.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/txrm/shifts_mixin.py` & `txrm2tiff-2.0.8/src/txrm2tiff/txrm/shifts_mixin.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/txrm/txrm_property.py` & `txrm2tiff-2.0.8/src/txrm2tiff/txrm/txrm_property.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/txrm/v3.py` & `txrm2tiff-2.0.8/src/txrm2tiff/txrm/v3.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/txrm/v5.py` & `txrm2tiff-2.0.8/src/txrm2tiff/txrm/v5.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/txrm_functions/general.py` & `txrm2tiff-2.0.8/src/txrm2tiff/txrm_functions/general.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/txrm_functions/images.py` & `txrm2tiff-2.0.8/src/txrm2tiff/txrm_functions/images.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/utils/file_handler.py` & `txrm2tiff-2.0.8/src/txrm2tiff/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/utils/image_processing.py` & `txrm2tiff-2.0.8/src/txrm2tiff/utils/image_processing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import List
 import numpy as np
-from numpy.typing import DTypeLike
+from numpy.typing import DTypeLike, NDArray
 
 from .functions import convert_to_int
 
 
 def dynamic_despeckle_and_average_series(
     images: np.ndarray, average: bool = True
 ) -> np.ndarray:
@@ -62,19 +62,25 @@
     # that can lead to the normalised image to be dark:
     if clip:
         num_std = 3.0
         logging.info("Clipping outliers (>%g std from mean)", num_std)
         new_max = np.mean(array) + num_std * np.std(array)
         np.clip(array, 0, new_max, out=array)
 
-    # Move minimum value of all corrected images to 0:
-    array -= array.min()
-    # New max should be the max allowed by datatype
-    new_max = np.iinfo(datatype).max
-    return array * (new_max / array.max())
+    return rescale_image(array, np.iinfo(datatype).min, np.iinfo(datatype).max)
+
+
+def rescale_image(
+    array, minimum, maximum, previous_minimum=None, previous_maximum=None
+):
+    if previous_minimum is None:
+        previous_minimum = np.min(array)
+    if previous_maximum is None:
+        previous_maximum = np.max(array)
+    return np.interp(array, (previous_minimum, previous_maximum), (minimum, maximum))
 
 
 def cast_to_dtype(image: np.ndarray, data_type: DTypeLike) -> np.ndarray:
     try:
         dtype = np.dtype(data_type)
         if dtype is image.dtype:
             logging.debug("Image is already %s", dtype)
@@ -102,15 +108,15 @@
                     "Image max %f above %s maximum of %i, values above this will be cut off",
                     img_max,
                     dtype,
                     dtype_max,
                 )
             else:
                 dtype_max = None
-            
+
             if dtype_min is not None or dtype_max is not None:
                 np.clip(image, dtype_min, dtype_max, out=image)
 
             if np.issubdtype(dtype, np.integer) and np.issubdtype(
                 image.dtype, np.floating
             ):
                 image = np.around(image, decimals=0)
@@ -141,17 +147,15 @@
 ) -> np.ndarray:
     ref_num_rows = convert_to_int(image_rows / mosaic_rows)
     ref_num_columns = convert_to_int(image_columns / mosaic_columns)
     refdata.shape = (ref_num_rows, ref_num_columns)
     return np.tile(refdata, (mosaic_rows, mosaic_columns))
 
 
-def stitch_images(
-    images: np.ndarray, mosaic_dims: List[int]
-) -> np.ndarray:
+def stitch_images(images: np.ndarray, mosaic_dims: List[int]) -> np.ndarray:
     """
     Stitches images into a mosaic stored as a 2D array.
 
     Mosaic dims should be X, Y.
     """
     # Convert to Y X for numpy:
     slow_np_axis = 0
```

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/utils/logging.py` & `txrm2tiff-2.0.8/src/txrm2tiff/utils/logging.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/utils/metadata.py` & `txrm2tiff-2.0.8/src/txrm2tiff/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/utils/shortcut_creation.py` & `txrm2tiff-2.0.8/src/txrm2tiff/utils/shortcut_creation.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/xradia_properties/enums.py` & `txrm2tiff-2.0.8/src/txrm2tiff/xradia_properties/enums.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff/xradia_properties/stream_dtypes.py` & `txrm2tiff-2.0.8/src/txrm2tiff/xradia_properties/stream_dtypes.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff.egg-info/PKG-INFO` & `txrm2tiff-2.0.8/src/txrm2tiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txrm2tiff
-Version: 2.0.7
+Version: 2.0.8
 Summary: A converter for Zeiss txrm and xrm files, created by & for B24 of Diamond Light Source
 Author-email: Thomas Fish <thomas.fish@diamond.ac.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `txrm2tiff-2.0.7/src/txrm2tiff.egg-info/SOURCES.txt` & `txrm2tiff-2.0.8/src/txrm2tiff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_abstract_txrm.py` & `txrm2tiff-2.0.8/tests/test_abstract_txrm.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_annotator.py` & `txrm2tiff-2.0.8/tests/test_annotator.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,17 +240,19 @@
             def thickness_modifier(self) -> float:
                 return 1
 
         fill = (0, 125, 0)
         x0, x1 = 1, 4
         y = 4
         im = np.zeros((5, 6, 7), dtype=np.uint8)  # Z, Y, X
+        im[0, 0, 0] = 255  # Ensure range stays the same as it is cast to 'L' (uint8)
+        im = np.flip(im, axis=1)
         num_annotations = 1
         ann = TestAnnotator()
-        ann.get_output = MagicMock(return_value=np.flip(im, axis=1))
+        ann.get_output = MagicMock(return_value=im)
         ann.output_shape = im.shape
         ann.has_stream = MagicMock(return_value=True)
         ann.read_stream = MagicMock(
             side_effect=[  # Draw a single line with the listed points
                 [num_annotations],
                 [AnnotationTypes.ANN_LINE.value],
                 [x0],
@@ -276,16 +278,16 @@
                 call("Annot/Ann0/X1", XrmDataTypes.XRM_FLOAT, strict=True),
                 call("Annot/Ann0/X2", XrmDataTypes.XRM_FLOAT, strict=True),
                 call("Annot/Ann0/Y1", XrmDataTypes.XRM_FLOAT, strict=True),
                 call("Annot/Ann0/Y2", XrmDataTypes.XRM_FLOAT, strict=True),
             ]
         )
 
-        # Extra 3 at the end for RGB
-        expected_output = np.zeros((*im.shape, 3), dtype=np.uint8)
+        # Extra axis of length 3 for RGB
+        expected_output = np.stack([im] * 3, axis=3)
         y = expected_output.shape[1] - 1 - y  # Invert y axis
         expected_output[:, y, x0 : x1 + 1, :] = fill
         self.assertEqual(
             ann.annotated_image.shape, expected_output.shape, msg="Shapes don't match"
         )
         unequal_pos = np.where(ann.annotated_image != expected_output)
         assert_array_equal(
```

### Comparing `txrm2tiff-2.0.7/tests/test_commandline_entrypoint.py` & `txrm2tiff-2.0.8/tests/test_commandline_entrypoint.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_file_handler.py` & `txrm2tiff-2.0.8/tests/test_file_handler.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_image_processing.py` & `txrm2tiff-2.0.8/tests/test_image_processing.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import numpy as np
 
 from txrm2tiff.utils.image_processing import (
     cast_to_dtype,
     dynamic_despeckle_and_average_series,
     stitch_images,
+    rescale_image,
 )
 
 
 class TestImageProcessing(unittest.TestCase):
     def test_stitch_mosaic(self):
         mosaic_xy_shape = (3, 4)
         image_size = (400, 400)
@@ -70,14 +71,41 @@
             )  # Should not be almost equal until despeckle & averaging
         assert_array_almost_equal(
             dynamic_despeckle_and_average_series(custom_reference),
             expected_approx_output,
             decimal=0,
         )
 
+    def test_rescale_image(self):
+        original_minimum = -6000
+        original_maximum = 6000
+        step_size = 500
+
+        target_minimum = -600
+        target_maximum = 600
+        expected_step_size = 50
+
+        array = np.arange(original_minimum, original_maximum + step_size, step_size)
+        output_array = rescale_image(
+            array, target_minimum, target_maximum, original_minimum, original_maximum
+        )
+        self.assertEqual(output_array[0], target_minimum)
+        self.assertEqual(output_array[-1], target_maximum)
+        self.assertEqual(output_array[1] - output_array[0], expected_step_size)
+
+    def test_rescale_image_keep_range(self):
+        target_minimum = 0
+        target_maximum = 255
+        array = np.zeros((5, 5), np.uint8)
+        array[0, 0] = 255
+
+        output_array = rescale_image(array, target_minimum, target_maximum)
+        self.assertTrue(np.all(output_array[1:] == target_minimum))
+        self.assertEqual(output_array[0, 0], target_maximum)
+
     def test_cast_to_dtype_with_no_change(self):
         dtype = np.float64
         info = np.finfo(dtype)
         min, max = info.min, info.max
         image = np.asarray([min, max], dtype=dtype)
         output = cast_to_dtype(image, dtype)
         assert_array_equal(image, output)
```

### Comparing `txrm2tiff-2.0.7/tests/test_inspector.py` & `txrm2tiff-2.0.8/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_main.py` & `txrm2tiff-2.0.8/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_metadata.py` & `txrm2tiff-2.0.8/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_referencer.py` & `txrm2tiff-2.0.8/tests/test_referencer.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_saver.py` & `txrm2tiff-2.0.8/tests/test_saver.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_setup_fuctions.py` & `txrm2tiff-2.0.8/tests/test_setup_fuctions.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_shifts.py` & `txrm2tiff-2.0.8/tests/test_shifts.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_txrm_functions.py` & `txrm2tiff-2.0.8/tests/test_txrm_functions.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_txrm_property.py` & `txrm2tiff-2.0.8/tests/test_txrm_property.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_txrm_v5.py` & `txrm2tiff-2.0.8/tests/test_txrm_v5.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_txrmv3.py` & `txrm2tiff-2.0.8/tests/test_txrmv3.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_util_functions.py` & `txrm2tiff-2.0.8/tests/test_util_functions.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.7/tests/test_with_files.py` & `txrm2tiff-2.0.8/tests/test_with_files.py`

 * *Files identical despite different names*

