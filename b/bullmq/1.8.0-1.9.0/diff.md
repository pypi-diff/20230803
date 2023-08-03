# Comparing `tmp/bullmq-1.8.0.tar.gz` & `tmp/bullmq-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-1.8.0.tar", last modified: Mon Jul 17 20:35:26 2023, max compression
+gzip compressed data, was "bullmq-1.9.0.tar", last modified: Tue Jul 18 15:17:30 2023, max compression
```

## Comparing `bullmq-1.8.0.tar` & `bullmq-1.9.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:35:26.152906 bullmq-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-17 20:35:26.152906 bullmq-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-17 20:34:17.000000 bullmq-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:35:26.148906 bullmq-1.8.0/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-17 20:35:23.000000 bullmq-1.8.0/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:35:26.152906 bullmq-1.8.0/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/addJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/changePriority-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/getState-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/getStateV2-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/moveToActive-10.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/moveToFinished-13.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/pause-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/promote-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/retryJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/updateProgress-2.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:35:26.152906 bullmq-1.8.0/bullmq/custom_errors/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/custom_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/custom_errors/waiting_children_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19424 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:35:26.152906 bullmq-1.8.0/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:35:26.148906 bullmq-1.8.0/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-17 20:35:26.000000 bullmq-1.8.0/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-17 20:35:26.000000 bullmq-1.8.0/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:35:26.000000 bullmq-1.8.0/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-17 20:35:26.000000 bullmq-1.8.0/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 20:35:26.000000 bullmq-1.8.0/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-17 20:35:23.000000 bullmq-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:35:26.152906 bullmq-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 20:34:17.000000 bullmq-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:17:30.446634 bullmq-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-18 15:17:30.446634 bullmq-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-18 15:15:28.000000 bullmq-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:17:30.434634 bullmq-1.9.0/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-18 15:17:27.000000 bullmq-1.9.0/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:17:30.446634 bullmq-1.9.0/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/addJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/changePriority-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/getState-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/getStateV2-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/moveToActive-10.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/moveToFinished-13.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/pause-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/promote-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/retryJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-18 15:16:54.000000 bullmq-1.9.0/bullmq/commands/updateProgress-2.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:17:30.446634 bullmq-1.9.0/bullmq/custom_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/custom_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/custom_errors/waiting_children_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:17:30.446634 bullmq-1.9.0/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-18 15:15:28.000000 bullmq-1.9.0/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:17:30.438634 bullmq-1.9.0/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-18 15:17:30.000000 bullmq-1.9.0/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-18 15:17:30.000000 bullmq-1.9.0/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:17:30.000000 bullmq-1.9.0/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-18 15:17:30.000000 bullmq-1.9.0/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 15:17:30.000000 bullmq-1.9.0/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-18 15:17:27.000000 bullmq-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:17:30.446634 bullmq-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-18 15:15:28.000000 bullmq-1.9.0/setup.py
```

### Comparing `bullmq-1.8.0/PKG-INFO` & `bullmq-1.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.8.0
+Version: 1.9.0
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-1.8.0/README.md` & `bullmq-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/backoffs.py` & `bullmq-1.9.0/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/addJob-9.lua` & `bullmq-1.9.0/bullmq/commands/addJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/changeDelay-3.lua` & `bullmq-1.9.0/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/changePriority-5.lua` & `bullmq-1.9.0/bullmq/commands/changePriority-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-1.9.0/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/drain-4.lua` & `bullmq-1.9.0/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/getCounts-1.lua` & `bullmq-1.9.0/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/getRanges-1.lua` & `bullmq-1.9.0/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/getState-8.lua` & `bullmq-1.9.0/bullmq/commands/getState-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/getStateV2-8.lua` & `bullmq-1.9.0/bullmq/commands/getStateV2-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/isFinished-3.lua` & `bullmq-1.9.0/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/moveJobFromActiveToWait-9.lua` & `bullmq-1.9.0/bullmq/commands/moveJobFromActiveToWait-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-1.9.0/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/moveToActive-10.lua` & `bullmq-1.9.0/bullmq/commands/moveToActive-10.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/moveToDelayed-8.lua` & `bullmq-1.9.0/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/moveToFinished-13.lua` & `bullmq-1.9.0/bullmq/commands/moveToFinished-13.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-1.9.0/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/obliterate-2.lua` & `bullmq-1.9.0/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/pause-5.lua` & `bullmq-1.9.0/bullmq/commands/pause-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/promote-7.lua` & `bullmq-1.9.0/bullmq/commands/promote-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/removeJob-1.lua` & `bullmq-1.9.0/bullmq/commands/removeJob-1.lua`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 --[[
     Remove a job from all the queues it may be in as well as all its data.
     In order to be able to remove a job, it cannot be active.
     Input:
       KEYS[1] queue prefix
       ARGV[1] jobId
+      ARGV[2] remove children
     Events:
       'removed'
 ]]
 local rcall = redis.call
 -- Includes
 --[[
   Functions to destructure job key.
@@ -21,29 +22,31 @@
 end
 --[[
   Function to recursively check if there are no locks
   on the jobs to be removed.
   returns:
     boolean
 ]]
-local function isLocked( prefix, jobId)
+local function isLocked( prefix, jobId, removeChildren)
   local jobKey = prefix .. jobId;
   -- Check if this job is locked
   local lockKey = jobKey .. ':lock'
   local lock = rcall("GET", lockKey)
   if not lock then
-    local dependencies = rcall("SMEMBERS", jobKey .. ":dependencies")
-    if (#dependencies > 0) then
-      for i, childJobKey in ipairs(dependencies) do
-        -- We need to get the jobId for this job.
-        local childJobId = getJobIdFromKey(childJobKey)
-        local childJobPrefix = getJobKeyPrefix(childJobKey, childJobId)
-        local result = isLocked( childJobPrefix, childJobId )
-        if result then
-          return true
+    if removeChildren == "1" then
+      local dependencies = rcall("SMEMBERS", jobKey .. ":dependencies")
+      if (#dependencies > 0) then
+        for i, childJobKey in ipairs(dependencies) do
+          -- We need to get the jobId for this job.
+          local childJobId = getJobIdFromKey(childJobKey)
+          local childJobPrefix = getJobKeyPrefix(childJobKey, childJobId)
+          local result = isLocked( childJobPrefix, childJobId, removeChildren )
+          if result then
+            return true
+          end
         end
       end
     end
     return false
   end
   return true
 end
@@ -153,48 +156,50 @@
             end
           end
         end
       end
     end
   end
 end
-local function removeJob( prefix, jobId, parentKey)
+local function removeJob( prefix, jobId, parentKey, removeChildren)
     local jobKey = prefix .. jobId;
     removeParentDependencyKey(jobKey, false, parentKey)
-    -- Check if this job has children
-    -- If so, we are going to try to remove the children recursively in deep first way because
-    -- if some job is locked we must exit with and error.
-    --local countProcessed = rcall("HLEN", jobKey .. ":processed")
-    local processed = rcall("HGETALL", jobKey .. ":processed")
-    if (#processed > 0) then
-        for i = 1, #processed, 2 do
-            local childJobId = getJobIdFromKey(processed[i])
-            local childJobPrefix = getJobKeyPrefix(processed[i], childJobId)
-            removeJob( childJobPrefix, childJobId, jobKey )
+    if removeChildren == "1" then
+        -- Check if this job has children
+        -- If so, we are going to try to remove the children recursively in deep first way because
+        -- if some job is locked we must exit with and error.
+        --local countProcessed = rcall("HLEN", jobKey .. ":processed")
+        local processed = rcall("HGETALL", jobKey .. ":processed")
+        if (#processed > 0) then
+            for i = 1, #processed, 2 do
+                local childJobId = getJobIdFromKey(processed[i])
+                local childJobPrefix = getJobKeyPrefix(processed[i], childJobId)
+                removeJob( childJobPrefix, childJobId, jobKey, removeChildren )
+            end
         end
-    end
-    local dependencies = rcall("SMEMBERS", jobKey .. ":dependencies")
-    if (#dependencies > 0) then
-        for i, childJobKey in ipairs(dependencies) do
-            -- We need to get the jobId for this job.
-            local childJobId = getJobIdFromKey(childJobKey)
-            local childJobPrefix = getJobKeyPrefix(childJobKey, childJobId)
-            removeJob( childJobPrefix, childJobId, jobKey )
+        local dependencies = rcall("SMEMBERS", jobKey .. ":dependencies")
+        if (#dependencies > 0) then
+            for i, childJobKey in ipairs(dependencies) do
+                -- We need to get the jobId for this job.
+                local childJobId = getJobIdFromKey(childJobKey)
+                local childJobPrefix = getJobKeyPrefix(childJobKey, childJobId)
+                removeJob( childJobPrefix, childJobId, jobKey, removeChildren )
+            end
         end
     end
     local prev = removeJobFromAnyState(prefix, jobId)
     rcall("DEL", jobKey, jobKey .. ":logs", jobKey .. ":dependencies", jobKey .. ":processed")
     -- -- delete keys related to rate limiter
         -- local limiterIndexTable = KEYS[10] .. ":index"
         -- local limitedSetKey = rcall("HGET", limiterIndexTable, jobId)
         -- if limitedSetKey then
         --     rcall("SREM", limitedSetKey, jobId)
         --     rcall("HDEL", limiterIndexTable, jobId)
     -- end
     rcall("XADD", prefix .. "events", "*", "event", "removed", "jobId", jobId, "prev", prev);
 end
 local prefix = KEYS[1]
-if not isLocked(prefix, ARGV[1]) then
-    removeJob(prefix, ARGV[1])
+if not isLocked(prefix, ARGV[1], ARGV[2]) then
+    removeJob(prefix, ARGV[1], nil, ARGV[2])
     return 1
 end
 return 0
```

### Comparing `bullmq-1.8.0/bullmq/commands/removeRepeatable-2.lua` & `bullmq-1.9.0/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/reprocessJob-6.lua` & `bullmq-1.9.0/bullmq/commands/reprocessJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/retryJob-9.lua` & `bullmq-1.9.0/bullmq/commands/retryJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/commands/retryJobs-6.lua` & `bullmq-1.9.0/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/event_emitter.py` & `bullmq-1.9.0/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/job.py` & `bullmq-1.9.0/bullmq/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,16 @@
     def changePriority(self, opts: dict):
         return self.scripts.changePriority(self.id, opts.get("priority", 0), opts.get("lifo", False))
 
     def updateProgress(self, progress):
         self.progress = progress
         return self.scripts.updateProgress(self.id, progress)
 
-    async def remove(self):
-        removed = await self.scripts.remove(self.id)
+    async def remove(self, opts: dict = {}):
+        removed = await self.scripts.remove(self.id, opts.get("removeChildren", True))
         
         if not removed:
             raise Exception(f"Could not remove job {self.id}")
 
     async def moveToFailed(self, err, token:str, fetchNext:bool = False):
         error_message = str(err)
         self.failedReason = error_message
```

### Comparing `bullmq-1.8.0/bullmq/queue.py` & `bullmq-1.9.0/bullmq/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,9 +213,9 @@
 
     def close(self):
         """
         Close the queue instance.
         """
         return self.redisConnection.close()
 
-    def remove(self, job_id: str):
-        return self.scripts.remove(job_id)
+    def remove(self, job_id: str, opts: dict = {}):
+        return self.scripts.remove(job_id, opts.get("removeChildren", True))
```

### Comparing `bullmq-1.8.0/bullmq/redis_connection.py` & `bullmq-1.9.0/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/scripts.py` & `bullmq-1.9.0/bullmq/scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,17 +219,17 @@
         result = await self.commands["moveToDelayed"](keys=keys, args=args)
 
         if result is not None:
             if result < 0:
                 raise self.finishedErrors(result, job_id, 'moveToDelayed', 'active')
         return None
 
-    def remove(self, job_id: str):
+    def remove(self, job_id: str, remove_children: bool):
         keys = self.getKeys([''])
-        args = [job_id]
+        args = [job_id, 1 if remove_children else 0]
 
         return self.commands["removeJob"](keys=keys, args=args)
 
     def getCounts(self, types):
         keys = self.getKeys([''])
         transformed_types = list(
             map(lambda type: 'wait' if type == 'waiting' else type, types))
```

### Comparing `bullmq-1.8.0/bullmq/timer.py` & `bullmq-1.9.0/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/types/job_options.py` & `bullmq-1.9.0/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/types/worker_options.py` & `bullmq-1.9.0/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/utils.py` & `bullmq-1.9.0/bullmq/utils.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq/worker.py` & `bullmq-1.9.0/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/bullmq.egg-info/PKG-INFO` & `bullmq-1.9.0/bullmq.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.8.0
+Version: 1.9.0
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-1.8.0/bullmq.egg-info/SOURCES.txt` & `bullmq-1.9.0/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-1.8.0/pyproject.toml` & `bullmq-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bullmq"
-version = "1.8.0"
+version = "1.9.0"
 description='BullMQ for Python'
 readme="README.md"
 authors = [
     {name = "Taskforce.sh Inc.", email = "manast@taskforce.sh"},
 ]
 requires-python = ">=3.10.0"
 classifiers=[
```

