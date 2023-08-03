# Comparing `tmp/s4-clarity-1.4.2.tar.gz` & `tmp/s4-clarity-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s4-clarity-1.4.2.tar", last modified: Fri Jul 28 22:22:47 2023, max compression
+gzip compressed data, was "s4-clarity-1.5.0.tar", last modified: Thu Aug  3 16:13:02 2023, max compression
```

## Comparing `s4-clarity-1.4.2.tar` & `s4-clarity-1.5.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.500718 s4-clarity-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-28 22:22:47.500718 s4-clarity-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.488718 s4-clarity-1.4.2/s4/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.492718 s4-clarity-1.4.2/s4/clarity/
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.496718 s4-clarity-1.4.2/s4/clarity/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/element.py
--rw-r--r--   0 runner    (1001) docker     (123)    16591 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/fakesession.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/lazy_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    27938 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/stepfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/udffactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9944 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.496718 s4-clarity-1.4.2/s4/clarity/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/configuration/process_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/configuration/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/configuration/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/configuration/udf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/configuration/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/control_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/iomaps.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/lab.py
--rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/process.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/reagent_kit.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/reagent_lot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/reagent_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/researcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.496718 s4-clarity-1.4.2/s4/clarity/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/derived_sample_automation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/epp_output_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/file_argument_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/genericscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/htmllogging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/stepepp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/triggered_step_epp.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/user_message_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/workflow_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.500718 s4-clarity-1.4.2/s4/clarity/steputils/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/steputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/steputils/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/steputils/copyudfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/steputils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/steputils/placement_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/steputils/step_average_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24069 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/steputils/step_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.500718 s4-clarity-1.4.2/s4/clarity/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/utils/artifact_ancestry.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/utils/date_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/utils/sorting_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/utils/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.500718 s4-clarity-1.4.2/s4_clarity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-28 22:22:47.000000 s4-clarity-1.4.2/s4_clarity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-28 22:22:47.000000 s4-clarity-1.4.2/s4_clarity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:22:47.000000 s4-clarity-1.4.2/s4_clarity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 22:22:47.000000 s4-clarity-1.4.2/s4_clarity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-28 22:22:47.000000 s4-clarity-1.4.2/s4_clarity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 22:22:47.500718 s4-clarity-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:13:02.555590 s4-clarity-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-08-03 16:13:02.555590 s4-clarity-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:13:02.547590 s4-clarity-1.5.0/s4/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:13:02.551590 s4-clarity-1.5.0/s4/clarity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:13:02.551590 s4-clarity-1.5.0/s4/clarity/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/_internal/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16591 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/_internal/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/_internal/fakesession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/_internal/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/_internal/lazy_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27938 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/_internal/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/_internal/stepfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/_internal/udffactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9944 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:13:02.551590 s4-clarity-1.5.0/s4/clarity/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/configuration/process_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/configuration/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/configuration/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/configuration/udf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/configuration/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/control_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/iomaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/reagent_kit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/reagent_lot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/reagent_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/researcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:13:02.551590 s4-clarity-1.5.0/s4/clarity/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/scripts/derived_sample_automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/scripts/epp_output_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/scripts/file_argument_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/scripts/genericscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/scripts/htmllogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/scripts/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/scripts/stepepp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/scripts/triggered_step_epp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/scripts/user_message_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/scripts/workflow_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:13:02.551590 s4-clarity-1.5.0/s4/clarity/steputils/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/steputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/steputils/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/steputils/copyudfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/steputils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/steputils/placement_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/steputils/step_average_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24453 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/steputils/step_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:13:02.555590 s4-clarity-1.5.0/s4/clarity/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/utils/artifact_ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/utils/date_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/utils/sorting_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/utils/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/s4/clarity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:13:02.555590 s4-clarity-1.5.0/s4_clarity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-08-03 16:13:02.000000 s4-clarity-1.5.0/s4_clarity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-03 16:13:02.000000 s4-clarity-1.5.0/s4_clarity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:13:02.000000 s4-clarity-1.5.0/s4_clarity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 16:13:02.000000 s4-clarity-1.5.0/s4_clarity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-03 16:13:02.000000 s4-clarity-1.5.0/s4_clarity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-03 16:13:02.555590 s4-clarity-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-03 16:13:00.000000 s4-clarity-1.5.0/setup.py
```

### Comparing `s4-clarity-1.4.2/LICENSE` & `s4-clarity-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/PKG-INFO` & `s4-clarity-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s4-clarity
-Version: 1.4.2
+Version: 1.5.0
 Summary: A general purpose library for interacting with Clarity LIMS
 Home-page: https://github.com/SemaphoreSolutions/s4-clarity-lib
 Author: Semaphore Solutions
 Author-email: info@semaphoresolutions.ca
 Project-URL: Documentation, https://readthedocs.org/projects/s4-clarity-lib
 Project-URL: Source, https://github.com/SemaphoreSolutions/s4-clarity-lib
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `s4-clarity-1.4.2/README.rst` & `s4-clarity-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/__init__.py` & `s4-clarity-1.5.0/s4/clarity/__init__.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/_internal/__init__.py` & `s4-clarity-1.5.0/s4/clarity/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/_internal/element.py` & `s4-clarity-1.5.0/s4/clarity/_internal/element.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/_internal/factory.py` & `s4-clarity-1.5.0/s4/clarity/_internal/factory.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/_internal/fakesession.py` & `s4-clarity-1.5.0/s4/clarity/_internal/fakesession.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/_internal/fields.py` & `s4-clarity-1.5.0/s4/clarity/_internal/fields.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/_internal/lazy_property.py` & `s4-clarity-1.5.0/s4/clarity/_internal/lazy_property.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/_internal/props.py` & `s4-clarity-1.5.0/s4/clarity/_internal/props.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/_internal/stepfactory.py` & `s4-clarity-1.5.0/s4/clarity/_internal/stepfactory.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/_internal/udffactory.py` & `s4-clarity-1.5.0/s4/clarity/_internal/udffactory.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/artifact.py` & `s4-clarity-1.5.0/s4/clarity/artifact.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/configuration/__init__.py` & `s4-clarity-1.5.0/s4/clarity/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/configuration/process_type.py` & `s4-clarity-1.5.0/s4/clarity/configuration/process_type.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/configuration/stage.py` & `s4-clarity-1.5.0/s4/clarity/configuration/stage.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/configuration/udf.py` & `s4-clarity-1.5.0/s4/clarity/configuration/udf.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/configuration/workflow.py` & `s4-clarity-1.5.0/s4/clarity/configuration/workflow.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/console.py` & `s4-clarity-1.5.0/s4/clarity/console.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/container.py` & `s4-clarity-1.5.0/s4/clarity/container.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     is_alpha = subnode_property("is-alpha", types.BOOLEAN)
     offset = subnode_property("offset", types.NUMERIC)  # type: float
     size = subnode_property("size", types.NUMERIC)  # type: float
 
     @lazy_property
     def dimension_range(self):
         """
-        List of the labels for the given dimension (row or column)
+        List of the labels for the given dimension
 
         :return: list[int]|list[str]
         """
 
         # Cast these to integers from floats to avoid deprecation warnings from range.
         start = int(self.offset)
         end = int(self.offset + self.size)
@@ -38,14 +38,18 @@
         if self.is_alpha:
             return chr(65 + index + int(self.offset))
         else:
             return str(index + int(self.offset))
 
 
 class ContainerType(ClarityElement):
+    """
+    A class to handle container types, with helper functions to create and encode well positions
+    For the purposes of this class, the y-dimension is considered the columns, and the x-dimension is considered the rows.
+    """
     UNIVERSAL_TAG = "{http://genologics.com/ri/containertype}container-type"
 
     is_tube = subnode_property("is-tube", types.BOOLEAN)  # type: bool
     x_dimension = subnode_element(ContainerDimension, "x-dimension")  # type: ContainerDimension
     y_dimension = subnode_element(ContainerDimension, "y-dimension")  # type: ContainerDimension
 
     def well_to_rc(self, well):
@@ -76,34 +80,38 @@
         :param rc: The zero based index of the row and the column.
         :type rc: tuple[int]
         :return: A Clarity formatted well position
         :rtype: str
         """
         return "%s:%s" % (self.y_dimension.as_label(rc[0]), self.x_dimension.as_label(rc[1]))
 
-    def row_order_wells(self):
+    def row_major_order_wells(self):
         """
-        Wells in row order, e.g., A:1, B:1, ...
-        Unavailable wells are omitted
+        Returns wells in the container type in row major order.
+        This will return the wells ordered: ["y1:x1", "y1:x2", "y1:x3", [...], "y1,xn", "y2:x1", "y2:x2", [...]]
+
+        Unavailable wells are omitted.
 
         :rtype: list[str]
         """
         l = []
         for y in self.y_dimension.dimension_range:
             for x in self.x_dimension.dimension_range:
                 well_name = "%s:%s" % (str(y), str(x))
 
                 if well_name not in self.unavailable_wells:
                     l.append(well_name)
         return l
 
-    def column_order_wells(self):
+    def column_major_order_wells(self):
         """
-        Wells in column order, e.g., A:1, A:2, ...
-        Unavailable wells are omitted
+        Returns wells in the container type in column major order.
+        This will return the wells ordered: ["y1:x1", "y2:x1", "y3:x1", [...], "yn:x1", "y1:x2", "y2:x2", [...]]
+
+        Unavailable wells are omitted.
 
         :rtype: list[str]
         """
         l = []
         for x in self.x_dimension.dimension_range:
             for y in self.y_dimension.dimension_range:
                 well_name = "%s:%s" % (str(y), str(x))
@@ -123,14 +131,26 @@
     @lazy_property
     def total_capacity(self):
         """
         :type: int
         """
         return len(self.x_dimension.dimension_range) * len(self.y_dimension.dimension_range) - len(self.unavailable_wells)
 
+    def row_order_wells(self):
+        """
+        :deprecated: use :class:`ContainerType.row_major_order_wells()` instead.
+        """
+        return self.row_major_order_wells()
+
+    def column_order_wells(self):
+        """
+        :deprecated: use :class:`ContainerType.column_major_order_wells()` instead.
+        """
+        return self.column_major_order_wells()
+
     def x_dimension_range(self):
         """
         :deprecated: use :class:`ContainerType.x_dimension.dimension_range` instead
         """
         return self.x_dimension.dimension_range
 
     def y_dimension_range(self):
```

### Comparing `s4-clarity-1.4.2/s4/clarity/control_type.py` & `s4-clarity-1.5.0/s4/clarity/control_type.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/exception.py` & `s4-clarity-1.5.0/s4/clarity/exception.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/file.py` & `s4-clarity-1.5.0/s4/clarity/file.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/instrument.py` & `s4-clarity-1.5.0/s4/clarity/instrument.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/iomaps.py` & `s4-clarity-1.5.0/s4/clarity/iomaps.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/lims.py` & `s4-clarity-1.5.0/s4/clarity/lims.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/process.py` & `s4-clarity-1.5.0/s4/clarity/process.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/project.py` & `s4-clarity-1.5.0/s4/clarity/project.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/queue.py` & `s4-clarity-1.5.0/s4/clarity/queue.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/reagent_kit.py` & `s4-clarity-1.5.0/s4/clarity/reagent_kit.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/reagent_lot.py` & `s4-clarity-1.5.0/s4/clarity/reagent_lot.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/reagent_type.py` & `s4-clarity-1.5.0/s4/clarity/reagent_type.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/researcher.py` & `s4-clarity-1.5.0/s4/clarity/researcher.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/role.py` & `s4-clarity-1.5.0/s4/clarity/role.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/routing.py` & `s4-clarity-1.5.0/s4/clarity/routing.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/sample.py` & `s4-clarity-1.5.0/s4/clarity/sample.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/scripts/__init__.py` & `s4-clarity-1.5.0/s4/clarity/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/scripts/derived_sample_automation.py` & `s4-clarity-1.5.0/s4/clarity/scripts/derived_sample_automation.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/scripts/epp_output_formatter.py` & `s4-clarity-1.5.0/s4/clarity/scripts/epp_output_formatter.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/scripts/file_argument_script.py` & `s4-clarity-1.5.0/s4/clarity/scripts/file_argument_script.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/scripts/genericscript.py` & `s4-clarity-1.5.0/s4/clarity/scripts/genericscript.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/scripts/htmllogging.py` & `s4-clarity-1.5.0/s4/clarity/scripts/htmllogging.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/scripts/shell.py` & `s4-clarity-1.5.0/s4/clarity/scripts/shell.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/scripts/stepepp.py` & `s4-clarity-1.5.0/s4/clarity/scripts/stepepp.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/scripts/triggered_step_epp.py` & `s4-clarity-1.5.0/s4/clarity/scripts/triggered_step_epp.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/step.py` & `s4-clarity-1.5.0/s4/clarity/step.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/steputils/actions.py` & `s4-clarity-1.5.0/s4/clarity/steputils/actions.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/steputils/copyudfs.py` & `s4-clarity-1.5.0/s4/clarity/steputils/copyudfs.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/steputils/file_utils.py` & `s4-clarity-1.5.0/s4/clarity/steputils/file_utils.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/steputils/placement_utils.py` & `s4-clarity-1.5.0/s4/clarity/steputils/placement_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,17 +81,17 @@
     number_outputs = len(artifacts)
     number_placed_outputs = 0
 
     # Note: This will not create new containers, only use the ones currently provided.
     containers = step.placements.selected_containers
     for container in containers:
         if order == ROW_ORDER:
-            wells = container.container_type.row_order_wells()
+            wells = container.container_type.row_major_order_wells()
         elif order == COLUMN_ORDER:
-            wells = container.container_type.column_order_wells()
+            wells = container.container_type.column_major_order_wells()
         else:
             raise Exception("Auto Place Error - Unrecognized order type '%s'" % order)
 
         for well in wells:
             output = next(output_iterator, None)
             if output is None:
                 break
```

### Comparing `s4-clarity-1.4.2/s4/clarity/steputils/step_average_utils.py` & `s4-clarity-1.5.0/s4/clarity/steputils/step_average_utils.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/steputils/step_runner.py` & `s4-clarity-1.5.0/s4/clarity/steputils/step_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 
 CONTAINER_TYPE_TUBE = "Tube"
 
 # Step States, each one representing a window in a step
 PLACEMENT_STATE = "Placement"
 ARRANGING_STATE = "Arranging"
 STARTED_STATE = "Started"
+SETUP_STATE = "Step Setup"
 POOLING_STATE = "Pooling"
 ADD_REAGENT_STATE = "Add Reagent"
 RECORD_DETAILS_STATE = "Record Details"
 ASSIGN_NEXT_STEPS_STATE = "Assign Next Steps"
 COMPLETED_STATE = "Completed"
 
 ALL_STEP_STATES = [PLACEMENT_STATE,
                    ARRANGING_STATE,
                    STARTED_STATE,
+                   SETUP_STATE,
                    POOLING_STATE,
                    ADD_REAGENT_STATE,
                    RECORD_DETAILS_STATE,
                    ASSIGN_NEXT_STEPS_STATE,
                    COMPLETED_STATE]
 
 
@@ -89,14 +91,18 @@
         # Override to generate a custom number of replicates for each control.
         return 1
 
     def replicates_for_inputuri(self, input_uri):
         # Override to generate a custom number of replicates for each sample.
         return 1
 
+    def setup(self):
+        # Override this method to implement actions on the step setup screen.
+        pass
+
     def placement(self):
         # Override this method to implement actions on the placement screen.
         pass
 
     def arranging(self):
         # Override this method to implement actions on the arrangement screen.
         pass
@@ -117,46 +123,52 @@
         # Override this method to implement actions on the next steps screen.
         pass
 
     ################################
     # End Virtual Methods
     ################################
 
+    def _run_setup(self):
+        # Runs the Step Setup phase
+        log.info("Starting Step Setup Phase")
+        self.setup()
+        self.step.advance()
+
     def _run_placement(self):
-        # Runs the placement step
+        # Runs the placement phase
         log.info("Starting Placement Phase")
         self.placement()
         self.step.advance()
 
     def _run_arranging(self):
-        # Runs the Arranging step
+        # Runs the Arranging phase
         log.info("Starting Arranging Phase")
         self.arranging()
         # Note: Most versions of Clarity do not support advancing from the Arranging state.
 
     def _run_pooling(self):
-        # Runs the Pooling step
+        # Runs the Pooling phase
         log.info("Starting Pooling Phase")
         self.pooling()
         self.step.advance()
 
     def _run_add_reagent(self):
-        # Runs the Add Reagent step
+        # Runs the Add Reagent phase
         log.info("Starting Add Reagent Phase")
         self.add_reagents_step()
         self.step.advance()
 
     def _run_record_details(self):
-        # Runs the Record Details step
+        # Runs the Record Details phase
         log.info("Starting Record Details Phase")
         self.record_details()
         self.step.advance()
 
     def _run_next_steps(self):
-        # Runs the Assign Next Steps step
+        # Runs the Assign Next Steps phase
         log.info("Starting Assign Next Steps Phase")
         self.next_steps()
         self.step.advance()
 
     def load_existing_step(self, step_limsid):
         """
         Loads an existing step from Clarity into the StepRunner.
@@ -259,14 +271,15 @@
         if goal_state_name not in ALL_STEP_STATES:
             raise StepRunnerException("Invalid goal state: %s" % goal_state_name)
 
         state_map = {
             PLACEMENT_STATE: self._run_placement,
             ARRANGING_STATE: self._run_arranging,
             STARTED_STATE: self._wait_on_started,
+            SETUP_STATE: self._run_setup,
             POOLING_STATE: self._run_pooling,
             ADD_REAGENT_STATE: self._run_add_reagent,
             RECORD_DETAILS_STATE: self._run_record_details,
             ASSIGN_NEXT_STEPS_STATE: self._run_next_steps
         }
 
         previous_state = ""
@@ -314,15 +327,15 @@
 
         new_containers = self.lims.containers.batch_create(
             [self.lims.containers.new(name=output.limsid, container_type=container_type)
              for output in self.step.details.outputs]
         )
 
         for index, output in enumerate(self.step.details.outputs):
-            self.step.placements.create_placement(output, new_containers[index], container_type.row_order_wells()[0])
+            self.step.placements.create_placement(output, new_containers[index], container_type.row_major_order_wells()[0])
 
         self.step.placements.post_and_parse()
         self.step.refresh()
 
     def add_default_reagents(self):
         """
         For every required reagent kit in the step, the first active lot
```

### Comparing `s4-clarity-1.4.2/s4/clarity/types.py` & `s4-clarity-1.5.0/s4/clarity/types.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/utils/__init__.py` & `s4-clarity-1.5.0/s4/clarity/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/utils/artifact_ancestry.py` & `s4-clarity-1.5.0/s4/clarity/utils/artifact_ancestry.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/utils/date_util.py` & `s4-clarity-1.5.0/s4/clarity/utils/date_util.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4/clarity/utils/ssh.py` & `s4-clarity-1.5.0/s4/clarity/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/s4_clarity.egg-info/PKG-INFO` & `s4-clarity-1.5.0/s4_clarity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s4-clarity
-Version: 1.4.2
+Version: 1.5.0
 Summary: A general purpose library for interacting with Clarity LIMS
 Home-page: https://github.com/SemaphoreSolutions/s4-clarity-lib
 Author: Semaphore Solutions
 Author-email: info@semaphoresolutions.ca
 Project-URL: Documentation, https://readthedocs.org/projects/s4-clarity-lib
 Project-URL: Source, https://github.com/SemaphoreSolutions/s4-clarity-lib
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `s4-clarity-1.4.2/s4_clarity.egg-info/SOURCES.txt` & `s4-clarity-1.5.0/s4_clarity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.2/setup.py` & `s4-clarity-1.5.0/setup.py`

 * *Files identical despite different names*

