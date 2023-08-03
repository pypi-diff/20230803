# Comparing `tmp/vdk-control-cli-1.3.948436673.tar.gz` & `tmp/vdk-control-cli-1.3.954631830.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-control-cli-1.3.948436673.tar", last modified: Fri Jul 28 09:42:30 2023, max compression
+gzip compressed data, was "vdk-control-cli-1.3.954631830.tar", last modified: Thu Aug  3 12:24:36 2023, max compression
```

## Comparing `vdk-control-cli-1.3.948436673.tar` & `vdk-control-cli-1.3.954631830.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.905512 vdk-control-cli-1.3.948436673/
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5153 2023-07-28 09:42:30.905512 vdk-control-cli-1.3.948436673/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1747 2023-07-28 09:42:30.909512 vdk-control-cli-1.3.948436673/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.897512 vdk-control-cli-1.3.948436673/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.897512 vdk-control-cli-1.3.948436673/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.897512 vdk-control-cli-1.3.948436673/src/vdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.897512 vdk-control-cli-1.3.948436673/src/vdk/api/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.897512 vdk-control-cli-1.3.948436673/src/vdk/api/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/api/control/plugin/markers.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/api/control/plugin/specs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.897512 vdk-control-cli-1.3.948436673/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.897512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.897512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.897512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/common_group/
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/common_group/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.897512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/info_group/
--rw-rw-rw-   0 root         (0) root         (0)     1868 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/info_group/info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.901512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/
--rw-rw-rw-   0 root         (0) root         (0)    12776 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/create.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/delete.py
--rw-rw-rw-   0 root         (0) root         (0)     7206 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/deploy_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14285 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     5129 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/download_job.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/download_key.py
--rw-rw-rw-   0 root         (0) root         (0)    12207 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/execute.py
--rw-rw-rw-   0 root         (0) root         (0)     8735 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/list.py
--rw-rw-rw-   0 root         (0) root         (0)    11314 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/properties.py
--rw-rw-rw-   0 root         (0) root         (0)    11433 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/secrets.py
--rw-rw-rw-   0 root         (0) root         (0)     3403 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/show.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.901512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/login_group/
--rw-rw-rw-   0 root         (0) root         (0)     6510 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/login_group/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.901512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/logout_group/
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/logout_group/logout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.901512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/version_group/
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/version_group/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.901512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/configuration/
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/configuration/default_options.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/configuration/defaults_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/configuration/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)     9551 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/configuration/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.901512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/exception/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/exception/vdk_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.901512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/job_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     4871 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/job_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.905512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/sample_job/
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/sample_job/10_sql_step.sql
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/sample_job/20_python_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/sample_job/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/sample_job/config.ini
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/sample_job/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     3666 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.905512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     3715 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/plugin/control_plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.905512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/rest_lib/
--rw-rw-rw-   0 root         (0) root         (0)     3239 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/rest_lib/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/rest_lib/rest_client_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.905512 vdk-control-cli-1.3.948436673/src/vdk/internal/control/utils/
--rw-rw-rw-   0 root         (0) root         (0)     7297 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/utils/cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/utils/control_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4587 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/utils/output_printer.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-28 09:42:07.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/utils/version_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-28 09:42:17.000000 vdk-control-cli-1.3.948436673/src/vdk/internal/control/vdk_control_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.905512 vdk-control-cli-1.3.948436673/src/vdk_control_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5153 2023-07-28 09:42:30.000000 vdk-control-cli-1.3.948436673/src/vdk_control_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2426 2023-07-28 09:42:30.000000 vdk-control-cli-1.3.948436673/src/vdk_control_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:30.000000 vdk-control-cli-1.3.948436673/src/vdk_control_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-28 09:42:30.000000 vdk-control-cli-1.3.948436673/src/vdk_control_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:30.000000 vdk-control-cli-1.3.948436673/src/vdk_control_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      185 2023-07-28 09:42:30.000000 vdk-control-cli-1.3.948436673/src/vdk_control_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:42:30.000000 vdk-control-cli-1.3.948436673/src/vdk_control_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-28 09:42:17.000000 vdk-control-cli-1.3.948436673/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.083489 vdk-control-cli-1.3.954631830/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-08-03 12:24:36.083489 vdk-control-cli-1.3.954631830/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2023-08-03 12:24:36.083489 vdk-control-cli-1.3.954631830/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.071489 vdk-control-cli-1.3.954631830/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.071489 vdk-control-cli-1.3.954631830/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.071489 vdk-control-cli-1.3.954631830/src/vdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.071489 vdk-control-cli-1.3.954631830/src/vdk/api/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.075489 vdk-control-cli-1.3.954631830/src/vdk/api/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/api/control/plugin/markers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/api/control/plugin/specs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.071489 vdk-control-cli-1.3.954631830/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.075489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.071489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.075489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/common_group/
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/common_group/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.075489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/info_group/
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/info_group/info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.079489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/
+-rw-rw-rw-   0 root         (0) root         (0)    12776 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/create.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     7206 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/deploy_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14285 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     5129 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/download_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/download_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    12207 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     8735 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/list.py
+-rw-rw-rw-   0 root         (0) root         (0)    11314 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)    12010 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     3403 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/show.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.079489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/login_group/
+-rw-rw-rw-   0 root         (0) root         (0)     6510 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/login_group/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.079489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/logout_group/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/logout_group/logout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.079489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/version_group/
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/version_group/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.079489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/configuration/default_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/configuration/defaults_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/configuration/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9551 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/configuration/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.079489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/exception/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/exception/vdk_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.079489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/job_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/job_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.079489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/sample_job/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/sample_job/10_sql_step.sql
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/sample_job/20_python_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/sample_job/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2902 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/sample_job/config.ini
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/sample_job/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3666 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.079489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/plugin/control_plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.083489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/rest_lib/
+-rw-rw-rw-   0 root         (0) root         (0)     3239 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/rest_lib/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/rest_lib/rest_client_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.083489 vdk-control-cli-1.3.954631830/src/vdk/internal/control/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     7297 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/utils/cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/utils/control_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4587 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/utils/output_printer.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-08-03 12:24:18.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/utils/version_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-08-03 12:24:23.000000 vdk-control-cli-1.3.954631830/src/vdk/internal/control/vdk_control_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 12:24:36.083489 vdk-control-cli-1.3.954631830/src/vdk_control_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-08-03 12:24:36.000000 vdk-control-cli-1.3.954631830/src/vdk_control_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-08-03 12:24:36.000000 vdk-control-cli-1.3.954631830/src/vdk_control_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 12:24:36.000000 vdk-control-cli-1.3.954631830/src/vdk_control_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-08-03 12:24:36.000000 vdk-control-cli-1.3.954631830/src/vdk_control_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 12:24:36.000000 vdk-control-cli-1.3.954631830/src/vdk_control_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      185 2023-08-03 12:24:36.000000 vdk-control-cli-1.3.954631830/src/vdk_control_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-08-03 12:24:36.000000 vdk-control-cli-1.3.954631830/src/vdk_control_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-08-03 12:24:23.000000 vdk-control-cli-1.3.954631830/version.txt
```

### Comparing `vdk-control-cli-1.3.948436673/PKG-INFO` & `vdk-control-cli-1.3.954631830/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.948436673
+Version: 1.3.954631830
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.948436673/README.md` & `vdk-control-cli-1.3.954631830/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/setup.cfg` & `vdk-control-cli-1.3.954631830/setup.cfg`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/api/control/plugin/markers.py` & `vdk-control-cli-1.3.954631830/src/vdk/api/control/plugin/markers.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/api/control/plugin/specs.py` & `vdk-control-cli-1.3.954631830/src/vdk/api/control/plugin/specs.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/common_group/default.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/common_group/default.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/info_group/info.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/info_group/info.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/create.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/create.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/delete.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/deploy_cli.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/download_job.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/download_job.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/download_key.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/download_key.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/execute.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/execute.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/list.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/list.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/properties.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/properties.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/secrets.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/secrets.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 @unique
 class SecretOperation(Enum):
     """
     An enum used to store the types of secrets operations
     """
 
     SET = "set"
+    SET_PROMPT = "set_prompt"  # nosec
     GET = "get"
 
 
 class JobSecrets:
     def __init__(
         self,
         rest_api_url: str,
@@ -179,16 +180,20 @@
 
      \b
      # Set single secret with key "my-key" and value "my-value". If no value is passed
      you'll get prompted so it's not printed on the screen.
      vdk secrets --set my-key "my-value"
 
      \b
+     # Will prompt for the value so it's not printed on the screen.
+     vdk secrets --set-prompt "my-secret"
+
+     \b
      # Update multiple secrets at once.
-     vdk secrets --set "key1" "value1" --set "key2" "value2" --set "secret1" --set "secret2"
+     vdk secrets --set "key1" "value1" --set "key2" "value2" --set-prompt "secret1" --set-prompt  "secret2"
 
      \b
      # Use backslash \\ to set them on multiple lines
      vdk secrets \\
         --set "key1" "value1" \\
         --set "key2" "value2"
 
@@ -225,14 +230,21 @@
     multiple=True,
     help="Set key value secret. "
     "If secret with same key exists we will override it but we will try to preserve the type."
     "Entirely new secrets will be set with string type"
     "You can set multiple secrets by using --set multiple times",
 )
 @click.option(
+    "--set-prompt",
+    multiple=True,
+    type=click.STRING,
+    help="Set a secret by only passing a key without a value and enter it when prompted."
+    "The difference from --set is that it will be prompted and input would be masked. ",
+)
+@click.option(
     "--delete",
     nargs=1,
     type=click.STRING,
     multiple=True,
     help="Delete a secret with the given key. "
     "You can delete multiple secrets by using --delete multiple times",
 )
@@ -255,42 +267,43 @@
 @cli_utils.rest_api_url_option()
 @cli_utils.output_option()
 @cli_utils.check_required_parameters
 def secrets_command(
     name: str,
     team: str,
     set: Tuple[str, str],  # pylint: disable=redefined-builtin
+    set_prompt: Tuple[str, str],  # pylint: disable=redefined-builtin
     delete: Tuple[str],
     delete_all_job_secrets: bool,
     overwrite_all_job_secrets: _io.BufferedReader,
     get: str,
     list: bool,  # pylint: disable=redefined-builtin
     rest_api_url: str,
     output: OutputFormat,
 ):
-    if (set or delete) and (get or list):
+    if (set or delete or set_prompt) and (get or list):
         raise VDKException(
             what="Invalid arguments",
-            why="Wrong input. Cannot pass --get or --list at the same time as --set and --delete.",
+            why="Wrong input. Cannot pass --get or --list at the same time as --set, --set-prompt and --delete.",
             consequence="Command will abort with error.",
             countermeasure="Fix passed arguments such that get/list are not passed in the same time as set/delete.",
         )
     if get and list:
         raise VDKException(
             what="Invalid arguments",
             why="Wrong input. Cannot pass --get at the same time as --list. Choose one of the two.",
             consequence="Command will abort with error",
             countermeasure="Fix passed arguments such that only --list or only --get are used.",
         )
     log.debug(
         f"secrets passed options: name: {name}, team: {team}, "
-        f"set: {set}, get: {get}, list: {list}, delete: {delete} "
+        f"set: {set}, set_prompt: {set_prompt}, get: {get}, list: {list}, delete: {delete} "
         f"rest_api_url: {rest_api_url}, output: {output}"
     )
-    key_value_pairs = _get_key_value_pairs(set)
+    key_value_pairs = _get_key_value_pairs(set, set_prompt)
     cmd = JobSecrets(rest_api_url, name, team, output)
     if key_value_pairs:
         cmd.update_secrets(key_value_pairs)
     if delete:
         cmd.delete_keys(delete)
     if delete_all_job_secrets:
         cmd.delete_all_job_secrets()
@@ -308,17 +321,17 @@
                 "Expected valid json for secrets overwrite.",
                 "JSON was not valid; error is " + str(e),
                 "Operation is aborted. Nothing has been changed.",
                 "Fix the file to be a valid json and re-try again.",
             )
 
 
-def _get_key_value_pairs(set):  # pylint: disable=redefined-builtin
+def _get_key_value_pairs(set, set_prompt):  # pylint: disable=redefined-builtin
     key_value_pairs = {}
     if set:
         for key, value in set:
-            if value:
-                key_value_pairs[key] = value
-            else:
-                value = click.prompt(f"{key}", hide_input=True)
-                key_value_pairs[key] = value
+            key_value_pairs[key] = value
+    if set_prompt:
+        for key in set_prompt:
+            value = click.prompt(f"{key}", hide_input=True)
+            key_value_pairs[key] = value
     return key_value_pairs
```

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/job/show.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/job/show.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/login_group/login.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/login_group/login.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/command_groups/version_group/version.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/command_groups/version_group/version.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/configuration/defaults_config.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/configuration/defaults_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/configuration/log_config.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/configuration/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/configuration/vdk_config.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/configuration/vdk_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/exception/vdk_exception.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/exception/vdk_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/job_archive.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/job_archive.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/job_config.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/job_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/sample_job/10_sql_step.sql` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/sample_job/10_sql_step.sql`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/sample_job/20_python_step.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/sample_job/20_python_step.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/sample_job/README.md` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/job/sample_job/config.ini` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/job/sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/main.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/main.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/plugin/control_plugin_manager.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/plugin/control_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/rest_lib/factory.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/rest_lib/factory.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/rest_lib/rest_client_errors.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/rest_lib/rest_client_errors.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/utils/cli_utils.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/utils/control_utils.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/utils/control_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/utils/output_printer.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/utils/output_printer.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk/internal/control/utils/version_utils.py` & `vdk-control-cli-1.3.954631830/src/vdk/internal/control/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.948436673/src/vdk_control_cli.egg-info/PKG-INFO` & `vdk-control-cli-1.3.954631830/src/vdk_control_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.948436673
+Version: 1.3.954631830
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.948436673/src/vdk_control_cli.egg-info/SOURCES.txt` & `vdk-control-cli-1.3.954631830/src/vdk_control_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

