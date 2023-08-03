# Comparing `tmp/reaxpro-wrappers-1.3.0.tar.gz` & `tmp/reaxpro-wrappers-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaxpro-wrappers-1.3.0.tar", last modified: Wed Aug  2 12:12:45 2023, max compression
+gzip compressed data, was "reaxpro-wrappers-1.3.1.tar", last modified: Thu Aug  3 14:14:28 2023, max compression
```

## Comparing `reaxpro-wrappers-1.3.0.tar` & `reaxpro-wrappers-1.3.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.532789 reaxpro-wrappers-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-08-02 12:12:45.532789 reaxpro-wrappers-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.520789 reaxpro-wrappers-1.3.0/osp/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.520789 reaxpro-wrappers-1.3.0/osp/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.524789 reaxpro-wrappers-1.3.0/osp/dictionaries/ams/
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/ams/co_pt111_meso.json
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/ams/energy_landscape.json
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/ams/pesexploration.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.524789 reaxpro-wrappers-1.3.0/osp/dictionaries/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/defaults/defaults_AMS.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.524789 reaxpro-wrappers-1.3.0/osp/dictionaries/energies/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/energies/gas_energies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.524789 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/CO_ads+Pt111.xyz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/lattice_input.dat
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state1.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state2.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state3.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state4.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state5.xyz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.524789 reaxpro-wrappers-1.3.0/osp/models/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/models/ams/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/ams/energy_landscape_refinement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/models/multiscale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/multiscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/multiscale/co_pt111_meso.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/models/settings/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/settings/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/utils/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/models/zacros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/zacros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49172 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/zacros/co_pyzacros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/tools/graph_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27318 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/tools/io_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    75884 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/tools/mapping_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/tools/set_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/wrappers/simams/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/wrappers/simams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/wrappers/simams/simams_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.532789 reaxpro-wrappers-1.3.0/osp/wrappers/simzacros/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/wrappers/simzacros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/wrappers/simzacros/simzacros_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.532789 reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-08-02 12:12:45.000000 reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-02 12:12:45.000000 reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:12:45.000000 reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 12:12:45.000000 reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-02 12:12:45.000000 reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-02 12:12:45.000000 reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-02 12:12:45.532789 reaxpro-wrappers-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.532789 reaxpro-wrappers-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/tests/test_energy_landscape_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/tests/test_pyzacros_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.576191 reaxpro-wrappers-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-08-03 14:14:28.576191 reaxpro-wrappers-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.568190 reaxpro-wrappers-1.3.1/osp/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.568190 reaxpro-wrappers-1.3.1/osp/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.568190 reaxpro-wrappers-1.3.1/osp/dictionaries/ams/
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/ams/co_pt111_meso.json
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/ams/energy_landscape.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/ams/pesexploration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.568190 reaxpro-wrappers-1.3.1/osp/dictionaries/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/defaults/defaults_AMS.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.568190 reaxpro-wrappers-1.3.1/osp/dictionaries/energies/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/energies/gas_energies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.572190 reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/CO_ads+Pt111.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/lattice_input.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/state1.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/state2.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/state3.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/state4.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/state5.xyz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.572190 reaxpro-wrappers-1.3.1/osp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.572190 reaxpro-wrappers-1.3.1/osp/models/ams/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/models/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/models/ams/energy_landscape_refinement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.572190 reaxpro-wrappers-1.3.1/osp/models/multiscale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/models/multiscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20603 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/models/multiscale/co_pt111_meso.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.572190 reaxpro-wrappers-1.3.1/osp/models/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/models/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/models/settings/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.572190 reaxpro-wrappers-1.3.1/osp/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/models/utils/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.572190 reaxpro-wrappers-1.3.1/osp/models/zacros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/models/zacros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49172 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/models/zacros/co_pyzacros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.576191 reaxpro-wrappers-1.3.1/osp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/tools/graph_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27318 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/tools/io_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75884 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/tools/mapping_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/tools/set_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.576191 reaxpro-wrappers-1.3.1/osp/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.576191 reaxpro-wrappers-1.3.1/osp/wrappers/simams/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/wrappers/simams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/wrappers/simams/simams_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.576191 reaxpro-wrappers-1.3.1/osp/wrappers/simzacros/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/wrappers/simzacros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/osp/wrappers/simzacros/simzacros_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.576191 reaxpro-wrappers-1.3.1/reaxpro_wrappers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-08-03 14:14:28.000000 reaxpro-wrappers-1.3.1/reaxpro_wrappers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-03 14:14:28.000000 reaxpro-wrappers-1.3.1/reaxpro_wrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:14:28.000000 reaxpro-wrappers-1.3.1/reaxpro_wrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 14:14:28.000000 reaxpro-wrappers-1.3.1/reaxpro_wrappers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-03 14:14:28.000000 reaxpro-wrappers-1.3.1/reaxpro_wrappers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-03 14:14:28.000000 reaxpro-wrappers-1.3.1/reaxpro_wrappers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-03 14:14:28.580191 reaxpro-wrappers-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:28.576191 reaxpro-wrappers-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/tests/test_energy_landscape_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/tests/test_pyzacros_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-03 14:14:09.000000 reaxpro-wrappers-1.3.1/tests/test_tools.py
```

### Comparing `reaxpro-wrappers-1.3.0/LICENSE` & `reaxpro-wrappers-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/PKG-INFO` & `reaxpro-wrappers-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxpro-wrappers
-Version: 1.3.0
+Version: 1.3.1
 Summary: The wrapper of AMS and Zacros drivers for SimPhoNy
 Home-page: https://www.esciencecenter.nl/
 Author: Netherlands eScience Center, Fraunhofer IWM
 Keywords: simphony,cuds,AMS,zacros,SCM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `reaxpro-wrappers-1.3.0/README.md` & `reaxpro-wrappers-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json` & `reaxpro-wrappers-1.3.1/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/dictionaries/ams/co_pt111_meso.json` & `reaxpro-wrappers-1.3.1/osp/dictionaries/ams/co_pt111_meso.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/dictionaries/ams/energy_landscape.json` & `reaxpro-wrappers-1.3.1/osp/dictionaries/ams/energy_landscape.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/dictionaries/defaults/defaults_AMS.yaml` & `reaxpro-wrappers-1.3.1/osp/dictionaries/defaults/defaults_AMS.yaml`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/CO_ads+Pt111.xyz` & `reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/CO_ads+Pt111.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/lattice_input.dat` & `reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/lattice_input.dat`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state1.xyz` & `reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/state1.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state2.xyz` & `reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/state2.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state3.xyz` & `reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/state3.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state4.xyz` & `reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/state4.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state5.xyz` & `reaxpro-wrappers-1.3.1/osp/dictionaries/example_data/state5.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/models/ams/energy_landscape_refinement.py` & `reaxpro-wrappers-1.3.1/osp/models/ams/energy_landscape_refinement.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/models/multiscale/co_pt111_meso.py` & `reaxpro-wrappers-1.3.1/osp/models/multiscale/co_pt111_meso.py`

 * *Files 0% similar despite different names*

```diff
@@ -483,32 +483,32 @@
     zgb_model: ZGBModel = Field(
         ..., description="ZGB model for mesoscopic scale."
     )
 
     def __post_init_post_parse__(self):
         with CoreSession() as session:
             workflow = emmo.Workflow()
-            workflow.add(self.pes_exploration.cuds, rel=emmo.hasSpatialFirst)
             self.pes_exploration.cuds.add(self.binding_site.cuds, rel=emmo.hasSpatialNext)
-            workflow.add(self.binding_site.cuds, rel=emmo.hasSpatialDirectPart)
             self.binding_site.cuds.add(self.zgb_model.cuds, rel=emmo.hasSpatialNext)
-            workflow.add(self.zgb_model.cuds, rel=emmo.hasSpatialLast)
             for oclass in [
                     emmo.ForceFieldIdentifierString,
                     emmo.Solver,
                     emmo.FixedRegion,
                     emmo.MaximumEnergy,
                     emmo.NeighborCutoff,
                     emmo.ReferenceRegion,
                     emmo.RandomSeed,
                     emmo.MolecularGeometry,
                     crystallography.UnitCell
                 ]:
                 input_cuds = self.pes_exploration.cuds.get(oclass=oclass, rel=emmo.hasInput)
-                self.binding_site.cuds.add(input_cuds.pop(), rel=emmo.hasInput)
+            self.binding_site.cuds.add(input_cuds.pop(), rel=emmo.hasInput)
+            workflow.add(self.pes_exploration.cuds, rel=emmo.hasSpatialFirst)
+            workflow.add(self.binding_site.cuds, rel=emmo.hasSpatialDirectPart)
+            workflow.add(self.zgb_model.cuds, rel=emmo.hasSpatialLast)
         file = tempfile.NamedTemporaryFile(suffix=".ttl", delete=False)
         export_cuds(session, file.name)
         self._file = file.name
         try:
             self._uuid = get_upload(file)
         except Exception as error:
             self._uuid = None
```

### Comparing `reaxpro-wrappers-1.3.0/osp/models/settings/general.py` & `reaxpro-wrappers-1.3.1/osp/models/settings/general.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/models/utils/general.py` & `reaxpro-wrappers-1.3.1/osp/models/utils/general.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/models/zacros/co_pyzacros.py` & `reaxpro-wrappers-1.3.1/osp/models/zacros/co_pyzacros.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/tools/graph_functions.py` & `reaxpro-wrappers-1.3.1/osp/tools/graph_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/tools/io_functions.py` & `reaxpro-wrappers-1.3.1/osp/tools/io_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/tools/mapping_functions.py` & `reaxpro-wrappers-1.3.1/osp/tools/mapping_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/tools/set_functions.py` & `reaxpro-wrappers-1.3.1/osp/tools/set_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/wrappers/simams/simams_session.py` & `reaxpro-wrappers-1.3.1/osp/wrappers/simams/simams_session.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/osp/wrappers/simzacros/simzacros_session.py` & `reaxpro-wrappers-1.3.1/osp/wrappers/simzacros/simzacros_session.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/PKG-INFO` & `reaxpro-wrappers-1.3.1/reaxpro_wrappers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxpro-wrappers
-Version: 1.3.0
+Version: 1.3.1
 Summary: The wrapper of AMS and Zacros drivers for SimPhoNy
 Home-page: https://www.esciencecenter.nl/
 Author: Netherlands eScience Center, Fraunhofer IWM
 Keywords: simphony,cuds,AMS,zacros,SCM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/SOURCES.txt` & `reaxpro-wrappers-1.3.1/reaxpro_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/setup.cfg` & `reaxpro-wrappers-1.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = reaxpro-wrappers
 author = Netherlands eScience Center, Fraunhofer IWM
 url = https://www.esciencecenter.nl/
-version = v1.3.0
+version = v1.3.1
 description = The wrapper of AMS and Zacros drivers for SimPhoNy
 keywords = simphony, cuds, AMS, zacros, SCM
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `reaxpro-wrappers-1.3.0/setup.py` & `reaxpro-wrappers-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/tests/test_energy_landscape_refinement.py` & `reaxpro-wrappers-1.3.1/tests/test_energy_landscape_refinement.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/tests/test_examples.py` & `reaxpro-wrappers-1.3.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/tests/test_pyzacros_model.py` & `reaxpro-wrappers-1.3.1/tests/test_pyzacros_model.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.3.0/tests/test_tools.py` & `reaxpro-wrappers-1.3.1/tests/test_tools.py`

 * *Files identical despite different names*

