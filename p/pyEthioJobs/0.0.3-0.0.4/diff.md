# Comparing `tmp/pyEthioJobs-0.0.3.tar.gz` & `tmp/pyEthioJobs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEthioJobs-0.0.3.tar", last modified: Wed Aug  2 16:23:54 2023, max compression
+gzip compressed data, was "pyEthioJobs-0.0.4.tar", last modified: Thu Aug  3 07:27:29 2023, max compression
```

## Comparing `pyEthioJobs-0.0.3.tar` & `pyEthioJobs-0.0.4.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.714229 pyEthioJobs-0.0.3/
--rw-rw-rw-   0        0        0     1083 2023-07-31 11:01:26.000000 pyEthioJobs-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3140 2023-08-02 16:23:54.713221 pyEthioJobs-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2856 2023-04-15 12:26:55.000000 pyEthioJobs-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.662981 pyEthioJobs-0.0.3/pyEthioJobs.egg-info/
--rw-rw-rw-   0        0        0     3140 2023-08-02 16:23:54.000000 pyEthioJobs-0.0.3/pyEthioJobs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1623 2023-08-02 16:23:54.000000 pyEthioJobs-0.0.3/pyEthioJobs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 16:23:54.000000 pyEthioJobs-0.0.3/pyEthioJobs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-02 16:23:54.000000 pyEthioJobs-0.0.3/pyEthioJobs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-02 16:23:54.000000 pyEthioJobs-0.0.3/pyEthioJobs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.677224 pyEthioJobs-0.0.3/pyethiojobs/
--rw-rw-rw-   0        0        0       35 2022-08-23 12:36:17.000000 pyEthioJobs-0.0.3/pyethiojobs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.677224 pyEthioJobs-0.0.3/pyethiojobs/errors/
--rw-rw-rw-   0        0        0      153 2023-07-31 10:59:34.000000 pyEthioJobs-0.0.3/pyethiojobs/errors/__init__.py
--rw-rw-rw-   0        0        0     3693 2023-04-10 07:51:27.000000 pyEthioJobs-0.0.3/pyethiojobs/filters.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.679231 pyEthioJobs-0.0.3/pyethiojobs/handler/
--rw-rw-rw-   0        0        0       45 2022-08-13 17:02:28.000000 pyEthioJobs-0.0.3/pyethiojobs/handler/__init__.py
--rw-rw-rw-   0        0        0     1105 2023-04-15 08:15:09.000000 pyEthioJobs-0.0.3/pyethiojobs/handler/handlers_holder.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.680218 pyEthioJobs-0.0.3/pyethiojobs/methods/
--rw-rw-rw-   0        0        0      239 2023-04-15 08:47:35.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.682222 pyEthioJobs-0.0.3/pyethiojobs/methods/category/
--rw-rw-rw-   0        0        0      143 2022-08-23 13:33:07.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/category/__init__.py
--rw-rw-rw-   0        0        0      799 2022-11-05 07:40:34.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/category/get_categories.py
--rw-rw-rw-   0        0        0      582 2022-08-23 12:09:41.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/category/get_category.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.684223 pyEthioJobs-0.0.3/pyethiojobs/methods/decorators/
--rw-rw-rw-   0        0        0       72 2023-04-15 08:39:30.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/decorators/__init__.py
--rw-rw-rw-   0        0        0      881 2023-04-10 07:57:37.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/decorators/on_new_job.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.686223 pyEthioJobs-0.0.3/pyethiojobs/methods/gov/
--rw-rw-rw-   0        0        0      161 2022-11-05 12:53:06.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/gov/__init__.py
--rw-rw-rw-   0        0        0     1590 2022-11-05 16:45:01.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/gov/get_gov_job_details.py
--rw-rw-rw-   0        0        0     1014 2022-11-05 12:51:10.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/gov/get_gov_jobs.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.690225 pyEthioJobs-0.0.3/pyethiojobs/methods/job/
--rw-rw-rw-   0        0        0      117 2023-07-31 14:36:54.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/job/__init__.py
--rw-rw-rw-   0        0        0      469 2023-07-31 10:54:54.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/job/get_job.py
--rw-rw-rw-   0        0        0     2626 2023-07-31 18:09:49.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/job/get_latest_jobs.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.693228 pyEthioJobs-0.0.3/pyethiojobs/methods/search/
--rw-rw-rw-   0        0        0       66 2022-08-23 13:33:40.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/search/__init__.py
--rw-rw-rw-   0        0        0     1019 2023-04-15 12:02:43.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/search/search.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.696233 pyEthioJobs-0.0.3/pyethiojobs/methods/utlis/
--rw-rw-rw-   0        0        0      155 2023-04-15 08:34:22.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/utlis/__init__.py
--rw-rw-rw-   0        0        0     2605 2023-08-02 13:57:40.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/utlis/get_job_detail.py
--rw-rw-rw-   0        0        0     2659 2023-07-31 18:56:17.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/utlis/get_jobs.py
--rw-rw-rw-   0        0        0     1247 2023-04-15 09:20:19.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/utlis/run.py
--rw-rw-rw-   0        0        0     1240 2023-07-31 11:00:30.000000 pyEthioJobs-0.0.3/pyethiojobs/pyethiojobs.py
--rw-rw-rw-   0        0        0     3329 2023-07-31 10:56:03.000000 pyEthioJobs-0.0.3/pyethiojobs/scaffold.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.697219 pyEthioJobs-0.0.3/pyethiojobs/types/
--rw-rw-rw-   0        0        0      316 2023-04-10 07:14:55.000000 pyEthioJobs-0.0.3/pyethiojobs/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.698223 pyEthioJobs-0.0.3/pyethiojobs/types/category/
--rw-rw-rw-   0        0        0       32 2022-08-21 18:57:29.000000 pyEthioJobs-0.0.3/pyethiojobs/types/category/__init__.py
--rw-rw-rw-   0        0        0      377 2022-11-04 18:31:26.000000 pyEthioJobs-0.0.3/pyethiojobs/types/category/category.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.700223 pyEthioJobs-0.0.3/pyethiojobs/types/employment/
--rw-rw-rw-   0        0        0       44 2023-04-10 07:14:02.000000 pyEthioJobs-0.0.3/pyethiojobs/types/employment/__init__.py
--rw-rw-rw-   0        0        0      136 2023-04-10 07:26:47.000000 pyEthioJobs-0.0.3/pyethiojobs/types/employment/employment_type.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.711221 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/
--rw-rw-rw-   0        0        0      231 2022-11-05 11:45:09.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/__init__.py
--rw-rw-rw-   0        0        0      652 2023-04-10 05:37:48.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/gov_job.py
--rw-rw-rw-   0        0        0      526 2022-11-05 15:24:04.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/gov_job_details.py
--rw-rw-rw-   0        0        0      112 2022-08-21 18:58:28.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/identifier.py
--rw-rw-rw-   0        0        0     1450 2023-07-31 18:07:17.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/job.py
--rw-rw-rw-   0        0        0     1082 2022-11-05 16:29:18.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/job_details.py
--rw-rw-rw-   0        0        0      203 2022-11-05 12:24:40.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/job_type.py
--rw-rw-rw-   0        0        0      296 2022-08-21 19:07:53.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/location.py
--rw-rw-rw-   0        0        0       85 2022-08-23 16:09:19.000000 pyEthioJobs-0.0.3/pyethiojobs/utils.py
--rw-rw-rw-   0        0        0       42 2023-08-02 16:23:54.714229 pyEthioJobs-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      580 2023-08-02 16:23:37.000000 pyEthioJobs-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.723404 pyEthioJobs-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-08-03 07:27:29.723404 pyEthioJobs-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.719404 pyEthioJobs-0.0.4/pyEthioJobs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-08-03 07:27:29.000000 pyEthioJobs-0.0.4/pyEthioJobs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-03 07:27:29.000000 pyEthioJobs-0.0.4/pyEthioJobs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:27:29.000000 pyEthioJobs-0.0.4/pyEthioJobs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 07:27:29.000000 pyEthioJobs-0.0.4/pyEthioJobs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 07:27:29.000000 pyEthioJobs-0.0.4/pyEthioJobs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.719404 pyEthioJobs-0.0.4/pyethiojobs/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.719404 pyEthioJobs-0.0.4/pyethiojobs/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.719404 pyEthioJobs-0.0.4/pyethiojobs/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/handler/handlers_holder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.719404 pyEthioJobs-0.0.4/pyethiojobs/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.719404 pyEthioJobs-0.0.4/pyethiojobs/methods/category/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/category/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/category/get_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/category/get_category.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.719404 pyEthioJobs-0.0.4/pyethiojobs/methods/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/decorators/on_new_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.719404 pyEthioJobs-0.0.4/pyethiojobs/methods/gov/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/gov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/gov/get_gov_job_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/gov/get_gov_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.719404 pyEthioJobs-0.0.4/pyethiojobs/methods/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/job/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/job/get_latest_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.723404 pyEthioJobs-0.0.4/pyethiojobs/methods/search/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/search/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.723404 pyEthioJobs-0.0.4/pyethiojobs/methods/utlis/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/utlis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/utlis/convert_to_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/utlis/get_job_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/utlis/get_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/methods/utlis/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/pyethiojobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.723404 pyEthioJobs-0.0.4/pyethiojobs/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.723404 pyEthioJobs-0.0.4/pyethiojobs/types/category/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/types/category/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/types/category/category.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.723404 pyEthioJobs-0.0.4/pyethiojobs/types/employment/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/types/employment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/types/employment/employment_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:27:29.723404 pyEthioJobs-0.0.4/pyethiojobs/types/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/types/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/types/jobs/gov_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/types/jobs/gov_job_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/types/jobs/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/types/jobs/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/types/jobs/job_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/types/jobs/job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/types/jobs/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/pyethiojobs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:27:29.723404 pyEthioJobs-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-03 07:27:17.000000 pyEthioJobs-0.0.4/setup.py
```

### Comparing `pyEthioJobs-0.0.3/PKG-INFO` & `pyEthioJobs-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-Metadata-Version: 2.1
-Name: pyEthioJobs
-Version: 0.0.3
-Summary: A python package to scrape jobs from ethiojobs.net
-Home-page: https://github.com/wizkiye/pyEthioJobs
-Author: Kidus
-Author-email: wizkiye@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-<p align="center">    
-<a href="https://github.com/wizkiye/pyethiojobs.git">    
-<img height="500" src="./.github/images/logo.png" alt="PyEthioJobs">    
-</a>    
-<br>    
-<b>Asynchronous <a href="https://ethiojobs.net">ethiojobs</a> Scraper written with python3 </b>    
-<br>    
-<a href="">    
-Examples</a>    
-
-# What is this?
-
-Asynchronous python3 Scrapper for ethiojobs.net
-
-# Installation
-
-`pip3 install -U git+https://github.com/wizkiye/pyethiojobs.git`
-
-# Example Usage
-
-
-
-```python 
-from pyethiojobs import EthioJobs  
-from pyethiojobs.types import EmploymentType
-
-ethiojobs = EthioJobs()
-
-
-#Searching for jobs
-async def main():  
-    results = await ethiojobs.search(
-        "designer", 
-        limit=10, 
-        employment_type=EmploymentType.FULL_TIME
-    )  # this will return list of jobs 
-    for result in results:
-        print(result.title) 
-        print(result.link) 
-
-# Getting list of categories        
-async def main():  
-    categories = await ethiojobs.get_categories()
-    for category in categories:
-        print(category.name)
-        print(category.link)
-        await category.get_jobs()  # this will return list of jobs in the category
-    
-
-# Getting list of jobs in a category
-async def main():  
-    jobs = await ethiojobs.get_category("category_link or Category Object")
-    for job in jobs:
-        print(job.title)
-        print(job.link)
-
-# Getting the latest jobs
-async def main():  
-    jobs = await ethiojobs.get_latest_jobs()
-    for job in jobs:
-        print(job.title)
-        print(job.link)
-        
-# Getting Government jobs
-async def main():  
-    jobs = await ethiojobs.get_gov_jobs() # this will return list of GovJob
-    for job in jobs:
-        print(job.company)
-        print(job.link)
-if __name__ == "__main__":  
-    import asyncio     
-    loop = asyncio.get_event_loop()  
-    loop.run_until_complete(main())
-```  
-
-# Using Decorators
-
-```python
-from pyethiojobs import EthioJobs, filters
-from pyethiojobs.types import  Job
-ethiojobs = EthioJobs()
-
-@ethiojobs.on_new_jobs()
-async def new_job_handler(job: Job):
-      print(job.__dict__)
-     
-     
-# this is not tested yet :D
-@ethiojobs.on_new_jobs(
-    filters.valid_through(20) 
-    & filters.work_place("Addis Ababa") 
-    & ~filters.hiring_organization("Ethio Telecom")
-)
-async def new_filtered_job_handler(job: Job):
-      print(job.__dict__)
-
-if __name__ == '__main__':
-     ethiojobs.run(poll_interval=30)
-```
-
-# Contributing
-
-If you want to contribute to this project, please read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
-
-# License
-
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
-
-# Acknowledgments
-
-* [ethiojobs](https://ethiojobs.net) for providing the data
-
-
-
-
+Metadata-Version: 2.1
+Name: pyEthioJobs
+Version: 0.0.4
+Summary: A python package to scrape jobs from ethiojobs.net
+Home-page: https://github.com/wizkiye/pyEthioJobs
+Author: Kidus
+Author-email: wizkiye@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+<p align="center">    
+<a href="https://github.com/wizkiye/pyethiojobs.git">    
+<img height="500" src="./.github/images/logo.png" alt="PyEthioJobs">    
+</a>    
+<br>    
+<b>Asynchronous <a href="https://ethiojobs.net">ethiojobs</a> Scraper written with python3 </b>    
+<br>    
+<a href="">    
+Examples</a>    
+
+# What is this?
+
+Asynchronous python3 Scrapper for ethiojobs.net
+
+# Installation
+
+`pip3 install -U git+https://github.com/wizkiye/pyethiojobs.git`
+
+# Example Usage
+
+
+
+```python 
+from pyethiojobs import EthioJobs  
+from pyethiojobs.types import EmploymentType
+
+ethiojobs = EthioJobs()
+
+
+#Searching for jobs
+async def main():  
+    results = await ethiojobs.search(
+        "designer", 
+        limit=10, 
+        employment_type=EmploymentType.FULL_TIME
+    )  # this will return list of jobs 
+    for result in results:
+        print(result.title) 
+        print(result.link) 
+
+# Getting list of categories        
+async def main():  
+    categories = await ethiojobs.get_categories()
+    for category in categories:
+        print(category.name)
+        print(category.link)
+        await category.get_jobs()  # this will return list of jobs in the category
+    
+
+# Getting list of jobs in a category
+async def main():  
+    jobs = await ethiojobs.get_category("category_link or Category Object")
+    for job in jobs:
+        print(job.title)
+        print(job.link)
+
+# Getting the latest jobs
+async def main():  
+    jobs = await ethiojobs.get_latest_jobs()
+    for job in jobs:
+        print(job.title)
+        print(job.link)
+        
+# Getting Government jobs
+async def main():  
+    jobs = await ethiojobs.get_gov_jobs() # this will return list of GovJob
+    for job in jobs:
+        print(job.company)
+        print(job.link)
+if __name__ == "__main__":  
+    import asyncio     
+    loop = asyncio.get_event_loop()  
+    loop.run_until_complete(main())
+```  
+
+# Using Decorators
+
+```python
+from pyethiojobs import EthioJobs, filters
+from pyethiojobs.types import  Job
+ethiojobs = EthioJobs()
+
+@ethiojobs.on_new_jobs()
+async def new_job_handler(job: Job):
+      print(job.__dict__)
+     
+     
+# this is not tested yet :D
+@ethiojobs.on_new_jobs(
+    filters.valid_through(20) 
+    & filters.work_place("Addis Ababa") 
+    & ~filters.hiring_organization("Ethio Telecom")
+)
+async def new_filtered_job_handler(job: Job):
+      print(job.__dict__)
+
+if __name__ == '__main__':
+     ethiojobs.run(poll_interval=30)
+```
+
+# Contributing
+
+If you want to contribute to this project, please read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+
+# License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
+
+# Acknowledgments
+
+* [ethiojobs](https://ethiojobs.net) for providing the data
+
+
+
+
```

### Comparing `pyEthioJobs-0.0.3/README.md` & `pyEthioJobs-0.0.4/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-
-<p align="center">    
-<a href="https://github.com/wizkiye/pyethiojobs.git">    
-<img height="500" src="./.github/images/logo.png" alt="PyEthioJobs">    
-</a>    
-<br>    
-<b>Asynchronous <a href="https://ethiojobs.net">ethiojobs</a> Scraper written with python3 </b>    
-<br>    
-<a href="">    
-Examples</a>    
-
-# What is this?
-
-Asynchronous python3 Scrapper for ethiojobs.net
-
-# Installation
-
-`pip3 install -U git+https://github.com/wizkiye/pyethiojobs.git`
-
-# Example Usage
-
-
-
-```python 
-from pyethiojobs import EthioJobs  
-from pyethiojobs.types import EmploymentType
-
-ethiojobs = EthioJobs()
-
-
-#Searching for jobs
-async def main():  
-    results = await ethiojobs.search(
-        "designer", 
-        limit=10, 
-        employment_type=EmploymentType.FULL_TIME
-    )  # this will return list of jobs 
-    for result in results:
-        print(result.title) 
-        print(result.link) 
-
-# Getting list of categories        
-async def main():  
-    categories = await ethiojobs.get_categories()
-    for category in categories:
-        print(category.name)
-        print(category.link)
-        await category.get_jobs()  # this will return list of jobs in the category
-    
-
-# Getting list of jobs in a category
-async def main():  
-    jobs = await ethiojobs.get_category("category_link or Category Object")
-    for job in jobs:
-        print(job.title)
-        print(job.link)
-
-# Getting the latest jobs
-async def main():  
-    jobs = await ethiojobs.get_latest_jobs()
-    for job in jobs:
-        print(job.title)
-        print(job.link)
-        
-# Getting Government jobs
-async def main():  
-    jobs = await ethiojobs.get_gov_jobs() # this will return list of GovJob
-    for job in jobs:
-        print(job.company)
-        print(job.link)
-if __name__ == "__main__":  
-    import asyncio     
-    loop = asyncio.get_event_loop()  
-    loop.run_until_complete(main())
-```  
-
-# Using Decorators
-
-```python
-from pyethiojobs import EthioJobs, filters
-from pyethiojobs.types import  Job
-ethiojobs = EthioJobs()
-
-@ethiojobs.on_new_jobs()
-async def new_job_handler(job: Job):
-      print(job.__dict__)
-     
-     
-# this is not tested yet :D
-@ethiojobs.on_new_jobs(
-    filters.valid_through(20) 
-    & filters.work_place("Addis Ababa") 
-    & ~filters.hiring_organization("Ethio Telecom")
-)
-async def new_filtered_job_handler(job: Job):
-      print(job.__dict__)
-
-if __name__ == '__main__':
-     ethiojobs.run(poll_interval=30)
-```
-
-# Contributing
-
-If you want to contribute to this project, please read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
-
-# License
-
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
-
-# Acknowledgments
-
-* [ethiojobs](https://ethiojobs.net) for providing the data
-
-
-
-
+
+<p align="center">    
+<a href="https://github.com/wizkiye/pyethiojobs.git">    
+<img height="500" src="./.github/images/logo.png" alt="PyEthioJobs">    
+</a>    
+<br>    
+<b>Asynchronous <a href="https://ethiojobs.net">ethiojobs</a> Scraper written with python3 </b>    
+<br>    
+<a href="">    
+Examples</a>    
+
+# What is this?
+
+Asynchronous python3 Scrapper for ethiojobs.net
+
+# Installation
+
+`pip3 install -U git+https://github.com/wizkiye/pyethiojobs.git`
+
+# Example Usage
+
+
+
+```python 
+from pyethiojobs import EthioJobs  
+from pyethiojobs.types import EmploymentType
+
+ethiojobs = EthioJobs()
+
+
+#Searching for jobs
+async def main():  
+    results = await ethiojobs.search(
+        "designer", 
+        limit=10, 
+        employment_type=EmploymentType.FULL_TIME
+    )  # this will return list of jobs 
+    for result in results:
+        print(result.title) 
+        print(result.link) 
+
+# Getting list of categories        
+async def main():  
+    categories = await ethiojobs.get_categories()
+    for category in categories:
+        print(category.name)
+        print(category.link)
+        await category.get_jobs()  # this will return list of jobs in the category
+    
+
+# Getting list of jobs in a category
+async def main():  
+    jobs = await ethiojobs.get_category("category_link or Category Object")
+    for job in jobs:
+        print(job.title)
+        print(job.link)
+
+# Getting the latest jobs
+async def main():  
+    jobs = await ethiojobs.get_latest_jobs()
+    for job in jobs:
+        print(job.title)
+        print(job.link)
+        
+# Getting Government jobs
+async def main():  
+    jobs = await ethiojobs.get_gov_jobs() # this will return list of GovJob
+    for job in jobs:
+        print(job.company)
+        print(job.link)
+if __name__ == "__main__":  
+    import asyncio     
+    loop = asyncio.get_event_loop()  
+    loop.run_until_complete(main())
+```  
+
+# Using Decorators
+
+```python
+from pyethiojobs import EthioJobs, filters
+from pyethiojobs.types import  Job
+ethiojobs = EthioJobs()
+
+@ethiojobs.on_new_jobs()
+async def new_job_handler(job: Job):
+      print(job.__dict__)
+     
+     
+# this is not tested yet :D
+@ethiojobs.on_new_jobs(
+    filters.valid_through(20) 
+    & filters.work_place("Addis Ababa") 
+    & ~filters.hiring_organization("Ethio Telecom")
+)
+async def new_filtered_job_handler(job: Job):
+      print(job.__dict__)
+
+if __name__ == '__main__':
+     ethiojobs.run(poll_interval=30)
+```
+
+# Contributing
+
+If you want to contribute to this project, please read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+
+# License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
+
+# Acknowledgments
+
+* [ethiojobs](https://ethiojobs.net) for providing the data
+
+
+
+
```

### Comparing `pyEthioJobs-0.0.3/pyEthioJobs.egg-info/PKG-INFO` & `pyEthioJobs-0.0.4/pyEthioJobs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-Metadata-Version: 2.1
-Name: pyEthioJobs
-Version: 0.0.3
-Summary: A python package to scrape jobs from ethiojobs.net
-Home-page: https://github.com/wizkiye/pyEthioJobs
-Author: Kidus
-Author-email: wizkiye@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-<p align="center">    
-<a href="https://github.com/wizkiye/pyethiojobs.git">    
-<img height="500" src="./.github/images/logo.png" alt="PyEthioJobs">    
-</a>    
-<br>    
-<b>Asynchronous <a href="https://ethiojobs.net">ethiojobs</a> Scraper written with python3 </b>    
-<br>    
-<a href="">    
-Examples</a>    
-
-# What is this?
-
-Asynchronous python3 Scrapper for ethiojobs.net
-
-# Installation
-
-`pip3 install -U git+https://github.com/wizkiye/pyethiojobs.git`
-
-# Example Usage
-
-
-
-```python 
-from pyethiojobs import EthioJobs  
-from pyethiojobs.types import EmploymentType
-
-ethiojobs = EthioJobs()
-
-
-#Searching for jobs
-async def main():  
-    results = await ethiojobs.search(
-        "designer", 
-        limit=10, 
-        employment_type=EmploymentType.FULL_TIME
-    )  # this will return list of jobs 
-    for result in results:
-        print(result.title) 
-        print(result.link) 
-
-# Getting list of categories        
-async def main():  
-    categories = await ethiojobs.get_categories()
-    for category in categories:
-        print(category.name)
-        print(category.link)
-        await category.get_jobs()  # this will return list of jobs in the category
-    
-
-# Getting list of jobs in a category
-async def main():  
-    jobs = await ethiojobs.get_category("category_link or Category Object")
-    for job in jobs:
-        print(job.title)
-        print(job.link)
-
-# Getting the latest jobs
-async def main():  
-    jobs = await ethiojobs.get_latest_jobs()
-    for job in jobs:
-        print(job.title)
-        print(job.link)
-        
-# Getting Government jobs
-async def main():  
-    jobs = await ethiojobs.get_gov_jobs() # this will return list of GovJob
-    for job in jobs:
-        print(job.company)
-        print(job.link)
-if __name__ == "__main__":  
-    import asyncio     
-    loop = asyncio.get_event_loop()  
-    loop.run_until_complete(main())
-```  
-
-# Using Decorators
-
-```python
-from pyethiojobs import EthioJobs, filters
-from pyethiojobs.types import  Job
-ethiojobs = EthioJobs()
-
-@ethiojobs.on_new_jobs()
-async def new_job_handler(job: Job):
-      print(job.__dict__)
-     
-     
-# this is not tested yet :D
-@ethiojobs.on_new_jobs(
-    filters.valid_through(20) 
-    & filters.work_place("Addis Ababa") 
-    & ~filters.hiring_organization("Ethio Telecom")
-)
-async def new_filtered_job_handler(job: Job):
-      print(job.__dict__)
-
-if __name__ == '__main__':
-     ethiojobs.run(poll_interval=30)
-```
-
-# Contributing
-
-If you want to contribute to this project, please read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
-
-# License
-
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
-
-# Acknowledgments
-
-* [ethiojobs](https://ethiojobs.net) for providing the data
-
-
-
-
+Metadata-Version: 2.1
+Name: pyEthioJobs
+Version: 0.0.4
+Summary: A python package to scrape jobs from ethiojobs.net
+Home-page: https://github.com/wizkiye/pyEthioJobs
+Author: Kidus
+Author-email: wizkiye@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+<p align="center">    
+<a href="https://github.com/wizkiye/pyethiojobs.git">    
+<img height="500" src="./.github/images/logo.png" alt="PyEthioJobs">    
+</a>    
+<br>    
+<b>Asynchronous <a href="https://ethiojobs.net">ethiojobs</a> Scraper written with python3 </b>    
+<br>    
+<a href="">    
+Examples</a>    
+
+# What is this?
+
+Asynchronous python3 Scrapper for ethiojobs.net
+
+# Installation
+
+`pip3 install -U git+https://github.com/wizkiye/pyethiojobs.git`
+
+# Example Usage
+
+
+
+```python 
+from pyethiojobs import EthioJobs  
+from pyethiojobs.types import EmploymentType
+
+ethiojobs = EthioJobs()
+
+
+#Searching for jobs
+async def main():  
+    results = await ethiojobs.search(
+        "designer", 
+        limit=10, 
+        employment_type=EmploymentType.FULL_TIME
+    )  # this will return list of jobs 
+    for result in results:
+        print(result.title) 
+        print(result.link) 
+
+# Getting list of categories        
+async def main():  
+    categories = await ethiojobs.get_categories()
+    for category in categories:
+        print(category.name)
+        print(category.link)
+        await category.get_jobs()  # this will return list of jobs in the category
+    
+
+# Getting list of jobs in a category
+async def main():  
+    jobs = await ethiojobs.get_category("category_link or Category Object")
+    for job in jobs:
+        print(job.title)
+        print(job.link)
+
+# Getting the latest jobs
+async def main():  
+    jobs = await ethiojobs.get_latest_jobs()
+    for job in jobs:
+        print(job.title)
+        print(job.link)
+        
+# Getting Government jobs
+async def main():  
+    jobs = await ethiojobs.get_gov_jobs() # this will return list of GovJob
+    for job in jobs:
+        print(job.company)
+        print(job.link)
+if __name__ == "__main__":  
+    import asyncio     
+    loop = asyncio.get_event_loop()  
+    loop.run_until_complete(main())
+```  
+
+# Using Decorators
+
+```python
+from pyethiojobs import EthioJobs, filters
+from pyethiojobs.types import  Job
+ethiojobs = EthioJobs()
+
+@ethiojobs.on_new_jobs()
+async def new_job_handler(job: Job):
+      print(job.__dict__)
+     
+     
+# this is not tested yet :D
+@ethiojobs.on_new_jobs(
+    filters.valid_through(20) 
+    & filters.work_place("Addis Ababa") 
+    & ~filters.hiring_organization("Ethio Telecom")
+)
+async def new_filtered_job_handler(job: Job):
+      print(job.__dict__)
+
+if __name__ == '__main__':
+     ethiojobs.run(poll_interval=30)
+```
+
+# Contributing
+
+If you want to contribute to this project, please read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+
+# License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
+
+# Acknowledgments
+
+* [ethiojobs](https://ethiojobs.net) for providing the data
+
+
+
+
```

### Comparing `pyEthioJobs-0.0.3/pyEthioJobs.egg-info/SOURCES.txt` & `pyEthioJobs-0.0.4/pyEthioJobs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 pyethiojobs/methods/gov/get_gov_jobs.py
 pyethiojobs/methods/job/__init__.py
 pyethiojobs/methods/job/get_job.py
 pyethiojobs/methods/job/get_latest_jobs.py
 pyethiojobs/methods/search/__init__.py
 pyethiojobs/methods/search/search.py
 pyethiojobs/methods/utlis/__init__.py
+pyethiojobs/methods/utlis/convert_to_pdf.py
 pyethiojobs/methods/utlis/get_job_detail.py
 pyethiojobs/methods/utlis/get_jobs.py
 pyethiojobs/methods/utlis/run.py
 pyethiojobs/types/__init__.py
 pyethiojobs/types/category/__init__.py
 pyethiojobs/types/category/category.py
 pyethiojobs/types/employment/__init__.py
```

### Comparing `pyEthioJobs-0.0.3/pyethiojobs/filters.py` & `pyEthioJobs-0.0.4/pyethiojobs/filters.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-import inspect
-from datetime import datetime, timedelta
-from typing import Callable, Union, List
-
-from pyethiojobs.types import Job
-
-
-class Filter:
-    async def __call__(self, job: Job):
-        raise NotImplementedError
-
-    def __invert__(self):
-        return Invert(self)
-
-    def __and__(self, other):
-        return And(self, other)
-
-    def __or__(self, other):
-        return Or(self, other)
-
-
-class Invert(Filter):
-    def __init__(self, base):
-        self.base = base
-
-    async def __call__(self, job: Job):
-        if inspect.iscoroutinefunction(self.base.__call__):
-            x = await self.base(job)
-            return not x
-        return
-
-
-class And(Filter):
-    def __init__(self, base, other):
-        self.base = base
-        self.other = other
-
-    async def __call__(self, job: Job):
-        x = await self.base(job)
-
-        if not x:
-            return False
-
-        y = await self.other(job)
-
-        return x and y
-
-
-class Or(Filter):
-    def __init__(self, base, other):
-        self.base = base
-        self.other = other
-
-    async def __call__(self, job: Job):
-        x = await self.base(job)
-        if x:
-            return True
-
-        y = await self.other(job)
-
-        return x or y
-
-
-CUSTOM_FILTER_NAME = "MyCustomFilter"
-
-
-def create(func: Callable, name: str = None, **kwargs) -> Filter:
-    return type(
-        name or func.__name__ or CUSTOM_FILTER_NAME,
-        (Filter,),
-        {"__call__": func, **kwargs},
-    )()
-
-
-def work_place(places: Union[str, List[str]]):
-    async def func(flt, job: Job):
-        if job.work_place in flt.places:
-            return True
-
-    return create(
-        func, "PlacesFilter", place=places if isinstance(places, list) else [places]
-    )
-
-
-def date(dates: Union[str, List[str]]):
-    async def func(flt, job: Job):
-        if job.date_posted in flt.dates:
-            return True
-
-    return create(
-        func, "DateFilter", dates=dates if isinstance(dates, list) else [dates]
-    )
-
-
-def valid_through(days: Union[str, int]):
-    async def func(flt, job: Job):
-        today = datetime.today()
-        job_valid_through = datetime.strptime(job.valid_through, "%Y-%m-%d %H:%M:%S")
-        if job_valid_through < today + timedelta(days=flt.days):
-            return True
-
-    return create(func, "ValidThroughFilter", days=days)
-
-
-def hiring_organization(organizations: Union[str, List[str]]):
-    async def func(flt, job: Job):
-        if job.hiring_organization in flt.organizations:
-            return True
-
-    return create(
-        func,
-        "HiringOrganizationFilter",
-        organizations=organizations
-        if isinstance(organizations, list)
-        else [organizations],
-    )
-
-
-def location(
-    address_country: Union[str, List[str]] = "ETH",
-    address_region: Union[str, List[str]] = None,
-    address_locality: Union[str, List[str]] = None,
-):
-    async def func(flt, job: Job):
-        if job.location.address_country in flt.address_country:
-            if flt.address_region is not None:
-                if job.location.address_region in flt.address_region:
-                    if flt.address_locality is not None:
-                        if job.location.address_locality in flt.address_locality:
-                            return True
-                    else:
-                        return True
-            else:
-                return True
-
-    return create(
-        func,
-        "LocationFilter",
-        address_country=address_country,
-        address_region=address_region,
-        address_locality=address_locality,
-    )
+import inspect
+from datetime import datetime, timedelta
+from typing import Callable, Union, List
+
+from pyethiojobs.types import Job
+
+
+class Filter:
+    async def __call__(self, job: Job):
+        raise NotImplementedError
+
+    def __invert__(self):
+        return Invert(self)
+
+    def __and__(self, other):
+        return And(self, other)
+
+    def __or__(self, other):
+        return Or(self, other)
+
+
+class Invert(Filter):
+    def __init__(self, base):
+        self.base = base
+
+    async def __call__(self, job: Job):
+        if inspect.iscoroutinefunction(self.base.__call__):
+            x = await self.base(job)
+            return not x
+        return
+
+
+class And(Filter):
+    def __init__(self, base, other):
+        self.base = base
+        self.other = other
+
+    async def __call__(self, job: Job):
+        x = await self.base(job)
+
+        if not x:
+            return False
+
+        y = await self.other(job)
+
+        return x and y
+
+
+class Or(Filter):
+    def __init__(self, base, other):
+        self.base = base
+        self.other = other
+
+    async def __call__(self, job: Job):
+        x = await self.base(job)
+        if x:
+            return True
+
+        y = await self.other(job)
+
+        return x or y
+
+
+CUSTOM_FILTER_NAME = "MyCustomFilter"
+
+
+def create(func: Callable, name: str = None, **kwargs) -> Filter:
+    return type(
+        name or func.__name__ or CUSTOM_FILTER_NAME,
+        (Filter,),
+        {"__call__": func, **kwargs},
+    )()
+
+
+def work_place(places: Union[str, List[str]]):
+    async def func(flt, job: Job):
+        if job.work_place in flt.places:
+            return True
+
+    return create(
+        func, "PlacesFilter", place=places if isinstance(places, list) else [places]
+    )
+
+
+def date(dates: Union[str, List[str]]):
+    async def func(flt, job: Job):
+        if job.date_posted in flt.dates:
+            return True
+
+    return create(
+        func, "DateFilter", dates=dates if isinstance(dates, list) else [dates]
+    )
+
+
+def valid_through(days: Union[str, int]):
+    async def func(flt, job: Job):
+        today = datetime.today()
+        job_valid_through = datetime.strptime(job.valid_through, "%Y-%m-%d %H:%M:%S")
+        if job_valid_through < today + timedelta(days=flt.days):
+            return True
+
+    return create(func, "ValidThroughFilter", days=days)
+
+
+def hiring_organization(organizations: Union[str, List[str]]):
+    async def func(flt, job: Job):
+        if job.hiring_organization in flt.organizations:
+            return True
+
+    return create(
+        func,
+        "HiringOrganizationFilter",
+        organizations=organizations
+        if isinstance(organizations, list)
+        else [organizations],
+    )
+
+
+def location(
+    address_country: Union[str, List[str]] = "ETH",
+    address_region: Union[str, List[str]] = None,
+    address_locality: Union[str, List[str]] = None,
+):
+    async def func(flt, job: Job):
+        if job.location.address_country in flt.address_country:
+            if flt.address_region is not None:
+                if job.location.address_region in flt.address_region:
+                    if flt.address_locality is not None:
+                        if job.location.address_locality in flt.address_locality:
+                            return True
+                    else:
+                        return True
+            else:
+                return True
+
+    return create(
+        func,
+        "LocationFilter",
+        address_country=address_country,
+        address_region=address_region,
+        address_locality=address_locality,
+    )
```

### Comparing `pyEthioJobs-0.0.3/pyethiojobs/handler/handlers_holder.py` & `pyEthioJobs-0.0.4/pyethiojobs/handler/handlers_holder.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import inspect
-from typing import Callable, Optional, List, Dict
-
-from pyethiojobs.types import Job
-
-
-class HandlersHolder:
-    def __init__(self, base):
-        self._base = base
-        self._events: Dict[str, List] = {
-            "NEW_JOB_HANDLER": [],
-        }
-
-    def set_handler(
-        self, event_name: str, func: Callable, filters: Optional[Callable] = None
-    ):
-        if inspect.iscoroutinefunction(func):
-            return self._events[event_name].append({"func": func, "filters": filters})
-        raise TypeError(f"{func.__name__} is not a coroutine function")
-
-    def remove_handler(self, event_name: str, func: Callable):
-        self._events[event_name] = [
-            event for event in self._events[event_name] if event["func"] != func
-        ]
-
-    async def incoming_job_handler(self, job: Job):
-        for event in self._events["NEW_JOB_HANDLER"]:
-            if event["filters"] is not None:
-                if event["filters"](job):
-                    await event["func"](job)
-            else:
-                await event["func"](job)
+import inspect
+from typing import Callable, Optional, List, Dict
+
+from pyethiojobs.types import Job
+
+
+class HandlersHolder:
+    def __init__(self, base):
+        self._base = base
+        self._events: Dict[str, List] = {
+            "NEW_JOB_HANDLER": [],
+        }
+
+    def set_handler(
+        self, event_name: str, func: Callable, filters: Optional[Callable] = None
+    ):
+        if inspect.iscoroutinefunction(func):
+            return self._events[event_name].append({"func": func, "filters": filters})
+        raise TypeError(f"{func.__name__} is not a coroutine function")
+
+    def remove_handler(self, event_name: str, func: Callable):
+        self._events[event_name] = [
+            event for event in self._events[event_name] if event["func"] != func
+        ]
+
+    async def incoming_job_handler(self, job: Job):
+        for event in self._events["NEW_JOB_HANDLER"]:
+            if event["filters"] is not None:
+                if event["filters"](job):
+                    await event["func"](job)
+            else:
+                await event["func"](job)
```

### Comparing `pyEthioJobs-0.0.3/pyethiojobs/methods/category/get_categories.py` & `pyEthioJobs-0.0.4/pyethiojobs/methods/category/get_categories.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.3/pyethiojobs/methods/decorators/on_new_job.py` & `pyEthioJobs-0.0.4/pyethiojobs/methods/decorators/on_new_job.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.3/pyethiojobs/methods/gov/get_gov_job_details.py` & `pyEthioJobs-0.0.4/pyethiojobs/methods/gov/get_gov_job_details.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from bs4 import Tag
-
-from pyethiojobs.scaffold import Scaffold
-from pyethiojobs.types import GovJobDetails, JobType
-
-
-class GetGovJobsDetails(Scaffold):
-    def _get_gov_job_details(self, html) -> GovJobDetails:
-        soup = self.soup(html)
-        job_title = soup.find("h1", {"class": "details-header__title "}).text
-        location, gov_type = soup.find_all(
-            "li",
-            {"class": "listing-item__info--item listing-item__info--item-location"},
-        )
-        company = soup.find(
-            "li", {"class": "listing-item__info--item listing-item__info--item-company"}
-        )
-        deadline = soup.find(
-            "li", {"class": "listing-item__info--item listing-item__info--item-date"}
-        )
-        job_: Tag = soup.find("div", {"class": "job-type"})
-        job_t = job_.find_all("span", {"class": "job-type__value"})
-        salary, working_time = job_t[:2]
-        type = ", ".join([j.text.strip() for j in job_t[2:]])
-        # Todo separate the discription to Education level, Work experience, Instruction ...
-        description = soup.find("div", {"class": "pull-left details-body__left"})
-        job = JobType(salary=salary.text, working_time=working_time.text, type=type)
-        return GovJobDetails(
-            job_title=job_title.strip(),
-            company=company.text.strip(),
-            location=location.text.strip(),
-            gov_type=gov_type.text.strip(),
-            deadline=deadline.text.strip(),
-            job_type=job,
-            description=description.text.strip(),
-        )
+from bs4 import Tag
+
+from pyethiojobs.scaffold import Scaffold
+from pyethiojobs.types import GovJobDetails, JobType
+
+
+class GetGovJobsDetails(Scaffold):
+    def _get_gov_job_details(self, html) -> GovJobDetails:
+        soup = self.soup(html)
+        job_title = soup.find("h1", {"class": "details-header__title "}).text
+        location, gov_type = soup.find_all(
+            "li",
+            {"class": "listing-item__info--item listing-item__info--item-location"},
+        )
+        company = soup.find(
+            "li", {"class": "listing-item__info--item listing-item__info--item-company"}
+        )
+        deadline = soup.find(
+            "li", {"class": "listing-item__info--item listing-item__info--item-date"}
+        )
+        job_: Tag = soup.find("div", {"class": "job-type"})
+        job_t = job_.find_all("span", {"class": "job-type__value"})
+        salary, working_time = job_t[:2]
+        type = ", ".join([j.text.strip() for j in job_t[2:]])
+        # Todo separate the discription to Education level, Work experience, Instruction ...
+        description = soup.find("div", {"class": "pull-left details-body__left"})
+        job = JobType(salary=salary.text, working_time=working_time.text, type=type)
+        return GovJobDetails(
+            job_title=job_title.strip(),
+            company=company.text.strip(),
+            location=location.text.strip(),
+            gov_type=gov_type.text.strip(),
+            deadline=deadline.text.strip(),
+            job_type=job,
+            description=description.text.strip(),
+        )
```

### Comparing `pyEthioJobs-0.0.3/pyethiojobs/methods/gov/get_gov_jobs.py` & `pyEthioJobs-0.0.4/pyethiojobs/methods/gov/get_gov_jobs.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import List
-
-from bs4 import Tag
-
-from pyethiojobs.scaffold import Scaffold
-from pyethiojobs.types.jobs import GovJob
-
-
-class GetGovernmentJobs(Scaffold):
-    async def get_gov_jobs(self) -> List[GovJob]:
-        res = await self._process_request(url="")
-        soup = self.soup(res.text)
-        div: Tag = soup.find("div", {"id": "public_latest"})
-        gov_jobs = []
-        for job in div.find_all("div", {"class": "single_listing col-md-6"}):
-            anchor = job.find("a")
-            link = anchor.get("href")
-            job_ = anchor.text
-            company = job.find("p", {"class": "no-marign"})
-            posted = job.find("span", {"class": "pull-right"})
-            gov_jobs.append(
-                GovJob(
-                    company=company.text.strip(),
-                    link=link,
-                    job=job_.strip(),
-                    posted=posted,
-                    base=self,
-                )
-            )
-        return gov_jobs
+from typing import List
+
+from bs4 import Tag
+
+from pyethiojobs.scaffold import Scaffold
+from pyethiojobs.types.jobs import GovJob
+
+
+class GetGovernmentJobs(Scaffold):
+    async def get_gov_jobs(self) -> List[GovJob]:
+        res = await self._process_request(url="")
+        soup = self.soup(res.text)
+        div: Tag = soup.find("div", {"id": "public_latest"})
+        gov_jobs = []
+        for job in div.find_all("div", {"class": "single_listing col-md-6"}):
+            anchor = job.find("a")
+            link = anchor.get("href")
+            job_ = anchor.text
+            company = job.find("p", {"class": "no-marign"})
+            posted = job.find("span", {"class": "pull-right"})
+            gov_jobs.append(
+                GovJob(
+                    company=company.text.strip(),
+                    link=link,
+                    job=job_.strip(),
+                    posted=posted,
+                    base=self,
+                )
+            )
+        return gov_jobs
```

### Comparing `pyEthioJobs-0.0.3/pyethiojobs/methods/job/get_latest_jobs.py` & `pyEthioJobs-0.0.4/pyethiojobs/methods/job/get_latest_jobs.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.3/pyethiojobs/methods/utlis/get_job_detail.py` & `pyEthioJobs-0.0.4/pyethiojobs/methods/utlis/get_job_detail.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.3/pyethiojobs/scaffold.py` & `pyEthioJobs-0.0.4/pyethiojobs/scaffold.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,116 +1,125 @@
-from typing import List, Callable, Union
-
-import httpx
-from bs4 import BeautifulSoup
-
-from pyethiojobs.filters import Filter
-from pyethiojobs.handler import HandlersHolder
-from pyethiojobs.types import Job, JobDetails, EmploymentType, GovJobDetails, Category
-from pyethiojobs.types.jobs import GovJob
-
-
-class Scaffold:
-    def __init__(self):
-        self._session = None
-        self._soup = None
-        self._BASE_URL = "https://www.ethiojobs.net/{}"
-        self._on_event_update: HandlersHolder = None
-
-    async def _process_request(
-        self, url: str, method="GET", **kwargs
-    ) -> httpx.Response:
-        """
-        Process a request.
-        :param url: URL to request.
-        :param method: Method to use. Default is GET.
-        :param kwargs: Keyword arguments to pass to the request.
-        :return:
-        """
-        pass
-
-    def soup(self, html: str) -> BeautifulSoup:
-        """
-        Get a BeautifulSoup object from an HTML string.
-        :param html: HTML string.
-        :return:
-        """
-        pass
-
-    def _get_jobs(self, html) -> List[Job]:
-        """
-        Get jobs from HTML.
-        :param html:
-        :return:
-        """
-        pass
-
-    def _get_job_details(self, html) -> JobDetails:
-        """
-        Get job details from HTML.
-        :param html:
-        :return:
-        """
-        pass
-
-    async def get_categories(self) -> List[Category]:
-        """
-        Get all categories from the site.
-        :return: List of categories.
-        """
-        pass
-
-    async def get_category(
-        self, category: Union[int, str, Category], limit: int = 10
-    ) -> List[Job]:
-        """
-        Get jobs from a category.
-        :param category: Category to get jobs from. Can be a Category object, a string or an int.
-        :param limit: Number of jobs to get. Default is 10.
-        :return: List of jobs.
-        """
-        pass
-
-    def on_new_jobs(self, filters: Filter = None) -> Callable:
-        """
-        Decorator to listen for new jobs.
-        :param filters: Filters to apply to the jobs.
-        :return: Decorator.
-        """
-        pass
-
-    def _get_gov_job_details(self, html) -> GovJobDetails:
-        pass
-
-    async def get_gov_jobs(self) -> List[GovJob]:
-        """
-        Get the latest government jobs from the site.
-        :return: List of Gov jobs.
-        """
-        pass
-
-    async def get_latest_jobs(self) -> List[Job]:
-        """
-        Get the latest jobs from the site.
-        :return: List of jobs.
-        """
-        pass
-
-    async def search(
-        self, query: str, limit: int = 10, employment_type: EmploymentType = None
-    ) -> List[Job]:
-        """
-        Search for jobs.
-        :param query: Query to search for.
-        :param limit: Number of jobs to return. Default is 10.
-        :param employment_type: Type of employment to search for. Default is None. Can be FULL_TIME, PART_TIME,
-        CONTRACT, INTERNSHIP, VOLUNTEER.
-        :return: List of jobs.
-        """
-        pass
-
-    def run(self, poll_interval: int = 60) -> None:
-        """
-        Run the listener.
-        :param poll_interval: Interval to poll for new jobs. Default is 60 seconds.
-        """
-        pass
+from typing import List, Callable, Union
+
+import httpx
+from bs4 import BeautifulSoup
+
+from pyethiojobs.filters import Filter
+from pyethiojobs.handler import HandlersHolder
+from pyethiojobs.types import Job, JobDetails, EmploymentType, GovJobDetails, Category
+from pyethiojobs.types.jobs import GovJob
+
+
+class Scaffold:
+    def __init__(self):
+        self._session = None
+        self._soup = None
+        self._BASE_URL = "https://www.ethiojobs.net/{}"
+        self._on_event_update: HandlersHolder = None
+
+    async def _process_request(
+        self, url: str, method="GET", **kwargs
+    ) -> httpx.Response:
+        """
+        Process a request.
+        :param url: URL to request.
+        :param method: Method to use. Default is GET.
+        :param kwargs: Keyword arguments to pass to the request.
+        :return:
+        """
+        pass
+
+    def soup(self, html: str) -> BeautifulSoup:
+        """
+        Get a BeautifulSoup object from an HTML string.
+        :param html: HTML string.
+        :return:
+        """
+        pass
+
+    def _get_jobs(self, html) -> List[Job]:
+        """
+        Get jobs from HTML.
+        :param html:
+        :return:
+        """
+        pass
+
+    def _get_job_details(self, html) -> JobDetails:
+        """
+        Get job details from HTML.
+        :param html:
+        :return:
+        """
+        pass
+
+    async def get_categories(self) -> List[Category]:
+        """
+        Get all categories from the site.
+        :return: List of categories.
+        """
+        pass
+
+    async def get_category(
+        self, category: Union[int, str, Category], limit: int = 10
+    ) -> List[Job]:
+        """
+        Get jobs from a category.
+        :param category: Category to get jobs from. Can be a Category object, a string or an int.
+        :param limit: Number of jobs to get. Default is 10.
+        :return: List of jobs.
+        """
+        pass
+
+    def on_new_jobs(self, filters: Filter = None) -> Callable:
+        """
+        Decorator to listen for new jobs.
+        :param filters: Filters to apply to the jobs.
+        :return: Decorator.
+        """
+        pass
+
+    def _get_gov_job_details(self, html) -> GovJobDetails:
+        pass
+
+    async def get_gov_jobs(self) -> List[GovJob]:
+        """
+        Get the latest government jobs from the site.
+        :return: List of Gov jobs.
+        """
+        pass
+
+    async def get_latest_jobs(self) -> List[Job]:
+        """
+        Get the latest jobs from the site.
+        :return: List of jobs.
+        """
+        pass
+
+    async def search(
+        self, query: str, limit: int = 10, employment_type: EmploymentType = None
+    ) -> List[Job]:
+        """
+        Search for jobs.
+        :param query: Query to search for.
+        :param limit: Number of jobs to return. Default is 10.
+        :param employment_type: Type of employment to search for. Default is None. Can be FULL_TIME, PART_TIME,
+        CONTRACT, INTERNSHIP, VOLUNTEER.
+        :return: List of jobs.
+        """
+        pass
+
+    def convert_to_pdf(self, job: Union[str, JobDetails], filename: str) -> str:
+        """
+        Convert a job to PDF.
+        :param job: Job to convert.
+        :param filename: Filename to save the PDF to.
+        :return: Path to the PDF.
+        """
+        pass
+
+    def run(self, poll_interval: int = 60) -> None:
+        """
+        Run the listener.
+        :param poll_interval: Interval to poll for new jobs. Default is 60 seconds.
+        """
+        pass
```

### Comparing `pyEthioJobs-0.0.3/pyethiojobs/types/jobs/job.py` & `pyEthioJobs-0.0.4/pyethiojobs/types/jobs/job.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from typing import Union
-
-from pyethiojobs import types
-
-
-class Job:
-    def __init__(
-        self,
-        job_id: str,
-        title: str,
-        description: str,
-        link: str,
-        identifier: "types.Identifier",
-        experience: str,
-        date_posted: str,
-        valid_through: str,
-        hiring_organization: str,
-        location: "types.Location",
-        work_place: Union[str, None],
-        type: str,
-        base: "pyethiojobs.pyEthioJobs" = None,
-    ):
-        self.job_id = job_id
-        self.experience = experience
-        self.work_place = work_place
-        self.title = title
-        self.description = description
-        self.link = link
-        self.identifier = identifier
-        self.date_posted = date_posted
-        self.valid_through = valid_through
-        self.hiring_organization = hiring_organization
-        self.location = location
-        self._base = base
-        self.type = type
-
-    async def get_details(self):
-        if self._base is not None:
-            res = await self._base._process_request(url=self.link)
-            return self._base._get_job_details(res.text)
-
-    def __repr__(self):
-        return f"Job(title={self.title}, link={self.link})"
-
-    def __str__(self):
-        return f"Job(title={self.title}, link={self.link})"
-
-    def __eq__(self, other):
-        return self.title == other.title and self.link == other.link
+from typing import Union
+
+from pyethiojobs import types
+
+
+class Job:
+    def __init__(
+        self,
+        job_id: str,
+        title: str,
+        description: str,
+        link: str,
+        identifier: "types.Identifier",
+        experience: str,
+        date_posted: str,
+        valid_through: str,
+        hiring_organization: str,
+        location: "types.Location",
+        work_place: Union[str, None],
+        type: str,
+        base: "pyethiojobs.pyEthioJobs" = None,
+    ):
+        self.job_id = job_id
+        self.experience = experience
+        self.work_place = work_place
+        self.title = title
+        self.description = description
+        self.link = link
+        self.identifier = identifier
+        self.date_posted = date_posted
+        self.valid_through = valid_through
+        self.hiring_organization = hiring_organization
+        self.location = location
+        self._base = base
+        self.type = type
+
+    async def get_details(self):
+        if self._base is not None:
+            res = await self._base._process_request(url=self.link)
+            return self._base._get_job_details(res.text)
+
+    def __repr__(self):
+        return f"Job(title={self.title}, link={self.link})"
+
+    def __str__(self):
+        return f"Job(title={self.title}, link={self.link})"
+
+    def __eq__(self, other):
+        return self.title == other.title and self.link == other.link
```

### Comparing `pyEthioJobs-0.0.3/setup.py` & `pyEthioJobs-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_file(filename: str) -> str:
     with open(filename, encoding="utf-8", mode="r") as f:
         return f.read()
 
 
 setup(
     name="pyEthioJobs",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(),
     url="https://github.com/wizkiye/pyEthioJobs",
     license="",
     author="Kidus",
     author_email="wizkiye@gmail.com",
     long_description=read_file("README.md"),
     install_requires=["httpx", "bs4"],
```

