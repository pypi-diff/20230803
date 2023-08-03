# Comparing `tmp/k1lib-1.4.3.3.tar.gz` & `tmp/k1lib-1.4.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k1lib-1.4.3.3.tar", last modified: Thu Aug  3 08:05:00 2023, max compression
+gzip compressed data, was "k1lib-1.4.3.4.tar", last modified: Thu Aug  3 08:12:06 2023, max compression
```

## Comparing `k1lib-1.4.3.3.tar` & `k1lib-1.4.3.4.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.455231 k1lib-1.4.3.3/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     1049 2023-08-02 00:51:20.000000 k1lib-1.4.3.3/LICENSE
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3429 2023-08-03 08:05:00.455231 k1lib-1.4.3.3/PKG-INFO
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.451231 k1lib-1.4.3.3/k1lib/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     1441 2023-05-26 17:16:37.000000 k1lib-1.4.3.3/k1lib/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    83638 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_baseClasses.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    25641 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_basics.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8208 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_context.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.451231 k1lib-1.4.3.3/k1lib/_hidden/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        0 2021-08-11 18:19:53.000000 k1lib-1.4.3.3/k1lib/_hidden/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       79 2021-08-11 18:19:53.000000 k1lib-1.4.3.3/k1lib/_hidden/hiddenFile.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4314 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_higher.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3085 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_k1a.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20567 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_learner.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.451231 k1lib-1.4.3.3/k1lib/_mo/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      615 2021-10-24 23:32:21.000000 k1lib-1.4.3.3/k1lib/_mo/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    24015 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_mo/atom.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    18173 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_mo/parseM.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5631 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_mo/substance.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15454 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_mo/system.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    36997 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_monkey.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5575 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/_perlin.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.451231 k1lib-1.4.3.3/k1lib/callbacks/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      378 2021-10-30 05:51:17.000000 k1lib-1.4.3.3/k1lib/callbacks/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31963 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/callbacks.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5455 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/confusionMatrix.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2245 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/core.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    19517 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/hookModule.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7488 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/hookParam.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5728 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/landscape.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14525 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/limits.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.451231 k1lib-1.4.3.3/k1lib/callbacks/lossFunctions/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       30 2021-10-27 12:39:02.000000 k1lib-1.4.3.3/k1lib/callbacks/lossFunctions/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3695 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/lossFunctions/accuracy.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5968 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/lossFunctions/shorts.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    10038 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/loss_accuracy.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6002 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/paramFinder.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5311 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/profiler.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.451231 k1lib-1.4.3.3/k1lib/callbacks/profilers/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       45 2021-08-11 18:19:53.000000 k1lib-1.4.3.3/k1lib/callbacks/profilers/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     9311 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/profilers/computation.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4069 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/profilers/io.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7368 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/profilers/memory.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6971 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/profilers/time.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4242 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/progress.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4370 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/recorder.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8363 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/callbacks/shorts.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.455231 k1lib-1.4.3.3/k1lib/cli/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      975 2023-07-13 16:14:07.000000 k1lib-1.4.3.3/k1lib/cli/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31282 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/_applyCl.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    13909 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/bio.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5162 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/cif.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    39336 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/conv.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    50607 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/filt.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8480 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/gb.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    12136 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/grep.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    35488 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/init.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    69938 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/inp.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14704 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/ktree.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7467 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/kxml.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15993 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/lsext.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2977 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/mgi.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    18005 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/models.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)   125352 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/modifier.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      735 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/mol.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5822 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/nb.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6311 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/optimizations.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20026 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/output.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3042 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/sam.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    72596 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/structural.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15949 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/trace.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    41733 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/typehint.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    49466 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/cli/utils.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    21263 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/eqn.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    12310 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/fmt.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    10890 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/graphEqn.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5180 2023-08-03 08:04:38.000000 k1lib-1.4.3.3/k1lib/imports.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.455231 k1lib-1.4.3.3/k1lib/k1ui/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)  2453826 2023-01-19 22:50:00.000000 k1lib-1.4.3.3/k1lib/k1ui/256.model.state_dict.pth
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       20 2023-01-19 22:00:40.000000 k1lib-1.4.3.3/k1lib/k1ui/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    88758 2023-08-03 08:04:39.000000 k1lib-1.4.3.3/k1lib/k1ui/main.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)   304735 2023-01-17 19:16:23.000000 k1lib-1.4.3.3/k1lib/k1ui/mouseKey.pth
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4919 2023-08-03 08:04:39.000000 k1lib-1.4.3.3/k1lib/knn.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31314 2023-08-03 08:04:39.000000 k1lib-1.4.3.3/k1lib/p5.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14079 2023-08-03 08:04:39.000000 k1lib-1.4.3.3/k1lib/schedule.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    29996 2023-08-03 08:04:39.000000 k1lib-1.4.3.3/k1lib/selector.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.455231 k1lib-1.4.3.3/k1lib/serve/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       20 2022-09-16 01:12:41.000000 k1lib-1.4.3.3/k1lib/serve/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20544 2023-03-19 11:14:40.000000 k1lib-1.4.3.3/k1lib/serve/main.html
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15412 2023-08-03 08:04:39.000000 k1lib-1.4.3.3/k1lib/serve/main.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      153 2023-05-05 16:00:40.000000 k1lib-1.4.3.3/k1lib/serve/suffix-dash.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      642 2023-02-13 19:00:39.000000 k1lib-1.4.3.3/k1lib/serve/suffix.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    28374 2023-08-03 08:04:39.000000 k1lib-1.4.3.3/k1lib/viz.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:05:00.451231 k1lib-1.4.3.3/k1lib.egg-info/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3429 2023-08-03 08:05:00.000000 k1lib-1.4.3.3/k1lib.egg-info/PKG-INFO
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2015 2023-08-03 08:05:00.000000 k1lib-1.4.3.3/k1lib.egg-info/SOURCES.txt
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        1 2023-08-03 08:05:00.000000 k1lib-1.4.3.3/k1lib.egg-info/dependency_links.txt
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      145 2023-08-03 08:05:00.000000 k1lib-1.4.3.3/k1lib.egg-info/requires.txt
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        6 2023-08-03 08:05:00.000000 k1lib-1.4.3.3/k1lib.egg-info/top_level.txt
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       38 2023-08-03 08:05:00.455231 k1lib-1.4.3.3/setup.cfg
--rwxrwxr-x   0 kelvin    (1000) kelvin    (1000)     1164 2023-08-03 08:04:50.000000 k1lib-1.4.3.3/setup.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:12:06.938129 k1lib-1.4.3.4/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     1049 2023-08-02 00:51:20.000000 k1lib-1.4.3.4/LICENSE
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3429 2023-08-03 08:12:06.938129 k1lib-1.4.3.4/PKG-INFO
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:12:06.930129 k1lib-1.4.3.4/k1lib/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     1441 2023-05-26 17:16:37.000000 k1lib-1.4.3.4/k1lib/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    83638 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/_baseClasses.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    25641 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/_basics.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8208 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/_context.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:12:06.930129 k1lib-1.4.3.4/k1lib/_hidden/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        0 2021-08-11 18:19:53.000000 k1lib-1.4.3.4/k1lib/_hidden/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       79 2021-08-11 18:19:53.000000 k1lib-1.4.3.4/k1lib/_hidden/hiddenFile.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4314 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/_higher.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3085 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/_k1a.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20567 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/_learner.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:12:06.930129 k1lib-1.4.3.4/k1lib/_mo/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      615 2021-10-24 23:32:21.000000 k1lib-1.4.3.4/k1lib/_mo/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    24015 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/_mo/atom.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    18173 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/_mo/parseM.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5631 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/_mo/substance.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15454 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/_mo/system.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    36997 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/_monkey.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5575 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/_perlin.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:12:06.934129 k1lib-1.4.3.4/k1lib/callbacks/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      378 2021-10-30 05:51:17.000000 k1lib-1.4.3.4/k1lib/callbacks/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31963 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/callbacks.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5455 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/confusionMatrix.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2245 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/core.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    19517 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/hookModule.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7488 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/hookParam.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5728 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/landscape.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14525 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/limits.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:12:06.934129 k1lib-1.4.3.4/k1lib/callbacks/lossFunctions/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       30 2021-10-27 12:39:02.000000 k1lib-1.4.3.4/k1lib/callbacks/lossFunctions/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3695 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/lossFunctions/accuracy.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5968 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/lossFunctions/shorts.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    10038 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/loss_accuracy.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6002 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/paramFinder.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5311 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/profiler.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:12:06.934129 k1lib-1.4.3.4/k1lib/callbacks/profilers/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       45 2021-08-11 18:19:53.000000 k1lib-1.4.3.4/k1lib/callbacks/profilers/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     9311 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/profilers/computation.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4069 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/profilers/io.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7368 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/profilers/memory.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6971 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/profilers/time.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4242 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/progress.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4370 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/recorder.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8363 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/callbacks/shorts.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:12:06.934129 k1lib-1.4.3.4/k1lib/cli/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      975 2023-07-13 16:14:07.000000 k1lib-1.4.3.4/k1lib/cli/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31282 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/_applyCl.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    13909 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/bio.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5162 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/cif.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    24772 2023-08-03 08:11:19.000000 k1lib-1.4.3.4/k1lib/cli/conv.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    50607 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/filt.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8480 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/gb.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    12136 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/grep.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    35488 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/init.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    69938 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/inp.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14704 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/ktree.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7467 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/kxml.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15993 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/lsext.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2977 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/mgi.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    18005 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/models.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)   125352 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/modifier.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      735 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/mol.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5822 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/nb.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6311 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/optimizations.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20026 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/output.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3042 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/sam.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    72596 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/structural.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15949 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/trace.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    41733 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/typehint.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    49466 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/cli/utils.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    21263 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/eqn.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    12310 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/fmt.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    10890 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/graphEqn.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5180 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/imports.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:12:06.938129 k1lib-1.4.3.4/k1lib/k1ui/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)  2453826 2023-01-19 22:50:00.000000 k1lib-1.4.3.4/k1lib/k1ui/256.model.state_dict.pth
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       20 2023-01-19 22:00:40.000000 k1lib-1.4.3.4/k1lib/k1ui/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    88758 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/k1ui/main.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)   304735 2023-01-17 19:16:23.000000 k1lib-1.4.3.4/k1lib/k1ui/mouseKey.pth
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4919 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/knn.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31314 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/p5.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14079 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/schedule.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    29996 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/selector.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:12:06.938129 k1lib-1.4.3.4/k1lib/serve/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       20 2022-09-16 01:12:41.000000 k1lib-1.4.3.4/k1lib/serve/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20544 2023-03-19 11:14:40.000000 k1lib-1.4.3.4/k1lib/serve/main.html
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15412 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/serve/main.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      153 2023-05-05 16:00:40.000000 k1lib-1.4.3.4/k1lib/serve/suffix-dash.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      642 2023-02-13 19:00:39.000000 k1lib-1.4.3.4/k1lib/serve/suffix.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    28374 2023-08-03 08:10:17.000000 k1lib-1.4.3.4/k1lib/viz.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-03 08:12:06.930129 k1lib-1.4.3.4/k1lib.egg-info/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3429 2023-08-03 08:12:06.000000 k1lib-1.4.3.4/k1lib.egg-info/PKG-INFO
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2015 2023-08-03 08:12:06.000000 k1lib-1.4.3.4/k1lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        1 2023-08-03 08:12:06.000000 k1lib-1.4.3.4/k1lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      145 2023-08-03 08:12:06.000000 k1lib-1.4.3.4/k1lib.egg-info/requires.txt
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        6 2023-08-03 08:12:06.000000 k1lib-1.4.3.4/k1lib.egg-info/top_level.txt
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       38 2023-08-03 08:12:06.938129 k1lib-1.4.3.4/setup.cfg
+-rwxrwxr-x   0 kelvin    (1000) kelvin    (1000)     1164 2023-08-03 08:11:52.000000 k1lib-1.4.3.4/setup.py
```

### Comparing `k1lib-1.4.3.3/LICENSE` & `k1lib-1.4.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/PKG-INFO` & `k1lib-1.4.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k1lib
-Version: 1.4.3.3
+Version: 1.4.3.4
 Summary: Some nice ML overhaul
 Home-page: https://k1lib.com
 Author: Quang Ho
 Author-email: 157239q@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `k1lib-1.4.3.3/k1lib/__init__.py` & `k1lib-1.4.3.4/k1lib/__init__.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/_baseClasses.py` & `k1lib-1.4.3.4/k1lib/_baseClasses.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/_basics.py` & `k1lib-1.4.3.4/k1lib/_basics.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/_context.py` & `k1lib-1.4.3.4/k1lib/_context.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/_higher.py` & `k1lib-1.4.3.4/k1lib/_higher.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/_k1a.py` & `k1lib-1.4.3.4/k1lib/_k1a.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/_learner.py` & `k1lib-1.4.3.4/k1lib/_learner.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/_mo/__init__.py` & `k1lib-1.4.3.4/k1lib/_mo/__init__.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/_mo/atom.py` & `k1lib-1.4.3.4/k1lib/_mo/atom.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/_mo/parseM.py` & `k1lib-1.4.3.4/k1lib/_mo/parseM.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/_mo/substance.py` & `k1lib-1.4.3.4/k1lib/_mo/substance.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/_mo/system.py` & `k1lib-1.4.3.4/k1lib/_mo/system.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/_monkey.py` & `k1lib-1.4.3.4/k1lib/_monkey.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/_perlin.py` & `k1lib-1.4.3.4/k1lib/_perlin.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/callbacks.py` & `k1lib-1.4.3.4/k1lib/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/confusionMatrix.py` & `k1lib-1.4.3.4/k1lib/callbacks/confusionMatrix.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/core.py` & `k1lib-1.4.3.4/k1lib/callbacks/core.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/hookModule.py` & `k1lib-1.4.3.4/k1lib/callbacks/hookModule.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/hookParam.py` & `k1lib-1.4.3.4/k1lib/callbacks/hookParam.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/landscape.py` & `k1lib-1.4.3.4/k1lib/callbacks/landscape.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/limits.py` & `k1lib-1.4.3.4/k1lib/callbacks/limits.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/lossFunctions/accuracy.py` & `k1lib-1.4.3.4/k1lib/callbacks/lossFunctions/accuracy.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/lossFunctions/shorts.py` & `k1lib-1.4.3.4/k1lib/callbacks/lossFunctions/shorts.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/loss_accuracy.py` & `k1lib-1.4.3.4/k1lib/callbacks/loss_accuracy.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/paramFinder.py` & `k1lib-1.4.3.4/k1lib/callbacks/paramFinder.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/profiler.py` & `k1lib-1.4.3.4/k1lib/callbacks/profiler.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/profilers/computation.py` & `k1lib-1.4.3.4/k1lib/callbacks/profilers/computation.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/profilers/io.py` & `k1lib-1.4.3.4/k1lib/callbacks/profilers/io.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/profilers/memory.py` & `k1lib-1.4.3.4/k1lib/callbacks/profilers/memory.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/profilers/time.py` & `k1lib-1.4.3.4/k1lib/callbacks/profilers/time.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/progress.py` & `k1lib-1.4.3.4/k1lib/callbacks/progress.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/recorder.py` & `k1lib-1.4.3.4/k1lib/callbacks/recorder.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/callbacks/shorts.py` & `k1lib-1.4.3.4/k1lib/callbacks/shorts.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/__init__.py` & `k1lib-1.4.3.4/k1lib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/_applyCl.py` & `k1lib-1.4.3.4/k1lib/cli/_applyCl.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/bio.py` & `k1lib-1.4.3.4/k1lib/cli/bio.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/cif.py` & `k1lib-1.4.3.4/k1lib/cli/cif.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/conv.py` & `k1lib-1.4.3.4/k1lib/cli/init.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,577 +1,476 @@
 # AUTOGENERATED FILE! PLEASE DON'T EDIT HERE. EDIT THE SOURCE NOTEBOOKS INSTEAD
-"""
-This is for all short utilities that converts from 1 data type to another. They
-might feel they have different styles, as :class:`toFloat` converts object iterator to
-float iterator, while :class:`toPIL` converts single image url to single PIL image,
-whereas :class:`toSum` converts float iterator into a single float value.
-
-The general convention is, if the intended operation sounds simple (convert to floats,
-strings, types, ...), then most likely it will convert iterator to iterator, as you
-can always use the function directly if you only want to apply it on 1 object.
-
-If it sounds complicated (convert to PIL image, tensor, ...) then most likely it will
-convert object to object. Lastly, there are some that just feels right to input
-an iterator and output a single object (like getting max, min, std, mean values)."""
-__all__ = ["toTensor", "toRange", "toList",
-           "toSum", "toProd", "toAvg", "toMean", "toStd", "toMax", "toMin", "toPIL", "toImg",
-           "toRgb", "toRgba", "toGray", "toDict",
-           "toFloat", "toInt", "toBytes", "toHtml", "toAscii", "toHash", "toCsv"]
-import re, k1lib, math, os, numpy as np, io, base64, unicodedata
-from k1lib.cli.init import BaseCli, T, yieldT; import k1lib.cli as cli
-from k1lib.cli.typehint import *; import matplotlib as mpl; import matplotlib.pyplot as plt
-from collections import deque, defaultdict; from typing import Iterator, Any, List, Set, Tuple, Dict, Callable, Union
-settings = k1lib.settings.cli
-try: import PIL; hasPIL = True
-except: hasPIL = False
+from typing import List, Iterator, Any, NewType, TypeVar, Generic
+import k1lib.cli as cli; from numbers import Number
+import k1lib, itertools, copy, xml, warnings, traceback, sys; import numpy as np
+import xml.etree.ElementTree
 try: import torch; hasTorch = True
-except: torch = k1lib.dep("torch"); hasTorch = False
-try: import rdkit; hasRdkit = True
-except: hasRdkit = False
-try: import graphviz; hasGraphviz = True
-except: hasGraphviz = False
-try: import plotly; import plotly.express as px; hasPlotly = True
-except: hasPlotly = False
-class toTensor(BaseCli):                                                         # toTensor
-    def __init__(self, dtype=torch.float32):                                     # toTensor
-        """Converts generator to :class:`torch.Tensor`. Essentially
-``torch.tensor(list(it))``.
-
-Also checks if input is a PIL Image. If yes, turn it into a :class:`torch.Tensor`
-and return."""                                                                   # toTensor
-        self.dtype = dtype                                                       # toTensor
-    def __ror__(self, it:Iterator[float]) -> torch.Tensor:                       # toTensor
-        try:                                                                     # toTensor
-            import PIL; pic=it                                                   # toTensor
-            if isinstance(pic, PIL.Image.Image): # stolen from torchvision ToTensor transform # toTensor
-                mode_to_nptype = {'I': np.int32, 'I;16': np.int16, 'F': np.float32} # toTensor
-                img = torch.from_numpy(np.array(pic, mode_to_nptype.get(pic.mode, np.uint8), copy=True)) # toTensor
-                if pic.mode == '1': img = 255 * img                              # toTensor
-                img = img.view(pic.size[1], pic.size[0], len(pic.getbands()))    # toTensor
-                return img.permute((2, 0, 1)).contiguous().to(self.dtype) # put it from HWC to CHW format # toTensor
-        except: pass                                                             # toTensor
-        if isinstance(it, np.ndarray): return torch.tensor(it).to(self.dtype)    # toTensor
-        return torch.tensor(list(it)).to(self.dtype)                             # toTensor
-class toList(BaseCli): # this still exists cause some LLVM optimizations are done on this, and too tired to change that at the moment # toList
-    def __init__(self):                                                          # toList
-        """Converts generator to list.
-Example::
-
-    # returns [0, 1, 2, 3, 4]
-    range(5) | toList()
-    # returns [0, 1, 2, 3, 4]
-    range(5) | aS(list)
-
-So this cli is sort of outdated. It still works fine, nothing wrong
-with it, but just do ``aS(list)`` instead. It's not removed to
-avoid breaking old projects."""                                                  # toList
-        super().__init__()                                                       # toList
-                                                                                 # toList
-    def _typehint(self, inp):                                                    # toList
-        if isinstance(inp, tListIterSet): return tList(inp.child)                # toList
-        if isinstance(inp, tCollection): return inp                              # toList
-        return tList(tAny())                                                     # toList
-    def __ror__(self, it:Iterator[Any]) -> List[Any]: return list(it)            # toList
-def _toRange(it):                                                                # _toRange
-    for i, _ in enumerate(it): yield i                                           # _toRange
-class toRange(BaseCli):                                                          # toRange
-    def __init__(self):                                                          # toRange
-        """Returns iter(range(len(it))), effectively.
-Example::
-
-    # returns [0, 1, 2]
-    [3, 2, 5] | toRange() | deref()"""                                           # toRange
-        super().__init__()                                                       # toRange
-    def __ror__(self, it:Iterator[Any]) -> Iterator[int]:                        # toRange
-        try: return range(len(it))                                               # toRange
-        except: return _toRange(it)                                              # toRange
-tOpt.addPass(lambda cs, ts, _: [cs[0]], [toRange, toRange])                      # toRange
-settings.add("arrayTypes", (torch.Tensor, np.ndarray), "default array types used to accelerate clis") # toRange
-def genericTypeHint(inp):                                                        # genericTypeHint
-    if isinstance(inp, tListIterSet): return inp.child                           # genericTypeHint
-    if isinstance(inp, tCollection): return inp.children[0]                      # genericTypeHint
-    if isinstance(inp, tArrayTypes): return inp.child                            # genericTypeHint
-    return tAny()                                                                # genericTypeHint
-class toSum(BaseCli):                                                            # toSum
-    def __init__(self):                                                          # toSum
-        """Calculates the sum of list of numbers. Can pipe in :class:`torch.Tensor` or :class:`numpy.ndarray`.
-Example::
-
-    # returns 45
-    range(10) | toSum()"""                                                       # toSum
-        super().__init__()                                                       # toSum
-    def _all_array_opt(self, it, level):                                         # toSum
-        bm = np if isinstance(it, np.ndarray) else (torch if hasTorch and isinstance(it, torch.Tensor) else None) # toSum
-        return NotImplemented if bm is None else bm.sum(it, tuple(range(level, len(it.shape)))) # toSum
-    def _typehint(self, inp): return genericTypeHint(inp)                        # toSum
-    def __ror__(self, it:Iterator[float]):                                       # toSum
-        if isinstance(it, settings.arrayTypes): return it.sum()                  # toSum
-        return sum(it)                                                           # toSum
-class toProd(BaseCli):                                                           # toProd
-    def __init__(self):                                                          # toProd
-        """Calculates the product of a list of numbers. Can pipe in :class:`torch.Tensor` or :class:`numpy.ndarray`.
-Example::
-
-    # returns 362880
-    range(1,10) | toProd()"""                                                    # toProd
-        super().__init__()                                                       # toProd
-    def _all_array_opt(self, it, level):                                         # toProd
-        if isinstance(it, np.ndarray): return np.prod(it, tuple(range(level, len(it.shape)))) # toProd
-        elif hasTorch and isinstance(it, torch.Tensor):                          # toProd
-            for i in range(level, len(it.shape)): it = torch.prod(it, level)     # toProd
-            return it                                                            # toProd
-        return NotImplemented                                                    # toProd
-    def _typehint(self, inp): return genericTypeHint(inp)                        # toProd
-    def __ror__(self, it):                                                       # toProd
-        if isinstance(it, settings.arrayTypes): return it.prod()                 # toProd
-        else: return math.prod(it)                                               # toProd
-class toAvg(BaseCli):                                                            # toAvg
-    def __init__(self):                                                          # toAvg
-        """Calculates average of list of numbers. Can pipe in :class:`torch.Tensor` or :class:`numpy.ndarray`.
-Example::
-
-    # returns 4.5
-    range(10) | toAvg()
-    # returns nan
-    [] | toAvg()"""                                                              # toAvg
-        super().__init__()                                                       # toAvg
-    def _all_array_opt(self, it, level):                                         # toAvg
-        bm = np if isinstance(it, np.ndarray) else (torch if hasTorch and isinstance(it, torch.Tensor) else None) # toAvg
-        return NotImplemented if bm is None else bm.mean(it, tuple(range(level, len(it.shape)))) # toAvg
-    def _typehint(self, inp):                                                    # toAvg
-        i = None                                                                 # toAvg
-        if isinstance(inp, tListIterSet): i = inp.child                          # toAvg
-        if isinstance(inp, tCollection): i = inp.children[0]                     # toAvg
-        if isinstance(inp, tArrayTypes): i = inp.child                           # toAvg
-        if i is not None: return float if i == int else i                        # toAvg
-        return tAny()                                                            # toAvg
-    def __ror__(self, it:Iterator[float]):                                       # toAvg
-        if isinstance(it, settings.arrayTypes): return it.mean()                 # toAvg
-        s = 0; i = -1                                                            # toAvg
-        for i, v in enumerate(it): s += v                                        # toAvg
-        i += 1                                                                   # toAvg
-        if not k1lib.settings.cli.strict and i == 0: return float("nan")         # toAvg
-        return s / i                                                             # toAvg
-if hasTorch:                                                                     # toAvg
-    torchVer = int(torch.__version__.split(".")[0])                              # toAvg
-    if torchVer >= 2:                                                            # toAvg
-        def torchStd(it, ddof, dim=None): return torch.std(it, dim, correction=ddof) # toAvg
-    else:                                                                        # toAvg
-        def torchStd(it, ddof, dim=None):                                        # toAvg
-            if ddof == 0: return torch.std(it, dim, unbiased=False)              # toAvg
-            if ddof == 1: return torch.std(it, dim, unbiased=True)               # toAvg
-            raise Exception(f"Please install PyTorch 2, as version 1 don't support correction factor of {ddof}") # toAvg
-else:                                                                            # toAvg
-    def torchStd(it, ddof): raise Exception("PyTorch not installed")             # toAvg
-class toStd(BaseCli):                                                            # toStd
-    def __init__(self, ddof:int=0):                                              # toStd
-        """Calculates standard deviation of list of numbers. Can pipe in :class:`torch.Tensor`
-or :class:`numpy.ndarray` to be faster. Example::
-
-    # returns 2.8722813232690143
-    range(10) | toStd()
-    # returns nan
-    [] | toStd()
-
-:param ddof: "delta degree of freedom". The divisor used in calculations is ``N - ddof``""" # toStd
-        self.ddof = ddof                                                         # toStd
-    def _all_array_opt(self, it, level):                                         # toStd
-        n = len(it.shape); ddof = self.ddof; dim = tuple(range(level, n))        # toStd
-        if isinstance(it, np.ndarray): return np.std(it, ddof=ddof, axis=dim)    # toStd
-        elif hasTorch and isinstance(it, torch.Tensor): return torchStd(it, ddof, dim) # toStd
-        return NotImplemented                                                    # toStd
-    def __ror__(self, it):                                                       # toStd
-        ddof = self.ddof                                                         # toStd
-        if isinstance(it, settings.arrayTypes):                                  # toStd
-            if isinstance(it, np.ndarray): return np.std(it, ddof=ddof)          # toStd
-            elif hasTorch and isinstance(it, torch.Tensor): return torchStd(it, ddof) # toStd
-        return np.std(np.array(list(it)))                                        # toStd
-toMean = toAvg                                                                   # toStd
-class toMax(BaseCli):                                                            # toMax
-    def __init__(self):                                                          # toMax
-        """Calculates the max of a bunch of numbers. Can pipe in :class:`torch.Tensor` or :class:`numpy.ndarray`.
-Example::
-
-    # returns 6
-    [2, 5, 6, 1, 2] | toMax()"""                                                 # toMax
-        super().__init__()                                                       # toMax
-    def _all_array_opt(self, it, level):                                         # toMax
-        if isinstance(it, np.ndarray): return np.max(it, tuple(range(level, len(it.shape)))) # toMax
-        elif hasTorch and isinstance(it, torch.Tensor):                          # toMax
-            for i in range(level, len(it.shape)): it = torch.max(it, level)[0]   # toMax
-            return it                                                            # toMax
-        return NotImplemented                                                    # toMax
-    def __ror__(self, it:Iterator[float]) -> float:                              # toMax
-        if isinstance(it, settings.arrayTypes): return it.max()                  # toMax
-        return max(it)                                                           # toMax
-class toMin(BaseCli):                                                            # toMin
-    def __init__(self):                                                          # toMin
-        """Calculates the min of a bunch of numbers. Can pipe in :class:`torch.Tensor` or :class:`numpy.ndarray`.
-Example::
-
-    # returns 1
-    [2, 5, 6, 1, 2] | toMin()"""                                                 # toMin
-        super().__init__()                                                       # toMin
-    def _all_array_opt(self, it, level):                                         # toMin
-        if isinstance(it, np.ndarray): return np.min(it, tuple(range(level, len(it.shape)))) # toMin
-        elif hasTorch and isinstance(it, torch.Tensor):                          # toMin
-            for i in range(level, len(it.shape)): it = torch.min(it, level)[0]   # toMin
-            return it                                                            # toMin
-        return NotImplemented                                                    # toMin
-    def __ror__(self, it:Iterator[float]) -> float:                              # toMin
-        if isinstance(it, settings.arrayTypes): return it.min()                  # toMin
-        return min(it)                                                           # toMin
-settings.add("font", None, "default font file. Best to use .ttf files, used by toPIL()") # toMin
-settings.add("chem", k1lib.Settings().add("imgSize", 200, "default image size used in toPIL() when drawing rdkit molecules"), "chemistry-related settings") # toMin
-def cropToContentNp(ogIm, pad=10):                                               # cropToContentNp
-    dim = len(ogIm.shape); im = ogIm                                             # cropToContentNp
-    if dim > 2: im = im.mean(0)                                                  # cropToContentNp
-    coords = np.argwhere(im.max()-im); x_min, y_min = coords.min(axis=0); x_max, y_max = coords.max(axis=0) # cropToContentNp
-    return ogIm[x_min-pad:x_max+1+pad, y_min-pad:y_max+1+pad] if dim == 2 else ogIm[:,x_min-pad:x_max+1+pad, y_min-pad:y_max+1+pad] # cropToContentNp
-def cropToContentPIL(im, pad=0):                                                 # cropToContentPIL
-    im = im | toTensor(int) | cli.op().numpy() | cli.aS(cropToContentNp, pad)    # cropToContentPIL
-    return torch.from_numpy(im).permute(1, 2, 0) | toImg() if len(im.shape) > 2 else im | toImg() # cropToContentPIL
-class toPIL(BaseCli):                                                            # toPIL
-    def __init__(self, closeFig=True, crop=True):                                # toPIL
-        """Converts multiple data types into a PIL image.
-Example::
-
-    # grabs first image in the current folder
-    ls(".") | toPIL().all() | item()
-    # converts from tensor/array to image
-    torch.randn(100, 200) | toPIL()
-    # grabs image, converts to byte stream, and converts back to image
-    "abc.jpg" | toPIL() | toBytes() | toPIL()
-    # converts paragraphs to image
-    ["abc", "def"] | toPIL()
-    # converts SMILES string to molecule, then to image
-    "c1ccc(C)cc1" | toMol() | toImg()
-
-You can also save a matplotlib figure by piping in a :class:`matplotlib.figure.Figure` object::
-
-    x = np.linspace(0, 4)
-    plt.plot(x, x**2)
-    plt.gcf() | toPIL()
-
-.. note::
-
-    If you are working with image tensors, which is typically have
-    dimensions of (C, H, W), you have to permute it to PIL's (H, W, C)
-    first before passing it into this cli.
-
-    Also it's expected that
-    your tensor image ranges from 0-255, and not 0-1. Make sure you
-    renormalize it
-
-:param closeFig: if input is a matplotlib figure, then closes the figure after generating the image
-:param crop: whether to crop white spaces around an image or not"""              # toPIL
-        import PIL; self.PIL = PIL; self.closeFig = closeFig; self.crop = crop   # toPIL
-    def _typehint(self, inp):                                                    # toPIL
-        return PIL.Image.Image                                                   # toPIL
-    def __ror__(self, path) -> "PIL.Image.Image":                                # toPIL
-        if isinstance(path, str):                                                # toPIL
-            return self.PIL.Image.open(os.path.expanduser(path))                 # toPIL
-        if isinstance(path, bytes):                                              # toPIL
-            return self.PIL.Image.open(io.BytesIO(path))                         # toPIL
-        if isinstance(path, torch.Tensor): path = path.numpy()                   # toPIL
-        if isinstance(path, np.ndarray):                                         # toPIL
-            return self.PIL.Image.fromarray(path.astype("uint8"))                # toPIL
-        if isinstance(path, mpl.figure.Figure):                                  # toPIL
-            canvas = path.canvas; canvas.draw()                                  # toPIL
-            img = self.PIL.Image.frombytes('RGB', canvas.get_width_height(), canvas.tostring_rgb()) # toPIL
-            if self.closeFig: plt.close(path)                                    # toPIL
-            return img | cli.aS(cropToContentPIL)                                # toPIL
-        if isinstance(path, graphviz.Digraph):                                   # toPIL
-            import tempfile; a = tempfile.NamedTemporaryFile()                   # toPIL
-            path.render(a.name, format="jpeg");                                  # toPIL
-            fn = f"{a.name}.jpeg"; im = fn | toImg()                             # toPIL
-            try: os.remove(fn)                                                   # toPIL
-            except: pass                                                         # toPIL
-            return im                                                            # toPIL
-        if hasRdkit and isinstance(path, rdkit.Chem.rdchem.Mol):                 # toPIL
-            sz = settings.chem.imgSize                                           # toPIL
-            return self.__ror__(rdkit.Chem.Draw.MolsToGridImage([path], subImgSize=[sz, sz]).data) | (cli.aS(cropToContentPIL) if self.crop else cli.iden()) # toPIL
-        path = path | cli.deref()                                                # toPIL
-        if len(path) > 0 and isinstance(path[0], str):                           # toPIL
-            from PIL import ImageDraw                                            # toPIL
-            h = path | cli.shape(0); w = path | cli.shape(0).all() | cli.aS(max) # toPIL
-            image = self.PIL.Image.new("L", ((w+1)*20, (h+1)*60), 255)           # toPIL
-            font = PIL.ImageFont.truetype(settings.font, 18) if settings.font else None # toPIL
-            ImageDraw.Draw(image).text((20, 20), path | cli.join("\n"), 0, font=font) # toPIL
-            return np.array(image)/255 | (cli.aS(cropToContentNp) if self.crop else iden()) | cli.op()*255 | toImg() # toPIL
-        return NotImplemented                                                    # toPIL
-toImg = toPIL                                                                    # toPIL
-class toRgb(BaseCli):                                                            # toRgb
-    def __init__(self):                                                          # toRgb
-        """Converts greyscale/rgb PIL image to rgb image.
-Example::
-
-    # reads image file and converts it to rgb
-    "a.png" | toPIL() | toRgb()"""                                               # toRgb
-        import PIL; self.PIL = PIL                                               # toRgb
-    def _typehint(self, inp): return inp                                         # toRgb
-    def __ror__(self, i):                                                        # toRgb
-        if i.getbands() == ("R", "G", "B"): return i                             # toRgb
-        rgbI = self.PIL.Image.new("RGB", i.size)                                 # toRgb
-        rgbI.paste(i); return rgbI                                               # toRgb
-class toRgba(BaseCli):                                                           # toRgba
-    def __init__(self):                                                          # toRgba
-        """Converts random PIL image to rgba image.
-Example::
-
-    # reads image file and converts it to rgba
-    "a.png" | toPIL() | toRgba()"""                                              # toRgba
-        import PIL; self.PIL = PIL                                               # toRgba
-    def _typehint(self, inp): return inp                                         # toRgba
-    def __ror__(self, i):                                                        # toRgba
-        if i.getbands() == ("R", "G", "B", "A"): return i                        # toRgba
-        rgbI = self.PIL.Image.new("RGBA", i.size)                                # toRgba
-        rgbI.paste(i); return rgbI                                               # toRgba
-class toGray(BaseCli):                                                           # toGray
-    def __init__(self):                                                          # toGray
-        """Converts random PIL image to a grayscale image.
-Example::
-
-    # reads image file and converts it to rgba
-    "a.png" | toPIL() | toGray()"""                                              # toGray
-        import PIL; self.PIL = PIL                                               # toGray
-    def _typehint(self, inp): return inp                                         # toGray
-    def __ror__(self, i):                                                        # toGray
-        if i.getbands() == ("L"): return i                                       # toGray
-        return self.PIL.ImageOps.grayscale(i)                                    # toGray
-class toDict(BaseCli):                                                           # toDict
-    def __init__(self, rows=True, f=None):                                       # toDict
-        """Converts 2 Iterators, 1 key, 1 value into a dictionary.
-Example::
-
-    # returns {1: 3, 2: 4}
-    [[1, 3], [2, 4]] | toDict()
-    # returns {1: 3, 2: 4}
-    [[1, 2], [3, 4]] | toDict(False)
-
-If ``rows`` is a string, then it will build a dictionary from key-value
-pairs delimited by this character. For example::
-
-    ['gene_id "ENSG00000290825.1"',
-     'transcript_id "ENST00000456328.2"',
-     'gene_type "lncRNA"',
-     'gene_name "DDX11L2"',
-     'transcript_type "lncRNA"',
-     'transcript_name "DDX11L2-202"',
-     'level 2',
-     'transcript_support_level "1"',
-     'tag "basic"',
-     'tag "Ensembl_canonical"',
-     'havana_transcript "OTTHUMT00000362751.1"'] | toDict(" ")
-
-That returns::
-
-    {'gene_id': '"ENSG00000290825.1"',
-     'transcript_id': '"ENST00000456328.2"',
-     'gene_type': '"lncRNA"',
-     'gene_name': '"DDX11L2"',
-     'transcript_type': '"lncRNA"',
-     'transcript_name': '"DDX11L2-202"',
-     'level': '2',
-     'transcript_support_level': '"1"',
-     'tag': '"Ensembl_canonical"',
-     'havana_transcript': '"OTTHUMT00000362751.1"'}
-
-:param rows: if True, reads input in row by row, else reads
-    in list of columns
-:param f: if specified, return a defaultdict that uses this function as its generator""" # toDict
-        self.rows = rows                                                         # toDict
-        if f is not None: self.f = lambda d: defaultdict(f, d)                   # toDict
-        else: self.f = lambda x: x                                               # toDict
-    def __ror__(self, it:Tuple[Iterator[T], Iterator[T]]) -> dict:               # toDict
-        r = self.rows; f = self.f                                                # toDict
-        if r:                                                                    # toDict
-            if isinstance(r, str): return it | cli.apply(cli.aS(lambda x: x.split(" ")) | cli.head(1).split() | cli.item() + cli.join(" ")) | toDict() # toDict
-            return f({_k:_v for _k, _v in it})                                   # toDict
-        return f({_k:_v for _k, _v in zip(*it)})                                 # toDict
-def _toop(toOp, c, force, defaultValue):                                         # _toop
-    return cli.apply(toOp, c) | (cli.apply(lambda x: x or defaultValue, c) if force else cli.filt(cli.op() != None, c)) # _toop
-def _toFloat(e) -> Union[float, None]:                                           # _toFloat
-    try: return float(e)                                                         # _toFloat
-    except: return None                                                          # _toFloat
-class toFloat(BaseCli):                                                          # toFloat
-    def __init__(self, *columns, mode=2):                                        # toFloat
-        """Converts every row into a float. Example::
-
-    # returns [1, 3, -2.3]
-    ["1", "3", "-2.3"] | toFloat() | deref()
-    # returns [[1.0, 'a'], [2.3, 'b'], [8.0, 'c']]
-    [["1", "a"], ["2.3", "b"], [8, "c"]] | toFloat(0) | deref()
-
-With weird rows::
-
-    # returns [[1.0, 'a'], [8.0, 'c']]
-    [["1", "a"], ["c", "b"], [8, "c"]] | toFloat(0) | deref()
-    # returns [[1.0, 'a'], [0.0, 'b'], [8.0, 'c']]
-    [["1", "a"], ["c", "b"], [8, "c"]] | toFloat(0, force=True) | deref()
-
-This also works well with :class:`torch.Tensor` and :class:`numpy.ndarray`,
-as they will not be broken up into an iterator::
-
-    # returns a numpy array, instead of an iterator
-    np.array(range(10)) | toFloat()
-
-:param columns: if nothing, then will convert each row. If available, then
-    convert all the specified columns
-:param mode: different conversion styles
-    - 0: simple ``float()`` function, fastest, but will throw errors if it can't be parsed
-    - 1: if there are errors, then replace it with zero
-    - 2: if there are errors, then eliminate the row"""                          # toFloat
-        self.columns = columns; self.mode = mode;                                # toFloat
-    def __ror__(self, it):                                                       # toFloat
-        columns = self.columns; mode = self.mode                                 # toFloat
-        if len(columns) == 0:                                                    # toFloat
-            if isinstance(it, np.ndarray): return it.astype(float)               # toFloat
-            if isinstance(it, torch.Tensor): return it.float()                   # toFloat
-            if mode == 0: return it | cli.apply(float)                           # toFloat
-            return it | _toop(_toFloat, None, mode == 1, 0.0)                    # toFloat
-        else: return it | cli.init.serial(*(_toop(_toFloat, c, mode == 1, 0.0) for c in columns)) # toFloat
-def _toInt(e) -> Union[int, None]:                                               # _toInt
-    try: return int(float(e))                                                    # _toInt
-    except: return None                                                          # _toInt
-class toInt(BaseCli):                                                            # toInt
-    def __init__(self, *columns, mode=2):                                        # toInt
-        """Converts every row into an integer. Example::
-
-    # returns [1, 3, -2]
-    ["1", "3", "-2.3"] | toInt() | deref()
-
-:param columns: if nothing, then will convert each row. If available, then
-    convert all the specified columns
-:param mode: different conversion styles
-    - 0: simple ``float()`` function, fastest, but will throw errors if it can't be parsed
-    - 1: if there are errors, then replace it with zero
-    - 2: if there are errors, then eliminate the row
-
-See also: :meth:`toFloat`"""                                                     # toInt
-        self.columns = columns; self.mode = mode;                                # toInt
-    def __ror__(self, it):                                                       # toInt
-        columns = self.columns; mode = self.mode                                 # toInt
-        if len(columns) == 0:                                                    # toInt
-            if isinstance(it, np.ndarray): return it.astype(int)                 # toInt
-            if isinstance(it, torch.Tensor): return it.int()                     # toInt
-            if mode == 0: return it | cli.apply(int)                             # toInt
-            return it | _toop(_toInt, None, mode == 1, 0.0)                      # toInt
-        else: return it | cli.init.serial(*(_toop(_toInt, c, mode == 1, 0.0) for c in columns)) # toInt
-class toBytes(BaseCli):                                                          # toBytes
-    def __init__(self, imgType="JPEG"):                                          # toBytes
-        """Converts several object types to bytes.
-Example::
-
-    # converts string to bytes
-    "abc" | toBytes()
-    # converts image to base64 bytes
-    torch.randn(200, 100) | toImg() | toBytes()
-
-
-.. admonition:: Custom datatype
-
-    It is possible to build objects that can interoperate with this cli,
-    like this::
-
-        class custom1:
-            def __init__(self, config=None): ...
-            def _toBytes(self): return b"abc"
-
-        custom1() | toBytes() # returns b"abc"
-
-    When called upon, :class:`toBytes` will detect that the input has the ``_toBytes``
-    method, which will prompt it to execute that method of the complex object. Of
-    course, this means that you can return anything, not necessarily bytes, but to
-    maintain intuitiveness, you should return either bytes or iterator of bytes
-
-:param imgType: if input is an image then this is the image type. Can
-    change to "PNG" or sth like that"""                                          # toBytes
-        self.imgType = imgType                                                   # toBytes
-    def __ror__(self, it):                                                       # toBytes
-        if isinstance(it, str): return it.encode()                               # toBytes
-        if hasPIL:                                                               # toBytes
-            if isinstance(it, PIL.Image.Image):                                  # toBytes
-                it = it | toRgb(); buffered = io.BytesIO()                       # toBytes
-                it.save(buffered, format=self.imgType); return buffered.getvalue() # toBytes
-        if hasattr(it, "_toBytes"): return it._toBytes()                         # toBytes
-        import dill; return dill.dumps(it)                                       # toBytes
-class toHtml(BaseCli):                                                           # toHtml
-    def __init__(self):                                                          # toHtml
-        """Converts several object types to bytes.
-Example::
-
-    # converts PIL image to html <img> tag
-    torch.randn(200, 100) | toImg() | toHtml()
-"""                                                                              # toHtml
-        pass                                                                     # toHtml
-    def __ror__(self, it):                                                       # toHtml
-        if hasPIL:                                                               # toHtml
-            if isinstance(it, PIL.Image.Image):                                  # toHtml
-                it = it | toBytes(imgType="PNG") | cli.aS(base64.b64encode) | cli.op().decode() # toHtml
-                return f"<img src=\"data:image/png;base64, {it}\" />"            # toHtml
-        if hasPlotly:                                                            # toHtml
-            if isinstance(it, plotly.graph_objs._figure.Figure):                 # toHtml
-                out = io.StringIO(); it.write_html(out); out.seek(0); return out.read() # toHtml
-        try: return it._repr_html_()                                             # toHtml
-        except: return it.__repr__()                                             # toHtml
-try:                                                                             # toHtml
-    from rdkit import Chem                                                       # toHtml
-    from rdkit.Chem import Draw                                                  # toHtml
-    from rdkit.Chem import AllChem                                               # toHtml
-    from rdkit.Chem.Draw import IPythonConsole                                   # toHtml
-    IPythonConsole.drawOptions.addAtomIndices = True                             # toHtml
-    __all__ = [*__all__, "toMol", "toSmiles"]                                    # toHtml
-    def toMol():                                                                 # toHtml
-        """Smiles to molecule.
-Example::
-
-    "c1ccc(C)cc1" | toMol()"""                                                   # toHtml
-        return cli.aS(Chem.MolFromSmiles)                                        # toHtml
-    def toSmiles():                                                              # toHtml
-        """Molecule to smiles.
-Example::
-
-    "c1ccc(C)cc1" | toMol() | toSmiles()"""                                      # toHtml
-        return cli.aS(Chem.MolToSmiles)                                          # toHtml
-except: pass                                                                     # toHtml
-import unicodedata, hashlib                                                      # toHtml
-def toAscii():                                                                   # toAscii
-    """Converts complex unicode text to its base ascii form.
-Example::
-
-    "hà nội" | toAscii() # returns "ha noi"
-
-Taken from https://stackoverflow.com/questions/2365411/convert-unicode-to-ascii-without-errors-in-python""" # toAscii
-    return cli.aS(lambda word: unicodedata.normalize('NFKD', word).encode('ascii', 'ignore')) # toAscii
-def toHash() -> str:                                                             # toHash
-    """Converts some string into some hash string.
-Example::
-
-    "abc" | toHash() # returns 'gASVJAAAAAAAAABDILp4Fr+PAc/qQUFA3l2uIiOwA2Gjlhd6nLQQ/2HyABWtlC4='
-
-Why not just use the builtin function ``hash("abc")``? Because it generates different
-hashes for different interpreter sessions, and that breaks many of my applications that
-need the hash value to stay constant forever."""                                 # toHash
-    def hashF(msg:str) -> str: m = hashlib.sha256(); m.update(f"{msg}".encode()); return k1lib.encode(m.digest()) # toHash
-    return cli.aS(hashF)                                                         # toHash
-import csv; pd = k1lib.dep("pandas")                                             # toHash
-class toCsv(BaseCli):                                                            # toCsv
-    def __init__(self, allSheets=False):                                         # toCsv
-        """Converts a csv file name into a table.
-Example::
+except: hasTorch = False; torch = k1lib.dep("torch")
 
-    "abc.csv"  | toCsv()     # returns table of values
-    "def.xlsx" | toCsv()     # returns table of values in the first sheet
-    "def.xlsx" | toCsv(True) # returns List[Sheet name (str), table of values]
-
-:param allSheets: if input is an Excel sheet, whether to read in all sheets or
-    just the first sheet. No effect if input is a normal csv file"""             # toCsv
-        self.allSheets = allSheets                                               # toCsv
-    def __ror__(self, fn:str):                                                   # toCsv
-        fn = os.path.expanduser(fn)                                              # toCsv
-        if fn.endswith(".xls") or fn.endswith(".xlsx"):                          # toCsv
-            if self.allSheets: return [[k, v.values] for k,v in pd.read_excel(fn, sheet_name=None).items()] # toCsv
-            else: return pd.read_excel(fn).values                                # toCsv
-        def gen():                                                               # toCsv
-            with open(fn) as f: yield from csv.reader(f)                         # toCsv
-        return gen()                                                             # toCsv
+__all__ = ["BaseCli", "Table", "T", "fastF", "yieldT",
+           "serial", "oneToMany", "mtmS"]
+settings = k1lib.Settings()
+atomic = k1lib.Settings()
+settings.add("atomic", atomic, "classes/types that are considered atomic and specified cli tools should never try to iterate over them")
+settings.add("defaultDelim", "\t", "default delimiter used in-between columns when creating tables. Defaulted to tab character.")
+settings.add("defaultIndent", "  ", "default indent used for displaying nested structures")
+settings.add("strict", False, "turning it on can help you debug stuff, but could also be a pain to work with")
+settings.add("inf", float("inf"), "infinity definition for many clis. Here because you might want to temporarily not loop things infinitely")
+k1lib.settings.add("cli", settings, "from k1lib.cli module")
+yieldT = object()
+def patchDefaultDelim(st:str):                                                   # patchDefaultDelim
+    """
+:param s:
+    - if not None, returns self
+    - else returns the default delimiter in :attr:`~k1lib.settings`"""           # patchDefaultDelim
+    return settings.defaultDelim if st is None else st                           # patchDefaultDelim
+def patchDefaultIndent(st:str):                                                  # patchDefaultIndent
+    """
+:param s:
+    - if not None, returns self
+    - else returns the default indent character in :attr:`~k1lib.settings`"""    # patchDefaultIndent
+    return settings.defaultIndent if st is None else st                          # patchDefaultIndent
+T = TypeVar("T")                                                                 # patchDefaultIndent
+"""Generic type variable"""                                                      # patchDefaultIndent
+class _MetaType(type):                                                           # _MetaType
+    def __getitem__(self, generic):                                              # _MetaType
+        d = {"__args__": generic, "_n": self._n, "__doc__": self.__doc__}        # _MetaType
+        return _MetaType(self._n, (), d)                                         # _MetaType
+    def __repr__(self):                                                          # _MetaType
+        def main(self):                                                          # _MetaType
+            def trueName(o):                                                     # _MetaType
+                if isinstance(o, _MetaType): return main(o)                      # _MetaType
+                try: return o.__name__                                           # _MetaType
+                except: return f"{o}"                                            # _MetaType
+            if hasattr(self, "__args__"):                                        # _MetaType
+                if isinstance(self.__args__, tuple):                             # _MetaType
+                    return f"{self._n}[{', '.join([trueName(e) for e in self.__args__])}]" # _MetaType
+                else: return f"{self._n}[{trueName(self.__args__)}]"             # _MetaType
+            return self._n                                                       # _MetaType
+        return main(self)                                                        # _MetaType
+def newTypeHint(name, docs=""):                                                  # newTypeHint
+    """Creates a new type hint that can be sliced and yet still looks fine
+in sphinx. Crudely written by my poorly understood idea of Python's
+metaclasses. Seriously, this shit is bonkers, read over it https://stackoverflow.com/questions/100003/what-are-metaclasses-in-python
+
+Example::
+
+    Table = newTypeHint("Table", "some docs")
+    Table[int] # prints out as "Table[int]", and sphinx fell for it too
+    Table[Table[str], float] # prints out as "Table[Table[str], float]"
+"""                                                                              # newTypeHint
+    return _MetaType(name, (), {"_n": name, "__doc__": docs})                    # newTypeHint
+#Table = newTypeHint("Table", """Essentially just Iterator[List[T]]. This class is just here so that I can generate the docs with nicely formatted types like "Table[str]".""") # newTypeHint
+#Table = NewType("Table", List)                                                  # newTypeHint
+class Table(Generic[T]):                                                         # Table
+    """Essentially just Iterator[List[T]]. This class is just here so that I can generate the docs with nicely formatted types like "Table[str]".""" # Table
+    pass                                                                         # Table
+Table._name = "Table"                                                            # Table
+#Table.__module__ = "cli"                                                        # Table
+class Row(list):                                                                 # Row
+    """Not really used currently. Just here for potential future feature"""      # Row
+    pass                                                                         # Row
+class BaseCli:                                                                   # BaseCli
+    """A base class for all the cli stuff. You can definitely create new cli tools that
+have the same feel without extending from this class, but advanced stream operations
+(like ``+``, ``&``, ``.all()``, ``|``) won't work.
+
+At the moment, you don't have to call super().__init__() and super().__ror__(),
+as __init__'s only job right now is to solidify any :class:`~k1lib.cli.modifier.op`
+passed to it, and __ror__ does nothing."""                                       # BaseCli
+    def __init__(self, fs:list=[], capture=False):                               # BaseCli
+        """Not expected to be instantiated by the end user.
+
+**fs param**
+
+Expected to use it like this::
+
+    class A(BaseCli):
+        def __init__(self, f):
+            fs = [f]; super().__init__(fs); self.f = fs[0]
+
+Where ``f`` is some (potentially exotic) function. This will replace f with a "normal"
+function that's executable. See source code of :class:`~k1lib.cli.filt.filt` for an
+example of why this is useful. Currently, it will:
+
+- Replace with last recorded ``4 in op()``, if ``f`` is :data:`True`, because Python does
+  not allow returning complex objects from __contains__ method
+- Solidifies every :class:`~k1lib.cli.modifier.op`.
+
+:param capture: whether to capture all clis to the right of it and make it accessible under capturedClis and capturedSerial properties""" # BaseCli
+        if isinstance(fs, tuple): raise AttributeError("`fs` should not be a tuple. Use a list instead, so that new functions can be returned") # BaseCli
+        _k1_init_l = []                                                          # BaseCli
+        for _k1_init_f in fs: cli.op.solidify(_k1_init_f); _k1_init_l.append(_k1_init_f) # this is supposed to turn the exotic function into a normal function and leave normal functions alone. Purposefully don't do heavy optimizations here, cause we might want to poke around and change its internal representation # BaseCli
+        fs.clear(); fs.extend(_k1_init_l);                                       # BaseCli
+        self.capture = capture; self._capturedClis = []; self._capturedSerial = None # BaseCli
+    @property                                                                    # BaseCli
+    def capturedClis(self):                                                      # BaseCli
+        if isinstance(self._capturedClis, list):                                 # BaseCli
+            ans = []                                                             # BaseCli
+            for e in self._capturedClis: ans.append(cli.op.solidify(e))          # BaseCli
+            self._capturedClis = tuple(ans)                                      # BaseCli
+        return self._capturedClis                                                # BaseCli
+    @property                                                                    # BaseCli
+    def capturedSerial(self):                                                    # BaseCli
+        if not self.capture: return None                                         # BaseCli
+        if self._capturedSerial is None: self._capturedSerial = serial(*self.capturedClis) # BaseCli
+        return self._capturedSerial                                              # BaseCli
+    def hint(self, _hint:"cli.typehint.tBase"):                                  # BaseCli
+        """Specifies output type hint."""                                        # BaseCli
+        self._hint = _hint; return self                                          # BaseCli
+    @property                                                                    # BaseCli
+    def hasHint(self): return "_hint" in self.__dict__ and self._hint is not None # BaseCli
+    def _typehint(self, inp:"cli.typehint.tBase"=None) -> "cli.typehint.tBase": return cli.typehint.tAny() if "_hint" not in self.__dict__ else self._hint # BaseCli
+    def __and__(self, cli:"BaseCli") -> "oneToMany":                             # BaseCli
+        """Duplicates input stream to multiple joined clis.
+Example::
+
+    # returns [[5], [0, 1, 2, 3, 4]]
+    range(5) | (shape() & iden()) | deref()
+
+Kinda like :class:`~k1lib.cli.modifier.apply`. There're just multiple ways of doing
+this. This I think, is more intuitive, and :class:`~k1lib.cli.modifier.apply` is more
+for lambdas and columns mode. Performances are pretty much identical."""         # BaseCli
+        if isinstance(self, oneToMany): return self._copy()._after(cli)          # BaseCli
+        if isinstance(cli, oneToMany): return cli._copy()._before(self)          # BaseCli
+        return oneToMany(self, cli)                                              # BaseCli
+    def __add__(self, cli:"BaseCli") -> "mtmS":                                  # BaseCli
+        """Parallel pass multiple streams to multiple clis.
+Example::
+
+    # returns [8, 15]
+    [2, 3] | ((op() * 4) + (op() * 5)) | deref()"""                              # BaseCli
+        if isinstance(self, mtmS): return self._copy()._after(cli)               # BaseCli
+        if isinstance(cli, mtmS): return cli._copy()._before(self)               # BaseCli
+        return mtmS(self, cli)                                                   # BaseCli
+    def all(self, n:int=1) -> "BaseCli":                                         # BaseCli
+        """Applies this cli to all incoming streams.
+Example::
+
+    # returns (3,)
+    torch.randn(3, 4) | toMean().all() | shape()
+    # returns (3, 4)
+    torch.randn(3, 4, 5) | toMean().all(2) | shape()
+
+:param n: how many times should I chain ``.all()``?"""                           # BaseCli
+        if n < 0: raise AttributeError(f"Does not make sense for `n` to be \"{n}\"") # BaseCli
+        s = self                                                                 # BaseCli
+        for i in range(n): s = cli.apply(s)                                      # BaseCli
+        return s                                                                 # BaseCli
+    def __or__(self, cli_) -> "serial": # cli is guaranteed (by typical usage, not law) that it's a BaseCli # BaseCli
+        """Joins clis end-to-end.
+Example::
+
+    c = apply(op() ** 2) | deref()
+    # returns [0, 1, 4, 9, 16]
+    range(5) | c"""                                                              # BaseCli
+        if not isinstance(self, cli.op):                                         # BaseCli
+            if not hasattr(self, "capture"): self.capture = False                # BaseCli
+            if self.capture: self._capturedClis.append(cli_); return self        # BaseCli
+        if isinstance(self, serial): return self._copy()._after(cli_)            # BaseCli
+        if isinstance(cli_, serial): return cli_._copy()._before(self)           # BaseCli
+        return serial(self, cli_)                                                # BaseCli
+    def __ror__(self, it): return NotImplemented                                 # BaseCli
+    def f(self) -> Table[Table[int]]:                                            # BaseCli
+        """Creates a normal function :math:`f(x)` which is equivalent to
+``x | self``."""                                                                 # BaseCli
+        return lambda it: self.__ror__(it)                                       # BaseCli
+    def __lt__(self, it):                                                        # BaseCli
+        """Backup pipe symbol `>`, purely for style, so that you can do something like
+this::
+
+    range(4) > file("a.txt")"""                                                  # BaseCli
+        return self.__ror__(it)                                                  # BaseCli
+    def __call__(self, it, *args):                                               # BaseCli
+        """Another way to do ``it | cli``. If multiple arguments are fed, then the
+argument list is passed to cli instead of just the first element. Example::
+
+    @applyS
+    def f(it):
+        return it
+    f(2) # returns 2
+    f(2, 3) # returns [2, 3]"""                                                  # BaseCli
+        if len(args) == 0: return self.__ror__(it)                               # BaseCli
+        else: return self.__ror__([it, *args])                                   # BaseCli
+    def __neg__(self):                                                           # BaseCli
+        """Alias for __invert__, for clis that support inverting stuff."""       # BaseCli
+        return ~self                                                             # BaseCli
+    def _all_array_opt(self, it, level:int):                                     # BaseCli
+        """Array types optimization for ``operator.all(level)``.
+
+Essentially, a lot of times, I'm trying to do ``array | op()[3].all()``,
+or ``array | transpose().all()``. But without this optimization, that ``.all()``
+function kinda loops through each element and operates on them in vanilla Python,
+which is super slow. So, this is a mechanism to speed it up. Here's how it works::
+
+    # you wrote this
+    array | operator.all() | deref()
+    # apply() detects that you're trying to operate on an array type. It then figures
+    # out how many nested apply() levels are there. In this case it's 1, so apply() returns this instead
+    operator._all_array_opt(array, 1)
+    # if that throws an error or returns NotImplemented, then it'll just loop through the array normally
+
+    # if you wrote this instead
+    array | operator.all(3) | deref()
+    # or this
+    array | apply(apply(operator.all())) | deref()
+    # apply() will try to execute this instead
+    operator._all_array_opt(array, 3)
+
+Also, if the operator is a complex one, made of an entire pipeline, then ``serial`` can break
+them apart and do this kind of optimization on each simple operator like this::
+
+    operator = op()[3] | transpose()
+    array | operator.all() | deref()
+    # that gets transformed into this
+    array | op()[3].all() | transpose().all() | deref()
+    # then, array() will be called 2 times
+    arr2 = op()[3]._all_array_opt(array, 1)
+    transpose()._all_array_opt(arr2, 1)
+
+It also works on something more complicated and nested like this::
+
+    # returns
+    np.random.randn(3,4,5,6,7,8) | apply(transpose().all(3) | item()) | shape()
+
+This breakdown also happens with op() (anticipated feature, not implemented yet)::
+
+    array | op()[3][:4].all() | deref()
+    # this will be broken down into
+    array | op()[3].all() | op()[:4].all() | deref()
+    # each piece will now have a chance to optimize the array structure independently,
+    # so even if op()[:4] can't be done, op()[3] still have a chance to do the C-optimized version
+
+Why don't I build a more standardized structure for these optimization passes? Well
+I did, along the lines of LLVM. But, the whole optimization process kinda takes a long
+time and I'm not sure if it's truly flexible for the kinds of workloads that I'm thinking
+about. So, I'll just do this quick dumb optimization hack to get it over with, and when
+I can think more clearly about this, I might move this mechanism back to LLVM.""" # BaseCli
+        return NotImplemented                                                    # BaseCli
+def _k1_init_frames():                                                           # _k1_init_frames
+    _k1_init_frames_count = 0                                                    # _k1_init_frames
+    try:                                                                         # _k1_init_frames
+        while True:                                                              # _k1_init_frames
+            yield sys._getframe(_k1_init_frames_count) # `sys._getframe()` trick stolen from pd.DataFrame.query # _k1_init_frames
+            _k1_init_frames_count += 1                                           # _k1_init_frames
+    except: pass                                                                 # _k1_init_frames
+def _k1_global_frame():                                                          # _k1_global_frame
+    try:                                                                         # _k1_global_frame
+        _k1_init_frames_ans = {}                                                 # _k1_global_frame
+        for _k1_init_frames_frame in reversed(list(_k1_init_frames())):          # _k1_global_frame
+            _k1_init_frames_ans = {**_k1_init_frames_ans, **_k1_init_frames_frame.f_locals} # _k1_global_frame
+        return _k1_init_frames_ans                                               # _k1_global_frame
+    except: return {}                                                            # _k1_global_frame
+def fastF(c, x=None):                                                            # fastF
+    """Tries to figure out what's going on, is it a normal function, or an applyS,
+or a BaseCli, etc., and return a really fast function for execution. Example::
+
+    # both returns 16, fastF returns "lambda x: x**2", so it's really fast
+    fastF(op()**2)(4)
+    fastF(applyS(lambda x: x**2))(4)
+
+At the moment, parameter ``x`` does nothing, but potentially in the future, you can
+pass in an example input to the cli, so that this returns an optimized, C compiled
+version.
+
+:param x: sample data for the cli"""                                             # fastF
+    if isinstance(c, str): return fastF(eval(f"lambda x: {c}", _k1_global_frame())) # fastF
+    if isinstance(c, cli.op): return c.ab_fastF()                                # fastF
+    if isinstance(c, cli.applyS):                                                # fastF
+        f = fastF(c.f)                                                           # fastF
+        if len(c.args) == 0 and len(c.kwargs) == 0: return f                     # fastF
+        else: return lambda x, *args, **kwargs: f(x, *c.args, **c.kwargs)        # fastF
+    if isinstance(c, BaseCli): return c.__ror__                                  # fastF
+    return c                                                                     # fastF
+def checkRor(c):                                                                 # checkRor
+    if isinstance(c, BaseCli): return c                                          # checkRor
+    if hasattr(c, "__ror__"): return cli.aS(c.__ror__)                           # checkRor
+    if callable(c): return cli.aS(c)                                             # checkRor
+    raise Exception(f"Trying to add an operator to the pipeline, but the given object is not derived from BaseCli nor does it define a __ror__ method") # checkRor
+class serial(BaseCli):                                                           # serial
+    def __init__(self, *clis:List[BaseCli]):                                     # serial
+        """Merges clis into 1, feeding end to end. Used in chaining clis
+together without a prime iterator. Meaning, without this, stuff like this
+fails to run::
+
+    [1, 2] | a() | b() # runs
+    c = a() | b(); [1, 2] | c # doesn't run if this class doesn't exist"""       # serial
+        fs = [checkRor(c) for c in clis]; super().__init__(fs); self.clis = fs; self._cache() # serial
+    def _cache(self):                                                            # serial
+        self._hasTrace = any(isinstance(c, cli.trace) for c in self.clis)        # serial
+        self._cliCs = [fastF(c) for c in self.clis]; return self                 # serial
+    def _typehint(self, inp=None):                                               # serial
+        for c in self.clis: inp = c._typehint(inp) or cli.typehint.tAny()        # serial
+        return inp                                                               # serial
+    def __ror__(self, it:Iterator[Any]) -> Iterator[Any]:                        # serial
+        if self._hasTrace: # slower, but tracable                                # serial
+            for cli in self.clis: it = it | cli                                  # serial
+        else: # faster, but not tracable                                         # serial
+            for cli in self._cliCs: it = cli(it)                                 # serial
+        return it                                                                # serial
+    def _before(self, c): self.clis = [checkRor(c)] + self.clis; return self._cache() # serial
+    def _after (self, c): self.clis = self.clis + [checkRor(c)]; return self._cache() # serial
+    def _copy(self): return serial(*self.clis)                                   # serial
+atomic.add("baseAnd", (Number, np.number, str, dict, bool, bytes, list, tuple, *([torch.Tensor] if hasTorch else []), np.ndarray, xml.etree.ElementTree.Element), "used by BaseCli.__and__") # serial
+def _iterable(it):                                                               # _iterable
+    try: iter(it); return True                                                   # _iterable
+    except: return False                                                         # _iterable
+class oneToMany(BaseCli):                                                        # oneToMany
+    def __init__(self, *clis:List[BaseCli]):                                     # oneToMany
+        """Duplicates 1 stream into multiple streams, each for a cli in the
+list. Used in the "a & b" joining operator. See also: :meth:`BaseCli.__and__`""" # oneToMany
+        fs = [checkRor(c) for c in clis]; super().__init__(fs); self.clis = fs; self._cache() # oneToMany
+    def _typehint(self, inp):                                                    # oneToMany
+        ts = []                                                                  # oneToMany
+        for f in self.clis:                                                      # oneToMany
+            try: ts.append(f._typehint(inp))                                     # oneToMany
+            except: ts.append(cli.typehint.tAny())                               # oneToMany
+        return cli.typehint.tCollection(*ts).reduce()                            # oneToMany
+    def __ror__(self, it:Iterator[Any]) -> Iterator[Iterator[Any]]:              # oneToMany
+        if isinstance(it, atomic.baseAnd) or isinstance(it, k1lib.cli.splitSeek) or not _iterable(it): # oneToMany
+            for cli in self._cliCs: yield cli(it)                                # oneToMany
+        else:                                                                    # oneToMany
+            its = itertools.tee(it, len(self.clis))                              # oneToMany
+            for cli, it in zip(self._cliCs, its): yield cli(it)                  # oneToMany
+    def _cache(self): self._cliCs = [fastF(c) for c in self.clis]; return self   # oneToMany
+    def _before(self, c): self.clis = [checkRor(c)] + self.clis; return self._cache() # oneToMany
+    def _after(self, c): self.clis = self.clis + [checkRor(c)]; return self._cache() # oneToMany
+    def _copy(self): return oneToMany(*self.clis)                                # oneToMany
+class mtmS(BaseCli):                                                             # mtmS
+    def __init__(self, *clis:List[BaseCli]):                                     # mtmS
+        """Applies multiple streams to multiple clis independently. Used in
+the "a + b" joining operator. See also: :meth:`BaseCli.__add__`.
+
+Weird name is actually a shorthand for "many to many specific"."""               # mtmS
+        fs = [checkRor(c) for c in clis]; super().__init__(fs=fs); self.clis = fs; self._cache() # mtmS
+    def _inpTypeHintExpand(self, t):                                             # mtmS
+        n = len(self.clis);                                                      # mtmS
+        if isinstance(t, (cli.typehint.tCollection, *cli.typehint.tListIterSet, cli.typehint.tArrayTypes)): return t.expand(n) # mtmS
+        else: return [cli.typehint.tAny()]*n                                     # mtmS
+    def _typehint(self, t):                                                      # mtmS
+        n = len(self.clis); outTs = []                                           # mtmS
+        for c, t in zip(self.clis, self._inpTypeHintExpand(t)):                  # mtmS
+            try: outTs.append(c._typehint(t))                                    # mtmS
+            except: outTs.append(cli.typehint.tAny())                            # mtmS
+        return cli.typehint.tCollection(*outTs).reduce()                         # mtmS
+    def _cache(self): self._cliCs = [fastF(c) for c in self.clis]; return self   # mtmS
+    def _before(self, c): self.clis = [checkRor(c)] + self.clis; return self._cache() # mtmS
+    def _after (self, c): self.clis = self.clis + [checkRor(c)]; return self._cache() # mtmS
+    def __ror__(self, its:Iterator[Any]) -> Iterator[Any]:                       # mtmS
+        for cli, it in zip(self._cliCs, its): yield cli(it)                      # mtmS
+    @staticmethod                                                                # mtmS
+    def f(f, i:int, n:int=100):                                                  # mtmS
+        """Convenience method, so
+that this::
+
+    mtmS(iden(), op()**2, iden(), iden(), iden())
+    # also the same as this btw:
+    (iden() + op()**2 + iden() + iden() + iden())
+
+is the same as this::
+
+    mtmS.f(op()**2, 1, 5)
+
+Example::
+
+    # returns [5, 36, 7, 8, 9]
+    range(5, 10) | mtmS.f(op()**2, 1, 5) | deref()
+
+:param i: where should I put the function?
+:param n: how many clis in total? Defaulted to 100"""                            # mtmS
+        return mtmS(*([cli.iden()]*i + [f] + [cli.iden()]*(n-i-1)))              # mtmS
+    def _copy(self): return mtmS(*self.clis)                                     # mtmS
+def patchNumpy():                                                                # patchNumpy
+    """Patches numpy arrays and data types, so that piping like
+this work::
+
+    a = np.random.randn(3)
+    a | shape() # returns (3,)"""                                                # patchNumpy
+    try:                                                                         # patchNumpy
+        if np._k1_patched: return                                                # patchNumpy
+    except: pass                                                                 # patchNumpy
+    try:                                                                         # patchNumpy
+        import forbiddenfruit, inspect; #forbiddenfruit.reverse(np.ndarray, "__or__") # old version # patchNumpy
+        oldOr = np.ndarray.__or__                                                # patchNumpy
+        def _newNpOr(self, v):                                                   # patchNumpy
+            if isinstance(v, BaseCli): return NotImplemented                     # patchNumpy
+            try: return oldOr(self, v)                                           # patchNumpy
+            except: warnings.warn(traceback.format_exc())                        # patchNumpy
+        forbiddenfruit.curse(np.ndarray, "__or__", _newNpOr)                     # patchNumpy
+        a = [getattr(np, dk) for dk in np.__dict__.keys()] # patching all numpy's numeric types # patchNumpy
+        for _type in [x for x in a if inspect.isclass(x) and issubclass(x, np.number) and not issubclass(x, np.integer)]: # patchNumpy
+            _oldOr = _type.__or__                                                # patchNumpy
+            def _typeNewOr(self, v):                                             # patchNumpy
+                if isinstance(v, BaseCli): return NotImplemented                 # patchNumpy
+                try: return _oldOr(self, v)                                      # patchNumpy
+                except: warnings.warn(traceback.format_exc())                    # patchNumpy
+            forbiddenfruit.curse(_type, "__or__", _typeNewOr)                    # patchNumpy
+        np._k1_patched = True                                                    # patchNumpy
+    except Exception as e: warnings.warn(f"Tried to patch __or__ operator of built-in type `np.ndarray` but can't because: {e}") # patchNumpy
+dict_keys = type({"a": 3}.keys());   oldDKOr = dict_keys.__or__                  # patchNumpy
+dict_items = type({"a": 3}.items()); oldDIOr = dict_items.__or__                 # patchNumpy
+oldSetOr = set.__or__                                                            # patchNumpy
+def patchDict():                                                                 # patchDict
+    """Patches dictionaries's items and keys, so that piping
+works::
+
+    d = {"a": 3, "b": 4}
+    d.keys() | deref() # returns ["a", "b"]
+    d.items() | deref() # returns [["a", 3], ["b", 4]]"""                        # patchDict
+    try:                                                                         # patchDict
+        if np._k1_dict_patched: return                                           # patchDict
+    except: pass                                                                 # patchDict
+    try:                                                                         # patchDict
+        import forbiddenfruit, traceback                                         # patchDict
+        def _newDOr(self, v):                                                    # patchDict
+            """Why is this so weird? For some reason, if you patch dict_keys, you will
+            also patch dict_items. So, if you were to have 2 functions, one for each,
+            then they will override each other. The way forward is to have 1 single
+            function detect whether it's dict_keys or dict_items, and call the correct
+            original function. So why are there 2 curses? Well cause I'm lazy to check
+            for this behavior in multiple python versions, so just have 2 to make sure.""" # patchDict
+            if isinstance(v, BaseCli): return NotImplemented                     # patchDict
+            try:                                                                 # patchDict
+                # print(self, type(self), v, type(v))                            # patchDict
+                if isinstance(self, dict_keys): return oldDKOr(self, v)          # patchDict
+                elif isinstance(self, dict):                                     # patchDict
+                    if isinstance(v, dict_keys): return oldSetOr(set(self.keys()), set(v)) # patchDict
+                    return oldDIOr(self, v)                                      # patchDict
+                elif isinstance(self, set):                                      # patchDict
+                    if isinstance(v, dict_keys): return oldSetOr(self, set(v))   # patchDict
+                    return oldSetOr(self, v)                                     # patchDict
+            except:                                                              # patchDict
+                print(self, type(self), v, type(v))                              # patchDict
+                warnings.warn(traceback.format_exc())                            # patchDict
+                return NotImplemented                                            # patchDict
+        forbiddenfruit.curse(dict_keys, "__or__", _newDOr)                       # patchDict
+        forbiddenfruit.curse(dict_items, "__or__", _newDOr)                      # patchDict
+        np._k1_dict_patched = True                                               # patchDict
+    except Exception as e: warnings.warn(f"Tried to patch __or__ operator of built-in type `dict_keys` and `dict_items` but can't because: {e}") # patchDict
+def patchPandas():                                                               # patchPandas
+    """Patches panda's :class:`pandas.core.series.Series` and
+:class:`pandas.core.frame.DataFrame` so that piping works::
+
+    pd.read_csv("a.csv")["col3"] | shape()"""                                    # patchPandas
+    try:                                                                         # patchPandas
+        import pandas as pd                                                      # patchPandas
+    except: return                                                               # patchPandas
+    try:                                                                         # patchPandas
+        if pd._k1_patched: return                                                # patchPandas
+    except: pass                                                                 # patchPandas
+    try:                                                                         # patchPandas
+        import forbiddenfruit                                                    # patchPandas
+        oldPdSOr = pd.core.series.Series.__or__                                  # patchPandas
+        def _newPdSOr(self, v):                                                  # patchPandas
+            if isinstance(v, BaseCli): return NotImplemented                     # patchPandas
+            try: return oldPdSOr(self, v)                                        # patchPandas
+            except: warnings.warn(traceback.format_exc())                        # patchPandas
+        forbiddenfruit.curse(pd.core.series.Series, "__or__", _newPdSOr)         # patchPandas
+                                                                                 # patchPandas
+        oldPdDFOr = pd.core.frame.DataFrame                                      # patchPandas
+        def _newPdDFOr(self, v):                                                 # patchPandas
+            if isinstance(v, BaseCli): return NotImplemented                     # patchPandas
+            try: return oldPdDFOr(self, v)                                       # patchPandas
+            except: warnings.warn(traceback.format_exc())                        # patchPandas
+        forbiddenfruit.curse(pd.core.frame.DataFrame, "__or__", _newPdDFOr)      # patchPandas
+        pd._k1_patched = True                                                    # patchPandas
+    except Exception as e: warnings.warn(f"Tried to patch __or__ operator of built-in type `pd.core.series.Series` but can't because: {e}") # patchPandas
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `k1lib-1.4.3.3/k1lib/cli/filt.py` & `k1lib-1.4.3.4/k1lib/cli/filt.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/gb.py` & `k1lib-1.4.3.4/k1lib/cli/gb.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/grep.py` & `k1lib-1.4.3.4/k1lib/cli/grep.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/inp.py` & `k1lib-1.4.3.4/k1lib/cli/inp.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/ktree.py` & `k1lib-1.4.3.4/k1lib/cli/ktree.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/kxml.py` & `k1lib-1.4.3.4/k1lib/cli/kxml.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/lsext.py` & `k1lib-1.4.3.4/k1lib/cli/lsext.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/mgi.py` & `k1lib-1.4.3.4/k1lib/cli/mgi.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/models.py` & `k1lib-1.4.3.4/k1lib/cli/models.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/modifier.py` & `k1lib-1.4.3.4/k1lib/cli/modifier.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/mol.py` & `k1lib-1.4.3.4/k1lib/cli/mol.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/nb.py` & `k1lib-1.4.3.4/k1lib/cli/nb.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/optimizations.py` & `k1lib-1.4.3.4/k1lib/cli/optimizations.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/output.py` & `k1lib-1.4.3.4/k1lib/cli/output.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/sam.py` & `k1lib-1.4.3.4/k1lib/cli/sam.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/structural.py` & `k1lib-1.4.3.4/k1lib/cli/structural.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/trace.py` & `k1lib-1.4.3.4/k1lib/cli/trace.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/typehint.py` & `k1lib-1.4.3.4/k1lib/cli/typehint.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/cli/utils.py` & `k1lib-1.4.3.4/k1lib/cli/utils.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/eqn.py` & `k1lib-1.4.3.4/k1lib/eqn.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/fmt.py` & `k1lib-1.4.3.4/k1lib/fmt.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/graphEqn.py` & `k1lib-1.4.3.4/k1lib/graphEqn.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/imports.py` & `k1lib-1.4.3.4/k1lib/imports.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/k1ui/256.model.state_dict.pth` & `k1lib-1.4.3.4/k1lib/k1ui/256.model.state_dict.pth`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/k1ui/main.py` & `k1lib-1.4.3.4/k1lib/k1ui/main.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/k1ui/mouseKey.pth` & `k1lib-1.4.3.4/k1lib/k1ui/mouseKey.pth`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/knn.py` & `k1lib-1.4.3.4/k1lib/knn.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/p5.py` & `k1lib-1.4.3.4/k1lib/p5.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/schedule.py` & `k1lib-1.4.3.4/k1lib/schedule.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/selector.py` & `k1lib-1.4.3.4/k1lib/selector.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/serve/main.html` & `k1lib-1.4.3.4/k1lib/serve/main.html`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/serve/main.py` & `k1lib-1.4.3.4/k1lib/serve/main.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/serve/suffix.py` & `k1lib-1.4.3.4/k1lib/serve/suffix.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib/viz.py` & `k1lib-1.4.3.4/k1lib/viz.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/k1lib.egg-info/PKG-INFO` & `k1lib-1.4.3.4/k1lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k1lib
-Version: 1.4.3.3
+Version: 1.4.3.4
 Summary: Some nice ML overhaul
 Home-page: https://k1lib.com
 Author: Quang Ho
 Author-email: 157239q@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `k1lib-1.4.3.3/k1lib.egg-info/SOURCES.txt` & `k1lib-1.4.3.4/k1lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.3.3/setup.py` & `k1lib-1.4.3.4/setup.py`

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
-    version="1.4.3.3",
+    version="1.4.3.4",
     python_requires='>=3.7',
     install_requires=["numpy>=1.14", "matplotlib>=2.0", "dill", "forbiddenfruit", "wurlitzer", "validators"],
     extras_require={"all": deps},
     description="Some nice ML overhaul",
     url="https://k1lib.com",
     author="Quang Ho",
     author_email="157239q@gmail.com",
```

