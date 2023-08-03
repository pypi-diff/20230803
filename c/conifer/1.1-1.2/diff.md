# Comparing `tmp/conifer-1.1.tar.gz` & `tmp/conifer-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conifer-1.1.tar", last modified: Wed Jun  7 14:16:15 2023, max compression
+gzip compressed data, was "conifer-1.2.tar", last modified: Thu Aug  3 15:06:36 2023, max compression
```

## Comparing `conifer-1.1.tar` & `conifer-1.2.tar`

### file list

```diff
@@ -1,121 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.667023 conifer-1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.635023 conifer-1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.639023 conifer-1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-07 14:16:04.000000 conifer-1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 14:16:04.000000 conifer-1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-07 14:16:04.000000 conifer-1.1/Jenkinsfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 14:16:04.000000 conifer-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-07 14:16:04.000000 conifer-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-07 14:16:15.667023 conifer-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-07 14:16:04.000000 conifer-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.643023 conifer-1.1/conifer/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-07 14:16:04.000000 conifer-1.1/conifer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.643023 conifer-1.1/conifer/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.643023 conifer-1.1/conifer/backends/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/cpp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.643023 conifer-1.1/conifer/backends/cpp/include/
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/cpp/include/conifer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.643023 conifer-1.1/conifer/backends/cpp/template/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/cpp/template/bridge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/cpp/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.647023 conifer-1.1/conifer/backends/fpu/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.647023 conifer-1.1/conifer/backends/fpu/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/src/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/src/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/src/build_bit.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/src/build_hls.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/src/changes.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/src/fpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/src/fpu.h
--rw-r--r--   0 runner    (1001) docker     (123)    22375 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.647023 conifer-1.1/conifer/backends/vhdl/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.651023 conifer-1.1/conifer/backends/vhdl/firmware/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/AddReduce.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/BDT.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/BDTTestbench.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/BDTTop.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/Constants.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/SimulationInput.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/SimulationOutput.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/TestUtil.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/Tree.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/Types.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.651023 conifer-1.1/conifer/backends/vhdl/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/scripts/ghdl_compile.sh
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/scripts/modelsim_compile.sh
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/scripts/synth.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/scripts/xsim_compile.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/simulators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.655023 conifer-1.1/conifer/backends/xilinxhls/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.655023 conifer-1.1/conifer/backends/xilinxhls/firmware/
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/firmware/BDT_rolled.h
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/firmware/BDT_unrolled.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.655023 conifer-1.1/conifer/backends/xilinxhls/hls-template/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/hls-template/bridge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/hls-template/build_prj.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.655023 conifer-1.1/conifer/backends/xilinxhls/hls-template/firmware/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/hls-template/firmware/BDT_rolled.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/hls-template/firmware/BDT_unrolled.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/hls-template/firmware/myproject.h
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/hls-template/myproject_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22013 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.659023 conifer-1.1/conifer/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-07 14:16:04.000000 conifer-1.1/conifer/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-07 14:16:04.000000 conifer-1.1/conifer/converters/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-07 14:16:04.000000 conifer-1.1/conifer/converters/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-06-07 14:16:04.000000 conifer-1.1/conifer/converters/tf_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-07 14:16:04.000000 conifer-1.1/conifer/converters/tmva.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-07 14:16:04.000000 conifer-1.1/conifer/converters/xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-06-07 14:16:04.000000 conifer-1.1/conifer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.659023 conifer-1.1/conifer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 14:16:04.000000 conifer-1.1/conifer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-07 14:16:04.000000 conifer-1.1/conifer/utils/fixed_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-07 14:16:04.000000 conifer-1.1/conifer/utils/fixed_point_conversions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-07 14:16:04.000000 conifer-1.1/conifer/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.643023 conifer-1.1/conifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-07 14:16:15.000000 conifer-1.1/conifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 14:16:15.000000 conifer-1.1/conifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:16:15.000000 conifer-1.1/conifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 14:16:15.000000 conifer-1.1/conifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 14:16:15.000000 conifer-1.1/conifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    28385 2023-06-07 14:16:04.000000 conifer-1.1/conifer_v1.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.639023 conifer-1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.659023 conifer-1.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-07 14:16:04.000000 conifer-1.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-07 14:16:04.000000 conifer-1.1/docs/source/fpu.rst
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-07 14:16:04.000000 conifer-1.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.663023 conifer-1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-07 14:16:04.000000 conifer-1.1/examples/build_fpu_alveo.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-07 14:16:04.000000 conifer-1.1/examples/build_fpu_pynq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-07 14:16:04.000000 conifer-1.1/examples/pruned_xgboost_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-07 14:16:04.000000 conifer-1.1/examples/sklearn_RandomForest.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-07 14:16:04.000000 conifer-1.1/examples/sklearn_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-07 14:16:04.000000 conifer-1.1/examples/sklearn_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-07 14:16:04.000000 conifer-1.1/examples/sklearn_to_cpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-07 14:16:04.000000 conifer-1.1/examples/sklearn_to_fpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-07 14:16:04.000000 conifer-1.1/examples/sklearn_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-07 14:16:04.000000 conifer-1.1/examples/sklearn_to_vhdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-07 14:16:04.000000 conifer-1.1/examples/tf_df_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-07 14:16:04.000000 conifer-1.1/examples/tf_df_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-07 14:16:04.000000 conifer-1.1/examples/xgboost_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-07 14:16:04.000000 conifer-1.1/examples/xgboost_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 14:16:04.000000 conifer-1.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:16:15.667023 conifer-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-07 14:16:04.000000 conifer-1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.667023 conifer-1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 14:16:04.000000 conifer-1.1/tests/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-07 14:16:04.000000 conifer-1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-07 14:16:04.000000 conifer-1.1/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-07 14:16:04.000000 conifer-1.1/tests/test_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-07 14:16:04.000000 conifer-1.1/tests/test_onnx_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-07 14:16:04.000000 conifer-1.1/tests/test_save_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-07 14:16:04.000000 conifer-1.1/tests/test_skl_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-07 14:16:04.000000 conifer-1.1/tests/test_tf_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-07 14:16:04.000000 conifer-1.1/tests/util.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.473315 conifer-1.2/
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.461316 conifer-1.2/.github/
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/.github/workflows/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1091 2023-08-03 15:04:34.000000 conifer-1.2/.github/workflows/python-publish.yml
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)       43 2023-08-03 15:04:34.000000 conifer-1.2/.gitignore
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1064 2023-08-03 15:04:34.000000 conifer-1.2/Jenkinsfile
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)    11357 2023-08-03 15:04:34.000000 conifer-1.2/LICENSE
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)       37 2023-08-03 15:04:34.000000 conifer-1.2/MANIFEST.in
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     5789 2023-08-03 15:06:36.473315 conifer-1.2/PKG-INFO
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     5477 2023-08-03 15:04:34.000000 conifer-1.2/README.md
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/conifer/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      346 2023-08-03 15:04:34.000000 conifer-1.2/conifer/__init__.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/conifer/backends/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1091 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/__init__.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/conifer/backends/__pycache__/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     2116 2023-08-03 15:05:38.000000 conifer-1.2/conifer/backends/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)    11597 2023-08-03 15:05:38.000000 conifer-1.2/conifer/backends/__pycache__/common.cpython-311.pyc
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     6932 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/common.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/conifer/backends/cpp/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)       63 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/cpp/__init__.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/conifer/backends/cpp/__pycache__/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      281 2023-08-03 15:05:38.000000 conifer-1.2/conifer/backends/cpp/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     9594 2023-08-03 15:05:38.000000 conifer-1.2/conifer/backends/cpp/__pycache__/writer.cpython-311.pyc
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/conifer/backends/cpp/include/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     5105 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/cpp/include/conifer.h
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/conifer/backends/cpp/template/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      386 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/cpp/template/bridge.cpp
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     4933 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/cpp/writer.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/conifer/backends/fpu/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      375 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/fpu/__init__.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/conifer/backends/fpu/__pycache__/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      923 2023-08-03 15:05:38.000000 conifer-1.2/conifer/backends/fpu/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)    15773 2023-08-03 15:05:38.000000 conifer-1.2/conifer/backends/fpu/__pycache__/runtime.cpython-311.pyc
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)    43289 2023-08-03 15:05:38.000000 conifer-1.2/conifer/backends/fpu/__pycache__/writer.cpython-311.pyc
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     9085 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/fpu/runtime.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/conifer/backends/fpu/src/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     8851 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/fpu/src/LICENSE
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      647 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/fpu/src/README.md
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     2430 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/fpu/src/build_bit.tcl
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      998 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/fpu/src/build_hls.tcl
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      312 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/fpu/src/changes.txt
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     5248 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/fpu/src/fpu.cpp
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     2587 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/fpu/src/fpu.h
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)    22375 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/fpu/writer.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/conifer/backends/vhdl/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      420 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/__init__.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/conifer/backends/vhdl/__pycache__/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      845 2023-08-03 15:05:38.000000 conifer-1.2/conifer/backends/vhdl/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     7859 2023-08-03 15:05:38.000000 conifer-1.2/conifer/backends/vhdl/__pycache__/simulators.cpython-311.pyc
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)    20327 2023-08-03 15:05:38.000000 conifer-1.2/conifer/backends/vhdl/__pycache__/writer.cpython-311.pyc
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.469315 conifer-1.2/conifer/backends/vhdl/firmware/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     2004 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/firmware/AddReduce.vhd
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1935 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/firmware/BDT.vhd
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      711 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/firmware/BDTTestbench.vhd
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      627 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/firmware/BDTTop.vhd
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      493 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/firmware/Constants.vhd
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1404 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/firmware/SimulationInput.vhd
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     2193 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/firmware/SimulationOutput.vhd
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      810 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/firmware/TestUtil.vhd
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     3249 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/firmware/Tree.vhd
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     3490 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/firmware/Types.vhd
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.469315 conifer-1.2/conifer/backends/vhdl/scripts/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      576 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/scripts/ghdl_compile.sh
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      591 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/scripts/modelsim_compile.sh
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      289 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/scripts/synth.tcl
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      439 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/scripts/xsim_compile.sh
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     3578 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/simulators.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)    11150 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/vhdl/writer.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.469315 conifer-1.2/conifer/backends/xilinxhls/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      327 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/xilinxhls/__init__.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.469315 conifer-1.2/conifer/backends/xilinxhls/__pycache__/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      768 2023-08-03 15:05:38.000000 conifer-1.2/conifer/backends/xilinxhls/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)    32130 2023-08-03 15:05:38.000000 conifer-1.2/conifer/backends/xilinxhls/__pycache__/writer.cpython-311.pyc
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.469315 conifer-1.2/conifer/backends/xilinxhls/firmware/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     4663 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/xilinxhls/firmware/BDT_rolled.h
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     3850 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/xilinxhls/firmware/BDT_unrolled.h
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.469315 conifer-1.2/conifer/backends/xilinxhls/hls-template/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      962 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/xilinxhls/hls-template/bridge.cpp
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1184 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/xilinxhls/hls-template/build_prj.tcl
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.469315 conifer-1.2/conifer/backends/xilinxhls/hls-template/firmware/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      401 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/xilinxhls/hls-template/firmware/BDT_rolled.cpp
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      241 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/xilinxhls/hls-template/firmware/BDT_unrolled.cpp
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      208 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/xilinxhls/hls-template/firmware/myproject.h
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     3104 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/xilinxhls/hls-template/myproject_test.cpp
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)    22065 2023-08-03 15:04:34.000000 conifer-1.2/conifer/backends/xilinxhls/writer.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.469315 conifer-1.2/conifer/converters/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1664 2023-08-03 15:04:34.000000 conifer-1.2/conifer/converters/__init__.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     3783 2023-08-03 15:04:34.000000 conifer-1.2/conifer/converters/onnx.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1994 2023-08-03 15:04:34.000000 conifer-1.2/conifer/converters/sklearn.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     6761 2023-08-03 15:04:34.000000 conifer-1.2/conifer/converters/tf_df.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     3039 2023-08-03 15:04:34.000000 conifer-1.2/conifer/converters/tmva.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     2812 2023-08-03 15:04:34.000000 conifer-1.2/conifer/converters/xgboost.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)    12308 2023-08-03 15:04:34.000000 conifer-1.2/conifer/model.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.469315 conifer-1.2/conifer/utils/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      145 2023-08-03 15:04:34.000000 conifer-1.2/conifer/utils/__init__.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     2958 2023-08-03 15:04:34.000000 conifer-1.2/conifer/utils/fixed_point.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      644 2023-08-03 15:04:34.000000 conifer-1.2/conifer/utils/fixed_point_conversions.cpp
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1752 2023-08-03 15:04:34.000000 conifer-1.2/conifer/utils/misc.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/conifer.egg-info/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     5789 2023-08-03 15:06:36.000000 conifer-1.2/conifer.egg-info/PKG-INFO
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     3793 2023-08-03 15:06:36.000000 conifer-1.2/conifer.egg-info/SOURCES.txt
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)        1 2023-08-03 15:06:36.000000 conifer-1.2/conifer.egg-info/dependency_links.txt
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)       25 2023-08-03 15:06:36.000000 conifer-1.2/conifer.egg-info/requires.txt
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)        8 2023-08-03 15:06:36.000000 conifer-1.2/conifer.egg-info/top_level.txt
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)    28385 2023-08-03 15:04:34.000000 conifer-1.2/conifer_v1.png
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.465316 conifer-1.2/docs/
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.469315 conifer-1.2/docs/source/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1314 2023-08-03 15:04:34.000000 conifer-1.2/docs/source/conf.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     4554 2023-08-03 15:04:34.000000 conifer-1.2/docs/source/fpu.rst
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      470 2023-08-03 15:04:34.000000 conifer-1.2/docs/source/index.rst
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.473315 conifer-1.2/examples/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      844 2023-08-03 15:04:34.000000 conifer-1.2/examples/build_fpu_alveo.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      776 2023-08-03 15:04:34.000000 conifer-1.2/examples/build_fpu_pynq.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1486 2023-08-03 15:04:34.000000 conifer-1.2/examples/pruned_xgboost_to_hls.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      940 2023-08-03 15:04:34.000000 conifer-1.2/examples/sklearn_RandomForest.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      740 2023-08-03 15:04:34.000000 conifer-1.2/examples/sklearn_multiclass.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1234 2023-08-03 15:04:34.000000 conifer-1.2/examples/sklearn_regression.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1769 2023-08-03 15:04:34.000000 conifer-1.2/examples/sklearn_to_cpp.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1746 2023-08-03 15:04:34.000000 conifer-1.2/examples/sklearn_to_fpu.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1086 2023-08-03 15:04:34.000000 conifer-1.2/examples/sklearn_to_hls.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1052 2023-08-03 15:04:34.000000 conifer-1.2/examples/sklearn_to_vhdl.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1788 2023-08-03 15:04:34.000000 conifer-1.2/examples/tf_df_binary.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1760 2023-08-03 15:04:34.000000 conifer-1.2/examples/tf_df_multiclass.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1356 2023-08-03 15:04:34.000000 conifer-1.2/examples/xgboost_multiclass.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1467 2023-08-03 15:04:34.000000 conifer-1.2/examples/xgboost_to_hls.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      118 2023-08-03 15:04:34.000000 conifer-1.2/pytest.ini
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)       38 2023-08-03 15:06:36.473315 conifer-1.2/setup.cfg
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      720 2023-08-03 15:04:34.000000 conifer-1.2/setup.py
+drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2023-08-03 15:06:36.473315 conifer-1.2/tests/
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)       24 2023-08-03 15:04:34.000000 conifer-1.2/tests/cleanup.sh
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)       76 2023-08-03 15:04:34.000000 conifer-1.2/tests/conftest.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     2789 2023-08-03 15:04:34.000000 conifer-1.2/tests/test_backends.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     2027 2023-08-03 15:04:34.000000 conifer-1.2/tests/test_multiclass.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     2919 2023-08-03 15:04:34.000000 conifer-1.2/tests/test_onnx_to_hls.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     1677 2023-08-03 15:04:34.000000 conifer-1.2/tests/test_save_load.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)      511 2023-08-03 15:04:34.000000 conifer-1.2/tests/test_skl_to_hls.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     5242 2023-08-03 15:04:34.000000 conifer-1.2/tests/test_tf_df.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     3364 2023-08-03 15:04:34.000000 conifer-1.2/tests/test_xgb_converter.py
+-rw-rw-r--   0 sioni     (1000) sioni     (1000)     2621 2023-08-03 15:04:34.000000 conifer-1.2/tests/util.py
```

### Comparing `conifer-1.1/.github/workflows/python-publish.yml` & `conifer-1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `conifer-1.1/Jenkinsfile` & `conifer-1.2/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `conifer-1.1/LICENSE` & `conifer-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conifer-1.1/PKG-INFO` & `conifer-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conifer
-Version: 1.1
+Version: 1.2
 Summary: BDT Inference for FPGAs
 Home-page: https://github.com/thesps/conifer
 Author: Sioni Summers
 Author-email: sioni@cern.ch
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `conifer-1.1/README.md` & `conifer-1.2/README.md`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/__init__.py` & `conifer-1.2/conifer/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/common.py` & `conifer-1.2/conifer/backends/common.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/cpp/include/conifer.h` & `conifer-1.2/conifer/backends/cpp/include/conifer.h`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/cpp/writer.py` & `conifer-1.2/conifer/backends/cpp/writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import numpy as np
 from shutil import copyfile
 import copy
-from conifer.utils import _ap_include, _json_include, copydocstring
+from conifer.utils import _ap_include, _json_include, _gcc_opts, _py_executable, copydocstring
 from conifer.model import ModelBase
 from conifer.backends.common import MultiPrecisionConfig
 import logging
 logger = logging.getLogger(__name__)
 
 class CPPConfig(MultiPrecisionConfig):
   backend = 'cpp'
@@ -15,16 +15,14 @@
     super(CPPConfig, self).__init__(configDict, validate=True)
     self._extra_validate()
 
   def _extra_validate(self):
     # TODO: proagate different precisions properly through backend
     # for now enforce that all the precisions are equal
     assert self.input_precision == self.threshold_precision, f'input & threshold precision must be equal, got: {self.input_precision} & {self.threshold_precision}'
-    assert self.threshold_precision == self.score_precision, f'threshold & score precision must be equal, got: {self.threshold_precision} & {self.score_precision}'
-
 
 class CPPModel(ModelBase):
   def __init__(self, ensembleDict, config, metadata=None):
     super(CPPModel, self).__init__(ensembleDict, config, metadata)
     self.config = CPPConfig(config)
 
   @copydocstring(ModelBase.write)
@@ -53,15 +51,15 @@
     fout = open(f"{cfg.output_dir}/bridge.cpp", 'w')
     for line in fin.readlines():
       newline = line
       if '// conifer insert typedef' in line:
         newline =  f"typedef {cfg.threshold_precision} T;\n"
         newline += f"typedef {cfg.score_precision} U;\n"
       elif 'PYBIND11_MODULE' in line:
-        newline = f'PYBIND11_MODULE(conifer_bridge_{self._stamp}, m){{\n'
+        newline = line.replace('conifer_bridge', f'conifer_bridge_{self._stamp}')
       elif '// conifer insert include' in line:
         newline = '#include "ap_fixed.h"' if cfg.any_ap_types() else ''
       fout.write(newline)
     fin.close()
     fout.close()
     os.remove(f"{cfg.output_dir}/bridge_tmp.cpp")
 
@@ -85,15 +83,15 @@
       os.chdir(curr_dir)
       raise Exception("Couldn't find the JSON headers. Install nlohmman JSON, and set JSON_ROOT")
     # find the conifer.h header
     filedir = os.path.dirname(os.path.abspath(__file__))
     conifer_include = f'-I{filedir}/include/'
 
     # Do the compile
-    cmd = f"g++ -O3 -shared -std=c++14 -fPIC $(python3 -m pybind11 --includes) {ap_include} {json_include} {conifer_include} bridge.cpp -o conifer_bridge_{self._stamp}.so"
+    cmd = f"g++ -O3 -shared -std=c++14 -fPIC $({_py_executable()} -m pybind11 --includes) {ap_include} {json_include} {conifer_include} {_gcc_opts()} bridge.cpp -o conifer_bridge_{self._stamp}.so"
     logger.debug(f'Compiling with command {cmd}')
     try:
       ret_val = os.system(cmd)
       if ret_val != 0:
         raise Exception(f'Failed to compile project {cfg.project_name}')
     except:
       os.chdir(curr_dir)
```

### Comparing `conifer-1.1/conifer/backends/fpu/runtime.py` & `conifer-1.2/conifer/backends/fpu/runtime.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/fpu/src/LICENSE` & `conifer-1.2/conifer/backends/fpu/src/LICENSE`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/fpu/src/README.md` & `conifer-1.2/conifer/backends/fpu/src/README.md`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/fpu/src/build_bit.tcl` & `conifer-1.2/conifer/backends/fpu/src/build_bit.tcl`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/fpu/src/build_hls.tcl` & `conifer-1.2/conifer/backends/fpu/src/build_hls.tcl`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/fpu/src/fpu.cpp` & `conifer-1.2/conifer/backends/fpu/src/fpu.cpp`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/fpu/src/fpu.h` & `conifer-1.2/conifer/backends/fpu/src/fpu.h`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/fpu/writer.py` & `conifer-1.2/conifer/backends/fpu/writer.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/vhdl/firmware/AddReduce.vhd` & `conifer-1.2/conifer/backends/vhdl/firmware/AddReduce.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/vhdl/firmware/BDT.vhd` & `conifer-1.2/conifer/backends/vhdl/firmware/BDT.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/vhdl/firmware/BDTTestbench.vhd` & `conifer-1.2/conifer/backends/vhdl/firmware/BDTTestbench.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/vhdl/firmware/BDTTop.vhd` & `conifer-1.2/conifer/backends/vhdl/firmware/BDTTop.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/vhdl/firmware/SimulationInput.vhd` & `conifer-1.2/conifer/backends/vhdl/firmware/SimulationInput.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/vhdl/firmware/SimulationOutput.vhd` & `conifer-1.2/conifer/backends/vhdl/firmware/SimulationOutput.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/vhdl/firmware/TestUtil.vhd` & `conifer-1.2/conifer/backends/vhdl/firmware/TestUtil.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/vhdl/firmware/Tree.vhd` & `conifer-1.2/conifer/backends/vhdl/firmware/Tree.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/vhdl/firmware/Types.vhd` & `conifer-1.2/conifer/backends/vhdl/firmware/Types.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/vhdl/scripts/ghdl_compile.sh` & `conifer-1.2/conifer/backends/vhdl/scripts/ghdl_compile.sh`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/vhdl/scripts/modelsim_compile.sh` & `conifer-1.2/conifer/backends/vhdl/scripts/modelsim_compile.sh`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/vhdl/simulators.py` & `conifer-1.2/conifer/backends/vhdl/simulators.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/vhdl/writer.py` & `conifer-1.2/conifer/backends/vhdl/writer.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/xilinxhls/firmware/BDT_rolled.h` & `conifer-1.2/conifer/backends/xilinxhls/firmware/BDT_rolled.h`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/xilinxhls/firmware/BDT_unrolled.h` & `conifer-1.2/conifer/backends/xilinxhls/firmware/BDT_unrolled.h`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/xilinxhls/hls-template/bridge.cpp` & `conifer-1.2/conifer/backends/xilinxhls/hls-template/bridge.cpp`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/xilinxhls/hls-template/build_prj.tcl` & `conifer-1.2/conifer/backends/xilinxhls/hls-template/build_prj.tcl`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/xilinxhls/hls-template/myproject_test.cpp` & `conifer-1.2/conifer/backends/xilinxhls/hls-template/myproject_test.cpp`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/backends/xilinxhls/writer.py` & `conifer-1.2/conifer/backends/xilinxhls/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from shutil import copyfile
 import warnings
 import numpy as np
 import copy
-from conifer.utils import _ap_include, copydocstring
+from conifer.utils import _ap_include, _gcc_opts, _py_executable, copydocstring
 from conifer.backends.common import BottomUpDecisionTree, MultiPrecisionConfig, read_hls_report
 from conifer.model import ModelBase
 import datetime
 import logging
 logger = logging.getLogger(__name__)
 
 _TOOLS = {
@@ -448,15 +448,15 @@
         cfg = self.config
         curr_dir = os.getcwd()
         os.chdir(cfg.output_dir)
         ap_include = _ap_include()
         if ap_include is None:
             os.chdir(curr_dir)
             raise Exception("Couldn't find Xilinx ap_ headers. Source the Vivado/Vitis HLS toolchain, or set XILINX_AP_INCLUDE environment variable.")
-        cmd = f"g++ -O3 -shared -std=c++14 -fPIC $(python3 -m pybind11 --includes) {ap_include} bridge.cpp firmware/BDT.cpp firmware/{cfg.project_name}.cpp -o conifer_bridge_{self._stamp}.so"
+        cmd = f"g++ -O3 -shared -std=c++14 -fPIC $({_py_executable()} -m pybind11 --includes) {ap_include} {_gcc_opts()} bridge.cpp firmware/BDT.cpp firmware/{cfg.project_name}.cpp -o conifer_bridge_{self._stamp}.so"
         logger.debug(f'Compiling with command {cmd}')
         try:
             ret_val = os.system(cmd)
             if ret_val != 0:
                 raise Exception(f'Failed to compile project {cfg.project_name}')
         except:
             os.chdir(curr_dir)
```

### Comparing `conifer-1.1/conifer/converters/__init__.py` & `conifer-1.2/conifer/converters/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-from conifer.converters import sklearn
-from conifer.converters import tmva
-from conifer.converters import xgboost
-from conifer.converters import onnx
-from conifer.model import make_model
-
-try:
-    from conifer.converters import tf_df
-except ImportError:
-    tf_df = None
-    print("Warning: The python package tensorflow_decision_forests is not available. Conversions "
-          "from TensorFlow Decision Forests models is not possible.")
-
 import logging
 logger = logging.getLogger(__name__)
 
-_converter_map = {'sklearn' : sklearn,
-                  'tmva'    : tmva,
-                  'xgboost' : xgboost,
-                  'onnx'    : onnx,
-                  'tf_df':  tf_df}
+_converter_map = {}
+import importlib
+for module in ['sklearn', 'tmva', 'xgboost', 'onnx', 'tf_df']:
+  try:
+    the_module = importlib.import_module(f'conifer.converters.{module}')
+    _converter_map[module] = the_module
+  except ImportError:
+    logger.warn(f'Could not import conifer {module} converter')
+
+from conifer.model import make_model
 
 def get_converter(converter):
   '''Get converter object from string'''
   converter_obj = _converter_map.get(converter)
   if converter_obj is None:
     raise RuntimeError(f'No converter "{converter}" found. Options are {[k for k in _converter_map.keys()]}')
   return converter_obj
```

### Comparing `conifer-1.1/conifer/converters/onnx.py` & `conifer-1.2/conifer/converters/onnx.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/converters/sklearn.py` & `conifer-1.2/conifer/converters/sklearn.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/converters/tf_df.py` & `conifer-1.2/conifer/converters/tf_df.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/converters/tmva.py` & `conifer-1.2/conifer/converters/tmva.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/model.py` & `conifer-1.2/conifer/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,17 +3,34 @@
 import numpy as np
 import os
 import json
 import copy
 import datetime
 import platform
 import getpass
+from typing import Union
+try:
+    import pydot
+except ImportError:
+    pydot = None
 import logging
 logger = logging.getLogger(__name__)
 
+def _check_pydot():
+    '''Returns True if PyDot and Graphviz are available, otherwise returns False'''
+    if pydot is None:
+        return False
+    try:
+        # Attempt to create an image of a blank graph
+        # to check the pydot/graphviz installation.
+        pydot.Dot.create(pydot.Dot())
+        return True
+    except OSError:
+        return False
+    
 class DecisionTreeBase:
   '''
   Conifer DecisionTreeBase representation class
   '''
   _tree_fields = ['feature', 'threshold', 'value', 'children_left', 'children_right']
   def __init__(self, treeDict):
     for key in DecisionTreeBase._tree_fields:
@@ -22,14 +39,60 @@
       setattr(self, key, val)
 
   def n_nodes(self):
     return len(self.feature)
 
   def n_leaves(self):
     return len([n for n in self.feature if n == -2])
+  
+  def draw(self, filename : str = None, graph=None, tree_id=None):
+    '''
+    Draw a pydot graph of the decision tree
+
+    Parameters
+    ----------
+    filename: string
+        filename to save to, with any extension supported by pydot write
+
+    graph:
+        existing pydot graph to add to
+
+    tree_id:
+        ID of the tree within an ensemble
+
+    Returns
+    ----------
+    pydot Dot graph object
+    '''
+    if not _check_pydot():
+        raise ImportError('Could not import pydot. Install Graphviz and pydot to draw trees')
+    graph = pydot.Dot(graph_type='graph') if graph is None else graph
+    tree_id = '' if tree_id is None else tree_id
+    sg = pydot.Cluster(tree_id, label=tree_id, peripheries=0 if tree_id=='' else 1)
+    graph.add_subgraph(sg)
+    for i in range(self.n_nodes()):
+      node_id = f'{tree_id}_{i}'
+      l = f'{tree_id}_{self.children_left[i]}'
+      r = f'{tree_id}_{self.children_right[i]}'
+      label = f'x[{self.feature[i]}] <= {self.threshold[i]:.2f}' if self.feature[i] != -2 else f'{self.value[i]:.2f}'
+      sg.add_node(pydot.Node(node_id, label=label))
+      if self.children_left[i] != -1:
+        sg.add_edge(pydot.Edge(node_id, l,))
+      if self.children_right[i] != -1:
+        sg.add_edge(pydot.Edge(node_id, r,))
+    if filename is not None:
+        _, extension = os.path.splitext(filename)
+        if not extension:
+            extension = 'png'
+        else:
+            extension = extension[1:]
+        graph.write(filename, format=extension)
+
+    return graph
+
 
 class ConfigBase:
     '''
     Conifer Config representation class
     '''
     _config_fields = ['output_dir', 'project_name', 'backend']
     _alternates = {'output_dir'   : ['OutputDir'],
@@ -149,14 +212,43 @@
     def compile(self):
         '''
         Compile conifer model ahead of running decision_function.
         Writes the project files first.
         Compilation is carried out by the model backend
         '''
         raise NotImplementedError
+    
+    def draw(self, filename=None):
+        '''
+        Draw a pydot graph of the decision tree
+
+        Parameters
+        ----------
+        filename: string
+            filename to save to, with any extension supported by pydot write
+
+        Returns
+        ----------
+        pydot Dot graph object
+        '''
+        if not _check_pydot():
+            raise ImportError('Could not import pydot. Install Graphviz and pydot to draw trees')
+        graph = pydot.Dot(graph_type='graph')
+        for i, treesi in enumerate(self.trees):
+            for j, tree in enumerate(treesi):
+                tree_id = f'Tree {i}, Class {j}'
+                tree.draw(filename=None, graph=graph, tree_id=tree_id)
+        if filename is not None:
+            _, extension = os.path.splitext(filename)
+            if not extension:
+                extension = 'png'
+            else:
+                extension = extension[1:]
+            graph.write(filename, format=extension)
+        return graph
 
     def decision_function(self, X, trees=False):
         '''
         Compute the decision function of `X`.
         The backend performs the actual computation
         
         Parameters
```

### Comparing `conifer-1.1/conifer/utils/fixed_point.py` & `conifer-1.2/conifer/utils/fixed_point.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/utils/fixed_point_conversions.cpp` & `conifer-1.2/conifer/utils/fixed_point_conversions.cpp`

 * *Files identical despite different names*

### Comparing `conifer-1.1/conifer/utils/misc.py` & `conifer-1.2/conifer/utils/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 import logging
 logger = logging.getLogger(__name__)
 
 def _ap_include():
   '''
   Get the -I include option for the g++ compile for the ap_ headers.
   If set use XILINX_AP_INCLUDE, then check for Vivado/Vitis HLS
@@ -28,14 +29,29 @@
     ret = f'-I{os.environ.get("JSON_ROOT")}'
     logger.debug(f'Include JSON headers from JSON_ROOT: {ret}')
   else:
     ret = None
     logger.warn('Could not find JSON headers. JSON_ROOT not defined')
   return ret
 
+def _gcc_opts():
+  '''
+  Get extra platform specific g++ compile options
+  '''
+  if sys.platform == 'darwin':
+     return '-undefined dynamic_lookup'
+  else:
+     return ''
+  
+def _py_executable():
+  '''
+  Get the python executable 
+  '''
+  return sys.executable
+
 def copydocstring(fromfunc, sep="\n"):
   """
   Decorator: Copy the docstring of `fromfunc`
   """
   def _decorator(func):
       sourcedoc = fromfunc.__doc__
       if func.__doc__ == None:
```

### Comparing `conifer-1.1/conifer.egg-info/PKG-INFO` & `conifer-1.2/conifer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conifer
-Version: 1.1
+Version: 1.2
 Summary: BDT Inference for FPGAs
 Home-page: https://github.com/thesps/conifer
 Author: Sioni Summers
 Author-email: sioni@cern.ch
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `conifer-1.1/conifer.egg-info/SOURCES.txt` & `conifer-1.2/conifer.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -12,31 +12,41 @@
 conifer.egg-info/PKG-INFO
 conifer.egg-info/SOURCES.txt
 conifer.egg-info/dependency_links.txt
 conifer.egg-info/requires.txt
 conifer.egg-info/top_level.txt
 conifer/backends/__init__.py
 conifer/backends/common.py
+conifer/backends/__pycache__/__init__.cpython-311.pyc
+conifer/backends/__pycache__/common.cpython-311.pyc
 conifer/backends/cpp/__init__.py
 conifer/backends/cpp/writer.py
+conifer/backends/cpp/__pycache__/__init__.cpython-311.pyc
+conifer/backends/cpp/__pycache__/writer.cpython-311.pyc
 conifer/backends/cpp/include/conifer.h
 conifer/backends/cpp/template/bridge.cpp
 conifer/backends/fpu/__init__.py
 conifer/backends/fpu/runtime.py
 conifer/backends/fpu/writer.py
+conifer/backends/fpu/__pycache__/__init__.cpython-311.pyc
+conifer/backends/fpu/__pycache__/runtime.cpython-311.pyc
+conifer/backends/fpu/__pycache__/writer.cpython-311.pyc
 conifer/backends/fpu/src/LICENSE
 conifer/backends/fpu/src/README.md
 conifer/backends/fpu/src/build_bit.tcl
 conifer/backends/fpu/src/build_hls.tcl
 conifer/backends/fpu/src/changes.txt
 conifer/backends/fpu/src/fpu.cpp
 conifer/backends/fpu/src/fpu.h
 conifer/backends/vhdl/__init__.py
 conifer/backends/vhdl/simulators.py
 conifer/backends/vhdl/writer.py
+conifer/backends/vhdl/__pycache__/__init__.cpython-311.pyc
+conifer/backends/vhdl/__pycache__/simulators.cpython-311.pyc
+conifer/backends/vhdl/__pycache__/writer.cpython-311.pyc
 conifer/backends/vhdl/firmware/AddReduce.vhd
 conifer/backends/vhdl/firmware/BDT.vhd
 conifer/backends/vhdl/firmware/BDTTestbench.vhd
 conifer/backends/vhdl/firmware/BDTTop.vhd
 conifer/backends/vhdl/firmware/Constants.vhd
 conifer/backends/vhdl/firmware/SimulationInput.vhd
 conifer/backends/vhdl/firmware/SimulationOutput.vhd
@@ -45,14 +55,16 @@
 conifer/backends/vhdl/firmware/Types.vhd
 conifer/backends/vhdl/scripts/ghdl_compile.sh
 conifer/backends/vhdl/scripts/modelsim_compile.sh
 conifer/backends/vhdl/scripts/synth.tcl
 conifer/backends/vhdl/scripts/xsim_compile.sh
 conifer/backends/xilinxhls/__init__.py
 conifer/backends/xilinxhls/writer.py
+conifer/backends/xilinxhls/__pycache__/__init__.cpython-311.pyc
+conifer/backends/xilinxhls/__pycache__/writer.cpython-311.pyc
 conifer/backends/xilinxhls/firmware/BDT_rolled.h
 conifer/backends/xilinxhls/firmware/BDT_unrolled.h
 conifer/backends/xilinxhls/hls-template/bridge.cpp
 conifer/backends/xilinxhls/hls-template/build_prj.tcl
 conifer/backends/xilinxhls/hls-template/myproject_test.cpp
 conifer/backends/xilinxhls/hls-template/firmware/BDT_rolled.cpp
 conifer/backends/xilinxhls/hls-template/firmware/BDT_unrolled.cpp
@@ -88,8 +100,9 @@
 tests/conftest.py
 tests/test_backends.py
 tests/test_multiclass.py
 tests/test_onnx_to_hls.py
 tests/test_save_load.py
 tests/test_skl_to_hls.py
 tests/test_tf_df.py
+tests/test_xgb_converter.py
 tests/util.py
```

### Comparing `conifer-1.1/conifer_v1.png` & `conifer-1.2/conifer_v1.png`

 * *Files identical despite different names*

### Comparing `conifer-1.1/docs/source/conf.py` & `conifer-1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/docs/source/fpu.rst` & `conifer-1.2/docs/source/fpu.rst`

 * *Files identical despite different names*

### Comparing `conifer-1.1/examples/build_fpu_alveo.py` & `conifer-1.2/examples/build_fpu_alveo.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/examples/build_fpu_pynq.py` & `conifer-1.2/examples/build_fpu_pynq.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/examples/pruned_xgboost_to_hls.py` & `conifer-1.2/examples/pruned_xgboost_to_hls.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/examples/sklearn_RandomForest.py` & `conifer-1.2/examples/sklearn_RandomForest.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/examples/sklearn_multiclass.py` & `conifer-1.2/examples/sklearn_multiclass.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/examples/sklearn_regression.py` & `conifer-1.2/examples/sklearn_regression.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/examples/sklearn_to_cpp.py` & `conifer-1.2/examples/sklearn_to_cpp.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/examples/sklearn_to_fpu.py` & `conifer-1.2/examples/sklearn_to_fpu.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/examples/sklearn_to_hls.py` & `conifer-1.2/examples/sklearn_to_hls.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/examples/sklearn_to_vhdl.py` & `conifer-1.2/examples/sklearn_to_vhdl.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/examples/tf_df_binary.py` & `conifer-1.2/examples/tf_df_binary.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/examples/tf_df_multiclass.py` & `conifer-1.2/examples/tf_df_multiclass.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/examples/xgboost_multiclass.py` & `conifer-1.2/examples/xgboost_multiclass.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/examples/xgboost_to_hls.py` & `conifer-1.2/examples/xgboost_to_hls.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/setup.py` & `conifer-1.2/setup.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/tests/test_backends.py` & `conifer-1.2/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/tests/test_multiclass.py` & `conifer-1.2/tests/test_multiclass.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/tests/test_onnx_to_hls.py` & `conifer-1.2/tests/test_onnx_to_hls.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/tests/test_save_load.py` & `conifer-1.2/tests/test_save_load.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/tests/test_tf_df.py` & `conifer-1.2/tests/test_tf_df.py`

 * *Files identical despite different names*

### Comparing `conifer-1.1/tests/util.py` & `conifer-1.2/tests/util.py`

 * *Files identical despite different names*

