# Comparing `tmp/scipion-em-imod-3.1.8.tar.gz` & `tmp/scipion-em-imod-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-imod-3.1.8.tar", last modified: Thu Apr 20 07:45:09 2023, max compression
+gzip compressed data, was "scipion-em-imod-3.1.9.tar", last modified: Thu Aug  3 08:45:25 2023, max compression
```

## Comparing `scipion-em-imod-3.1.8.tar` & `scipion-em-imod-3.1.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:09.096839 scipion-em-imod-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-20 07:45:09.096839 scipion-em-imod-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:09.092838 scipion-em-imod-3.1.8/imod/
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/file_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:09.092838 scipion-em-imod-3.1.8/imod/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_applyTransformationMatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_auto3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    24073 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_ctfCorrection.py
--rw-r--r--   0 runner    (1001) docker     (123)    24526 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_ctfEstimation_automatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_ctfEstimation_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_doseFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    28762 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_etomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_excludeViews.py
--rw-r--r--   0 runner    (1001) docker     (123)    40520 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_fiducialAlignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    26801 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_fiducialModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_goldBeadEraser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_goldBeadPicker3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_importSetOfCTFTomoSeries.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_importSetOfTM.py
--rw-r--r--   0 runner    (1001) docker     (123)    14231 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_tomoNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_tomoProjection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_tomoReconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_tsNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_xCorrPrealignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/protocol_xRaysEraser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols/script_imod_auto3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:09.092838 scipion-em-imod-3.1.8/imod/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/templates/automatic_tilt_series_alignment.json.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:09.092838 scipion-em-imod-3.1.8/imod/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38359 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/tests/test_protocols_imod.py
--rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:09.092838 scipion-em-imod-3.1.8/imod/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/viewers/viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14220 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/imod/viewers/views_tkinter_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:09.096839 scipion-em-imod-3.1.8/scipion_em_imod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-20 07:45:09.000000 scipion-em-imod-3.1.8/scipion_em_imod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-20 07:45:09.000000 scipion-em-imod-3.1.8/scipion_em_imod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:45:09.000000 scipion-em-imod-3.1.8/scipion_em_imod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 07:45:09.000000 scipion-em-imod-3.1.8/scipion_em_imod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 07:45:09.000000 scipion-em-imod-3.1.8/scipion_em_imod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 07:45:09.096839 scipion-em-imod-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-04-20 07:43:27.000000 scipion-em-imod-3.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:45:25.666467 scipion-em-imod-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-08-03 08:45:25.666467 scipion-em-imod-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:45:25.662467 scipion-em-imod-3.1.9/imod/
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/file_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:45:25.662467 scipion-em-imod-3.1.9/imod/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_applyTransformationMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_auto3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24073 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_ctfCorrection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24526 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_ctfEstimation_automatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_ctfEstimation_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_doseFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28762 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_etomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_excludeViews.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40585 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_fiducialAlignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26801 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_fiducialModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_goldBeadEraser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_goldBeadPicker3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_importSetOfCTFTomoSeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_importSetOfTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14194 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_tomoNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_tomoProjection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_tomoReconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15451 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_tsNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_xCorrPrealignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/protocol_xRaysEraser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols/script_imod_auto3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:45:25.662467 scipion-em-imod-3.1.9/imod/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/templates/automatic_tilt_series_alignment.json.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:45:25.662467 scipion-em-imod-3.1.9/imod/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38359 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/tests/test_protocols_imod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38785 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:45:25.662467 scipion-em-imod-3.1.9/imod/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/viewers/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14220 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/imod/viewers/views_tkinter_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:45:25.666467 scipion-em-imod-3.1.9/scipion_em_imod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-08-03 08:45:25.000000 scipion-em-imod-3.1.9/scipion_em_imod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-08-03 08:45:25.000000 scipion-em-imod-3.1.9/scipion_em_imod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:45:25.000000 scipion-em-imod-3.1.9/scipion_em_imod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 08:45:25.000000 scipion-em-imod-3.1.9/scipion_em_imod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 08:45:25.000000 scipion-em-imod-3.1.9/scipion_em_imod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:45:25.666467 scipion-em-imod-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-08-03 08:43:24.000000 scipion-em-imod-3.1.9/setup.py
```

### Comparing `scipion-em-imod-3.1.8/CHANGES.txt` & `scipion-em-imod-3.1.9/CHANGES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+3.1.9:
+  - fix binning for normalization protocols
+  - fix excluded views parsing
 3.1.8:
   - Reconstruction:
      - tomoWidth added to specify a width when reconstructing
      - Shift in Z is registered in tomogram origin
 
   - Ctf correction: Allows different size of ctf set and ts set. Only paired (TS-CTF) ones will be processed
 3.1.7:
```

### Comparing `scipion-em-imod-3.1.8/LICENSE` & `scipion-em-imod-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/PKG-INFO` & `scipion-em-imod-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-em-imod
-Version: 3.1.8
+Version: 3.1.9
 Summary: Plugin to use some of the Tomography tools from IMOD in Scipion
 Home-page: https://github.com/scipion-em/scipion-em-imod
 Author: J.M. De la Rosa, Federico P. de Isidro Gomez
 Author-email: delarosatrevin@scilifelab.se, fp.deisidro@cnb.csic.es
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-imod/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-imod/
```

### Comparing `scipion-em-imod-3.1.8/README.rst` & `scipion-em-imod-3.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/__init__.py` & `scipion-em-imod-3.1.9/imod/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from pyworkflow.gui import FileTreeProvider
 from pyworkflow.gui.project.utils import OS
 import pwem
 
 from .constants import IMOD_HOME, ETOMO_CMD, DEFAULT_VERSION, VERSIONS
 
 
-__version__ = '3.1.8'
+__version__ = '3.1.9'
 _logo = "icon.png"
 _references = ['Kremer1996', 'Mastronarde2017']
 
 
 def getImodEnv():
     """ This function allows to call imod outside this plugin. """
```

### Comparing `scipion-em-imod-3.1.8/imod/bibtex.py` & `scipion-em-imod-3.1.9/imod/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/constants.py` & `scipion-em-imod-3.1.9/imod/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/icon.png` & `scipion-em-imod-3.1.9/imod/icon.png`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/__init__.py` & `scipion-em-imod-3.1.9/imod/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_applyTransformationMatrix.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_applyTransformationMatrix.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_auto3d.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_auto3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_base.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_ctfCorrection.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_ctfCorrection.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_ctfEstimation_automatic.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_ctfEstimation_automatic.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_ctfEstimation_manual.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_ctfEstimation_manual.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_doseFilter.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_doseFilter.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_etomo.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_etomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_excludeViews.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_excludeViews.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,19 @@
 from .. import Plugin, utils
 from .protocol_base import ProtImodBase, OUTPUT_TILTSERIES_NAME
 
 
 class ProtImodExcludeViews(ProtImodBase):
     """
     excludeviews - Reversibly remove views from a tilt series stack
-    If you use this protocol, make sure tis output tilt series is use for everything else
+
+    By default, the protocol will remove disabled tilt images from the input TS.
+    Alternatively, you can provide a text file with a list of tilts to exclude.
+
+    If you use this protocol, make sure this output tilt series is use for everything else
     CTF estimation, per particle per tilt, tomogram reconstruction....
     More info:
         https://bio3d.colorado.edu/imod/doc/man/excludeviews.html
     """
 
     _label = 'Exclude views'
     _devStatus = BETA
@@ -94,15 +98,15 @@
         return self.excludeViewsInfoMatrix
 
     def getExcludedViewsFromMatrix(self, ts):
         """ Returns the indexes of the tilt to exclude for a
         specified tilt series read from de input file """
         matrix = self.getExcludedViewsFromFile()
 
-        pattern = matrix.get(ts.getTsId(), [])
+        pattern = matrix.get(ts.getTsId(), "")
 
         views = self.makeExclusionPatternAsList(pattern)
 
         # Return the matrix or an empty list
         return views
 
     def getExcludedViews(self, ts):
@@ -179,24 +183,25 @@
         self._store()
 
     # --------------------------- UTILS functions -----------------------------
 
     def makeExclusionPatternAsList(self, excludedViews):
         excludedViewsAsList = []
 
-        vector = excludedViews.split(',')
+        if excludedViews:
+            vector = excludedViews.split(',')
 
-        for element in vector:
-            elementVector = element.split('-')
+            for element in vector:
+                elementVector = element.split('-')
 
-            if len(elementVector) > 1:
-                for i in range(int(elementVector[0]), int(elementVector[1]) + 1):
-                    excludedViewsAsList.append(int(i))
-            else:
-                excludedViewsAsList.append(int(elementVector[0]))
+                if len(elementVector) > 1:
+                    for i in range(int(elementVector[0]), int(elementVector[1]) + 1):
+                        excludedViewsAsList.append(int(i))
+                else:
+                    excludedViewsAsList.append(int(elementVector[0]))
 
         return excludedViewsAsList
 
     # --------------------------- INFO functions ------------------------------
     def _summary(self):
         summary = []
         if self.TiltSeries:
```

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_fiducialAlignment.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_fiducialAlignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,14 +495,15 @@
             output.append(newTs)
 
             for index, tiltImage in enumerate(ts):
                 newTi = TiltImage()
                 newTi.copyInfo(tiltImage, copyId=True, copyTM=False)
                 newTi.setLocation(tiltImage.getLocation())
                 newTi.setTiltAngle(float(tltList[index]))
+                newTi.setAcquisition(tiltImage.getAcquisition())
 
                 if tiltImage.hasTransform():
                     transform = Transform()
                     previousTransform = tiltImage.getTransform().getMatrix()
                     newTransform = newTransformationMatricesList[:, :, index]
                     previousTransformArray = np.array(previousTransform)
                     newTransformArray = np.array(newTransform)
```

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_fiducialModel.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_fiducialModel.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_goldBeadEraser.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_goldBeadEraser.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_goldBeadPicker3d.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_goldBeadPicker3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_importSetOfCTFTomoSeries.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_importSetOfCTFTomoSeries.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_importSetOfTM.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_importSetOfTM.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_tomoNormalization.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_tomoNormalization.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
         form.addParam('inputSetOfTomograms',
                       params.PointerParam,
                       pointerClass='SetOfTomograms',
                       important=True,
                       label='Input set of tomograms')
 
         form.addParam('binning',
-                      params.FloatParam,
-                      default=1.0,
+                      params.IntParam,
+                      default=1,
                       label='Binning',
                       important=True,
                       help='Binning to be applied to the normalized tomograms '
                            'in IMOD convention. Volumes will be binned by the '
                            'given factor. Must be an integer bigger than 1')
 
         form.addParam('floatDensities',
@@ -233,51 +233,53 @@
         if self.getModeToOutput() is not None:
             runNewstack = True
             argsNewstack += " -ModeToOutput " + str(self.getModeToOutput())
 
         if runNewstack:
             Plugin.runImod(self, 'newstack', argsNewstack % paramsNewstack)
 
-        if self.binning.get() != 1:
+        binning = self.binning.get()
+
+        if binning != 1:
             if runNewstack:
                 path.moveFile(os.path.join(extraPrefix, os.path.basename(location)),
                               os.path.join(tmpPrefix, os.path.basename(location)))
                 inputTomoPath = os.path.join(tmpPrefix, os.path.basename(location))
             else:
                 inputTomoPath = location
 
             paramsBinvol = {
                 'input': inputTomoPath,
                 'output': os.path.join(extraPrefix, os.path.basename(location)),
-                'binning': self.binning.get(),
+                'binning': binning,
                 'antialias': self.antialias.get() + 1
             }
 
             argsBinvol = "-input %(input)s " \
                          "-output %(output)s " \
                          "-binning %(binning)d "\
                          "-antialias %(antialias)d "
 
             Plugin.runImod(self, 'binvol', argsBinvol % paramsBinvol)
 
         output = self.getOutputSetOfTomograms(self.inputSetOfTomograms.get(),
-                                              self.binning.get())
+                                              binning)
 
         newTomogram = Tomogram()
         newTomogram.copyInfo(tomo)
         newTomogram.setTsId(tomo.getTsId())
 
-        if not runNewstack and self.binning.get() == 1:
+        if not runNewstack and binning == 1:
             newTomogram.setLocation(location)
         else:
             location = os.path.join(extraPrefix, os.path.basename(location))
             newTomogram.setLocation(location)
 
-        if self.binning.get() > 1:
-            sr = tomo.getSamplingRate() * int(self.binning.get())
+        if binning > 1:
+            sr = tomo.getSamplingRate() * binning
 
             newTomogram.setSamplingRate(sr)
 
             # Set default tomogram origin
             newTomogram.setOrigin(newOrigin=None)
 
         else:
```

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_tomoProjection.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_tomoProjection.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_tomoReconstruction.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_tomoReconstruction.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_tsNormalization.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_tsNormalization.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         form.addParam('inputSetOfTiltSeries',
                       params.PointerParam,
                       pointerClass='SetOfTiltSeries',
                       important=True,
                       label='Input set of tilt-series')
 
         form.addParam('binning',
-                      params.FloatParam,
+                      params.IntParam,
                       default=1,
                       label='Binning',
                       important=True,
                       help='Binning to be applied to the normalized tilt-series '
                            'in IMOD convention. Images will be binned by the '
                            'given factor. Must be an integer bigger than 1')
 
@@ -215,15 +215,15 @@
 
         xfFile = None
 
         if self.applyAlignment.get() and ts.hasAlignment():
             xfFile = os.path.join(tmpPrefix, firstItem.parseFileName(extension=".xf"))
             formatTransformFile(ts, xfFile)
 
-        binning = int(self.binning.get())
+        binning = self.binning.get()
 
         argsNewstack, paramsNewstack = self.getBasicNewstackParams(ts,
                                                                    os.path.join(extraPrefix, firstItem.parseFileName()),
                                                                    inputTsFileName=os.path.join(tmpPrefix, firstItem.parseFileName()),
                                                                    xfFile=xfFile,
                                                                    firstItem=firstItem,
                                                                    binning=binning,
@@ -260,15 +260,15 @@
         Plugin.runImod(self, 'newstack', argsNewstack % paramsNewstack)
 
         newTs = tomoObj.TiltSeries(tsId=tsId)
         newTs.copyInfo(ts)
         output.append(newTs)
 
         if binning > 1:
-            newTs.setSamplingRate(ts.getSamplingRate() * int(self.binning.get()))
+            newTs.setSamplingRate(ts.getSamplingRate() * binning)
 
         for index, tiltImage in enumerate(ts):
             newTi = tomoObj.TiltImage()
             newTi.copyInfo(tiltImage, copyId=True, copyTM=True)
 
             # Tranformation matrix
             if tiltImage.hasTransform() and not self.applyAlignment.get():
```

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_xCorrPrealignment.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_xCorrPrealignment.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/protocol_xRaysEraser.py` & `scipion-em-imod-3.1.9/imod/protocols/protocol_xRaysEraser.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols/script_imod_auto3d.py` & `scipion-em-imod-3.1.9/imod/protocols/script_imod_auto3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/protocols.conf` & `scipion-em-imod-3.1.9/imod/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/templates/automatic_tilt_series_alignment.json.template` & `scipion-em-imod-3.1.9/imod/templates/automatic_tilt_series_alignment.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/tests/__init__.py` & `scipion-em-imod-3.1.9/imod/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/tests/test_protocols_imod.py` & `scipion-em-imod-3.1.9/imod/tests/test_protocols_imod.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/utils.py` & `scipion-em-imod-3.1.9/imod/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1008,15 +1008,16 @@
     file path a dictionary where the key is the tsId and the
     value, the views to exclude"""
 
     excludedViews = {}
 
     logger.debug("Reading excluded views from %s" % excludeViewsFilePath)
     with open(excludeViewsFilePath, 'r') as f:
-        lines = f.read().splitlines()
+        lines = f.readlines()
+        lines = filter(lambda x: x.strip(), lines)
 
         for line in lines:
             vector = line.split()
             tsId = vector[0]
             views = vector[1]
             logger.info("For %s found excluded views: %s" % (tsId, views))
             excludedViews[tsId] = views
```

### Comparing `scipion-em-imod-3.1.8/imod/viewers/__init__.py` & `scipion-em-imod-3.1.9/imod/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/viewers/viewers.py` & `scipion-em-imod-3.1.9/imod/viewers/viewers.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/imod/viewers/views_tkinter_tree.py` & `scipion-em-imod-3.1.9/imod/viewers/views_tkinter_tree.py`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/scipion_em_imod.egg-info/PKG-INFO` & `scipion-em-imod-3.1.9/scipion_em_imod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-em-imod
-Version: 3.1.8
+Version: 3.1.9
 Summary: Plugin to use some of the Tomography tools from IMOD in Scipion
 Home-page: https://github.com/scipion-em/scipion-em-imod
 Author: J.M. De la Rosa, Federico P. de Isidro Gomez
 Author-email: delarosatrevin@scilifelab.se, fp.deisidro@cnb.csic.es
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-imod/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-imod/
```

### Comparing `scipion-em-imod-3.1.8/scipion_em_imod.egg-info/SOURCES.txt` & `scipion-em-imod-3.1.9/scipion_em_imod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-imod-3.1.8/setup.py` & `scipion-em-imod-3.1.9/setup.py`

 * *Files identical despite different names*

