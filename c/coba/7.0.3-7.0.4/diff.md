# Comparing `tmp/coba-7.0.3.tar.gz` & `tmp/coba-7.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coba-7.0.3.tar", last modified: Tue Jul 25 03:34:38 2023, max compression
+gzip compressed data, was "coba-7.0.4.tar", last modified: Wed Aug  2 22:01:12 2023, max compression
```

## Comparing `coba-7.0.3.tar` & `coba-7.0.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.556975 coba-7.0.3/
--rw-rw-rw-   0        0        0       40 2023-06-12 16:34:36.000000 coba-7.0.3/AUTHORS
--rw-rw-rw-   0        0        0     1593 2023-06-12 16:34:36.000000 coba-7.0.3/LICENSE
--rw-rw-rw-   0        0        0     7942 2023-07-25 03:34:38.556975 coba-7.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7327 2023-06-16 20:10:41.000000 coba-7.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.006947 coba-7.0.3/coba/
--rw-rw-rw-   0        0        0     1427 2023-07-25 02:03:33.000000 coba-7.0.3/coba/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.069639 coba-7.0.3/coba/backports/
--rw-rw-rw-   0        0        0       50 2023-07-20 03:01:25.000000 coba-7.0.3/coba/backports/__init__.py
--rw-rw-rw-   0        0        0      262 2023-07-20 02:54:01.000000 coba-7.0.3/coba/backports/metadata.py
-drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.096052 coba-7.0.3/coba/contexts/
--rw-rw-rw-   0        0        0      703 2023-06-22 17:38:27.000000 coba-7.0.3/coba/contexts/__init__.py
--rw-rw-rw-   0        0        0     9727 2023-06-12 16:34:36.000000 coba-7.0.3/coba/contexts/cachers.py
--rw-rw-rw-   0        0        0     9236 2023-07-20 02:56:24.000000 coba-7.0.3/coba/contexts/core.py
--rw-rw-rw-   0        0        0     9726 2023-06-12 16:34:36.000000 coba-7.0.3/coba/contexts/loggers.py
--rw-rw-rw-   0        0        0    15875 2023-07-20 03:19:10.000000 coba-7.0.3/coba/encodings.py
-drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.211009 coba-7.0.3/coba/environments/
--rw-rw-rw-   0        0        0     1448 2023-07-16 19:49:49.000000 coba-7.0.3/coba/environments/__init__.py
--rw-rw-rw-   0        0        0    22841 2023-07-20 03:16:24.000000 coba-7.0.3/coba/environments/core.py
--rw-rw-rw-   0        0        0    52650 2023-07-25 01:55:42.000000 coba-7.0.3/coba/environments/filters.py
--rw-rw-rw-   0        0        0    14347 2023-07-16 19:49:49.000000 coba-7.0.3/coba/environments/openml.py
--rw-rw-rw-   0        0        0     7646 2023-07-16 19:49:49.000000 coba-7.0.3/coba/environments/primitives.py
--rw-rw-rw-   0        0        0     2966 2023-07-16 19:49:49.000000 coba-7.0.3/coba/environments/serialized.py
--rw-rw-rw-   0        0        0     9524 2023-07-20 02:57:00.000000 coba-7.0.3/coba/environments/supervised.py
--rw-rw-rw-   0        0        0    24174 2023-07-20 02:57:08.000000 coba-7.0.3/coba/environments/synthetics.py
--rw-rw-rw-   0        0        0     6179 2023-06-12 16:34:36.000000 coba-7.0.3/coba/environments/templates.py
-drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.258300 coba-7.0.3/coba/evaluators/
--rw-rw-rw-   0        0        0      217 2023-06-24 23:45:33.000000 coba-7.0.3/coba/evaluators/__init__.py
--rw-rw-rw-   0        0        0    15064 2023-07-20 07:42:27.000000 coba-7.0.3/coba/evaluators/offline.py
--rw-rw-rw-   0        0        0    22406 2023-07-20 19:01:31.000000 coba-7.0.3/coba/evaluators/online.py
--rw-rw-rw-   0        0        0     2095 2023-07-16 19:49:49.000000 coba-7.0.3/coba/evaluators/primitives.py
--rw-rw-rw-   0        0        0     1126 2023-06-12 16:34:36.000000 coba-7.0.3/coba/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.289549 coba-7.0.3/coba/experiments/
--rw-rw-rw-   0        0        0      379 2023-06-22 17:38:27.000000 coba-7.0.3/coba/experiments/__init__.py
--rw-rw-rw-   0        0        0    10512 2023-07-16 19:49:49.000000 coba-7.0.3/coba/experiments/core.py
--rw-rw-rw-   0        0        0     7686 2023-07-16 19:49:49.000000 coba-7.0.3/coba/experiments/process.py
--rw-rw-rw-   0        0        0    65589 2023-07-25 03:02:35.000000 coba-7.0.3/coba/experiments/results.py
-drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.383751 coba-7.0.3/coba/learners/
--rw-rw-rw-   0        0        0      761 2023-07-16 19:49:49.000000 coba-7.0.3/coba/learners/__init__.py
--rw-rw-rw-   0        0        0     7907 2023-07-23 04:42:34.000000 coba-7.0.3/coba/learners/bandit.py
--rw-rw-rw-   0        0        0     8028 2023-07-23 04:42:34.000000 coba-7.0.3/coba/learners/corral.py
--rw-rw-rw-   0        0        0     4947 2023-06-23 09:01:59.000000 coba-7.0.3/coba/learners/linucb.py
--rw-rw-rw-   0        0        0      958 2023-07-16 19:49:49.000000 coba-7.0.3/coba/learners/misguided.py
--rw-rw-rw-   0        0        0     4376 2023-06-12 16:34:36.000000 coba-7.0.3/coba/learners/primitives.py
--rw-rw-rw-   0        0        0     8975 2023-07-21 04:36:06.000000 coba-7.0.3/coba/learners/safety.py
--rw-rw-rw-   0        0        0    30984 2023-07-23 04:42:34.000000 coba-7.0.3/coba/learners/vowpal.py
--rw-rw-rw-   0        0        0     4139 2023-07-16 19:49:49.000000 coba-7.0.3/coba/multiprocessing.py
-drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.462605 coba-7.0.3/coba/pipes/
--rw-rw-rw-   0        0        0     1456 2023-07-16 19:49:49.000000 coba-7.0.3/coba/pipes/__init__.py
--rw-rw-rw-   0        0        0     1890 2023-06-12 16:34:36.000000 coba-7.0.3/coba/pipes/core.py
--rw-rw-rw-   0        0        0    16751 2023-07-16 19:49:49.000000 coba-7.0.3/coba/pipes/filters.py
--rw-rw-rw-   0        0        0    16062 2023-07-20 05:27:58.000000 coba-7.0.3/coba/pipes/multiprocessing.py
--rw-rw-rw-   0        0        0     6622 2023-06-12 16:34:36.000000 coba-7.0.3/coba/pipes/primitives.py
--rw-rw-rw-   0        0        0    13003 2023-06-12 16:34:36.000000 coba-7.0.3/coba/pipes/readers.py
--rw-rw-rw-   0        0        0    19458 2023-07-20 02:58:18.000000 coba-7.0.3/coba/pipes/rows.py
--rw-rw-rw-   0        0        0     4474 2023-07-16 19:49:49.000000 coba-7.0.3/coba/pipes/sinks.py
--rw-rw-rw-   0        0        0     6483 2023-07-20 02:58:25.000000 coba-7.0.3/coba/pipes/sources.py
-drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.556975 coba-7.0.3/coba/primitives/
--rw-rw-rw-   0        0        0      477 2023-06-22 17:38:27.000000 coba-7.0.3/coba/primitives/__init__.py
--rw-rw-rw-   0        0        0      913 2023-06-16 20:10:41.000000 coba-7.0.3/coba/primitives/feedbacks.py
--rw-rw-rw-   0        0        0     4624 2023-07-20 08:45:03.000000 coba-7.0.3/coba/primitives/rewards.py
--rw-rw-rw-   0        0        0     4421 2023-07-16 19:49:49.000000 coba-7.0.3/coba/primitives/rows.py
--rw-rw-rw-   0        0        0      219 2023-07-19 06:20:25.000000 coba-7.0.3/coba/primitives/semantic.py
--rw-rw-rw-   0        0        0      657 2023-06-12 16:34:36.000000 coba-7.0.3/coba/primitives/types.py
--rw-rw-rw-   0        0        0    11151 2023-07-16 18:38:46.000000 coba-7.0.3/coba/random.py
--rw-rw-rw-   0        0        0     1479 2023-07-16 19:49:49.000000 coba-7.0.3/coba/register.py
--rw-rw-rw-   0        0        0    10657 2023-06-12 16:34:36.000000 coba-7.0.3/coba/registry.py
--rw-rw-rw-   0        0        0     9022 2023-07-20 02:56:10.000000 coba-7.0.3/coba/statistics.py
--rw-rw-rw-   0        0        0     5212 2023-06-12 16:34:36.000000 coba-7.0.3/coba/utilities.py
-drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.054637 coba-7.0.3/coba.egg-info/
--rw-rw-rw-   0        0        0     7942 2023-07-25 03:34:37.000000 coba-7.0.3/coba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1583 2023-07-25 03:34:37.000000 coba-7.0.3/coba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 03:34:37.000000 coba-7.0.3/coba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-25 03:34:37.000000 coba-7.0.3/coba.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2023-07-25 03:34:37.000000 coba-7.0.3/coba.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-25 03:34:37.000000 coba-7.0.3/coba.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1194 2023-07-20 03:21:22.000000 coba-7.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 03:34:38.556975 coba-7.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 22:01:12.529459 coba-7.0.4/
+-rw-rw-rw-   0        0        0       40 2023-06-12 16:34:36.000000 coba-7.0.4/AUTHORS
+-rw-rw-rw-   0        0        0     1593 2023-06-12 16:34:36.000000 coba-7.0.4/LICENSE
+-rw-rw-rw-   0        0        0     7942 2023-08-02 22:01:12.529459 coba-7.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7327 2023-06-16 20:10:41.000000 coba-7.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 22:01:11.479301 coba-7.0.4/coba/
+-rw-rw-rw-   0        0        0     1410 2023-07-31 00:11:40.000000 coba-7.0.4/coba/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:01:11.581123 coba-7.0.4/coba/backports/
+-rw-rw-rw-   0        0        0       50 2023-07-20 03:01:25.000000 coba-7.0.4/coba/backports/__init__.py
+-rw-rw-rw-   0        0        0      262 2023-07-20 02:54:01.000000 coba-7.0.4/coba/backports/metadata.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:01:11.669619 coba-7.0.4/coba/contexts/
+-rw-rw-rw-   0        0        0      703 2023-06-22 17:38:27.000000 coba-7.0.4/coba/contexts/__init__.py
+-rw-rw-rw-   0        0        0     9727 2023-06-12 16:34:36.000000 coba-7.0.4/coba/contexts/cachers.py
+-rw-rw-rw-   0        0        0     9236 2023-07-20 02:56:24.000000 coba-7.0.4/coba/contexts/core.py
+-rw-rw-rw-   0        0        0     9726 2023-06-12 16:34:36.000000 coba-7.0.4/coba/contexts/loggers.py
+-rw-rw-rw-   0        0        0    15875 2023-07-20 03:19:10.000000 coba-7.0.4/coba/encodings.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:01:11.931650 coba-7.0.4/coba/environments/
+-rw-rw-rw-   0        0        0     1448 2023-07-16 19:49:49.000000 coba-7.0.4/coba/environments/__init__.py
+-rw-rw-rw-   0        0        0    22841 2023-07-20 03:16:24.000000 coba-7.0.4/coba/environments/core.py
+-rw-rw-rw-   0        0        0    52650 2023-07-25 01:55:42.000000 coba-7.0.4/coba/environments/filters.py
+-rw-rw-rw-   0        0        0    14347 2023-07-16 19:49:49.000000 coba-7.0.4/coba/environments/openml.py
+-rw-rw-rw-   0        0        0     7646 2023-07-16 19:49:49.000000 coba-7.0.4/coba/environments/primitives.py
+-rw-rw-rw-   0        0        0     2937 2023-07-25 07:10:46.000000 coba-7.0.4/coba/environments/serialized.py
+-rw-rw-rw-   0        0        0     9524 2023-07-20 02:57:00.000000 coba-7.0.4/coba/environments/supervised.py
+-rw-rw-rw-   0        0        0    24174 2023-07-20 02:57:08.000000 coba-7.0.4/coba/environments/synthetics.py
+-rw-rw-rw-   0        0        0     6179 2023-06-12 16:34:36.000000 coba-7.0.4/coba/environments/templates.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:01:11.979445 coba-7.0.4/coba/evaluators/
+-rw-rw-rw-   0        0        0      217 2023-06-24 23:45:33.000000 coba-7.0.4/coba/evaluators/__init__.py
+-rw-rw-rw-   0        0        0    15064 2023-07-29 18:51:58.000000 coba-7.0.4/coba/evaluators/offline.py
+-rw-rw-rw-   0        0        0    22371 2023-07-30 19:52:13.000000 coba-7.0.4/coba/evaluators/online.py
+-rw-rw-rw-   0        0        0     2095 2023-07-16 19:49:49.000000 coba-7.0.4/coba/evaluators/primitives.py
+-rw-rw-rw-   0        0        0     1126 2023-06-12 16:34:36.000000 coba-7.0.4/coba/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:01:12.079515 coba-7.0.4/coba/experiments/
+-rw-rw-rw-   0        0        0      379 2023-06-22 17:38:27.000000 coba-7.0.4/coba/experiments/__init__.py
+-rw-rw-rw-   0        0        0    10512 2023-07-16 19:49:49.000000 coba-7.0.4/coba/experiments/core.py
+-rw-rw-rw-   0        0        0     7686 2023-07-16 19:49:49.000000 coba-7.0.4/coba/experiments/process.py
+-rw-rw-rw-   0        0        0    66159 2023-08-02 21:16:09.000000 coba-7.0.4/coba/experiments/results.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:01:12.253456 coba-7.0.4/coba/learners/
+-rw-rw-rw-   0        0        0      744 2023-07-31 00:11:24.000000 coba-7.0.4/coba/learners/__init__.py
+-rw-rw-rw-   0        0        0     7811 2023-07-30 19:52:14.000000 coba-7.0.4/coba/learners/bandit.py
+-rw-rw-rw-   0        0        0     7989 2023-07-30 19:46:33.000000 coba-7.0.4/coba/learners/corral.py
+-rw-rw-rw-   0        0        0     4924 2023-07-30 19:47:39.000000 coba-7.0.4/coba/learners/linucb.py
+-rw-rw-rw-   0        0        0      940 2023-07-29 17:58:46.000000 coba-7.0.4/coba/learners/misguided.py
+-rw-rw-rw-   0        0        0     4041 2023-07-31 00:09:47.000000 coba-7.0.4/coba/learners/primitives.py
+-rw-rw-rw-   0        0        0    13383 2023-08-01 07:35:39.000000 coba-7.0.4/coba/learners/safety.py
+-rw-rw-rw-   0        0        0    31052 2023-07-30 19:51:33.000000 coba-7.0.4/coba/learners/vowpal.py
+-rw-rw-rw-   0        0        0     4139 2023-07-16 19:49:49.000000 coba-7.0.4/coba/multiprocessing.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:01:12.432170 coba-7.0.4/coba/pipes/
+-rw-rw-rw-   0        0        0     1456 2023-07-16 19:49:49.000000 coba-7.0.4/coba/pipes/__init__.py
+-rw-rw-rw-   0        0        0     1890 2023-06-12 16:34:36.000000 coba-7.0.4/coba/pipes/core.py
+-rw-rw-rw-   0        0        0    16751 2023-07-16 19:49:49.000000 coba-7.0.4/coba/pipes/filters.py
+-rw-rw-rw-   0        0        0    16062 2023-07-20 05:27:58.000000 coba-7.0.4/coba/pipes/multiprocessing.py
+-rw-rw-rw-   0        0        0     6622 2023-06-12 16:34:36.000000 coba-7.0.4/coba/pipes/primitives.py
+-rw-rw-rw-   0        0        0    13003 2023-06-12 16:34:36.000000 coba-7.0.4/coba/pipes/readers.py
+-rw-rw-rw-   0        0        0    19458 2023-07-20 02:58:18.000000 coba-7.0.4/coba/pipes/rows.py
+-rw-rw-rw-   0        0        0     4474 2023-07-16 19:49:49.000000 coba-7.0.4/coba/pipes/sinks.py
+-rw-rw-rw-   0        0        0     6483 2023-07-20 02:58:25.000000 coba-7.0.4/coba/pipes/sources.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:01:12.529459 coba-7.0.4/coba/primitives/
+-rw-rw-rw-   0        0        0      477 2023-06-22 17:38:27.000000 coba-7.0.4/coba/primitives/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-06-16 20:10:41.000000 coba-7.0.4/coba/primitives/feedbacks.py
+-rw-rw-rw-   0        0        0     4624 2023-07-20 08:45:03.000000 coba-7.0.4/coba/primitives/rewards.py
+-rw-rw-rw-   0        0        0     4421 2023-07-16 19:49:49.000000 coba-7.0.4/coba/primitives/rows.py
+-rw-rw-rw-   0        0        0      219 2023-07-19 06:20:25.000000 coba-7.0.4/coba/primitives/semantic.py
+-rw-rw-rw-   0        0        0      657 2023-06-12 16:34:36.000000 coba-7.0.4/coba/primitives/types.py
+-rw-rw-rw-   0        0        0    11151 2023-07-16 18:38:46.000000 coba-7.0.4/coba/random.py
+-rw-rw-rw-   0        0        0     1479 2023-07-16 19:49:49.000000 coba-7.0.4/coba/register.py
+-rw-rw-rw-   0        0        0    10657 2023-06-12 16:34:36.000000 coba-7.0.4/coba/registry.py
+-rw-rw-rw-   0        0        0     9022 2023-07-20 02:56:10.000000 coba-7.0.4/coba/statistics.py
+-rw-rw-rw-   0        0        0     5212 2023-06-12 16:34:36.000000 coba-7.0.4/coba/utilities.py
+drwxrwxrwx   0        0        0        0 2023-08-02 22:01:11.543719 coba-7.0.4/coba.egg-info/
+-rw-rw-rw-   0        0        0     7942 2023-08-02 22:01:11.000000 coba-7.0.4/coba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1583 2023-08-02 22:01:11.000000 coba-7.0.4/coba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 22:01:11.000000 coba-7.0.4/coba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-08-02 22:01:11.000000 coba-7.0.4/coba.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2023-08-02 22:01:11.000000 coba-7.0.4/coba.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-02 22:01:11.000000 coba-7.0.4/coba.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1194 2023-07-20 03:21:22.000000 coba-7.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 22:01:12.529459 coba-7.0.4/setup.cfg
```

### Comparing `coba-7.0.3/LICENSE` & `coba-7.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/PKG-INFO` & `coba-7.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coba
-Version: 7.0.3
+Version: 7.0.4
 Summary: A contextual bandit research package
 Author-email: Mark Rucker <rucker.mark@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/vowpalwabbit/coba
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `coba-7.0.3/README.md` & `coba-7.0.4/README.md`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/__init__.py` & `coba-7.0.4/coba/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from coba.random import CobaRandom
 from coba.contexts import CobaContext, NullLogger
 
 from coba.environments import Environments, ArffSource, CsvSource, LibSvmSource, ManikSource
 from coba.environments import Interaction, SimulatedInteraction, LoggedInteraction, GroundedInteraction, LambdaSimulation
 
-from coba.learners import Learner, ActionProb, PMF
+from coba.learners import Learner
 from coba.learners import SafeLearner, FixedLearner, RandomLearner
 from coba.learners import EpsilonBanditLearner, UcbBanditLearner
 from coba.learners import CorralLearner, LinUCBLearner
 from coba.learners import VowpalLearner, VowpalEpsilonLearner, VowpalSoftmaxLearner, VowpalBagLearner, VowpalRndLearner
 from coba.learners import VowpalCoverLearner, VowpalRegcbLearner, VowpalSquarecbLearner, VowpalOffPolicyLearner
 from coba.learners import MisguidedLearner
 
@@ -22,8 +22,8 @@
 
 from coba.primitives.semantic import Batch
 from coba.primitives.rewards import L1Reward, HammingReward, BinaryReward, IPSReward
 from coba.primitives.rewards import SequenceReward, MappingReward, MulticlassReward, BatchReward
 
 from coba.statistics import BootstrapCI, mean
 
-__version__ = "7.0.3"
+__version__ = "7.0.4"
```

### Comparing `coba-7.0.3/coba/contexts/__init__.py` & `coba-7.0.4/coba/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/contexts/cachers.py` & `coba-7.0.4/coba/contexts/cachers.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/contexts/core.py` & `coba-7.0.4/coba/contexts/core.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/contexts/loggers.py` & `coba-7.0.4/coba/contexts/loggers.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/encodings.py` & `coba-7.0.4/coba/encodings.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/environments/__init__.py` & `coba-7.0.4/coba/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/environments/core.py` & `coba-7.0.4/coba/environments/core.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/environments/filters.py` & `coba-7.0.4/coba/environments/filters.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/environments/openml.py` & `coba-7.0.4/coba/environments/openml.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/environments/primitives.py` & `coba-7.0.4/coba/environments/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/environments/serialized.py` & `coba-7.0.4/coba/environments/serialized.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pickle
 
 from pathlib import Path
-from collections import abc
 from zipfile import ZipFile, ZIP_DEFLATED
 from itertools import islice, repeat, chain
 from typing import Union, Sequence, Mapping, Iterable, Any
 
 from coba.contexts import CobaContext
 from coba.pipes import Source, Sink, Filter
 from coba.environments.primitives import Environment, Interaction
```

### Comparing `coba-7.0.3/coba/environments/supervised.py` & `coba-7.0.4/coba/environments/supervised.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/environments/synthetics.py` & `coba-7.0.4/coba/environments/synthetics.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/environments/templates.py` & `coba-7.0.4/coba/environments/templates.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/evaluators/offline.py` & `coba-7.0.4/coba/evaluators/offline.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/evaluators/online.py` & `coba-7.0.4/coba/evaluators/online.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             action,prob,kwargs = predict(context, actions)
             predict_time       = time.time()-start_time
 
             reward   = rewards.eval(action)
             feedback = feedbacks.eval(action) if feedbacks else None
 
             start_time = time.time()
-            if self._learn: learn(context, actions, action, feedback if feedbacks else reward, prob, **kwargs)
+            if self._learn: learn(context, action, feedback if feedbacks else reward, prob, **kwargs)
             learn_time = time.time() - start_time
 
             if record_time    : out['predict_time'] = predict_time
             if record_time    : out['learn_time']   = learn_time
             if record_prob    : out['probability']  = prob
             if record_action  : out['action']       = action
             if feedbacks      : out['feedback']     = feedback
@@ -255,15 +255,15 @@
                     #in theory we could use a ratio average in this case
                     #this would give us a lower variance estimate but we'd have
                     #to add a "weight" column to our output and handle this in Result
                     ope_reward = log_rewards.eval(on_action)
 
             if self._learn:
                 start_time = time.time()
-                if self._learn: learn(log_context, log_actions, log_action, log_reward, log_prob)
+                if self._learn: learn(log_context, log_action, log_reward, log_prob)
                 learn_time = time.time() - start_time
 
             if record_time  :  out['predict_time'] = predict_time
             if record_time  :  out['learn_time']   = learn_time
             if record_reward:  out['reward']       = ope_reward
             if record_action:  out['action']       = log_action
             if record_prob:    out['probability']  = log_prob
@@ -421,15 +421,15 @@
                 out = {}
                 if ope_rewards:
                     ope_rewards[-1] = log_reward
                 else:
                     ope_rewards.append(log_reward)
 
                 start_time = time.time()
-                learn(log_context, log_actions, log_action, log_reward, on_prob)
+                learn(log_context, log_action, log_reward, on_prob)
                 learn_time = time.time() - start_time
 
                 if record_time    : out['predict_time'] = predict_time
                 if record_time    : out['learn_time']   = learn_time
                 if record_context : out['context']      = log_context
                 if record_actions : out['actions']      = log_actions
                 if record_action  : out['action']       = log_action
```

### Comparing `coba-7.0.3/coba/evaluators/primitives.py` & `coba-7.0.4/coba/evaluators/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/exceptions.py` & `coba-7.0.4/coba/exceptions.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/experiments/core.py` & `coba-7.0.4/coba/experiments/core.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/experiments/process.py` & `coba-7.0.4/coba/experiments/process.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/experiments/results.py` & `coba-7.0.4/coba/experiments/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -641,15 +641,15 @@
                 ax.autoscale(axis='y')
 
             ax.set_xlim(*xlim)
             ax.set_ylim(*ylim)
 
             ax.autoscale(axis='both')
 
-            ax.set_title(title, loc='left', pad=15)
+            ax.set_title(title, loc='left')
             ax.set_ylabel(ylabel)
             ax.set_xlabel(xlabel)
 
             if ax.get_legend() is None: #pragma: no cover
                 scale = 0.65
                 box1 = ax.get_position()
                 ax.set_position([box1.x0, box1.y0 + box1.height * (1-scale), box1.width, box1.height * scale])
@@ -998,14 +998,17 @@
         l       : Union[str, Sequence[str]] = 'full_name',
         p       : Union[str, Sequence[str]] = 'environment_id',
         span    : int = None,
         err     : Union[Literal['se','sd','bs','bi'], None, PointAndInterval] = None,
         errevery: int = None,
         labels  : Sequence[str] = None,
         colors  : Union[int,Sequence[Union[str,int]]] = None,
+        title   : str = None,
+        xlabel  : str = None,
+        ylabel  : str = None,
         xlim    : Tuple[Optional[Number],Optional[Number]] = None,
         ylim    : Tuple[Optional[Number],Optional[Number]] = None,
         xticks  : bool = True,
         yticks  : bool = True,
         top_n   : int = None,
         out     : Union[None,Literal['screen'],str] = 'screen',
         ax = None) -> None:
@@ -1022,14 +1025,17 @@
                 values up to current is shown otherwise a moving average with window size of span (the window will be
                 smaller than span initially).
             err: This determines what kind of error bars to plot (if any). If `None` then no bars are plotted, if 'se'
                 the standard error is shown, and if 'sd' the standard deviation is shown.
             errevery: This determines the frequency of errorbars. If `None` they appear 5% of the time.
             labels: The legend labels to use in the plot. These should be in order of the actual legend labels.
             colors: The colors used to plot the learners plot.
+            title : The title give the plot.
+            xlabel: The label on the x-axis.
+            ylabel: The label on the y-axis.
             xlim: Define the x-axis limits to plot. If `None` the x-axis limits will be inferred.
             ylim: Define the y-axis limits to plot. If `None` the y-axis limits will be inferred.
             xticks: Whether the x-axis labels should be drawn.
             yticks: Whether the y-axis labels should be drawn.
             top_n: Only plot the top_n learners. If `None` all learners will be plotted. If negative the bottom will be plotted.
             out: Indicate where the plot should be sent to after plotting is finished.
             ax: Provide an optional axes that the plot will be drawn to. If not provided a new figure/axes is created.
@@ -1059,21 +1065,21 @@
                 for _xi, (_x, group) in enumerate(groupby(group, key=itemgetter(0))):
                     Y = [g[-1] for g in group]
                     lines[-1].add(x_prep(_x), *err(Y, _xi))
 
             lines  = sorted(lines, key=lambda line: line.Y[-1], reverse=True)
             labels = [l.label or str(l.label) for l in lines]
             colors = [l.color                 for l in lines]
-            xlabel = "Interaction" if x=='index' else x[0] if len(x) == 1 else x
-            ylabel = y.capitalize().replace("_pct"," Percent")
+            xlabel = xlabel or ("Interaction" if x=='index' else x[0] if len(x) == 1 else x)
+            ylabel = ylabel or (y.capitalize().replace("_pct"," Percent"))
 
             y_location = "Total" if x != 'index' else ""
             y_avg_type = ("Instant" if span == 1 else f"Span {span}" if span else "Progressive")
             y_samples  = f"({len(Y)} Environments)"
-            title      = ' '.join(filter(None,[y_location, y_avg_type, ylabel, y_samples]))
+            title      = title if title is not None else (' '.join(filter(None,[y_location, y_avg_type, ylabel, y_samples])))
 
             xrotation = 90 if x != 'index' and len(lines[0].X)>5 else 0
             yrotation = 0
 
             if top_n:
                 if abs(top_n) > len(lines): top_n = len(lines)*abs(top_n)/top_n
                 if top_n > 0: lines = [replace(l,color=plottable._get_color(colors,i),label=plottable._get_label(labels,l.label,i)) for i,l in enumerate(lines[:top_n],0    ) ]
@@ -1093,14 +1099,17 @@
         p       : Union[str, Sequence[str]] = 'environment_id',
         mode    : Union[Literal["diff","prob"], Callable[[float,float],float]] = "diff",
         span    : int = None,
         err     : Union[Literal['se','sd','bs','bi'], None, PointAndInterval] = None,
         errevery: int = None,
         labels  : Sequence[str] = None,
         colors  : Sequence[str] = None,
+        title   : str = None,
+        xlabel  : str = None,
+        ylabel  : str = None,
         xlim    : Tuple[Optional[Number],Optional[Number]] = None,
         ylim    : Tuple[Optional[Number],Optional[Number]] = None,
         xticks  : bool = True,
         yticks  : bool = True,
         boundary: bool = True,
         legend  : bool = True,
         out     : Union[None,Literal['screen'],str] = 'screen',
@@ -1119,15 +1128,18 @@
             span: The number of y values to smooth together when reporting y. If this is None then the average of all y
                 values up to current is shown otherwise a moving average with window size of span (the window will be
                 smaller than span initially).
             err: This determines what kind of error bars to plot (if any). If `None` then no bars are plotted, if 'se'
                 the standard error is shown, and if 'sd' the standard deviation is shown.
             errevery: This determines the frequency of errorbars. If `None` they appear 5% of the time.
             labels: The legend labels to use in the plot. These should be in order of the actual legend labels.
+            title : The title give the plot.
             colors: The colors used to plot the learners plot.
+            xlabel: The label on the x-axis.
+            ylabel: The label on the y-axis.
             xlim: Define the x-axis limits to plot. If `None` the x-axis limits will be inferred.
             ylim: Define the y-axis limits to plot. If `None` the y-axis limits will be inferred.
             xticks: Whether the x-axis labels should be drawn.
             yticks: Whether the y-axis labels should be drawn.
             boundary: Whether we want to plot the boundary line between which set is the best performing.
             out: Indicate where the plot should be sent to after plotting is finished.
             ax: Provide an optional axes that the plot will be drawn to. If not provided a new figure/axes is created.
@@ -1260,17 +1272,17 @@
                 leftmost_x  = lines[0 ].X[0 ]
                 rightmost_x = lines[-1].X[-1]
                 lines.append(Points((leftmost_x,rightmost_x),(_boundary,_boundary), None, None , "#888", 1, None, '-',.5))
 
             xrotation = 90 if x != 'index' and len(X_Y_YE)>5 else 0
             yrotation = 0
 
-            xlabel = "Interaction" if x=='index' else x[0] if len(x) == 1 else x
-            ylabel = f"$\Delta$ {y}" if mode=="diff" else f"P($\Delta$ {y} > 0)"
-            title  = f"{ylabel} ({len(_Y)} Environments)"
+            xlabel = xlabel or ("Interaction" if x=='index' else x[0] if len(x) == 1 else x)
+            ylabel = ylabel or (f"$\Delta$ {y}" if mode=="diff" else f"P($\Delta$ {y} > 0)")
+            title  = title if title is not None else (f"{ylabel} ({len(_Y)} Environments)")
 
             self._plotter.plot(ax, lines, title, xlabel, ylabel, xlim, ylim, xticks, yticks, xrotation, yrotation, out)
 
         except CobaException as e:
             CobaContext.logger.log(str(e))
 
     def __str__(self) -> str:
```

### Comparing `coba-7.0.3/coba/learners/__init__.py` & `coba-7.0.4/coba/learners/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """This module contains all public learners and learner interfaces."""
 
-from coba.learners.primitives import Learner, PMF, ActionProb
+from coba.learners.primitives import Learner
 from coba.learners.safety     import SafeLearner
 from coba.learners.bandit     import EpsilonBanditLearner, UcbBanditLearner, FixedLearner, RandomLearner
 from coba.learners.corral     import CorralLearner
 from coba.learners.vowpal     import VowpalMediator
 from coba.learners.vowpal     import VowpalLearner, VowpalEpsilonLearner, VowpalSoftmaxLearner, VowpalBagLearner, VowpalRndLearner
 from coba.learners.vowpal     import VowpalCoverLearner, VowpalRegcbLearner, VowpalSquarecbLearner, VowpalOffPolicyLearner
 from coba.learners.linucb     import LinUCBLearner
```

### Comparing `coba-7.0.3/coba/learners/bandit.py` & `coba-7.0.4/coba/learners/bandit.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         values      = [ self._Q[action] for action in actions ]
         max_value   = None if set(values) == {None} else max(v for v in values if v is not None)
         max_indexes = [i for i in range(len(values)) if values[i]==max_value]
 
         prob_selected_randomly = [1/len(actions) * self._epsilon] * len(actions)
         prob_selected_greedily = [ int(i in max_indexes)/len(max_indexes) * (1-self._epsilon) for i in range(len(actions))]
 
-        return PMF([p1+p2 for p1,p2 in zip(prob_selected_randomly,prob_selected_greedily)])
+        return [p1+p2 for p1,p2 in zip(prob_selected_randomly,prob_selected_greedily)]
 
-    def learn(self, context: Context, actions: Actions, action: Action, reward: float, prob: float) -> None:
+    def learn(self, context: Context, action: Action, reward: float, probability: float) -> None:
 
         alpha = 1/(self._N[action]+1)
         old_Q = self._Q[action] or 0.0
 
         self._Q[action] = (1-alpha) * old_Q + alpha * reward
         self._N[action] = self._N[action] + 1
 
@@ -73,15 +73,14 @@
         self._t     : int = 0
         self._m     : Mapping[Action, float         ] = {}
         self._s     : Mapping[Action, int           ] = {}
         self._v     : Mapping[Action, OnlineVariance] = {}
 
     @property
     def params(self) -> Mapping[str, Any]:
-
         return { "family": "UCB_bandit" }
 
     def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
         never_observed_actions = set(actions) - self._m.keys()
 
         if never_observed_actions:
             max_actions = never_observed_actions
@@ -99,18 +98,18 @@
         if never_observed_actions:
             max_actions = never_observed_actions
         else:
             values      = [ self._m[a] + self._Avg_R_UCB(a) for a in actions ]
             max_value   = max(values)
             max_actions = [ a for a,v in zip(actions,values) if v==max_value ]
 
-        return PMF([int(action in max_actions)/len(max_actions) for action in actions])
+        return [int(action in max_actions)/len(max_actions) for action in actions]
+
+    def learn(self, context: Context, action: Action, reward: float, probability: float) -> None:
 
-    def learn(self, context: Context, actions: Actions, action: Action, reward: float, prob: float) -> None:
-        
         self._t += 1
 
         assert 0 <= reward and reward <= 1, "This algorithm assumes that reward has support in [0,1]."
 
         if action not in self._m:
             self._m[action] = reward
             self._s[action] = 1
@@ -166,37 +165,37 @@
         assert round(sum(pmf),3) == 1, "The given pmf must sum to one to be a valid pmf."
         assert all([p >= 0 for p in pmf]), "All given probabilities of the pmf must be greater than or equal to 0."
         self._pmf = pmf
 
     @property
     def params(self) -> Mapping[str, Any]:
         return {"family":"fixed"}
-    
+
     def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
         probs = self._pmf
         return [ probs[actions.index(a)] for a in request ]
 
     def predict(self, context: Context, actions: Actions) -> PMF:
-        return PMF(self._pmf)
+        return self._pmf
 
-    def learn(self, context: Context, actions: Actions, action: Action, reward: float, prob: float) -> None:
+    def learn(self, context: Context, action: Action, reward: float, prob: float) -> None:
         pass
 
 class RandomLearner(Learner):
     """A learner that selects actions according to a uniform distribution."""
 
     def __init__(self):
         """Instantiate a RandomLearner."""
         pass
 
     @property
     def params(self) -> Mapping[str, Any]:
         return {"family":"random"}
-    
+
     def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
         return [1/len(actions)]*len(request)
 
     def predict(self, context: Context, actions: Actions) -> PMF:
-        return PMF([1/len(actions)]*len(actions))
+        return [1/len(actions)]*len(actions)
 
-    def learn(self, context: Context, actions: Actions, action: Action, reward: float, probability: float) -> None:
+    def learn(self, context: Context, action: Action, reward: float, probability: float) -> None:
         pass
```

### Comparing `coba-7.0.3/coba/learners/corral.py` & `coba-7.0.4/coba/learners/corral.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,44 +72,45 @@
         return [ probs[actions.index(a)] for a in request ]
 
     def predict(self, context: Context, actions: Sequence[Action]) -> Tuple[PMF,kwargs]:
 
         base_predicts = [ base_algorithm.predict(context, actions) for base_algorithm in self._base_learners ]
         base_actions, base_probs, base_infos = zip(*base_predicts)
 
-        predict = [ sum([p_b*int(a==b_a) for p_b,b_a in zip(self._p_bars, base_actions)]) for a in actions ]
-        info    = (base_actions, base_probs, base_infos)
+        pmf  = [ sum([p_b*int(a==b_a) for p_b,b_a in zip(self._p_bars, base_actions)]) for a in actions ]
+        info = (actions, base_actions, base_probs, base_infos)
 
-        return (predict, {'info':info})
+        return pmf, {'info':info}
 
-    def learn(self, context: Context, actions: Actions, action: Action, reward: float, probability:float, **kwargs) -> None:
+    def learn(self, context: Context, action: Action, reward: float, probability:float, info) -> None:
 
         assert  0 <= reward and reward <= 1, "This Corral implementation assumes a loss between 0 and 1"
 
-        base_actions = kwargs['info'][0]
-        base_probs   = kwargs['info'][1]
-        base_infos   = kwargs['info'][2]
+        actions      = info[0]
+        base_actions = info[1]
+        base_probs   = info[2]
+        base_infos   = info[3]
 
         if self._mode == "importance":
             # This is what is in the original paper. It has the following characteristics:
             #   > It is able to provide feedback to every base learner on every iteration
             #   > It uses a reward estimator with higher variance and no bias (aka, importance sampling)
             #   > It is "on-policy" with respect to base learner's prediction distributions
             # The reward, R, supplied to the base learners satisifies E[R|context,A] = E[reward|context,A]
             for learner, A, P, base_info in zip(self._base_learners, base_actions, base_probs, base_infos):
                 R = reward * int(A==action)/probability
-                learner.learn(context, actions, A, R, P, **base_info)
+                learner.learn(context, A, R, P, **base_info)
 
         if self._mode == "off-policy":
             # An alternative variation to the paper is provided below. It has the following characterisitcs:
             #   > It is able to provide feedback to every base learner on every iteration
             #   > It uses a MVUB reward estimator (aka, the unmodified, observed reward)
             #   > It is "off-policy" (i.e., base learners receive action feedback distributed differently from their predicts).
             for learner, base_info in zip(self._base_learners, base_infos):
-                learner.learn(context, actions, action, reward, probability, **base_info)
+                learner.learn(context, action, reward, probability, **base_info)
 
         loss = 1-reward
 
         instant_loss = [ loss/probability * (base_action==action) for base_action in base_actions ]
         self._ps     = CorralLearner._log_barrier_omd(self._ps, instant_loss, self._etas)
         self._p_bars = [ (1-self._gamma)*p + self._gamma*1/len(self._base_learners) for p in self._ps ]
 
@@ -173,8 +174,8 @@
         if lmbda is None:
             raise Exception(f'Something went wrong in Corral OMD {ps}, {etas}, {losses}')
 
         new_ps = [ 1/((1/p) + eta*(loss-lmbda)) for p, eta, loss in zip(ps, etas, losses)]
 
         assert round(sum(new_ps),precision) == 1, "An invalid update was made by the log barrier in Corral"
 
-        return new_ps
+        return new_ps
```

### Comparing `coba-7.0.3/coba/learners/linucb.py` & `coba-7.0.4/coba/learners/linucb.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,17 +77,17 @@
 
         point_estimate = self._theta @ features
         point_bounds   = np.diagonal(features.T @ self._A_inv @ features)
 
         action_values = point_estimate + self._alpha*np.sqrt(point_bounds)
         max_indexes   = np.where(action_values == np.amax(action_values))[0]
 
-        return PMF([int(ind in max_indexes)/len(max_indexes) for ind in range(len(actions))])
+        return [int(ind in max_indexes)/len(max_indexes) for ind in range(len(actions))]
 
-    def learn(self, context: Context, actions: Actions, action: Action, reward: float, probability: float) -> None:
+    def learn(self, context: Context, action: Action, reward: float, probability: float) -> None:
         import numpy as np
 
         if isinstance(action, dict) or isinstance(context, dict):
             raise CobaException("Sparse data cannot be handled by this algorithm.")
 
         if not context:
             self._X_encoder = InteractionsEncoder(list(set(filter(None,[ f.replace('x','') if isinstance(f,str) else f for f in self._X ]))))
```

### Comparing `coba-7.0.3/coba/learners/misguided.py` & `coba-7.0.4/coba/learners/misguided.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 
     def request(self, context, actions, request):
         return self._learner.request(context, actions, request)
 
     def predict(self, context, actions):
         return self._learner.predict(context, actions)
 
-    def learn(self, context, actions, action, reward, probability):
-        self._learner.learn(context, actions, action, self._shifter + self._scaler*reward, probability)
+    def learn(self, context, action, reward, probability):
+        self._learner.learn(context, action, self._shifter + self._scaler*reward, probability)
```

### Comparing `coba-7.0.3/coba/learners/primitives.py` & `coba-7.0.4/coba/learners/primitives.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 
-from abc import ABC, abstractmethod
 from typing import Any, Sequence, Union, Tuple, Callable, Mapping, Type
 
 from coba.exceptions import CobaException
 from coba.primitives import Context, Action, Actions
 from coba.primitives import Dense, Sparse, HashableDense, HashableSparse
 
 kwargs = Mapping[str,Any]
 Prob   = float
 PDF    = Callable[[Action],float]
-
-class PMF(list):
-    pass
-
-class ActionProb(tuple):
-    def __new__(self, action: Action, prob: Prob):
-        return tuple.__new__(ActionProb, (action, prob))
+PMF    = Sequence[float]
 
 Prediction = Union[
     PMF,
-    ActionProb,
+    Action,
+    Tuple[Action,Prob],
     Tuple[PMF        , kwargs],
-    Tuple[ActionProb , kwargs],
+    Tuple[Action     , kwargs],
     Tuple[Action,Prob, kwargs],
 ]
 
 class Learner:
     """The Learner interface for contextual bandit learning."""
 
     @property
@@ -70,30 +64,23 @@
         Returns:
             A Prediction. Several prediction formats are supported. See the type-hint for these.
         """
         raise CobaException((
             "The `predict` interface has not been implemented for this learner."
         ))
 
-    def learn(self,
-        context: Context,
-        actions: Actions,
-        action: Action,
-        reward: Union[float,Any],
-        probability: float,
-        **kwargs) -> None:
+    def learn(self, context: Context, action: Action, reward: float, probability: float, **kwargs) -> None:
         """Learn about the action taken in the context.
 
         Args:
             context: The context in which the action was taken.
-            actions: The set of actions that were available.
             action: The action that was taken.
-            reward: The reward for contextual bandit problems and feedback for IGL problems.
+            reward: The reward for the given context and action (feedback for IGL problems).
             probability: The probability the given action was taken.
-            **kwargs: Optional information returned with the prediction.
+            **kwargs: Optional information returned during prediction.
         """
         raise CobaException((
             "The `learn` interface has not been implemented for this learner."
         ))
 
 def requires_hashables(cls:Type[Learner]):
 
@@ -104,14 +91,14 @@
 
     old_predict = cls.predict
     old_learn   = cls.learn
 
     def new_predict(self,c,A):
         return old_predict(self,make_hashable(c),list(map(make_hashable,A)))
 
-    def new_learn(self,c,A,a,r,p,**kwargs):
-        old_learn(self,make_hashable(c),list(map(make_hashable,A)), make_hashable(a),r,p,**kwargs)
+    def new_learn(self,c,a,r,p,**kwargs):
+        old_learn(self,make_hashable(c),make_hashable(a),r,p,**kwargs)
 
     cls.predict = new_predict
     cls.learn   = new_learn
 
     return cls
```

### Comparing `coba-7.0.3/coba/learners/vowpal.py` & `coba-7.0.4/coba/learners/vowpal.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """A class to handle all communication between Coba and VW."""
 
     def __init__(self) -> None:
         self._vw = None
         self._args = ""
         self._ns_keys = {}
         self._ns_keys_cnt = 0
- 
+
         PackageChecker.vowpalwabbit('VowpalMediator.__init__')
 
     @property
     def is_initialized(self) -> bool:
         """Indicate whether init_learner has been called previously."""
         return self._vw is not None
 
@@ -94,26 +94,26 @@
         ex.setup_example()
 
         return ex
 
     def finish(self):
         if self.is_initialized:
             self._vw.finish()
-    
+
     # override to transform example before they get pushed down to VW
     # i.e. change namespaces from the default 'x' in shared to any other namespace
     def transform_example(self, vw_shared, vw_uniques, labels):
         pass
 
     def make_examples(self, shared: Namespaces, uniques: Sequence[Namespaces], labels:Optional[Sequence[str]] = None) -> Sequence[Any]:
         """Create a list of VW examples.
 
         Args:
             shared: The features grouped by namespace in this example.
-            separates: The features, grouped by namespace, unique to each each example. 
+            separates: The features, grouped by namespace, unique to each each example.
             label: An optional label (required if this example will be used for learning).
         """
 
         labels     = repeat(None) if labels is None else labels
         vw_shared  = dict(self._prep_namespaces(shared))
         vw_uniques = list(map(dict,map(self._prep_namespaces,uniques)))
 
@@ -270,25 +270,25 @@
 
         self._n_actions = None
         self._actions   = None
 
         if not self._adf:
             n_action_str = re.match("--cb.*?\s*(\d*)\\b.*", args).group(1)
             self._n_actions = int(n_action_str) if n_action_str else None
-            #useful for removing the n_actions from args 
+            #useful for removing the n_actions from args
             #re.sub("(--cb)\s*(\d+)", '\g<1>', "--cb 123", count=1)
 
         self._vw = vw or VowpalMediator()
 
     @property
     def params(self) -> Mapping[str, Any]:
         return {"family": "vw", 'args': self._args.replace("--quiet","").strip()}
 
     def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
-        probs = self.predict(context,actions)
+        probs = self.predict(context,actions)[0]
         return probs if actions == request else list(map(probs.__getitem__,map(actions.index,request)))
 
     def predict(self, context: Context, actions: Sequence[Action]) -> PMF:
 
         if not self._vw.is_initialized and isinstance(context,Batch):#pragma: no cover
             raise CobaException("VW learner does not support batched calls.")
 
@@ -332,27 +332,29 @@
             probs = self._vw.predict(self._vw.make_example(context, None))
             if probs is None: probs = [1/len(actions)] * len(actions)
 
         if not self._adf and not self._explore:
             index = self._vw.predict(self._vw.make_example(context, None))
             probs = [ int(i==index) for i in range(1,len(actions)+1) ]
 
-        return PMF(probs)
+        return probs, {'actions':actions}
 
-    def learn(self, context: Context, actions:Actions, action: Action, reward: float, probability: float) -> None:
+    def learn(self, context: Context, action: Action, reward: float, probability: float, actions: Actions = None) -> None:
 
         if not self._vw.is_initialized and self._adf:
             self._vw.init_learner(self._args, 4)
 
         if not self._vw.is_initialized and not self._adf and self._n_actions:
             self._vw.init_learner(self._args, 4)
 
         if not self._vw.is_initialized and not self._adf and not self._n_actions:
             raise CobaException("When using `cb` without `adf` predict must be called before learn to initialize the vw learner")
 
+        if actions is None: actions = [action]
+
         index   = actions.index(action)
         labels  = self._labels(actions, index, reward, probability)
         label   = labels[index]
 
         context = {'x':context}
         adfs    = None if not self._adf else [{'a':action} for action in actions]
 
@@ -644,16 +646,16 @@
         vw_args_string = " ".join(self.make_args(namespace_interactions=features, vw_kwargs=vw_kwargs))
         super().__init__(vw_args_string, vw)
 
 class VowpalOffPolicyLearner(VowpalLearner):
     """A wrapper around VowpalLearner that provides more documentation. For more
         information on the types of exploration algorithms availabe in VW see `here`__.
 
-        This wrapper performs policy learning without any exploration. This is only correct 
-        when training examples come from a logging policy so that any exploration on our 
+        This wrapper performs policy learning without any exploration. This is only correct
+        when training examples come from a logging policy so that any exploration on our
         part would be irrelevant.
 
         __ https://github.com/VowpalWabbit/vowpal_wabbit/wiki/Contextual-Bandit-algorithms
     """
 
     def __init__(self,
                  features: Sequence[str] = DEFAULT_NAMESPACE_INTERACTIONS,
```

### Comparing `coba-7.0.3/coba/multiprocessing.py` & `coba-7.0.4/coba/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/pipes/__init__.py` & `coba-7.0.4/coba/pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/pipes/core.py` & `coba-7.0.4/coba/pipes/core.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/pipes/filters.py` & `coba-7.0.4/coba/pipes/filters.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/pipes/multiprocessing.py` & `coba-7.0.4/coba/pipes/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/pipes/primitives.py` & `coba-7.0.4/coba/pipes/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/pipes/readers.py` & `coba-7.0.4/coba/pipes/readers.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/pipes/rows.py` & `coba-7.0.4/coba/pipes/rows.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/pipes/sinks.py` & `coba-7.0.4/coba/pipes/sinks.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/pipes/sources.py` & `coba-7.0.4/coba/pipes/sources.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/primitives/feedbacks.py` & `coba-7.0.4/coba/primitives/feedbacks.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/primitives/rewards.py` & `coba-7.0.4/coba/primitives/rewards.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/primitives/rows.py` & `coba-7.0.4/coba/primitives/rows.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/primitives/types.py` & `coba-7.0.4/coba/primitives/types.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/random.py` & `coba-7.0.4/coba/random.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/register.py` & `coba-7.0.4/coba/register.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/registry.py` & `coba-7.0.4/coba/registry.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/statistics.py` & `coba-7.0.4/coba/statistics.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba/utilities.py` & `coba-7.0.4/coba/utilities.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/coba.egg-info/PKG-INFO` & `coba-7.0.4/coba.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coba
-Version: 7.0.3
+Version: 7.0.4
 Summary: A contextual bandit research package
 Author-email: Mark Rucker <rucker.mark@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/vowpalwabbit/coba
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `coba-7.0.3/coba.egg-info/SOURCES.txt` & `coba-7.0.4/coba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coba-7.0.3/pyproject.toml` & `coba-7.0.4/pyproject.toml`

 * *Files identical despite different names*

