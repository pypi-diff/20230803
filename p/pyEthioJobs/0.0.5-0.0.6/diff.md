# Comparing `tmp/pyEthioJobs-0.0.5.tar.gz` & `tmp/pyEthioJobs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEthioJobs-0.0.5.tar", last modified: Thu Aug  3 07:31:57 2023, max compression
+gzip compressed data, was "pyEthioJobs-0.0.6.tar", last modified: Thu Aug  3 08:00:28 2023, max compression
```

## Comparing `pyEthioJobs-0.0.5.tar` & `pyEthioJobs-0.0.6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.286685 pyEthioJobs-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-08-03 07:31:57.286685 pyEthioJobs-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.282685 pyEthioJobs-0.0.5/pyEthioJobs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-08-03 07:31:57.000000 pyEthioJobs-0.0.5/pyEthioJobs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-03 07:31:57.000000 pyEthioJobs-0.0.5/pyEthioJobs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:31:57.000000 pyEthioJobs-0.0.5/pyEthioJobs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 07:31:57.000000 pyEthioJobs-0.0.5/pyEthioJobs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 07:31:57.000000 pyEthioJobs-0.0.5/pyEthioJobs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.282685 pyEthioJobs-0.0.5/pyethiojobs/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.282685 pyEthioJobs-0.0.5/pyethiojobs/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.282685 pyEthioJobs-0.0.5/pyethiojobs/handler/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/handler/handlers_holder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.282685 pyEthioJobs-0.0.5/pyethiojobs/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.282685 pyEthioJobs-0.0.5/pyethiojobs/methods/category/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/category/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/category/get_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/category/get_category.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.282685 pyEthioJobs-0.0.5/pyethiojobs/methods/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/decorators/on_new_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.282685 pyEthioJobs-0.0.5/pyethiojobs/methods/gov/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/gov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/gov/get_gov_job_details.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/gov/get_gov_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.282685 pyEthioJobs-0.0.5/pyethiojobs/methods/job/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/job/get_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/job/get_latest_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.282685 pyEthioJobs-0.0.5/pyethiojobs/methods/search/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/search/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.282685 pyEthioJobs-0.0.5/pyethiojobs/methods/utlis/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/utlis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/utlis/convert_to_pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/utlis/get_job_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/utlis/get_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/methods/utlis/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/pyethiojobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.282685 pyEthioJobs-0.0.5/pyethiojobs/types/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.286685 pyEthioJobs-0.0.5/pyethiojobs/types/category/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/types/category/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/types/category/category.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.286685 pyEthioJobs-0.0.5/pyethiojobs/types/employment/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/types/employment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/types/employment/employment_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:31:57.286685 pyEthioJobs-0.0.5/pyethiojobs/types/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/types/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/types/jobs/gov_job.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/types/jobs/gov_job_details.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/types/jobs/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/types/jobs/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/types/jobs/job_details.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/types/jobs/job_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/types/jobs/location.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/pyethiojobs/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:31:57.286685 pyEthioJobs-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-03 07:31:47.000000 pyEthioJobs-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.549508 pyEthioJobs-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-08-03 08:00:28.549508 pyEthioJobs-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.537508 pyEthioJobs-0.0.6/pyEthioJobs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-08-03 08:00:28.000000 pyEthioJobs-0.0.6/pyEthioJobs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-03 08:00:28.000000 pyEthioJobs-0.0.6/pyEthioJobs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:00:28.000000 pyEthioJobs-0.0.6/pyEthioJobs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 08:00:28.000000 pyEthioJobs-0.0.6/pyEthioJobs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 08:00:28.000000 pyEthioJobs-0.0.6/pyEthioJobs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.541509 pyEthioJobs-0.0.6/pyethiojobs/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.541509 pyEthioJobs-0.0.6/pyethiojobs/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.541509 pyEthioJobs-0.0.6/pyethiojobs/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/handler/handlers_holder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.541509 pyEthioJobs-0.0.6/pyethiojobs/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.541509 pyEthioJobs-0.0.6/pyethiojobs/methods/category/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/category/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/category/get_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/category/get_category.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.541509 pyEthioJobs-0.0.6/pyethiojobs/methods/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/decorators/on_new_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.541509 pyEthioJobs-0.0.6/pyethiojobs/methods/gov/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/gov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/gov/get_gov_job_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/gov/get_gov_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.545508 pyEthioJobs-0.0.6/pyethiojobs/methods/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/job/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/job/get_latest_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.545508 pyEthioJobs-0.0.6/pyethiojobs/methods/search/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/search/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.545508 pyEthioJobs-0.0.6/pyethiojobs/methods/utlis/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/utlis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/utlis/convert_to_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/utlis/get_job_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/utlis/get_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/methods/utlis/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/pyethiojobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.545508 pyEthioJobs-0.0.6/pyethiojobs/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.545508 pyEthioJobs-0.0.6/pyethiojobs/types/category/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/types/category/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/types/category/category.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.545508 pyEthioJobs-0.0.6/pyethiojobs/types/employment/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/types/employment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/types/employment/employment_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:00:28.549508 pyEthioJobs-0.0.6/pyethiojobs/types/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/types/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/types/jobs/gov_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/types/jobs/gov_job_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/types/jobs/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/types/jobs/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/types/jobs/job_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/types/jobs/job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/types/jobs/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/pyethiojobs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:00:28.549508 pyEthioJobs-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-03 08:00:12.000000 pyEthioJobs-0.0.6/setup.py
```

### Comparing `pyEthioJobs-0.0.5/LICENSE` & `pyEthioJobs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/PKG-INFO` & `pyEthioJobs-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEthioJobs
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package to scrape jobs from ethiojobs.net
 Home-page: https://github.com/wizkiye/pyEthioJobs
 Author: Kidus
 Author-email: wizkiye@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyEthioJobs-0.0.5/README.md` & `pyEthioJobs-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyEthioJobs.egg-info/PKG-INFO` & `pyEthioJobs-0.0.6/pyEthioJobs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEthioJobs
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package to scrape jobs from ethiojobs.net
 Home-page: https://github.com/wizkiye/pyEthioJobs
 Author: Kidus
 Author-email: wizkiye@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyEthioJobs-0.0.5/pyEthioJobs.egg-info/SOURCES.txt` & `pyEthioJobs-0.0.6/pyEthioJobs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/filters.py` & `pyEthioJobs-0.0.6/pyethiojobs/filters.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/handler/handlers_holder.py` & `pyEthioJobs-0.0.6/pyethiojobs/handler/handlers_holder.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/methods/category/get_categories.py` & `pyEthioJobs-0.0.6/pyethiojobs/methods/category/get_categories.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/methods/category/get_category.py` & `pyEthioJobs-0.0.6/pyethiojobs/methods/category/get_category.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/methods/decorators/on_new_job.py` & `pyEthioJobs-0.0.6/pyethiojobs/methods/decorators/on_new_job.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/methods/gov/get_gov_job_details.py` & `pyEthioJobs-0.0.6/pyethiojobs/methods/gov/get_gov_job_details.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/methods/gov/get_gov_jobs.py` & `pyEthioJobs-0.0.6/pyethiojobs/methods/gov/get_gov_jobs.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/methods/job/get_latest_jobs.py` & `pyEthioJobs-0.0.6/pyethiojobs/methods/job/get_latest_jobs.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/methods/search/search.py` & `pyEthioJobs-0.0.6/pyethiojobs/methods/search/search.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/methods/utlis/get_job_detail.py` & `pyEthioJobs-0.0.6/pyethiojobs/methods/utlis/get_job_detail.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/methods/utlis/get_jobs.py` & `pyEthioJobs-0.0.6/pyethiojobs/methods/utlis/get_jobs.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/methods/utlis/run.py` & `pyEthioJobs-0.0.6/pyethiojobs/methods/utlis/run.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/pyethiojobs.py` & `pyEthioJobs-0.0.6/pyethiojobs/pyethiojobs.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/scaffold.py` & `pyEthioJobs-0.0.6/pyethiojobs/scaffold.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/types/jobs/gov_job.py` & `pyEthioJobs-0.0.6/pyethiojobs/types/jobs/gov_job.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/types/jobs/job.py` & `pyEthioJobs-0.0.6/pyethiojobs/types/jobs/job.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/pyethiojobs/types/jobs/job_details.py` & `pyEthioJobs-0.0.6/pyethiojobs/types/jobs/job_details.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.5/setup.py` & `pyEthioJobs-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_file(filename: str) -> str:
     with open(filename, encoding="utf-8", mode="r") as f:
         return f.read()
 
 
 setup(
     name="pyEthioJobs",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(),
     url="https://github.com/wizkiye/pyEthioJobs",
     license="",
     author="Kidus",
     author_email="wizkiye@gmail.com",
     long_description=read_file("README.md"),
     install_requires=[
```

