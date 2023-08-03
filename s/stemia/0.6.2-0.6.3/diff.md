# Comparing `tmp/stemia-0.6.2.tar.gz` & `tmp/stemia-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stemia-0.6.2.tar", last modified: Wed Aug  2 17:04:16 2023, max compression
+gzip compressed data, was "stemia-0.6.3.tar", last modified: Thu Aug  3 08:48:53 2023, max compression
```

## Comparing `stemia-0.6.2.tar` & `stemia-0.6.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.912599 stemia-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.900599 stemia-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.904599 stemia-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-02 17:03:57.000000 stemia-0.6.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 17:03:57.000000 stemia-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 17:03:57.000000 stemia-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-08-02 17:04:16.912599 stemia-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-08-02 17:03:57.000000 stemia-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.904599 stemia-0.6.2/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-08-02 17:03:57.000000 stemia-0.6.2/docs/generate_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-02 17:03:57.000000 stemia-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 17:04:16.912599 stemia-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.904599 stemia-0.6.2/stemia/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-02 17:04:16.000000 stemia-0.6.2/stemia/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.904599 stemia-0.6.2/stemia/aretomo/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/aretomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/aretomo/aln2xf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/aretomo/batch.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.904599 stemia-0.6.2/stemia/aretomo/batch_warp/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/aretomo/batch_warp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/aretomo/batch_warp/aretomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/aretomo/batch_warp/fix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/aretomo/batch_warp/fix_mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/aretomo/batch_warp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/aretomo/batch_warp/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/aretomo/batch_warp/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/aretomo/batch_warp/threaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/aretomo/batch_warp/topaz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.908599 stemia-0.6.2/stemia/cryosparc/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/cryosparc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.908599 stemia-0.6.2/stemia/cryosparc/csplot/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/cryosparc/csplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/cryosparc/csplot/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/cryosparc/csplot/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/cryosparc/csplot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/cryosparc/fix_filament_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/cryosparc/generate_tilt_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/cryosparc/merge_defects_gainref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.908599 stemia-0.6.2/stemia/image/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.908599 stemia-0.6.2/stemia/image/center_filament/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/image/center_filament/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2696 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/image/center_filament/center_filament.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/image/center_filament/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/image/create_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/image/extract_z_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/image/flip_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/image/fourier_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/image/rescale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.908599 stemia-0.6.2/stemia/imod/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/imod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/imod/find_NAD_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.908599 stemia-0.6.2/stemia/relion/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/relion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/relion/align_filament_particles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.908599 stemia-0.6.2/stemia/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/utils/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/utils/io_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.912599 stemia-0.6.2/stemia/warp/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/warp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/warp/fix_mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/warp/offset_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/warp/parse_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/warp/prepare_isonet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/warp/preprocess_serialem.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/warp/spoof_mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-02 17:03:57.000000 stemia-0.6.2/stemia/warp/summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:04:16.904599 stemia-0.6.2/stemia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-08-02 17:04:16.000000 stemia-0.6.2/stemia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-08-02 17:04:16.000000 stemia-0.6.2/stemia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:04:16.000000 stemia-0.6.2/stemia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:04:16.000000 stemia-0.6.2/stemia.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:04:16.000000 stemia-0.6.2/stemia.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-02 17:04:16.000000 stemia-0.6.2/stemia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 17:04:16.000000 stemia-0.6.2/stemia.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.967450 stemia-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.959450 stemia-0.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.963450 stemia-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-03 08:48:32.000000 stemia-0.6.3/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 08:48:32.000000 stemia-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 08:48:32.000000 stemia-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-08-03 08:48:53.967450 stemia-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-08-03 08:48:32.000000 stemia-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.963450 stemia-0.6.3/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-08-03 08:48:32.000000 stemia-0.6.3/docs/generate_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-03 08:48:32.000000 stemia-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-03 08:48:53.967450 stemia-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.963450 stemia-0.6.3/stemia/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 08:48:53.000000 stemia-0.6.3/stemia/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.963450 stemia-0.6.3/stemia/aretomo/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/aretomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/aretomo/aln2xf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/aretomo/batch.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.963450 stemia-0.6.3/stemia/aretomo/batch_warp/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/aretomo/batch_warp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/aretomo/batch_warp/aretomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/aretomo/batch_warp/fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/aretomo/batch_warp/fix_mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/aretomo/batch_warp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/aretomo/batch_warp/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/aretomo/batch_warp/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/aretomo/batch_warp/threaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/aretomo/batch_warp/topaz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.963450 stemia-0.6.3/stemia/cryosparc/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/cryosparc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.963450 stemia-0.6.3/stemia/cryosparc/csplot/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/cryosparc/csplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/cryosparc/csplot/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/cryosparc/csplot/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/cryosparc/csplot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/cryosparc/fix_filament_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/cryosparc/generate_tilt_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/cryosparc/merge_defects_gainref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.967450 stemia-0.6.3/stemia/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.967450 stemia-0.6.3/stemia/image/center_filament/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/image/center_filament/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2696 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/image/center_filament/center_filament.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/image/center_filament/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/image/create_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/image/extract_z_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/image/flip_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/image/fourier_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/image/rescale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.967450 stemia-0.6.3/stemia/imod/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/imod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/imod/find_NAD_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.967450 stemia-0.6.3/stemia/relion/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/relion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/relion/align_filament_particles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.967450 stemia-0.6.3/stemia/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/utils/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/utils/io_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.967450 stemia-0.6.3/stemia/warp/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/warp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/warp/fix_mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/warp/offset_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/warp/parse_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/warp/prepare_isonet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/warp/preprocess_serialem.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/warp/spoof_mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-03 08:48:32.000000 stemia-0.6.3/stemia/warp/summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:53.963450 stemia-0.6.3/stemia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-08-03 08:48:53.000000 stemia-0.6.3/stemia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-08-03 08:48:53.000000 stemia-0.6.3/stemia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:48:53.000000 stemia-0.6.3/stemia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:48:53.000000 stemia-0.6.3/stemia.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:48:53.000000 stemia-0.6.3/stemia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-03 08:48:53.000000 stemia-0.6.3/stemia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 08:48:53.000000 stemia-0.6.3/stemia.egg-info/top_level.txt
```

### Comparing `stemia-0.6.2/.github/workflows/deploy.yml` & `stemia-0.6.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/LICENSE` & `stemia-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/PKG-INFO` & `stemia-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemia
-Version: 0.6.2
+Version: 0.6.3
 Summary: Scripts and Tools for Electron Microscopy Analysis.
 Home-page: https://github.com/brisvag/stemia/
 Author: Lorenzo Gaifas
 Author-email: brisvag@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `stemia-0.6.2/README.md` & `stemia-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/docs/generate_readme.py` & `stemia-0.6.3/docs/generate_readme.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/setup.cfg` & `stemia-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/aretomo/aln2xf.py` & `stemia-0.6.3/stemia/aretomo/aln2xf.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/aretomo/batch_warp/aretomo.py` & `stemia-0.6.3/stemia/aretomo/batch_warp/aretomo.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/aretomo/batch_warp/fix.py` & `stemia-0.6.3/stemia/aretomo/batch_warp/fix.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/aretomo/batch_warp/fix_mdoc.py` & `stemia-0.6.3/stemia/aretomo/batch_warp/fix_mdoc.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/aretomo/batch_warp/main.py` & `stemia-0.6.3/stemia/aretomo/batch_warp/main.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/aretomo/batch_warp/parse.py` & `stemia-0.6.3/stemia/aretomo/batch_warp/parse.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/aretomo/batch_warp/stack.py` & `stemia-0.6.3/stemia/aretomo/batch_warp/stack.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/aretomo/batch_warp/threaded.py` & `stemia-0.6.3/stemia/aretomo/batch_warp/threaded.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/aretomo/batch_warp/topaz.py` & `stemia-0.6.3/stemia/aretomo/batch_warp/topaz.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/cryosparc/csplot/main.py` & `stemia-0.6.3/stemia/cryosparc/csplot/main.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/cryosparc/csplot/parse.py` & `stemia-0.6.3/stemia/cryosparc/csplot/parse.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/cryosparc/csplot/plot.py` & `stemia-0.6.3/stemia/cryosparc/csplot/plot.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/cryosparc/fix_filament_ids.py` & `stemia-0.6.3/stemia/cryosparc/fix_filament_ids.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/cryosparc/generate_tilt_angles.py` & `stemia-0.6.3/stemia/cryosparc/generate_tilt_angles.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/cryosparc/merge_defects_gainref.py` & `stemia-0.6.3/stemia/cryosparc/merge_defects_gainref.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/image/center_filament/center_filament.py` & `stemia-0.6.3/stemia/image/center_filament/center_filament.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/image/center_filament/funcs.py` & `stemia-0.6.3/stemia/image/center_filament/funcs.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/image/create_mask.py` & `stemia-0.6.3/stemia/image/create_mask.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/image/extract_z_snapshots.py` & `stemia-0.6.3/stemia/image/extract_z_snapshots.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/image/flip_z.py` & `stemia-0.6.3/stemia/image/flip_z.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/image/fourier_crop.py` & `stemia-0.6.3/stemia/image/fourier_crop.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/image/rescale.py` & `stemia-0.6.3/stemia/image/rescale.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/imod/find_NAD_params.py` & `stemia-0.6.3/stemia/imod/find_NAD_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,17 +33,17 @@
         def _process_output(task, line):
             if it_n.match(line):
                 progress.update(task, advance=1)
 
         procs = []
         for k_ in ks:
             k = k_ * std
-            out = inp.with_stem(inp.stem + f'-{k:.5f}_i').with_suffix('')
+            out = inp.with_stem(inp.stem + f'-{k}_i').with_suffix('')
 
-            task = progress.add_task(f'Iterating with k={k:.5f} ({k_} * std)...', total=max_it)
+            task = progress.add_task(f'Iterating with k={k} ({k_} * std)...', total=max_it)
 
             proc = sh.nad_eed_3d(
                 '-k', k,
                 '-i', iterations,
                 '-e', 'mrc',
                 str(inp),
                 str(out),
```

### Comparing `stemia-0.6.2/stemia/relion/align_filament_particles.py` & `stemia-0.6.3/stemia/relion/align_filament_particles.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/utils/click.py` & `stemia-0.6.3/stemia/utils/click.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/utils/image_processing.py` & `stemia-0.6.3/stemia/utils/image_processing.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/utils/io_.py` & `stemia-0.6.3/stemia/utils/io_.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/warp/fix_mdoc.py` & `stemia-0.6.3/stemia/warp/fix_mdoc.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/warp/offset_angle.py` & `stemia-0.6.3/stemia/warp/offset_angle.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/warp/prepare_isonet.py` & `stemia-0.6.3/stemia/warp/prepare_isonet.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/warp/preprocess_serialem.sh` & `stemia-0.6.3/stemia/warp/preprocess_serialem.sh`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/warp/spoof_mdoc.py` & `stemia-0.6.3/stemia/warp/spoof_mdoc.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia/warp/summarize.py` & `stemia-0.6.3/stemia/warp/summarize.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.2/stemia.egg-info/PKG-INFO` & `stemia-0.6.3/stemia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemia
-Version: 0.6.2
+Version: 0.6.3
 Summary: Scripts and Tools for Electron Microscopy Analysis.
 Home-page: https://github.com/brisvag/stemia/
 Author: Lorenzo Gaifas
 Author-email: brisvag@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `stemia-0.6.2/stemia.egg-info/SOURCES.txt` & `stemia-0.6.3/stemia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

