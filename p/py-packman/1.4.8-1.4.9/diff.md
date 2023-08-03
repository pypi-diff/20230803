# Comparing `tmp/py-packman-1.4.8.tar.gz` & `tmp/py-packman-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-packman-1.4.8.tar", last modified: Mon Jul 17 20:50:44 2023, max compression
+gzip compressed data, was "py-packman-1.4.9.tar", last modified: Thu Aug  3 21:45:30 2023, max compression
```

## Comparing `py-packman-1.4.8.tar` & `py-packman-1.4.9.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-17 20:50:30.000000 py-packman-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-17 20:50:44.927688 py-packman-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-17 20:50:30.000000 py-packman-1.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.919688 py-packman-1.4.8/packman/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/anm/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/anm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/anm/anm.py
--rw-r--r--   0 runner    (1001) docker     (123)    43080 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/anm/hd_anm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/apps/calculate_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/apps/dci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/apps/hdanm.py
--rw-r--r--   0 runner    (1001) docker     (123)    19366 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/apps/predict_hinge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    37386 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/bin/GUI.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/bin/PACKMAN.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   200702 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/bin/logo.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/constants/
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/constants/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/entropy/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/entropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/entropy/entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/geometry/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/gnm/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/gnm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/gnm/gnm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/molecule/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/bond.py
--rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/hetmol.py
--rw-r--r--   0 runner    (1001) docker     (123)    41580 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    24426 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/protein.py
--rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/residue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/packman/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/packman/tests/anm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/anm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/anm/test_anm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/packman/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/data/1prw.hng
--rw-r--r--   0 runner    (1001) docker     (123)   151551 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/data/1prw.pdb
--rw-r--r--   0 runner    (1001) docker     (123)   355003 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/data/4hla.cif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/packman/tests/entropy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/entropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/entropy/test_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/packman/tests/molecule/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/molecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/molecule/test_molecule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/packman/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/utilities/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/py_packman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-17 20:50:44.000000 py-packman-1.4.8/py_packman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-17 20:50:44.000000 py-packman-1.4.8/py_packman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:50:44.000000 py-packman-1.4.8/py_packman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 20:50:44.000000 py-packman-1.4.8/py_packman.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-17 20:50:44.000000 py-packman-1.4.8/py_packman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 20:50:44.000000 py-packman-1.4.8/py_packman.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:50:44.927688 py-packman-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-17 20:50:30.000000 py-packman-1.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.220424 py-packman-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-03 21:45:20.000000 py-packman-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-08-03 21:45:30.220424 py-packman-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-08-03 21:45:20.000000 py-packman-1.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.208424 py-packman-1.4.9/packman/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.208424 py-packman-1.4.9/packman/anm/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/anm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/anm/anm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43080 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/anm/hd_anm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.208424 py-packman-1.4.9/packman/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/apps/calculate_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/apps/dci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/apps/hdanm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19366 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/apps/predict_hinge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.208424 py-packman-1.4.9/packman/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    37386 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/bin/GUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/bin/PACKMAN.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   200702 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/bin/logo.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.212424 py-packman-1.4.9/packman/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/constants/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.212424 py-packman-1.4.9/packman/entropy/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/entropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/entropy/entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.212424 py-packman-1.4.9/packman/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/geometry/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.212424 py-packman-1.4.9/packman/gnm/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/gnm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/gnm/gnm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.212424 py-packman-1.4.9/packman/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/molecule/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/molecule/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/molecule/bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/molecule/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/molecule/hetmol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41902 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/molecule/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24426 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/molecule/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/molecule/protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/molecule/residue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.212424 py-packman-1.4.9/packman/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.216424 py-packman-1.4.9/packman/tests/anm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/tests/anm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/tests/anm/test_anm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.216424 py-packman-1.4.9/packman/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/tests/data/1prw.hng
+-rw-r--r--   0 runner    (1001) docker     (123)   151551 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/tests/data/1prw.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)   355003 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/tests/data/4hla.cif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.216424 py-packman-1.4.9/packman/tests/entropy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/tests/entropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/tests/entropy/test_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.216424 py-packman-1.4.9/packman/tests/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/tests/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/tests/molecule/test_molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.216424 py-packman-1.4.9/packman/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-08-03 21:45:20.000000 py-packman-1.4.9/packman/utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:45:30.216424 py-packman-1.4.9/py_packman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-08-03 21:45:30.000000 py-packman-1.4.9/py_packman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-03 21:45:30.000000 py-packman-1.4.9/py_packman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 21:45:30.000000 py-packman-1.4.9/py_packman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-03 21:45:30.000000 py-packman-1.4.9/py_packman.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 21:45:30.000000 py-packman-1.4.9/py_packman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 21:45:30.000000 py-packman-1.4.9/py_packman.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 21:45:30.220424 py-packman-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-08-03 21:45:20.000000 py-packman-1.4.9/setup.py
```

### Comparing `py-packman-1.4.8/LICENSE` & `py-packman-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/PKG-INFO` & `py-packman-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-packman
-Version: 1.4.8
+Version: 1.4.9
 Summary: A software package for molecular PACKing and Motion ANalysis (PACKMAN)
 Home-page: https://github.com/Pranavkhade/PACKMAN
 Author: Pranav Khade
 Author-email: pranavk@iastate.edu
 License: MIT
 Keywords: protein,dynamics,protein packing,protein domain,protein hinge
 Classifier: Intended Audience :: Education
```

### Comparing `py-packman-1.4.8/README.md` & `py-packman-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/__init__.py` & `py-packman-1.4.9/packman/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 from .bin import *
 from .anm import *
 from .constants import *
 from .utilities import *
 
 
 #VERSION CHANGE HERE CHANGES IT IN docs AND setup.py
-__version__='1.4.8'
+__version__='1.4.9'
```

### Comparing `py-packman-1.4.8/packman/anm/__init__.py` & `py-packman-1.4.9/packman/anm/__init__.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/anm/anm.py` & `py-packman-1.4.9/packman/anm/anm.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/anm/hd_anm.py` & `py-packman-1.4.9/packman/anm/hd_anm.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/apps/__init__.py` & `py-packman-1.4.9/packman/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/apps/calculate_entropy.py` & `py-packman-1.4.9/packman/apps/calculate_entropy.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/apps/dci.py` & `py-packman-1.4.9/packman/apps/dci.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/apps/hdanm.py` & `py-packman-1.4.9/packman/apps/hdanm.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/apps/predict_hinge.py` & `py-packman-1.4.9/packman/apps/predict_hinge.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/bin/GUI.py` & `py-packman-1.4.9/packman/bin/GUI.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/bin/PACKMAN.py` & `py-packman-1.4.9/packman/bin/PACKMAN.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/bin/__init__.py` & `py-packman-1.4.9/packman/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/bin/logo.ico` & `py-packman-1.4.9/packman/bin/logo.ico`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/constants/Constants.py` & `py-packman-1.4.9/packman/constants/Constants.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/entropy/entropy.py` & `py-packman-1.4.9/packman/entropy/entropy.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/geometry/geometry.py` & `py-packman-1.4.9/packman/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/gnm/__init__.py` & `py-packman-1.4.9/packman/gnm/__init__.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/gnm/gnm.py` & `py-packman-1.4.9/packman/gnm/gnm.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/molecule/__init__.py` & `py-packman-1.4.9/packman/molecule/__init__.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/molecule/annotations.py` & `py-packman-1.4.9/packman/molecule/annotations.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/molecule/atom.py` & `py-packman-1.4.9/packman/molecule/atom.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/molecule/bond.py` & `py-packman-1.4.9/packman/molecule/bond.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/molecule/chain.py` & `py-packman-1.4.9/packman/molecule/chain.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/molecule/hetmol.py` & `py-packman-1.4.9/packman/molecule/hetmol.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/molecule/model.py` & `py-packman-1.4.9/packman/molecule/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -483,16 +483,22 @@
         for i in after_componets:
             if(i in before_components):
                 #All the unchanged componets after breaking the bridge
                 None
             else:
                 changed_components.append(i)
 
-        #Smaller component will be rotated to keep computational intensity low
-        to_rotate = list(changed_components[min((len(l), i) for i, l in enumerate(changed_components))[1]])
+        # Whatever component neighbour 1 is in, rotate that. This keeps $\vec{e_a}$ condition satisfied
+        if( self.__AllAtoms_inverse[neighbor1] in changed_components[0] ):
+            to_rotate = list(changed_components[0])
+        elif( self.__AllAtoms_inverse[neighbor1] in changed_components[1] ):
+            to_rotate = list(changed_components[1])
+        else:
+            logging.error('Atom :'+str(neighbor1.get_id())+' is not in the connected to the components')
+            return None
 
         #Setting up rotation matrix
         sn=numpy.sin(rotang)
         cs=numpy.cos(rotang)
         t=1-cs
 
         v2x = atom1.get_location()[0] - atom2.get_location()[0]
```

### Comparing `py-packman-1.4.8/packman/molecule/molecule.py` & `py-packman-1.4.9/packman/molecule/molecule.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/molecule/protein.py` & `py-packman-1.4.9/packman/molecule/protein.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/molecule/residue.py` & `py-packman-1.4.9/packman/molecule/residue.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/tests/anm/test_anm.py` & `py-packman-1.4.9/packman/tests/anm/test_anm.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/tests/data/1prw.pdb` & `py-packman-1.4.9/packman/tests/data/1prw.pdb`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/tests/data/4hla.cif` & `py-packman-1.4.9/packman/tests/data/4hla.cif`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/tests/entropy/test_entropy.py` & `py-packman-1.4.9/packman/tests/entropy/test_entropy.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/tests/molecule/test_molecule.py` & `py-packman-1.4.9/packman/tests/molecule/test_molecule.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/packman/utilities/utilities.py` & `py-packman-1.4.9/packman/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/py_packman.egg-info/PKG-INFO` & `py-packman-1.4.9/py_packman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-packman
-Version: 1.4.8
+Version: 1.4.9
 Summary: A software package for molecular PACKing and Motion ANalysis (PACKMAN)
 Home-page: https://github.com/Pranavkhade/PACKMAN
 Author: Pranav Khade
 Author-email: pranavk@iastate.edu
 License: MIT
 Keywords: protein,dynamics,protein packing,protein domain,protein hinge
 Classifier: Intended Audience :: Education
```

### Comparing `py-packman-1.4.8/py_packman.egg-info/SOURCES.txt` & `py-packman-1.4.9/py_packman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.8/setup.py` & `py-packman-1.4.9/setup.py`

 * *Files identical despite different names*

