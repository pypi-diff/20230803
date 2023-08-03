# Comparing `tmp/pyPhasesML-0.7.8.tar.gz` & `tmp/pyPhasesML-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.7.8.tar", last modified: Wed Aug  2 07:24:32 2023, max compression
+gzip compressed data, was "pyPhasesML-0.7.9.tar", last modified: Thu Aug  3 09:02:43 2023, max compression
```

## Comparing `pyPhasesML-0.7.8.tar` & `pyPhasesML-0.7.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.526917 pyPhasesML-0.7.8/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3690 2023-08-02 07:24:32.526917 pyPhasesML-0.7.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3183 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.520917 pyPhasesML-0.7.8/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/DataversionManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     4074 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/ModelAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     4952 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4566 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.522917 pyPhasesML-0.7.8/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10255 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7159 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)     9901 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.523917 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/
--rw-rw-rw-   0 root         (0) root         (0)      734 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/CSVLogger.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/Callback.py
--rw-rw-rw-   0 root         (0) root         (0)     3710 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/CheckPoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/CyclicLearningrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/FindLearningRate.py
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/LoadOptimizer.py
--rw-rw-rw-   0 root         (0) root         (0)     2430 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/SystemCheckPoint.py
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.524917 pyPhasesML-0.7.8/pyPhasesML/datapipes/
--rw-rw-rw-   0 root         (0) root         (0)      464 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/datapipes/Augmentor.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/datapipes/DatasetXY.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/datapipes/FoldMapper.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/datapipes/RecordMap.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/datapipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.525917 pyPhasesML-0.7.8/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5385 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.526917 pyPhasesML-0.7.8/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    19017 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.521917 pyPhasesML-0.7.8/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3690 2023-08-02 07:24:32.000000 pyPhasesML-0.7.8/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1398 2023-08-02 07:24:32.000000 pyPhasesML-0.7.8/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 07:24:32.000000 pyPhasesML-0.7.8/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-08-02 07:24:32.000000 pyPhasesML-0.7.8/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-08-02 07:24:32.000000 pyPhasesML-0.7.8/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 07:24:32.526917 pyPhasesML-0.7.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-08-02 07:24:16.000000 pyPhasesML-0.7.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:02:43.095086 pyPhasesML-0.7.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3690 2023-08-03 09:02:43.095086 pyPhasesML-0.7.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3183 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:02:43.090086 pyPhasesML-0.7.9/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/DataversionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4074 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/ModelAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4952 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4566 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:02:43.091086 pyPhasesML-0.7.9/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10245 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7159 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9917 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/adapter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:02:43.093086 pyPhasesML-0.7.9/pyPhasesML/adapter/torch/
+-rw-rw-rw-   0 root         (0) root         (0)      734 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/adapter/torch/CSVLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/adapter/torch/Callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     3710 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/adapter/torch/CheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/adapter/torch/CyclicLearningrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/adapter/torch/FindLearningRate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/adapter/torch/LoadOptimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2430 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/adapter/torch/SystemCheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/adapter/torch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:02:43.093086 pyPhasesML-0.7.9/pyPhasesML/datapipes/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/datapipes/Augmentor.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/datapipes/DatasetXY.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/datapipes/FoldMapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/datapipes/RecordMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/datapipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:02:43.094086 pyPhasesML-0.7.9/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5385 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:02:43.094086 pyPhasesML-0.7.9/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    19017 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:02:43.091086 pyPhasesML-0.7.9/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3690 2023-08-03 09:02:43.000000 pyPhasesML-0.7.9/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-08-03 09:02:43.000000 pyPhasesML-0.7.9/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 09:02:43.000000 pyPhasesML-0.7.9/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-08-03 09:02:43.000000 pyPhasesML-0.7.9/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-08-03 09:02:43.000000 pyPhasesML-0.7.9/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-08-03 09:02:24.000000 pyPhasesML-0.7.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 09:02:43.095086 pyPhasesML-0.7.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-08-03 09:02:25.000000 pyPhasesML-0.7.9/setup.py
```

### Comparing `pyPhasesML-0.7.8/LICENSE` & `pyPhasesML-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/PKG-INFO` & `pyPhasesML-0.7.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.7.8
+Version: 0.7.9
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.7.8/README.md` & `pyPhasesML-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.7.9/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/DataSet.py` & `pyPhasesML-0.7.9/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/DataversionManager.py` & `pyPhasesML-0.7.9/pyPhasesML/DataversionManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.7.9/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/Model.py` & `pyPhasesML-0.7.9/pyPhasesML/Model.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/ModelManager.py` & `pyPhasesML-0.7.9/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/Plugin.py` & `pyPhasesML-0.7.9/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.7.9/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.7.9/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from pyPhasesML import ModelAdapter
+from ..ModelAdapter import ModelAdapter
 from ..scorer.ScorerTF import ScorerTF
 
 import shutil
 import tensorflow as tf
 import tensorflow.keras as K
 import matplotlib.pyplot as plt
 import numpy as np
 import io
 
-from ..DataSet import TrainingSet
-from ..Model import Model
+from ..DataSet import TrainingSetLoader
 
 
 def plot_to_image(figure):
     """Converts the matplotlib plot specified by 'figure' to a PNG image and
     returns it. The supplied figure is closed and inaccessible after this call."""
     # Save the plot to a PNG in memory.
     buf = io.BytesIO()
@@ -55,15 +54,15 @@
         if hasattr(self, "freeze"):
             layers_freeze = self.freeze
             # len(self.model.layers)
             for layer in self.model.layers[:layers_freeze]:
                 layer.trainable = False
         return
 
-    def train(self, dataset: TrainingSet):
+    def train(self, dataset: TrainingSetLoader):
         callbacks = []
         mainMetric = self._metrics(self.metrics[self.validationMetrics[0]])
         metricStop = self.getMetric(mainMetric)
         metricSave = self.getMetric(mainMetric)
 
         tbLogDir = self.logPath + "/tb"
         shutil.rmtree(tbLogDir, ignore_errors=True)
```

### Comparing `pyPhasesML-0.7.8/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.7.9/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.7.9/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,18 +196,18 @@
                     self.model(batchFeats)
                     lossCriterion(output, targs)
                     raise Exception("batch loss should be a number")
 
                 if self.batchScheduler is not None:
                     self.batchScheduler.step()
 
-                self.trigger("batchEnd", self, batchIndex)
-
                 self.runningStats["loss"] += currentBatchLoss
                 self.runningStats["lr"] = self.optimizer.param_groups[0]["lr"]
+                
+                self.trigger("batchEnd", self, batchIndex)
 
                 del output
                 del targs
                 del loss
                 gc.collect()
                 currentCount = processList.n + 1
                 processList.set_postfix(ordered_dict={n: v / currentCount for n, v in self.runningStats.items()})
```

### Comparing `pyPhasesML-0.7.8/pyPhasesML/adapter/torch/CSVLogger.py` & `pyPhasesML-0.7.9/pyPhasesML/adapter/torch/CSVLogger.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/adapter/torch/Callback.py` & `pyPhasesML-0.7.9/pyPhasesML/adapter/torch/Callback.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/adapter/torch/CheckPoint.py` & `pyPhasesML-0.7.9/pyPhasesML/adapter/torch/CheckPoint.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/adapter/torch/CyclicLearningrate.py` & `pyPhasesML-0.7.9/pyPhasesML/adapter/torch/CyclicLearningrate.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/adapter/torch/FindLearningRate.py` & `pyPhasesML-0.7.9/pyPhasesML/adapter/torch/FindLearningRate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 import math
-import numpy as np
 
 from pyPhases import classLogger
 from pyPhasesML.Model import ModelConfig
 from pyPhasesML.adapter.torch.Callback import Callback
 from pyPhases import CSVLogger as Logger
 
 
 @classLogger
 class FindLearningRate(Callback):
     def __init__(self, config: ModelConfig, minLR, maxLR, iterations=3) -> None:
         super().__init__(config)
         self.smoothing = 0.05
-        self.csvPath = self.getLogPath() + "/rangetest.png"
+        self.csvPath = self.getLogPath() + "/rangetest.csv"
         self.minLR = minLR
         self.maxLR = maxLR
         self.iterations = iterations
         self.logger = Logger(self.csvPath)
 
     def onTrainingStart(self, model, dataset):
         import torch
         model.maxEpochs = self.iterations
         start_lr = self.minLR
         end_lr = self.maxLR
 
         def cyclical_lr(x):
             return math.exp(x * math.log(end_lr / start_lr) / (model.maxEpochs * len(dataset.trainingData)))
+        
+        for param_group in model.optimizer.param_groups:
+            param_group['lr'] = start_lr
 
         model.batchScheduler = torch.optim.lr_scheduler.LambdaLR(model.optimizer, cyclical_lr)
         model.skipValidation = True
 
 
     def onBatchEnd(self, model, batchIndex):
         lr_step = model.optimizer.state_dict()["param_groups"][0]["lr"]
 
         # smooth the loss
-        loss = model.runningStats["loss"]
+        loss = model.runningStats["loss"] / (batchIndex + 1)
         if batchIndex == 0 and model.epoch == 0:
             loss_smooth = loss
         else:
-            loss_smooth = self.smoothing * loss + (1 - self.smoothing) * self.lr_find_loss[-1]
+            loss_smooth = self.smoothing * loss + (1 - self.smoothing) * self.lastLoss
         
+        self.lastLoss = loss_smooth        
         self.logger.addCsvRow({
             "step": lr_step,
             "loss": loss,
-            "loss_smooth": lr_step,
+            "loss_smooth": loss_smooth,
         })
```

### Comparing `pyPhasesML-0.7.8/pyPhasesML/adapter/torch/LoadOptimizer.py` & `pyPhasesML-0.7.9/pyPhasesML/adapter/torch/LoadOptimizer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/adapter/torch/SystemCheckPoint.py` & `pyPhasesML-0.7.9/pyPhasesML/adapter/torch/SystemCheckPoint.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/config.yaml` & `pyPhasesML-0.7.9/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/datapipes/DatasetXY.py` & `pyPhasesML-0.7.9/pyPhasesML/datapipes/DatasetXY.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/datapipes/FoldMapper.py` & `pyPhasesML-0.7.9/pyPhasesML/datapipes/FoldMapper.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.7.9/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.7.9/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.7.9/pyPhasesML/scorer/Scorer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.7.9/pyPhasesML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.7.8
+Version: 0.7.9
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.7.8/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.7.9/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.8/setup.py` & `pyPhasesML-0.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.7.8"[1:],
+    version="v0.7.9"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

