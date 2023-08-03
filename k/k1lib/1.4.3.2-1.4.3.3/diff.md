# Comparing `tmp/k1lib-1.4.3.2.tar.gz` & `tmp/k1lib-1.4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k1lib-1.4.3.2.tar", last modified: Thu Aug  3 08:00:19 2023, max compression
+gzip compressed data, was "k1lib-1.4.3.3.tar", last modified: Thu Aug  3 08:05:00 2023, max compression
```

## Comparing `k1lib-1.4.3.2.tar` & `k1lib-1.4.3.3.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:00:19.355949 k1lib-1.4.3.2/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     1049 2023-08-02 00:51:20.000000 k1lib-1.4.3.2/LICENSE
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3429 2023-08-03 08:00:19.355949 k1lib-1.4.3.2/PKG-INFO
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:00:19.343949 k1lib-1.4.3.2/k1lib/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     1441 2023-05-26 17:16:37.000000 k1lib-1.4.3.2/k1lib/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    83638 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/_baseClasses.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    25641 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/_basics.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8208 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/_context.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:00:19.343949 k1lib-1.4.3.2/k1lib/_hidden/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        0 2021-08-11 18:19:53.000000 k1lib-1.4.3.2/k1lib/_hidden/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       79 2021-08-11 18:19:53.000000 k1lib-1.4.3.2/k1lib/_hidden/hiddenFile.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4314 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/_higher.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3085 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/_k1a.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20567 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/_learner.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:00:19.343949 k1lib-1.4.3.2/k1lib/_mo/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      615 2021-10-24 23:32:21.000000 k1lib-1.4.3.2/k1lib/_mo/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    24015 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/_mo/atom.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    18173 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/_mo/parseM.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5631 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/_mo/substance.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15454 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/_mo/system.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    36997 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/_monkey.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5575 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/_perlin.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:00:19.347949 k1lib-1.4.3.2/k1lib/callbacks/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      378 2021-10-30 05:51:17.000000 k1lib-1.4.3.2/k1lib/callbacks/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31963 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/callbacks.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5455 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/confusionMatrix.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2245 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/core.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    19517 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/hookModule.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7488 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/hookParam.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5728 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/landscape.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14525 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/limits.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:00:19.347949 k1lib-1.4.3.2/k1lib/callbacks/lossFunctions/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       30 2021-10-27 12:39:02.000000 k1lib-1.4.3.2/k1lib/callbacks/lossFunctions/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3695 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/lossFunctions/accuracy.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5968 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/lossFunctions/shorts.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    10038 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/loss_accuracy.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6002 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/paramFinder.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5311 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/profiler.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:00:19.347949 k1lib-1.4.3.2/k1lib/callbacks/profilers/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       45 2021-08-11 18:19:53.000000 k1lib-1.4.3.2/k1lib/callbacks/profilers/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     9311 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/profilers/computation.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4069 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/profilers/io.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7368 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/profilers/memory.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6971 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/profilers/time.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4242 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/progress.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4370 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/recorder.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8363 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/callbacks/shorts.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:00:19.351949 k1lib-1.4.3.2/k1lib/cli/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      975 2023-07-13 16:14:07.000000 k1lib-1.4.3.2/k1lib/cli/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31282 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/_applyCl.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    13909 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/bio.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5162 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/cif.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    39336 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/conv.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    50607 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/filt.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8480 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/gb.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    12136 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/grep.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    35488 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/init.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    69938 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/inp.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14704 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/ktree.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7467 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/kxml.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15993 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/lsext.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2977 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/mgi.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    18005 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/models.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)   125028 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/modifier.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      735 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/mol.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5822 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/nb.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6311 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/optimizations.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20026 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/output.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3042 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/sam.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    72596 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/structural.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15949 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/trace.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    41733 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/typehint.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    49466 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/cli/utils.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    21263 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/eqn.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    12310 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/fmt.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    10890 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/graphEqn.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5180 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/imports.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:00:19.351949 k1lib-1.4.3.2/k1lib/k1ui/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)  2453826 2023-01-19 22:50:00.000000 k1lib-1.4.3.2/k1lib/k1ui/256.model.state_dict.pth
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       20 2023-01-19 22:00:40.000000 k1lib-1.4.3.2/k1lib/k1ui/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    88758 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/k1ui/main.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)   304735 2023-01-17 19:16:23.000000 k1lib-1.4.3.2/k1lib/k1ui/mouseKey.pth
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4919 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/knn.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31314 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/p5.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14079 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/schedule.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    29996 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/selector.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:00:19.355949 k1lib-1.4.3.2/k1lib/serve/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       20 2022-09-16 01:12:41.000000 k1lib-1.4.3.2/k1lib/serve/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20544 2023-03-19 11:14:40.000000 k1lib-1.4.3.2/k1lib/serve/main.html
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15412 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/serve/main.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      153 2023-05-05 16:00:40.000000 k1lib-1.4.3.2/k1lib/serve/suffix-dash.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      642 2023-02-13 19:00:39.000000 k1lib-1.4.3.2/k1lib/serve/suffix.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    28374 2023-08-02 03:41:46.000000 k1lib-1.4.3.2/k1lib/viz.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:00:19.343949 k1lib-1.4.3.2/k1lib.egg-info/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3429 2023-08-03 08:00:19.000000 k1lib-1.4.3.2/k1lib.egg-info/PKG-INFO
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2015 2023-08-03 08:00:19.000000 k1lib-1.4.3.2/k1lib.egg-info/SOURCES.txt
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        1 2023-08-03 08:00:19.000000 k1lib-1.4.3.2/k1lib.egg-info/dependency_links.txt
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      145 2023-08-03 08:00:19.000000 k1lib-1.4.3.2/k1lib.egg-info/requires.txt
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        6 2023-08-03 08:00:19.000000 k1lib-1.4.3.2/k1lib.egg-info/top_level.txt
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       38 2023-08-03 08:00:19.355949 k1lib-1.4.3.2/setup.cfg
--rwxrwxr-x   0 kelvin    (1000) kelvin    (1000)     1164 2023-08-03 08:00:08.000000 k1lib-1.4.3.2/setup.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.455231 k1lib-1.4.3.3/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     1049 2023-08-02 00:51:20.000000 k1lib-1.4.3.3/LICENSE
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3429 2023-08-03 08:05:00.455231 k1lib-1.4.3.3/PKG-INFO
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.451231 k1lib-1.4.3.3/k1lib/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     1441 2023-05-26 17:16:37.000000 k1lib-1.4.3.3/k1lib/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    83638 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_baseClasses.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    25641 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_basics.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8208 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_context.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.451231 k1lib-1.4.3.3/k1lib/_hidden/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        0 2021-08-11 18:19:53.000000 k1lib-1.4.3.3/k1lib/_hidden/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       79 2021-08-11 18:19:53.000000 k1lib-1.4.3.3/k1lib/_hidden/hiddenFile.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4314 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_higher.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3085 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_k1a.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20567 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_learner.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.451231 k1lib-1.4.3.3/k1lib/_mo/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      615 2021-10-24 23:32:21.000000 k1lib-1.4.3.3/k1lib/_mo/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    24015 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_mo/atom.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    18173 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_mo/parseM.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5631 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_mo/substance.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15454 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_mo/system.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    36997 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_monkey.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5575 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_perlin.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.451231 k1lib-1.4.3.3/k1lib/callbacks/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      378 2021-10-30 05:51:17.000000 k1lib-1.4.3.3/k1lib/callbacks/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31963 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/callbacks.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5455 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/confusionMatrix.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2245 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/core.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    19517 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/hookModule.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7488 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/hookParam.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5728 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/landscape.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14525 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/limits.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.451231 k1lib-1.4.3.3/k1lib/callbacks/lossFunctions/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       30 2021-10-27 12:39:02.000000 k1lib-1.4.3.3/k1lib/callbacks/lossFunctions/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3695 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/lossFunctions/accuracy.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5968 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/lossFunctions/shorts.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    10038 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/loss_accuracy.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6002 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/paramFinder.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5311 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/profiler.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.451231 k1lib-1.4.3.3/k1lib/callbacks/profilers/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       45 2021-08-11 18:19:53.000000 k1lib-1.4.3.3/k1lib/callbacks/profilers/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     9311 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/profilers/computation.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4069 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/profilers/io.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7368 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/profilers/memory.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6971 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/profilers/time.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4242 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/progress.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4370 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/recorder.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8363 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/shorts.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.455231 k1lib-1.4.3.3/k1lib/cli/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      975 2023-07-13 16:14:07.000000 k1lib-1.4.3.3/k1lib/cli/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31282 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/_applyCl.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    13909 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/bio.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5162 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/cif.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    39336 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/conv.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    50607 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/filt.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8480 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/gb.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    12136 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/grep.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    35488 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/init.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    69938 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/inp.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14704 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/ktree.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7467 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/kxml.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15993 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/lsext.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2977 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/mgi.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    18005 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/models.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)   125352 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/modifier.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      735 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/mol.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5822 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/nb.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6311 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/optimizations.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20026 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/output.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3042 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/sam.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    72596 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/structural.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15949 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/trace.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    41733 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/typehint.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    49466 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/utils.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    21263 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/eqn.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    12310 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/fmt.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    10890 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/graphEqn.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5180 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/imports.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.455231 k1lib-1.4.3.3/k1lib/k1ui/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)  2453826 2023-01-19 22:50:00.000000 k1lib-1.4.3.3/k1lib/k1ui/256.model.state_dict.pth
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       20 2023-01-19 22:00:40.000000 k1lib-1.4.3.3/k1lib/k1ui/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    88758 2023-08-03 08:04:39.000000 k1lib-1.4.3.3/k1lib/k1ui/main.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)   304735 2023-01-17 19:16:23.000000 k1lib-1.4.3.3/k1lib/k1ui/mouseKey.pth
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4919 2023-08-03 08:04:39.000000 k1lib-1.4.3.3/k1lib/knn.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31314 2023-08-03 08:04:39.000000 k1lib-1.4.3.3/k1lib/p5.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14079 2023-08-03 08:04:39.000000 k1lib-1.4.3.3/k1lib/schedule.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    29996 2023-08-03 08:04:39.000000 k1lib-1.4.3.3/k1lib/selector.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.455231 k1lib-1.4.3.3/k1lib/serve/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       20 2022-09-16 01:12:41.000000 k1lib-1.4.3.3/k1lib/serve/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20544 2023-03-19 11:14:40.000000 k1lib-1.4.3.3/k1lib/serve/main.html
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15412 2023-08-03 08:04:39.000000 k1lib-1.4.3.3/k1lib/serve/main.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      153 2023-05-05 16:00:40.000000 k1lib-1.4.3.3/k1lib/serve/suffix-dash.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      642 2023-02-13 19:00:39.000000 k1lib-1.4.3.3/k1lib/serve/suffix.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    28374 2023-08-03 08:04:39.000000 k1lib-1.4.3.3/k1lib/viz.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.451231 k1lib-1.4.3.3/k1lib.egg-info/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3429 2023-08-03 08:05:00.000000 k1lib-1.4.3.3/k1lib.egg-info/PKG-INFO
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2015 2023-08-03 08:05:00.000000 k1lib-1.4.3.3/k1lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        1 2023-08-03 08:05:00.000000 k1lib-1.4.3.3/k1lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      145 2023-08-03 08:05:00.000000 k1lib-1.4.3.3/k1lib.egg-info/requires.txt
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        6 2023-08-03 08:05:00.000000 k1lib-1.4.3.3/k1lib.egg-info/top_level.txt
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       38 2023-08-03 08:05:00.455231 k1lib-1.4.3.3/setup.cfg
+-rwxrwxr-x   0 kelvin    (1000) kelvin    (1000)     1164 2023-08-03 08:04:50.000000 k1lib-1.4.3.3/setup.py
```

### Comparing `k1lib-1.4.3.2/LICENSE` & `k1lib-1.4.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/PKG-INFO` & `k1lib-1.4.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k1lib
-Version: 1.4.3.2
+Version: 1.4.3.3
 Summary: Some nice ML overhaul
 Home-page: https://k1lib.com
 Author: Quang Ho
 Author-email: 157239q@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `k1lib-1.4.3.2/k1lib/__init__.py` & `k1lib-1.4.3.3/k1lib/__init__.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/_baseClasses.py` & `k1lib-1.4.3.3/k1lib/_baseClasses.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/_basics.py` & `k1lib-1.4.3.3/k1lib/_basics.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/_context.py` & `k1lib-1.4.3.3/k1lib/_context.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/_higher.py` & `k1lib-1.4.3.3/k1lib/_higher.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/_k1a.py` & `k1lib-1.4.3.3/k1lib/_k1a.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/_learner.py` & `k1lib-1.4.3.3/k1lib/_learner.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/_mo/__init__.py` & `k1lib-1.4.3.3/k1lib/_mo/__init__.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/_mo/atom.py` & `k1lib-1.4.3.3/k1lib/_mo/atom.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/_mo/parseM.py` & `k1lib-1.4.3.3/k1lib/_mo/parseM.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/_mo/substance.py` & `k1lib-1.4.3.3/k1lib/_mo/substance.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/_mo/system.py` & `k1lib-1.4.3.3/k1lib/_mo/system.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/_monkey.py` & `k1lib-1.4.3.3/k1lib/_monkey.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/_perlin.py` & `k1lib-1.4.3.3/k1lib/_perlin.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/callbacks.py` & `k1lib-1.4.3.3/k1lib/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/confusionMatrix.py` & `k1lib-1.4.3.3/k1lib/callbacks/confusionMatrix.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/core.py` & `k1lib-1.4.3.3/k1lib/callbacks/core.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/hookModule.py` & `k1lib-1.4.3.3/k1lib/callbacks/hookModule.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/hookParam.py` & `k1lib-1.4.3.3/k1lib/callbacks/hookParam.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/landscape.py` & `k1lib-1.4.3.3/k1lib/callbacks/landscape.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/limits.py` & `k1lib-1.4.3.3/k1lib/callbacks/limits.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/lossFunctions/accuracy.py` & `k1lib-1.4.3.3/k1lib/callbacks/lossFunctions/accuracy.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/lossFunctions/shorts.py` & `k1lib-1.4.3.3/k1lib/callbacks/lossFunctions/shorts.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/loss_accuracy.py` & `k1lib-1.4.3.3/k1lib/callbacks/loss_accuracy.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/paramFinder.py` & `k1lib-1.4.3.3/k1lib/callbacks/paramFinder.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/profiler.py` & `k1lib-1.4.3.3/k1lib/callbacks/profiler.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/profilers/computation.py` & `k1lib-1.4.3.3/k1lib/callbacks/profilers/computation.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/profilers/io.py` & `k1lib-1.4.3.3/k1lib/callbacks/profilers/io.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/profilers/memory.py` & `k1lib-1.4.3.3/k1lib/callbacks/profilers/memory.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/profilers/time.py` & `k1lib-1.4.3.3/k1lib/callbacks/profilers/time.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/progress.py` & `k1lib-1.4.3.3/k1lib/callbacks/progress.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/recorder.py` & `k1lib-1.4.3.3/k1lib/callbacks/recorder.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/callbacks/shorts.py` & `k1lib-1.4.3.3/k1lib/callbacks/shorts.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/__init__.py` & `k1lib-1.4.3.3/k1lib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/_applyCl.py` & `k1lib-1.4.3.3/k1lib/cli/_applyCl.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/bio.py` & `k1lib-1.4.3.3/k1lib/cli/bio.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/cif.py` & `k1lib-1.4.3.3/k1lib/cli/cif.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/conv.py` & `k1lib-1.4.3.3/k1lib/cli/conv.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/filt.py` & `k1lib-1.4.3.3/k1lib/cli/filt.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/gb.py` & `k1lib-1.4.3.3/k1lib/cli/gb.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/grep.py` & `k1lib-1.4.3.3/k1lib/cli/grep.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/init.py` & `k1lib-1.4.3.3/k1lib/cli/init.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/inp.py` & `k1lib-1.4.3.3/k1lib/cli/inp.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/ktree.py` & `k1lib-1.4.3.3/k1lib/cli/ktree.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/kxml.py` & `k1lib-1.4.3.3/k1lib/cli/kxml.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/lsext.py` & `k1lib-1.4.3.3/k1lib/cli/lsext.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/mgi.py` & `k1lib-1.4.3.3/k1lib/cli/mgi.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/models.py` & `k1lib-1.4.3.3/k1lib/cli/models.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/modifier.py` & `k1lib-1.4.3.3/k1lib/cli/modifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 import k1lib.cli as cli, numpy as np, threading, gc; import k1lib
 from collections import deque, defaultdict
 from functools import partial, update_wrapper, lru_cache
 from k1lib.cli.typehint import *
 import dill, pickle, k1lib, warnings, atexit, signal, time, os, random, sys
 try: import torch; import torch.multiprocessing as mp; hasTorch = True
 except: import multiprocessing as mp; hasTorch = False
-ray = k1lib.dep("ray")
+try: import ray; hasRay = True
+except: hasRay = False
 settings = k1lib.settings.cli
 class applyS(BaseCli):                                                           # applyS
     def __init__(self, f:Callable[[Any], Any], *args, **kwargs):                 # applyS
         """Like :class:`apply`, but much simpler, just operating on the entire input
 object, essentially. The "S" stands for "single". There's
 also an alias shorthand for this called :class:`aS`. Example::
 
@@ -1237,39 +1238,42 @@
         if folder is None: return getFolderSize                                  # applyCl
         return folder | getFolderSize                                            # applyCl
     @staticmethod                                                                # applyCl
     def getFilesInFolder(folder:str=None):                                       # applyCl
         from k1lib.cli._applyCl import getFilesInFolder                          # applyCl
         if folder is None: return getFilesInFolder                               # applyCl
         return folder | getFilesInFolder                                         # applyCl
-@ray.remote(num_cpus=0)                                                          # applyCl
-class Storage: # a wrapper for specific objects, kinda like ObjectRef, but it's an ObjectRef in my control. Should not be serialized to every other place # Storage
-    def __init__(self, v=None):                                                  # Storage
-        self.nodeId = applyCl.nodeId(); self.d = {}; self.refs = defaultdict(lambda: 0) # Storage
-        self.autoInc = k1lib.AutoIncrement(prefix="_d"); self.deposit(v)         # Storage
-        self.idx = f"{self.nodeId}_" + f"{random.random()}"[:10] + f"_{time.time()}" # Storage
-    def getIdx(self): return self.idx                                            # Storage
-    def getMeta(self): return [self.nodeId, self.idx]                            # Storage
-    def lookup(self, idx:str): return self.d[idx]                                # Storage
-    def remove(self, idx:str): del self.d[idx]                                   # Storage
-    def keys(self): return list(self.d.keys())                                   # Storage
-    def incref(self, idx:str): self.refs[idx] += 1#; return self                 # Storage
-    def decref(self, idx:str):                                                   # Storage
-        self.refs[idx] -= 1                                                      # Storage
-        if self.refs[idx] == 0: self.remove(idx)                                 # Storage
-        # return self                                                            # Storage
-    def deposit(self, v:"1/or1/h1", s:"Storage"=None) -> "idx:str": # injecting s into v if v is a Handle # Storage
-        if isinstance(v, Handle): v.setStorage(s); v = v.get()                   # Storage
-        if isinstance(v, ray.ObjectRef): v = ray.get(v)                          # Storage
-        idx = self.autoInc(); self.d[idx] = v; self.incref(idx); return idx      # Storage
-    def execute(self, f, s:"Storage", idx:str) -> "idx:str": return self.deposit(f(s, self.d[idx])) # executing "pure" f with some argument taken from the storage # Storage
-    def __getstate__(self): raise Exception("Can't be serialized!")              # Storage
-_storages = {} # nodeId -> {idx: int, ss: [Storage]}, idx for current index to yield the storage # Storage
-_cpuCounts = {} # nodeId -> int                                                  # Storage
-_nodeIdsGen = None                                                               # Storage
+if hasRay:                                                                       # applyCl
+    @ray.remote(num_cpus=0)                                                      # applyCl
+    class Storage: # a wrapper for specific objects, kinda like ObjectRef, but it's an ObjectRef in my control. Should not be serialized to every other place # applyCl
+        def __init__(self, v=None):                                              # applyCl
+            self.nodeId = applyCl.nodeId(); self.d = {}; self.refs = defaultdict(lambda: 0) # applyCl
+            self.autoInc = k1lib.AutoIncrement(prefix="_d"); self.deposit(v)     # applyCl
+            self.idx = f"{self.nodeId}_" + f"{random.random()}"[:10] + f"_{time.time()}" # applyCl
+        def getIdx(self): return self.idx                                        # applyCl
+        def getMeta(self): return [self.nodeId, self.idx]                        # applyCl
+        def lookup(self, idx:str): return self.d[idx]                            # applyCl
+        def remove(self, idx:str): del self.d[idx]                               # applyCl
+        def keys(self): return list(self.d.keys())                               # applyCl
+        def incref(self, idx:str): self.refs[idx] += 1#; return self             # applyCl
+        def decref(self, idx:str):                                               # applyCl
+            self.refs[idx] -= 1                                                  # applyCl
+            if self.refs[idx] == 0: self.remove(idx)                             # applyCl
+            # return self                                                        # applyCl
+        def deposit(self, v:"1/or1/h1", s:"Storage"=None) -> "idx:str": # injecting s into v if v is a Handle # applyCl
+            if isinstance(v, Handle): v.setStorage(s); v = v.get()               # applyCl
+            if isinstance(v, ray.ObjectRef): v = ray.get(v)                      # applyCl
+            idx = self.autoInc(); self.d[idx] = v; self.incref(idx); return idx  # applyCl
+        def execute(self, f, s:"Storage", idx:str) -> "idx:str": return self.deposit(f(s, self.d[idx])) # executing "pure" f with some argument taken from the storage # applyCl
+        def __getstate__(self): raise Exception("Can't be serialized!")          # applyCl
+else:                                                                            # applyCl
+    class Storage: pass                                                          # applyCl
+_storages = {} # nodeId -> {idx: int, ss: [Storage]}, idx for current index to yield the storage # applyCl
+_cpuCounts = {} # nodeId -> int                                                  # applyCl
+_nodeIdsGen = None                                                               # applyCl
 def getStorage(nodeId:str=None):                                                 # getStorage
     """Handles creating storage contexts. This is created mainly because it's
 costly to actually instantiate a new actor (1-2 second/actor!), so this will
 spawn new storage contexts till the cpu count of each node is reached. From
 then on, it will keep reusing old storage contexts"""                            # getStorage
     global _nodeIdsGen; _nodeIdsGen = _nodeIdsGen or applyCl.balancedNodeIds()   # getStorage
     nodeId = nodeId or next(_nodeIdsGen)                                         # getStorage
```

### Comparing `k1lib-1.4.3.2/k1lib/cli/mol.py` & `k1lib-1.4.3.3/k1lib/cli/mol.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/nb.py` & `k1lib-1.4.3.3/k1lib/cli/nb.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/optimizations.py` & `k1lib-1.4.3.3/k1lib/cli/optimizations.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/output.py` & `k1lib-1.4.3.3/k1lib/cli/output.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/sam.py` & `k1lib-1.4.3.3/k1lib/cli/sam.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/structural.py` & `k1lib-1.4.3.3/k1lib/cli/structural.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/trace.py` & `k1lib-1.4.3.3/k1lib/cli/trace.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/typehint.py` & `k1lib-1.4.3.3/k1lib/cli/typehint.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/cli/utils.py` & `k1lib-1.4.3.3/k1lib/cli/utils.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/eqn.py` & `k1lib-1.4.3.3/k1lib/eqn.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/fmt.py` & `k1lib-1.4.3.3/k1lib/fmt.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/graphEqn.py` & `k1lib-1.4.3.3/k1lib/graphEqn.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/imports.py` & `k1lib-1.4.3.3/k1lib/imports.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/k1ui/256.model.state_dict.pth` & `k1lib-1.4.3.3/k1lib/k1ui/256.model.state_dict.pth`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/k1ui/main.py` & `k1lib-1.4.3.3/k1lib/k1ui/main.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/k1ui/mouseKey.pth` & `k1lib-1.4.3.3/k1lib/k1ui/mouseKey.pth`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/knn.py` & `k1lib-1.4.3.3/k1lib/knn.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/p5.py` & `k1lib-1.4.3.3/k1lib/p5.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/schedule.py` & `k1lib-1.4.3.3/k1lib/schedule.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/selector.py` & `k1lib-1.4.3.3/k1lib/selector.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/serve/main.html` & `k1lib-1.4.3.3/k1lib/serve/main.html`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/serve/main.py` & `k1lib-1.4.3.3/k1lib/serve/main.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/serve/suffix.py` & `k1lib-1.4.3.3/k1lib/serve/suffix.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib/viz.py` & `k1lib-1.4.3.3/k1lib/viz.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/k1lib.egg-info/PKG-INFO` & `k1lib-1.4.3.3/k1lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k1lib
-Version: 1.4.3.2
+Version: 1.4.3.3
 Summary: Some nice ML overhaul
 Home-page: https://k1lib.com
 Author: Quang Ho
 Author-email: 157239q@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `k1lib-1.4.3.2/k1lib.egg-info/SOURCES.txt` & `k1lib-1.4.3.3/k1lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.2/setup.py` & `k1lib-1.4.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     packages=["k1lib", "k1lib._hidden",
               "k1lib.cli",
               "k1lib.callbacks", "k1lib.callbacks.profilers",
               "k1lib.callbacks.lossFunctions",
               "k1lib._mo", "k1lib.serve", "k1lib.k1ui"],
     data_files=[('k1lib/serve', ['k1lib/serve/main.html']),
                 ('k1lib/k1ui', ['k1lib/k1ui/mouseKey.pth', 'k1lib/k1ui/256.model.state_dict.pth'])],
-    version="1.4.3.2",
+    version="1.4.3.3",
     python_requires='>=3.7',
     install_requires=["numpy>=1.14", "matplotlib>=2.0", "dill", "forbiddenfruit", "wurlitzer", "validators"],
     extras_require={"all": deps},
     description="Some nice ML overhaul",
     url="https://k1lib.com",
     author="Quang Ho",
     author_email="157239q@gmail.com",
```

