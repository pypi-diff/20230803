# Comparing `tmp/pdpp-0.4.3.tar.gz` & `tmp/pdpp-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pierson/netlab/pdpp/dist/tmpodblqrgu/pdpp-0.4.3.tar", last modified: Wed Apr 21 20:51:05 2021, max compression
+gzip compressed data, was "pdpp-0.4.5.tar", last modified: Thu Aug  3 18:52:00 2023, max compression
```

## Comparing `pdpp-0.4.3.tar` & `pdpp-0.4.5.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-21 20:51:05.311252 pdpp-0.4.3/
--rwxrwxr-x   0 root         (0) root         (0)     1063 2021-01-19 19:02:33.000000 pdpp-0.4.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      501 2021-04-21 20:51:05.311252 pdpp-0.4.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-21 20:51:05.303252 pdpp-0.4.3/pdpp/
--rwxrwxr-x   0 root         (0) root         (0)        0 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-21 20:51:05.307252 pdpp-0.4.3/pdpp/automation/
--rwxrwxr-x   0 root         (0) root         (0)        0 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/automation/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)      165 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/automation/doit_run.py
--rwxrwxr-x   0 root         (0) root         (0)     2393 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/automation/link_task.py
--rwxrwxr-x   0 root         (0) root         (0)      459 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/automation/mylinker.py
--rwxrwxr-x   0 root         (0) root         (0)     1844 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/automation/task_creator.py
--rwxrwxr-x   0 root         (0) root         (0)     1115 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/automation/task_enabler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-21 20:51:05.307252 pdpp-0.4.3/pdpp/languages/
--rwxrwxr-x   0 root         (0) root         (0)        0 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/languages/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      612 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/languages/extension_parser.py
--rw-rw-r--   0 root         (0) root         (0)       92 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/languages/language_enum.py
--rw-rw-r--   0 root         (0) root         (0)      370 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/languages/language_parser.py
--rw-rw-r--   0 root         (0) root         (0)      650 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/languages/runners.py
--rwxrwxr-x   0 root         (0) root         (0)     5257 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-21 20:51:05.307252 pdpp-0.4.3/pdpp/questions/
--rwxrwxr-x   0 root         (0) root         (0)      163 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/questions/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)      873 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/questions/question_0.py
--rwxrwxr-x   0 root         (0) root         (0)     1668 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/questions/question_1.py
--rwxrwxr-x   0 root         (0) root         (0)     2914 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/questions/question_2.py
--rwxrwxr-x   0 root         (0) root         (0)     1417 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/questions/question_3.py
--rwxrwxr-x   0 root         (0) root         (0)     2042 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/questions/question_4.py
--rw-rw-r--   0 root         (0) root         (0)     1113 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/questions/question_extant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-21 20:51:05.307252 pdpp-0.4.3/pdpp/styles/
--rwxrwxr-x   0 root         (0) root         (0)        0 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/styles/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1716 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/styles/graph_style.py
--rwxrwxr-x   0 root         (0) root         (0)      593 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/styles/prompt_style.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-21 20:51:05.311252 pdpp-0.4.3/pdpp/tasks/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/tasks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2430 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/tasks/base_task.py
--rw-rw-r--   0 root         (0) root         (0)     1692 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/tasks/custom_task.py
--rw-rw-r--   0 root         (0) root         (0)     1136 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/tasks/export_task.py
--rw-rw-r--   0 root         (0) root         (0)     1286 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/tasks/import_task.py
--rw-rw-r--   0 root         (0) root         (0)     1666 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/tasks/standard_task.py
--rw-rw-r--   0 root         (0) root         (0)     1466 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/tasks/sub_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-21 20:51:05.311252 pdpp-0.4.3/pdpp/templates/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/templates/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2323 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/templates/create_gitignore.py
--rw-rw-r--   0 root         (0) root         (0)      542 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/templates/create_in_out_src.py
--rw-rw-r--   0 root         (0) root         (0)      502 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/templates/dep_dataclass.py
--rw-rw-r--   0 root         (0) root         (0)      210 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/templates/dodo_template.py
--rw-rw-r--   0 root         (0) root         (0)      575 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/templates/populate_new_project.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-21 20:51:05.311252 pdpp-0.4.3/pdpp/utils/
--rwxrwxr-x   0 root         (0) root         (0)        0 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1918 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/utils/directory_test.py
--rw-rw-r--   0 root         (0) root         (0)      313 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/utils/execute_at_target.py
--rwxrwxr-x   0 root         (0) root         (0)     7336 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/utils/graph_dependencies.py
--rw-rw-r--   0 root         (0) root         (0)      131 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/utils/ignorelist.py
--rwxrwxr-x   0 root         (0) root         (0)     1171 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/utils/immediate_link.py
--rwxrwxr-x   0 root         (0) root         (0)      252 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/utils/rem_slash.py
--rwxrwxr-x   0 root         (0) root         (0)     2241 2021-01-19 19:02:33.000000 pdpp-0.4.3/pdpp/utils/task_directory_test.py
--rw-rw-r--   0 root         (0) root         (0)      513 2021-04-21 20:42:33.000000 pdpp-0.4.3/pdpp/utils/yaml_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-21 20:51:05.307252 pdpp-0.4.3/pdpp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      501 2021-04-21 20:51:05.000000 pdpp-0.4.3/pdpp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1466 2021-04-21 20:51:05.000000 pdpp-0.4.3/pdpp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-21 20:51:05.000000 pdpp-0.4.3/pdpp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2021-04-21 20:51:05.000000 pdpp-0.4.3/pdpp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       99 2021-04-21 20:51:05.000000 pdpp-0.4.3/pdpp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2021-04-21 20:51:05.000000 pdpp-0.4.3/pdpp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-21 20:51:05.311252 pdpp-0.4.3/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)      812 2021-04-21 20:50:55.000000 pdpp-0.4.3/setup.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 18:52:00.899050 pdpp-0.4.5/
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1063 2023-03-30 23:25:51.000000 pdpp-0.4.5/LICENSE.txt
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      471 2023-08-03 18:52:00.899050 pdpp-0.4.5/PKG-INFO
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1355 2023-08-03 18:47:40.000000 pdpp-0.4.5/README.md
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 18:52:00.879050 pdpp-0.4.5/pdpp/
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/__init__.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 18:52:00.883050 pdpp-0.4.5/pdpp/automation/
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/automation/__init__.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)      165 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/automation/doit_run.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     2393 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/automation/link_task.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)      459 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/automation/mylinker.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1838 2022-10-17 20:28:37.000000 pdpp-0.4.5/pdpp/automation/task_creator.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1115 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/automation/task_enabler.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 18:52:00.883050 pdpp-0.4.5/pdpp/languages/
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/languages/__init__.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      612 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/languages/extension_parser.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)       92 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/languages/language_enum.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      370 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/languages/language_parser.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      650 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/languages/runners.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     5278 2022-10-17 20:25:25.000000 pdpp-0.4.5/pdpp/main.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 18:52:00.887050 pdpp-0.4.5/pdpp/questions/
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)      163 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/questions/__init__.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)      873 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/questions/question_0.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1668 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/questions/question_1.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     2914 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/questions/question_2.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1417 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/questions/question_3.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1944 2023-07-26 20:34:29.000000 pdpp-0.4.5/pdpp/questions/question_4.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1113 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/questions/question_extant.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 18:52:00.887050 pdpp-0.4.5/pdpp/styles/
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/styles/__init__.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1716 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/styles/graph_style.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)      593 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/styles/prompt_style.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 18:52:00.891050 pdpp-0.4.5/pdpp/tasks/
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/tasks/__init__.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     2430 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/tasks/base_task.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1692 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/tasks/custom_task.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1136 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/tasks/export_task.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1286 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/tasks/import_task.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1666 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/tasks/standard_task.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1466 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/tasks/sub_task.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 18:52:00.895050 pdpp-0.4.5/pdpp/templates/
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/templates/__init__.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     2323 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/templates/create_gitignore.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      542 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/templates/create_in_out_src.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      502 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/templates/dep_dataclass.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      210 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/templates/dodo_template.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      575 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/templates/populate_new_project.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 18:52:00.899050 pdpp-0.4.5/pdpp/utils/
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/utils/__init__.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1918 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/utils/directory_test.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      313 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/utils/execute_at_target.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     7336 2022-10-17 21:03:33.000000 pdpp-0.4.5/pdpp/utils/graph_dependencies.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      131 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/utils/ignorelist.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1171 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/utils/immediate_link.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)      252 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/utils/rem_slash.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     2241 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/utils/task_directory_test.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      513 2022-10-17 19:41:09.000000 pdpp-0.4.5/pdpp/utils/yaml_task.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 18:52:00.879050 pdpp-0.4.5/pdpp.egg-info/
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      471 2023-08-03 18:52:00.000000 pdpp-0.4.5/pdpp.egg-info/PKG-INFO
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1476 2023-08-03 18:52:00.000000 pdpp-0.4.5/pdpp.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)        1 2023-08-03 18:52:00.000000 pdpp-0.4.5/pdpp.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)       40 2023-08-03 18:52:00.000000 pdpp-0.4.5/pdpp.egg-info/entry_points.txt
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)       99 2023-08-03 18:52:00.000000 pdpp-0.4.5/pdpp.egg-info/requires.txt
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)        5 2023-08-03 18:52:00.000000 pdpp-0.4.5/pdpp.egg-info/top_level.txt
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)       38 2023-08-03 18:52:00.899050 pdpp-0.4.5/setup.cfg
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)      884 2023-07-31 23:51:36.000000 pdpp-0.4.5/setup.py
```

### Comparing `pdpp-0.4.3/LICENSE.txt` & `pdpp-0.4.5/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018 NetLab
+Copyright (c) 2023 NetLab
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pdpp-0.4.3/pdpp/automation/link_task.py` & `pdpp-0.4.5/pdpp/automation/link_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/automation/task_creator.py` & `pdpp-0.4.5/pdpp/automation/task_creator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from pdpp.utils.directory_test import get_pdpp_tasks
 from typing import List
 from pdpp.tasks.base_task import BaseTask
 from pdpp.automation.link_task import make_link_task
 
 
 def find_dependencies_from_others(task: BaseTask, loaded_tasks: List[BaseTask]) -> List[str]:
-
     dependencies = []
 
     for other_task in loaded_tasks:
         dependencies.extend(other_task.provide_dependencies(task))
 
     return [d for d in set(dependencies)] # This is just a hackier way of unpacking everything; pylance type-checking REALLY didn't like list(set(dependencies)) for some reason
  
 def gen_many_tasks():
-    
     # 1. Get all of the tasks in the current scope
     loaded_tasks = get_pdpp_tasks()
 
     # 2. Create a list of all the disabled tasks loaded in task #1
     disabled_list = [t.target_dir for t in loaded_tasks if not t.enabled]
 
     for task in loaded_tasks:
```

### Comparing `pdpp-0.4.3/pdpp/automation/task_enabler.py` & `pdpp-0.4.5/pdpp/automation/task_enabler.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/languages/extension_parser.py` & `pdpp-0.4.5/pdpp/languages/extension_parser.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/languages/runners.py` & `pdpp-0.4.5/pdpp/languages/runners.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/main.py` & `pdpp-0.4.5/pdpp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 
 GRAPH_STYLE_LIST: List[Type[base_graph_style]] = [default_graph_style, greyscale_graph_style] 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 FILES_LIST = ['png', 'pdf', 'jpg']
 
 
 @click.group()
-def main():
+def main() -> None:
     """A command line tool to automate the use of the Principled Data Processing methodology for reproducibility."""
     pass
 
 
 @main.command(short_help="Prepares a directory to become a pdpp project")
-def init():
-
+def init() -> None:      
     from pdpp.templates.populate_new_project import populate_new_project
     populate_new_project()
 
 
 @main.command(short_help="""Create a new task directory
 """,
               context_settings=CONTEXT_SETTINGS)
```

### Comparing `pdpp-0.4.3/pdpp/questions/question_0.py` & `pdpp-0.4.5/pdpp/questions/question_0.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/questions/question_1.py` & `pdpp-0.4.5/pdpp/questions/question_1.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/questions/question_2.py` & `pdpp-0.4.5/pdpp/questions/question_2.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/questions/question_3.py` & `pdpp-0.4.5/pdpp/questions/question_3.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/questions/question_4.py` & `pdpp-0.4.5/pdpp/questions/question_4.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from pdpp.languages.language_enum import Language
 from pdpp.languages.extension_parser import extension_parser
 
 
 def q4(task: BaseTask) -> str:
     """
     This question is used to determine the language of the source code this task will run. 
-    This needs documentation badly, because I'm not entirely certain what it does at the moment.
     """
 
     click_clear()
 
     language_list = extension_parser(task)
 
     if len(set(language_list)) != 1 or '???' in language_list:
```

### Comparing `pdpp-0.4.3/pdpp/questions/question_extant.py` & `pdpp-0.4.5/pdpp/questions/question_extant.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/styles/graph_style.py` & `pdpp-0.4.5/pdpp/styles/graph_style.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/styles/prompt_style.py` & `pdpp-0.4.5/pdpp/styles/prompt_style.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/tasks/base_task.py` & `pdpp-0.4.5/pdpp/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/tasks/custom_task.py` & `pdpp-0.4.5/pdpp/tasks/custom_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/tasks/export_task.py` & `pdpp-0.4.5/pdpp/tasks/export_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/tasks/import_task.py` & `pdpp-0.4.5/pdpp/tasks/import_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/tasks/standard_task.py` & `pdpp-0.4.5/pdpp/tasks/standard_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/tasks/sub_task.py` & `pdpp-0.4.5/pdpp/tasks/sub_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/templates/create_gitignore.py` & `pdpp-0.4.5/pdpp/templates/create_gitignore.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/templates/create_in_out_src.py` & `pdpp-0.4.5/pdpp/templates/create_in_out_src.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/templates/populate_new_project.py` & `pdpp-0.4.5/pdpp/templates/populate_new_project.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/utils/directory_test.py` & `pdpp-0.4.5/pdpp/utils/directory_test.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/utils/graph_dependencies.py` & `pdpp-0.4.5/pdpp/utils/graph_dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     toPdot = nx.drawing.nx_pydot.to_pydot # type:ignore
     N:pydot.Dot = toPdot(G)
 
     N.obj_dict['attributes']['concentrate'] = 'true' # Combines edges
     N.obj_dict['attributes']['rankdir'] = 'LR' # Runs graph left-to-right
     N.obj_dict['attributes']['dpi'] = 300
 
-    # Add all source nodes to supgraphs with their tasks so that they are 
+    # Add all source nodes to subgraphs with their tasks so that they are 
     # displayed on the same rank:
 
     for edge in N.get_edge_list():
         if N.get_node(edge.get_source())[0].get('categ') == "source":
             S = pydot.Subgraph(rank = 'same')
             S.add_node(N.get_node(edge.get_source())[0])
             S.add_node(N.get_node(edge.get_destination())[0])
```

### Comparing `pdpp-0.4.3/pdpp/utils/immediate_link.py` & `pdpp-0.4.5/pdpp/utils/immediate_link.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/utils/task_directory_test.py` & `pdpp-0.4.5/pdpp/utils/task_directory_test.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp/utils/yaml_task.py` & `pdpp-0.4.5/pdpp/utils/yaml_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.3/pdpp.egg-info/SOURCES.txt` & `pdpp-0.4.5/pdpp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE.txt
+README.md
 setup.py
 pdpp/__init__.py
 pdpp/main.py
 pdpp.egg-info/PKG-INFO
 pdpp.egg-info/SOURCES.txt
 pdpp.egg-info/dependency_links.txt
 pdpp.egg-info/entry_points.txt
```

### Comparing `pdpp-0.4.3/setup.py` & `pdpp-0.4.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pdpp",
-    version="0.4.3",
-    install_requires=['Click>=7.0', 'doit>=0.31.1', 'networkx>=2.2', 'graphviz>=0.10.1', 'pydot>=1.4.1', 'questionary>=1.0.2', 'pyyaml>=5.3'],
+    version="0.4.5",
+    install_requires=[
+        'Click>=7.0', 
+        'doit>=0.31.1', 
+        'networkx>=2.2', 
+        'graphviz>=0.10.1', 
+        'pydot>=1.4.1', 
+        'questionary>=1.0.2', 
+        'pyyaml>=5.3'
+        ],
     packages=find_packages(),
 	include_package_data=True,
     entry_points = """
         [console_scripts]
         pdpp=pdpp.main:main
         """,
```

