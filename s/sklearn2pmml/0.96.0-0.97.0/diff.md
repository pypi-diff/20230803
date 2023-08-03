# Comparing `tmp/sklearn2pmml-0.96.0.tar.gz` & `tmp/sklearn2pmml-0.97.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sklearn2pmml-0.96.0.tar", last modified: Sun Jul 30 06:33:42 2023, max compression
+gzip compressed data, was "dist/sklearn2pmml-0.97.0.tar", last modified: Thu Aug  3 12:57:47 2023, max compression
```

## Comparing `sklearn2pmml-0.96.0.tar` & `sklearn2pmml-0.97.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.96.0/setup.cfg
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.96.0/LICENSE.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1403 2023-07-16 18:17:01.000000 sklearn2pmml-0.96.0/setup.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/PKG-INFO
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/h2o.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/ruleset/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/ruleset/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/pipeline/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/pipeline/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/tpot.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    12289 2023-07-14 16:34:45.000000 sklearn2pmml-0.96.0/sklearn2pmml/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/decoration/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16924 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/decoration/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/neural_network/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/neural_network/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/pycaret.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/util/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/util/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/xgboost.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/feature_extraction/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.96.0/sklearn2pmml/feature_extraction/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/feature_extraction/text/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/feature_extraction/text/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/ensemble/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     9294 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/ensemble/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4574 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/statsmodels.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/feature_selection/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/feature_selection/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/postprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/postprocessing/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  3041245 2023-07-30 06:21:29.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/guava-32.1.1-jre.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7311 2023-07-30 06:21:30.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.33.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    51724 2023-07-30 06:21:29.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-h2o-1.2.9.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/jcommander-1.72.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   198931 2023-07-30 06:21:29.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-converter-1.5.5.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    68200 2023-07-30 06:21:29.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-lightgbm-1.4.6.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-model-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    82951 2023-07-30 06:21:30.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.33.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/ubjson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   283367 2023-07-30 06:21:29.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/gson-2.10.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   442631 2023-07-30 06:21:29.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/h2o-genmodel-3.42.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      818 2023-07-30 06:21:29.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/classpath.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-07-30 06:21:29.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/h2o-logger-3.42.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     5761 2023-07-30 06:21:30.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   209112 2023-07-30 06:21:29.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-python-1.1.17.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/serpent-1.40.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   470133 2023-07-30 06:21:30.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-sklearn-1.7.33.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7767 2023-07-30 06:21:30.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.33.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6239 2023-07-30 06:21:30.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.33.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7976 2023-07-30 06:21:30.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.33.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    30899 2023-07-30 06:21:30.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-statsmodels-1.0.5.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    54294 2023-06-11 07:47:11.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pickle-1.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-07-30 06:21:30.000000 sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-xgboost-1.7.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-07-30 05:57:43.000000 sklearn2pmml-0.96.0/sklearn2pmml/metadata.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/preprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/preprocessing/h2o.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16423 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/preprocessing/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/preprocessing/xgboost.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/preprocessing/lightgbm.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/tree/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/tree/chaid.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/tree/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-30 06:33:42.000000 sklearn2pmml-0.96.0/sklearn2pmml/expression/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.96.0/sklearn2pmml/expression/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.97.0/setup.cfg
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.97.0/LICENSE.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1403 2023-07-16 18:17:01.000000 sklearn2pmml-0.97.0/setup.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/PKG-INFO
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/h2o.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/ruleset/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/ruleset/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/pipeline/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/pipeline/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/tpot.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    12365 2023-07-31 06:07:51.000000 sklearn2pmml-0.97.0/sklearn2pmml/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/decoration/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16924 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/decoration/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/neural_network/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/neural_network/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/pycaret.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/util/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/util/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/xgboost.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/feature_extraction/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.97.0/sklearn2pmml/feature_extraction/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/feature_extraction/text/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/feature_extraction/text/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/ensemble/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     9294 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/ensemble/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4574 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/statsmodels.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/feature_selection/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/feature_selection/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/postprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/postprocessing/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   474695 2023-08-03 12:40:49.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-1.7.34.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  3041245 2023-07-18 12:18:27.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/guava-32.1.1-jre.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    51724 2023-07-22 06:57:40.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-h2o-1.2.9.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/jcommander-1.72.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   198931 2023-07-20 20:18:17.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-converter-1.5.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    68200 2023-07-21 08:53:01.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-lightgbm-1.4.6.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-model-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6242 2023-08-03 12:40:52.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.34.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/ubjson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   283367 2023-07-21 09:00:16.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/gson-2.10.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   442631 2023-07-30 05:41:05.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/h2o-genmodel-3.42.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      818 2023-08-03 12:46:00.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/classpath.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-07-30 05:41:05.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/h2o-logger-3.42.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4888 2023-08-03 12:46:01.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   209112 2023-07-21 07:47:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-python-1.1.17.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7357 2023-08-03 12:40:52.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.34.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/serpent-1.40.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7767 2023-08-03 12:40:51.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.34.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    84465 2023-08-03 12:40:51.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.34.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7977 2023-08-03 12:40:52.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.34.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    30899 2023-07-21 19:03:56.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-statsmodels-1.0.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    54294 2023-06-11 07:47:11.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pickle-1.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-07-21 09:07:53.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-xgboost-1.7.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-08-03 12:45:30.000000 sklearn2pmml-0.97.0/sklearn2pmml/metadata.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/h2o.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16423 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/xgboost.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/lightgbm.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/tree/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/tree/chaid.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/tree/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/expression/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/expression/__init__.py
```

### Comparing `sklearn2pmml-0.96.0/LICENSE.txt` & `sklearn2pmml-0.97.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/setup.py` & `sklearn2pmml-0.97.0/setup.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/PKG-INFO` & `sklearn2pmml-0.97.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: sklearn2pmml
-Version: 0.96.0
+Version: 0.97.0
 Summary: Python library for converting Scikit-Learn pipelines to PMML
 Home-page: https://github.com/jpmml/sklearn2pmml
 Author: Villu Ruusmann
 Author-email: villu.ruusmann@gmail.com
 License: GNU Affero General Public License (AGPL) version 3.0
-Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.96.0.tar.gz
+Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.97.0.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/h2o.py` & `sklearn2pmml-0.97.0/sklearn2pmml/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/ruleset/__init__.py` & `sklearn2pmml-0.97.0/sklearn2pmml/ruleset/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/pipeline/__init__.py` & `sklearn2pmml-0.97.0/sklearn2pmml/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/tpot.py` & `sklearn2pmml-0.97.0/sklearn2pmml/tpot.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/__init__.py` & `sklearn2pmml-0.97.0/sklearn2pmml/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,22 +88,14 @@
 		self.selector.fit(X, y, **fit_params)
 		self._copy_attrs()
 		return self
 
 	def transform(self, X):
 		return self.selector.transform(X)
 
-def _get_steps(obj):
-	if isinstance(obj, Pipeline):
-		return obj.steps
-	elif isinstance(obj, BaseEstimator):
-		return [("estimator", obj)]
-	else:
-		raise TypeError("The object is not an instance of {0}".format(BaseEstimator.__name__))
-
 def _escape(obj, escape_func):
 	if isinstance(obj, DataFrameMapper):
 		obj.features = _escape_steps(obj.features, escape_func = escape_func)
 		if hasattr(obj, "built_features"):
 			if obj.built_features is not None:
 				obj.built_features = _escape_steps(obj.built_features, escape_func = escape_func)
 	elif isinstance(obj, ColumnTransformer):
@@ -120,31 +112,35 @@
 	elif isinstance(obj, list):
 		return [escape_func(e, escape_func = escape_func) for e in obj]
 	return obj
 
 def _escape_steps(steps, escape_func):
 	return [(step[:1] + (escape_func(step[1], escape_func = escape_func), ) + step[2:]) for step in steps]
 
-def make_pmml_pipeline(obj, active_fields = None, target_fields = None, escape_func = _escape):
-	"""Translates a regular Scikit-Learn estimator or pipeline to a PMML pipeline.
+def make_pmml_pipeline(estimator, active_fields = None, target_fields = None, escape_func = _escape):
+	"""Wraps a Scikit-Learn estimator or pipeline object into a PMML pipeline object.
 
 	Parameters:
 	----------
-	obj: BaseEstimator
-		The object.
+	estimator: BaseEstimator
+		The estimator or pipeline object.
 
 	active_fields: list of strings, optional
 		Feature names. If missing, "x1", "x2", .., "xn" are assumed.
 
 	target_fields: list of strings, optional
 		Label name(s). If missing, "y" is assumed.
 
 	"""
-	steps = _escape_steps(_get_steps(obj), escape_func = escape_func)
-	pipeline = PMMLPipeline(steps)
+	if not isinstance(estimator, BaseEstimator):
+		raise TypeError("The estimator object is not an instance of {0}".format(BaseEstimator.__name__))
+	pipeline = PMMLPipeline([
+		("estimator", estimator)
+	])
+	pipeline = _escape(pipeline, escape_func = escape_func)
 	if active_fields is not None:
 		pipeline.active_fields = numpy.asarray(active_fields)
 	if target_fields is not None:
 		pipeline.target_fields = numpy.asarray(target_fields)
 	return pipeline
 
 def _make_java_command(java_home, java_opts, java_args):
@@ -210,27 +206,27 @@
 	fd, path = tempfile.mkstemp(prefix = (prefix + "-"), suffix = ".pkl.z")
 	try:
 		joblib.dump(obj, path, compress = 3)
 	finally:
 		os.close(fd)
 	return path
 
-def sklearn2pmml(pipeline, pmml, with_repr = False, java_home = None, java_opts = None, user_classpath = [], dump_flavour = "joblib", debug = False):
-	"""Converts a fitted PMML pipeline object to PMML file.
+def sklearn2pmml(estimator, pmml_path, with_repr = False, java_home = None, java_opts = None, user_classpath = [], dump_flavour = "joblib", debug = False):
+	"""Converts a fitted estimator or pipeline object to PMML.
 
 	Parameters:
 	----------
-	pipeline: PMMLPipeline
-		The input PMML pipeline object.
+	estimator: BaseEstimator
+		The estimator or pipeline object.
 
-	pmml: string
-		The path to output PMML file.
+	pmml_path: string
+		The file path where the PMML document should be saved.
 
 	with_repr: boolean, optional
-		If true, insert the string representation of pipeline into the PMML document.
+		If true, insert a string containing a printable representation of the estimator object into the PMML document.
 
 	java_home: string, optional
 		The path to Java installation directory.
 		Functionally analogous to the JAVA_HOME environment variable.
 
 	java_opts: list of strings, optional
 		Java options.
@@ -248,48 +244,53 @@
 
 	"""
 	if debug:
 		java_version = _java_version(java_home = java_home)
 		if java_version is None:
 			java_version = ("java", "N/A")
 		print("python: {0}".format(platform.python_version()))
-		print("sklearn: {0}".format(sklearn.__version__))
 		print("sklearn2pmml: {0}".format(__version__))
-		print("joblib: {0}".format(joblib.__version__))
+		print("sklearn: {0}".format(sklearn.__version__))
 		print("sklearn_pandas: {0}".format(sklearn_pandas.__version__))
 		print("pandas: {0}".format(pandas.__version__))
 		print("numpy: {0}".format(numpy.__version__))
+		print("dill: {0}".format(dill.__version__))
+		print("joblib: {0}".format(joblib.__version__))
 		print("{0}: {1}".format(java_version[0], java_version[1]))
-	if not isinstance(pipeline, PMMLPipeline):
-		raise TypeError("The pipeline object is not an instance of {0}. Use the 'sklearn2pmml.make_pmml_pipeline(obj)' utility function to translate a regular Scikit-Learn pipeline or estimator to a PMML pipeline".format(PMMLPipeline.__name__))
-	if with_repr:
-		pipeline.repr_ = repr(pipeline)
+	if not isinstance(estimator, BaseEstimator):
+		raise TypeError("The estimator object is not an instance of {0}".format(BaseEstimator.__name__))
+	# if isinstance(estimator, Pipeline):
+	if hasattr(estimator, "_final_estimator"):
+		final_estimator = estimator._final_estimator
+	else:
+		final_estimator = estimator
 	dumps = []
 	try:
 		java_args = ["-cp", os.pathsep.join(_classpath(user_classpath)), "com.sklearn2pmml.Main"]
-		estimator = pipeline._final_estimator
-		# if isinstance(estimator, H2OEstimator):
-		if hasattr(estimator, "download_mojo"):
+		if with_repr:
+			estimator.repr_ = repr(estimator)
+		# if isinstance(final_estimator, H2OEstimator):
+		if hasattr(final_estimator, "download_mojo"):
 			if dump_flavour != "dill":
 				warnings.warn("Changing dump flavour to dill")
 				dump_flavour = "dill"
 			# Avoid MOJO (re-)download if the indicator attribute is set
-			if not hasattr(estimator, "_mojo_path"):
-				estimator_mojo = estimator.download_mojo()
-				dumps.append(estimator_mojo)
-				estimator._mojo_path = estimator_mojo
+			if not hasattr(final_estimator, "_mojo_path"):
+				mojo_path = final_estimator.download_mojo()
+				dumps.append(mojo_path)
+				final_estimator._mojo_path = mojo_path
 		if dump_flavour == "dill":
-			pipeline_pkl = _dill_dump(pipeline, "pipeline")
+			pkl_path = _dill_dump(estimator, "estimator")
 		elif dump_flavour == "joblib":
-			pipeline_pkl = _joblib_dump(pipeline, "pipeline")
+			pkl_path = _joblib_dump(estimator, "estimator")
 		else:
 			raise ValueError("Dump flavour {0} not in {1}".format(dump_flavour, ["dill", "joblib"]))
-		java_args.extend(["--pkl-pipeline-input", pipeline_pkl])
-		dumps.append(pipeline_pkl)
-		java_args.extend(["--pmml-output", pmml])
+		java_args.extend(["--pkl-input", pkl_path])
+		dumps.append(pkl_path)
+		java_args.extend(["--pmml-output", pmml_path])
 		cmd = _make_java_command(java_home = java_home, java_opts = java_opts, java_args = java_args)
 		if debug:
 			print("Executing command:\n{0}".format(" ".join(cmd)))
 		try:
 			process = Popen(cmd, stdout = PIPE, stderr = PIPE, bufsize = 1, universal_newlines = True)
 		except OSError:
 			raise RuntimeError("Java is not installed, or the Java executable is not on system path")
```

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/decoration/__init__.py` & `sklearn2pmml-0.97.0/sklearn2pmml/decoration/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/neural_network/__init__.py` & `sklearn2pmml-0.97.0/sklearn2pmml/neural_network/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/pycaret.py` & `sklearn2pmml-0.97.0/sklearn2pmml/pycaret.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/util/__init__.py` & `sklearn2pmml-0.97.0/sklearn2pmml/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/xgboost.py` & `sklearn2pmml-0.97.0/sklearn2pmml/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/feature_extraction/text/__init__.py` & `sklearn2pmml-0.97.0/sklearn2pmml/feature_extraction/text/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/ensemble/__init__.py` & `sklearn2pmml-0.97.0/sklearn2pmml/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/statsmodels.py` & `sklearn2pmml-0.97.0/sklearn2pmml/statsmodels.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/feature_selection/__init__.py` & `sklearn2pmml-0.97.0/sklearn2pmml/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/postprocessing/__init__.py` & `sklearn2pmml-0.97.0/sklearn2pmml/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/guava-32.1.1-jre.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/guava-32.1.1-jre.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.33.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.34.jar`

 * *Files 17% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 7311 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jul-30 08:48 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 lightgbm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 lightgbm/sklearn/
--rw-rw-r--  2.0 unx      177 b- defN 23-Jul-30 08:48 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      170 b- defN 23-Jul-30 08:48 lightgbm/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     1953 b- defN 23-Jul-30 08:48 lightgbm/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2102 b- defN 23-Jul-30 08:48 lightgbm/sklearn/LGBMRegressor.class
--rw-rw-r--  2.0 unx     2126 b- defN 23-Jul-30 08:48 lightgbm/sklearn/LGBMClassifier.class
--rw-rw-r--  2.0 unx     3298 b- defN 23-Jul-30 08:48 lightgbm/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
--rw-rw-r--  2.0 unx     1319 b- defN 23-Jul-30 08:47 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
--rw-rw-r--  2.0 unx      117 b- defN 23-Jul-30 08:48 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
-15 files, 11392 bytes uncompressed, 5231 bytes compressed:  54.1%
+Zip file size: 7357 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Aug-03 15:40 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 lightgbm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 lightgbm/sklearn/
+-rw-rw-r--  2.0 unx      177 b- defN 23-Aug-03 15:40 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      170 b- defN 23-Aug-03 15:40 lightgbm/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     2047 b- defN 23-Aug-03 15:40 lightgbm/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2102 b- defN 23-Aug-03 15:40 lightgbm/sklearn/LGBMRegressor.class
+-rw-rw-r--  2.0 unx     2126 b- defN 23-Aug-03 15:40 lightgbm/sklearn/LGBMClassifier.class
+-rw-rw-r--  2.0 unx     3298 b- defN 23-Aug-03 15:40 lightgbm/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
+-rw-rw-r--  2.0 unx     1319 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
+-rw-rw-r--  2.0 unx      117 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
+15 files, 11486 bytes uncompressed, 5277 bytes compressed:  54.1%
```

#### lightgbm/sklearn/Booster.class

##### procyon -ec {}

```diff
@@ -34,10 +34,13 @@
         }
         catch (final IOException ioe) {
             throw new RuntimeException(ioe);
         }
     }
     
     public String getHandle() {
-        return this.getString("handle");
+        if (this.containsKey((Object)"handle")) {
+            return this.getString("handle");
+        }
+        return this.getString("_handle");
     }
 }
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.33</version>
+    <version>1.7.34</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-lightgbm</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn LightGBM converter</name>
   <description>JPMML Scikit-Learn LightGBM to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Sun Jul 30 08:48:19 EEST 2023
-version=1.7.33
+#Thu Aug 03 15:40:51 EEST 2023
+version=1.7.34
 groupId=org.jpmml
 artifactId=pmml-sklearn-lightgbm
```

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-h2o-1.2.9.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-h2o-1.2.9.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/jcommander-1.72.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/jcommander-1.72.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-converter-1.5.5.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-converter-1.5.5.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-lightgbm-1.4.6.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-lightgbm-1.4.6.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-model-1.6.4.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-model-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.33.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.34.jar`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,65 +1,67 @@
-Zip file size: 82951 bytes, number of entries: 63
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jul-30 08:48 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 pycaret/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 pycaret/preprocess/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 tpot/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 tpot/builtins/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 optbinning/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 optbinning/scorecard/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 imblearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 category_encoders/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklego/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklego/meta/
--rw-rw-r--  2.0 unx     4312 b- defN 23-Jul-30 08:48 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      412 b- defN 23-Jul-30 08:48 pycaret/preprocess/FixImbalancer.class
--rw-rw-r--  2.0 unx     2818 b- defN 23-Jul-30 08:48 pycaret/preprocess/RemoveMulticollinearity.class
--rw-rw-r--  2.0 unx      421 b- defN 23-Jul-30 08:48 pycaret/preprocess/CleanColumnNames.class
--rw-rw-r--  2.0 unx     1332 b- defN 23-Jul-30 08:48 pycaret/preprocess/RemoveOutliers$1.class
--rw-rw-r--  2.0 unx     2747 b- defN 23-Jul-30 08:48 pycaret/preprocess/RareCategoryGrouping.class
--rw-rw-r--  2.0 unx     3125 b- defN 23-Jul-30 08:48 pycaret/preprocess/RemoveOutliers.class
--rw-rw-r--  2.0 unx     7830 b- defN 23-Jul-30 08:48 pycaret/preprocess/TransformerWrapper.class
--rw-rw-r--  2.0 unx     4174 b- defN 23-Jul-30 08:48 pycaret/preprocess/TransformerWrapperWithInverse.class
--rw-rw-r--  2.0 unx      720 b- defN 23-Jul-30 08:48 tpot/builtins/StackingEstimator$1.class
--rw-rw-r--  2.0 unx     4530 b- defN 23-Jul-30 08:48 tpot/builtins/StackingEstimator.class
--rw-rw-r--  2.0 unx     2433 b- defN 23-Jul-30 08:48 optbinning/BinnedFeature.class
--rw-rw-r--  2.0 unx     8333 b- defN 23-Jul-30 08:48 optbinning/scorecard/Scorecard.class
--rw-rw-r--  2.0 unx     2133 b- defN 23-Jul-30 08:48 optbinning/OptimalBinningUtil.class
--rw-rw-r--  2.0 unx     6372 b- defN 23-Jul-30 08:48 optbinning/BinningProcess.class
--rw-rw-r--  2.0 unx     2274 b- defN 23-Jul-30 08:48 optbinning/ContinuousOptimalBinning.class
--rw-rw-r--  2.0 unx     3917 b- defN 23-Jul-30 08:48 optbinning/MulticlassOptimalBinning.class
--rw-rw-r--  2.0 unx     1240 b- defN 23-Jul-30 08:48 optbinning/BinningProcess$1.class
--rw-rw-r--  2.0 unx    14050 b- defN 23-Jul-30 08:48 optbinning/OptimalBinning.class
--rw-rw-r--  2.0 unx      374 b- defN 23-Jul-30 08:48 imblearn/Sampler.class
--rw-rw-r--  2.0 unx     1916 b- defN 23-Jul-30 08:48 category_encoders/MapEncoder.class
--rw-rw-r--  2.0 unx     8449 b- defN 23-Jul-30 08:48 category_encoders/MapFeature.class
--rw-rw-r--  2.0 unx      527 b- defN 23-Jul-30 08:48 category_encoders/TargetEncoder.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-Jul-30 08:48 category_encoders/CountEncoder$1.class
--rw-rw-r--  2.0 unx      515 b- defN 23-Jul-30 08:48 category_encoders/WOEEncoder.class
--rw-rw-r--  2.0 unx     8474 b- defN 23-Jul-30 08:48 category_encoders/MeanEncoder.class
--rw-rw-r--  2.0 unx     8520 b- defN 23-Jul-30 08:48 category_encoders/CountEncoder.class
--rw-rw-r--  2.0 unx    12815 b- defN 23-Jul-30 08:48 category_encoders/BaseNFeature.class
--rw-rw-r--  2.0 unx     1481 b- defN 23-Jul-30 08:48 category_encoders/OrdinalMapEncoder$1.class
--rw-rw-r--  2.0 unx     1445 b- defN 23-Jul-30 08:48 category_encoders/MeanEncoder$1.class
--rw-rw-r--  2.0 unx     2119 b- defN 23-Jul-30 08:48 category_encoders/OrdinalEncoder$Mapping.class
--rw-rw-r--  2.0 unx     1323 b- defN 23-Jul-30 08:48 category_encoders/LeaveOneOutEncoder$1.class
--rw-rw-r--  2.0 unx     8108 b- defN 23-Jul-30 08:48 category_encoders/OrdinalMapEncoder.class
--rw-rw-r--  2.0 unx     9241 b- defN 23-Jul-30 08:48 category_encoders/BaseNEncoder.class
--rw-rw-r--  2.0 unx     1334 b- defN 23-Jul-30 08:48 category_encoders/BinaryEncoder.class
--rw-rw-r--  2.0 unx     3547 b- defN 23-Jul-30 08:48 category_encoders/OneHotEncoder.class
--rw-rw-r--  2.0 unx     1325 b- defN 23-Jul-30 08:48 category_encoders/CatBoostEncoder.class
--rw-rw-r--  2.0 unx     2062 b- defN 23-Jul-30 08:48 category_encoders/CategoryEncoderUtil.class
--rw-rw-r--  2.0 unx     1564 b- defN 23-Jul-30 08:48 category_encoders/OrdinalEncoder$1.class
--rw-rw-r--  2.0 unx     1047 b- defN 23-Jul-30 08:48 category_encoders/LeaveOneOutEncoder.class
--rw-rw-r--  2.0 unx     4690 b- defN 23-Jul-30 08:48 category_encoders/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      742 b- defN 23-Jul-30 08:48 category_encoders/MeanEncoder$MeanFunction.class
--rw-rw-r--  2.0 unx     1378 b- defN 23-Jul-30 08:48 category_encoders/CatBoostEncoder$1.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-Jul-30 08:48 category_encoders/CategoryEncoder.class
--rw-rw-r--  2.0 unx      725 b- defN 23-Jul-30 08:48 sklego/meta/EstimatorTransformer$1.class
--rw-rw-r--  2.0 unx     7272 b- defN 23-Jul-30 08:48 sklego/meta/EstimatorTransformer.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/org.jpmml/pmml-sklearn-extension/
--rw-rw-r--  2.0 unx     1226 b- defN 23-Jul-30 08:47 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
--rw-rw-r--  2.0 unx      118 b- defN 23-Jul-30 08:48 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
-63 files, 169253 bytes uncompressed, 73885 bytes compressed:  56.3%
+Zip file size: 84465 bytes, number of entries: 65
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Aug-03 15:40 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 pycaret/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 pycaret/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 pycaret/preprocess/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 tpot/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 tpot/builtins/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 optbinning/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 optbinning/scorecard/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 imblearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 category_encoders/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklego/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklego/meta/
+-rw-rw-r--  2.0 unx     4312 b- defN 23-Aug-03 15:40 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     2928 b- defN 23-Aug-03 15:40 pycaret/pipeline/Pipeline.class
+-rw-rw-r--  2.0 unx      412 b- defN 23-Aug-03 15:40 pycaret/preprocess/FixImbalancer.class
+-rw-rw-r--  2.0 unx     2818 b- defN 23-Aug-03 15:40 pycaret/preprocess/RemoveMulticollinearity.class
+-rw-rw-r--  2.0 unx      421 b- defN 23-Aug-03 15:40 pycaret/preprocess/CleanColumnNames.class
+-rw-rw-r--  2.0 unx     1332 b- defN 23-Aug-03 15:40 pycaret/preprocess/RemoveOutliers$1.class
+-rw-rw-r--  2.0 unx     2747 b- defN 23-Aug-03 15:40 pycaret/preprocess/RareCategoryGrouping.class
+-rw-rw-r--  2.0 unx     3125 b- defN 23-Aug-03 15:40 pycaret/preprocess/RemoveOutliers.class
+-rw-rw-r--  2.0 unx     7826 b- defN 23-Aug-03 15:40 pycaret/preprocess/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     4170 b- defN 23-Aug-03 15:40 pycaret/preprocess/TransformerWrapperWithInverse.class
+-rw-rw-r--  2.0 unx      720 b- defN 23-Aug-03 15:40 tpot/builtins/StackingEstimator$1.class
+-rw-rw-r--  2.0 unx     4530 b- defN 23-Aug-03 15:40 tpot/builtins/StackingEstimator.class
+-rw-rw-r--  2.0 unx     2433 b- defN 23-Aug-03 15:40 optbinning/BinnedFeature.class
+-rw-rw-r--  2.0 unx     8333 b- defN 23-Aug-03 15:40 optbinning/scorecard/Scorecard.class
+-rw-rw-r--  2.0 unx     2133 b- defN 23-Aug-03 15:40 optbinning/OptimalBinningUtil.class
+-rw-rw-r--  2.0 unx     6372 b- defN 23-Aug-03 15:40 optbinning/BinningProcess.class
+-rw-rw-r--  2.0 unx     2274 b- defN 23-Aug-03 15:40 optbinning/ContinuousOptimalBinning.class
+-rw-rw-r--  2.0 unx     3917 b- defN 23-Aug-03 15:40 optbinning/MulticlassOptimalBinning.class
+-rw-rw-r--  2.0 unx     1240 b- defN 23-Aug-03 15:40 optbinning/BinningProcess$1.class
+-rw-rw-r--  2.0 unx    14050 b- defN 23-Aug-03 15:40 optbinning/OptimalBinning.class
+-rw-rw-r--  2.0 unx      374 b- defN 23-Aug-03 15:40 imblearn/Sampler.class
+-rw-rw-r--  2.0 unx     1916 b- defN 23-Aug-03 15:40 category_encoders/MapEncoder.class
+-rw-rw-r--  2.0 unx     8449 b- defN 23-Aug-03 15:40 category_encoders/MapFeature.class
+-rw-rw-r--  2.0 unx      527 b- defN 23-Aug-03 15:40 category_encoders/TargetEncoder.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-Aug-03 15:40 category_encoders/CountEncoder$1.class
+-rw-rw-r--  2.0 unx      515 b- defN 23-Aug-03 15:40 category_encoders/WOEEncoder.class
+-rw-rw-r--  2.0 unx     8474 b- defN 23-Aug-03 15:40 category_encoders/MeanEncoder.class
+-rw-rw-r--  2.0 unx     8520 b- defN 23-Aug-03 15:40 category_encoders/CountEncoder.class
+-rw-rw-r--  2.0 unx    12815 b- defN 23-Aug-03 15:40 category_encoders/BaseNFeature.class
+-rw-rw-r--  2.0 unx     1481 b- defN 23-Aug-03 15:40 category_encoders/OrdinalMapEncoder$1.class
+-rw-rw-r--  2.0 unx     1445 b- defN 23-Aug-03 15:40 category_encoders/MeanEncoder$1.class
+-rw-rw-r--  2.0 unx     2119 b- defN 23-Aug-03 15:40 category_encoders/OrdinalEncoder$Mapping.class
+-rw-rw-r--  2.0 unx     1323 b- defN 23-Aug-03 15:40 category_encoders/LeaveOneOutEncoder$1.class
+-rw-rw-r--  2.0 unx     8108 b- defN 23-Aug-03 15:40 category_encoders/OrdinalMapEncoder.class
+-rw-rw-r--  2.0 unx     9241 b- defN 23-Aug-03 15:40 category_encoders/BaseNEncoder.class
+-rw-rw-r--  2.0 unx     1334 b- defN 23-Aug-03 15:40 category_encoders/BinaryEncoder.class
+-rw-rw-r--  2.0 unx     3547 b- defN 23-Aug-03 15:40 category_encoders/OneHotEncoder.class
+-rw-rw-r--  2.0 unx     1325 b- defN 23-Aug-03 15:40 category_encoders/CatBoostEncoder.class
+-rw-rw-r--  2.0 unx     2062 b- defN 23-Aug-03 15:40 category_encoders/CategoryEncoderUtil.class
+-rw-rw-r--  2.0 unx     1564 b- defN 23-Aug-03 15:40 category_encoders/OrdinalEncoder$1.class
+-rw-rw-r--  2.0 unx     1047 b- defN 23-Aug-03 15:40 category_encoders/LeaveOneOutEncoder.class
+-rw-rw-r--  2.0 unx     4690 b- defN 23-Aug-03 15:40 category_encoders/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      742 b- defN 23-Aug-03 15:40 category_encoders/MeanEncoder$MeanFunction.class
+-rw-rw-r--  2.0 unx     1378 b- defN 23-Aug-03 15:40 category_encoders/CatBoostEncoder$1.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-Aug-03 15:40 category_encoders/CategoryEncoder.class
+-rw-rw-r--  2.0 unx      725 b- defN 23-Aug-03 15:40 sklego/meta/EstimatorTransformer$1.class
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Aug-03 15:40 sklego/meta/EstimatorTransformer.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-extension/
+-rw-rw-r--  2.0 unx     1226 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
+-rw-rw-r--  2.0 unx      118 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
+65 files, 172173 bytes uncompressed, 75151 bytes compressed:  56.4%
```

#### zipnote «TEMP»/diffoscope_q23y7y7v_/tmp058dvdmz_.zip

```diff
@@ -3,14 +3,17 @@
 
 Filename: META-INF/MANIFEST.MF
 Comment: 
 
 Filename: pycaret/
 Comment: 
 
+Filename: pycaret/pipeline/
+Comment: 
+
 Filename: pycaret/preprocess/
 Comment: 
 
 Filename: tpot/
 Comment: 
 
 Filename: tpot/builtins/
@@ -33,14 +36,17 @@
 
 Filename: sklego/meta/
 Comment: 
 
 Filename: META-INF/sklearn2pmml.properties
 Comment: 
 
+Filename: pycaret/pipeline/Pipeline.class
+Comment: 
+
 Filename: pycaret/preprocess/FixImbalancer.class
 Comment: 
 
 Filename: pycaret/preprocess/RemoveMulticollinearity.class
 Comment: 
 
 Filename: pycaret/preprocess/CleanColumnNames.class
```

#### META-INF/sklearn2pmml.properties

```diff
@@ -32,15 +32,15 @@
 imblearn.under_sampling._prototype_selection._tomek_links.TomekLinks = imblearn.Sampler
 mlxtend.preprocessing.dense_transformer.DenseTransformer = sklearn.IdentityTransformer
 optbinning.binning.binning.OptimalBinning = optbinning.OptimalBinning
 optbinning.binning.continuous_binning.ContinuousOptimalBinning = optbinning.ContinuousOptimalBinning
 optbinning.binning.binning_process.BinningProcess = optbinning.BinningProcess
 optbinning.binning.multiclass_binning.MulticlassOptimalBinning = optbinning.MulticlassOptimalBinning
 optbinning.scorecard.scorecard.Scorecard = optbinning.scorecard.Scorecard
-pycaret.internal.pipeline.Pipeline = sklearn.pipeline.Pipeline
+pycaret.internal.pipeline.Pipeline = pycaret.pipeline.Pipeline
 pycaret.internal.preprocess.transformers.CleanColumnNames = pycaret.preprocess.CleanColumnNames
 pycaret.internal.preprocess.transformers.FixImbalancer = pycaret.preprocess.FixImbalancer
 pycaret.internal.preprocess.transformers.RareCategoryGrouping = pycaret.preprocess.RareCategoryGrouping
 pycaret.internal.preprocess.transformers.RemoveMulticollinearity = pycaret.preprocess.RemoveMulticollinearity
 pycaret.internal.preprocess.transformers.RemoveOutliers = pycaret.preprocess.RemoveOutliers
 pycaret.internal.preprocess.transformers.TransformerWrapper = pycaret.preprocess.TransformerWrapper
 pycaret.internal.preprocess.transformers.TransformerWrapperWithInverse = pycaret.preprocess.TransformerWrapperWithInverse
```

#### pycaret/preprocess/TransformerWrapper.class

##### procyon -ec {}

```diff
@@ -26,45 +26,45 @@
 public class TransformerWrapper extends Initializer
 {
     public TransformerWrapper(final String module, final String name) {
         super(module, name);
     }
     
     public int getNumberOfFeatures() {
-        final List<String> featureNamesIn = this.getFeatureNamesIn();
-        return featureNamesIn.size();
+        final List<String> featureNames = this.getFeatureNames();
+        return featureNames.size();
     }
     
     public void checkFeatures(final List<? extends Feature> features) {
         if (!features.isEmpty()) {
             super.checkFeatures((List)features);
         }
     }
     
     public List<Feature> initializeFeatures(final SkLearnEncoder encoder) {
         return this.encodeFeatures(Collections.emptyList(), encoder);
     }
     
     public List<Feature> encodeFeatures(List<Feature> features, final SkLearnEncoder encoder) {
-        final List<String> featureNamesIn = this.getFeatureNamesIn();
+        final List<String> featureNames = this.getFeatureNames();
         final List<String> include = this.getInclude();
         final Boolean trainOnly = this.getTrainOnly();
         final Transformer transformer = this.getTransformer();
         if ((boolean)trainOnly) {
             return features;
         }
         if (features.isEmpty()) {
-            features = InitializerUtil.selectFeatures((List)featureNamesIn, (List)features, encoder);
+            features = InitializerUtil.selectFeatures((List)featureNames, (List)features, encoder);
         }
         final List<Feature> includeFeatures = new ArrayList<Feature>();
         for (int i = 0; i < include.size(); ++i) {
             final String includeColumn = (String)include.get(i);
             Feature includeFeature;
             if (!features.isEmpty()) {
-                final int index = featureNamesIn.indexOf(includeColumn);
+                final int index = featureNames.indexOf(includeColumn);
                 includeFeature = features.get(index);
             }
             else {
                 includeFeature = InitializerUtil.selectFeature(includeColumn, (List)features, encoder);
             }
             includeFeatures.add(includeFeature);
         }
@@ -88,15 +88,15 @@
         }
         if (replaceFeatures) {
             final List<List<Feature>> transformedIncludeFeatureGroups = groupByField(transformedIncludeFeatures);
             ClassDictUtil.checkSize(new Collection[] { includeFeatures, transformedIncludeFeatureGroups });
             final List<Object> result = new ArrayList<Object>(features);
             for (int j = 0; j < include.size(); ++j) {
                 final String includeColumn2 = (String)include.get(j);
-                final int index2 = featureNamesIn.indexOf(includeColumn2);
+                final int index2 = featureNames.indexOf(includeColumn2);
                 final List<Feature> transformedIncludeFeatureGroup = (List<Feature>)transformedIncludeFeatureGroups.get(j);
                 result.set(index2, transformedIncludeFeatureGroup);
             }
             return result.stream().flatMap(element -> {
                 if (element instanceof List) {
                     final List<Feature> featureGroup = (List)element;
                     return featureGroup.stream();
@@ -115,15 +115,15 @@
             if (labelFeature != null) {
                 result2.add(labelFeature);
             }
         }
         return result2;
     }
     
-    public List<String> getFeatureNamesIn() {
+    public List<String> getFeatureNames() {
         return this.getList("_feature_names_in", (Class)String.class);
     }
     
     public List<String> getExclude() {
         return this.getList("_exclude", (Class)String.class);
     }
```

#### pycaret/preprocess/TransformerWrapperWithInverse.class

##### procyon -ec {}

```diff
@@ -24,23 +24,23 @@
 public class TransformerWrapperWithInverse extends TransformerWrapper
 {
     public TransformerWrapperWithInverse(final String module, final String name) {
         super(module, name);
     }
     
     public List<Feature> encodeFeatures(final List<Feature> features, final SkLearnEncoder encoder) {
-        final List<String> featureNamesIn = this.getFeatureNamesIn();
+        final List<String> featureNames = this.getFeatureNames();
         final LabelEncoder transformer = this.getTransformer();
         final Label label = encoder.getLabel();
         if (label == null) {
             throw new IllegalArgumentException();
         }
         List<Feature> result;
         if (features.isEmpty()) {
-            result = InitializerUtil.selectFeatures((List)featureNamesIn, (List)Collections.emptyList(), encoder);
+            result = InitializerUtil.selectFeatures((List)featureNames, (List)Collections.emptyList(), encoder);
         }
         else {
             result = features;
         }
         ScalarLabel scalarLabel = (ScalarLabel)label;
         final Feature labelFeature = FeatureUtil.findLabelFeature((List)result, scalarLabel);
         if (labelFeature == null) {
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.33</version>
+    <version>1.7.34</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-extension</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn extensions converter</name>
   <description>JPMML Scikit-Learn extension packages to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Sun Jul 30 08:48:18 EEST 2023
-version=1.7.33
+#Thu Aug 03 15:40:51 EEST 2023
+version=1.7.34
 groupId=org.jpmml
 artifactId=pmml-sklearn-extension
```

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/ubjson-0.1.8.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/ubjson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/gson-2.10.1.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/gson-2.10.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/h2o-genmodel-3.42.0.2.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/h2o-genmodel-3.42.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/classpath.txt` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/classpath.txt`

 * *Files 13% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 pickle-1.4.jar
 pmml-converter-1.5.5.jar
 pmml-h2o-1.2.9.jar
 pmml-lightgbm-1.4.6.jar
 pmml-model-1.6.4.jar
 pmml-model-metro-1.6.4.jar
 pmml-python-1.1.17.jar
-pmml-sklearn-1.7.33.jar
-pmml-sklearn-extension-1.7.33.jar
-pmml-sklearn-h2o-1.7.33.jar
-pmml-sklearn-lightgbm-1.7.33.jar
-pmml-sklearn-statsmodels-1.7.33.jar
-pmml-sklearn-xgboost-1.7.33.jar
+pmml-sklearn-1.7.34.jar
+pmml-sklearn-extension-1.7.34.jar
+pmml-sklearn-h2o-1.7.34.jar
+pmml-sklearn-lightgbm-1.7.34.jar
+pmml-sklearn-statsmodels-1.7.34.jar
+pmml-sklearn-xgboost-1.7.34.jar
 pmml-statsmodels-1.0.5.jar
 pmml-xgboost-1.7.4.jar
 serpent-1.40.jar
 slf4j-api-1.7.36.jar
 slf4j-jdk14-1.7.36.jar
 ubjson-0.1.8.jar
 ubjson-gson-0.1.8.jar
```

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/h2o-logger-3.42.0.2.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/h2o-logger-3.42.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-python-1.1.17.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-python-1.1.17.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/serpent-1.40.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/serpent-1.40.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-sklearn-1.7.33.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-1.7.34.jar`

 * *Files 13% similar despite different names*

#### zipinfo {}

```diff
@@ -1,406 +1,412 @@
-Zip file size: 470133 bytes, number of entries: 404
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/
--rw-r--r--  2.0 unx      159 b- defN 23-Jul-30 08:48 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn_pandas/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 chaid/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 stop_words/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/calibration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/dummy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/svm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/impute/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/naive_bayes/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/linear_model/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/linear_model/logistic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/linear_model/ridge/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/linear_model/glm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/linear_model/stochastic_gradient/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/compose/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/model_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/decomposition/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/neighbors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/multioutput/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/isotonic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/metrics/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/ensemble/bagging/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/ensemble/stacking/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/ensemble/forest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/ensemble/iforest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/ensemble/voting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/ensemble/hist_gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/ensemble/weight_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/loss/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/discriminant_analysis/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/tree/visitors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/cluster/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn/multiclass/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/ruleset/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/decoration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/util/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/postprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/expression/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 org/jpmml/sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 org/jpmml/sklearn/testing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/org.jpmml/pmml-sklearn/
--rw-rw-r--  2.0 unx    16829 b- defN 23-Jul-30 08:48 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     2287 b- defN 23-Jul-30 08:48 sklearn_pandas/CategoricalImputer.class
--rw-rw-r--  2.0 unx      656 b- defN 23-Jul-30 08:48 sklearn_pandas/TransformerPipeline.class
--rw-rw-r--  2.0 unx     1154 b- defN 23-Jul-30 08:48 sklearn_pandas/DataFrameMapper$2.class
--rw-rw-r--  2.0 unx     6280 b- defN 23-Jul-30 08:48 sklearn_pandas/DataFrameMapper.class
--rw-rw-r--  2.0 unx     1126 b- defN 23-Jul-30 08:48 sklearn_pandas/DataFrameMapper$1.class
--rw-rw-r--  2.0 unx      609 b- defN 23-Jul-30 08:48 chaid/ContinuousColumn.class
--rw-rw-r--  2.0 unx      925 b- defN 23-Jul-30 08:48 chaid/Node.class
--rw-rw-r--  2.0 unx      467 b- defN 23-Jul-30 08:48 chaid/Column.class
--rw-rw-r--  2.0 unx     3283 b- defN 23-Jul-30 08:48 chaid/Split.class
--rw-rw-r--  2.0 unx      401 b- defN 23-Jul-30 08:48 chaid/InvalidSplitReason.class
--rw-rw-r--  2.0 unx      602 b- defN 23-Jul-30 08:48 chaid/NominalColumn.class
--rw-rw-r--  2.0 unx     1912 b- defN 23-Jul-30 08:48 stop_words/english.txt
--rw-rw-r--  2.0 unx      147 b- defN 23-Jul-30 08:48 sklearn/HasHead.class
--rw-rw-r--  2.0 unx     1728 b- defN 23-Jul-30 08:48 sklearn/StepUtil.class
--rw-rw-r--  2.0 unx    12045 b- defN 23-Jul-30 08:48 sklearn/calibration/CalibratedClassifier.class
--rw-rw-r--  2.0 unx     2953 b- defN 23-Jul-30 08:48 sklearn/calibration/SigmoidCalibration.class
--rw-rw-r--  2.0 unx      683 b- defN 23-Jul-30 08:48 sklearn/calibration/CalibratedClassifier$1.class
--rw-rw-r--  2.0 unx     3672 b- defN 23-Jul-30 08:48 sklearn/calibration/CalibratedClassifierCV.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-Jul-30 08:48 sklearn/pipeline/PipelineTransformer.class
--rw-rw-r--  2.0 unx     1671 b- defN 23-Jul-30 08:48 sklearn/pipeline/Pipeline$2.class
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jul-30 08:48 sklearn/pipeline/FeatureUnion.class
--rw-rw-r--  2.0 unx     5062 b- defN 23-Jul-30 08:48 sklearn/pipeline/Pipeline.class
--rw-rw-r--  2.0 unx     2003 b- defN 23-Jul-30 08:48 sklearn/pipeline/PipelineRegressor.class
--rw-rw-r--  2.0 unx     1716 b- defN 23-Jul-30 08:48 sklearn/pipeline/Pipeline$1.class
--rw-rw-r--  2.0 unx     1111 b- defN 23-Jul-30 08:48 sklearn/pipeline/PipelineUtil.class
--rw-rw-r--  2.0 unx     2298 b- defN 23-Jul-30 08:48 sklearn/pipeline/PipelineClassifier.class
--rw-rw-r--  2.0 unx     4913 b- defN 23-Jul-30 08:48 sklearn/dummy/DummyClassifier.class
--rw-rw-r--  2.0 unx     2055 b- defN 23-Jul-30 08:48 sklearn/dummy/DummyRegressor.class
--rw-rw-r--  2.0 unx      454 b- defN 23-Jul-30 08:48 sklearn/SkLearnFields.class
--rw-rw-r--  2.0 unx     2293 b- defN 23-Jul-30 08:48 sklearn/SkLearnOutlierTransformation.class
--rw-rw-r--  2.0 unx      240 b- defN 23-Jul-30 08:48 sklearn/HasEstimator.class
--rw-rw-r--  2.0 unx     3421 b- defN 23-Jul-30 08:48 sklearn/OutlierDetectorUtil.class
--rw-rw-r--  2.0 unx     1236 b- defN 23-Jul-30 08:48 sklearn/HasMultiApplyField.class
--rw-rw-r--  2.0 unx     2393 b- defN 23-Jul-30 08:48 sklearn/svm/SupportVectorMachineUtil.class
--rw-rw-r--  2.0 unx     1109 b- defN 23-Jul-30 08:48 sklearn/svm/LinearSVC.class
--rw-rw-r--  2.0 unx     5037 b- defN 23-Jul-30 08:48 sklearn/svm/LibSVMClassifier.class
--rw-rw-r--  2.0 unx      966 b- defN 23-Jul-30 08:48 sklearn/svm/SupportVectorMachineUtil$1.class
--rw-rw-r--  2.0 unx     1265 b- defN 23-Jul-30 08:48 sklearn/svm/OneClassSVM.class
--rw-rw-r--  2.0 unx     3594 b- defN 23-Jul-30 08:48 sklearn/svm/LibSVMRegressor.class
--rw-rw-r--  2.0 unx     3007 b- defN 23-Jul-30 08:48 sklearn/InitializerUtil$1.class
--rw-rw-r--  2.0 unx      735 b- defN 23-Jul-30 08:48 sklearn/Estimator$1.class
--rw-rw-r--  2.0 unx      342 b- defN 23-Jul-30 08:48 sklearn/HasOutlierField.class
--rw-rw-r--  2.0 unx      214 b- defN 23-Jul-30 08:48 sklearn/HasNumberOfFeatures.class
--rw-rw-r--  2.0 unx      660 b- defN 23-Jul-30 08:48 sklearn/MultiTransformer.class
--rw-rw-r--  2.0 unx     2110 b- defN 23-Jul-30 08:48 sklearn/neural_network/MLPRegressor.class
--rw-rw-r--  2.0 unx     2555 b- defN 23-Jul-30 08:48 sklearn/neural_network/MLPClassifier.class
--rw-rw-r--  2.0 unx      759 b- defN 23-Jul-30 08:48 sklearn/neural_network/MultilayerPerceptronUtil$1.class
--rw-rw-r--  2.0 unx     8927 b- defN 23-Jul-30 08:48 sklearn/neural_network/MultilayerPerceptronUtil.class
--rw-rw-r--  2.0 unx     1728 b- defN 23-Jul-30 08:48 sklearn/Step.class
--rw-rw-r--  2.0 unx      168 b- defN 23-Jul-30 08:48 sklearn/HasDefaultValue.class
--rw-rw-r--  2.0 unx     2936 b- defN 23-Jul-30 08:48 sklearn/impute/MissingIndicator.class
--rw-rw-r--  2.0 unx     4027 b- defN 23-Jul-30 08:48 sklearn/impute/ImputerUtil.class
--rw-rw-r--  2.0 unx     5703 b- defN 23-Jul-30 08:48 sklearn/impute/SimpleImputer.class
--rw-rw-r--  2.0 unx     6948 b- defN 23-Jul-30 08:48 sklearn/naive_bayes/GaussianNB.class
--rw-rw-r--  2.0 unx     4446 b- defN 23-Jul-30 08:48 sklearn/linear_model/LinearRegressor.class
--rw-rw-r--  2.0 unx     5037 b- defN 23-Jul-30 08:48 sklearn/linear_model/LinearClassifier.class
--rw-rw-r--  2.0 unx     7645 b- defN 23-Jul-30 08:48 sklearn/linear_model/logistic/LogisticRegression.class
--rw-rw-r--  2.0 unx     1042 b- defN 23-Jul-30 08:48 sklearn/linear_model/ridge/RidgeClassifier.class
--rw-rw-r--  2.0 unx      596 b- defN 23-Jul-30 08:48 sklearn/linear_model/glm/DistributionBoundary.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-Jul-30 08:48 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
--rw-rw-r--  2.0 unx      947 b- defN 23-Jul-30 08:48 sklearn/linear_model/stochastic_gradient/Hinge.class
--rw-rw-r--  2.0 unx     2440 b- defN 23-Jul-30 08:48 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
--rw-rw-r--  2.0 unx      461 b- defN 23-Jul-30 08:48 sklearn/linear_model/stochastic_gradient/LossFunction.class
--rw-rw-r--  2.0 unx      452 b- defN 23-Jul-30 08:48 sklearn/linear_model/stochastic_gradient/Log.class
--rw-rw-r--  2.0 unx     1165 b- defN 23-Jul-30 08:48 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
--rw-rw-r--  2.0 unx      482 b- defN 23-Jul-30 08:48 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
--rw-rw-r--  2.0 unx      968 b- defN 23-Jul-30 08:48 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
--rw-rw-r--  2.0 unx     1720 b- defN 23-Jul-30 08:48 sklearn/compose/ColumnTransformer$1.class
--rw-rw-r--  2.0 unx     3239 b- defN 23-Jul-30 08:48 sklearn/compose/TransformedTargetRegressor.class
--rw-rw-r--  2.0 unx     3649 b- defN 23-Jul-30 08:48 sklearn/compose/ColumnTransformer.class
--rw-rw-r--  2.0 unx     1534 b- defN 23-Jul-30 08:48 sklearn/compose/TransformedTargetRegressor$1.class
--rw-rw-r--  2.0 unx      894 b- defN 23-Jul-30 08:48 sklearn/IdentityTransformer.class
--rw-rw-r--  2.0 unx     4089 b- defN 23-Jul-30 08:48 sklearn/Classifier.class
--rw-rw-r--  2.0 unx     1457 b- defN 23-Jul-30 08:48 sklearn/model_selection/EstimatorSearcher.class
--rw-rw-r--  2.0 unx     1685 b- defN 23-Jul-30 08:48 sklearn/Selector.class
--rw-rw-r--  2.0 unx      419 b- defN 23-Jul-30 08:48 sklearn/decomposition/IncrementalPCA.class
--rw-rw-r--  2.0 unx     3471 b- defN 23-Jul-30 08:48 sklearn/decomposition/TruncatedSVD.class
--rw-rw-r--  2.0 unx     4759 b- defN 23-Jul-30 08:48 sklearn/decomposition/PCA.class
--rw-rw-r--  2.0 unx      911 b- defN 23-Jul-30 08:48 sklearn/decomposition/BasePCA.class
--rw-rw-r--  2.0 unx      336 b- defN 23-Jul-30 08:48 sklearn/HasPredictField.class
--rw-rw-r--  2.0 unx     3018 b- defN 23-Jul-30 08:48 sklearn/neighbors/NearestNeighbors.class
--rw-rw-r--  2.0 unx     4505 b- defN 23-Jul-30 08:48 sklearn/neighbors/KNeighborsClassifier.class
--rw-rw-r--  2.0 unx     3794 b- defN 23-Jul-30 08:48 sklearn/neighbors/NearestCentroid.class
--rw-rw-r--  2.0 unx     2061 b- defN 23-Jul-30 08:48 sklearn/neighbors/BinaryTree.class
--rw-rw-r--  2.0 unx     1266 b- defN 23-Jul-30 08:48 sklearn/neighbors/KNeighborsUtil$1.class
--rw-rw-r--  2.0 unx      181 b- defN 23-Jul-30 08:48 sklearn/neighbors/HasMetric.class
--rw-rw-r--  2.0 unx    10745 b- defN 23-Jul-30 08:48 sklearn/neighbors/KNeighborsUtil.class
--rw-rw-r--  2.0 unx     4387 b- defN 23-Jul-30 08:48 sklearn/neighbors/KNeighborsRegressor.class
--rw-rw-r--  2.0 unx     1068 b- defN 23-Jul-30 08:48 sklearn/neighbors/DistanceMetric.class
--rw-rw-r--  2.0 unx      351 b- defN 23-Jul-30 08:48 sklearn/neighbors/HasTrainingData.class
--rw-rw-r--  2.0 unx      176 b- defN 23-Jul-30 08:48 sklearn/neighbors/HasNumberOfNeighbors.class
--rw-rw-r--  2.0 unx     2666 b- defN 23-Jul-30 08:48 sklearn/multioutput/MultiOutputUtil.class
--rw-rw-r--  2.0 unx     3522 b- defN 23-Jul-30 08:48 sklearn/multioutput/ChainUtil.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-Jul-30 08:48 sklearn/multioutput/RegressorChain.class
--rw-rw-r--  2.0 unx     1316 b- defN 23-Jul-30 08:48 sklearn/multioutput/MultiOutputClassifier.class
--rw-rw-r--  2.0 unx     1310 b- defN 23-Jul-30 08:48 sklearn/multioutput/MultiOutputRegressor.class
--rw-rw-r--  2.0 unx     1745 b- defN 23-Jul-30 08:48 sklearn/multioutput/ClassifierChain.class
--rw-rw-r--  2.0 unx     4450 b- defN 23-Jul-30 08:48 sklearn/isotonic/IsotonicRegression.class
--rw-rw-r--  2.0 unx      326 b- defN 23-Jul-30 08:48 sklearn/HasApplyField.class
--rw-rw-r--  2.0 unx      273 b- defN 23-Jul-30 08:48 sklearn/HasEstimatorEnsemble.class
--rw-rw-r--  2.0 unx     2094 b- defN 23-Jul-30 08:48 sklearn/Transformer$1.class
--rw-rw-r--  2.0 unx      953 b- defN 23-Jul-30 08:48 sklearn/LabelEncoderClassifier.class
--rw-rw-r--  2.0 unx      451 b- defN 23-Jul-30 08:48 sklearn/PassThrough.class
--rw-rw-r--  2.0 unx      181 b- defN 23-Jul-30 08:48 sklearn/HasPriorProbability.class
--rw-rw-r--  2.0 unx     5693 b- defN 23-Jul-30 08:48 sklearn/feature_extraction/text/TfidfVectorizer.class
--rw-rw-r--  2.0 unx      809 b- defN 23-Jul-30 08:48 sklearn/feature_extraction/text/TfidfVectorizer$1.class
--rw-rw-r--  2.0 unx      675 b- defN 23-Jul-30 08:48 sklearn/feature_extraction/text/Tokenizer.class
--rw-rw-r--  2.0 unx    13329 b- defN 23-Jul-30 08:48 sklearn/feature_extraction/text/CountVectorizer.class
--rw-rw-r--  2.0 unx     2129 b- defN 23-Jul-30 08:48 sklearn/feature_extraction/text/CountVectorizer$1.class
--rw-rw-r--  2.0 unx     1433 b- defN 23-Jul-30 08:48 sklearn/feature_extraction/text/TfidfTransformer.class
--rw-rw-r--  2.0 unx     4031 b- defN 23-Jul-30 08:48 sklearn/feature_extraction/DictVectorizer.class
--rw-rw-r--  2.0 unx      762 b- defN 23-Jul-30 08:48 sklearn/Clusterer.class
--rw-rw-r--  2.0 unx     1411 b- defN 23-Jul-30 08:48 sklearn/metrics/DistanceMetric.class
--rw-rw-r--  2.0 unx     1069 b- defN 23-Jul-30 08:48 sklearn/ensemble/EnsembleUtil.class
--rw-rw-r--  2.0 unx     2112 b- defN 23-Jul-30 08:48 sklearn/ensemble/bagging/BaggingRegressor.class
--rw-rw-r--  2.0 unx     3293 b- defN 23-Jul-30 08:48 sklearn/ensemble/bagging/BaggingUtil.class
--rw-rw-r--  2.0 unx     3031 b- defN 23-Jul-30 08:48 sklearn/ensemble/bagging/BaggingClassifier.class
--rw-rw-r--  2.0 unx     1409 b- defN 23-Jul-30 08:48 sklearn/ensemble/EnsembleRegressor.class
--rw-rw-r--  2.0 unx     3485 b- defN 23-Jul-30 08:48 sklearn/ensemble/stacking/StackingClassifier.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Jul-30 08:48 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
--rw-rw-r--  2.0 unx     3109 b- defN 23-Jul-30 08:48 sklearn/ensemble/stacking/StackingRegressor.class
--rw-rw-r--  2.0 unx     3862 b- defN 23-Jul-30 08:48 sklearn/ensemble/stacking/StackingUtil.class
--rw-rw-r--  2.0 unx     2524 b- defN 23-Jul-30 08:48 sklearn/ensemble/stacking/StackingClassifier$1.class
--rw-rw-r--  2.0 unx     2254 b- defN 23-Jul-30 08:48 sklearn/ensemble/stacking/StackingRegressor$1.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
--rw-rw-r--  2.0 unx     2563 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
--rw-rw-r--  2.0 unx      858 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/LossFunction.class
--rw-rw-r--  2.0 unx     1588 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
--rw-rw-r--  2.0 unx     1317 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
--rw-rw-r--  2.0 unx     7945 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
--rw-rw-r--  2.0 unx      960 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/MeanEstimator.class
--rw-rw-r--  2.0 unx     1265 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
--rw-rw-r--  2.0 unx      980 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
--rw-rw-r--  2.0 unx     1578 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
--rw-rw-r--  2.0 unx      811 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
--rw-rw-r--  2.0 unx     3003 b- defN 23-Jul-30 08:48 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
--rw-rw-r--  2.0 unx     1148 b- defN 23-Jul-30 08:48 sklearn/ensemble/EnsembleUtil$1.class
--rw-rw-r--  2.0 unx     3059 b- defN 23-Jul-30 08:48 sklearn/ensemble/forest/ForestUtil.class
--rw-rw-r--  2.0 unx     2528 b- defN 23-Jul-30 08:48 sklearn/ensemble/forest/ForestRegressor.class
--rw-rw-r--  2.0 unx     2987 b- defN 23-Jul-30 08:48 sklearn/ensemble/forest/ForestClassifier.class
--rw-rw-r--  2.0 unx     1752 b- defN 23-Jul-30 08:48 sklearn/ensemble/iforest/IsolationForest$3.class
--rw-rw-r--  2.0 unx     2206 b- defN 23-Jul-30 08:48 sklearn/ensemble/iforest/IsolationForest$1.class
--rw-rw-r--  2.0 unx     1716 b- defN 23-Jul-30 08:48 sklearn/ensemble/iforest/IsolationForest$2.class
--rw-rw-r--  2.0 unx     8225 b- defN 23-Jul-30 08:48 sklearn/ensemble/iforest/IsolationForest.class
--rw-rw-r--  2.0 unx     5055 b- defN 23-Jul-30 08:48 sklearn/ensemble/voting/VotingClassifier.class
--rw-rw-r--  2.0 unx     3716 b- defN 23-Jul-30 08:48 sklearn/ensemble/voting/VotingRegressor.class
--rw-rw-r--  2.0 unx     2814 b- defN 23-Jul-30 08:48 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
--rw-rw-r--  2.0 unx     1247 b- defN 23-Jul-30 08:48 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
--rw-rw-r--  2.0 unx     3041 b- defN 23-Jul-30 08:48 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
--rw-rw-r--  2.0 unx     6152 b- defN 23-Jul-30 08:48 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
--rw-rw-r--  2.0 unx      505 b- defN 23-Jul-30 08:48 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
--rw-rw-r--  2.0 unx      490 b- defN 23-Jul-30 08:48 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
--rw-rw-r--  2.0 unx     1572 b- defN 23-Jul-30 08:48 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
--rw-rw-r--  2.0 unx     6374 b- defN 23-Jul-30 08:48 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     8868 b- defN 23-Jul-30 08:48 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
--rw-rw-r--  2.0 unx      441 b- defN 23-Jul-30 08:48 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jul-30 08:48 sklearn/ensemble/EnsembleClassifier.class
--rw-rw-r--  2.0 unx     3564 b- defN 23-Jul-30 08:48 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
--rw-rw-r--  2.0 unx     6076 b- defN 23-Jul-30 08:48 sklearn/Transformer.class
--rw-rw-r--  2.0 unx      859 b- defN 23-Jul-30 08:48 sklearn/Transformer$1$1.class
--rw-rw-r--  2.0 unx      981 b- defN 23-Jul-30 08:48 sklearn/Drop.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Jul-30 08:48 sklearn/feature_selection/SelectKBest$Entry.class
--rw-rw-r--  2.0 unx     3486 b- defN 23-Jul-30 08:48 sklearn/feature_selection/SelectFromModel.class
--rw-rw-r--  2.0 unx     2922 b- defN 23-Jul-30 08:48 sklearn/feature_selection/SelectKBest.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-Jul-30 08:48 sklearn/feature_selection/PySelector.class
--rw-rw-r--  2.0 unx      607 b- defN 23-Jul-30 08:48 sklearn/Transformer$2.class
--rw-rw-r--  2.0 unx     2216 b- defN 23-Jul-30 08:48 sklearn/SkLearnUtil.class
--rw-rw-r--  2.0 unx      412 b- defN 23-Jul-30 08:48 sklearn/loss/HalfMultinomialLoss.class
--rw-rw-r--  2.0 unx      602 b- defN 23-Jul-30 08:48 sklearn/loss/CyLossFunction.class
--rw-rw-r--  2.0 unx      403 b- defN 23-Jul-30 08:48 sklearn/loss/HalfBinomialLoss.class
--rw-rw-r--  2.0 unx      387 b- defN 23-Jul-30 08:48 sklearn/loss/BaseLoss.class
--rw-rw-r--  2.0 unx      381 b- defN 23-Jul-30 08:48 sklearn/HasDecisionFunctionField.class
--rw-rw-r--  2.0 unx      338 b- defN 23-Jul-30 08:48 sklearn/SkLearnMethods.class
--rw-rw-r--  2.0 unx     1515 b- defN 23-Jul-30 08:48 sklearn/OutlierDetectorUtil$1.class
--rw-rw-r--  2.0 unx      195 b- defN 23-Jul-30 08:48 sklearn/HasClasses.class
--rw-rw-r--  2.0 unx     4682 b- defN 23-Jul-30 08:48 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
--rw-rw-r--  2.0 unx      696 b- defN 23-Jul-30 08:48 sklearn/EstimatorUtil$1.class
--rw-rw-r--  2.0 unx     3311 b- defN 23-Jul-30 08:48 sklearn/Composite.class
--rw-rw-r--  2.0 unx     1194 b- defN 23-Jul-30 08:48 sklearn/preprocessing/KBinsDiscretizer$1.class
--rw-rw-r--  2.0 unx     4567 b- defN 23-Jul-30 08:48 sklearn/preprocessing/PowerTransformer.class
--rw-rw-r--  2.0 unx     2381 b- defN 23-Jul-30 08:48 sklearn/preprocessing/LabelEncoder.class
--rw-rw-r--  2.0 unx     4924 b- defN 23-Jul-30 08:48 sklearn/preprocessing/LabelBinarizer.class
--rw-rw-r--  2.0 unx     1158 b- defN 23-Jul-30 08:48 sklearn/preprocessing/EncoderUtil$3.class
--rw-rw-r--  2.0 unx      389 b- defN 23-Jul-30 08:48 sklearn/preprocessing/Scaler.class
--rw-rw-r--  2.0 unx      797 b- defN 23-Jul-30 08:48 sklearn/preprocessing/MultiOneHotEncoder$1.class
--rw-rw-r--  2.0 unx     3242 b- defN 23-Jul-30 08:48 sklearn/preprocessing/MaxAbsScaler.class
--rw-rw-r--  2.0 unx     2948 b- defN 23-Jul-30 08:48 sklearn/preprocessing/FunctionTransformer.class
--rw-rw-r--  2.0 unx     3291 b- defN 23-Jul-30 08:48 sklearn/preprocessing/BaseEncoder.class
--rw-rw-r--  2.0 unx     1270 b- defN 23-Jul-30 08:48 sklearn/preprocessing/EncoderUtil$1.class
--rw-rw-r--  2.0 unx     4549 b- defN 23-Jul-30 08:48 sklearn/preprocessing/StandardScaler.class
--rw-rw-r--  2.0 unx     9005 b- defN 23-Jul-30 08:48 sklearn/preprocessing/EncoderUtil.class
--rw-rw-r--  2.0 unx     6343 b- defN 23-Jul-30 08:48 sklearn/preprocessing/PolynomialFeatures.class
--rw-rw-r--  2.0 unx     8486 b- defN 23-Jul-30 08:48 sklearn/preprocessing/KBinsDiscretizer.class
--rw-rw-r--  2.0 unx     4671 b- defN 23-Jul-30 08:48 sklearn/preprocessing/OneHotEncoder.class
--rw-rw-r--  2.0 unx      729 b- defN 23-Jul-30 08:48 sklearn/preprocessing/EncoderUtil$4.class
--rw-rw-r--  2.0 unx     2553 b- defN 23-Jul-30 08:48 sklearn/preprocessing/Binarizer.class
--rw-rw-r--  2.0 unx     1054 b- defN 23-Jul-30 08:48 sklearn/preprocessing/EncoderUtil$2.class
--rw-rw-r--  2.0 unx     3595 b- defN 23-Jul-30 08:48 sklearn/preprocessing/MinMaxScaler.class
--rw-rw-r--  2.0 unx     4467 b- defN 23-Jul-30 08:48 sklearn/preprocessing/RobustScaler.class
--rw-rw-r--  2.0 unx     3740 b- defN 23-Jul-30 08:48 sklearn/preprocessing/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      957 b- defN 23-Jul-30 08:48 sklearn/preprocessing/Imputer.class
--rw-rw-r--  2.0 unx     2033 b- defN 23-Jul-30 08:48 sklearn/preprocessing/PolynomialFeatures$1.class
--rw-rw-r--  2.0 unx    10333 b- defN 23-Jul-30 08:48 sklearn/preprocessing/MultiOneHotEncoder.class
--rw-rw-r--  2.0 unx     2153 b- defN 23-Jul-30 08:48 sklearn/tree/TreeClassifier.class
--rw-rw-r--  2.0 unx     3111 b- defN 23-Jul-30 08:48 sklearn/tree/TreeUtil$1.class
--rw-rw-r--  2.0 unx     2664 b- defN 23-Jul-30 08:48 sklearn/tree/TreeUtil$4.class
--rw-rw-r--  2.0 unx     4805 b- defN 23-Jul-30 08:48 sklearn/tree/visitors/TreeModelFlattener.class
--rw-rw-r--  2.0 unx      739 b- defN 23-Jul-30 08:48 sklearn/tree/visitors/TreeModelCompactor$1.class
--rw-rw-r--  2.0 unx     5431 b- defN 23-Jul-30 08:48 sklearn/tree/visitors/TreeModelCompactor.class
--rw-rw-r--  2.0 unx     2988 b- defN 23-Jul-30 08:48 sklearn/tree/visitors/TreeModelPruner.class
--rw-rw-r--  2.0 unx      739 b- defN 23-Jul-30 08:48 sklearn/tree/visitors/TreeModelFlattener$1.class
--rw-rw-r--  2.0 unx      730 b- defN 23-Jul-30 08:48 sklearn/tree/visitors/TreeModelPruner$1.class
--rw-rw-r--  2.0 unx      915 b- defN 23-Jul-30 08:48 sklearn/tree/RegressionCriterion.class
--rw-rw-r--  2.0 unx     1151 b- defN 23-Jul-30 08:48 sklearn/tree/TreeUtil$5.class
--rw-rw-r--  2.0 unx     1014 b- defN 23-Jul-30 08:48 sklearn/tree/PresortBestSplitter.class
--rw-rw-r--  2.0 unx     1589 b- defN 23-Jul-30 08:48 sklearn/tree/TreeUtil$6.class
--rw-rw-r--  2.0 unx     1764 b- defN 23-Jul-30 08:48 sklearn/tree/TreeRegressor.class
--rw-rw-r--  2.0 unx     1489 b- defN 23-Jul-30 08:48 sklearn/tree/TreeUtil$7.class
--rw-rw-r--  2.0 unx    19425 b- defN 23-Jul-30 08:48 sklearn/tree/TreeUtil.class
--rw-rw-r--  2.0 unx     1123 b- defN 23-Jul-30 08:48 sklearn/tree/TreeUtil$3.class
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jul-30 08:48 sklearn/tree/HasTreeOptions.class
--rw-rw-r--  2.0 unx     2293 b- defN 23-Jul-30 08:48 sklearn/tree/Tree.class
--rw-rw-r--  2.0 unx      754 b- defN 23-Jul-30 08:48 sklearn/tree/TreeUtil$2.class
--rw-rw-r--  2.0 unx      150 b- defN 23-Jul-30 08:48 sklearn/tree/HasTree.class
--rw-rw-r--  2.0 unx     1967 b- defN 23-Jul-30 08:48 sklearn/InitializerUtil.class
--rw-rw-r--  2.0 unx      570 b- defN 23-Jul-30 08:48 sklearn/Regressor.class
--rw-rw-r--  2.0 unx      211 b- defN 23-Jul-30 08:48 sklearn/HasNumberOfOutputs.class
--rw-rw-r--  2.0 unx      534 b- defN 23-Jul-30 08:48 sklearn/OutlierDetector.class
--rw-rw-r--  2.0 unx     2808 b- defN 23-Jul-30 08:48 sklearn/Calibrator.class
--rw-rw-r--  2.0 unx      273 b- defN 23-Jul-30 08:48 sklearn/HasClassifierOptions.class
--rw-rw-r--  2.0 unx     7080 b- defN 23-Jul-30 08:48 sklearn/EstimatorUtil.class
--rw-rw-r--  2.0 unx      199 b- defN 23-Jul-30 08:48 sklearn/HasType.class
--rw-rw-r--  2.0 unx      678 b- defN 23-Jul-30 08:48 sklearn/cluster/MiniBatchKMeans.class
--rw-rw-r--  2.0 unx     5086 b- defN 23-Jul-30 08:48 sklearn/cluster/KMeans.class
--rw-rw-r--  2.0 unx    13887 b- defN 23-Jul-30 08:48 sklearn/Estimator.class
--rw-rw-r--  2.0 unx     1624 b- defN 23-Jul-30 08:48 sklearn/Initializer.class
--rw-rw-r--  2.0 unx     4595 b- defN 23-Jul-30 08:48 sklearn/multiclass/OneVsRestClassifier.class
--rw-rw-r--  2.0 unx     5157 b- defN 23-Jul-30 08:48 sklearn2pmml/ruleset/RuleSetClassifier.class
--rw-rw-r--  2.0 unx      980 b- defN 23-Jul-30 08:48 sklearn2pmml/pipeline/PMMLPipeline$3.class
--rw-rw-r--  2.0 unx     1023 b- defN 23-Jul-30 08:48 sklearn2pmml/pipeline/PMMLPipeline$4.class
--rw-rw-r--  2.0 unx    27064 b- defN 23-Jul-30 08:48 sklearn2pmml/pipeline/PMMLPipeline.class
--rw-rw-r--  2.0 unx     1421 b- defN 23-Jul-30 08:48 sklearn2pmml/pipeline/PMMLPipeline$2.class
--rw-rw-r--  2.0 unx     1346 b- defN 23-Jul-30 08:48 sklearn2pmml/pipeline/PMMLPipeline$1.class
--rw-rw-r--  2.0 unx     1811 b- defN 23-Jul-30 08:48 sklearn2pmml/pipeline/Verification.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/MultiDomain.class
--rw-rw-r--  2.0 unx     1152 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/ContinuousDomainEraser.class
--rw-rw-r--  2.0 unx     1654 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/Alias.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/TemporalDomain.class
--rw-rw-r--  2.0 unx      779 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/ContinuousDomain$1.class
--rw-rw-r--  2.0 unx    11878 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/Domain.class
--rw-rw-r--  2.0 unx     1416 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/MultiAlias.class
--rw-rw-r--  2.0 unx     5055 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/DiscreteDomain.class
--rw-rw-r--  2.0 unx     1952 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/CategoricalDomain.class
--rw-rw-r--  2.0 unx     1453 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/DomainEraser.class
--rw-rw-r--  2.0 unx      613 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/DateTimeDomain.class
--rw-rw-r--  2.0 unx     7764 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/ContinuousDomain.class
--rw-rw-r--  2.0 unx     1077 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/DiscreteDomainEraser.class
--rw-rw-r--  2.0 unx     1590 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/TransformerWrapper.class
--rw-rw-r--  2.0 unx     1045 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/Domain$2.class
--rw-rw-r--  2.0 unx      596 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/DateDomain.class
--rw-rw-r--  2.0 unx     2374 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/DomainUtil.class
--rw-rw-r--  2.0 unx     1033 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/Domain$1.class
--rw-rw-r--  2.0 unx     1577 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/OrdinalDomain.class
--rw-rw-r--  2.0 unx      672 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/Domain$4.class
--rw-rw-r--  2.0 unx      799 b- defN 23-Jul-30 08:48 sklearn2pmml/decoration/Domain$3.class
--rw-rw-r--  2.0 unx     7879 b- defN 23-Jul-30 08:48 sklearn2pmml/neural_network/MLPTransformer.class
--rw-rw-r--  2.0 unx      391 b- defN 23-Jul-30 08:48 sklearn2pmml/SkLearn2PMMLFields.class
--rw-rw-r--  2.0 unx     1160 b- defN 23-Jul-30 08:48 sklearn2pmml/util/Evaluatable.class
--rw-rw-r--  2.0 unx     1196 b- defN 23-Jul-30 08:48 sklearn2pmml/util/Expression.class
--rw-rw-r--  2.0 unx     1189 b- defN 23-Jul-30 08:48 sklearn2pmml/util/Predicate.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Jul-30 08:48 sklearn2pmml/util/Reshaper.class
--rw-rw-r--  2.0 unx     3392 b- defN 23-Jul-30 08:48 sklearn2pmml/util/EvaluatableUtil.class
--rw-rw-r--  2.0 unx     1658 b- defN 23-Jul-30 08:48 sklearn2pmml/util/Slicer.class
--rw-rw-r--  2.0 unx     2418 b- defN 23-Jul-30 08:48 sklearn2pmml/feature_extraction/text/Splitter.class
--rw-rw-r--  2.0 unx     3184 b- defN 23-Jul-30 08:48 sklearn2pmml/feature_extraction/text/Matcher.class
--rw-rw-r--  2.0 unx     1262 b- defN 23-Jul-30 08:48 sklearn2pmml/ensemble/SelectFirstRegressor.class
--rw-rw-r--  2.0 unx     2083 b- defN 23-Jul-30 08:48 sklearn2pmml/ensemble/GBDTUtil$2.class
--rw-rw-r--  2.0 unx     1934 b- defN 23-Jul-30 08:48 sklearn2pmml/ensemble/GBDTLMRegressor.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Jul-30 08:48 sklearn2pmml/ensemble/GBDTUtil$1.class
--rw-rw-r--  2.0 unx     7410 b- defN 23-Jul-30 08:48 sklearn2pmml/ensemble/EstimatorChain.class
--rw-rw-r--  2.0 unx     6582 b- defN 23-Jul-30 08:48 sklearn2pmml/ensemble/GBDTUtil.class
--rw-rw-r--  2.0 unx     3995 b- defN 23-Jul-30 08:48 sklearn2pmml/ensemble/Link.class
--rw-rw-r--  2.0 unx     4360 b- defN 23-Jul-30 08:48 sklearn2pmml/ensemble/SelectFirstUtil.class
--rw-rw-r--  2.0 unx     4249 b- defN 23-Jul-30 08:48 sklearn2pmml/ensemble/GBDTLRClassifier.class
--rw-rw-r--  2.0 unx     2608 b- defN 23-Jul-30 08:48 sklearn2pmml/ensemble/SelectFirstClassifier.class
--rw-rw-r--  2.0 unx     1438 b- defN 23-Jul-30 08:48 sklearn2pmml/EstimatorProxy$1.class
--rw-rw-r--  2.0 unx      946 b- defN 23-Jul-30 08:48 sklearn2pmml/feature_selection/SelectUnique.class
--rw-rw-r--  2.0 unx     6477 b- defN 23-Jul-30 08:48 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
--rw-rw-r--  2.0 unx      791 b- defN 23-Jul-30 08:48 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
--rw-rw-r--  2.0 unx     1197 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/PatternTransformer.class
--rw-rw-r--  2.0 unx     2908 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/ReplaceTransformer.class
--rw-rw-r--  2.0 unx     1844 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/WordCountTransformer.class
--rw-rw-r--  2.0 unx      597 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/DateTimeFormatter.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
--rw-rw-r--  2.0 unx     4621 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/DurationTransformer.class
--rw-rw-r--  2.0 unx      444 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
--rw-rw-r--  2.0 unx     2777 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/FilterLookupTransformer.class
--rw-rw-r--  2.0 unx     2545 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/Formatter.class
--rw-rw-r--  2.0 unx     3424 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/CastTransformer.class
--rw-rw-r--  2.0 unx     2758 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/MatchesTransformer.class
--rw-rw-r--  2.0 unx      589 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/NumberFormatter.class
--rw-rw-r--  2.0 unx     4149 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/MultiLookupTransformer.class
--rw-rw-r--  2.0 unx     3871 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/StringNormalizer.class
--rw-rw-r--  2.0 unx     7145 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/ExpressionTransformer.class
--rw-rw-r--  2.0 unx      635 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
--rw-rw-r--  2.0 unx     3604 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/DataFrameConstructor.class
--rw-rw-r--  2.0 unx     2847 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/ConcatTransformer.class
--rw-rw-r--  2.0 unx     5993 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/CutTransformer.class
--rw-rw-r--  2.0 unx     7025 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/BSplineTransformer.class
--rw-rw-r--  2.0 unx     6410 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/LookupTransformer.class
--rw-rw-r--  2.0 unx     3236 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/SubstringTransformer.class
--rw-rw-r--  2.0 unx     3181 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
--rw-rw-r--  2.0 unx     2132 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
--rw-rw-r--  2.0 unx     3328 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/Aggregator.class
--rw-rw-r--  2.0 unx      647 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
--rw-rw-r--  2.0 unx     1639 b- defN 23-Jul-30 08:48 sklearn2pmml/tree/CHAIDRegressor.class
--rw-rw-r--  2.0 unx    10719 b- defN 23-Jul-30 08:48 sklearn2pmml/tree/CHAIDUtil.class
--rw-rw-r--  2.0 unx     2032 b- defN 23-Jul-30 08:48 sklearn2pmml/tree/CHAIDClassifier.class
--rw-rw-r--  2.0 unx     1417 b- defN 23-Jul-30 08:48 sklearn2pmml/tree/CHAIDUtil$1.class
--rw-rw-r--  2.0 unx     3864 b- defN 23-Jul-30 08:48 sklearn2pmml/EstimatorProxy.class
--rw-rw-r--  2.0 unx     1458 b- defN 23-Jul-30 08:48 sklearn2pmml/SelectorProxy.class
--rw-rw-r--  2.0 unx     2046 b- defN 23-Jul-30 08:48 sklearn2pmml/expression/ExpressionUtil.class
--rw-rw-r--  2.0 unx     3799 b- defN 23-Jul-30 08:48 sklearn2pmml/expression/ExpressionRegressor.class
--rw-rw-r--  2.0 unx      990 b- defN 23-Jul-30 08:48 sklearn2pmml/expression/ExpressionClassifier$1.class
--rw-rw-r--  2.0 unx     8687 b- defN 23-Jul-30 08:48 sklearn2pmml/expression/ExpressionClassifier.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Jul-30 08:48 sklearn2pmml/expression/ExpressionUtil$1.class
--rw-rw-r--  2.0 unx     1774 b- defN 23-Jul-30 08:48 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
--rw-rw-r--  2.0 unx     2764 b- defN 23-Jul-30 08:48 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
--rw-rw-r--  2.0 unx     3549 b- defN 23-Jul-30 08:48 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
--rw-rw-r--  2.0 unx    16114 b- defN 23-Jul-30 08:48 org/jpmml/sklearn/SkLearnEncoder.class
--rw-rw-r--  2.0 unx      194 b- defN 23-Jul-30 08:48 org/jpmml/sklearn/FieldNames.class
--rw-rw-r--  2.0 unx      171 b- defN 23-Jul-30 08:48 org/jpmml/sklearn/HasSkLearnOptions.class
--rw-rw-r--  2.0 unx     1179 b- defN 23-Jul-30 08:48 org/jpmml/sklearn/SkLearnEncoder$1.class
--rw-rw-r--  2.0 unx     1822 b- defN 23-Jul-30 08:47 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
--rw-rw-r--  2.0 unx       57 b- defN 23-Jul-30 08:48 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
-404 files, 925614 bytes uncompressed, 408091 bytes compressed:  55.9%
+Zip file size: 474695 bytes, number of entries: 410
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/
+-rw-r--r--  2.0 unx      159 b- defN 23-Aug-03 15:40 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn_pandas/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 chaid/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 stop_words/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/calibration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/dummy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/svm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/impute/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/naive_bayes/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/linear_model/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/linear_model/logistic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/linear_model/ridge/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/linear_model/glm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/compose/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/model_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/decomposition/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/neighbors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/multioutput/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/isotonic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/metrics/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/bagging/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/stacking/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/forest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/iforest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/voting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/weight_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/loss/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/discriminant_analysis/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/tree/visitors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/cluster/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/multiclass/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/ruleset/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/decoration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/util/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/postprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/expression/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 org/jpmml/sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 org/jpmml/sklearn/testing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn/
+-rw-rw-r--  2.0 unx    16829 b- defN 23-Aug-03 15:40 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     2287 b- defN 23-Aug-03 15:40 sklearn_pandas/CategoricalImputer.class
+-rw-rw-r--  2.0 unx      656 b- defN 23-Aug-03 15:40 sklearn_pandas/TransformerPipeline.class
+-rw-rw-r--  2.0 unx     1154 b- defN 23-Aug-03 15:40 sklearn_pandas/DataFrameMapper$2.class
+-rw-rw-r--  2.0 unx     6280 b- defN 23-Aug-03 15:40 sklearn_pandas/DataFrameMapper.class
+-rw-rw-r--  2.0 unx     1126 b- defN 23-Aug-03 15:40 sklearn_pandas/DataFrameMapper$1.class
+-rw-rw-r--  2.0 unx      609 b- defN 23-Aug-03 15:40 chaid/ContinuousColumn.class
+-rw-rw-r--  2.0 unx      925 b- defN 23-Aug-03 15:40 chaid/Node.class
+-rw-rw-r--  2.0 unx      467 b- defN 23-Aug-03 15:40 chaid/Column.class
+-rw-rw-r--  2.0 unx     3283 b- defN 23-Aug-03 15:40 chaid/Split.class
+-rw-rw-r--  2.0 unx      401 b- defN 23-Aug-03 15:40 chaid/InvalidSplitReason.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-Aug-03 15:40 chaid/NominalColumn.class
+-rw-rw-r--  2.0 unx     1912 b- defN 23-Aug-03 15:40 stop_words/english.txt
+-rw-rw-r--  2.0 unx      147 b- defN 23-Aug-03 15:40 sklearn/HasHead.class
+-rw-rw-r--  2.0 unx     1728 b- defN 23-Aug-03 15:40 sklearn/StepUtil.class
+-rw-rw-r--  2.0 unx    12045 b- defN 23-Aug-03 15:40 sklearn/calibration/CalibratedClassifier.class
+-rw-rw-r--  2.0 unx     2953 b- defN 23-Aug-03 15:40 sklearn/calibration/SigmoidCalibration.class
+-rw-rw-r--  2.0 unx      683 b- defN 23-Aug-03 15:40 sklearn/calibration/CalibratedClassifier$1.class
+-rw-rw-r--  2.0 unx     3672 b- defN 23-Aug-03 15:40 sklearn/calibration/CalibratedClassifierCV.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-Aug-03 15:40 sklearn/pipeline/PipelineTransformer.class
+-rw-rw-r--  2.0 unx     1697 b- defN 23-Aug-03 15:40 sklearn/pipeline/Pipeline$2.class
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Aug-03 15:40 sklearn/pipeline/FeatureUnion.class
+-rw-rw-r--  2.0 unx     5599 b- defN 23-Aug-03 15:40 sklearn/pipeline/Pipeline.class
+-rw-rw-r--  2.0 unx     2327 b- defN 23-Aug-03 15:40 sklearn/pipeline/PipelineRegressor.class
+-rw-rw-r--  2.0 unx     1742 b- defN 23-Aug-03 15:40 sklearn/pipeline/Pipeline$1.class
+-rw-rw-r--  2.0 unx     1111 b- defN 23-Aug-03 15:40 sklearn/pipeline/PipelineUtil.class
+-rw-rw-r--  2.0 unx     2589 b- defN 23-Aug-03 15:40 sklearn/pipeline/PipelineClassifier.class
+-rw-rw-r--  2.0 unx     2435 b- defN 23-Aug-03 15:40 sklearn/pipeline/PipelineClusterer.class
+-rw-rw-r--  2.0 unx     5027 b- defN 23-Aug-03 15:40 sklearn/dummy/DummyClassifier.class
+-rw-rw-r--  2.0 unx     2174 b- defN 23-Aug-03 15:40 sklearn/dummy/DummyRegressor.class
+-rw-rw-r--  2.0 unx      512 b- defN 23-Aug-03 15:40 sklearn/SkLearnFields.class
+-rw-rw-r--  2.0 unx     2293 b- defN 23-Aug-03 15:40 sklearn/SkLearnOutlierTransformation.class
+-rw-rw-r--  2.0 unx      240 b- defN 23-Aug-03 15:40 sklearn/HasEstimator.class
+-rw-rw-r--  2.0 unx     3421 b- defN 23-Aug-03 15:40 sklearn/OutlierDetectorUtil.class
+-rw-rw-r--  2.0 unx     1236 b- defN 23-Aug-03 15:40 sklearn/HasMultiApplyField.class
+-rw-rw-r--  2.0 unx     2393 b- defN 23-Aug-03 15:40 sklearn/svm/SupportVectorMachineUtil.class
+-rw-rw-r--  2.0 unx     1109 b- defN 23-Aug-03 15:40 sklearn/svm/LinearSVC.class
+-rw-rw-r--  2.0 unx     5037 b- defN 23-Aug-03 15:40 sklearn/svm/LibSVMClassifier.class
+-rw-rw-r--  2.0 unx      966 b- defN 23-Aug-03 15:40 sklearn/svm/SupportVectorMachineUtil$1.class
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Aug-03 15:40 sklearn/svm/OneClassSVM.class
+-rw-rw-r--  2.0 unx     3594 b- defN 23-Aug-03 15:40 sklearn/svm/LibSVMRegressor.class
+-rw-rw-r--  2.0 unx     3007 b- defN 23-Aug-03 15:40 sklearn/InitializerUtil$1.class
+-rw-rw-r--  2.0 unx      735 b- defN 23-Aug-03 15:40 sklearn/Estimator$1.class
+-rw-rw-r--  2.0 unx      342 b- defN 23-Aug-03 15:40 sklearn/HasOutlierField.class
+-rw-rw-r--  2.0 unx      214 b- defN 23-Aug-03 15:40 sklearn/HasNumberOfFeatures.class
+-rw-rw-r--  2.0 unx      660 b- defN 23-Aug-03 15:40 sklearn/MultiTransformer.class
+-rw-rw-r--  2.0 unx     2110 b- defN 23-Aug-03 15:40 sklearn/neural_network/MLPRegressor.class
+-rw-rw-r--  2.0 unx     2555 b- defN 23-Aug-03 15:40 sklearn/neural_network/MLPClassifier.class
+-rw-rw-r--  2.0 unx      759 b- defN 23-Aug-03 15:40 sklearn/neural_network/MultilayerPerceptronUtil$1.class
+-rw-rw-r--  2.0 unx     8927 b- defN 23-Aug-03 15:40 sklearn/neural_network/MultilayerPerceptronUtil.class
+-rw-rw-r--  2.0 unx     1761 b- defN 23-Aug-03 15:40 sklearn/Step.class
+-rw-rw-r--  2.0 unx      168 b- defN 23-Aug-03 15:40 sklearn/HasDefaultValue.class
+-rw-rw-r--  2.0 unx       99 b- defN 23-Aug-03 15:40 sklearn/Proxy.class
+-rw-rw-r--  2.0 unx     2936 b- defN 23-Aug-03 15:40 sklearn/impute/MissingIndicator.class
+-rw-rw-r--  2.0 unx     4027 b- defN 23-Aug-03 15:40 sklearn/impute/ImputerUtil.class
+-rw-rw-r--  2.0 unx     5703 b- defN 23-Aug-03 15:40 sklearn/impute/SimpleImputer.class
+-rw-rw-r--  2.0 unx     6948 b- defN 23-Aug-03 15:40 sklearn/naive_bayes/GaussianNB.class
+-rw-rw-r--  2.0 unx      233 b- defN 23-Aug-03 15:40 sklearn/HasFeatureNamesIn.class
+-rw-rw-r--  2.0 unx     4446 b- defN 23-Aug-03 15:40 sklearn/linear_model/LinearRegressor.class
+-rw-rw-r--  2.0 unx     5037 b- defN 23-Aug-03 15:40 sklearn/linear_model/LinearClassifier.class
+-rw-rw-r--  2.0 unx     7645 b- defN 23-Aug-03 15:40 sklearn/linear_model/logistic/LogisticRegression.class
+-rw-rw-r--  2.0 unx     1042 b- defN 23-Aug-03 15:40 sklearn/linear_model/ridge/RidgeClassifier.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-Aug-03 15:40 sklearn/linear_model/glm/DistributionBoundary.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-Aug-03 15:40 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
+-rw-rw-r--  2.0 unx      947 b- defN 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/Hinge.class
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
+-rw-rw-r--  2.0 unx      461 b- defN 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/LossFunction.class
+-rw-rw-r--  2.0 unx      452 b- defN 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/Log.class
+-rw-rw-r--  2.0 unx     1165 b- defN 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
+-rw-rw-r--  2.0 unx      482 b- defN 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
+-rw-rw-r--  2.0 unx      968 b- defN 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
+-rw-rw-r--  2.0 unx     1746 b- defN 23-Aug-03 15:40 sklearn/compose/ColumnTransformer$1.class
+-rw-rw-r--  2.0 unx     3239 b- defN 23-Aug-03 15:40 sklearn/compose/TransformedTargetRegressor.class
+-rw-rw-r--  2.0 unx     3649 b- defN 23-Aug-03 15:40 sklearn/compose/ColumnTransformer.class
+-rw-rw-r--  2.0 unx     1534 b- defN 23-Aug-03 15:40 sklearn/compose/TransformedTargetRegressor$1.class
+-rw-rw-r--  2.0 unx      894 b- defN 23-Aug-03 15:40 sklearn/IdentityTransformer.class
+-rw-rw-r--  2.0 unx     4089 b- defN 23-Aug-03 15:40 sklearn/Classifier.class
+-rw-rw-r--  2.0 unx     1457 b- defN 23-Aug-03 15:40 sklearn/model_selection/EstimatorSearcher.class
+-rw-rw-r--  2.0 unx     1685 b- defN 23-Aug-03 15:40 sklearn/Selector.class
+-rw-rw-r--  2.0 unx      419 b- defN 23-Aug-03 15:40 sklearn/decomposition/IncrementalPCA.class
+-rw-rw-r--  2.0 unx     3471 b- defN 23-Aug-03 15:40 sklearn/decomposition/TruncatedSVD.class
+-rw-rw-r--  2.0 unx     4759 b- defN 23-Aug-03 15:40 sklearn/decomposition/PCA.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-Aug-03 15:40 sklearn/decomposition/BasePCA.class
+-rw-rw-r--  2.0 unx      336 b- defN 23-Aug-03 15:40 sklearn/HasPredictField.class
+-rw-rw-r--  2.0 unx     3018 b- defN 23-Aug-03 15:40 sklearn/neighbors/NearestNeighbors.class
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Aug-03 15:40 sklearn/neighbors/KNeighborsClassifier.class
+-rw-rw-r--  2.0 unx     3794 b- defN 23-Aug-03 15:40 sklearn/neighbors/NearestCentroid.class
+-rw-rw-r--  2.0 unx     2061 b- defN 23-Aug-03 15:40 sklearn/neighbors/BinaryTree.class
+-rw-rw-r--  2.0 unx     1266 b- defN 23-Aug-03 15:40 sklearn/neighbors/KNeighborsUtil$1.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-Aug-03 15:40 sklearn/neighbors/HasMetric.class
+-rw-rw-r--  2.0 unx    10745 b- defN 23-Aug-03 15:40 sklearn/neighbors/KNeighborsUtil.class
+-rw-rw-r--  2.0 unx     4387 b- defN 23-Aug-03 15:40 sklearn/neighbors/KNeighborsRegressor.class
+-rw-rw-r--  2.0 unx     1068 b- defN 23-Aug-03 15:40 sklearn/neighbors/DistanceMetric.class
+-rw-rw-r--  2.0 unx      351 b- defN 23-Aug-03 15:40 sklearn/neighbors/HasTrainingData.class
+-rw-rw-r--  2.0 unx      176 b- defN 23-Aug-03 15:40 sklearn/neighbors/HasNumberOfNeighbors.class
+-rw-rw-r--  2.0 unx     2666 b- defN 23-Aug-03 15:40 sklearn/multioutput/MultiOutputUtil.class
+-rw-rw-r--  2.0 unx     3522 b- defN 23-Aug-03 15:40 sklearn/multioutput/ChainUtil.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-Aug-03 15:40 sklearn/multioutput/RegressorChain.class
+-rw-rw-r--  2.0 unx     1316 b- defN 23-Aug-03 15:40 sklearn/multioutput/MultiOutputClassifier.class
+-rw-rw-r--  2.0 unx     1310 b- defN 23-Aug-03 15:40 sklearn/multioutput/MultiOutputRegressor.class
+-rw-rw-r--  2.0 unx     1745 b- defN 23-Aug-03 15:40 sklearn/multioutput/ClassifierChain.class
+-rw-rw-r--  2.0 unx     4450 b- defN 23-Aug-03 15:40 sklearn/isotonic/IsotonicRegression.class
+-rw-rw-r--  2.0 unx      326 b- defN 23-Aug-03 15:40 sklearn/HasApplyField.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-Aug-03 15:40 sklearn/HasEstimatorEnsemble.class
+-rw-rw-r--  2.0 unx     2094 b- defN 23-Aug-03 15:40 sklearn/Transformer$1.class
+-rw-rw-r--  2.0 unx      953 b- defN 23-Aug-03 15:40 sklearn/LabelEncoderClassifier.class
+-rw-rw-r--  2.0 unx      451 b- defN 23-Aug-03 15:40 sklearn/PassThrough.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-Aug-03 15:40 sklearn/HasPriorProbability.class
+-rw-rw-r--  2.0 unx      230 b- defN 23-Aug-03 15:40 sklearn/SkLearnSteps.class
+-rw-rw-r--  2.0 unx     5693 b- defN 23-Aug-03 15:40 sklearn/feature_extraction/text/TfidfVectorizer.class
+-rw-rw-r--  2.0 unx      809 b- defN 23-Aug-03 15:40 sklearn/feature_extraction/text/TfidfVectorizer$1.class
+-rw-rw-r--  2.0 unx      675 b- defN 23-Aug-03 15:40 sklearn/feature_extraction/text/Tokenizer.class
+-rw-rw-r--  2.0 unx    13329 b- defN 23-Aug-03 15:40 sklearn/feature_extraction/text/CountVectorizer.class
+-rw-rw-r--  2.0 unx     2129 b- defN 23-Aug-03 15:40 sklearn/feature_extraction/text/CountVectorizer$1.class
+-rw-rw-r--  2.0 unx     1433 b- defN 23-Aug-03 15:40 sklearn/feature_extraction/text/TfidfTransformer.class
+-rw-rw-r--  2.0 unx     4030 b- defN 23-Aug-03 15:40 sklearn/feature_extraction/DictVectorizer.class
+-rw-rw-r--  2.0 unx      762 b- defN 23-Aug-03 15:40 sklearn/Clusterer.class
+-rw-rw-r--  2.0 unx     1411 b- defN 23-Aug-03 15:40 sklearn/metrics/DistanceMetric.class
+-rw-rw-r--  2.0 unx     1069 b- defN 23-Aug-03 15:40 sklearn/ensemble/EnsembleUtil.class
+-rw-rw-r--  2.0 unx     2112 b- defN 23-Aug-03 15:40 sklearn/ensemble/bagging/BaggingRegressor.class
+-rw-rw-r--  2.0 unx     3293 b- defN 23-Aug-03 15:40 sklearn/ensemble/bagging/BaggingUtil.class
+-rw-rw-r--  2.0 unx     3031 b- defN 23-Aug-03 15:40 sklearn/ensemble/bagging/BaggingClassifier.class
+-rw-rw-r--  2.0 unx     1409 b- defN 23-Aug-03 15:40 sklearn/ensemble/EnsembleRegressor.class
+-rw-rw-r--  2.0 unx     3485 b- defN 23-Aug-03 15:40 sklearn/ensemble/stacking/StackingClassifier.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Aug-03 15:40 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
+-rw-rw-r--  2.0 unx     3109 b- defN 23-Aug-03 15:40 sklearn/ensemble/stacking/StackingRegressor.class
+-rw-rw-r--  2.0 unx     3862 b- defN 23-Aug-03 15:40 sklearn/ensemble/stacking/StackingUtil.class
+-rw-rw-r--  2.0 unx     2524 b- defN 23-Aug-03 15:40 sklearn/ensemble/stacking/StackingClassifier$1.class
+-rw-rw-r--  2.0 unx     2254 b- defN 23-Aug-03 15:40 sklearn/ensemble/stacking/StackingRegressor$1.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
+-rw-rw-r--  2.0 unx     2563 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx      858 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/LossFunction.class
+-rw-rw-r--  2.0 unx     1588 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
+-rw-rw-r--  2.0 unx     1317 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
+-rw-rw-r--  2.0 unx     7945 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
+-rw-rw-r--  2.0 unx      960 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/MeanEstimator.class
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
+-rw-rw-r--  2.0 unx     1578 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
+-rw-rw-r--  2.0 unx      811 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
+-rw-rw-r--  2.0 unx     3003 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
+-rw-rw-r--  2.0 unx     1148 b- defN 23-Aug-03 15:40 sklearn/ensemble/EnsembleUtil$1.class
+-rw-rw-r--  2.0 unx     3059 b- defN 23-Aug-03 15:40 sklearn/ensemble/forest/ForestUtil.class
+-rw-rw-r--  2.0 unx     2528 b- defN 23-Aug-03 15:40 sklearn/ensemble/forest/ForestRegressor.class
+-rw-rw-r--  2.0 unx     2987 b- defN 23-Aug-03 15:40 sklearn/ensemble/forest/ForestClassifier.class
+-rw-rw-r--  2.0 unx     1752 b- defN 23-Aug-03 15:40 sklearn/ensemble/iforest/IsolationForest$3.class
+-rw-rw-r--  2.0 unx     2206 b- defN 23-Aug-03 15:40 sklearn/ensemble/iforest/IsolationForest$1.class
+-rw-rw-r--  2.0 unx     1716 b- defN 23-Aug-03 15:40 sklearn/ensemble/iforest/IsolationForest$2.class
+-rw-rw-r--  2.0 unx     8225 b- defN 23-Aug-03 15:40 sklearn/ensemble/iforest/IsolationForest.class
+-rw-rw-r--  2.0 unx     5055 b- defN 23-Aug-03 15:40 sklearn/ensemble/voting/VotingClassifier.class
+-rw-rw-r--  2.0 unx     3716 b- defN 23-Aug-03 15:40 sklearn/ensemble/voting/VotingRegressor.class
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx     1247 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
+-rw-rw-r--  2.0 unx     3041 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
+-rw-rw-r--  2.0 unx     6152 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
+-rw-rw-r--  2.0 unx      505 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
+-rw-rw-r--  2.0 unx      490 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
+-rw-rw-r--  2.0 unx     1572 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
+-rw-rw-r--  2.0 unx     6374 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     8868 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
+-rw-rw-r--  2.0 unx      441 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Aug-03 15:40 sklearn/ensemble/EnsembleClassifier.class
+-rw-rw-r--  2.0 unx     3564 b- defN 23-Aug-03 15:40 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
+-rw-rw-r--  2.0 unx     6362 b- defN 23-Aug-03 15:40 sklearn/Transformer.class
+-rw-rw-r--  2.0 unx      859 b- defN 23-Aug-03 15:40 sklearn/Transformer$1$1.class
+-rw-rw-r--  2.0 unx      981 b- defN 23-Aug-03 15:40 sklearn/Drop.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Aug-03 15:40 sklearn/feature_selection/SelectKBest$Entry.class
+-rw-rw-r--  2.0 unx     3486 b- defN 23-Aug-03 15:40 sklearn/feature_selection/SelectFromModel.class
+-rw-rw-r--  2.0 unx     2922 b- defN 23-Aug-03 15:40 sklearn/feature_selection/SelectKBest.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-Aug-03 15:40 sklearn/feature_selection/PySelector.class
+-rw-rw-r--  2.0 unx      607 b- defN 23-Aug-03 15:40 sklearn/Transformer$2.class
+-rw-rw-r--  2.0 unx     2216 b- defN 23-Aug-03 15:40 sklearn/SkLearnUtil.class
+-rw-rw-r--  2.0 unx      412 b- defN 23-Aug-03 15:40 sklearn/loss/HalfMultinomialLoss.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-Aug-03 15:40 sklearn/loss/CyLossFunction.class
+-rw-rw-r--  2.0 unx      403 b- defN 23-Aug-03 15:40 sklearn/loss/HalfBinomialLoss.class
+-rw-rw-r--  2.0 unx      387 b- defN 23-Aug-03 15:40 sklearn/loss/BaseLoss.class
+-rw-rw-r--  2.0 unx      381 b- defN 23-Aug-03 15:40 sklearn/HasDecisionFunctionField.class
+-rw-rw-r--  2.0 unx      338 b- defN 23-Aug-03 15:40 sklearn/SkLearnMethods.class
+-rw-rw-r--  2.0 unx     1515 b- defN 23-Aug-03 15:40 sklearn/OutlierDetectorUtil$1.class
+-rw-rw-r--  2.0 unx      195 b- defN 23-Aug-03 15:40 sklearn/HasClasses.class
+-rw-rw-r--  2.0 unx     4682 b- defN 23-Aug-03 15:40 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
+-rw-rw-r--  2.0 unx      696 b- defN 23-Aug-03 15:40 sklearn/EstimatorUtil$1.class
+-rw-rw-r--  2.0 unx     3817 b- defN 23-Aug-03 15:40 sklearn/Composite.class
+-rw-rw-r--  2.0 unx     1194 b- defN 23-Aug-03 15:40 sklearn/preprocessing/KBinsDiscretizer$1.class
+-rw-rw-r--  2.0 unx     4567 b- defN 23-Aug-03 15:40 sklearn/preprocessing/PowerTransformer.class
+-rw-rw-r--  2.0 unx     2381 b- defN 23-Aug-03 15:40 sklearn/preprocessing/LabelEncoder.class
+-rw-rw-r--  2.0 unx     4924 b- defN 23-Aug-03 15:40 sklearn/preprocessing/LabelBinarizer.class
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Aug-03 15:40 sklearn/preprocessing/EncoderUtil$3.class
+-rw-rw-r--  2.0 unx      389 b- defN 23-Aug-03 15:40 sklearn/preprocessing/Scaler.class
+-rw-rw-r--  2.0 unx      797 b- defN 23-Aug-03 15:40 sklearn/preprocessing/MultiOneHotEncoder$1.class
+-rw-rw-r--  2.0 unx     3242 b- defN 23-Aug-03 15:40 sklearn/preprocessing/MaxAbsScaler.class
+-rw-rw-r--  2.0 unx     2948 b- defN 23-Aug-03 15:40 sklearn/preprocessing/FunctionTransformer.class
+-rw-rw-r--  2.0 unx     3291 b- defN 23-Aug-03 15:40 sklearn/preprocessing/BaseEncoder.class
+-rw-rw-r--  2.0 unx     1270 b- defN 23-Aug-03 15:40 sklearn/preprocessing/EncoderUtil$1.class
+-rw-rw-r--  2.0 unx     4549 b- defN 23-Aug-03 15:40 sklearn/preprocessing/StandardScaler.class
+-rw-rw-r--  2.0 unx     9005 b- defN 23-Aug-03 15:40 sklearn/preprocessing/EncoderUtil.class
+-rw-rw-r--  2.0 unx     6343 b- defN 23-Aug-03 15:40 sklearn/preprocessing/PolynomialFeatures.class
+-rw-rw-r--  2.0 unx     8486 b- defN 23-Aug-03 15:40 sklearn/preprocessing/KBinsDiscretizer.class
+-rw-rw-r--  2.0 unx     4671 b- defN 23-Aug-03 15:40 sklearn/preprocessing/OneHotEncoder.class
+-rw-rw-r--  2.0 unx      729 b- defN 23-Aug-03 15:40 sklearn/preprocessing/EncoderUtil$4.class
+-rw-rw-r--  2.0 unx     2553 b- defN 23-Aug-03 15:40 sklearn/preprocessing/Binarizer.class
+-rw-rw-r--  2.0 unx     1054 b- defN 23-Aug-03 15:40 sklearn/preprocessing/EncoderUtil$2.class
+-rw-rw-r--  2.0 unx     3595 b- defN 23-Aug-03 15:40 sklearn/preprocessing/MinMaxScaler.class
+-rw-rw-r--  2.0 unx     4467 b- defN 23-Aug-03 15:40 sklearn/preprocessing/RobustScaler.class
+-rw-rw-r--  2.0 unx     3740 b- defN 23-Aug-03 15:40 sklearn/preprocessing/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      957 b- defN 23-Aug-03 15:40 sklearn/preprocessing/Imputer.class
+-rw-rw-r--  2.0 unx     2033 b- defN 23-Aug-03 15:40 sklearn/preprocessing/PolynomialFeatures$1.class
+-rw-rw-r--  2.0 unx    10333 b- defN 23-Aug-03 15:40 sklearn/preprocessing/MultiOneHotEncoder.class
+-rw-rw-r--  2.0 unx     2153 b- defN 23-Aug-03 15:40 sklearn/tree/TreeClassifier.class
+-rw-rw-r--  2.0 unx     3111 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil$1.class
+-rw-rw-r--  2.0 unx     2664 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil$4.class
+-rw-rw-r--  2.0 unx     4805 b- defN 23-Aug-03 15:40 sklearn/tree/visitors/TreeModelFlattener.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-Aug-03 15:40 sklearn/tree/visitors/TreeModelCompactor$1.class
+-rw-rw-r--  2.0 unx     5431 b- defN 23-Aug-03 15:40 sklearn/tree/visitors/TreeModelCompactor.class
+-rw-rw-r--  2.0 unx     2988 b- defN 23-Aug-03 15:40 sklearn/tree/visitors/TreeModelPruner.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-Aug-03 15:40 sklearn/tree/visitors/TreeModelFlattener$1.class
+-rw-rw-r--  2.0 unx      730 b- defN 23-Aug-03 15:40 sklearn/tree/visitors/TreeModelPruner$1.class
+-rw-rw-r--  2.0 unx      915 b- defN 23-Aug-03 15:40 sklearn/tree/RegressionCriterion.class
+-rw-rw-r--  2.0 unx     1151 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil$5.class
+-rw-rw-r--  2.0 unx     1014 b- defN 23-Aug-03 15:40 sklearn/tree/PresortBestSplitter.class
+-rw-rw-r--  2.0 unx     1589 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil$6.class
+-rw-rw-r--  2.0 unx     1764 b- defN 23-Aug-03 15:40 sklearn/tree/TreeRegressor.class
+-rw-rw-r--  2.0 unx     1489 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil$7.class
+-rw-rw-r--  2.0 unx    19425 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil.class
+-rw-rw-r--  2.0 unx     1123 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil$3.class
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Aug-03 15:40 sklearn/tree/HasTreeOptions.class
+-rw-rw-r--  2.0 unx     2293 b- defN 23-Aug-03 15:40 sklearn/tree/Tree.class
+-rw-rw-r--  2.0 unx      754 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil$2.class
+-rw-rw-r--  2.0 unx      150 b- defN 23-Aug-03 15:40 sklearn/tree/HasTree.class
+-rw-rw-r--  2.0 unx     1967 b- defN 23-Aug-03 15:40 sklearn/InitializerUtil.class
+-rw-rw-r--  2.0 unx      570 b- defN 23-Aug-03 15:40 sklearn/Regressor.class
+-rw-rw-r--  2.0 unx      211 b- defN 23-Aug-03 15:40 sklearn/HasNumberOfOutputs.class
+-rw-rw-r--  2.0 unx      534 b- defN 23-Aug-03 15:40 sklearn/OutlierDetector.class
+-rw-rw-r--  2.0 unx     2808 b- defN 23-Aug-03 15:40 sklearn/Calibrator.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-Aug-03 15:40 sklearn/HasClassifierOptions.class
+-rw-rw-r--  2.0 unx     7080 b- defN 23-Aug-03 15:40 sklearn/EstimatorUtil.class
+-rw-rw-r--  2.0 unx      199 b- defN 23-Aug-03 15:40 sklearn/HasType.class
+-rw-rw-r--  2.0 unx      678 b- defN 23-Aug-03 15:40 sklearn/cluster/MiniBatchKMeans.class
+-rw-rw-r--  2.0 unx     5086 b- defN 23-Aug-03 15:40 sklearn/cluster/KMeans.class
+-rw-rw-r--  2.0 unx    14149 b- defN 23-Aug-03 15:40 sklearn/Estimator.class
+-rw-rw-r--  2.0 unx     1624 b- defN 23-Aug-03 15:40 sklearn/Initializer.class
+-rw-rw-r--  2.0 unx     4595 b- defN 23-Aug-03 15:40 sklearn/multiclass/OneVsRestClassifier.class
+-rw-rw-r--  2.0 unx     5157 b- defN 23-Aug-03 15:40 sklearn2pmml/ruleset/RuleSetClassifier.class
+-rw-rw-r--  2.0 unx     1187 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/PMMLPipelineUtil$1.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/PMMLPipeline$3.class
+-rw-rw-r--  2.0 unx     1023 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/PMMLPipeline$4.class
+-rw-rw-r--  2.0 unx    27315 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/PMMLPipeline.class
+-rw-rw-r--  2.0 unx     1421 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/PMMLPipeline$2.class
+-rw-rw-r--  2.0 unx     1346 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/PMMLPipeline$1.class
+-rw-rw-r--  2.0 unx     1593 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/PMMLPipelineUtil.class
+-rw-rw-r--  2.0 unx     1811 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/Verification.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/MultiDomain.class
+-rw-rw-r--  2.0 unx     1152 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/ContinuousDomainEraser.class
+-rw-rw-r--  2.0 unx     1654 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/Alias.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/TemporalDomain.class
+-rw-rw-r--  2.0 unx      779 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/ContinuousDomain$1.class
+-rw-rw-r--  2.0 unx    11878 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/Domain.class
+-rw-rw-r--  2.0 unx     1416 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/MultiAlias.class
+-rw-rw-r--  2.0 unx     5055 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/DiscreteDomain.class
+-rw-rw-r--  2.0 unx     1952 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/CategoricalDomain.class
+-rw-rw-r--  2.0 unx     1453 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/DomainEraser.class
+-rw-rw-r--  2.0 unx      613 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/DateTimeDomain.class
+-rw-rw-r--  2.0 unx     7764 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/ContinuousDomain.class
+-rw-rw-r--  2.0 unx     1077 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/DiscreteDomainEraser.class
+-rw-rw-r--  2.0 unx     1590 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     1045 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/Domain$2.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/DateDomain.class
+-rw-rw-r--  2.0 unx     2374 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/DomainUtil.class
+-rw-rw-r--  2.0 unx     1033 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/Domain$1.class
+-rw-rw-r--  2.0 unx     1577 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/OrdinalDomain.class
+-rw-rw-r--  2.0 unx      672 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/Domain$4.class
+-rw-rw-r--  2.0 unx      799 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/Domain$3.class
+-rw-rw-r--  2.0 unx     7879 b- defN 23-Aug-03 15:40 sklearn2pmml/neural_network/MLPTransformer.class
+-rw-rw-r--  2.0 unx      391 b- defN 23-Aug-03 15:40 sklearn2pmml/SkLearn2PMMLFields.class
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Aug-03 15:40 sklearn2pmml/util/Evaluatable.class
+-rw-rw-r--  2.0 unx     1196 b- defN 23-Aug-03 15:40 sklearn2pmml/util/Expression.class
+-rw-rw-r--  2.0 unx     1189 b- defN 23-Aug-03 15:40 sklearn2pmml/util/Predicate.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Aug-03 15:40 sklearn2pmml/util/Reshaper.class
+-rw-rw-r--  2.0 unx     3392 b- defN 23-Aug-03 15:40 sklearn2pmml/util/EvaluatableUtil.class
+-rw-rw-r--  2.0 unx     1658 b- defN 23-Aug-03 15:40 sklearn2pmml/util/Slicer.class
+-rw-rw-r--  2.0 unx     2418 b- defN 23-Aug-03 15:40 sklearn2pmml/feature_extraction/text/Splitter.class
+-rw-rw-r--  2.0 unx     3184 b- defN 23-Aug-03 15:40 sklearn2pmml/feature_extraction/text/Matcher.class
+-rw-rw-r--  2.0 unx     1262 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/SelectFirstRegressor.class
+-rw-rw-r--  2.0 unx     2083 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/GBDTUtil$2.class
+-rw-rw-r--  2.0 unx     1934 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/GBDTLMRegressor.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/GBDTUtil$1.class
+-rw-rw-r--  2.0 unx     7410 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/EstimatorChain.class
+-rw-rw-r--  2.0 unx     6582 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/GBDTUtil.class
+-rw-rw-r--  2.0 unx     3995 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/Link.class
+-rw-rw-r--  2.0 unx     4360 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/SelectFirstUtil.class
+-rw-rw-r--  2.0 unx     4249 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/GBDTLRClassifier.class
+-rw-rw-r--  2.0 unx     2608 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/SelectFirstClassifier.class
+-rw-rw-r--  2.0 unx     1438 b- defN 23-Aug-03 15:40 sklearn2pmml/EstimatorProxy$1.class
+-rw-rw-r--  2.0 unx      946 b- defN 23-Aug-03 15:40 sklearn2pmml/feature_selection/SelectUnique.class
+-rw-rw-r--  2.0 unx     6477 b- defN 23-Aug-03 15:40 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
+-rw-rw-r--  2.0 unx      791 b- defN 23-Aug-03 15:40 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
+-rw-rw-r--  2.0 unx     1197 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/PatternTransformer.class
+-rw-rw-r--  2.0 unx     2908 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/ReplaceTransformer.class
+-rw-rw-r--  2.0 unx     1844 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/WordCountTransformer.class
+-rw-rw-r--  2.0 unx      597 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/DateTimeFormatter.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
+-rw-rw-r--  2.0 unx     4621 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/DurationTransformer.class
+-rw-rw-r--  2.0 unx      444 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
+-rw-rw-r--  2.0 unx     2777 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/FilterLookupTransformer.class
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/Formatter.class
+-rw-rw-r--  2.0 unx     3424 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/CastTransformer.class
+-rw-rw-r--  2.0 unx     2758 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/MatchesTransformer.class
+-rw-rw-r--  2.0 unx      589 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/NumberFormatter.class
+-rw-rw-r--  2.0 unx     4149 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/MultiLookupTransformer.class
+-rw-rw-r--  2.0 unx     3871 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/StringNormalizer.class
+-rw-rw-r--  2.0 unx     7145 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/ExpressionTransformer.class
+-rw-rw-r--  2.0 unx      635 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     3604 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/DataFrameConstructor.class
+-rw-rw-r--  2.0 unx     2847 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/ConcatTransformer.class
+-rw-rw-r--  2.0 unx     5993 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/CutTransformer.class
+-rw-rw-r--  2.0 unx     7025 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/BSplineTransformer.class
+-rw-rw-r--  2.0 unx     6410 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/LookupTransformer.class
+-rw-rw-r--  2.0 unx     3236 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/SubstringTransformer.class
+-rw-rw-r--  2.0 unx     3181 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
+-rw-rw-r--  2.0 unx     2132 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
+-rw-rw-r--  2.0 unx     3328 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/Aggregator.class
+-rw-rw-r--  2.0 unx      647 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     1639 b- defN 23-Aug-03 15:40 sklearn2pmml/tree/CHAIDRegressor.class
+-rw-rw-r--  2.0 unx    10719 b- defN 23-Aug-03 15:40 sklearn2pmml/tree/CHAIDUtil.class
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Aug-03 15:40 sklearn2pmml/tree/CHAIDClassifier.class
+-rw-rw-r--  2.0 unx     1417 b- defN 23-Aug-03 15:40 sklearn2pmml/tree/CHAIDUtil$1.class
+-rw-rw-r--  2.0 unx     4170 b- defN 23-Aug-03 15:40 sklearn2pmml/EstimatorProxy.class
+-rw-rw-r--  2.0 unx     1479 b- defN 23-Aug-03 15:40 sklearn2pmml/SelectorProxy.class
+-rw-rw-r--  2.0 unx     2046 b- defN 23-Aug-03 15:40 sklearn2pmml/expression/ExpressionUtil.class
+-rw-rw-r--  2.0 unx     3799 b- defN 23-Aug-03 15:40 sklearn2pmml/expression/ExpressionRegressor.class
+-rw-rw-r--  2.0 unx      990 b- defN 23-Aug-03 15:40 sklearn2pmml/expression/ExpressionClassifier$1.class
+-rw-rw-r--  2.0 unx     8687 b- defN 23-Aug-03 15:40 sklearn2pmml/expression/ExpressionClassifier.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Aug-03 15:40 sklearn2pmml/expression/ExpressionUtil$1.class
+-rw-rw-r--  2.0 unx     1774 b- defN 23-Aug-03 15:40 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
+-rw-rw-r--  2.0 unx     2764 b- defN 23-Aug-03 15:40 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
+-rw-rw-r--  2.0 unx     3549 b- defN 23-Aug-03 15:40 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
+-rw-rw-r--  2.0 unx    15476 b- defN 23-Aug-03 15:40 org/jpmml/sklearn/SkLearnEncoder.class
+-rw-rw-r--  2.0 unx      194 b- defN 23-Aug-03 15:40 org/jpmml/sklearn/FieldNames.class
+-rw-rw-r--  2.0 unx      171 b- defN 23-Aug-03 15:40 org/jpmml/sklearn/HasSkLearnOptions.class
+-rw-rw-r--  2.0 unx     1179 b- defN 23-Aug-03 15:40 org/jpmml/sklearn/SkLearnEncoder$1.class
+-rw-rw-r--  2.0 unx     1822 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
+-rw-rw-r--  2.0 unx       57 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
+410 files, 933938 bytes uncompressed, 411785 bytes compressed:  55.9%
```

#### zipnote «TEMP»/diffoscope_q23y7y7v_/tmpa2ymr09d_.zip

```diff
@@ -270,14 +270,17 @@
 
 Filename: sklearn/pipeline/PipelineUtil.class
 Comment: 
 
 Filename: sklearn/pipeline/PipelineClassifier.class
 Comment: 
 
+Filename: sklearn/pipeline/PipelineClusterer.class
+Comment: 
+
 Filename: sklearn/dummy/DummyClassifier.class
 Comment: 
 
 Filename: sklearn/dummy/DummyRegressor.class
 Comment: 
 
 Filename: sklearn/SkLearnFields.class
@@ -342,26 +345,32 @@
 
 Filename: sklearn/Step.class
 Comment: 
 
 Filename: sklearn/HasDefaultValue.class
 Comment: 
 
+Filename: sklearn/Proxy.class
+Comment: 
+
 Filename: sklearn/impute/MissingIndicator.class
 Comment: 
 
 Filename: sklearn/impute/ImputerUtil.class
 Comment: 
 
 Filename: sklearn/impute/SimpleImputer.class
 Comment: 
 
 Filename: sklearn/naive_bayes/GaussianNB.class
 Comment: 
 
+Filename: sklearn/HasFeatureNamesIn.class
+Comment: 
+
 Filename: sklearn/linear_model/LinearRegressor.class
 Comment: 
 
 Filename: sklearn/linear_model/LinearClassifier.class
 Comment: 
 
 Filename: sklearn/linear_model/logistic/LogisticRegression.class
@@ -504,14 +513,17 @@
 
 Filename: sklearn/PassThrough.class
 Comment: 
 
 Filename: sklearn/HasPriorProbability.class
 Comment: 
 
+Filename: sklearn/SkLearnSteps.class
+Comment: 
+
 Filename: sklearn/feature_extraction/text/TfidfVectorizer.class
 Comment: 
 
 Filename: sklearn/feature_extraction/text/TfidfVectorizer$1.class
 Comment: 
 
 Filename: sklearn/feature_extraction/text/Tokenizer.class
@@ -915,14 +927,17 @@
 
 Filename: sklearn/multiclass/OneVsRestClassifier.class
 Comment: 
 
 Filename: sklearn2pmml/ruleset/RuleSetClassifier.class
 Comment: 
 
+Filename: sklearn2pmml/pipeline/PMMLPipelineUtil$1.class
+Comment: 
+
 Filename: sklearn2pmml/pipeline/PMMLPipeline$3.class
 Comment: 
 
 Filename: sklearn2pmml/pipeline/PMMLPipeline$4.class
 Comment: 
 
 Filename: sklearn2pmml/pipeline/PMMLPipeline.class
@@ -930,14 +945,17 @@
 
 Filename: sklearn2pmml/pipeline/PMMLPipeline$2.class
 Comment: 
 
 Filename: sklearn2pmml/pipeline/PMMLPipeline$1.class
 Comment: 
 
+Filename: sklearn2pmml/pipeline/PMMLPipelineUtil.class
+Comment: 
+
 Filename: sklearn2pmml/pipeline/Verification.class
 Comment: 
 
 Filename: sklearn2pmml/decoration/MultiDomain.class
 Comment: 
 
 Filename: sklearn2pmml/decoration/ContinuousDomainEraser.class
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-SkLearn library
-Implementation-Version: 1.7.33
+Implementation-Version: 1.7.34
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### sklearn/pipeline/Pipeline$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,95 +1,97 @@
-  SHA-256 checksum 56f9a79bda77f8bf022d7c361606ba0a1bd7339bd97071ca77a6e1ac4fb56516
+  SHA-256 checksum 3c4fe13554c603f6527e4d65f5043d460f481e2cfe6e497e090218b4cf4a9c84
   Compiled from "Pipeline.java"
 class sklearn.pipeline.Pipeline$2 extends org.jpmml.python.CastFunction<E>
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
-  this_class: #15                         // sklearn/pipeline/Pipeline$2
-  super_class: #16                        // org/jpmml/python/CastFunction
+  this_class: #16                         // sklearn/pipeline/Pipeline$2
+  super_class: #17                        // org/jpmml/python/CastFunction
   interfaces: 0, fields: 1, methods: 4, attributes: 4
 Constant pool:
-   #1 = Fieldref           #15.#47        // sklearn/pipeline/Pipeline$2.this$0:Lsklearn/pipeline/Pipeline;
-   #2 = Methodref          #16.#48        // org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
-   #3 = String             #49            // passthrough
-   #4 = Methodref          #50.#51        // java/lang/String.equals:(Ljava/lang/Object;)Z
-   #5 = Methodref          #16.#52        // org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
-   #6 = Class              #53            // sklearn/Estimator
-   #7 = Class              #54            // java/lang/StringBuilder
-   #8 = Methodref          #7.#55         // java/lang/StringBuilder."<init>":()V
-   #9 = String             #56            // The transformer object of the final step (
-  #10 = Methodref          #7.#57         // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #11 = Methodref          #58.#59        // org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
-  #12 = String             #60            // ) is not a supported Estimator
-  #13 = Methodref          #7.#61         // java/lang/StringBuilder.toString:()Ljava/lang/String;
-  #14 = Methodref          #15.#62        // sklearn/pipeline/Pipeline$2.apply:(Ljava/lang/Object;)Lsklearn/Estimator;
-  #15 = Class              #63            // sklearn/pipeline/Pipeline$2
-  #16 = Class              #64            // org/jpmml/python/CastFunction
-  #17 = Utf8               this$0
-  #18 = Utf8               Lsklearn/pipeline/Pipeline;
-  #19 = Utf8               <init>
-  #20 = Utf8               (Lsklearn/pipeline/Pipeline;Ljava/lang/Class;)V
-  #21 = Utf8               Code
-  #22 = Utf8               LineNumberTable
-  #23 = Utf8               LocalVariableTable
-  #24 = Utf8               this
-  #25 = Utf8               InnerClasses
-  #26 = Utf8               Lsklearn/pipeline/Pipeline$2;
-  #27 = Utf8               x0
-  #28 = Utf8               Ljava/lang/Class;
-  #29 = Utf8               LocalVariableTypeTable
-  #30 = Utf8               Ljava/lang/Class<+TE;>;
-  #31 = Utf8               apply
-  #32 = Utf8               (Ljava/lang/Object;)Lsklearn/Estimator;
-  #33 = Utf8               object
-  #34 = Utf8               Ljava/lang/Object;
-  #35 = Utf8               StackMapTable
-  #36 = Utf8               Signature
-  #37 = Utf8               (Ljava/lang/Object;)TE;
-  #38 = Utf8               formatMessage
-  #39 = Utf8               (Ljava/lang/Object;)Ljava/lang/String;
-  #40 = Utf8               (Ljava/lang/Object;)Ljava/lang/Object;
-  #41 = Utf8               Lorg/jpmml/python/CastFunction<TE;>;
-  #42 = Utf8               SourceFile
-  #43 = Utf8               Pipeline.java
-  #44 = Utf8               EnclosingMethod
-  #45 = Class              #65            // sklearn/pipeline/Pipeline
-  #46 = NameAndType        #66:#67        // getFinalEstimator:(Ljava/lang/Class;)Lsklearn/Estimator;
-  #47 = NameAndType        #17:#18        // this$0:Lsklearn/pipeline/Pipeline;
-  #48 = NameAndType        #19:#68        // "<init>":(Ljava/lang/Class;)V
-  #49 = Utf8               passthrough
-  #50 = Class              #69            // java/lang/String
-  #51 = NameAndType        #70:#71        // equals:(Ljava/lang/Object;)Z
-  #52 = NameAndType        #31:#40        // apply:(Ljava/lang/Object;)Ljava/lang/Object;
-  #53 = Utf8               sklearn/Estimator
-  #54 = Utf8               java/lang/StringBuilder
-  #55 = NameAndType        #19:#72        // "<init>":()V
-  #56 = Utf8               The transformer object of the final step (
-  #57 = NameAndType        #73:#74        // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #58 = Class              #75            // org/jpmml/python/ClassDictUtil
-  #59 = NameAndType        #76:#39        // formatClass:(Ljava/lang/Object;)Ljava/lang/String;
-  #60 = Utf8               ) is not a supported Estimator
-  #61 = NameAndType        #77:#78        // toString:()Ljava/lang/String;
-  #62 = NameAndType        #31:#32        // apply:(Ljava/lang/Object;)Lsklearn/Estimator;
-  #63 = Utf8               sklearn/pipeline/Pipeline$2
-  #64 = Utf8               org/jpmml/python/CastFunction
-  #65 = Utf8               sklearn/pipeline/Pipeline
-  #66 = Utf8               getFinalEstimator
-  #67 = Utf8               (Ljava/lang/Class;)Lsklearn/Estimator;
-  #68 = Utf8               (Ljava/lang/Class;)V
-  #69 = Utf8               java/lang/String
-  #70 = Utf8               equals
-  #71 = Utf8               (Ljava/lang/Object;)Z
-  #72 = Utf8               ()V
-  #73 = Utf8               append
-  #74 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #75 = Utf8               org/jpmml/python/ClassDictUtil
-  #76 = Utf8               formatClass
-  #77 = Utf8               toString
-  #78 = Utf8               ()Ljava/lang/String;
+   #1 = Fieldref           #16.#48        // sklearn/pipeline/Pipeline$2.this$0:Lsklearn/pipeline/Pipeline;
+   #2 = Methodref          #17.#49        // org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
+   #3 = Class              #50            // sklearn/SkLearnSteps
+   #4 = String             #51            // passthrough
+   #5 = Methodref          #52.#53        // java/lang/String.equals:(Ljava/lang/Object;)Z
+   #6 = Methodref          #17.#54        // org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
+   #7 = Class              #55            // sklearn/Estimator
+   #8 = Class              #56            // java/lang/StringBuilder
+   #9 = Methodref          #8.#57         // java/lang/StringBuilder."<init>":()V
+  #10 = String             #58            // The transformer object of the final step (
+  #11 = Methodref          #8.#59         // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #12 = Methodref          #60.#61        // org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
+  #13 = String             #62            // ) is not a supported Estimator
+  #14 = Methodref          #8.#63         // java/lang/StringBuilder.toString:()Ljava/lang/String;
+  #15 = Methodref          #16.#64        // sklearn/pipeline/Pipeline$2.apply:(Ljava/lang/Object;)Lsklearn/Estimator;
+  #16 = Class              #65            // sklearn/pipeline/Pipeline$2
+  #17 = Class              #66            // org/jpmml/python/CastFunction
+  #18 = Utf8               this$0
+  #19 = Utf8               Lsklearn/pipeline/Pipeline;
+  #20 = Utf8               <init>
+  #21 = Utf8               (Lsklearn/pipeline/Pipeline;Ljava/lang/Class;)V
+  #22 = Utf8               Code
+  #23 = Utf8               LineNumberTable
+  #24 = Utf8               LocalVariableTable
+  #25 = Utf8               this
+  #26 = Utf8               InnerClasses
+  #27 = Utf8               Lsklearn/pipeline/Pipeline$2;
+  #28 = Utf8               x0
+  #29 = Utf8               Ljava/lang/Class;
+  #30 = Utf8               LocalVariableTypeTable
+  #31 = Utf8               Ljava/lang/Class<+TE;>;
+  #32 = Utf8               apply
+  #33 = Utf8               (Ljava/lang/Object;)Lsklearn/Estimator;
+  #34 = Utf8               object
+  #35 = Utf8               Ljava/lang/Object;
+  #36 = Utf8               StackMapTable
+  #37 = Utf8               Signature
+  #38 = Utf8               (Ljava/lang/Object;)TE;
+  #39 = Utf8               formatMessage
+  #40 = Utf8               (Ljava/lang/Object;)Ljava/lang/String;
+  #41 = Utf8               (Ljava/lang/Object;)Ljava/lang/Object;
+  #42 = Utf8               Lorg/jpmml/python/CastFunction<TE;>;
+  #43 = Utf8               SourceFile
+  #44 = Utf8               Pipeline.java
+  #45 = Utf8               EnclosingMethod
+  #46 = Class              #67            // sklearn/pipeline/Pipeline
+  #47 = NameAndType        #68:#69        // getFinalEstimator:(Ljava/lang/Class;)Lsklearn/Estimator;
+  #48 = NameAndType        #18:#19        // this$0:Lsklearn/pipeline/Pipeline;
+  #49 = NameAndType        #20:#70        // "<init>":(Ljava/lang/Class;)V
+  #50 = Utf8               sklearn/SkLearnSteps
+  #51 = Utf8               passthrough
+  #52 = Class              #71            // java/lang/String
+  #53 = NameAndType        #72:#73        // equals:(Ljava/lang/Object;)Z
+  #54 = NameAndType        #32:#41        // apply:(Ljava/lang/Object;)Ljava/lang/Object;
+  #55 = Utf8               sklearn/Estimator
+  #56 = Utf8               java/lang/StringBuilder
+  #57 = NameAndType        #20:#74        // "<init>":()V
+  #58 = Utf8               The transformer object of the final step (
+  #59 = NameAndType        #75:#76        // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #60 = Class              #77            // org/jpmml/python/ClassDictUtil
+  #61 = NameAndType        #78:#40        // formatClass:(Ljava/lang/Object;)Ljava/lang/String;
+  #62 = Utf8               ) is not a supported Estimator
+  #63 = NameAndType        #79:#80        // toString:()Ljava/lang/String;
+  #64 = NameAndType        #32:#33        // apply:(Ljava/lang/Object;)Lsklearn/Estimator;
+  #65 = Utf8               sklearn/pipeline/Pipeline$2
+  #66 = Utf8               org/jpmml/python/CastFunction
+  #67 = Utf8               sklearn/pipeline/Pipeline
+  #68 = Utf8               getFinalEstimator
+  #69 = Utf8               (Ljava/lang/Class;)Lsklearn/Estimator;
+  #70 = Utf8               (Ljava/lang/Class;)V
+  #71 = Utf8               java/lang/String
+  #72 = Utf8               equals
+  #73 = Utf8               (Ljava/lang/Object;)Z
+  #74 = Utf8               ()V
+  #75 = Utf8               append
+  #76 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #77 = Utf8               org/jpmml/python/ClassDictUtil
+  #78 = Utf8               formatClass
+  #79 = Utf8               toString
+  #80 = Utf8               ()Ljava/lang/String;
 {
   final sklearn.pipeline.Pipeline this$0;
     descriptor: Lsklearn/pipeline/Pipeline;
     flags: (0x1010) ACC_FINAL, ACC_SYNTHETIC
 
   sklearn.pipeline.Pipeline$2(sklearn.pipeline.Pipeline, java.lang.Class);
     descriptor: (Lsklearn/pipeline/Pipeline;Ljava/lang/Class;)V
@@ -100,89 +102,89 @@
          1: aload_1
          2: putfield      #1                  // Field this$0:Lsklearn/pipeline/Pipeline;
          5: aload_0
          6: aload_2
          7: invokespecial #2                  // Method org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
         10: return
       LineNumberTable:
-        line 132: 0
+        line 134: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lsklearn/pipeline/Pipeline$2;
             0      11     1 this$0   Lsklearn/pipeline/Pipeline;
             0      11     2    x0   Ljava/lang/Class;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      11     2    x0   Ljava/lang/Class<+TE;>;
 
   public E apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Lsklearn/Estimator;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=2, locals=2, args_size=2
-         0: ldc           #3                  // String passthrough
+         0: ldc           #4                  // String passthrough
          2: aload_1
-         3: invokevirtual #4                  // Method java/lang/String.equals:(Ljava/lang/Object;)Z
+         3: invokevirtual #5                  // Method java/lang/String.equals:(Ljava/lang/Object;)Z
          6: ifeq          11
          9: aconst_null
         10: areturn
         11: aload_0
         12: aload_1
-        13: invokespecial #5                  // Method org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
-        16: checkcast     #6                  // class sklearn/Estimator
+        13: invokespecial #6                  // Method org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
+        16: checkcast     #7                  // class sklearn/Estimator
         19: areturn
       LineNumberTable:
-        line 137: 0
-        line 138: 9
-        line 141: 11
+        line 139: 0
+        line 140: 9
+        line 143: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lsklearn/pipeline/Pipeline$2;
             0      20     1 object   Ljava/lang/Object;
       StackMapTable: number_of_entries = 1
         frame_type = 11 /* same */
-    Signature: #37                          // (Ljava/lang/Object;)TE;
+    Signature: #38                          // (Ljava/lang/Object;)TE;
 
   public java.lang.String formatMessage(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/String;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=2, locals=2, args_size=2
-         0: new           #7                  // class java/lang/StringBuilder
+         0: new           #8                  // class java/lang/StringBuilder
          3: dup
-         4: invokespecial #8                  // Method java/lang/StringBuilder."<init>":()V
-         7: ldc           #9                  // String The transformer object of the final step (
-         9: invokevirtual #10                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+         4: invokespecial #9                  // Method java/lang/StringBuilder."<init>":()V
+         7: ldc           #10                 // String The transformer object of the final step (
+         9: invokevirtual #11                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         12: aload_1
-        13: invokestatic  #11                 // Method org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
-        16: invokevirtual #10                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-        19: ldc           #12                 // String ) is not a supported Estimator
-        21: invokevirtual #10                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-        24: invokevirtual #13                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
+        13: invokestatic  #12                 // Method org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
+        16: invokevirtual #11                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+        19: ldc           #13                 // String ) is not a supported Estimator
+        21: invokevirtual #11                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+        24: invokevirtual #14                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
         27: areturn
       LineNumberTable:
-        line 146: 0
+        line 148: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      28     0  this   Lsklearn/pipeline/Pipeline$2;
             0      28     1 object   Ljava/lang/Object;
 
   public java.lang.Object apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/Object;
     flags: (0x1041) ACC_PUBLIC, ACC_BRIDGE, ACC_SYNTHETIC
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
-         2: invokevirtual #14                 // Method apply:(Ljava/lang/Object;)Lsklearn/Estimator;
+         2: invokevirtual #15                 // Method apply:(Ljava/lang/Object;)Lsklearn/Estimator;
          5: areturn
       LineNumberTable:
-        line 132: 0
+        line 134: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/pipeline/Pipeline$2;
 }
-Signature: #41                          // Lorg/jpmml/python/CastFunction<TE;>;
+Signature: #42                          // Lorg/jpmml/python/CastFunction<TE;>;
 SourceFile: "Pipeline.java"
-EnclosingMethod: #45.#46                // sklearn.pipeline.Pipeline.getFinalEstimator
+EnclosingMethod: #46.#47                // sklearn.pipeline.Pipeline.getFinalEstimator
 InnerClasses:
-  #15;                                    // class sklearn/pipeline/Pipeline$2
+  #16;                                    // class sklearn/pipeline/Pipeline$2
```

#### sklearn/pipeline/Pipeline.class

##### procyon -ec {}

```diff
@@ -1,10 +1,11 @@
 
 package sklearn.pipeline;
 
+import sklearn.Clusterer;
 import sklearn.Regressor;
 import sklearn.Classifier;
 import org.jpmml.python.CastFunction;
 import com.google.common.base.Function;
 import com.google.common.collect.Lists;
 import sklearn.Transformer;
 import org.jpmml.python.CastUtil;
@@ -108,22 +109,34 @@
         final Estimator estimator = this.getFinalEstimator();
         if (estimator instanceof Classifier) {
             return (Estimator)this.toClassifier();
         }
         if (estimator instanceof Regressor) {
             return (Estimator)this.toRegressor();
         }
+        if (estimator instanceof Clusterer) {
+            return (Estimator)this.toClusterer();
+        }
         throw new IllegalArgumentException();
     }
     
     public Classifier toClassifier() {
         return (Classifier)new PipelineClassifier(this);
     }
     
     public Regressor toRegressor() {
         return (Regressor)new PipelineRegressor(this);
     }
     
+    public Clusterer toClusterer() {
+        return (Clusterer)new PipelineClusterer(this);
+    }
+    
     public List<Object[]> getSteps() {
         return this.getTupleList("steps");
     }
+    
+    protected Pipeline setSteps(final List<Object[]> steps) {
+        this.put((Object)"steps", (Object)steps);
+        return this;
+    }
 }
```

#### sklearn/pipeline/PipelineRegressor.class

##### procyon -ec {}

```diff
@@ -2,32 +2,44 @@
 package sklearn.pipeline;
 
 import sklearn.Transformer;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
 import org.dmg.pmml.DataType;
 import org.dmg.pmml.OpType;
+import java.util.List;
+import sklearn.Proxy;
 import sklearn.HasHead;
 import sklearn.Regressor;
 
-public class PipelineRegressor extends Regressor implements HasHead
+public class PipelineRegressor extends Regressor implements HasHead, Proxy
 {
     private Pipeline pipeline;
     
     public PipelineRegressor(final Pipeline pipeline) {
         super(pipeline.getPythonModule(), pipeline.getPythonName());
         this.pipeline = null;
         this.setPipeline(pipeline);
     }
     
+    public List<String> getFeatureNamesIn() {
+        final Pipeline pipeline = this.getPipeline();
+        return pipeline.getFeatureNamesIn();
+    }
+    
     public int getNumberOfFeatures() {
         final Pipeline pipeline = this.getPipeline();
         return pipeline.getNumberOfFeatures();
     }
     
+    public int getNumberOfOutputs() {
+        final Regressor regressor = this.getFinalRegressor();
+        return regressor.getNumberOfOutputs();
+    }
+    
     public OpType getOpType() {
         final Pipeline pipeline = this.getPipeline();
         return pipeline.getOpType();
     }
     
     public DataType getDataType() {
         final Pipeline pipeline = this.getPipeline();
```

#### sklearn/pipeline/Pipeline$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,100 +1,102 @@
-  SHA-256 checksum d1ba32dcbdebd2bd059bc3d30fccdb6d56adbddd25b82f4a21fd5f7cf49599b9
+  SHA-256 checksum 3b513eee5a1485ec18be204f6679c9edb7c2c7b0fba4166446677bbcb5fb2115
   Compiled from "Pipeline.java"
 class sklearn.pipeline.Pipeline$1 extends org.jpmml.python.CastFunction<sklearn.Transformer>
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
-  this_class: #16                         // sklearn/pipeline/Pipeline$1
-  super_class: #17                        // org/jpmml/python/CastFunction
+  this_class: #17                         // sklearn/pipeline/Pipeline$1
+  super_class: #18                        // org/jpmml/python/CastFunction
   interfaces: 0, fields: 1, methods: 4, attributes: 4
 Constant pool:
-   #1 = Fieldref           #16.#47        // sklearn/pipeline/Pipeline$1.this$0:Lsklearn/pipeline/Pipeline;
-   #2 = Methodref          #17.#48        // org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
-   #3 = String             #49            // passthrough
-   #4 = Methodref          #50.#51        // java/lang/String.equals:(Ljava/lang/Object;)Z
-   #5 = Fieldref           #52.#53        // sklearn/PassThrough.INSTANCE:Lsklearn/PassThrough;
-   #6 = Methodref          #17.#54        // org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
-   #7 = Class              #55            // sklearn/Transformer
-   #8 = Class              #56            // java/lang/StringBuilder
-   #9 = Methodref          #8.#57         // java/lang/StringBuilder."<init>":()V
-  #10 = String             #58            // The transformer object (
-  #11 = Methodref          #8.#59         // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #12 = Methodref          #60.#61        // org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
-  #13 = String             #62            // ) is not a supported Transformer
-  #14 = Methodref          #8.#63         // java/lang/StringBuilder.toString:()Ljava/lang/String;
-  #15 = Methodref          #16.#64        // sklearn/pipeline/Pipeline$1.apply:(Ljava/lang/Object;)Lsklearn/Transformer;
-  #16 = Class              #65            // sklearn/pipeline/Pipeline$1
-  #17 = Class              #66            // org/jpmml/python/CastFunction
-  #18 = Utf8               this$0
-  #19 = Utf8               Lsklearn/pipeline/Pipeline;
-  #20 = Utf8               <init>
-  #21 = Utf8               (Lsklearn/pipeline/Pipeline;Ljava/lang/Class;)V
-  #22 = Utf8               Code
-  #23 = Utf8               LineNumberTable
-  #24 = Utf8               LocalVariableTable
-  #25 = Utf8               this
-  #26 = Utf8               InnerClasses
-  #27 = Utf8               Lsklearn/pipeline/Pipeline$1;
-  #28 = Utf8               x0
-  #29 = Utf8               Ljava/lang/Class;
-  #30 = Utf8               LocalVariableTypeTable
-  #31 = Utf8               Ljava/lang/Class<+Lsklearn/Transformer;>;
-  #32 = Utf8               apply
-  #33 = Utf8               (Ljava/lang/Object;)Lsklearn/Transformer;
-  #34 = Utf8               object
-  #35 = Utf8               Ljava/lang/Object;
-  #36 = Utf8               StackMapTable
-  #37 = Utf8               formatMessage
-  #38 = Utf8               (Ljava/lang/Object;)Ljava/lang/String;
-  #39 = Utf8               (Ljava/lang/Object;)Ljava/lang/Object;
-  #40 = Utf8               Signature
-  #41 = Utf8               Lorg/jpmml/python/CastFunction<Lsklearn/Transformer;>;
-  #42 = Utf8               SourceFile
-  #43 = Utf8               Pipeline.java
-  #44 = Utf8               EnclosingMethod
-  #45 = Class              #67            // sklearn/pipeline/Pipeline
-  #46 = NameAndType        #68:#69        // getTransformers:()Ljava/util/List;
-  #47 = NameAndType        #18:#19        // this$0:Lsklearn/pipeline/Pipeline;
-  #48 = NameAndType        #20:#70        // "<init>":(Ljava/lang/Class;)V
-  #49 = Utf8               passthrough
-  #50 = Class              #71            // java/lang/String
-  #51 = NameAndType        #72:#73        // equals:(Ljava/lang/Object;)Z
-  #52 = Class              #74            // sklearn/PassThrough
-  #53 = NameAndType        #75:#76        // INSTANCE:Lsklearn/PassThrough;
-  #54 = NameAndType        #32:#39        // apply:(Ljava/lang/Object;)Ljava/lang/Object;
-  #55 = Utf8               sklearn/Transformer
-  #56 = Utf8               java/lang/StringBuilder
-  #57 = NameAndType        #20:#77        // "<init>":()V
-  #58 = Utf8               The transformer object (
-  #59 = NameAndType        #78:#79        // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #60 = Class              #80            // org/jpmml/python/ClassDictUtil
-  #61 = NameAndType        #81:#38        // formatClass:(Ljava/lang/Object;)Ljava/lang/String;
-  #62 = Utf8               ) is not a supported Transformer
-  #63 = NameAndType        #82:#83        // toString:()Ljava/lang/String;
-  #64 = NameAndType        #32:#33        // apply:(Ljava/lang/Object;)Lsklearn/Transformer;
-  #65 = Utf8               sklearn/pipeline/Pipeline$1
-  #66 = Utf8               org/jpmml/python/CastFunction
-  #67 = Utf8               sklearn/pipeline/Pipeline
-  #68 = Utf8               getTransformers
-  #69 = Utf8               ()Ljava/util/List;
-  #70 = Utf8               (Ljava/lang/Class;)V
-  #71 = Utf8               java/lang/String
-  #72 = Utf8               equals
-  #73 = Utf8               (Ljava/lang/Object;)Z
-  #74 = Utf8               sklearn/PassThrough
-  #75 = Utf8               INSTANCE
-  #76 = Utf8               Lsklearn/PassThrough;
-  #77 = Utf8               ()V
-  #78 = Utf8               append
-  #79 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #80 = Utf8               org/jpmml/python/ClassDictUtil
-  #81 = Utf8               formatClass
-  #82 = Utf8               toString
-  #83 = Utf8               ()Ljava/lang/String;
+   #1 = Fieldref           #17.#48        // sklearn/pipeline/Pipeline$1.this$0:Lsklearn/pipeline/Pipeline;
+   #2 = Methodref          #18.#49        // org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
+   #3 = Class              #50            // sklearn/SkLearnSteps
+   #4 = String             #51            // passthrough
+   #5 = Methodref          #52.#53        // java/lang/String.equals:(Ljava/lang/Object;)Z
+   #6 = Fieldref           #54.#55        // sklearn/PassThrough.INSTANCE:Lsklearn/PassThrough;
+   #7 = Methodref          #18.#56        // org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
+   #8 = Class              #57            // sklearn/Transformer
+   #9 = Class              #58            // java/lang/StringBuilder
+  #10 = Methodref          #9.#59         // java/lang/StringBuilder."<init>":()V
+  #11 = String             #60            // The transformer object (
+  #12 = Methodref          #9.#61         // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #13 = Methodref          #62.#63        // org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
+  #14 = String             #64            // ) is not a supported Transformer
+  #15 = Methodref          #9.#65         // java/lang/StringBuilder.toString:()Ljava/lang/String;
+  #16 = Methodref          #17.#66        // sklearn/pipeline/Pipeline$1.apply:(Ljava/lang/Object;)Lsklearn/Transformer;
+  #17 = Class              #67            // sklearn/pipeline/Pipeline$1
+  #18 = Class              #68            // org/jpmml/python/CastFunction
+  #19 = Utf8               this$0
+  #20 = Utf8               Lsklearn/pipeline/Pipeline;
+  #21 = Utf8               <init>
+  #22 = Utf8               (Lsklearn/pipeline/Pipeline;Ljava/lang/Class;)V
+  #23 = Utf8               Code
+  #24 = Utf8               LineNumberTable
+  #25 = Utf8               LocalVariableTable
+  #26 = Utf8               this
+  #27 = Utf8               InnerClasses
+  #28 = Utf8               Lsklearn/pipeline/Pipeline$1;
+  #29 = Utf8               x0
+  #30 = Utf8               Ljava/lang/Class;
+  #31 = Utf8               LocalVariableTypeTable
+  #32 = Utf8               Ljava/lang/Class<+Lsklearn/Transformer;>;
+  #33 = Utf8               apply
+  #34 = Utf8               (Ljava/lang/Object;)Lsklearn/Transformer;
+  #35 = Utf8               object
+  #36 = Utf8               Ljava/lang/Object;
+  #37 = Utf8               StackMapTable
+  #38 = Utf8               formatMessage
+  #39 = Utf8               (Ljava/lang/Object;)Ljava/lang/String;
+  #40 = Utf8               (Ljava/lang/Object;)Ljava/lang/Object;
+  #41 = Utf8               Signature
+  #42 = Utf8               Lorg/jpmml/python/CastFunction<Lsklearn/Transformer;>;
+  #43 = Utf8               SourceFile
+  #44 = Utf8               Pipeline.java
+  #45 = Utf8               EnclosingMethod
+  #46 = Class              #69            // sklearn/pipeline/Pipeline
+  #47 = NameAndType        #70:#71        // getTransformers:()Ljava/util/List;
+  #48 = NameAndType        #19:#20        // this$0:Lsklearn/pipeline/Pipeline;
+  #49 = NameAndType        #21:#72        // "<init>":(Ljava/lang/Class;)V
+  #50 = Utf8               sklearn/SkLearnSteps
+  #51 = Utf8               passthrough
+  #52 = Class              #73            // java/lang/String
+  #53 = NameAndType        #74:#75        // equals:(Ljava/lang/Object;)Z
+  #54 = Class              #76            // sklearn/PassThrough
+  #55 = NameAndType        #77:#78        // INSTANCE:Lsklearn/PassThrough;
+  #56 = NameAndType        #33:#40        // apply:(Ljava/lang/Object;)Ljava/lang/Object;
+  #57 = Utf8               sklearn/Transformer
+  #58 = Utf8               java/lang/StringBuilder
+  #59 = NameAndType        #21:#79        // "<init>":()V
+  #60 = Utf8               The transformer object (
+  #61 = NameAndType        #80:#81        // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #62 = Class              #82            // org/jpmml/python/ClassDictUtil
+  #63 = NameAndType        #83:#39        // formatClass:(Ljava/lang/Object;)Ljava/lang/String;
+  #64 = Utf8               ) is not a supported Transformer
+  #65 = NameAndType        #84:#85        // toString:()Ljava/lang/String;
+  #66 = NameAndType        #33:#34        // apply:(Ljava/lang/Object;)Lsklearn/Transformer;
+  #67 = Utf8               sklearn/pipeline/Pipeline$1
+  #68 = Utf8               org/jpmml/python/CastFunction
+  #69 = Utf8               sklearn/pipeline/Pipeline
+  #70 = Utf8               getTransformers
+  #71 = Utf8               ()Ljava/util/List;
+  #72 = Utf8               (Ljava/lang/Class;)V
+  #73 = Utf8               java/lang/String
+  #74 = Utf8               equals
+  #75 = Utf8               (Ljava/lang/Object;)Z
+  #76 = Utf8               sklearn/PassThrough
+  #77 = Utf8               INSTANCE
+  #78 = Utf8               Lsklearn/PassThrough;
+  #79 = Utf8               ()V
+  #80 = Utf8               append
+  #81 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #82 = Utf8               org/jpmml/python/ClassDictUtil
+  #83 = Utf8               formatClass
+  #84 = Utf8               toString
+  #85 = Utf8               ()Ljava/lang/String;
 {
   final sklearn.pipeline.Pipeline this$0;
     descriptor: Lsklearn/pipeline/Pipeline;
     flags: (0x1010) ACC_FINAL, ACC_SYNTHETIC
 
   sklearn.pipeline.Pipeline$1(sklearn.pipeline.Pipeline, java.lang.Class);
     descriptor: (Lsklearn/pipeline/Pipeline;Ljava/lang/Class;)V
@@ -105,15 +107,15 @@
          1: aload_1
          2: putfield      #1                  // Field this$0:Lsklearn/pipeline/Pipeline;
          5: aload_0
          6: aload_2
          7: invokespecial #2                  // Method org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
         10: return
       LineNumberTable:
-        line 95: 0
+        line 97: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lsklearn/pipeline/Pipeline$1;
             0      11     1 this$0   Lsklearn/pipeline/Pipeline;
             0      11     2    x0   Ljava/lang/Class;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -122,74 +124,74 @@
   public sklearn.Transformer apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Lsklearn/Transformer;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=2, locals=2, args_size=2
          0: aload_1
          1: ifnull        13
-         4: ldc           #3                  // String passthrough
+         4: ldc           #4                  // String passthrough
          6: aload_1
-         7: invokevirtual #4                  // Method java/lang/String.equals:(Ljava/lang/Object;)Z
+         7: invokevirtual #5                  // Method java/lang/String.equals:(Ljava/lang/Object;)Z
         10: ifeq          17
-        13: getstatic     #5                  // Field sklearn/PassThrough.INSTANCE:Lsklearn/PassThrough;
+        13: getstatic     #6                  // Field sklearn/PassThrough.INSTANCE:Lsklearn/PassThrough;
         16: areturn
         17: aload_0
         18: aload_1
-        19: invokespecial #6                  // Method org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
-        22: checkcast     #7                  // class sklearn/Transformer
+        19: invokespecial #7                  // Method org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
+        22: checkcast     #8                  // class sklearn/Transformer
         25: areturn
       LineNumberTable:
-        line 100: 0
-        line 101: 13
-        line 104: 17
+        line 102: 0
+        line 103: 13
+        line 106: 17
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      26     0  this   Lsklearn/pipeline/Pipeline$1;
             0      26     1 object   Ljava/lang/Object;
       StackMapTable: number_of_entries = 2
         frame_type = 13 /* same */
         frame_type = 3 /* same */
 
   public java.lang.String formatMessage(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/String;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=2, locals=2, args_size=2
-         0: new           #8                  // class java/lang/StringBuilder
+         0: new           #9                  // class java/lang/StringBuilder
          3: dup
-         4: invokespecial #9                  // Method java/lang/StringBuilder."<init>":()V
-         7: ldc           #10                 // String The transformer object (
-         9: invokevirtual #11                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+         4: invokespecial #10                 // Method java/lang/StringBuilder."<init>":()V
+         7: ldc           #11                 // String The transformer object (
+         9: invokevirtual #12                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         12: aload_1
-        13: invokestatic  #12                 // Method org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
-        16: invokevirtual #11                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-        19: ldc           #13                 // String ) is not a supported Transformer
-        21: invokevirtual #11                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-        24: invokevirtual #14                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
+        13: invokestatic  #13                 // Method org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
+        16: invokevirtual #12                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+        19: ldc           #14                 // String ) is not a supported Transformer
+        21: invokevirtual #12                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+        24: invokevirtual #15                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
         27: areturn
       LineNumberTable:
-        line 109: 0
+        line 111: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      28     0  this   Lsklearn/pipeline/Pipeline$1;
             0      28     1 object   Ljava/lang/Object;
 
   public java.lang.Object apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/Object;
     flags: (0x1041) ACC_PUBLIC, ACC_BRIDGE, ACC_SYNTHETIC
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
-         2: invokevirtual #15                 // Method apply:(Ljava/lang/Object;)Lsklearn/Transformer;
+         2: invokevirtual #16                 // Method apply:(Ljava/lang/Object;)Lsklearn/Transformer;
          5: areturn
       LineNumberTable:
-        line 95: 0
+        line 97: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/pipeline/Pipeline$1;
 }
-Signature: #41                          // Lorg/jpmml/python/CastFunction<Lsklearn/Transformer;>;
+Signature: #42                          // Lorg/jpmml/python/CastFunction<Lsklearn/Transformer;>;
 SourceFile: "Pipeline.java"
-EnclosingMethod: #45.#46                // sklearn.pipeline.Pipeline.getTransformers
+EnclosingMethod: #46.#47                // sklearn.pipeline.Pipeline.getTransformers
 InnerClasses:
-  #16;                                    // class sklearn/pipeline/Pipeline$1
+  #17;                                    // class sklearn/pipeline/Pipeline$1
```

#### sklearn/pipeline/PipelineClassifier.class

##### procyon -ec {}

```diff
@@ -1,34 +1,45 @@
 
 package sklearn.pipeline;
 
 import sklearn.Transformer;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
-import java.util.List;
 import org.dmg.pmml.DataType;
 import org.dmg.pmml.OpType;
+import java.util.List;
+import sklearn.Proxy;
 import sklearn.HasHead;
 import sklearn.Classifier;
 
-public class PipelineClassifier extends Classifier implements HasHead
+public class PipelineClassifier extends Classifier implements HasHead, Proxy
 {
     private Pipeline pipeline;
     
     public PipelineClassifier(final Pipeline pipeline) {
         super(pipeline.getPythonModule(), pipeline.getPythonName());
         this.pipeline = null;
         this.setPipeline(pipeline);
     }
     
+    public List<String> getFeatureNamesIn() {
+        final Pipeline pipeline = this.getPipeline();
+        return pipeline.getFeatureNamesIn();
+    }
+    
     public int getNumberOfFeatures() {
         final Pipeline pipeline = this.getPipeline();
         return pipeline.getNumberOfFeatures();
     }
     
+    public int getNumberOfOutputs() {
+        final Classifier classifier = this.getFinalClassifier();
+        return classifier.getNumberOfOutputs();
+    }
+    
     public OpType getOpType() {
         final Pipeline pipeline = this.getPipeline();
         return pipeline.getOpType();
     }
     
     public DataType getDataType() {
         final Pipeline pipeline = this.getPipeline();
```

#### sklearn/dummy/DummyClassifier.class

##### procyon -ec {}

```diff
@@ -20,14 +20,18 @@
 import org.jpmml.python.ClassDictUtil;
 import java.util.Collection;
 import sklearn.HasPriorProbability;
 import sklearn.Classifier;
 
 public class DummyClassifier extends Classifier implements HasPriorProbability
 {
+    public DummyClassifier() {
+        this("sklearn.dummy", "DummyClassifier");
+    }
+    
     public DummyClassifier(final String module, final String name) {
         super(module, name);
     }
     
     public Number getPriorProbability(final int index) {
         final List<?> classes = this.getClasses();
         final List<? extends Number> classPrior = this.getClassPrior();
```

#### sklearn/dummy/DummyRegressor.class

##### procyon -ec {}

```diff
@@ -9,14 +9,18 @@
 import java.util.List;
 import com.google.common.collect.Iterables;
 import sklearn.HasDefaultValue;
 import sklearn.Regressor;
 
 public class DummyRegressor extends Regressor implements HasDefaultValue
 {
+    public DummyRegressor() {
+        this("sklearn.dummy", "DummyRegressor");
+    }
+    
     public DummyRegressor(final String module, final String name) {
         super(module, name);
     }
     
     public Number getDefaultValue() {
         final List<? extends Number> constant = this.getConstant();
         return (Number)Iterables.getOnlyElement((Iterable)constant);
```

#### sklearn/SkLearnFields.class

##### procyon -ec {}

```diff
@@ -1,12 +1,13 @@
 
 package sklearn;
 
 public interface SkLearnFields
 {
     public static final String CLASSES = "classes_";
     public static final String FEATURE_IMPORTANCES = "feature_importances_";
+    public static final String FEATURE_NAMES_IN = "feature_names_in_";
     public static final String N_FEATURES = "n_features_";
     public static final String N_FEATURES_IN = "n_features_in_";
     public static final String N_OUTPUTS = "n_outputs_";
     public static final String SKLEARN_VERSION = "_sklearn_version";
 }
```

#### sklearn/Estimator$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 514424329a09acf594bae97a6fb982c696553a1aad76adf2458d561dfb7540d3
+  SHA-256 checksum 47dbbbd886a30764dda53e8a063a005c252f85100531be8ea0950965caebe80d
   Compiled from "Estimator.java"
 class sklearn.Estimator$1
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #8                          // sklearn/Estimator$1
   super_class: #9                         // java/lang/Object
@@ -89,15 +89,15 @@
         54: return
       Exception table:
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
             24    35    38   Class java/lang/NoSuchFieldError
             39    50    53   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 106: 0
+        line 116: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 6
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
```

#### sklearn/Step.class

##### procyon -ec {}

```diff
@@ -1,13 +1,13 @@
 
 package sklearn;
 
 import org.jpmml.python.PythonObject;
 
-public abstract class Step extends PythonObject implements HasNumberOfFeatures, HasType
+public abstract class Step extends PythonObject implements HasFeatureNamesIn, HasNumberOfFeatures, HasType
 {
     public Step(final String module, final String name) {
         super(module, name);
     }
     
     public void checkVersion() {
         final String sklearnVersion = this.getSkLearnVersion();
```

#### sklearn/compose/ColumnTransformer$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,195 +1,197 @@
-  SHA-256 checksum c908d9ad7fa4559381a1709f5cd91e8231c538d8a3b9911d172ca3408a409502
+  SHA-256 checksum 2c55f5a5535f42b469bf7309e9d1ed39aa809c9f8f694ebd2cd8dac6befe7533
   Compiled from "ColumnTransformer.java"
 final class sklearn.compose.ColumnTransformer$1 extends org.jpmml.python.CastFunction<sklearn.Transformer>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
-  this_class: #17                         // sklearn/compose/ColumnTransformer$1
-  super_class: #18                        // org/jpmml/python/CastFunction
+  this_class: #18                         // sklearn/compose/ColumnTransformer$1
+  super_class: #19                        // org/jpmml/python/CastFunction
   interfaces: 0, fields: 0, methods: 4, attributes: 4
 Constant pool:
-   #1 = Methodref          #18.#46        // org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
-   #2 = String             #47            // drop
-   #3 = Methodref          #48.#49        // java/lang/String.equals:(Ljava/lang/Object;)Z
-   #4 = Fieldref           #50.#51        // sklearn/Drop.INSTANCE:Lsklearn/Drop;
-   #5 = String             #52            // passthrough
-   #6 = Fieldref           #53.#54        // sklearn/PassThrough.INSTANCE:Lsklearn/PassThrough;
-   #7 = Methodref          #18.#55        // org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
-   #8 = Class              #56            // sklearn/Transformer
-   #9 = Class              #57            // java/lang/StringBuilder
-  #10 = Methodref          #9.#58         // java/lang/StringBuilder."<init>":()V
-  #11 = String             #59            // The estimator object (
-  #12 = Methodref          #9.#60         // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #13 = Methodref          #61.#62        // org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
-  #14 = String             #63            // ) is not a supported Transformer
-  #15 = Methodref          #9.#64         // java/lang/StringBuilder.toString:()Ljava/lang/String;
-  #16 = Methodref          #17.#65        // sklearn/compose/ColumnTransformer$1.apply:(Ljava/lang/Object;)Lsklearn/Transformer;
-  #17 = Class              #66            // sklearn/compose/ColumnTransformer$1
-  #18 = Class              #67            // org/jpmml/python/CastFunction
-  #19 = Utf8               <init>
-  #20 = Utf8               (Ljava/lang/Class;)V
-  #21 = Utf8               Code
-  #22 = Utf8               LineNumberTable
-  #23 = Utf8               LocalVariableTable
-  #24 = Utf8               this
-  #25 = Utf8               InnerClasses
-  #26 = Utf8               Lsklearn/compose/ColumnTransformer$1;
-  #27 = Utf8               x0
-  #28 = Utf8               Ljava/lang/Class;
-  #29 = Utf8               LocalVariableTypeTable
-  #30 = Utf8               Ljava/lang/Class<+Lsklearn/Transformer;>;
-  #31 = Utf8               apply
-  #32 = Utf8               (Ljava/lang/Object;)Lsklearn/Transformer;
-  #33 = Utf8               object
-  #34 = Utf8               Ljava/lang/Object;
-  #35 = Utf8               StackMapTable
-  #36 = Utf8               formatMessage
-  #37 = Utf8               (Ljava/lang/Object;)Ljava/lang/String;
-  #38 = Utf8               (Ljava/lang/Object;)Ljava/lang/Object;
-  #39 = Utf8               Signature
-  #40 = Utf8               Lorg/jpmml/python/CastFunction<Lsklearn/Transformer;>;
-  #41 = Utf8               SourceFile
-  #42 = Utf8               ColumnTransformer.java
-  #43 = Utf8               EnclosingMethod
-  #44 = Class              #68            // sklearn/compose/ColumnTransformer
-  #45 = NameAndType        #69:#70        // getTransformer:([Ljava/lang/Object;)Lsklearn/Transformer;
-  #46 = NameAndType        #19:#20        // "<init>":(Ljava/lang/Class;)V
-  #47 = Utf8               drop
-  #48 = Class              #71            // java/lang/String
-  #49 = NameAndType        #72:#73        // equals:(Ljava/lang/Object;)Z
-  #50 = Class              #74            // sklearn/Drop
-  #51 = NameAndType        #75:#76        // INSTANCE:Lsklearn/Drop;
-  #52 = Utf8               passthrough
-  #53 = Class              #77            // sklearn/PassThrough
-  #54 = NameAndType        #75:#78        // INSTANCE:Lsklearn/PassThrough;
-  #55 = NameAndType        #31:#38        // apply:(Ljava/lang/Object;)Ljava/lang/Object;
-  #56 = Utf8               sklearn/Transformer
-  #57 = Utf8               java/lang/StringBuilder
-  #58 = NameAndType        #19:#79        // "<init>":()V
-  #59 = Utf8               The estimator object (
-  #60 = NameAndType        #80:#81        // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #61 = Class              #82            // org/jpmml/python/ClassDictUtil
-  #62 = NameAndType        #83:#37        // formatClass:(Ljava/lang/Object;)Ljava/lang/String;
-  #63 = Utf8               ) is not a supported Transformer
-  #64 = NameAndType        #84:#85        // toString:()Ljava/lang/String;
-  #65 = NameAndType        #31:#32        // apply:(Ljava/lang/Object;)Lsklearn/Transformer;
-  #66 = Utf8               sklearn/compose/ColumnTransformer$1
-  #67 = Utf8               org/jpmml/python/CastFunction
-  #68 = Utf8               sklearn/compose/ColumnTransformer
-  #69 = Utf8               getTransformer
-  #70 = Utf8               ([Ljava/lang/Object;)Lsklearn/Transformer;
-  #71 = Utf8               java/lang/String
-  #72 = Utf8               equals
-  #73 = Utf8               (Ljava/lang/Object;)Z
-  #74 = Utf8               sklearn/Drop
-  #75 = Utf8               INSTANCE
-  #76 = Utf8               Lsklearn/Drop;
-  #77 = Utf8               sklearn/PassThrough
-  #78 = Utf8               Lsklearn/PassThrough;
-  #79 = Utf8               ()V
-  #80 = Utf8               append
-  #81 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #82 = Utf8               org/jpmml/python/ClassDictUtil
-  #83 = Utf8               formatClass
-  #84 = Utf8               toString
-  #85 = Utf8               ()Ljava/lang/String;
+   #1 = Methodref          #19.#47        // org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
+   #2 = Class              #48            // sklearn/SkLearnSteps
+   #3 = String             #49            // drop
+   #4 = Methodref          #50.#51        // java/lang/String.equals:(Ljava/lang/Object;)Z
+   #5 = Fieldref           #52.#53        // sklearn/Drop.INSTANCE:Lsklearn/Drop;
+   #6 = String             #54            // passthrough
+   #7 = Fieldref           #55.#56        // sklearn/PassThrough.INSTANCE:Lsklearn/PassThrough;
+   #8 = Methodref          #19.#57        // org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
+   #9 = Class              #58            // sklearn/Transformer
+  #10 = Class              #59            // java/lang/StringBuilder
+  #11 = Methodref          #10.#60        // java/lang/StringBuilder."<init>":()V
+  #12 = String             #61            // The estimator object (
+  #13 = Methodref          #10.#62        // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #14 = Methodref          #63.#64        // org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
+  #15 = String             #65            // ) is not a supported Transformer
+  #16 = Methodref          #10.#66        // java/lang/StringBuilder.toString:()Ljava/lang/String;
+  #17 = Methodref          #18.#67        // sklearn/compose/ColumnTransformer$1.apply:(Ljava/lang/Object;)Lsklearn/Transformer;
+  #18 = Class              #68            // sklearn/compose/ColumnTransformer$1
+  #19 = Class              #69            // org/jpmml/python/CastFunction
+  #20 = Utf8               <init>
+  #21 = Utf8               (Ljava/lang/Class;)V
+  #22 = Utf8               Code
+  #23 = Utf8               LineNumberTable
+  #24 = Utf8               LocalVariableTable
+  #25 = Utf8               this
+  #26 = Utf8               InnerClasses
+  #27 = Utf8               Lsklearn/compose/ColumnTransformer$1;
+  #28 = Utf8               x0
+  #29 = Utf8               Ljava/lang/Class;
+  #30 = Utf8               LocalVariableTypeTable
+  #31 = Utf8               Ljava/lang/Class<+Lsklearn/Transformer;>;
+  #32 = Utf8               apply
+  #33 = Utf8               (Ljava/lang/Object;)Lsklearn/Transformer;
+  #34 = Utf8               object
+  #35 = Utf8               Ljava/lang/Object;
+  #36 = Utf8               StackMapTable
+  #37 = Utf8               formatMessage
+  #38 = Utf8               (Ljava/lang/Object;)Ljava/lang/String;
+  #39 = Utf8               (Ljava/lang/Object;)Ljava/lang/Object;
+  #40 = Utf8               Signature
+  #41 = Utf8               Lorg/jpmml/python/CastFunction<Lsklearn/Transformer;>;
+  #42 = Utf8               SourceFile
+  #43 = Utf8               ColumnTransformer.java
+  #44 = Utf8               EnclosingMethod
+  #45 = Class              #70            // sklearn/compose/ColumnTransformer
+  #46 = NameAndType        #71:#72        // getTransformer:([Ljava/lang/Object;)Lsklearn/Transformer;
+  #47 = NameAndType        #20:#21        // "<init>":(Ljava/lang/Class;)V
+  #48 = Utf8               sklearn/SkLearnSteps
+  #49 = Utf8               drop
+  #50 = Class              #73            // java/lang/String
+  #51 = NameAndType        #74:#75        // equals:(Ljava/lang/Object;)Z
+  #52 = Class              #76            // sklearn/Drop
+  #53 = NameAndType        #77:#78        // INSTANCE:Lsklearn/Drop;
+  #54 = Utf8               passthrough
+  #55 = Class              #79            // sklearn/PassThrough
+  #56 = NameAndType        #77:#80        // INSTANCE:Lsklearn/PassThrough;
+  #57 = NameAndType        #32:#39        // apply:(Ljava/lang/Object;)Ljava/lang/Object;
+  #58 = Utf8               sklearn/Transformer
+  #59 = Utf8               java/lang/StringBuilder
+  #60 = NameAndType        #20:#81        // "<init>":()V
+  #61 = Utf8               The estimator object (
+  #62 = NameAndType        #82:#83        // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #63 = Class              #84            // org/jpmml/python/ClassDictUtil
+  #64 = NameAndType        #85:#38        // formatClass:(Ljava/lang/Object;)Ljava/lang/String;
+  #65 = Utf8               ) is not a supported Transformer
+  #66 = NameAndType        #86:#87        // toString:()Ljava/lang/String;
+  #67 = NameAndType        #32:#33        // apply:(Ljava/lang/Object;)Lsklearn/Transformer;
+  #68 = Utf8               sklearn/compose/ColumnTransformer$1
+  #69 = Utf8               org/jpmml/python/CastFunction
+  #70 = Utf8               sklearn/compose/ColumnTransformer
+  #71 = Utf8               getTransformer
+  #72 = Utf8               ([Ljava/lang/Object;)Lsklearn/Transformer;
+  #73 = Utf8               java/lang/String
+  #74 = Utf8               equals
+  #75 = Utf8               (Ljava/lang/Object;)Z
+  #76 = Utf8               sklearn/Drop
+  #77 = Utf8               INSTANCE
+  #78 = Utf8               Lsklearn/Drop;
+  #79 = Utf8               sklearn/PassThrough
+  #80 = Utf8               Lsklearn/PassThrough;
+  #81 = Utf8               ()V
+  #82 = Utf8               append
+  #83 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #84 = Utf8               org/jpmml/python/ClassDictUtil
+  #85 = Utf8               formatClass
+  #86 = Utf8               toString
+  #87 = Utf8               ()Ljava/lang/String;
 {
   sklearn.compose.ColumnTransformer$1(java.lang.Class);
     descriptor: (Ljava/lang/Class;)V
     flags: (0x0000)
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokespecial #1                  // Method org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
          5: return
       LineNumberTable:
-        line 75: 0
+        line 76: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/compose/ColumnTransformer$1;
             0       6     1    x0   Ljava/lang/Class;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0       6     1    x0   Ljava/lang/Class<+Lsklearn/Transformer;>;
 
   public sklearn.Transformer apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Lsklearn/Transformer;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=2, locals=2, args_size=2
-         0: ldc           #2                  // String drop
+         0: ldc           #3                  // String drop
          2: aload_1
-         3: invokevirtual #3                  // Method java/lang/String.equals:(Ljava/lang/Object;)Z
+         3: invokevirtual #4                  // Method java/lang/String.equals:(Ljava/lang/Object;)Z
          6: ifeq          13
-         9: getstatic     #4                  // Field sklearn/Drop.INSTANCE:Lsklearn/Drop;
+         9: getstatic     #5                  // Field sklearn/Drop.INSTANCE:Lsklearn/Drop;
         12: areturn
-        13: ldc           #5                  // String passthrough
+        13: ldc           #6                  // String passthrough
         15: aload_1
-        16: invokevirtual #3                  // Method java/lang/String.equals:(Ljava/lang/Object;)Z
+        16: invokevirtual #4                  // Method java/lang/String.equals:(Ljava/lang/Object;)Z
         19: ifeq          26
-        22: getstatic     #6                  // Field sklearn/PassThrough.INSTANCE:Lsklearn/PassThrough;
+        22: getstatic     #7                  // Field sklearn/PassThrough.INSTANCE:Lsklearn/PassThrough;
         25: areturn
         26: aload_0
         27: aload_1
-        28: invokespecial #7                  // Method org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
-        31: checkcast     #8                  // class sklearn/Transformer
+        28: invokespecial #8                  // Method org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
+        31: checkcast     #9                  // class sklearn/Transformer
         34: areturn
       LineNumberTable:
-        line 80: 0
-        line 81: 9
-        line 84: 13
-        line 85: 22
-        line 88: 26
+        line 81: 0
+        line 82: 9
+        line 85: 13
+        line 86: 22
+        line 89: 26
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      35     0  this   Lsklearn/compose/ColumnTransformer$1;
             0      35     1 object   Ljava/lang/Object;
       StackMapTable: number_of_entries = 2
         frame_type = 13 /* same */
         frame_type = 12 /* same */
 
   protected java.lang.String formatMessage(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/String;
     flags: (0x0004) ACC_PROTECTED
     Code:
       stack=2, locals=2, args_size=2
-         0: new           #9                  // class java/lang/StringBuilder
+         0: new           #10                 // class java/lang/StringBuilder
          3: dup
-         4: invokespecial #10                 // Method java/lang/StringBuilder."<init>":()V
-         7: ldc           #11                 // String The estimator object (
-         9: invokevirtual #12                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+         4: invokespecial #11                 // Method java/lang/StringBuilder."<init>":()V
+         7: ldc           #12                 // String The estimator object (
+         9: invokevirtual #13                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         12: aload_1
-        13: invokestatic  #13                 // Method org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
-        16: invokevirtual #12                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-        19: ldc           #14                 // String ) is not a supported Transformer
-        21: invokevirtual #12                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-        24: invokevirtual #15                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
+        13: invokestatic  #14                 // Method org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
+        16: invokevirtual #13                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+        19: ldc           #15                 // String ) is not a supported Transformer
+        21: invokevirtual #13                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+        24: invokevirtual #16                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
         27: areturn
       LineNumberTable:
-        line 93: 0
+        line 94: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      28     0  this   Lsklearn/compose/ColumnTransformer$1;
             0      28     1 object   Ljava/lang/Object;
 
   public java.lang.Object apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/Object;
     flags: (0x1041) ACC_PUBLIC, ACC_BRIDGE, ACC_SYNTHETIC
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
-         2: invokevirtual #16                 // Method apply:(Ljava/lang/Object;)Lsklearn/Transformer;
+         2: invokevirtual #17                 // Method apply:(Ljava/lang/Object;)Lsklearn/Transformer;
          5: areturn
       LineNumberTable:
-        line 75: 0
+        line 76: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/compose/ColumnTransformer$1;
 }
-Signature: #40                          // Lorg/jpmml/python/CastFunction<Lsklearn/Transformer;>;
+Signature: #41                          // Lorg/jpmml/python/CastFunction<Lsklearn/Transformer;>;
 SourceFile: "ColumnTransformer.java"
-EnclosingMethod: #44.#45                // sklearn.compose.ColumnTransformer.getTransformer
+EnclosingMethod: #45.#46                // sklearn.compose.ColumnTransformer.getTransformer
 InnerClasses:
-  static #17;                             // class sklearn/compose/ColumnTransformer$1
+  static #18;                             // class sklearn/compose/ColumnTransformer$1
```

#### sklearn/compose/ColumnTransformer.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum aad1515d46585761ada44dc878812b8eccf235db1894afd965a6dd1423a75d47
+  SHA-256 checksum 21fe02d01cc832cd040f55f233889345cfd185680002c4b31b712a92a7ae333d
   Compiled from "ColumnTransformer.java"
 public class sklearn.compose.ColumnTransformer extends sklearn.Initializer
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #29                         // sklearn/compose/ColumnTransformer
   super_class: #30                        // sklearn/Initializer
@@ -162,16 +162,16 @@
       stack=3, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: aload_2
          3: invokespecial #1                  // Method sklearn/Initializer."<init>":(Ljava/lang/String;Ljava/lang/String;)V
          6: return
       LineNumberTable:
-        line 40: 0
-        line 41: 6
+        line 41: 0
+        line 42: 6
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lsklearn/compose/ColumnTransformer;
             0       7     1 module   Ljava/lang/String;
             0       7     2  name   Ljava/lang/String;
 
   public java.util.List<org.jpmml.converter.Feature> initializeFeatures(org.jpmml.sklearn.SkLearnEncoder);
@@ -181,15 +181,15 @@
       stack=3, locals=2, args_size=2
          0: aload_0
          1: invokestatic  #2                  // Method java/util/Collections.emptyList:()Ljava/util/List;
          4: aload_1
          5: invokevirtual #3                  // Method encodeFeatures:(Ljava/util/List;Lorg/jpmml/sklearn/SkLearnEncoder;)Ljava/util/List;
          8: areturn
       LineNumberTable:
-        line 45: 0
+        line 46: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lsklearn/compose/ColumnTransformer;
             0       9     1 encoder   Lorg/jpmml/sklearn/SkLearnEncoder;
     Signature: #47                          // (Lorg/jpmml/sklearn/SkLearnEncoder;)Ljava/util/List<Lorg/jpmml/converter/Feature;>;
 
   public java.util.List<org.jpmml.converter.Feature> encodeFeatures(java.util.List<org.jpmml.converter.Feature>, org.jpmml.sklearn.SkLearnEncoder);
@@ -231,23 +231,23 @@
         72: aload         8
         74: invokeinterface #14,  2           // InterfaceMethod java/util/List.addAll:(Ljava/util/Collection;)Z
         79: pop
         80: goto          22
         83: aload         4
         85: areturn
       LineNumberTable:
-        line 50: 0
-        line 52: 5
-        line 54: 14
-        line 55: 44
-        line 57: 51
-        line 59: 60
-        line 61: 70
-        line 62: 80
-        line 64: 83
+        line 51: 0
+        line 53: 5
+        line 55: 14
+        line 56: 44
+        line 58: 51
+        line 60: 60
+        line 62: 70
+        line 63: 80
+        line 65: 83
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            51      29     7 transformer   Lsklearn/Transformer;
            60      20     8 rowFeatures   Ljava/util/List;
            44      36     6 fittedTransformer   [Ljava/lang/Object;
             0      86     0  this   Lsklearn/compose/ColumnTransformer;
             0      86     1 features   Ljava/util/List;
@@ -274,15 +274,15 @@
     Code:
       stack=2, locals=1, args_size=1
          0: aload_0
          1: ldc           #15                 // String transformers_
          3: invokevirtual #16                 // Method getTupleList:(Ljava/lang/String;)Ljava/util/List;
          6: areturn
       LineNumberTable:
-        line 68: 0
+        line 69: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lsklearn/compose/ColumnTransformer;
     Signature: #68                          // ()Ljava/util/List<[Ljava/lang/Object;>;
 
   private static sklearn.Transformer getTransformer(java.lang.Object[]);
     descriptor: ([Ljava/lang/Object;)Lsklearn/Transformer;
@@ -300,17 +300,17 @@
         15: astore_2
         16: aload_2
         17: aload_1
         18: invokevirtual #21                 // Method org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
         21: checkcast     #19                 // class sklearn/Transformer
         24: areturn
       LineNumberTable:
-        line 73: 0
-        line 75: 6
-        line 97: 16
+        line 74: 0
+        line 76: 6
+        line 98: 16
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      25     0 fittedTransformer   [Ljava/lang/Object;
             6      19     1 transformer   Ljava/lang/Object;
            16       9     2 castFunction   Lorg/jpmml/python/CastFunction;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -347,21 +347,21 @@
         49: aload_3
         50: checkcast     #27                 // class java/util/List
         53: aload_1
         54: aload_2
         55: invokestatic  #28                 // Method sklearn/InitializerUtil.selectFeatures:(Ljava/util/List;Ljava/util/List;Lorg/jpmml/sklearn/SkLearnEncoder;)Ljava/util/List;
         58: areturn
       LineNumberTable:
-        line 102: 0
-        line 104: 6
-        line 105: 20
-        line 108: 28
-        line 109: 35
-        line 111: 41
-        line 114: 49
+        line 103: 0
+        line 105: 6
+        line 106: 20
+        line 109: 28
+        line 110: 35
+        line 112: 41
+        line 115: 49
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            41       8     4 hasArray   Lorg/jpmml/python/HasArray;
             0      59     0 fittedTransformer   [Ljava/lang/Object;
             0      59     1 features   Ljava/util/List;
             0      59     2 encoder   Lorg/jpmml/sklearn/SkLearnEncoder;
             6      53     3 columns   Ljava/lang/Object;
```

#### sklearn/Transformer$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 9ff1e426db45933a0039028b9b1e967bdee0d5b23bbceb880af41c6b4589767a
+  SHA-256 checksum 1f93d9e0ef7978f72d144440fbd4f2c82cc2797685ac28a424a70d444ff6734d
   Compiled from "Transformer.java"
 class sklearn.Transformer$1 extends org.jpmml.python.CastFunction<org.jpmml.python.TypeInfo>
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #20                         // sklearn/Transformer$1
   super_class: #21                        // org/jpmml/python/CastFunction
@@ -130,15 +130,15 @@
         11: aload         4
         13: putfield      #3                  // Field val$name:Ljava/lang/String;
         16: aload_0
         17: aload_2
         18: invokespecial #4                  // Method org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
         21: return
       LineNumberTable:
-        line 156: 0
+        line 166: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      22     0  this   Lsklearn/Transformer$1;
             0      22     1 this$0   Lsklearn/Transformer;
             0      22     2    x0   Ljava/lang/Class;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -176,22 +176,22 @@
         48: areturn
         49: aload_0
         50: aload_1
         51: invokespecial #11                 // Method org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
         54: checkcast     #7                  // class org/jpmml/python/TypeInfo
         57: areturn
       LineNumberTable:
-        line 161: 0
-        line 162: 7
-        line 164: 12
-        line 167: 20
-        line 168: 27
-        line 170: 32
-        line 171: 39
-        line 181: 49
+        line 171: 0
+        line 172: 7
+        line 174: 12
+        line 177: 20
+        line 178: 27
+        line 180: 32
+        line 181: 39
+        line 191: 49
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            12       8     2 typeConstructor   Lbuiltins/TypeConstructor;
            32      17     2 string   Ljava/lang/String;
             0      58     0  this   Lsklearn/Transformer$1;
             0      58     1 object   Ljava/lang/Object;
       StackMapTable: number_of_entries = 2
@@ -215,15 +215,15 @@
         20: invokestatic  #16                 // Method org/jpmml/python/ClassDictUtil.formatMember:(Lnet/razorvine/pickle/objects/ClassDict;Ljava/lang/String;)Ljava/lang/String;
         23: invokevirtual #15                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         26: ldc           #17                 // String ) is not a supported type info
         28: invokevirtual #15                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         31: invokevirtual #18                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
         34: areturn
       LineNumberTable:
-        line 186: 0
+        line 196: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      35     0  this   Lsklearn/Transformer$1;
             0      35     1 object   Ljava/lang/Object;
 
   public java.lang.Object apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/Object;
@@ -231,15 +231,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #19                 // Method apply:(Ljava/lang/Object;)Lorg/jpmml/python/TypeInfo;
          5: areturn
       LineNumberTable:
-        line 156: 0
+        line 166: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/Transformer$1;
 }
 Signature: #52                          // Lorg/jpmml/python/CastFunction<Lorg/jpmml/python/TypeInfo;>;
 SourceFile: "Transformer.java"
 EnclosingMethod: #56.#57                // sklearn.Transformer.getDType
```

#### sklearn/feature_extraction/DictVectorizer.class

##### procyon -ec {}

```diff
@@ -59,15 +59,15 @@
             featureArray[(int)Integer.valueOf(vocabulary.get((Object)featureName))] = feature;
         }
         final List<Feature> result = new ArrayList<Feature>();
         result.addAll(Arrays.asList(featureArray));
         return result;
     }
     
-    public List<? extends String> getFeatureNames() {
+    public List<String> getFeatureNames() {
         return this.getList("feature_names_", (Class)String.class);
     }
     
     public String getSeparator() {
         return this.getString("separator");
     }
```

#### sklearn/Transformer.class

##### procyon -ec {}

```diff
@@ -20,14 +20,21 @@
 {
     public Transformer(final String module, final String name) {
         super(module, name);
     }
     
     public abstract List<Feature> encodeFeatures(final List<Feature> p0, final SkLearnEncoder p1);
     
+    public List<String> getFeatureNamesIn() {
+        if (this.containsKey((Object)"feature_names_in_")) {
+            return this.getArray("feature_names_in_", (Class)String.class);
+        }
+        return null;
+    }
+    
     public int getNumberOfFeatures() {
         if (this.containsKey((Object)"n_features_in_")) {
             return this.getInteger("n_features_in_");
         }
         return -1;
     }
```

#### sklearn/Transformer$1$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum ea81f21f596f9bcf568251a711b9c7d2c58fdacadb36471b89449dfd04aa6d49
+  SHA-256 checksum e7dd1d54cee72ced261dfbed9f3699afd23a13b6879a46a7336a997f0a15c179
   Compiled from "Transformer.java"
 class sklearn.Transformer$1$1 implements org.jpmml.python.TypeInfo
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #5                          // sklearn/Transformer$1$1
   super_class: #6                         // java/lang/Object
@@ -69,15 +69,15 @@
          5: aload_0
          6: aload_2
          7: putfield      #2                  // Field val$string:Ljava/lang/String;
         10: aload_0
         11: invokespecial #3                  // Method java/lang/Object."<init>":()V
         14: return
       LineNumberTable:
-        line 171: 0
+        line 181: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0  this   Lsklearn/Transformer$1$1;
             0      15     1 this$1   Lsklearn/Transformer$1;
 
   public org.dmg.pmml.DataType getDataType();
     descriptor: ()Lorg/dmg/pmml/DataType;
@@ -85,15 +85,15 @@
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #2                  // Field val$string:Ljava/lang/String;
          4: invokestatic  #4                  // Method org/jpmml/python/PythonTypeUtil.parseDataType:(Ljava/lang/String;)Lorg/dmg/pmml/DataType;
          7: areturn
       LineNumberTable:
-        line 175: 0
+        line 185: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lsklearn/Transformer$1$1;
 }
 SourceFile: "Transformer.java"
 EnclosingMethod: #11.#26                // sklearn.Transformer$1.apply
 InnerClasses:
```

#### sklearn/Transformer$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum aae937205b5f0178af34d94614c4ac3f26adb42bfd46ddefe671f3c92c7a6f4e
+  SHA-256 checksum 5920265519511cc9060bed7bafef6f38148fae016579adf8827c9e893830e810
   Compiled from "Transformer.java"
 class sklearn.Transformer$2
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #6                          // sklearn/Transformer$2
   super_class: #7                         // java/lang/Object
@@ -67,15 +67,15 @@
         20: goto          24
         23: astore_0
         24: return
       Exception table:
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 127: 0
+        line 137: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 2
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
 }
```

#### sklearn/Composite.class

##### procyon -ec {}

```diff
@@ -4,16 +4,16 @@
 import org.jpmml.converter.Label;
 import org.jpmml.converter.PMMLEncoder;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
 import org.jpmml.sklearn.SkLearnEncoder;
 import org.jpmml.converter.Feature;
 import org.dmg.pmml.DataType;
-import java.util.Iterator;
 import org.dmg.pmml.OpType;
+import java.util.Iterator;
 import java.util.List;
 
 public abstract class Composite extends Step
 {
     public Composite(final String module, final String name) {
         super(module, name);
     }
@@ -22,14 +22,30 @@
     
     public abstract List<? extends Transformer> getTransformers();
     
     public abstract boolean hasFinalEstimator();
     
     public abstract Estimator getFinalEstimator();
     
+    public List<String> getFeatureNamesIn() {
+        if (this.hasTransformers()) {
+            final List<? extends Transformer> transformers = this.getTransformers();
+            final Iterator<? extends Transformer> iterator = transformers.iterator();
+            if (iterator.hasNext()) {
+                final Transformer transformer = (Transformer)iterator.next();
+                return transformer.getFeatureNamesIn();
+            }
+        }
+        if (this.hasFinalEstimator()) {
+            final Estimator estimator = this.getFinalEstimator();
+            return estimator.getFeatureNamesIn();
+        }
+        return null;
+    }
+    
     public int getNumberOfFeatures() {
         if (this.hasTransformers()) {
             final List<? extends Transformer> transformers = this.getTransformers();
             return StepUtil.getNumberOfFeatures((List)transformers);
         }
         if (this.hasFinalEstimator()) {
             final Estimator estimator = this.getFinalEstimator();
@@ -79,20 +95,25 @@
             features = transformer.encode((List)features, encoder);
         }
         return features;
     }
     
     public Model encodeModel(Schema schema) {
         final SkLearnEncoder encoder = (SkLearnEncoder)schema.getEncoder();
-        final Label label = schema.getLabel();
+        Label label = schema.getLabel();
         List<? extends Feature> features = schema.getFeatures();
         if (this.hasTransformers()) {
             features = this.encodeFeatures((List<Feature>)features, encoder);
+            label = this.refreshLabel(label, encoder);
             schema = new Schema((PMMLEncoder)encoder, label, (List)features);
         }
         if (this.hasFinalEstimator()) {
             final Estimator estimator = this.getFinalEstimator();
             return estimator.encode(schema);
         }
         throw new UnsupportedOperationException();
     }
+    
+    protected Label refreshLabel(final Label label, final SkLearnEncoder encoder) {
+        return label;
+    }
 }
```

#### sklearn/Estimator.class

##### procyon -ec {}

```diff
@@ -17,17 +17,17 @@
 import java.util.Map;
 import net.razorvine.pickle.objects.ClassDict;
 import org.jpmml.python.ClassDictUtil;
 import java.util.Collection;
 import org.jpmml.converter.ModelEncoder;
 import org.jpmml.converter.Label;
 import org.jpmml.converter.Feature;
-import java.util.List;
 import org.dmg.pmml.DataType;
 import org.dmg.pmml.OpType;
+import java.util.List;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
 import org.dmg.pmml.MiningFunction;
 import org.slf4j.Logger;
 
 public abstract class Estimator extends Step implements HasNumberOfOutputs
 {
@@ -40,14 +40,21 @@
         super(module, name);
     }
     
     public abstract MiningFunction getMiningFunction();
     
     public abstract Model encodeModel(final Schema p0);
     
+    public List<String> getFeatureNamesIn() {
+        if (this.containsKey((Object)"feature_names_in_")) {
+            return this.getArray("feature_names_in_", (Class)String.class);
+        }
+        return null;
+    }
+    
     public int getNumberOfFeatures() {
         if (this.containsKey((Object)"n_features_in_") && this.get((Object)"n_features_in_") != null) {
             return this.getInteger("n_features_in_");
         }
         if (this.containsKey((Object)"n_features_")) {
             return this.getInteger("n_features_");
         }
```

#### sklearn2pmml/pipeline/PMMLPipeline$3.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum bb91048635043df9a6f259644251783b70250545cd05ec7efc19c20274d5d273
+  SHA-256 checksum 572b3193c38934b75fa208b24f1365819741f1268017177b3cdc4f63aa233ca9
   Compiled from "PMMLPipeline.java"
 final class sklearn2pmml.pipeline.PMMLPipeline$3 extends java.lang.Object implements com.google.common.base.Function<java.lang.Object, java.lang.Object>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #4                          // sklearn2pmml/pipeline/PMMLPipeline$3
   super_class: #5                         // java/lang/Object
@@ -56,15 +56,15 @@
     flags: (0x0000)
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 712: 0
+        line 717: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$3;
 
   public java.lang.Object apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/Object;
     flags: (0x0001) ACC_PUBLIC
@@ -77,18 +77,18 @@
          6: invokestatic  #3                  // Method org/jpmml/converter/ValueUtil.isNaN:(Ljava/lang/Object;)Z
          9: ifeq          14
         12: aconst_null
         13: areturn
         14: aload_1
         15: areturn
       LineNumberTable:
-        line 716: 0
-        line 718: 5
-        line 719: 12
-        line 722: 14
+        line 721: 0
+        line 723: 5
+        line 724: 12
+        line 727: 14
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$3;
             0      16     1 value   Ljava/lang/Object;
       StackMapTable: number_of_entries = 1
         frame_type = 14 /* same */
 }
```

#### sklearn2pmml/pipeline/PMMLPipeline$4.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum bef47cfdfdf636c1139448c8bdcf1434889acbca4eecfd581e87745513e43406
+  SHA-256 checksum 95ff94f650595d2fb6ef2af9dd77ccfbec9a253afe6fe705c22a950889aff80c
   Compiled from "PMMLPipeline.java"
 class sklearn2pmml.pipeline.PMMLPipeline$4
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #13                         // sklearn2pmml/pipeline/PMMLPipeline$4
   super_class: #14                        // java/lang/Object
@@ -129,16 +129,16 @@
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
             24    35    38   Class java/lang/NoSuchFieldError
             39    50    53   Class java/lang/NoSuchFieldError
             63    74    77   Class java/lang/NoSuchFieldError
             78    89    92   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 566: 0
-        line 332: 54
+        line 571: 0
+        line 333: 54
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 10
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
```

#### sklearn2pmml/pipeline/PMMLPipeline.class

##### procyon -ec {}

```diff
@@ -292,16 +292,15 @@
     }
     
     public List<Object[]> getSteps() {
         return super.getSteps();
     }
     
     public PMMLPipeline setSteps(final List<Object[]> steps) {
-        this.put((Object)"steps", (Object)steps);
-        return this;
+        return (PMMLPipeline)super.setSteps((List)steps);
     }
     
     public Map<?, ?> getHeader() {
         return (Map)this.getOptional("header", (Class)Map.class);
     }
     
     public List<? extends Number> getPMMLFeatureImportances() {
@@ -369,15 +368,19 @@
     
     public PMMLPipeline setVerification(final Verification verification) {
         this.put((Object)"verification", (Object)verification);
         return this;
     }
     
     private List<String> initActiveFields(final Step step) {
+        final List<String> featureNamesIn = step.getFeatureNamesIn();
         final int numberOfFeatures = step.getNumberOfFeatures();
+        if (featureNamesIn != null) {
+            return featureNamesIn;
+        }
         if (numberOfFeatures == -1) {
             throw new IllegalArgumentException("The transformer object of the first step (" + ClassDictUtil.formatClass((Object)step) + ") does not specify the number of input features");
         }
         final List<String> activeFields = makeVariables("x", numberOfFeatures, true);
         PMMLPipeline.logger.warn("Attribute '" + ClassDictUtil.formatMember((ClassDict)this, "active_fields") + "' is not set. Assuming {} as the names of active fields", (Object)activeFields);
         return activeFields;
     }
```

#### sklearn2pmml/pipeline/PMMLPipeline$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 479d50341cf68c4df4880fe0f59a0804eee638c39586dff3e7b943d86d92c3e2
+  SHA-256 checksum eb0ca6cf9c387cae56fae3aadff956e8b28d6fc40c57c4d2239af16f777cc8c8
   Compiled from "PMMLPipeline.java"
 final class sklearn2pmml.pipeline.PMMLPipeline$2 extends org.jpmml.converter.visitors.AbstractExtender
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #9                          // sklearn2pmml/pipeline/PMMLPipeline$2
   super_class: #10                        // org/jpmml/converter/visitors/AbstractExtender
@@ -89,15 +89,15 @@
          1: aload_2
          2: putfield      #1                  // Field val$values:Ljava/util/Map;
          5: aload_0
          6: aload_1
          7: invokespecial #2                  // Method org/jpmml/converter/visitors/AbstractExtender."<init>":(Ljava/lang/String;)V
         10: return
       LineNumberTable:
-        line 663: 0
+        line 668: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$2;
             0      11     1    x0   Ljava/lang/String;
 
   public org.dmg.pmml.VisitorAction visit(org.dmg.pmml.Value);
     descriptor: (Lorg/dmg/pmml/Value;)Lorg/dmg/pmml/VisitorAction;
@@ -121,19 +121,19 @@
         26: invokestatic  #6                  // Method org/jpmml/converter/ValueUtil.asString:(Ljava/lang/Object;)Ljava/lang/String;
         29: invokevirtual #7                  // Method addExtension:(Lorg/dmg/pmml/PMMLObject;Ljava/lang/String;)V
         32: aload_0
         33: aload_1
         34: invokespecial #8                  // Method org/jpmml/converter/visitors/AbstractExtender.visit:(Lorg/dmg/pmml/Value;)Lorg/dmg/pmml/VisitorAction;
         37: areturn
       LineNumberTable:
-        line 667: 0
-        line 669: 14
-        line 670: 18
-        line 672: 23
-        line 675: 32
+        line 672: 0
+        line 674: 14
+        line 675: 18
+        line 677: 23
+        line 680: 32
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      38     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$2;
             0      38     1 pmmlValue   Lorg/dmg/pmml/Value;
            14      24     2 value   Ljava/lang/Object;
       StackMapTable: number_of_entries = 1
         frame_type = 252 /* append */
```

#### sklearn2pmml/pipeline/PMMLPipeline$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 26d012e00007fbd21a2827d02d03a2990201ec0e642f0ed850961aab8e0e810d
+  SHA-256 checksum 8e06ac2621148ef2f077c68371e735e95127dcc9f1c3a18e1aa0a351c66670a5
   Compiled from "PMMLPipeline.java"
 final class sklearn2pmml.pipeline.PMMLPipeline$1 extends org.jpmml.python.CastFunction<java.util.List<?>>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #11                         // sklearn2pmml/pipeline/PMMLPipeline$1
   super_class: #12                        // org/jpmml/python/CastFunction
@@ -83,15 +83,15 @@
          1: aload_2
          2: putfield      #1                  // Field val$targetField:Ljava/lang/String;
          5: aload_0
          6: aload_1
          7: invokespecial #2                  // Method org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
         10: return
       LineNumberTable:
-        line 587: 0
+        line 592: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$1;
             0      11     1    x0   Ljava/lang/Class;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      11     1    x0   Ljava/lang/Class<+Ljava/util/List<*>;>;
@@ -115,15 +115,15 @@
         25: invokestatic  #8                  // Method org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
         28: invokevirtual #6                  // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         31: ldc           #9                  // String ) is not supported
         33: invokevirtual #6                  // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         36: invokevirtual #10                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
         39: areturn
       LineNumberTable:
-        line 591: 0
+        line 596: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      40     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$1;
             0      40     1 object   Ljava/lang/Object;
 }
 Signature: #32                          // Lorg/jpmml/python/CastFunction<Ljava/util/List<*>;>;
 SourceFile: "PMMLPipeline.java"
```

#### sklearn2pmml/EstimatorProxy$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum d42545e044565b26d410c4b8643ba6dfab5473181860a9febfb53e4b4a05f942
+  SHA-256 checksum 600ca86f935d310b445a2c28c02cd16847404e795129be15640cf5998d84614f
   Compiled from "EstimatorProxy.java"
 class sklearn2pmml.EstimatorProxy$1 extends org.jpmml.python.CastFunction<sklearn.Estimator>
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #13                         // sklearn2pmml/EstimatorProxy$1
   super_class: #14                        // org/jpmml/python/CastFunction
@@ -98,15 +98,15 @@
          6: aload_3
          7: putfield      #2                  // Field val$name:Ljava/lang/String;
         10: aload_0
         11: aload_2
         12: invokespecial #3                  // Method org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
         15: return
       LineNumberTable:
-        line 140: 0
+        line 155: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lsklearn2pmml/EstimatorProxy$1;
             0      16     1 this$0   Lsklearn2pmml/EstimatorProxy;
             0      16     2    x0   Ljava/lang/Class;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -134,15 +134,15 @@
         32: invokestatic  #10                 // Method org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
         35: invokevirtual #7                  // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         38: ldc           #11                 // String )
         40: invokevirtual #7                  // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         43: invokevirtual #12                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
         46: areturn
       LineNumberTable:
-        line 144: 0
+        line 159: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      47     0  this   Lsklearn2pmml/EstimatorProxy$1;
             0      47     1 object   Ljava/lang/Object;
 }
 Signature: #36                          // Lorg/jpmml/python/CastFunction<Lsklearn/Estimator;>;
 SourceFile: "EstimatorProxy.java"
```

#### sklearn2pmml/EstimatorProxy.class

##### procyon -ec {}

```diff
@@ -5,37 +5,48 @@
 import net.razorvine.pickle.objects.ClassDict;
 import org.jpmml.python.ClassDictUtil;
 import org.jpmml.converter.Feature;
 import org.jpmml.converter.Label;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
 import sklearn.EstimatorUtil;
-import java.util.List;
 import org.dmg.pmml.MiningFunction;
 import org.dmg.pmml.DataType;
 import org.dmg.pmml.OpType;
+import java.util.List;
+import sklearn.Proxy;
 import sklearn.HasEstimator;
 import sklearn.HasClasses;
 import sklearn.Estimator;
 
-public class EstimatorProxy extends Estimator implements HasClasses, HasEstimator<Estimator>
+public class EstimatorProxy extends Estimator implements HasClasses, HasEstimator<Estimator>, Proxy
 {
     public EstimatorProxy() {
         super("sklearn2pmml", "EstimatorProxy");
     }
     
     public EstimatorProxy(final String module, final String name) {
         super(module, name);
     }
     
+    public List<String> getFeatureNamesIn() {
+        final Estimator estimator = this.getEstimator();
+        return estimator.getFeatureNamesIn();
+    }
+    
     public int getNumberOfFeatures() {
         final Estimator estimator = this.getEstimator();
         return estimator.getNumberOfFeatures();
     }
     
+    public int getNumberOfOutputs() {
+        final Estimator estimator = this.getEstimator();
+        return estimator.getNumberOfOutputs();
+    }
+    
     public OpType getOpType() {
         final Estimator estimator = this.getEstimator();
         return estimator.getOpType();
     }
     
     public DataType getDataType() {
         final Estimator estimator = this.getEstimator();
```

#### sklearn2pmml/SelectorProxy.class

##### procyon -ec {}

```diff
@@ -1,14 +1,15 @@
 
 package sklearn2pmml;
 
 import java.util.List;
+import sklearn.Proxy;
 import sklearn.Selector;
 
-public class SelectorProxy extends Selector
+public class SelectorProxy extends Selector implements Proxy
 {
     public SelectorProxy() {
         this("sklearn2pmml", "SelectorProxy");
     }
     
     public SelectorProxy(final String module, final String name) {
         super(module, name);
```

#### org/jpmml/sklearn/SkLearnEncoder.class

##### procyon -ec {}

```diff
@@ -4,16 +4,14 @@
 import sklearn.ensemble.hist_gradient_boosting.TreePredictor;
 import sklearn.tree.Tree;
 import numpy.DType;
 import sklearn.neighbors.BinaryTree;
 import org.jpmml.python.PickleUtil;
 import org.dmg.pmml.ResultFeature;
 import java.util.Objects;
-import org.jpmml.converter.ScalarLabelUtil;
-import org.jpmml.converter.FeatureUtil;
 import org.jpmml.converter.Schema;
 import org.jpmml.python.ClassDictUtil;
 import org.dmg.pmml.Field;
 import org.jpmml.model.ReflectionUtil;
 import sklearn2pmml.decoration.Alias;
 import org.dmg.pmml.DerivedField;
 import org.dmg.pmml.Expression;
@@ -190,26 +188,15 @@
             final String renamedName = (String)renamedNames.get(i);
             this.renameFeature(feature, renamedName);
         }
     }
     
     public Schema createSchema() {
         final Label label = this.getLabel();
-        List<? extends Feature> features = this.getFeatures();
-        if (label instanceof ScalarLabel) {
-            final ScalarLabel scalarLabel = (ScalarLabel)label;
-            final Feature labelFeature = FeatureUtil.findLabelFeature((List)features, scalarLabel);
-            if (labelFeature != null) {
-                final DataField dataField = (DataField)labelFeature.getField();
-                this.setLabel((Label)ScalarLabelUtil.createScalarLabel(dataField));
-                features = new ArrayList<Feature>(features);
-                features.remove(labelFeature);
-            }
-            this.setFeatures(features);
-        }
+        final List<? extends Feature> features = this.getFeatures();
         return new Schema((PMMLEncoder)this, label, (List)features);
     }
     
     public boolean isFrozen(final String name) {
         return this.domains.containsKey(name);
     }
```

#### org/jpmml/sklearn/SkLearnEncoder$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum a28671dc60fef949cad48ba050a3deed61c457e57ec87d2a8a45de141674381d
+  SHA-256 checksum 20ea313a92f30b7c54b74fc5946cbaa8b370d9e53b62b382fe5c1cc30ad176fa
   Compiled from "SkLearnEncoder.java"
 class org.jpmml.sklearn.SkLearnEncoder$1
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #12                         // org/jpmml/sklearn/SkLearnEncoder$1
   super_class: #13                        // java/lang/Object
@@ -121,16 +121,16 @@
       Exception table:
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
             24    35    38   Class java/lang/NoSuchFieldError
             39    50    53   Class java/lang/NoSuchFieldError
             63    74    77   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 339: 0
-        line 109: 54
+        line 320: 0
+        line 107: 54
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 8
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.33</version>
+    <version>1.7.34</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn converter</name>
   <description>JPMML Scikit-Learn to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-sklearn
 groupId=org.jpmml
-version=1.7.33
+version=1.7.34
```

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.33.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.34.jar`

 * *Files 21% similar despite different names*

#### zipinfo {}

```diff
@@ -1,20 +1,20 @@
 Zip file size: 7767 bytes, number of entries: 18
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jul-30 08:48 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 h2o/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 h2o/utils/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 h2o/utils/metaclass/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 h2o/estimators/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 sklearn2pmml/preprocessing/h2o/
--rw-rw-r--  2.0 unx      748 b- defN 23-Jul-30 08:48 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     1049 b- defN 23-Jul-30 08:48 h2o/utils/metaclass/H2OMetaConstructor.class
--rw-rw-r--  2.0 unx     6662 b- defN 23-Jul-30 08:48 h2o/estimators/H2OEstimator.class
--rw-rw-r--  2.0 unx     1694 b- defN 23-Jul-30 08:48 sklearn2pmml/preprocessing/h2o/H2OFrameConstructor.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/org.jpmml/pmml-sklearn-h2o/
--rw-rw-r--  2.0 unx     1305 b- defN 23-Jul-30 08:47 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml
--rw-rw-r--  2.0 unx      112 b- defN 23-Jul-30 08:48 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Aug-03 15:40 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 h2o/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 h2o/utils/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 h2o/utils/metaclass/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 h2o/estimators/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/preprocessing/h2o/
+-rw-rw-r--  2.0 unx      748 b- defN 23-Aug-03 15:40 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     1049 b- defN 23-Aug-03 15:40 h2o/utils/metaclass/H2OMetaConstructor.class
+-rw-rw-r--  2.0 unx     6662 b- defN 23-Aug-03 15:40 h2o/estimators/H2OEstimator.class
+-rw-rw-r--  2.0 unx     1694 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/h2o/H2OFrameConstructor.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-h2o/
+-rw-rw-r--  2.0 unx     1305 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml
+-rw-rw-r--  2.0 unx      112 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties
 18 files, 11700 bytes uncompressed, 5375 bytes compressed:  54.1%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.33</version>
+    <version>1.7.34</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-h2o</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn H2O.ai converter</name>
   <description>JPMML Scikit-Learn H2O.ai to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Sun Jul 30 08:48:19 EEST 2023
-version=1.7.33
+#Thu Aug 03 15:40:51 EEST 2023
+version=1.7.34
 groupId=org.jpmml
 artifactId=pmml-sklearn-h2o
```

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.33.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.34.jar`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 7976 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jul-30 08:48 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 xgboost/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-30 08:48 xgboost/sklearn/
--rw-rw-r--  2.0 unx      364 b- defN 23-Jul-30 08:48 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      168 b- defN 23-Jul-30 08:48 xgboost/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     2270 b- defN 23-Jul-30 08:48 xgboost/sklearn/XGBClassifier.class
--rw-rw-r--  2.0 unx     2210 b- defN 23-Jul-30 08:48 xgboost/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2246 b- defN 23-Jul-30 08:48 xgboost/sklearn/XGBRegressor.class
--rw-rw-r--  2.0 unx     4204 b- defN 23-Jul-30 08:48 xgboost/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-30 08:48 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
--rw-rw-r--  2.0 unx     1453 b- defN 23-Jul-30 08:47 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
--rw-rw-r--  2.0 unx      116 b- defN 23-Jul-30 08:48 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
-15 files, 13161 bytes uncompressed, 5920 bytes compressed:  55.0%
+Zip file size: 7977 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Aug-03 15:40 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 xgboost/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 xgboost/sklearn/
+-rw-rw-r--  2.0 unx      364 b- defN 23-Aug-03 15:40 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      168 b- defN 23-Aug-03 15:40 xgboost/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     2270 b- defN 23-Aug-03 15:40 xgboost/sklearn/XGBClassifier.class
+-rw-rw-r--  2.0 unx     2210 b- defN 23-Aug-03 15:40 xgboost/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2246 b- defN 23-Aug-03 15:40 xgboost/sklearn/XGBRegressor.class
+-rw-rw-r--  2.0 unx     4204 b- defN 23-Aug-03 15:40 xgboost/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
+-rw-rw-r--  2.0 unx     1453 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
+-rw-rw-r--  2.0 unx      116 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
+15 files, 13161 bytes uncompressed, 5921 bytes compressed:  55.0%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.33</version>
+    <version>1.7.34</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-xgboost</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn XGBoost converter</name>
   <description>JPMML Scikit-Learn XGBoost to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Sun Jul 30 08:48:19 EEST 2023
-version=1.7.33
+#Thu Aug 03 15:40:52 EEST 2023
+version=1.7.34
 groupId=org.jpmml
 artifactId=pmml-sklearn-xgboost
```

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-statsmodels-1.0.5.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-statsmodels-1.0.5.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/pickle-1.4.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/pickle-1.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/resources/pmml-xgboost-1.7.4.jar` & `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-xgboost-1.7.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/preprocessing/h2o.py` & `sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/preprocessing/__init__.py` & `sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/preprocessing/xgboost.py` & `sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/preprocessing/lightgbm.py` & `sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/lightgbm.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/tree/chaid.py` & `sklearn2pmml-0.97.0/sklearn2pmml/tree/chaid.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.96.0/sklearn2pmml/expression/__init__.py` & `sklearn2pmml-0.97.0/sklearn2pmml/expression/__init__.py`

 * *Files identical despite different names*

