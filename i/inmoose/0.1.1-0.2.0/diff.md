# Comparing `tmp/inmoose-0.1.1.tar.gz` & `tmp/inmoose-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inmoose-0.1.1.tar", last modified: Wed May 10 12:13:43 2023, max compression
+gzip compressed data, was "inmoose-0.2.0.tar", last modified: Thu Aug  3 09:37:10 2023, max compression
```

## Comparing `inmoose-0.1.1.tar` & `inmoose-0.2.0.tar`

### file list

```diff
@@ -1,96 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.962212 inmoose-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 12:13:28.000000 inmoose-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-10 12:13:43.962212 inmoose-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-10 12:13:28.000000 inmoose-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.946212 inmoose-0.1.1/inmoose/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.950212 inmoose-0.1.1/inmoose/batch/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/batch/covariates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/batch/helper_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    25565 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/batch/pycombat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/batch/pycombat_seq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.950212 inmoose-0.1.1/inmoose/common_cpp/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/common_cpp/common_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/common_cpp/matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/common_cpp/matrix.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.954212 inmoose-0.1.1/inmoose/edgepy/
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/DGEGLM.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/DGEList.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/addPriorCount.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/adjustedProfileLik.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/aveLogCPM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/dispCoxReid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/dispCoxReidInterpolateTagwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/dropEmptyLevels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.958212 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior.h
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior_count.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior_count.h
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/adj_coxreid.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/ave_log_cpm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/compute_apl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/compute_nbdev.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/edgepy_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/fit_levenberg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/fit_levenberg.h
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/fit_one_group.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/get_one_way_fitted.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/glm.h
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/glm_levenberg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/glm_one_group.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/initialize_levenberg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/initialize_levenberg.h
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/interpolator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/interpolator.h
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/maximize_interpolant.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/nbdev.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/objects.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/objects.h
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/estimateGLMCommonDisp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/estimateGLMTagwiseDisp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/glmFit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/makeCompressedMatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/maximizeInterpolant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/mglmLevenberg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/mglmOneGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/mglmOneWay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/movingAverageByCol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/nbinomDeviance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/predFC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/splitIntoGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/systematicSubset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/validDGEList.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.958212 inmoose-0.1.1/inmoose/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/utils/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.950212 inmoose-0.1.1/inmoose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-10 12:13:43.000000 inmoose-0.1.1/inmoose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-10 12:13:43.000000 inmoose-0.1.1/inmoose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:13:43.000000 inmoose-0.1.1/inmoose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 12:13:43.000000 inmoose-0.1.1/inmoose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-10 12:13:43.000000 inmoose-0.1.1/inmoose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-10 12:13:28.000000 inmoose-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:13:43.962212 inmoose-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-10 12:13:28.000000 inmoose-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.962212 inmoose-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_DGEList.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_aveLogCPM.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_compressMatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_dispersion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_glm.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_lik.py
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_mglm.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_pycombat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_pycombatseq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:10.655456 inmoose-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 09:36:53.000000 inmoose-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-03 09:36:53.000000 inmoose-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-08-03 09:37:10.655456 inmoose-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-08-03 09:36:53.000000 inmoose-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:10.643456 inmoose-0.2.0/inmoose/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:10.647456 inmoose-0.2.0/inmoose/common_cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/common_cpp/common_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/common_cpp/matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/common_cpp/matrix.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:10.651456 inmoose-0.2.0/inmoose/edgepy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/DGEGLM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/DGEList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/addPriorCount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/adjustedProfileLik.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/aveLogCPM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/dispCoxReid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/dispCoxReidInterpolateTagwise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:10.651456 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/add_prior.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/add_prior.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/add_prior_count.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/add_prior_count.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/adj_coxreid.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/ave_log_cpm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/compute_apl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/compute_nbdev.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/edgepy_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/fit_levenberg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/fit_levenberg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/fit_one_group.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/get_one_way_fitted.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/glm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/glm_levenberg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/glm_one_group.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/initialize_levenberg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/initialize_levenberg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/interpolator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/interpolator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/maximize_interpolant.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/nbdev.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/objects.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/objects.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/estimateGLMCommonDisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/estimateGLMTagwiseDisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/glmFit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/makeCompressedMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/maximizeInterpolant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/mglmLevenberg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/mglmOneGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/mglmOneWay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/movingAverageByCol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/nbinomDeviance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/predFC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/splitIntoGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/systematicSubset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/edgepy/validDGEList.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:10.651456 inmoose-0.2.0/inmoose/pycombat/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/pycombat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/pycombat/covariates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/pycombat/helper_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21544 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/pycombat/pycombat_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/pycombat/pycombat_seq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:10.655456 inmoose-0.2.0/inmoose/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/utils/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-08-03 09:36:53.000000 inmoose-0.2.0/inmoose/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:10.647456 inmoose-0.2.0/inmoose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-08-03 09:37:10.000000 inmoose-0.2.0/inmoose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-08-03 09:37:10.000000 inmoose-0.2.0/inmoose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:37:10.000000 inmoose-0.2.0/inmoose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 09:37:10.000000 inmoose-0.2.0/inmoose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 09:37:10.000000 inmoose-0.2.0/inmoose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-03 09:36:53.000000 inmoose-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 09:37:10.655456 inmoose-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-03 09:36:53.000000 inmoose-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:10.655456 inmoose-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:10.655456 inmoose-0.2.0/tests/edgepy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/edgepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/edgepy/test_DGEList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/edgepy/test_aveLogCPM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/edgepy/test_compressMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/edgepy/test_dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/edgepy/test_glm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/edgepy/test_lik.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/edgepy/test_mglm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/edgepy/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/edgepy/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:10.655456 inmoose-0.2.0/tests/pycombat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/pycombat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/pycombat/test_covariates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/pycombat/test_pycombat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/pycombat/test_pycombatseq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:10.655456 inmoose-0.2.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-03 09:36:53.000000 inmoose-0.2.0/tests/utils/test_factor.py
```

### Comparing `inmoose-0.1.1/LICENSE` & `inmoose-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/PKG-INFO` & `inmoose-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: inmoose
-Version: 0.1.1
+Version: 0.2.0
 Summary: InMoose: the Integrated Multi Omic Open Source Environment
-Home-page: https://github.com/epigenelabs/inmoose
-Author: Maximilien Colange
-Author-email: maximilien@epigenelabs.com
+Author-email: Maximilien Colange <maximilien@epigenelabs.com>
+Project-URL: Source, https://github.com/epigenelabs/inmoose
+Project-URL: Documentation, https://inmoose.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: doc
 License-File: LICENSE
 
+[![Documentation Status](https://readthedocs.org/projects/inmoose/badge/?version=latest)](https://inmoose.readthedocs.io/en/latest/?badge=latest)
+
 # InMoose
 
 InMoose is the **In**tegrated **M**ulti **O**mic **O**pen **S**ource **E**nvironment.
 It is a collection of tools for the analysis of omic data.
 
-Currently it focuses on transcriptomic data.
-
 # Installation
 
 You can install InMoose directly with:
 
 ```
 pip install inmoose
 ```
@@ -29,23 +31,23 @@
 # Batch Effect Correction
 
 InMoose provides features to correct technical biases, also called batch
 effects, in transcriptomic data:
 - for microarray data, InMoose supersedes pyCombat [1], a Python 3
   implementation of ComBat [2], one of the most widely used tool for batch effect
   correction on microarray data.
-- for RNASeq, InMoose features a port to Python3 of ComBat-Seq [3], one the most
-  widely used tool for batch effect correction on RNASeq data.
+- for RNASeq, InMoose features a port to Python3 of ComBat-Seq [3], one of the
+  most widely used tool for batch effect correction on RNASeq data.
 
 To use these functions, simply import them and call them with default
 parameters:
 ```python
-from inmoose.batch import pycombat, pycombat_seq
+from inmoose.pycombat import pycombat_norm, pycombat_seq
 
-microarray_corrected = pycombat(microarray_data, microarray_batches)
+microarray_corrected = pycombat_norm(microarray_data, microarray_batches)
 rnaseq_corrected = pycombat_seq(rnaseq_data, rnaseq_batches)
 ```
 
 * `microarray_data`, `rnaseq_data`: the expression matrices, containing the
   information about the gene expression (rows) for each sample (columns).
 * `microarray_batches`, `rnaseq_batches`: list of batch indices, describing the
   batch for each sample. The list of batches should contain as many elements as
```

### Comparing `inmoose-0.1.1/README.md` & `inmoose-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+[![Documentation Status](https://readthedocs.org/projects/inmoose/badge/?version=latest)](https://inmoose.readthedocs.io/en/latest/?badge=latest)
+
 # InMoose
 
 InMoose is the **In**tegrated **M**ulti **O**mic **O**pen **S**ource **E**nvironment.
 It is a collection of tools for the analysis of omic data.
 
-Currently it focuses on transcriptomic data.
-
 # Installation
 
 You can install InMoose directly with:
 
 ```
 pip install inmoose
 ```
@@ -16,23 +16,23 @@
 # Batch Effect Correction
 
 InMoose provides features to correct technical biases, also called batch
 effects, in transcriptomic data:
 - for microarray data, InMoose supersedes pyCombat [1], a Python 3
   implementation of ComBat [2], one of the most widely used tool for batch effect
   correction on microarray data.
-- for RNASeq, InMoose features a port to Python3 of ComBat-Seq [3], one the most
-  widely used tool for batch effect correction on RNASeq data.
+- for RNASeq, InMoose features a port to Python3 of ComBat-Seq [3], one of the
+  most widely used tool for batch effect correction on RNASeq data.
 
 To use these functions, simply import them and call them with default
 parameters:
 ```python
-from inmoose.batch import pycombat, pycombat_seq
+from inmoose.pycombat import pycombat_norm, pycombat_seq
 
-microarray_corrected = pycombat(microarray_data, microarray_batches)
+microarray_corrected = pycombat_norm(microarray_data, microarray_batches)
 rnaseq_corrected = pycombat_seq(rnaseq_data, rnaseq_batches)
 ```
 
 * `microarray_data`, `rnaseq_data`: the expression matrices, containing the
   information about the gene expression (rows) for each sample (columns).
 * `microarray_batches`, `rnaseq_batches`: list of batch indices, describing the
   batch for each sample. The list of batches should contain as many elements as
```

### Comparing `inmoose-0.1.1/inmoose/batch/helper_seq.py` & `inmoose-0.2.0/inmoose/pycombat/helper_seq.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,29 +28,35 @@
     """
     vec = np.asarray(vec)
     vec = vec.reshape(vec.shape[0],1)
     return np.full((vec.shape[0], n_times), vec)
 
 def match_quantiles(counts_sub, old_mu, old_phi, new_mu, new_phi):
     """
-    Match quantiles from a source negative binomial distribution to a target negative binomial distribution.
+    Match quantiles from a source negative binomial distribution to a target
+    negative binomial distribution.
 
-    :param counts_sub: the original data following the source distribution
-    :type counts_sub: matrix
-    :param old_mu: the mean of the source distribution
-    :type old_mu: matrix
-    :param old_phi: the dispersion of the source distribution
-    :type old_phi: vector
-    :param new_mu: the mean of the target distribution
-    :type new_mu: matrix
-    :param new_phi: the dispersion of the target distribution
-    :type new_phi: vector
+    Arguments
+    ---------
+    counts_sub : array_like
+        the original data following the source distribution
+    old_mu : array_like
+        the mean of the source distribution
+    old_phi : array_like
+        the dispersion of the source distribution
+    new_mu : array_like
+        the mean of the target distribution
+    new_phi : array_like
+        the dispersion of the target distribution
 
-    :return: adjusted data, corresponding in the target distribution to the same quantiles as the input data has in the source distribution
-    :rtype: matrix
+    Returns
+    -------
+    ndarray
+        adjusted data, corresponding in the target distribution to the same
+        quantiles as the input data in the source distribution
     """
     new_counts_sub = np.full(counts_sub.shape, np.nan)
 
     i = counts_sub <= 1
     new_counts_sub[i] = counts_sub[i]
     i = np.logical_not(i)
     old_size = np.full(old_mu.shape, 1 / old_phi.reshape(old_mu.shape[0], 1))
```

### Comparing `inmoose-0.1.1/inmoose/batch/pycombat.py` & `inmoose-0.2.0/inmoose/pycombat/pycombat_norm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #-----------------------------------------------------------------------------
-# Copyright (C) 2019-2023 A. Behdenna, A. Nordor, J. Haziza and A. Gema
+# Copyright (C) 2019-2023 A. Behdenna, A. Nordor, J. Haziza, A. Gema and M. Colange
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -11,55 +11,21 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #-----------------------------------------------------------------------------
 
+import logging
 import numpy as np
 from functools import partial
 import mpmath as mp
 import pandas as pd
 
-from .covariates import check_confounded_covariates
-
-
-def model_matrix(info, intercept=True, drop_first=True):
-    """Creates the model_matrix from batch list
-
-    Arguments:
-        info {list} -- list info with batch or covariates data
-        intercept {bool} -- boolean for intercept in model matrix
-
-    Returns:
-        matrix -- model matrix generate from batch list
-    """
-    if not isinstance(info[0], list):
-        info = [info]
-    else:
-        info = info
-    info_dict = {}
-    for i in range(len(info)):
-        info_dict[f"col{str(i)}"] = list(map(str,info[i]))
-    df = pd.get_dummies(pd.DataFrame(info_dict), drop_first=drop_first, dtype=float)
-    if intercept:
-        df["intercept"] = 1.0
-    return df.to_numpy()
-
-
-def all_1(list_of_elements):
-    """checks if all elements in a list are 1s
-
-    Arguments:
-        list_of_elements {list} -- list of elements
-
-    Returns:
-        bool -- True iff all elements of the list are 1s
-    """
-    return((list_of_elements == 1).all())
+from .covariates import make_design_matrix
 
 
 # aprior and bprior are useful to compute "hyper-prior values"
 # -> prior parameters used to estimate the prior gamma distribution for multiplicative batch effect
 # aprior - calculates empirical hyper-prior values
 
 def compute_prior(prior, gamma_hat, mean_only):
@@ -199,15 +165,15 @@
             buf_pow = np.array(list(map(partial(mp.power, y=n/2), 1/(np.pi*temp_2d))))
             #print(buf_exp.dtype, buf_pow.dtype)
             LH = buf_pow*buf_exp  # likelihood
         # /end{handling high precision computing}
         LH = np.nan_to_num(LH)  # corrects NaNs in likelihood
         if np.sum(LH) == 0 and test_approximation == 0:
             test_approximation = 1  # this message won't appear again
-            print("###\nValues too small, approximation applied to avoid division by 0.\nPrecision mode can correct this problem, but increases computation time.\n###")
+            logging.info("###\nValues too small, approximation applied to avoid division by 0.\nPrecision mode can correct this problem, but increases computation time.\n###")
 
         if np.sum(LH) == 0: # correction for LH full of 0.0
             LH[LH == 0] = np.exp(-745)
             g_star.append(np.sum(g*LH)/np.sum(LH))
             d_star.append(np.sum(d*LH)/np.sum(LH))
         else:
             g_star.append(np.sum(g*LH)/np.sum(LH))
@@ -278,127 +244,30 @@
     Arguments:
         mean_only {boolean} -- user's choice about mean_only
 
     Returns:
         ()
     """
     if mean_only == True:
-        print("Using mean only version")
-
-
-def define_batchmod(batch):
-    """generates model matrix
-
-    Arguments:
-        batch {list} -- list of batch id
-
-    Returns:
-        batchmod {matrix} -- model matrix for batches
-    """
-    batchmod = model_matrix(list(batch), intercept=False, drop_first=False)
-    return(batchmod)
-
-
-def check_ref_batch(ref_batch, batch, batchmod):
-    """check ref_batch option and treat it if needed
-
-    Arguments:
-        ref_batch -- the reference batch
-        batch {list} -- list of batch id
-        batchmod {matrix} -- model matrix related to batches
-
-    Returns:
-        ref {int} -- the index of the reference batch in the batch list
-        batchmod {matrix} -- updated model matrix related to batches, with reference
-    """
-    if ref_batch is not None:
-        if ref_batch not in batch:
-            raise ValueError("Reference level ref.batch must be one of the levels of batch.")
-        print("Using batch "+str(ref_batch) +
-              " as a reference batch.")
-        # ref keeps in memory the columns concerned by the reference batch
-        ref = np.where(np.unique(batch) == ref_batch)[0][0]
-        # updates batchmod with reference
-        batchmod[:,ref] = 1
-    else:
-        ref = None  # default settings
-    return(ref, batchmod)
-
-
-def treat_batches(batch):
-    """treat batches
-
-    Arguments:
-        batch {list} -- batch list
-
-    Returns:
-        n_batch {int} -- number of batches
-        batches {int list} -- list of unique batches
-        n_batches {int list} -- list of batches lengths
-        n_array {int} -- total size of dataset
-    """
-    batch = pd.Series(batch)
-    n_batch = len(np.unique(batch))  # number of batches
-    print("Found "+str(n_batch)+" batches.")
-    batches = []  # list of lists, contains the list of position for each batch
-    for i in range(n_batch):
-        batches.append(np.where(batch == np.unique(batch)[i])[0].astype(np.int32))
-    n_batches = list(map(len, batches))
-    if 1 in n_batches:
-        #mean_only = True  # no variance if only one sample in a batch - mean_only has to be used
-        print("\nOne batch has only one sample, try setting mean_only=True.\n")
-    n_array = sum(n_batches)
-    return(n_batch, batches, n_batches, n_array)
-
-
-def treat_covariates(batchmod, mod, ref, n_batch):
-    """treat covariates
-
-    Arguments:
-        batchmod {matrix} -- model matrix for batch
-        mod {matrix} -- model matrix for other covariates
-        ref {int} -- index of reference batch
-        n_batch {int} -- number of batches
-
-    Returns:
-        check {bool list} -- a list characterising all covariates
-        design {matrix} -- model matrix for all covariates, including batch
-    """
-    # design matrix for sample conditions
-    if mod == []:
-        design = batchmod
-    else:
-        mod_matrix = model_matrix(mod, intercept=True)
-        design = np.concatenate((batchmod, mod_matrix), axis=1)
-    check = list(map(all_1, np.transpose(design)))
-    if ref is not None:  # if ref
-        check[ref] = False  # the reference batch is not considered a covariate
-    design = design[:, ~np.array(check)]
-    design = np.transpose(design)
-
-    print("Adjusting for "+str(len(design)-len(np.transpose(batchmod))) +
-          " covariate(s) or covariate level(s).")
-
-    check_confounded_covariates(design.T, n_batch)
-    return(design)
+        logging.info("Using mean only version")
 
 
 def check_NAs(dat):
     """check if NaNs - in theory, we construct the data without NAs
 
     Arguments:
         dat {matrix} -- the data matrix
 
     Returns:
         NAs {bool} -- boolean characterising the presence of NaNs in the data matrix
     """
     # NAs = True in (np.isnan(dat))
     NAs = np.isnan(np.sum(dat))  # Check if NaN exists
     if NAs:
-        print("Found missing data values. Please remove all missing values before proceeding with pyComBat.")
+        logging.error("Found missing data values. Please remove all missing values before proceeding with pyComBat.")
     return(NAs)
 
 
 def calculate_mean_var(design, batches, ref, dat, NAs, n_batches, n_batch, n_array):
     """ calculates the Normalisation factors
 
     Arguments:
@@ -411,15 +280,15 @@
         n_array {int} -- total size of dataset
 
     Returns:
         B_hat {matrix} -- regression coefficients corresponding to the design matrix
         grand_mean {matrix} -- Mean for each gene and each batch
         var_pooled {matrix} -- Variance for each gene and each batch
     """
-    print("Standardizing Data across genes.")
+    logging.info("Standardizing Data across genes.")
     if not(NAs):  # NAs not supported
         # B_hat is the vector of regression coefficients corresponding to the design matrix
         B_hat = np.linalg.solve(np.dot(design, np.transpose(
             design)), np.dot(design, np.transpose(dat)))
 
     # Calculates the general mean
     if ref is not None:
@@ -477,15 +346,15 @@
     """
     s_data = (dat - stand_mean) / \
         np.dot(np.transpose(np.mat(np.sqrt(var_pooled))), np.mat([1]*n_array))
     return(s_data)
 
 
 def fit_model(design, n_batch, s_data, batches, mean_only, par_prior, precision, ref, NAs):
-    print("Fitting L/S model and finding priors.")
+    logging.info("Fitting L/S model and finding priors.")
 
     # fraction of design matrix related to batches
     batch_design = design[0:n_batch]
 
     if not NAs:  # CF SUPRA FOR NAs
         # gamma_hat is the vector of additive batch effect
         gamma_hat = np.linalg.solve(np.dot(batch_design, np.transpose(batch_design)),
@@ -513,28 +382,28 @@
 
     # initialise gamma and delta for parameters estimation
     gamma_star = np.empty((n_batch, len(s_data)))
     delta_star = np.empty((n_batch, len(s_data)))
 
     if par_prior:
         # use param_fun function for parametric adjustments (cf. function definition)
-        print("Finding parametric adjustments.")
+        logging.info("Finding parametric adjustments.")
         results = list(map(partial(param_fun,
                                    s_data=s_data,
                                    batches=batches,
                                    mean_only=mean_only,
                                    gamma_hat=gamma_hat,
                                    gamma_bar=gamma_bar,
                                    delta_hat=delta_hat,
                                    t2=t2,
                                    a_prior=a_prior,
                                    b_prior=b_prior), range(n_batch)))
     else:
         # use nonparam_fun for non-parametric adjustments (cf. function definition)
-        print("Finding nonparametric adjustments")
+        logging.info("Finding nonparametric adjustments")
         results = list(map(partial(nonparam_fun, mean_only=mean_only, delta_hat=delta_hat,
                                    s_data=s_data, batches=batches, gamma_hat=gamma_hat, precision=precision), range(n_batch)))
 
     for i in range(n_batch):  # store the results in gamma/delta_star
         results_i = results[i]
         gamma_star[i], delta_star[i] = results_i[0], results_i[1]
 
@@ -565,15 +434,15 @@
 
     Returns:
         bayes_data [matrix] -- data adjusted for correction of batch effects
     """
     # Now we adjust the data:
     # 1. substract additive batch effect (gamma_star)
     # 2. divide by multiplicative batch effect (delta_star)
-    print("Adjusting the Data")
+    logging.info("Adjusting the Data")
     bayes_data = np.transpose(s_data)
     j = 0
     for i in batches:  # for each batch, specific correction
         bayes_data[i] = (bayes_data[i] - np.dot(np.transpose(batch_design)[i], gamma_star)) / \
             np.transpose(
                 np.outer(np.sqrt(delta_star[j]), np.asarray([1]*n_batches[j])))
         j += 1
@@ -588,65 +457,70 @@
     if ref is not None:
         bayes_data[batches[ref]] = dat[batches[ref]]
 
     # returns the data corrected for batch effects
     return bayes_data
 
 
-def pycombat(data, batch, mod=[], par_prior=True, prior_plots=False, mean_only=False, ref_batch=None, precision=None, **kwargs):
+def pycombat_norm(data, batch, mod=None, par_prior=True, prior_plots=False, mean_only=False, ref_batch=None, precision=None, **kwargs):
     """Corrects batch effect in microarray expression data. Takes an gene expression file and a list of known batches corresponding to each sample.
 
     Arguments
     ---------
     data : matrix
-        expression matrix (dataframe). It contains the information about the gene expression (rows) for each sample (columns).
+        expression matrix (dataframe or numpy array). It contains the information about the gene expression (rows) for each sample (columns).
     batch : list
         batch indices. Must have as many elements as the number of columns in the expression matrix.
-    mod : list, optional
-        list (or list of lists) of covariate(s) indexes. The mod list describes the covariate(s) for each sample.
-        Each mod list has as many elements as the number of columns in the expression matrix (default: `[]`).
+    mod : matrix, optional
+        matrix model for multiple covariates to include in linear model (signal from these variables are kept in data after adjustment)
     par_prior : bool, optional
         False for non-parametric estimation of batch effects (default: `True`).
     prior_plots : bool, optional
         True if requires to plot the priors (default: `False`). -- Not implemented yet!
     mean_only : bool, optional
         True iff just adjusting the means and not individual batch effects (default: `False`).
     ref_batch, optional
         batch id of the batch to use as reference (default: `None`)
     precision : float, optional
         level of precision for precision computing (default: `None`).
 
     Returns
     -------
-    dataframe
+    matrix
         the input expression matrix adjusted for batch effects.
+        same type as the input `data`
     """
 
-    list_samples = data.columns
-    list_genes = data.index
-    dat = data.values
+    if isinstance(data, pd.DataFrame):
+        list_samples = data.columns
+        list_genes = data.index
+        dat = data.values
+    else:
+        dat = data
 
     check_mean_only(mean_only)
 
-    batchmod = define_batchmod(batch)
-    ref, batchmod = check_ref_batch(ref_batch, batch, batchmod)
-    n_batch, batches, n_batches, n_array = treat_batches(batch)
-    design = treat_covariates(batchmod, mod, ref, n_batch)
-    NAs = check_NAs(dat)
-    if not(NAs):
-        B_hat, grand_mean, var_pooled = calculate_mean_var(
-            design, batches, ref, dat, NAs, n_batches, n_batch, n_array)
-        stand_mean = calculate_stand_mean(
-            grand_mean, n_array, design, n_batch, B_hat)
-        s_data = standardise_data(dat, stand_mean, var_pooled, n_array)
-        gamma_star, delta_star, batch_design = fit_model(
-            design, n_batch, s_data, batches, mean_only, par_prior, precision, ref, NAs)
-        bayes_data = adjust_data(s_data, gamma_star, delta_star, batch_design,
-                                n_batches, var_pooled, stand_mean, n_array, ref, batches, dat)
-
-        bayes_data_df = pd.DataFrame(bayes_data,
-                    columns = list_samples,
-                    index = list_genes)
+    design, batchmod, mod, batches, n_batches, n_batch, n_array, ref = \
+            make_design_matrix(dat, batch, None, mod, True, ref_batch)
+    design = np.transpose(design)
+
+    # Check for missing values in count matrix
+    NAs = np.isnan(dat).any()
+    if NAs:
+        raise ValueError(f"Found {np.isnan(dat).sum()} missing values (NaN) in count matrix. NaN values are not accepted. Please remove them before proceeding with pycombat_norm.")
 
-        return(bayes_data_df)
+    B_hat, grand_mean, var_pooled = calculate_mean_var(
+        design, batches, ref, dat, NAs, n_batches, n_batch, n_array)
+    stand_mean = calculate_stand_mean(
+        grand_mean, n_array, design, n_batch, B_hat)
+    s_data = standardise_data(dat, stand_mean, var_pooled, n_array)
+    gamma_star, delta_star, batch_design = fit_model(
+        design, n_batch, s_data, batches, mean_only, par_prior, precision, ref, NAs)
+    bayes_data = adjust_data(s_data, gamma_star, delta_star, batch_design,
+                            n_batches, var_pooled, stand_mean, n_array, ref, batches, dat)
+
+    if isinstance(data, pd.DataFrame):
+        return pd.DataFrame(bayes_data,
+                            columns = list_samples,
+                            index = list_genes)
     else:
-        raise ValueError("NaN value is not accepted")
+        return bayes_data
```

### Comparing `inmoose-0.1.1/inmoose/batch/pycombat_seq.py` & `inmoose-0.2.0/inmoose/pycombat/pycombat_seq.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,137 +14,86 @@
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #-----------------------------------------------------------------------------
 
 # This file is based on the file 'R/ComBat_seq.R' of the Bioconductor sva package (version 3.44.0).
 
+import logging
 import numpy as np
-from pandas import DataFrame
-from patsy import dmatrix
-from warnings import warn
+import pandas as pd
 
 from ..edgepy import DGEList, estimateGLMCommonDisp, estimateGLMTagwiseDisp, glmFit
 from ..utils import asfactor
-from .covariates import check_confounded_covariates
+from .covariates import make_design_matrix
 from .helper_seq import vec2mat, match_quantiles
 
-def pycombat_seq(counts, batch, group=None, covar_mod=None, full_mod=True, shrink=False, shrink_disp=False, gene_subset_n=None, ref_batch=None):
+def pycombat_seq(data, batch, group=None, covar_mod=None, full_mod=True, shrink=False, shrink_disp=False, gene_subset_n=None, ref_batch=None):
     """pycombat_seq is an improved model from ComBat using negative binomial regression, which specifically targets RNA-Seq count data.
 
     Arguments
     ---------
-    counts : matrix
-        raw count matrix from genomic studies (dimensions gene x sample)
-    batch : vector or list or :obj:`inmoose.utils.factor.Factor`
+    data : matrix
+        raw count matrix (dataframe or numpy array) from genomic studies (dimensions gene x sample)
+    batch : array or list or :obj:`inmoose.utils.factor.Factor`
         Batch indices. Must have as many elements as the number of columns in the expression matrix.
-    group : vector or list or :obj:`inmoose.utils.factor.Factor`, optional
+    group : array or list or :obj:`inmoose.utils.factor.Factor`, optional
         vector/factor for biological condition of interest (default: `None`)
     covar_mod : matrix, optional
         model matrix for multiple covariates to include in linear model (signal from these variables are kept in data after adjustment)
     full_mod : bool, optional
         if True, include condition of interest in model
     shrink : bool, optional
         whether to apply shrinkage on parameter estimation
     shrink_disp : bool, optional
         whether to apply shrinkage on dispersion
     gene_subset_n : int, optional
         number of genes to use in emprirical Bayes estimation, only useful when shrink = True
-    ref_batch, optional
+    ref_batch : any, optional
         batch id of the batch to use as reference (default: `None`)
 
     Returns
     -------
     matrix
-        the input expression matrix adjusted for batch effects
+        the input expression matrix adjusted for batch effects.
+        same type as the input `data`
     """
 
+    if isinstance(data, pd.DataFrame):
+        list_samples = data.columns
+        list_genes = data.index
+        counts = data.values
+    else:
+        counts = data
+
     ####### Preparation #######
+    # make sure batch is a factor
     batch = asfactor(batch)
-    # TODO No support for single-sample batch yet
 
     # Remove genes with only 0 counts in any batch
     keep = np.full((counts.shape[0],), True)
     for b in batch.categories:
         keep &= counts[:, batch == b].sum(axis=1) > 0
     rm = np.logical_not(keep).nonzero()[0]
     keep = keep.nonzero()[0]
     countsOri = counts.copy()
     counts = counts[keep,:]
 
     dge_obj = DGEList(counts=counts)
 
-    # Prepare characteristics on batches
-    n_batch = batch.nlevels()
-    # list of samples in each batch
-    batches_ind = [(batch == batch.categories[i]).nonzero()[0] for i in range(n_batch)]
-    n_batches = [len(i) for i in batches_ind]
-    n_sample = np.sum(n_batches)
-    print("Found", n_batch, "batches")
-
-    # Make design matrix
-    # batch
-    batchmod = dmatrix("~-1 + C(batch)")
-    # reference batch
-    if ref_batch is not None:
-        if ref_batch not in batch.categories:
-            raise ValueError("Reference batch must identify one of the batches")
-        print("Using batch", ref_batch, "as reference batch")
-        # ref_batch_index is the index of the reference batch in batch.categories
-        ref_batch_index = np.where(batch.categories == ref_batch)[0][0]
-        # update batchmod with reference
-        batchmod[:,ref_batch_index] = 1
-    else:
-        ref_batch_index = None
-
-    # covariate
-    group = asfactor([] if group is None else group)
-    # handle missing covariates, by creating a distinct covariate per batch where a missing covariate appears
-    nan_group = group.isna()
-    if nan_group.any():
-        warn(f"{nan_group.sum()} missing covariates in group. Creating a distinct covariate per batch for the missing values. You may want to double check your covariates.")
-        nan_batch_group = [f"nan_batch_{batch[i]}" for i in range(len(group)) if nan_group[i]]
-        group = group.add_categories(np.unique(nan_batch_group))
-        for i,j in enumerate(np.where(nan_group)[0]):
-            group[j] = nan_batch_group[i]
-
-    if full_mod and group.nlevels() > 1:
-        print("Using full model in pycombat_seq")
-        mod = dmatrix("~group")
-    else:
-        print("Using null model in pycombat_seq")
-        mod = dmatrix("~1", DataFrame(counts.T))
-    # drop intercept in covariate model
-    if covar_mod is not None:
-        check = [(covar_mod[:,i] == 1).all() for i in range(covar_mod.shape[1])]
-        covar_mod = covar_mod[:, np.logical_not(check)]
-        # bind with biological condition of interest
-        mod = np.concatenate((mod, covar_mod), axis=1)
-    # combine
-    design = dmatrix("~-1 + batchmod + mod")
-
-    # Check for intercept in covariates, and drop if present
-    check = [(design[:,i] == 1).all() for i in range(design.shape[1])]
-    if ref_batch_index is not None:
-        # the reference batch is not considered as a covariate
-        check[ref_batch_index] = False
-    design = design[:, np.logical_not(check)]
-    print("Adjusting for", design.shape[1]-batchmod.shape[1], "covariate(s) or covariate level(s)")
-
-    # Check if the design is confounded
-    check_confounded_covariates(design, n_batch)
+    # Handle batches, covariates and prepare design matrix
+    design, batchmod, mod, batches_ind, n_batches, n_batch, n_sample, ref_batch_index = \
+        make_design_matrix(counts, batch, group, covar_mod, full_mod, ref_batch)
 
     # Check for missing values in count matrix
-    nas = np.isnan(counts).any()
-    if nas:
-        print("Found", np.isnan(counts).sum(), "missing data values")
-        raise RuntimeError("missing values in count matrix")
+    if np.isnan(counts).any():
+        raise ValueError(f"Found {np.isnan(counts).sum()} missing values (NaN) in count matrix. NaN values are not accepted. Please remove them before proceeding with pycombat_seq.")
 
     ####### Estimate gene-wise dispersions within each batch #######
-    print("Estimating dispersions")
+    logging.info("Estimating dispersions")
     # Estimate common dispersion within each batch as an initial value
     def disp_common_helper(i):
         if n_batches[i] <= design.shape[1]-batchmod.shape[1]+1 or np.linalg.matrix_rank(mod[batches_ind[i]]) < mod.shape[1]:
             # not enough residual degree of freedom
             return estimateGLMCommonDisp(counts[:, batches_ind[i]], design=None, subset=counts.shape[0])
         else:
             return estimateGLMCommonDisp(counts[:, batches_ind[i]], design=mod[batches_ind[i]], subset=counts.shape[0])
@@ -162,15 +111,15 @@
 
     # construction dispersion matrix
     phi_matrix = np.full(counts.shape, np.nan)
     for k in range(n_batch):
         phi_matrix[:, batches_ind[k]] = vec2mat(genewise_disp_lst[k], n_batches[k])
 
     ####### Estimate parameters from NB GLM #######
-    print("Fitting the GLM model")
+    logging.info("Fitting the GLM model")
     # no intercept - nonEstimable; compute offset (library sizes) within function
     glm_f = dge_obj.glmFit(design=design, dispersion=phi_matrix, prior_count=1e-4)
     # compute intercept as batch-size-weighted average from batches
     alpha_g = glm_f.coefficients[:, range(n_batch)] @ (n_batches/n_sample)
     # original offset - sample (library size)
     new_offset = vec2mat(dge_obj.getOffset(), counts.shape[0]).T
     # new offset - gene background expression (dge_obj.getOffset() is the same as log(dge_obj.samples.lib_size)
@@ -180,29 +129,29 @@
 
     gamma_hat = glm_f2.coefficients[:, range(n_batch)]
     mu_hat = glm_f2.fitted_values
     phi_hat = np.column_stack(genewise_disp_lst)
 
     ####### In each batch, compute posterior estimation through Monte-Carlo integration #######
     if shrink:
-        print("Apply shrinkage - computing posterior estimates for parameters")
+        logging.info("Apply shrinkage - computing posterior estimates for parameters")
         raise NotImplementedError
     else:
-        print("shrinkage off - using GLM estimates for parameters")
+        logging.info("shrinkage off - using GLM estimates for parameters")
         gamma_star_mat = gamma_hat
         phi_star_mat = phi_hat
 
     ####### Obtain adjusted batch-free distribution #######
     mu_star = np.full(counts.shape, np.nan)
     for jj in range(n_batch):
         mu_star[:, batches_ind[jj]] = np.exp(np.log(mu_hat[:, batches_ind[jj]]) - vec2mat(gamma_star_mat[:, jj], n_batches[jj]))
     phi_star = phi_star_mat.mean(axis=1)
 
     ####### Ajust the data #######
-    print("Adjusting the data")
+    logging.info("Adjusting the data")
     adjust_counts = np.full(counts.shape, np.nan)
     for kk in range(n_batch):
         counts_sub = counts[:, batches_ind[kk]]
         if kk == ref_batch_index:
             adjust_counts[:, batches_ind[kk]] = counts_sub
             continue
         old_mu = mu_hat[:, batches_ind[kk]]
@@ -211,8 +160,14 @@
         new_phi = phi_star
         adjust_counts[:, batches_ind[kk]] = match_quantiles(counts_sub=counts_sub, old_mu=old_mu, old_phi=old_phi, new_mu=new_mu, new_phi=new_phi)
 
     # Add back genes with only 0 counts in any batch (so that dimensions do not change)
     adjust_counts_whole = np.full(countsOri.shape, np.nan)
     adjust_counts_whole[keep,:] = adjust_counts
     adjust_counts_whole[rm,:] = countsOri[rm,:]
-    return adjust_counts_whole
+
+    if isinstance(data, pd.DataFrame):
+        return pd.DataFrame(adjust_counts_whole,
+                            columns = list_samples,
+                            index = list_genes)
+    else:
+        return adjust_counts_whole
```

### Comparing `inmoose-0.1.1/inmoose/common_cpp/common_cpp.pyx` & `inmoose-0.2.0/inmoose/common_cpp/common_cpp.pyx`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/common_cpp/matrix.cpp` & `inmoose-0.2.0/inmoose/common_cpp/matrix.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/common_cpp/matrix.h` & `inmoose-0.2.0/inmoose/common_cpp/matrix.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/DGEGLM.py` & `inmoose-0.2.0/inmoose/edgepy/DGEGLM.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/DGEList.py` & `inmoose-0.2.0/inmoose/edgepy/DGEList.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,35 +14,82 @@
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #-----------------------------------------------------------------------------
 
 # This file is based on the file 'R/DGEList.R' of the Bioconductor edgeR package (version 3.38.4).
 
-
+import logging
 import numpy as np
 import pandas as pd
-from warnings import warn
 
 from .edgepy_cpp import is_integer_array
 from ..utils import Factor
 from .utils import _isAllZero
 
 class DGEList(object):
+    """
+    A class for storing read counts and associated information from digital
+    gene expression or sequencing technologies.
+
+    Attributes
+    ----------
+    counts : ndarray
+        matrix of read counts, one row per gene and one column per sample
+    samples : DataFrame
+        dataframe with a row for each sample and columns :code:`group`,
+        :code:`lib_size` and :code:`norm_factors` containing the group labels,
+        library sizes and normalization factors.
+        Other columns can be optionally added to give more detailed sample
+        information.
+    common_dispersion : float, optional
+        the overall dispersion estimate
+    tagwise_dispersion : ndarray, optional
+        genewise dispersion estimates for each gene ("tag" and "gene" are
+        synonymous here)
+    trended_dispersion : ndarray, optional
+        trended dispersion estimates for each gene
+    offset : array_like, optional
+        matrix of same shape as :code:`counts` giving offsets for log-linear
+        models
+    genes : DataFrame, optional
+        annotation information for each gene. Same number of rows as
+        :code:`counts`
+    AveLogCPM : ndarray, optional
+        average log2 counts per million for each gene
+    """
 
     from .aveLogCPM import aveLogCPM_DGEList as aveLogCPM
     from .estimateGLMCommonDisp import estimateGLMCommonDisp_DGEList as estimateGLMCommonDisp
     from .estimateGLMTagwiseDisp import estimateGLMTagwiseDisp_DGEList as estimateGLMTagwiseDisp
     from .glmFit import glmFit_DGEList as glmFit
     from .predFC import predFC_DGEList as predFC
     from .splitIntoGroups import splitIntoGroups_DGEList as splitIntoGroups
 
     def __init__(self, counts, lib_size=None, norm_factors=None, samples=None, group=None, genes=None, remove_zeroes=False):
         """
         Construct DGEList object from components with some checking
+
+        Arguments
+        ---------
+        counts : array_like
+            matrix of counts
+        lib_size : array_like, optional
+            vector of total counts (sequence depth) for each library
+        norm_factors : array_like, optional
+            vector of normalization factors that modify the library sizes
+        samples : DataFrame, optional
+            information for each sample
+        group : array_like or Factor, optional
+            vector or factor giving the experimental group/condition for each
+            sample/library
+        genes : DataFrame, optional
+            annotation information for each gene
+        remove_zeroes : bool
+            whether to remove rows that have 0 total count
         """
 
         # Check counts
         counts = np.asarray(counts, order='F')
         if len(counts.shape) != 2:
             raise ValueError("'counts' is not a matrix!")
         try:
@@ -65,15 +112,15 @@
         minlibsize = np.min(lib_size)
         # TODO check lib_size for NaN
         if minlibsize < 0:
             raise ValueError("negative library size not permitted")
         if minlibsize == 0:
             if np.logical_and(lib_size == 0, (counts.sum(axis=0) > 0)).any():
                 raise ValueError("library size set to zero but counts are nonzero")
-            warn("library size of zero detected")
+            logging.warnings.warn("library size of zero detected")
 
         # Check norm_factors
         if norm_factors is None:
             norm_factors = np.ones(nlibs)
         # TODO check that norm_factors is numeric
         if nlibs != len(norm_factors):
             raise ValueError("Length of 'norm_factors' must be equal to the number of columns in 'counts'")
```

### Comparing `inmoose-0.1.1/inmoose/edgepy/__init__.py` & `inmoose-0.2.0/inmoose/edgepy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from .addPriorCount import addPriorCount
 from .adjustedProfileLik import adjustedProfileLik
 from .aveLogCPM import aveLogCPM
 from .DGEGLM import DGEGLM
 from .DGEList import DGEList
 from .dispCoxReid import dispCoxReid
+from .dispCoxReidInterpolateTagwise import dispCoxReidInterpolateTagwise
 from .estimateGLMCommonDisp import estimateGLMCommonDisp
 from .estimateGLMTagwiseDisp import estimateGLMTagwiseDisp
 from .glmFit import glmFit
 from .maximizeInterpolant import maximizeInterpolant
 from .mglmLevenberg import mglmLevenberg
 from .mglmOneGroup import mglmOneGroup
 from .mglmOneWay import mglmOneWay, designAsFactor
 from .movingAverageByCol import movingAverageByCol
 from .nbinomDeviance import nbinomDeviance
+from .predFC import predFC
+from .splitIntoGroups import splitIntoGroups
 from .stats import pnbinom, qnbinom
 from .systematicSubset import systematicSubset
 from .validDGEList import validDGEList
 from .edgepy_cpp import *
```

### Comparing `inmoose-0.1.1/inmoose/edgepy/aveLogCPM.py` & `inmoose-0.2.0/inmoose/edgepy/addPriorCount.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,85 +12,84 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #-----------------------------------------------------------------------------
 
-# This file is based on the file 'R/aveLogCPM.R' of the Bioconductor edgeR package (version 3.38.4).
+# This file is based on the file 'R/addPriorCount.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
-from inspect import signature
 import numpy as np
+from .makeCompressedMatrix import _compressOffsets, _compressPrior, makeCompressedMatrix
+from .edgepy_cpp import cxx_add_prior_count
 
-from .utils import _isAllZero
-from .makeCompressedMatrix import _compressDispersions, _compressWeights, _compressOffsets, _compressPrior
-from .mglmOneGroup import mglmOneGroup
-from .edgepy_cpp import cxx_ave_log_cpm
-
-def aveLogCPM_DGEList(self, normalized_lib_sizes=True, prior_count=2, dispersion=None):
-    """
-    log2(AveCOM)
+def addPriorCount(y, lib_size=None, offset=None, prior_count=1):
     """
-    # Library sizes should be stored in y but are sometimes missing
-    lib_size = self.samples.lib_size
-    if (lib_size.values == None).any():
-        lib_size = self.counts.sum(axis=0)
-
-    # Normalization factors should be stored in y but are sometimes missing
-    if normalized_lib_sizes:
-        nf = self.samples.norm_factors
-        if (nf.values != None).all():
-            lib_size = lib_size*nf
-
-    # Dispersion supplied as argument takes precedence over value in object
-    # Should trended_dispersion or tagwise_dispersion be used instead of common_dispersion if available?
-    if dispersion is None:
-        dispersion = self.common_dispersion
-
-    return aveLogCPM(self.counts, lib_size=lib_size, prior_count=prior_count, dispersion=dispersion, weights=self.weights)
+    Add a library size-adjusted prior count to each observation.
 
-def aveLogCPM(y, lib_size=None, offset=None, prior_count=2, dispersion=None, weights=None):
+    This function adds a positive prior count to each observation, often useful
+    to avoid zeroes during calculation of log-values. For example,
+    :func:`predFC` will call this function to calculate shrunken log-fold
+    changes. :func:`aveLogCPM` and :func:`cpm` also use the same underlying
+    code to calculate (average) log-counts per million.
+
+    The actual value added to the counts for each library is scaled according
+    to the library size. This ensures that the relatives contribution of the
+    prior is the same for each library. Otherwise, a fixed prior would have
+    little effect on a large library, but a big effect on a small library.
+
+    The library sizes are also modified, with twice the scales prior being
+    added to the library size for each library. To understand the motication
+    for this, consider that each observation is, effectively, a proportion of
+    the total count in the library. The addition scheme implemented here
+    represents an empirical logistic transform and ensures that the proportion
+    can never be zero or one.
+
+    If :code:`offset` is supplied, this is used in favor of :code:`lib_size`,
+    where :code:`exp(offset)` is defined as the vector/matrix of library sizes.
+    If an offset matrix is supplied, this will lead to gene-specific scaling of
+    the prior as described above.
+
+    Most use cases of this function will involve supplying a constant value to
+    :code:`prior_count` for all genes. However, it is also possible to use
+    gene-specific values by supplying a vector of length equal to the number of
+    rows in :code:`y`.
+
+    Arguments
+    ---------
+    y : matrix
+        a numeric count matrix, with rows corresponding to genes and columns to
+        libraries
+    lib_size : array, optional
+        a numeric vector of library sizes
+    offset : array, optional
+        a numeric vector or matrix of offsets
+    prior_count : float or array
+        a constant or gene-specific vector of prior counts to be added genes
+
+    Returns
+    -------
+    matrix
+        matrix of counts with the added priors
+    CompressedMatrix
+        the log-transformed modified library sizes
     """
-    Compute average log2-cpm for each gene over all samples.
-    This measure is designed to be used as the x-axis for all abundance-dependent trend analyses in edgeR.
-    It is generally held fixed through an edgeR analysis.
-    """
-    y = np.asarray(y, order='F')
-    if len(y.shape) != 2:
-        raise ValueError("y should be a matrix")
-    if y.shape[0] == 0:
-        return 0
-
-    # Special case when all counts and library sizes are zero
-    if _isAllZero(y):
-        if (lib_size is None or max(lib_size) == 0) and (offset is None or max(offset) == np.NINF):
-            abundance = np.full((y.shape[0],), -np.log(y.shape[0]))
-            return (abundance + np.log(1e6)) / np.log(2)
-
-    # Check dispersion
-    if dispersion is None:
-        dispersion = 0.05
-    isna = np.isnan(dispersion)
-    if isna.all():
-        dispersion = 0.05
-    elif isna.any():
-        dispersion = np.asanyarray(dispersion, order='F')
-        dispersion[isna] = np.nanmean(dispersion)
 
-    dispersion = _compressDispersions(y, dispersion)
+    # Check y
+    y = np.asarray(y, order='F')
+    if not np.issubdtype(y.dtype, np.number):
+        raise ValueError("count matrix must be numeric")
 
-    # Check weights
-    weights = _compressWeights(y, weights)
+    # Check prior_count
+    prior_count = _compressPrior(y, prior_count)
 
-    # Check offsets
+    # Check lib_size and offset
+    # If offsets are provided, they must have a similar average to log(lib_size)
+    # for the results to be meaningful as logCPM values
     offset = _compressOffsets(y, lib_size=lib_size, offset=offset)
 
-    # Check prior counts
-    prior_count = _compressPrior(y, prior_count)
-
-    # Retrieve GLM fitting parameters
-    maxit = signature(mglmOneGroup).parameters['maxit'].default
-    tol = signature(mglmOneGroup).parameters['tol'].default
+    # Adding the prior count
+    (out_y, out_offset) = cxx_add_prior_count(y, offset, prior_count)
+    out_offset = makeCompressedMatrix(out_offset, y.shape, byrow=True)
+    return (out_y, out_offset)
 
-    # Calling the C++ code
-    return cxx_ave_log_cpm(y, offset, prior_count, dispersion, weights, maxit, tol)
```

### Comparing `inmoose-0.1.1/inmoose/edgepy/dispCoxReidInterpolateTagwise.py` & `inmoose-0.2.0/inmoose/edgepy/mglmOneGroup.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,90 +12,98 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #-----------------------------------------------------------------------------
 
-# This file is based on the file 'R/dispCoxReidInterpolateTagwise.R' of the Bioconductor edgeR package (version 3.38.4).
+# This file is based on the file 'R/mglmOneGroup.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
+import logging
 import numpy as np
-from math import floor
 
-from .adjustedProfileLik import adjustedProfileLik
-from .aveLogCPM import aveLogCPM
-from .makeCompressedMatrix import _compressOffsets, _compressWeights
-from .maximizeInterpolant import maximizeInterpolant
-from .movingAverageByCol import movingAverageByCol
-from .edgepy_cpp import cxx_maximize_interpolant
+from .makeCompressedMatrix import _compressDispersions, _compressOffsets, _compressWeights
+from .utils import _isAllZero
+from .edgepy_cpp import cxx_fit_one_group
 
-def dispCoxReidInterpolateTagwise(y, design, dispersion, offset=None, trend=True, AveLogCPM=None, min_row_sum=5, prior_df=10, span=0.3, grid_npts=11, grid_range=(-6,6), weights=None):
+def mglmOneGroup(y, dispersion=0, offset=0, weights=None, coef_start=None, maxit=50, tol=1e-10, verbose=False):
     """
-    Estimate tagwise NB dispersions using weighted Cox-Reid Adjusted Profile-likelihood and cubic spline interpolation over a tagwise grid.
+    Fit single-group negative-binomial GLMs genewise.
+
+    This is a low-level work-horse used by higher-level functions, especially
+    :func:`glmFit`. Most users will not need to call this function directly.
+
+    This function fits a negative binomial GLM to each row of :code:`y`. The
+    row-wise GLMs all have the same design matrix but possibly different
+    dispersions, offsets and weights. It is low-level in that it
+    operates on atomic objects (matrices and vectors).
+
+    This function fits an intercept only moel to each response vector. In other
+    words, it treats all the libraries as belonging to one group. It implements
+    Fisher scoring with a score-statistic stopping criterion for each gene.  It
+    treats the dispersion parameter of the negative binomial distribution as a
+    known input.  Excellent starting values are available for the null model so
+    this function seldom has any problems with convergence. It is used by other
+    functions to compute the overall abundance for each gene.
+
+    Arguments
+    ---------
+    y : array_like
+        matrix of negative binomial counts. Rows for genes and columns for
+        libraries.
+    dispersion : float or array_like
+        scalar or vector giving the dispersion parameter for each GLM. Can be a
+        scalar giving one value for all genes, or a vector of length equal to
+        the number of genes giving genewise dispersions.
+    offset : array_like
+        vector or matrix giving the offset that is to be included in the log
+        linear model predictor. Can be a scalar, a vector of length equal to the
+        number of libraries, or a matrix of the same shape as :code:`y`.
+    weights : matrix, optional
+        vector or matrix of non-negative quantitative weights. Can be a vector
+        of length equal to the number of libraries, or a matrix of the same
+        shape as :code:`y`.
+    coef_start : array_like, optional
+        matrix of starting values for the linear model coefficient. Number of
+        rows should agree with :code:`y` and a single column. This argument does
+        not usually need to be set as the automatic starting values perform well.
+    maxit : int
+        the maximum number of iterations for the Fisher scoring algorithm. The
+        iteration will be stopped when this limit is reached even if the
+        convergence criterion has not been satisfied.
+    tol : float
+        the convergence tolerance. Convergence if judged successful when the
+        step size falls below :code:`tol` in absolute size.
+
+    Returns
+    -------
+    ndarray
+        vector of coefficients
     """
     # Check y
-    y = np.asarray(y, order='F')
-    (ntags, nlibs) = y.shape
+    # TODO check that y is a matrix and numeric
+    _isAllZero(y)
 
-    # Check design
-    design = np.asarray(design, order='F')
-    if np.linalg.matrix_rank(design) != design.shape[1]:
-        raise ValueError("design matrix must be full column rank")
-    ncoefs = design.shape[1]
-    if ncoefs >= nlibs:
-        raise ValueError("no residual degrees of freedom")
+    # Check dispersion
+    dispersion = _compressDispersions(y, dispersion)
 
     # Check offset
-    lib_size = None
-    if offset is None:
-        lib_size = y.sum(axis=0)
-        offset = np.log(lib_size)
-    if len(offset.shape) == 1:
-        offset = np.full(y.shape, offset, order='F')
-    assert offset.shape == y.shape
-
-    # Check AveLogCPM
-    if AveLogCPM is None:
-        AveLogCPM = aveLogCPM(y, lib_size=lib_size)
-    AveLogCPM = np.asarray(AveLogCPM, order='F')
-
-    # Check dispersion
-    dispersion = np.asanyarray(dispersion, order='F')
-    if len(dispersion.shape) == 0:
-        dispersion = np.full((ntags,), dispersion, order='F')
-    else:
-        if len(dispersion) != ntags:
-            raise ValueError("length of dispersion does not match nrow(y)")
-
-    # Apply min_row_sum and use input dispersion for small count tags
-    i = y.sum(axis=1) >= min_row_sum
-    if np.logical_not(i).any():
-        if i.any():
-            dispersion[i] = dispCoxReidInterpolateTagwise(y=y[i,:], design=design, offset=offset[i,:], dispersion=dispersion[i], AveLogCPM=AveLogCPM[i], grid_npts=grid_npts, min_row_sum=0, prior_df=prior_df, span=span, trend=trend, weights=(weights[i,:] if weights is not None else None))
-        return dispersion
-
-    # Posterior profile likelihood
-    prior_n = prior_df / (nlibs-ncoefs)
-    spline_pts = [grid_range[0] + i*(grid_range[1]-grid_range[0])/(grid_npts-1) for i in range(grid_npts)]
-    apl = np.zeros((ntags, grid_npts), order='F')
-    # anticipate the calls to _compress* in adjustedProfileLik
-    y = np.asarray(y, order='F')
     offset = _compressOffsets(y, offset=offset)
+
+    # Check starting values
+    if coef_start is None:
+        coef_start = np.NaN
+    coef_start = np.full((y.shape[0],), coef_start, dtype='double', order='F')
+
+    # Check weights
     weights = _compressWeights(y, weights)
-    for i in range(grid_npts):
-        spline_disp = dispersion * 2**spline_pts[i]
-        apl[:,i] = adjustedProfileLik(spline_disp, y=y, design=design, offset=offset, weights=weights)
-
-    if trend:
-        o = np.argsort(AveLogCPM)
-        oo = np.argsort(o)
-        width = floor(span * ntags)
-        apl_smooth = movingAverageByCol(apl[o,:], width=width)[oo,:]
-    else:
-        apl_smooth = np.full((ntags, grid_npts), apl.mean(axis=0), order='F')
-    apl_smooth = (apl + prior_n*apl_smooth) / (1+prior_n)
-
-    # Tagwise maximization
-    d = maximizeInterpolant(spline_pts, apl_smooth)
-    d = np.asarray(d, order='F')
-    return dispersion * 2**d
+
+    # Fisher scoring iteration
+    output = cxx_fit_one_group(y, offset, dispersion, weights, maxit, tol, coef_start)
+
+    # Convergence achieved for all tags?
+    if np.count_nonzero(output[1]) > 0:
+        logging.debug(f"max iterations exceeded for {np.count_nonzero(output[1])} tags")
+
+    return output[0]
+
```

### Comparing `inmoose-0.1.1/inmoose/edgepy/dropEmptyLevels.py` & `inmoose-0.2.0/inmoose/utils/stats.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #-----------------------------------------------------------------------------
-# Copyright (C) 2008-2022 Yunshun Chen, Aaron TL Lun, Davis J McCarthy, Matthew E Ritchie, Belinda Phipson, Yifang Hu, Xiaobei Zhou, Mark D Robinson, Gordon K Smyth
-# Copyright (C) 2022-2023 Maximilien Colange
+# Copyright (C) 2022-2023 M. Colange
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -12,20 +11,31 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #-----------------------------------------------------------------------------
 
-# This file is based on the file 'R/dropEmptyLevels.R' of the Bioconductor edgeR package (version 3.38.4).
+from scipy.stats import nbinom
 
+def rnbinom(n, size, mu, seed=None):
+    """mimic R rnbinom function, to draw samples from a Negative Binomial distribution.
 
-from ..utils import Factor
+    The (:math:`size`, :math:`p`) parameterization used in R is the same as in scipy.stats:
+    :math:`p = 1 / (1 + \mu/size) = size / (size + \mu)`.
 
-def dropEmptyLevels(x):
+    Arguments
+    ---------
+    n : int or tuple of ints
+        shape of the output. If n = (n1, n2, ..., np) then n1*n2*...*np random samples are drawn.
+    size : float or array-like
+        size parameter of the Negative Binomial distribution.
+        all values must be positive
+    mu : float or array-like
+        mean parameter of the Negative Binomial distribution
+        all values must be positive
+    seed : int, optional
+        pass a seed to the underlying RNG. If `None`, then the RNG is seeded using unpredictable entropy from the system.
+        See the documentation of scipy.stats about RNG seeding for more details.
     """
-    Drop levels of a factor that does not occur
-    """
-    if isinstance(x, Factor):
-        return Factor(x.arr)
-    else:
-        return Factor(x)
+    p = size / (size + mu)
+    return nbinom(size, p).rvs(n, random_state=seed)
```

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/__init__.pxd` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/__init__.pxd`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/add_prior.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior.h` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/add_prior.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior_count.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/add_prior_count.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior_count.h` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/add_prior_count.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/adj_coxreid.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/adj_coxreid.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/ave_log_cpm.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/ave_log_cpm.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/compute_apl.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/compute_apl.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/compute_nbdev.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/compute_nbdev.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/edgepy_cpp.pyx` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/edgepy_cpp.pyx`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/fit_levenberg.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/fit_levenberg.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/fit_levenberg.h` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/fit_levenberg.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/fit_one_group.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/fit_one_group.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/get_one_way_fitted.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/get_one_way_fitted.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/glm.h` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/glm.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/glm_levenberg.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/glm_levenberg.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/glm_one_group.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/glm_one_group.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/initialize_levenberg.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/initialize_levenberg.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/initialize_levenberg.h` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/initialize_levenberg.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/interpolator.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/interpolator.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/interpolator.h` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/interpolator.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/maximize_interpolant.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/maximize_interpolant.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/nbdev.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/nbdev.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/objects.cpp` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/objects.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/objects.h` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/objects.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/utils.h` & `inmoose-0.2.0/inmoose/edgepy/edgepy_cpp/utils.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/makeCompressedMatrix.py` & `inmoose-0.2.0/inmoose/edgepy/makeCompressedMatrix.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/maximizeInterpolant.py` & `inmoose-0.2.0/inmoose/edgepy/maximizeInterpolant.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,16 +21,39 @@
 
 import numpy as np
 
 from .edgepy_cpp import cxx_maximize_interpolant
 
 def maximizeInterpolant(x,y):
     """
-    This function takes an ordered set of spline points and a likelihood matrix where each row corresponds to a tag and each column corresponds to a spline point.
-    It then calculates the position at which the maximum interpolated likelihood occurs for each by solving the derivative of the spline function.
+    Maximize a function given a table of values by spline interpolation.
+
+    Calculate the cubic spline interpolant for each row with the method of
+    Forsythe et al. (1977) [1]_, then calculate the derivatives of the spline
+    segments adjacent to the input with the maximum function value. This allows
+    identification of the maximum of the interpolating spline.
+
+    Arguments
+    ---------
+    x : array_like
+        vector of inputs for the function
+    y : array_like
+        matrix of function values at the values of :code:`x`. Columns correspond
+        to :code:`x` values and each row corresponds to a different function to
+        be maximized.
+
+    Returns
+    -------
+    ndarray
+        vector of input values at which the function maxima occur
+
+    References
+    ----------
+    .. [1] G. E. Forsythe, M. A. Malcolm, C. B. Moler. 1977. Computer Methods
+       for Mathematical Computations. Prentice-Hall.
     """
     x = np.asarray(x, order='F', dtype='double')
     y = np.asarray(y, order='F', dtype='double')
     if len(y.shape) != 2:
         raise ValueError("y is not a matrix: cannot perform interpolation")
     if len(x) != y.shape[1]:
         raise ValueError("number of columns must equal number of spline points")
```

### Comparing `inmoose-0.1.1/inmoose/edgepy/mglmOneWay.py` & `inmoose-0.2.0/inmoose/edgepy/nbinomDeviance.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,95 +12,98 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #-----------------------------------------------------------------------------
 
-# This file is based on the file 'R/mglmOneWay.R' of the Bioconductor edgeR package (version 3.38.4).
+# This file is based on the file 'R/nbinomDeviance.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 import numpy as np
-from ..utils import Factor, asfactor
-from .makeCompressedMatrix import _compressOffsets, _compressDispersions, _compressWeights
-from .mglmOneGroup import mglmOneGroup
-from .edgepy_cpp import cxx_get_one_way_fitted
-from scipy.linalg import solve
+from .makeCompressedMatrix import _compressDispersions, _compressWeights
+from .edgepy_cpp import cxx_compute_nbdev_sum, cxx_compute_nbdev_nosum
 
-def designAsFactor(design):
+def nbinomDeviance(y, mean, dispersion=0, weights=None):
     """
-    Construct a factor from the unique rows of a matrix
-    """
-    design = np.asarray(design, order='F')
-    z = (np.e + np.pi) / 5
-    col = np.full(design.shape, np.arange(design.shape[1]), order='F')
-    means = (design * z**col).mean(axis=1)
-    uniq = np.unique(means)
-    fact = np.zeros(means.shape, dtype='int64', order='F')
-    for i in range(len(uniq)):
-        fact[means == uniq[i]] = i+1
-    return Factor(fact)
-
-def mglmOneWay(y, design=None, group=None, dispersion=0, offset=0, weights=None, coef_start=None, maxit=50, tol=1e-10):
-    """
-    Fit multiple negative binomial GLMs with log link by Fisher scoring with a single explanatory factor in the model
-    """
-    y = np.asarray(y, order='F')
-    (ngenes, nlibs) = y.shape
+    Residual deviances for row-wise negative binomial GLMs.
 
-    offset = _compressOffsets(y, offset=offset)
-    dispersion = _compressDispersions(y, dispersion)
-    weights = _compressWeights(y, weights)
+    This function computes the total residual deviance for each row of :code:`y`,
+    i.e. weighted row sums of the unit deviances.
 
-    # If necessary, the group factor is computed from the design matrix.
-    # However, if group is supplied, we can avoid creating a design matrix altogether.
-    if group is None:
-        if design is None:
-            group = Factor(np.ones((nlibs,)))
-        else:
-            design = np.asarray(design, order='F')
-            group = designAsFactor(design)
-    else:
-        group = asfactor(group)
+    Care is taken to ensure accurate computation in limiting cases when the
+    dispersion is near zero of :code:`mean * dispersion` is very large.
 
-    # Convert factor to integer levels for efficiency
-    levg = group.categories
-    ngroups = len(levg)
-    i = group.__array__()
-
-    if design is not None:
-        if design.shape[1] != ngroups:
-            raise ValueError("design matrix is not equivalent to a oneway layout")
-
-    # Reduce to representative design matrix, based on the column in which each group appears first
-    firstjofgroup = [(i == x).nonzero()[0][0] for x in levg]
-    if design is not None:
-        designunique = design[firstjofgroup,:]
-    else:
-        designunique = None
-
-    # Is it just a group indicator matrix?
-    if np.sum(designunique == 1) == ngroups and np.sum(designunique == 0) == (ngroups-1)*ngroups:
-        design = None
+    See also
+    --------
+    nbinomUnitDeviance
+
+    Arguments
+    ---------
+    y : array_like
+        matrix containing the negative binomial counts, with rows for genes and
+        columns for libraries. A vector will be treated as a matrix with one row.
+    mean : array_like
+        matrix of expected values, of same shape as :code:`y`. A vector will be
+        treated as a matrix with one row.
+    dispersion : array_like
+        vector or matrix of negative binomial dispersions, as in :code:`glmFit`.
+        Can be a scalar, a vector of length equal to the number of rows in
+        :code:`y`, or a matrix of same shape as :code:`y`.
+    weights : array_like, optional
+        vector or matrix of non-negative weights, as in :code:`glmFit`. Can be
+        a scalar, a vector of length equal to the number of columns in :code:`y`,
+        or a matrix of same shape as :code:`y`.
+
+    Returns
+    -------
+    ndarray
+        vector of length equal to the number of rows in :code:`y`
+    """
+    out = _compute_nbdeviance(y=y, mean=mean, dispersion=dispersion, weights=weights, dosum=True)
+    return out
 
-    # If necessary, convert starting values to group fitted values
-    if design is not None and coef_start is not None:
-        coef_start = coef_start @ designunique.T
+def _compute_nbdeviance(y, mean, dispersion, weights, dosum):
+    y = np.asarray(y, order='F')
+    mean = np.asanyarray(mean, order='F', dtype='double')
+    dispersion = np.asanyarray(dispersion, order='F', dtype='double')
 
-    # Cycle through groups
-    beta = np.zeros((ngenes, ngroups), order='F', dtype='double')
-    for g in range(ngroups):
-        j = np.nonzero(i == (g+1))[0]
-        beta[:, g] = mglmOneGroup(y[:,j], dispersion=dispersion[:,j], offset=offset[:,j], weights=weights[:,j] if weights is not None else None, coef_start=coef_start[:,g] if coef_start is not None else None, maxit=maxit, tol=tol)
+    # Check y. May be matrix or vector
+    if len(y.shape) == 2:
+        if len(mean.shape) != 2:
+            raise ValueError("y is a matrix but mean is not")
+    else:
+        n = y.shape[0]
+        y = y.reshape((1,n))
+        if len(mean.shape) == 2:
+            raise ValueError("mean is a matrix but y is not")
+        else:
+            if mean.shape[0] == n:
+                mean = mean.reshape((1,n))
+            else:
+                raise ValueError("length of mean differs from that of y")
 
-    # Reset -inf values to finite values to simplify calculations downstream
-    beta = np.where(beta > -1e8, beta, -1e8)
+        if len(dispersion.shape) == 2:
+            raise ValueError("dispersion is a matrix but y is not")
+        else:
+            if len(dispersion.shape) > 0 and dispersion.shape[0] == n:
+                dispersion = dispersion.reshape((1,n))
+            else:
+                raise ValueError("length of dispersion differs from that of y")
+
+    # Check mean
+    if y.shape != mean.shape:
+        raise ValueError("mean should have the same dimensions as y")
+    mean = mean.astype(np.float64, copy=False)
 
-    # Fitted values from group-wise beta's
-    mu = cxx_get_one_way_fitted(beta, offset, i-1)
+    # Check dispersion (can be tagwise (i.e. rowwise) or observation-wise)
+    dispersion = _compressDispersions(y, dispersion)
 
-    # If necessary, reformat the beta's to reflect the original design.
-    if design is not None:
-        beta = solve(designunique, beta.T).T
+    # Check weights
+    weights = _compressWeights(y, weights)
 
-    return (beta, mu)
+    # Compute matrix of unit deviances, or residual deviance per gene, depending on `dosum`
+    if dosum:
+        return cxx_compute_nbdev_sum(y, mean, dispersion, weights)
+    else:
+        return cxx_compute_nbdev_nosum(y, mean, dispersion, weights)
```

### Comparing `inmoose-0.1.1/inmoose/edgepy/movingAverageByCol.py` & `inmoose-0.2.0/inmoose/edgepy/movingAverageByCol.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,30 +15,46 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #-----------------------------------------------------------------------------
 
 # This file is based on the file 'R/movingAverageByCol.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
+import logging
 import numpy as np
 from math import ceil, floor
-from warnings import warn
 
 def movingAverageByCol(x, width=5, full_length=True):
     """
-    Moving average smoother for columns of a matrix
+    Moving average smoother for matrix columns.
+
+    Arguments
+    ---------
+    x : array_like
+        numeric matrix
+    width : int
+        width of window of rows to be averaged
+    full_length : bool
+        whether the output should have the same number of rows as the input
+
+    Returns
+    -------
+    ndarray
+        numeric matrix with smoothed values. If :code:`full_length = True`, of
+        same shape as :code:`x`. If :code:`full_length = False`, has
+        :code:`width-1` fewer rows than :code:`x`.
     """
     x = np.asanyarray(x, order='F')
     width = int(width)
     if width <= 1:
         return x
     (n,m) = x.shape
     if width > n:
         width = n
-        warn("reducing moving average width to x.shape[0]")
+        logging.warnings.warn("reducing moving average width to x.shape[0]")
 
     if full_length:
         half1 = ceil(width/2)
         half2 = floor(width/2)
         x = np.vstack([np.zeros((half1, m)), x, np.zeros((half2, m))])
     else:
         if width == n:
```

### Comparing `inmoose-0.1.1/inmoose/edgepy/predFC.py` & `inmoose-0.2.0/inmoose/edgepy/validDGEList.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,40 +12,42 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #-----------------------------------------------------------------------------
 
-# This file is based on the file 'R/predFC.R' of the Bioconductor edgeR package (version 3.38.4).
+# This file is based on the file 'R/validDGEList.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 import numpy as np
-from warnings import warn
+from ..utils import gl
 
-from .addPriorCount import addPriorCount
-
-def predFC_DGEList(self, design, prior_count=0.125, offset=None, dispersion=None, weights=None):
-    if offset is None:
-        offset = self.getOffset()
-    if dispersion is None:
-        dispersion = self.getDispersion()
-    if dispersion is None:
-        dispersion = 0
-        warn("dispersion set to zero")
+def validDGEList(y):
+    """
+    Check for standard components of DGEList object
 
-    return predFC(y=self.counts, design=design, prior_count=prior_count, offset=offset, dispersion=dispersion, weights=weights)
+    NB: Modifies :code:`y` in place.
 
-def predFC(y, design, prior_count=0.125, offset=None, dispersion=0, weights=None):
-    """
-    Shrink log-fold-changes towards zero by augmenting data counts
+    Arguments
+    ---------
+    y : DGEList
+        the object to check for validity
+
+    Returns
+    -------
+    DGEList
+        the input :code:`y`, with missing components added
     """
-    from .glmFit import glmFit
-    # Add prior counts in proportion to library size
-    (out_y, out_offset) = addPriorCount(y, offset=offset, prior_count=prior_count)
-
-    # Check design
-    design = np.asarray(design, order='F')
-
-    # Return matrix of coefficients on log2 scale
-    g = glmFit(out_y, design, offset=out_offset, dispersion=dispersion, prior_count=0, weights=weights)
-    return g.coefficients / np.log(2)
+    if y.counts is None:
+        raise RuntimeError("No count matrix")
+    y.counts = np.asarray(y.counts, order='F')
+    nlib = y.counts.shape[1]
+    if (y.samples.group.values == None).any():
+        y.samples.group = gl(1, nlib)
+    if (y.samples.lib_size.values == None).any():
+        y.samples.lib_size = y.counts.sum(axis=0)
+    if (y.samples.norm_factors.values == None).any():
+        y.samples.norm_factors = np.ones(nlib)
+
+    return y
+
```

### Comparing `inmoose-0.1.1/inmoose/edgepy/splitIntoGroups.py` & `inmoose-0.2.0/inmoose/edgepy/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,30 +12,40 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #-----------------------------------------------------------------------------
 
-# This file is based on the file 'R/splitIntoGroups.R' of the Bioconductor edgeR package (version 3.38.4).
+# This file is based on the file 'R/DGEList.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
-from .dropEmptyLevels import dropEmptyLevels
 import numpy as np
 
-def splitIntoGroups_DGEList(self):
-    group = self.samples.group
-    return splitIntoGroups(self.counts, group=group)
-
-def splitIntoGroups(y, group=None):
-    # Check y
-    (ntags, nlibs) = y.shape
-
-    # Check group
-    if group is None:
-        group = np.ones(nlibs)
-    if len(group) != nlibs:
-        raise ValueError("Incorrect length of group.")
-    group = dropEmptyLevels(group)
+def _isAllZero(y):
+    """
+    Check for all-zero, negative, Nan and infinite counts
+
+    This function check if :code:`y` is all zero, and raises an error if it
+    contains negative, NaN or infinite values.
+
+    Arguments
+    ---------
+    y : array_like
+        matrix of counts
+
+    Returns
+    -------
+    bool
+        whether :code:`y` only contains zeroes
+    """
+    if len(y) == 0:
+        return False
+    check_range = (np.amin(y), np.nanmax(y))
+    if np.isnan(check_range[0]):
+        raise ValueError("NaN counts are not allowed")
+    if check_range[0] < 0:
+        raise ValueError("negative counts are not allowed")
+    if np.isinf(check_range[1]):
+        raise ValueError("infinite counts are not allowed")
+    return check_range[1] == 0
 
-    out = [y.T[group == i].T for i in np.unique(group)]
-    return out
```

### Comparing `inmoose-0.1.1/inmoose/edgepy/stats.py` & `inmoose-0.2.0/inmoose/edgepy/stats.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/inmoose/edgepy/systematicSubset.py` & `inmoose-0.2.0/inmoose/edgepy/systematicSubset.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,16 +20,27 @@
 
 
 import numpy as np
 from math import floor
 
 def systematicSubset(n, order_by):
     """
-    Take a systematic subset of indices,
-    stratified by a ranking variable
+    Take a systematic subset of indices stratified by a ranking variable
+
+    Arguments
+    ---------
+    n : int
+        the size of the subset
+    order_by : array_like
+        vector of the values by which the indices are ordered
+
+    Returns
+    -------
+    ndarray
+        a vector of size :code:`n`
     """
     ntotal = len(order_by)
     sampling_ratio = floor(ntotal / n)
     if sampling_ratio <= 1:
         return np.arange(ntotal)
     i1 = floor(sampling_ratio / 2)
     i = np.arange(i1, ntotal, step=sampling_ratio)
```

### Comparing `inmoose-0.1.1/inmoose/utils/factor.py` & `inmoose-0.2.0/inmoose/utils/factor.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,40 +16,45 @@
 #-----------------------------------------------------------------------------
 
 
 import numpy as np
 from pandas import Categorical
 
 class Factor(Categorical):
-    """A class to represent a factor, as in R.
+    """
+    A class to represent a factor, as in R.
 
-    It is essentially a :obj:`pandas.Categorical` object, with additional methods to mimic R API.
+    It is essentially a :obj:`pandas.Categorical` object, with additional
+    methods to mimic R API.
     """
 
     def __init__(self, arr):
-        """Constructs a Factor instance from an array
         """
-        super().__init__(arr)
+        Constructs a Factor instance from an array
 
-#    def __len__(self):
-#        return len(self.arr)
-#
-#    def __eq__(self, other):
-#        if type(other) is type(self):
-#            return np.array_equal(self.arr, other.arr)
-#        else:
-#            return NotImplemented
+        Arguments
+        ---------
+        arr : array_like
+            a list of factors
+        """
+
+        super().__init__(arr)
 
     def droplevels(self):
         """
         drop unused levels
         """
+
         return Factor(self.__array__())
 
     def nlevels(self):
+        """
+        the number of levels
+        """
+
         return len(self.categories)
 
 def asfactor(g):
     if type(g) is Factor:
         return g
     else:
         return Factor(g)
```

### Comparing `inmoose-0.1.1/inmoose.egg-info/PKG-INFO` & `inmoose-0.2.0/inmoose.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: inmoose
-Version: 0.1.1
+Version: 0.2.0
 Summary: InMoose: the Integrated Multi Omic Open Source Environment
-Home-page: https://github.com/epigenelabs/inmoose
-Author: Maximilien Colange
-Author-email: maximilien@epigenelabs.com
+Author-email: Maximilien Colange <maximilien@epigenelabs.com>
+Project-URL: Source, https://github.com/epigenelabs/inmoose
+Project-URL: Documentation, https://inmoose.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: doc
 License-File: LICENSE
 
+[![Documentation Status](https://readthedocs.org/projects/inmoose/badge/?version=latest)](https://inmoose.readthedocs.io/en/latest/?badge=latest)
+
 # InMoose
 
 InMoose is the **In**tegrated **M**ulti **O**mic **O**pen **S**ource **E**nvironment.
 It is a collection of tools for the analysis of omic data.
 
-Currently it focuses on transcriptomic data.
-
 # Installation
 
 You can install InMoose directly with:
 
 ```
 pip install inmoose
 ```
@@ -29,23 +31,23 @@
 # Batch Effect Correction
 
 InMoose provides features to correct technical biases, also called batch
 effects, in transcriptomic data:
 - for microarray data, InMoose supersedes pyCombat [1], a Python 3
   implementation of ComBat [2], one of the most widely used tool for batch effect
   correction on microarray data.
-- for RNASeq, InMoose features a port to Python3 of ComBat-Seq [3], one the most
-  widely used tool for batch effect correction on RNASeq data.
+- for RNASeq, InMoose features a port to Python3 of ComBat-Seq [3], one of the
+  most widely used tool for batch effect correction on RNASeq data.
 
 To use these functions, simply import them and call them with default
 parameters:
 ```python
-from inmoose.batch import pycombat, pycombat_seq
+from inmoose.pycombat import pycombat_norm, pycombat_seq
 
-microarray_corrected = pycombat(microarray_data, microarray_batches)
+microarray_corrected = pycombat_norm(microarray_data, microarray_batches)
 rnaseq_corrected = pycombat_seq(rnaseq_data, rnaseq_batches)
 ```
 
 * `microarray_data`, `rnaseq_data`: the expression matrices, containing the
   information about the gene expression (rows) for each sample (columns).
 * `microarray_batches`, `rnaseq_batches`: list of batch indices, describing the
   batch for each sample. The list of batches should contain as many elements as
```

### Comparing `inmoose-0.1.1/inmoose.egg-info/SOURCES.txt` & `inmoose-0.2.0/inmoose.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 inmoose/__init__.py
-inmoose/__version__.py
 inmoose.egg-info/PKG-INFO
 inmoose.egg-info/SOURCES.txt
 inmoose.egg-info/dependency_links.txt
 inmoose.egg-info/requires.txt
 inmoose.egg-info/top_level.txt
-inmoose/batch/__init__.py
-inmoose/batch/covariates.py
-inmoose/batch/helper_seq.py
-inmoose/batch/pycombat.py
-inmoose/batch/pycombat_seq.py
 inmoose/common_cpp/common_cpp.pyx
 inmoose/common_cpp/matrix.cpp
 inmoose/common_cpp/matrix.h
 inmoose/edgepy/DGEGLM.py
 inmoose/edgepy/DGEList.py
 inmoose/edgepy/__init__.py
 inmoose/edgepy/addPriorCount.py
 inmoose/edgepy/adjustedProfileLik.py
 inmoose/edgepy/aveLogCPM.py
 inmoose/edgepy/dispCoxReid.py
 inmoose/edgepy/dispCoxReidInterpolateTagwise.py
-inmoose/edgepy/dropEmptyLevels.py
 inmoose/edgepy/estimateGLMCommonDisp.py
 inmoose/edgepy/estimateGLMTagwiseDisp.py
 inmoose/edgepy/glmFit.py
 inmoose/edgepy/makeCompressedMatrix.py
 inmoose/edgepy/maximizeInterpolant.py
 inmoose/edgepy/mglmLevenberg.py
 inmoose/edgepy/mglmOneGroup.py
@@ -64,22 +58,32 @@
 inmoose/edgepy/edgepy_cpp/interpolator.cpp
 inmoose/edgepy/edgepy_cpp/interpolator.h
 inmoose/edgepy/edgepy_cpp/maximize_interpolant.cpp
 inmoose/edgepy/edgepy_cpp/nbdev.cpp
 inmoose/edgepy/edgepy_cpp/objects.cpp
 inmoose/edgepy/edgepy_cpp/objects.h
 inmoose/edgepy/edgepy_cpp/utils.h
+inmoose/pycombat/__init__.py
+inmoose/pycombat/covariates.py
+inmoose/pycombat/helper_seq.py
+inmoose/pycombat/pycombat_norm.py
+inmoose/pycombat/pycombat_seq.py
 inmoose/utils/__init__.py
 inmoose/utils/factor.py
 inmoose/utils/stats.py
-tests/test_DGEList.py
-tests/test_aveLogCPM.py
-tests/test_compressMatrix.py
-tests/test_dispersion.py
-tests/test_factor.py
-tests/test_glm.py
-tests/test_lik.py
-tests/test_mglm.py
-tests/test_objects.py
-tests/test_pycombat.py
-tests/test_pycombatseq.py
-tests/test_stats.py
+tests/__init__.py
+tests/edgepy/__init__.py
+tests/edgepy/test_DGEList.py
+tests/edgepy/test_aveLogCPM.py
+tests/edgepy/test_compressMatrix.py
+tests/edgepy/test_dispersion.py
+tests/edgepy/test_glm.py
+tests/edgepy/test_lik.py
+tests/edgepy/test_mglm.py
+tests/edgepy/test_objects.py
+tests/edgepy/test_stats.py
+tests/pycombat/__init__.py
+tests/pycombat/test_covariates.py
+tests/pycombat/test_pycombat.py
+tests/pycombat/test_pycombatseq.py
+tests/utils/__init__.py
+tests/utils/test_factor.py
```

### Comparing `inmoose-0.1.1/setup.py` & `inmoose-0.2.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,11 @@
-from codecs import open
-import os
 import sys
 import numpy
 from setuptools import Extension, setup
 
-here = os.path.abspath(os.path.dirname(__file__))
-
-about: dict = dict()
-with open(os.path.join(here, "inmoose", "__version__.py"), "r", "utf-8") as fp:
-    exec(fp.read(), about)
-
-with open(os.path.join(here, "README.md"), "r") as fh:
-    long_description = fh.read()
-
 cxx_compile_flags = ["-std=c++17"]
 macros = [("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION")]
 profiling = False
 linetrace = False
 if "--profile" in sys.argv:
     profiling = True
     linetrace = True
@@ -51,37 +40,17 @@
     include_dirs = [numpy.get_include(), 'inmoose/common_cpp/'],
     extra_compile_args = cxx_compile_flags,
     define_macros = macros,
     )
 
 
 setup(
-    install_requires=[
-        "mpmath>=1.1.0",
-        "numpy>=1.18.5",
-        "pandas",
-        "patsy",
-        "scipy",
-    ],
-    name="inmoose",
-    version=about["__version__"],
-    author="Maximilien Colange",
-    author_email="maximilien@epigenelabs.com",
-    description="InMoose: the Integrated Multi Omic Open Source Environment",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url = "https://github.com/epigenelabs/inmoose",
-    classifiers = [
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-        "Topic :: Scientific/Engineering :: Bio-Informatics",
-    ],
     packages = [
         "inmoose",
-        "inmoose/batch",
+        "inmoose/pycombat",
         "inmoose/common_cpp",
         "inmoose/edgepy",
         "inmoose/edgepy/edgepy_cpp",
         "inmoose/utils",
     ],
     package_data = {
         "inmoose/edgepy/edgepy_cpp": [
```

### Comparing `inmoose-0.1.1/tests/test_DGEList.py` & `inmoose-0.2.0/tests/edgepy/test_DGEList.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/tests/test_aveLogCPM.py` & `inmoose-0.2.0/tests/edgepy/test_aveLogCPM.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/tests/test_compressMatrix.py` & `inmoose-0.2.0/tests/edgepy/test_compressMatrix.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 import numpy as np
 
 from inmoose.edgepy.makeCompressedMatrix import makeCompressedMatrix
 
-class test_DGEList(unittest.TestCase):
+class Test(unittest.TestCase):
     def test_makeCompressedMatrix(self):
         self.assertTrue(np.array_equal(makeCompressedMatrix(42, dims=(2,3), byrow=True), np.full((2,3), 42)))
         self.assertTrue(np.array_equal(makeCompressedMatrix(42, dims=(2,3), byrow=False), np.full((2,3), 42)))
 
         ref = np.array([[1,2,3] for i in range(2)])
         self.assertTrue(np.array_equal(makeCompressedMatrix([1,2,3], dims=(2,3), byrow=True), ref))
         self.assertTrue(np.array_equal(makeCompressedMatrix([1,2,3], dims=(3,2), byrow=False), ref.T))
```

### Comparing `inmoose-0.1.1/tests/test_dispersion.py` & `inmoose-0.2.0/tests/edgepy/test_dispersion.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/tests/test_factor.py` & `inmoose-0.2.0/tests/utils/test_factor.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/tests/test_glm.py` & `inmoose-0.2.0/tests/edgepy/test_glm.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/tests/test_lik.py` & `inmoose-0.2.0/tests/edgepy/test_lik.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 import numpy as np
 
 from inmoose.utils import rnbinom
 from inmoose.edgepy import DGEList, adjustedProfileLik
 
-class test_dispersion(unittest.TestCase):
+class test_APL(unittest.TestCase):
     def setUp(self):
         y = np.array(rnbinom(80, size=5, mu=20, seed=42)).reshape((20,4))
         y = np.vstack(([0,0,0,0], [0,0,2,2], y))
         self.group = np.array([1,1,2,2])
         self.d = DGEList(counts=y, group=self.group, lib_size=np.arange(1001,1005))
 
     def test_adjustedProfileLik(self):
```

### Comparing `inmoose-0.1.1/tests/test_mglm.py` & `inmoose-0.2.0/tests/edgepy/test_mglm.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/tests/test_objects.py` & `inmoose-0.2.0/tests/edgepy/test_objects.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.1/tests/test_pycombat.py` & `inmoose-0.2.0/tests/pycombat/test_pycombat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,40 @@
 import unittest
 import numpy as np
 import pandas as pd
 
-from inmoose.batch.pycombat import model_matrix, all_1
-from inmoose.batch.pycombat import compute_prior, postmean, postvar, it_sol, int_eprior
-from inmoose.batch.pycombat import check_mean_only, define_batchmod, check_ref_batch, treat_batches, treat_covariates, check_NAs
-from inmoose.batch.pycombat import calculate_mean_var, calculate_stand_mean
-from inmoose.batch.pycombat import standardise_data, fit_model, adjust_data
-from inmoose.batch import pycombat
+from inmoose.pycombat.covariates import make_design_matrix
+from inmoose.pycombat.pycombat_norm import check_mean_only, check_NAs
+from inmoose.pycombat.pycombat_norm import compute_prior, postmean, postvar, it_sol, int_eprior
+from inmoose.pycombat.pycombat_norm import calculate_mean_var, calculate_stand_mean
+from inmoose.pycombat.pycombat_norm import standardise_data, fit_model, adjust_data
+from inmoose.pycombat import pycombat_norm
 
 class test_pycombat(unittest.TestCase):
 
     @classmethod
     def setUpClass(self):
         self.batch = np.asarray([1,1,1,2,2,3,3,3,3])
-        # matrix = np.transpose(np.asmatrix([np.random.normal(size=1000,loc=3,scale=1),np.random.normal(size=1000,loc=3,scale=1),np.random.normal(size=1000,loc=3,scale=1),
-        #                       np.random.normal(size=1000,loc=2,scale=0.6),np.random.normal(size=1000,loc=2,scale=0.6),
-        #                       np.random.normal(size=1000,loc=4,scale=1),np.random.normal(size=1000,loc=4,scale=1),np.random.normal(size=1000,loc=4,scale=1),np.random.normal(size=1000,loc=4,scale=1)]))
         matrix = np.transpose([np.random.normal(size=1000,loc=3,scale=1),np.random.normal(size=1000,loc=3,scale=1),np.random.normal(size=1000,loc=3,scale=1),
                               np.random.normal(size=1000,loc=2,scale=0.6),np.random.normal(size=1000,loc=2,scale=0.6),
                               np.random.normal(size=1000,loc=4,scale=1),np.random.normal(size=1000,loc=4,scale=1),np.random.normal(size=1000,loc=4,scale=1),np.random.normal(size=1000,loc=4,scale=1)])
 
         self.matrix = pd.DataFrame(data=matrix,columns=["sample_"+str(i+1) for i in range(9)],index=["gene_"+str(i+1) for i in range(1000)])
-        self.matrix_adjusted = pycombat(self.matrix, self.batch)
+        self.matrix_adjusted = pycombat_norm(self.matrix, self.batch)
 
         # useful constants for unit testing
         ref_batch = None
         mean_only = False
         par_prior = False
         precision = None
-        mod = []
+        mod = None
         self.dat = self.matrix.values
-        #batchmod = define_batchmod(batch)
-        batchmod = model_matrix(list(self.batch), intercept=False, drop_first=False)
-        ref,self.batchmod = check_ref_batch(ref_batch,self.batch,batchmod)
-        self.n_batch, self.batches, self.n_batches, self.n_array = treat_batches(self.batch)
-        self.design = treat_covariates(self.batchmod, mod, ref, self.n_batch)
+        design, self.batchmod, _, self.batches, self.n_batches, self.n_batch, self.n_array, ref = make_design_matrix(self.dat, self.batch, None, mod, True, ref_batch)
+        self.design = np.transpose(design)
+
         NAs = check_NAs(self.dat)
         self.B_hat, self.grand_mean, self.var_pooled = calculate_mean_var(self.design, self.batches, ref, self.dat, NAs, self.n_batches, self.n_batch, self.n_array)
         self.stand_mean = calculate_stand_mean(self.grand_mean, self.n_array, self.design, self.n_batch,self.B_hat)
         self.s_data = standardise_data(self.dat, self.stand_mean, self.var_pooled, self.n_array)
         self.gamma_star, self.delta_star, self.batch_design = fit_model(self.design,self.n_batch, self.s_data, self.batches, mean_only, par_prior, precision, ref, NAs)
         self.bayes_data = adjust_data(self.s_data, self.gamma_star, self.delta_star, self.batch_design, self.n_batches, self.var_pooled, self.stand_mean, self.n_array, ref, self.batches, self.dat)
 
@@ -57,56 +52,21 @@
 
     #def test_it_sol(self):
     #    ()
 
     #def test_int_eprior(self):
     #    ()
 
-    def test_model_matrix(self):
-        model_matrix_test = model_matrix([1,1,0,1,0])
-        self.assertEqual(np.shape(model_matrix_test), (5,2))
-        self.assertEqual(list(model_matrix_test[0]), [1.0,1.0])
-
-    def test_all_1(self):
-        self.assertTrue(all_1(np.array([1,1,1,1,1])))
-
-        self.assertFalse(all_1(np.array([1,1,1,1,0])))
-        self.assertFalse(all_1(np.array([0,0,0,0,0])))
-
-        # this test to show the limit of the method we use
-        self.assertFalse(all_1(np.array([1.5,0.5,1,1,1])))
-
 
     @unittest.skip("automate the verification")
     def test_check_mean_only(self):
         check_mean_only(True)
         check_mean_only(False)
         print("Only one line of text should have been printed above.")
 
-    def test_define_batchmod(self):
-        self.assertEqual(np.shape(define_batchmod(self.batch)), (9,3))
-
-    def test_check_ref_batch(self):
-        self.assertEqual(check_ref_batch(1,self.batch,self.batchmod), (0, self.batchmod))
-        self.assertEqual(check_ref_batch(2,self.batch,self.batchmod), (1, self.batchmod))
-        print("Using batch 1 then 2. Above lines should inform on that.")
-        self.assertEqual(check_ref_batch(None,self.batch,self.batchmod), (None, self.batchmod))
-
-    def test_treat_batches(self):
-        self.assertEqual(self.n_batch, 3)
-        self.assertEqual(self.batches[0].tolist(), [0,1,2])
-        self.assertEqual(self.batches[1].tolist(), [3,4])
-        self.assertEqual(self.batches[2].tolist(), [5,6,7,8])
-        self.assertEqual(self.n_batches, [3,2,4])
-        self.assertEqual(self.n_array, 9)
-
-    def test_treat_covariates(self):
-        batchmod = define_batchmod(self.batch)
-        self.assertEqual(np.sum(self.design - np.transpose(batchmod)), 0)
-
     def test_check_NAs(self):
         self.assertFalse(check_NAs([0,1,2]))
 
     def test_calculate_mean_var(self):
         self.assertEqual(np.shape(self.B_hat)[0], np.shape(self.design)[0])
         self.assertEqual(np.shape(self.grand_mean)[0], np.shape(self.dat)[0])
         self.assertEqual(np.shape(self.var_pooled)[0], np.shape(self.dat)[0])
```

### Comparing `inmoose-0.1.1/tests/test_pycombatseq.py` & `inmoose-0.2.0/tests/pycombat/test_pycombatseq.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 import numpy as np
 
 from inmoose.utils import rnbinom
-from inmoose.batch import pycombat_seq
+from inmoose.pycombat import pycombat_seq
 
 class test_pycombatseq(unittest.TestCase):
 
     def setUp(self):
         y = np.array(rnbinom(80, size=5, mu=20, seed=42)).reshape((20,4))
         self.y = np.vstack(([0,0,0,0], [0,0,2,2], y))
         self.batch = np.array([1,1,2,2])
```

### Comparing `inmoose-0.1.1/tests/test_stats.py` & `inmoose-0.2.0/tests/edgepy/test_stats.py`

 * *Files identical despite different names*

