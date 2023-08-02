# Comparing `tmp/testflows.github.runners-1.4.230802.1223657.tar.gz` & `tmp/testflows.github.runners-1.4.230802.1233850.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.4.230802.1223657.tar", last modified: Wed Aug  2 22:36:57 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.4.230802.1233850.tar", last modified: Wed Aug  2 23:38:51 2023, max compression
```

## Comparing `testflows.github.runners-1.4.230802.1223657.tar` & `testflows.github.runners-1.4.230802.1233850.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 22:36:57.770819 testflows.github.runners-1.4.230802.1223657/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1223657/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    64483 2023-08-02 22:36:57.770819 testflows.github.runners-1.4.230802.1223657/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    63891 2023-08-02 21:05:00.000000 testflows.github.runners-1.4.230802.1223657/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-02 22:36:57.770819 testflows.github.runners-1.4.230802.1223657/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-02 22:36:57.000000 testflows.github.runners-1.4.230802.1223657/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 22:36:57.766819 testflows.github.runners-1.4.230802.1223657/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 22:36:57.766819 testflows.github.runners-1.4.230802.1223657/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 22:36:57.770819 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-02 22:36:57.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1741 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     3019 2023-08-02 18:47:51.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 22:36:57.770819 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    26367 2023-08-02 19:33:45.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13654 2023-08-02 19:18:14.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     4481 2023-08-02 19:46:06.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    15656 2023-08-02 20:33:51.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    27664 2023-08-02 22:30:47.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 22:36:57.770819 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 22:36:57.770819 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     3032 2023-08-02 20:36:59.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5553 2023-08-02 18:56:43.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1512 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1223657/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 22:36:57.766819 testflows.github.runners-1.4.230802.1223657/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    64483 2023-08-02 22:36:57.000000 testflows.github.runners-1.4.230802.1223657/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-02 22:36:57.000000 testflows.github.runners-1.4.230802.1223657/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-02 22:36:57.000000 testflows.github.runners-1.4.230802.1223657/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.4.230802.1223657/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-02 22:36:57.000000 testflows.github.runners-1.4.230802.1223657/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-02 22:36:57.000000 testflows.github.runners-1.4.230802.1223657/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 23:38:51.196169 testflows.github.runners-1.4.230802.1233850/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1233850/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    64476 2023-08-02 23:38:51.196169 testflows.github.runners-1.4.230802.1233850/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    63884 2023-08-02 23:37:46.000000 testflows.github.runners-1.4.230802.1233850/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-02 23:38:51.196169 testflows.github.runners-1.4.230802.1233850/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-02 23:38:50.000000 testflows.github.runners-1.4.230802.1233850/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 23:38:51.192168 testflows.github.runners-1.4.230802.1233850/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 23:38:51.192168 testflows.github.runners-1.4.230802.1233850/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 23:38:51.196169 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-02 23:38:50.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1741 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3019 2023-08-02 18:47:51.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 23:38:51.196169 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    26388 2023-08-02 23:38:02.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13654 2023-08-02 19:18:14.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4481 2023-08-02 19:46:06.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15656 2023-08-02 20:33:51.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27664 2023-08-02 22:30:47.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 23:38:51.196169 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 23:38:51.196169 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     3032 2023-08-02 20:36:59.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5553 2023-08-02 18:56:43.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1512 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1233850/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 23:38:51.196169 testflows.github.runners-1.4.230802.1233850/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    64476 2023-08-02 23:38:51.000000 testflows.github.runners-1.4.230802.1233850/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-02 23:38:51.000000 testflows.github.runners-1.4.230802.1233850/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-02 23:38:51.000000 testflows.github.runners-1.4.230802.1233850/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.4.230802.1233850/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-02 23:38:51.000000 testflows.github.runners-1.4.230802.1233850/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-02 23:38:51.000000 testflows.github.runners-1.4.230802.1233850/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.4.230802.1223657/LICENSE` & `testflows.github.runners-1.4.230802.1233850/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/PKG-INFO` & `testflows.github.runners-1.4.230802.1233850/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.4.230802.1223657
+Version: 1.4.230802.1233850
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -420,41 +420,37 @@
 
    github-runners --max-runners 40
 
 =========================================================
 Specifying Maximum Number of Runners Used in Workflow Run
 =========================================================
 
-By default, the maximum number of runners that could be used by a single workflow run
-is not defined. Therefore, for example, if you have **--max-runners** set to *10*,
-and you have a few workflow runs that are **queued**, and each workflow
-contains more than *10* jobs, then only one workflow run will be running its jobs while
-the jobs in other workflow runs will be waiting as there will be no runners
-available until the run that uses all the runners for its jobs completes.
-
-If you would like for the runners to be divided more evenly between different
-**queued** workflow runs, then you can use the **--max-runners-in-workflow-run**
-option to limit the maximum number of runners used in a single workflow run.
+By default, the maximum number of runners that could be created for a single workflow run
+is not defined. 
+
+:❗Warning:
+   In general, GitHub does not allow to assign a job to a specific runner, and any available runner
+   that matches the labels could be used. Therefore, one can't control how runners are allocated
+   to queued workflow run jobs and this is why the **--max-runners-in-workflow-run** option will not behave
+   as one would intuitively expect.
+
+If you set the **--max-runners-in-workflow-run** to some value *X*, then **github-runners**
+will created the *X * number of queued workflow runs* runners. How these runners will be allocated by
+GitHub is out of our control. Therefore, the more runs are queued up the more runners will be created, up to the **--max-runners**
+limit, to try to complete the jobs faster. However, this does not mean that you will see exactly *X* number of jobs
+being executed in each queued workflow run. 
 
 For example,
 
 .. code-block:: bash
 
    github-runners --max-runners 40 --max-runners-in-workflow-run 5
 
-will allow only up to *5* runners to be used at the maximum in any single workflow run, and
-therefore would allow up to *8* **queued** workflow runs to run up to *5* jobs in each **queued**
-workflow run in parallel.
-
-:✋ Note:
-   Specifying the **--max-runners-in-workflow-run** option will increase the time a specific
-   workflow run takes to complete it jobs, if number of jobs in the workflow
-   is greater than the value of this option, as compared to the case if all available runners
-   would be allowed.
-
+will create upto *5* runners for each queued up workflow run. If there is only one workflow run, then the maximum number of
+runners will be *5* unless more queued up workflow runs appear, which then could speed up the execution of the run in progress.
 
 =============================
 Recycling Powered Off Servers
 =============================
 
 By default, recycling of powered off servers that has completed executing a job is turned on.
 
@@ -1701,15 +1697,15 @@
   and type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
 * **--max-runners-in-workflow-run count**
-  maximum number of runners allowed in a workflow run, default: not set
+  maximum number of runners allowed to be created for a single workflow run, default: not set
 
 * **--with-label label**
   only create runners for jobs that have the specified label,
   by default jobs are not skipped and runners will be created for any queued job
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
```

### Comparing `testflows.github.runners-1.4.230802.1223657/README.rst` & `testflows.github.runners-1.4.230802.1233850/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -403,41 +403,37 @@
 
    github-runners --max-runners 40
 
 =========================================================
 Specifying Maximum Number of Runners Used in Workflow Run
 =========================================================
 
-By default, the maximum number of runners that could be used by a single workflow run
-is not defined. Therefore, for example, if you have **--max-runners** set to *10*,
-and you have a few workflow runs that are **queued**, and each workflow
-contains more than *10* jobs, then only one workflow run will be running its jobs while
-the jobs in other workflow runs will be waiting as there will be no runners
-available until the run that uses all the runners for its jobs completes.
-
-If you would like for the runners to be divided more evenly between different
-**queued** workflow runs, then you can use the **--max-runners-in-workflow-run**
-option to limit the maximum number of runners used in a single workflow run.
+By default, the maximum number of runners that could be created for a single workflow run
+is not defined. 
+
+:❗Warning:
+   In general, GitHub does not allow to assign a job to a specific runner, and any available runner
+   that matches the labels could be used. Therefore, one can't control how runners are allocated
+   to queued workflow run jobs and this is why the **--max-runners-in-workflow-run** option will not behave
+   as one would intuitively expect.
+
+If you set the **--max-runners-in-workflow-run** to some value *X*, then **github-runners**
+will created the *X * number of queued workflow runs* runners. How these runners will be allocated by
+GitHub is out of our control. Therefore, the more runs are queued up the more runners will be created, up to the **--max-runners**
+limit, to try to complete the jobs faster. However, this does not mean that you will see exactly *X* number of jobs
+being executed in each queued workflow run. 
 
 For example,
 
 .. code-block:: bash
 
    github-runners --max-runners 40 --max-runners-in-workflow-run 5
 
-will allow only up to *5* runners to be used at the maximum in any single workflow run, and
-therefore would allow up to *8* **queued** workflow runs to run up to *5* jobs in each **queued**
-workflow run in parallel.
-
-:✋ Note:
-   Specifying the **--max-runners-in-workflow-run** option will increase the time a specific
-   workflow run takes to complete it jobs, if number of jobs in the workflow
-   is greater than the value of this option, as compared to the case if all available runners
-   would be allowed.
-
+will create upto *5* runners for each queued up workflow run. If there is only one workflow run, then the maximum number of
+runners will be *5* unless more queued up workflow runs appear, which then could speed up the execution of the run in progress.
 
 =============================
 Recycling Powered Off Servers
 =============================
 
 By default, recycling of powered off servers that has completed executing a job is turned on.
 
@@ -1684,15 +1680,15 @@
   and type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
 * **--max-runners-in-workflow-run count**
-  maximum number of runners allowed in a workflow run, default: not set
+  maximum number of runners allowed to be created for a single workflow run, default: not set
 
 * **--with-label label**
   only create runners for jobs that have the specified label,
   by default jobs are not skipped and runners will be created for any queued job
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
```

### Comparing `testflows.github.runners-1.4.230802.1223657/setup.py` & `testflows.github.runners-1.4.230802.1233850/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.4.230802.1223657",
+    version="1.4.230802.1233850",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/__init__.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.4.230802.1223657"
+__version__ = "1.4.230802.1233850"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/actions.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/api_watch.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/args.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/bin/github-runners`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         ),
     )
 
     parser.add_argument(
         "--max-runners-in-workflow-run",
         metavar="count",
         type=args.count_type,
-        help="maximum number of runners allowed for a workflow run, default: not set",
+        help="maximum number of runners allowed to be created for a single workflow run, default: not set",
     )
 
     parser.add_argument(
         "--with-label",
         metavar="label",
         type=str,
         help=(
```

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/cloud.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/config.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/config.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/delete.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/logger.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/request.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/server.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/service.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows/github/runners/shell.py` & `testflows.github.runners-1.4.230802.1233850/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.4.230802.1233850/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.4.230802.1223657
+Version: 1.4.230802.1233850
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -420,41 +420,37 @@
 
    github-runners --max-runners 40
 
 =========================================================
 Specifying Maximum Number of Runners Used in Workflow Run
 =========================================================
 
-By default, the maximum number of runners that could be used by a single workflow run
-is not defined. Therefore, for example, if you have **--max-runners** set to *10*,
-and you have a few workflow runs that are **queued**, and each workflow
-contains more than *10* jobs, then only one workflow run will be running its jobs while
-the jobs in other workflow runs will be waiting as there will be no runners
-available until the run that uses all the runners for its jobs completes.
-
-If you would like for the runners to be divided more evenly between different
-**queued** workflow runs, then you can use the **--max-runners-in-workflow-run**
-option to limit the maximum number of runners used in a single workflow run.
+By default, the maximum number of runners that could be created for a single workflow run
+is not defined. 
+
+:❗Warning:
+   In general, GitHub does not allow to assign a job to a specific runner, and any available runner
+   that matches the labels could be used. Therefore, one can't control how runners are allocated
+   to queued workflow run jobs and this is why the **--max-runners-in-workflow-run** option will not behave
+   as one would intuitively expect.
+
+If you set the **--max-runners-in-workflow-run** to some value *X*, then **github-runners**
+will created the *X * number of queued workflow runs* runners. How these runners will be allocated by
+GitHub is out of our control. Therefore, the more runs are queued up the more runners will be created, up to the **--max-runners**
+limit, to try to complete the jobs faster. However, this does not mean that you will see exactly *X* number of jobs
+being executed in each queued workflow run. 
 
 For example,
 
 .. code-block:: bash
 
    github-runners --max-runners 40 --max-runners-in-workflow-run 5
 
-will allow only up to *5* runners to be used at the maximum in any single workflow run, and
-therefore would allow up to *8* **queued** workflow runs to run up to *5* jobs in each **queued**
-workflow run in parallel.
-
-:✋ Note:
-   Specifying the **--max-runners-in-workflow-run** option will increase the time a specific
-   workflow run takes to complete it jobs, if number of jobs in the workflow
-   is greater than the value of this option, as compared to the case if all available runners
-   would be allowed.
-
+will create upto *5* runners for each queued up workflow run. If there is only one workflow run, then the maximum number of
+runners will be *5* unless more queued up workflow runs appear, which then could speed up the execution of the run in progress.
 
 =============================
 Recycling Powered Off Servers
 =============================
 
 By default, recycling of powered off servers that has completed executing a job is turned on.
 
@@ -1701,15 +1697,15 @@
   and type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
 * **--max-runners-in-workflow-run count**
-  maximum number of runners allowed in a workflow run, default: not set
+  maximum number of runners allowed to be created for a single workflow run, default: not set
 
 * **--with-label label**
   only create runners for jobs that have the specified label,
   by default jobs are not skipped and runners will be created for any queued job
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
```

### Comparing `testflows.github.runners-1.4.230802.1223657/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.4.230802.1233850/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

