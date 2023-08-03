# Comparing `tmp/meggie-1.5.1.tar.gz` & `tmp/meggie-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meggie-1.5.1.tar", last modified: Wed Apr  5 17:45:27 2023, max compression
+gzip compressed data, was "meggie-1.5.2.tar", last modified: Thu Aug  3 10:00:42 2023, max compression
```

## Comparing `meggie-1.5.1.tar` & `meggie-1.5.2.tar`

### file list

```diff
@@ -1,327 +1,327 @@
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.705226 meggie-1.5.1/
--rw-r--r--   0 erpipehe (41746) users      (100)      170 2021-09-08 08:30:55.000000 meggie-1.5.1/AUTHORS.rst
--rw-r--r--   0 erpipehe (41746) users      (100)     1519 2021-09-08 08:30:55.000000 meggie-1.5.1/LICENSE
--rw-r--r--   0 erpipehe (41746) users      (100)      129 2021-09-08 08:30:55.000000 meggie-1.5.1/MANIFEST.in
--rw-r--r--   0 erpipehe (41746) users      (100)      414 2023-04-05 17:45:27.704226 meggie-1.5.1/PKG-INFO
--rw-r--r--   0 erpipehe (41746) users      (100)     1656 2022-12-14 15:40:56.000000 meggie-1.5.1/README.md
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.632226 meggie-1.5.1/meggie/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/__init__.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.634226 meggie-1.5.1/meggie/actions/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/__init__.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.634226 meggie-1.5.1/meggie/actions/epochs_create/
--rw-r--r--   0 erpipehe (41746) users      (100)     1096 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_create/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       88 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_create/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.635226 meggie-1.5.1/meggie/actions/epochs_create/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_create/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3510 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_create/controller/epoching.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.635226 meggie-1.5.1/meggie/actions/epochs_create/dialogs/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_create/dialogs/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     7057 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)    19922 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogUi.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.636226 meggie-1.5.1/meggie/actions/epochs_delete/
--rw-r--r--   0 erpipehe (41746) users      (100)      871 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_delete/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       81 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_delete/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.637226 meggie-1.5.1/meggie/actions/epochs_delete_from_all/
--rw-r--r--   0 erpipehe (41746) users      (100)     1254 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_delete_from_all/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      106 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_delete_from_all/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.637226 meggie-1.5.1/meggie/actions/epochs_info/
--rw-r--r--   0 erpipehe (41746) users      (100)     1687 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_info/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       76 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_info/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.638226 meggie-1.5.1/meggie/actions/epochs_plot/
--rw-r--r--   0 erpipehe (41746) users      (100)      843 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_plot/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       75 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_plot/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.639226 meggie-1.5.1/meggie/actions/epochs_plot_image/
--rw-r--r--   0 erpipehe (41746) users      (100)     1131 2022-12-12 14:01:39.000000 meggie-1.5.1/meggie/actions/epochs_plot_image/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       92 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/epochs_plot_image/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.640226 meggie-1.5.1/meggie/actions/evoked_create/
--rw-r--r--   0 erpipehe (41746) users      (100)     2230 2022-10-17 15:12:21.000000 meggie-1.5.1/meggie/actions/evoked_create/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       88 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_create/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.641226 meggie-1.5.1/meggie/actions/evoked_delete/
--rw-r--r--   0 erpipehe (41746) users      (100)      870 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_delete/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       81 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_delete/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.641226 meggie-1.5.1/meggie/actions/evoked_delete_from_all/
--rw-r--r--   0 erpipehe (41746) users      (100)     1252 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_delete_from_all/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      106 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_delete_from_all/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.642226 meggie-1.5.1/meggie/actions/evoked_group_average/
--rw-r--r--   0 erpipehe (41746) users      (100)     1766 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_group_average/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      103 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_group_average/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.642226 meggie-1.5.1/meggie/actions/evoked_group_average/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_group_average/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2440 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_group_average/controller/evoked.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.643226 meggie-1.5.1/meggie/actions/evoked_info/
--rw-r--r--   0 erpipehe (41746) users      (100)      950 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_info/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       76 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_info/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.643226 meggie-1.5.1/meggie/actions/evoked_plot/
--rw-r--r--   0 erpipehe (41746) users      (100)     1957 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_plot/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       75 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_plot/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.644226 meggie-1.5.1/meggie/actions/evoked_plot/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_plot/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3989 2022-10-18 09:24:21.000000 meggie-1.5.1/meggie/actions/evoked_plot/controller/evoked.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.644226 meggie-1.5.1/meggie/actions/evoked_plot_topomap/
--rw-r--r--   0 erpipehe (41746) users      (100)     2913 2023-04-05 16:39:58.000000 meggie-1.5.1/meggie/actions/evoked_plot_topomap/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       99 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_plot_topomap/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.645226 meggie-1.5.1/meggie/actions/evoked_plot_topomap/dialogs/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_plot_topomap/dialogs/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     1453 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     6774 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogUi.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.646226 meggie-1.5.1/meggie/actions/evoked_save/
--rw-r--r--   0 erpipehe (41746) users      (100)     2203 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_save/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       82 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_save/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.646226 meggie-1.5.1/meggie/actions/evoked_save/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_save/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2885 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/evoked_save/controller/evoked.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.647226 meggie-1.5.1/meggie/actions/raw_event_info/
--rw-r--r--   0 erpipehe (41746) users      (100)     1134 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_event_info/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       78 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_event_info/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.647226 meggie-1.5.1/meggie/actions/raw_events_from_annotations/
--rw-r--r--   0 erpipehe (41746) users      (100)     1209 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_events_from_annotations/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      121 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_events_from_annotations/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.648226 meggie-1.5.1/meggie/actions/raw_events_from_annotations/dialogs/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_events_from_annotations/dialogs/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3435 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     7842 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogUi.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.649226 meggie-1.5.1/meggie/actions/raw_filter/
--rw-r--r--   0 erpipehe (41746) users      (100)      997 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_filter/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       72 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_filter/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.649226 meggie-1.5.1/meggie/actions/raw_filter/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_filter/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     1279 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_filter/controller/filter.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.650226 meggie-1.5.1/meggie/actions/raw_filter/dialogs/
--rw-r--r--   0 erpipehe (41746) users      (100)     4738 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_filter/dialogs/filterDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)    15931 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_filter/dialogs/filterDialogUi.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.651226 meggie-1.5.1/meggie/actions/raw_ica/
--rw-r--r--   0 erpipehe (41746) users      (100)      704 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_ica/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       76 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_ica/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.652226 meggie-1.5.1/meggie/actions/raw_ica/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_ica/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     1964 2022-10-18 08:56:41.000000 meggie-1.5.1/meggie/actions/raw_ica/controller/ica.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.653226 meggie-1.5.1/meggie/actions/raw_ica/dialogs/
--rw-r--r--   0 erpipehe (41746) users      (100)     7232 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_ica/dialogs/icaDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     8809 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_ica/dialogs/icaDialogUi.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.654226 meggie-1.5.1/meggie/actions/raw_measurement_info/
--rw-r--r--   0 erpipehe (41746) users      (100)     1622 2022-10-17 16:22:30.000000 meggie-1.5.1/meggie/actions/raw_measurement_info/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       90 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_measurement_info/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.654226 meggie-1.5.1/meggie/actions/raw_montage/
--rw-r--r--   0 erpipehe (41746) users      (100)     1491 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_montage/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       96 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_montage/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.656226 meggie-1.5.1/meggie/actions/raw_montage/dialogs/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_montage/dialogs/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     4305 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_montage/dialogs/montageDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     8039 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_montage/dialogs/montageDialogUi.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.658226 meggie-1.5.1/meggie/actions/raw_plot/
--rw-r--r--   0 erpipehe (41746) users      (100)     2225 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_plot/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       73 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_plot/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.658226 meggie-1.5.1/meggie/actions/raw_plot_projections/
--rw-r--r--   0 erpipehe (41746) users      (100)     1077 2022-10-18 08:57:38.000000 meggie-1.5.1/meggie/actions/raw_plot_projections/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      101 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_plot_projections/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.659226 meggie-1.5.1/meggie/actions/raw_rereference/
--rw-r--r--   0 erpipehe (41746) users      (100)     1366 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_rereference/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      108 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_rereference/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.659226 meggie-1.5.1/meggie/actions/raw_rereference/dialogs/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_rereference/dialogs/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2959 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_rereference/dialogs/rereferencingDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     5250 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_rereference/dialogs/rereferencingDialogUi.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.660226 meggie-1.5.1/meggie/actions/raw_resample/
--rw-r--r--   0 erpipehe (41746) users      (100)     1005 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_resample/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       78 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_resample/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.660226 meggie-1.5.1/meggie/actions/raw_resample/dialogs/
--rw-r--r--   0 erpipehe (41746) users      (100)     2573 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_resample/dialogs/resamplingDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     6019 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/raw_resample/dialogs/resamplingDialogUi.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.661226 meggie-1.5.1/meggie/actions/spectrum_create/
--rw-r--r--   0 erpipehe (41746) users      (100)     1291 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_create/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       94 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_create/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.661226 meggie-1.5.1/meggie/actions/spectrum_create/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_create/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2826 2023-04-05 16:31:05.000000 meggie-1.5.1/meggie/actions/spectrum_create/controller/spectrum.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.662226 meggie-1.5.1/meggie/actions/spectrum_delete/
--rw-r--r--   0 erpipehe (41746) users      (100)      881 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_delete/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       85 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_delete/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.662226 meggie-1.5.1/meggie/actions/spectrum_delete_from_all/
--rw-r--r--   0 erpipehe (41746) users      (100)     1266 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_delete_from_all/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      110 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_delete_from_all/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.663226 meggie-1.5.1/meggie/actions/spectrum_group_average/
--rw-r--r--   0 erpipehe (41746) users      (100)     1772 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_group_average/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      105 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_group_average/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.663226 meggie-1.5.1/meggie/actions/spectrum_group_average/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_group_average/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     4107 2023-04-05 16:27:52.000000 meggie-1.5.1/meggie/actions/spectrum_group_average/controller/spectrum.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.664226 meggie-1.5.1/meggie/actions/spectrum_info/
--rw-r--r--   0 erpipehe (41746) users      (100)     1736 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_info/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       80 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_info/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.664226 meggie-1.5.1/meggie/actions/spectrum_plot/
--rw-r--r--   0 erpipehe (41746) users      (100)     1866 2022-11-24 07:02:58.000000 meggie-1.5.1/meggie/actions/spectrum_plot/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       79 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_plot/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.665226 meggie-1.5.1/meggie/actions/spectrum_plot/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_plot/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     4415 2022-11-24 07:54:26.000000 meggie-1.5.1/meggie/actions/spectrum_plot/controller/spectrum.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.665226 meggie-1.5.1/meggie/actions/spectrum_save/
--rw-r--r--   0 erpipehe (41746) users      (100)     2163 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_save/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       86 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_save/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.666226 meggie-1.5.1/meggie/actions/spectrum_save/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/spectrum_save/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2660 2022-11-25 09:32:24.000000 meggie-1.5.1/meggie/actions/spectrum_save/controller/spectrum.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.666226 meggie-1.5.1/meggie/actions/tfr_create/
--rw-r--r--   0 erpipehe (41746) users      (100)     1455 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_create/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       79 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_create/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.667226 meggie-1.5.1/meggie/actions/tfr_create/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_create/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     1575 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_create/controller/tfr.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.668226 meggie-1.5.1/meggie/actions/tfr_create/dialogs/
--rw-r--r--   0 erpipehe (41746) users      (100)     5725 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_create/dialogs/TFRDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)    14124 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_create/dialogs/TFRDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_create/dialogs/__init__.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.668226 meggie-1.5.1/meggie/actions/tfr_delete/
--rw-r--r--   0 erpipehe (41746) users      (100)      856 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_delete/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       75 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_delete/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.669226 meggie-1.5.1/meggie/actions/tfr_delete_from_all/
--rw-r--r--   0 erpipehe (41746) users      (100)     1231 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_delete_from_all/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      100 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_delete_from_all/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.669226 meggie-1.5.1/meggie/actions/tfr_group_average/
--rw-r--r--   0 erpipehe (41746) users      (100)     1735 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_group_average/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      100 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_group_average/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.670226 meggie-1.5.1/meggie/actions/tfr_group_average/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_group_average/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     4023 2023-04-03 15:27:42.000000 meggie-1.5.1/meggie/actions/tfr_group_average/controller/tfr.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.671226 meggie-1.5.1/meggie/actions/tfr_info/
--rw-r--r--   0 erpipehe (41746) users      (100)     1650 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_info/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       70 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_info/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.672226 meggie-1.5.1/meggie/actions/tfr_plot/
--rw-r--r--   0 erpipehe (41746) users      (100)     2835 2023-04-03 15:27:42.000000 meggie-1.5.1/meggie/actions/tfr_plot/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       73 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_plot/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.673226 meggie-1.5.1/meggie/actions/tfr_plot/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_plot/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     4509 2023-04-03 15:27:42.000000 meggie-1.5.1/meggie/actions/tfr_plot/controller/tfr.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.674226 meggie-1.5.1/meggie/actions/tfr_plot_tse/
--rw-r--r--   0 erpipehe (41746) users      (100)     2505 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_plot_tse/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       77 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_plot_tse/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.674226 meggie-1.5.1/meggie/actions/tfr_plot_tse/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_plot_tse/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     5800 2022-10-18 09:08:05.000000 meggie-1.5.1/meggie/actions/tfr_plot_tse/controller/tfr.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.675226 meggie-1.5.1/meggie/actions/tfr_save/
--rw-r--r--   0 erpipehe (41746) users      (100)     2513 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_save/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       80 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_save/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.675226 meggie-1.5.1/meggie/actions/tfr_save/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_save/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3919 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_save/controller/tfr.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.676226 meggie-1.5.1/meggie/actions/tfr_save_tse/
--rw-r--r--   0 erpipehe (41746) users      (100)     2493 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_save_tse/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)       84 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_save_tse/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.676226 meggie-1.5.1/meggie/actions/tfr_save_tse/controller/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_save_tse/controller/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     4006 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/actions/tfr_save_tse/controller/tfr.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2348 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.677226 meggie-1.5.1/meggie/datatypes/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/datatypes/__init__.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.678226 meggie-1.5.1/meggie/datatypes/epochs/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/datatypes/epochs/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      122 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/datatypes/epochs/configuration.json
--rw-r--r--   0 erpipehe (41746) users      (100)     2250 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/datatypes/epochs/epochs.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.678226 meggie-1.5.1/meggie/datatypes/epochs/tests/
--rw-r--r--   0 erpipehe (41746) users      (100)     1149 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/datatypes/epochs/tests/test_epochs.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.678226 meggie-1.5.1/meggie/datatypes/evoked/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/datatypes/evoked/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      124 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/datatypes/evoked/configuration.json
--rw-r--r--   0 erpipehe (41746) users      (100)     3678 2022-10-17 14:57:14.000000 meggie-1.5.1/meggie/datatypes/evoked/evoked.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.679226 meggie-1.5.1/meggie/datatypes/evoked/tests/
--rw-r--r--   0 erpipehe (41746) users      (100)     1313 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/datatypes/evoked/tests/test_evoked.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.679226 meggie-1.5.1/meggie/datatypes/spectrum/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/datatypes/spectrum/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      136 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/datatypes/spectrum/configuration.json
--rw-r--r--   0 erpipehe (41746) users      (100)     7834 2023-04-03 15:27:42.000000 meggie-1.5.1/meggie/datatypes/spectrum/spectrum.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.680226 meggie-1.5.1/meggie/datatypes/spectrum/tests/
--rw-r--r--   0 erpipehe (41746) users      (100)     1522 2023-04-05 17:42:16.000000 meggie-1.5.1/meggie/datatypes/spectrum/tests/test_spectrum.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.681226 meggie-1.5.1/meggie/datatypes/tfr/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/datatypes/tfr/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      106 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/datatypes/tfr/configuration.json
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.681226 meggie-1.5.1/meggie/datatypes/tfr/tests/
--rw-r--r--   0 erpipehe (41746) users      (100)     1517 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/datatypes/tfr/tests/test_tfr.py
--rw-r--r--   0 erpipehe (41746) users      (100)     5696 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/datatypes/tfr/tfr.py
--rw-r--r--   0 erpipehe (41746) users      (100)    15230 2022-10-17 16:23:46.000000 meggie-1.5.1/meggie/experiment.py
--rw-r--r--   0 erpipehe (41746) users      (100)    14100 2022-10-17 15:11:30.000000 meggie-1.5.1/meggie/mainWindowMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)    12155 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainWindowUi.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.682226 meggie-1.5.1/meggie/mainwindow/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/__init__.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.690226 meggie-1.5.1/meggie/mainwindow/dialogs/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)      775 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/aboutDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)    11990 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/aboutDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)     5732 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/actionDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3449 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/actionDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)     1601 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/activePluginsDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2610 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/activePluginsDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)     4020 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/addSubjectDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     4176 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/addSubjectDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)     7946 2022-10-17 16:26:26.000000 meggie-1.5.1/meggie/mainwindow/dialogs/channelGroupsDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     7419 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/channelGroupsDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3278 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/createExperimentDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     5039 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/createExperimentDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3063 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/pipelineDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3537 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/pipelineDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2656 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/preferencesDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     5385 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dialogs/preferencesDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)    29690 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/mainwindow/dynamic.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3508 2022-11-24 07:55:47.000000 meggie-1.5.1/meggie/mainwindow/preferences.py
--rw-r--r--   0 erpipehe (41746) users      (100)      575 2022-11-21 17:08:42.000000 meggie-1.5.1/meggie/run.py
--rw-r--r--   0 erpipehe (41746) users      (100)     5597 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/subject.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.690226 meggie-1.5.1/meggie/tests/
--rw-r--r--   0 erpipehe (41746) users      (100)     1778 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/tests/test_experiment_and_subject.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.695226 meggie-1.5.1/meggie/utilities/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     9796 2022-10-17 17:58:41.000000 meggie-1.5.1/meggie/utilities/channels.py
--rw-r--r--   0 erpipehe (41746) users      (100)     1775 2022-04-01 09:59:41.000000 meggie-1.5.1/meggie/utilities/compare.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2165 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/datatype.py
--rw-r--r--   0 erpipehe (41746) users      (100)      651 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/debug.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.701226 meggie-1.5.1/meggie/utilities/dialogs/
--rw-r--r--   0 erpipehe (41746) users      (100)     3450 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/TFROutputOptionsMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)    13752 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/TFROutputOptionsUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2482 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/bitSelectionDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)    19408 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/bitSelectionDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3399 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/groupSelectionDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3686 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/groupSelectionDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)      957 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/outputOptionsMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3133 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/outputOptionsUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2547 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)    13106 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)     7762 2022-12-14 14:49:51.000000 meggie-1.5.1/meggie/utilities/dialogs/powerSpectrumDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)    13547 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/powerSpectrumDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)      518 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/shortMessageBoxMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3368 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/shortMessageBoxUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)      765 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/shortQuestionBoxMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3723 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/shortQuestionBoxUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3151 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/simpleDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     4664 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/simpleDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2750 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/singleChannelDialogMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     9173 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/dialogs/singleChannelDialogUi.py
--rw-r--r--   0 erpipehe (41746) users      (100)     8009 2023-04-05 17:39:50.000000 meggie-1.5.1/meggie/utilities/events.py
--rw-r--r--   0 erpipehe (41746) users      (100)     7038 2023-04-03 15:27:42.000000 meggie-1.5.1/meggie/utilities/filemanager.py
--rw-r--r--   0 erpipehe (41746) users      (100)      612 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/formats.py
--rw-r--r--   0 erpipehe (41746) users      (100)     4550 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/generate_experiments.py
--rw-r--r--   0 erpipehe (41746) users      (100)     1547 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/measurement_info.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2239 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/messaging.py
--rw-r--r--   0 erpipehe (41746) users      (100)      851 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/names.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2134 2022-12-12 14:00:29.000000 meggie-1.5.1/meggie/utilities/plotting.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.702226 meggie-1.5.1/meggie/utilities/tests/
--rw-r--r--   0 erpipehe (41746) users      (100)     3057 2022-10-17 16:27:55.000000 meggie-1.5.1/meggie/utilities/tests/test_channels.py
--rw-r--r--   0 erpipehe (41746) users      (100)     1493 2023-04-05 15:55:57.000000 meggie-1.5.1/meggie/utilities/tests/test_events.py
--rw-r--r--   0 erpipehe (41746) users      (100)     1283 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/tests/test_filemanager.py
--rw-r--r--   0 erpipehe (41746) users      (100)      585 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/tests/test_measurement_info.py
--rw-r--r--   0 erpipehe (41746) users      (100)      573 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/tests/test_names.py
--rw-r--r--   0 erpipehe (41746) users      (100)      202 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/tests/test_plotting.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2330 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/threading.py
--rw-r--r--   0 erpipehe (41746) users      (100)      160 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/uid.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2169 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/units.py
--rw-r--r--   0 erpipehe (41746) users      (100)     2108 2023-04-03 15:27:42.000000 meggie-1.5.1/meggie/utilities/validators.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.703226 meggie-1.5.1/meggie/utilities/widgets/
--rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/widgets/__init__.py
--rw-r--r--   0 erpipehe (41746) users      (100)     3899 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/widgets/batchingWidgetMain.py
--rw-r--r--   0 erpipehe (41746) users      (100)     5911 2021-09-08 08:30:55.000000 meggie-1.5.1/meggie/utilities/widgets/batchingWidgetUi.py
-drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-04-05 17:45:27.634226 meggie-1.5.1/meggie.egg-info/
--rw-r--r--   0 erpipehe (41746) users      (100)      414 2023-04-05 17:45:27.000000 meggie-1.5.1/meggie.egg-info/PKG-INFO
--rw-r--r--   0 erpipehe (41746) users      (100)    10622 2023-04-05 17:45:27.000000 meggie-1.5.1/meggie.egg-info/SOURCES.txt
--rw-r--r--   0 erpipehe (41746) users      (100)        1 2023-04-05 17:45:27.000000 meggie-1.5.1/meggie.egg-info/dependency_links.txt
--rw-r--r--   0 erpipehe (41746) users      (100)       44 2023-04-05 17:45:27.000000 meggie-1.5.1/meggie.egg-info/entry_points.txt
--rw-r--r--   0 erpipehe (41746) users      (100)        1 2022-10-18 08:25:51.000000 meggie-1.5.1/meggie.egg-info/not-zip-safe
--rw-r--r--   0 erpipehe (41746) users      (100)        7 2023-04-05 17:45:27.000000 meggie-1.5.1/meggie.egg-info/top_level.txt
--rw-r--r--   0 erpipehe (41746) users      (100)       38 2023-04-05 17:45:27.705226 meggie-1.5.1/setup.cfg
--rw-r--r--   0 erpipehe (41746) users      (100)      603 2023-04-05 17:44:26.000000 meggie-1.5.1/setup.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.337139 meggie-1.5.2/
+-rw-r--r--   0 erpipehe (41746) users      (100)      170 2021-09-08 08:30:55.000000 meggie-1.5.2/AUTHORS.rst
+-rw-r--r--   0 erpipehe (41746) users      (100)     1519 2021-09-08 08:30:55.000000 meggie-1.5.2/LICENSE
+-rw-r--r--   0 erpipehe (41746) users      (100)      129 2021-09-08 08:30:55.000000 meggie-1.5.2/MANIFEST.in
+-rw-r--r--   0 erpipehe (41746) users      (100)      414 2023-08-03 10:00:42.336139 meggie-1.5.2/PKG-INFO
+-rw-r--r--   0 erpipehe (41746) users      (100)     1656 2022-12-14 15:40:56.000000 meggie-1.5.2/README.md
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.233139 meggie-1.5.2/meggie/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/__init__.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.235139 meggie-1.5.2/meggie/actions/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/__init__.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.235139 meggie-1.5.2/meggie/actions/epochs_create/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1096 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_create/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       88 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_create/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.236139 meggie-1.5.2/meggie/actions/epochs_create/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_create/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3510 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_create/controller/epoching.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.237139 meggie-1.5.2/meggie/actions/epochs_create/dialogs/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_create/dialogs/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     7057 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)    19922 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogUi.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.238139 meggie-1.5.2/meggie/actions/epochs_delete/
+-rw-r--r--   0 erpipehe (41746) users      (100)      871 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_delete/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       81 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_delete/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.239139 meggie-1.5.2/meggie/actions/epochs_delete_from_all/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1254 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_delete_from_all/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      106 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_delete_from_all/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.240139 meggie-1.5.2/meggie/actions/epochs_info/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1687 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_info/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       76 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_info/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.241139 meggie-1.5.2/meggie/actions/epochs_plot/
+-rw-r--r--   0 erpipehe (41746) users      (100)      843 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_plot/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       75 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_plot/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.243139 meggie-1.5.2/meggie/actions/epochs_plot_image/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1131 2022-12-12 14:01:39.000000 meggie-1.5.2/meggie/actions/epochs_plot_image/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       92 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/epochs_plot_image/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.245139 meggie-1.5.2/meggie/actions/evoked_create/
+-rw-r--r--   0 erpipehe (41746) users      (100)     2230 2022-10-17 15:12:21.000000 meggie-1.5.2/meggie/actions/evoked_create/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       88 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_create/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.246139 meggie-1.5.2/meggie/actions/evoked_delete/
+-rw-r--r--   0 erpipehe (41746) users      (100)      870 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_delete/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       81 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_delete/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.248139 meggie-1.5.2/meggie/actions/evoked_delete_from_all/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1252 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_delete_from_all/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      106 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_delete_from_all/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.249139 meggie-1.5.2/meggie/actions/evoked_group_average/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1766 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_group_average/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      103 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_group_average/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.250139 meggie-1.5.2/meggie/actions/evoked_group_average/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_group_average/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2440 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_group_average/controller/evoked.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.251139 meggie-1.5.2/meggie/actions/evoked_info/
+-rw-r--r--   0 erpipehe (41746) users      (100)      950 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_info/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       76 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_info/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.253139 meggie-1.5.2/meggie/actions/evoked_plot/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1957 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_plot/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       75 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_plot/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.255139 meggie-1.5.2/meggie/actions/evoked_plot/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_plot/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3989 2022-10-18 09:24:21.000000 meggie-1.5.2/meggie/actions/evoked_plot/controller/evoked.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.256139 meggie-1.5.2/meggie/actions/evoked_plot_topomap/
+-rw-r--r--   0 erpipehe (41746) users      (100)     2913 2023-04-05 16:39:58.000000 meggie-1.5.2/meggie/actions/evoked_plot_topomap/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       99 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_plot_topomap/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.257139 meggie-1.5.2/meggie/actions/evoked_plot_topomap/dialogs/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_plot_topomap/dialogs/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     1453 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     6774 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogUi.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.258139 meggie-1.5.2/meggie/actions/evoked_save/
+-rw-r--r--   0 erpipehe (41746) users      (100)     2203 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_save/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       82 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_save/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.259139 meggie-1.5.2/meggie/actions/evoked_save/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_save/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2885 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/evoked_save/controller/evoked.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.260139 meggie-1.5.2/meggie/actions/raw_event_info/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1134 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_event_info/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       78 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_event_info/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.261139 meggie-1.5.2/meggie/actions/raw_events_from_annotations/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1209 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_events_from_annotations/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      121 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_events_from_annotations/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.263139 meggie-1.5.2/meggie/actions/raw_events_from_annotations/dialogs/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_events_from_annotations/dialogs/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3435 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     7842 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogUi.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.264139 meggie-1.5.2/meggie/actions/raw_filter/
+-rw-r--r--   0 erpipehe (41746) users      (100)      997 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_filter/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       72 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_filter/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.265139 meggie-1.5.2/meggie/actions/raw_filter/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_filter/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     1279 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_filter/controller/filter.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.265139 meggie-1.5.2/meggie/actions/raw_filter/dialogs/
+-rw-r--r--   0 erpipehe (41746) users      (100)     4738 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_filter/dialogs/filterDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)    15931 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_filter/dialogs/filterDialogUi.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.266139 meggie-1.5.2/meggie/actions/raw_ica/
+-rw-r--r--   0 erpipehe (41746) users      (100)      704 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_ica/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       76 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_ica/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.267139 meggie-1.5.2/meggie/actions/raw_ica/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_ica/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     1964 2022-10-18 08:56:41.000000 meggie-1.5.2/meggie/actions/raw_ica/controller/ica.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.267139 meggie-1.5.2/meggie/actions/raw_ica/dialogs/
+-rw-r--r--   0 erpipehe (41746) users      (100)     7232 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_ica/dialogs/icaDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     8809 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_ica/dialogs/icaDialogUi.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.268139 meggie-1.5.2/meggie/actions/raw_measurement_info/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1622 2022-10-17 16:22:30.000000 meggie-1.5.2/meggie/actions/raw_measurement_info/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       90 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_measurement_info/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.272139 meggie-1.5.2/meggie/actions/raw_montage/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1491 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_montage/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       96 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_montage/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.273139 meggie-1.5.2/meggie/actions/raw_montage/dialogs/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_montage/dialogs/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     4305 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_montage/dialogs/montageDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     8039 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_montage/dialogs/montageDialogUi.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.273139 meggie-1.5.2/meggie/actions/raw_plot/
+-rw-r--r--   0 erpipehe (41746) users      (100)     2225 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_plot/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       73 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_plot/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.277139 meggie-1.5.2/meggie/actions/raw_plot_projections/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1077 2022-10-18 08:57:38.000000 meggie-1.5.2/meggie/actions/raw_plot_projections/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      101 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_plot_projections/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.278139 meggie-1.5.2/meggie/actions/raw_rereference/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1156 2023-08-03 09:57:09.000000 meggie-1.5.2/meggie/actions/raw_rereference/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      108 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_rereference/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.279139 meggie-1.5.2/meggie/actions/raw_rereference/dialogs/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_rereference/dialogs/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3372 2023-08-03 09:57:09.000000 meggie-1.5.2/meggie/actions/raw_rereference/dialogs/rereferencingDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     7235 2023-08-03 09:57:09.000000 meggie-1.5.2/meggie/actions/raw_rereference/dialogs/rereferencingDialogUi.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.281139 meggie-1.5.2/meggie/actions/raw_resample/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1005 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_resample/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       78 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_resample/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.281139 meggie-1.5.2/meggie/actions/raw_resample/dialogs/
+-rw-r--r--   0 erpipehe (41746) users      (100)     2573 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_resample/dialogs/resamplingDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     6019 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/raw_resample/dialogs/resamplingDialogUi.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.282139 meggie-1.5.2/meggie/actions/spectrum_create/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1291 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_create/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       94 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_create/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.283139 meggie-1.5.2/meggie/actions/spectrum_create/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_create/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2826 2023-04-05 16:31:05.000000 meggie-1.5.2/meggie/actions/spectrum_create/controller/spectrum.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.284139 meggie-1.5.2/meggie/actions/spectrum_delete/
+-rw-r--r--   0 erpipehe (41746) users      (100)      881 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_delete/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       85 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_delete/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.284139 meggie-1.5.2/meggie/actions/spectrum_delete_from_all/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1266 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_delete_from_all/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      110 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_delete_from_all/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.285139 meggie-1.5.2/meggie/actions/spectrum_group_average/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1772 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_group_average/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      105 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_group_average/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.286139 meggie-1.5.2/meggie/actions/spectrum_group_average/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_group_average/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     4107 2023-04-05 16:27:52.000000 meggie-1.5.2/meggie/actions/spectrum_group_average/controller/spectrum.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.287139 meggie-1.5.2/meggie/actions/spectrum_info/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1736 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_info/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       80 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_info/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.289139 meggie-1.5.2/meggie/actions/spectrum_plot/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1866 2022-11-24 07:02:58.000000 meggie-1.5.2/meggie/actions/spectrum_plot/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       79 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_plot/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.289139 meggie-1.5.2/meggie/actions/spectrum_plot/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_plot/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     4415 2022-11-24 07:54:26.000000 meggie-1.5.2/meggie/actions/spectrum_plot/controller/spectrum.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.290139 meggie-1.5.2/meggie/actions/spectrum_save/
+-rw-r--r--   0 erpipehe (41746) users      (100)     2163 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_save/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       86 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_save/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.291139 meggie-1.5.2/meggie/actions/spectrum_save/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/spectrum_save/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2660 2022-11-25 09:32:24.000000 meggie-1.5.2/meggie/actions/spectrum_save/controller/spectrum.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.291139 meggie-1.5.2/meggie/actions/tfr_create/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1455 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_create/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       79 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_create/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.292139 meggie-1.5.2/meggie/actions/tfr_create/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_create/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     1575 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_create/controller/tfr.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.293139 meggie-1.5.2/meggie/actions/tfr_create/dialogs/
+-rw-r--r--   0 erpipehe (41746) users      (100)     5725 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_create/dialogs/TFRDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)    14124 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_create/dialogs/TFRDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_create/dialogs/__init__.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.293139 meggie-1.5.2/meggie/actions/tfr_delete/
+-rw-r--r--   0 erpipehe (41746) users      (100)      856 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_delete/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       75 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_delete/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.294139 meggie-1.5.2/meggie/actions/tfr_delete_from_all/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1231 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_delete_from_all/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      100 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_delete_from_all/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.295139 meggie-1.5.2/meggie/actions/tfr_group_average/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1735 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_group_average/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      100 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_group_average/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.296139 meggie-1.5.2/meggie/actions/tfr_group_average/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_group_average/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     4023 2023-04-03 15:27:42.000000 meggie-1.5.2/meggie/actions/tfr_group_average/controller/tfr.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.298139 meggie-1.5.2/meggie/actions/tfr_info/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1650 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_info/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       70 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_info/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.298139 meggie-1.5.2/meggie/actions/tfr_plot/
+-rw-r--r--   0 erpipehe (41746) users      (100)     2835 2023-04-03 15:27:42.000000 meggie-1.5.2/meggie/actions/tfr_plot/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       73 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_plot/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.300139 meggie-1.5.2/meggie/actions/tfr_plot/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_plot/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     4509 2023-04-03 15:27:42.000000 meggie-1.5.2/meggie/actions/tfr_plot/controller/tfr.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.301139 meggie-1.5.2/meggie/actions/tfr_plot_tse/
+-rw-r--r--   0 erpipehe (41746) users      (100)     2505 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_plot_tse/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       77 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_plot_tse/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.301139 meggie-1.5.2/meggie/actions/tfr_plot_tse/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_plot_tse/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     5800 2022-10-18 09:08:05.000000 meggie-1.5.2/meggie/actions/tfr_plot_tse/controller/tfr.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.302139 meggie-1.5.2/meggie/actions/tfr_save/
+-rw-r--r--   0 erpipehe (41746) users      (100)     2513 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_save/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       80 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_save/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.303139 meggie-1.5.2/meggie/actions/tfr_save/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_save/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3919 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_save/controller/tfr.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.304139 meggie-1.5.2/meggie/actions/tfr_save_tse/
+-rw-r--r--   0 erpipehe (41746) users      (100)     2493 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_save_tse/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)       84 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_save_tse/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.304139 meggie-1.5.2/meggie/actions/tfr_save_tse/controller/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_save_tse/controller/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     4006 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/actions/tfr_save_tse/controller/tfr.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2348 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.305139 meggie-1.5.2/meggie/datatypes/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/datatypes/__init__.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.306139 meggie-1.5.2/meggie/datatypes/epochs/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/datatypes/epochs/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      122 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/datatypes/epochs/configuration.json
+-rw-r--r--   0 erpipehe (41746) users      (100)     2250 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/datatypes/epochs/epochs.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.306139 meggie-1.5.2/meggie/datatypes/epochs/tests/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1149 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/datatypes/epochs/tests/test_epochs.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.307139 meggie-1.5.2/meggie/datatypes/evoked/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/datatypes/evoked/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      124 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/datatypes/evoked/configuration.json
+-rw-r--r--   0 erpipehe (41746) users      (100)     3678 2022-10-17 14:57:14.000000 meggie-1.5.2/meggie/datatypes/evoked/evoked.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.307139 meggie-1.5.2/meggie/datatypes/evoked/tests/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1313 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/datatypes/evoked/tests/test_evoked.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.309139 meggie-1.5.2/meggie/datatypes/spectrum/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/datatypes/spectrum/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      136 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/datatypes/spectrum/configuration.json
+-rw-r--r--   0 erpipehe (41746) users      (100)     7834 2023-04-03 15:27:42.000000 meggie-1.5.2/meggie/datatypes/spectrum/spectrum.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.310139 meggie-1.5.2/meggie/datatypes/spectrum/tests/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1522 2023-04-05 17:42:16.000000 meggie-1.5.2/meggie/datatypes/spectrum/tests/test_spectrum.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.311139 meggie-1.5.2/meggie/datatypes/tfr/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/datatypes/tfr/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      106 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/datatypes/tfr/configuration.json
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.311139 meggie-1.5.2/meggie/datatypes/tfr/tests/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1517 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/datatypes/tfr/tests/test_tfr.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     5696 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/datatypes/tfr/tfr.py
+-rw-r--r--   0 erpipehe (41746) users      (100)    15230 2022-10-17 16:23:46.000000 meggie-1.5.2/meggie/experiment.py
+-rw-r--r--   0 erpipehe (41746) users      (100)    14100 2022-10-17 15:11:30.000000 meggie-1.5.2/meggie/mainWindowMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)    12155 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainWindowUi.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.313139 meggie-1.5.2/meggie/mainwindow/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/__init__.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.319139 meggie-1.5.2/meggie/mainwindow/dialogs/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      775 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/aboutDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)    11990 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/aboutDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     5732 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/actionDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3449 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/actionDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     1601 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/activePluginsDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2610 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/activePluginsDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     4020 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/addSubjectDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     4176 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/addSubjectDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     7946 2022-10-17 16:26:26.000000 meggie-1.5.2/meggie/mainwindow/dialogs/channelGroupsDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     7419 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/channelGroupsDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3278 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/createExperimentDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     5039 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/createExperimentDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3063 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/pipelineDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3537 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/pipelineDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2656 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/preferencesDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     5385 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dialogs/preferencesDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)    29690 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/mainwindow/dynamic.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3508 2022-11-24 07:55:47.000000 meggie-1.5.2/meggie/mainwindow/preferences.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      575 2022-11-21 17:08:42.000000 meggie-1.5.2/meggie/run.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     5597 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/subject.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.320139 meggie-1.5.2/meggie/tests/
+-rw-r--r--   0 erpipehe (41746) users      (100)     1778 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/tests/test_experiment_and_subject.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.326139 meggie-1.5.2/meggie/utilities/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     9796 2022-10-17 17:58:41.000000 meggie-1.5.2/meggie/utilities/channels.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     1775 2022-04-01 09:59:41.000000 meggie-1.5.2/meggie/utilities/compare.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2165 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/datatype.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      651 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/debug.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.334139 meggie-1.5.2/meggie/utilities/dialogs/
+-rw-r--r--   0 erpipehe (41746) users      (100)     3450 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/TFROutputOptionsMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)    13752 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/TFROutputOptionsUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2482 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/bitSelectionDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)    19408 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/bitSelectionDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3399 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/groupSelectionDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3686 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/groupSelectionDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      957 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/outputOptionsMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3133 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/outputOptionsUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2547 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)    13106 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     7762 2022-12-14 14:49:51.000000 meggie-1.5.2/meggie/utilities/dialogs/powerSpectrumDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)    13547 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/powerSpectrumDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      518 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/shortMessageBoxMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3368 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/shortMessageBoxUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      765 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/shortQuestionBoxMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3723 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/shortQuestionBoxUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3151 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/simpleDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     4664 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/simpleDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2750 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/singleChannelDialogMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     9173 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/dialogs/singleChannelDialogUi.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     8009 2023-04-05 17:39:50.000000 meggie-1.5.2/meggie/utilities/events.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     7038 2023-04-03 15:27:42.000000 meggie-1.5.2/meggie/utilities/filemanager.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      612 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/formats.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     4550 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/generate_experiments.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     1547 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/measurement_info.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2239 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/messaging.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      851 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/names.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2134 2022-12-12 14:00:29.000000 meggie-1.5.2/meggie/utilities/plotting.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.335139 meggie-1.5.2/meggie/utilities/tests/
+-rw-r--r--   0 erpipehe (41746) users      (100)     3057 2022-10-17 16:27:55.000000 meggie-1.5.2/meggie/utilities/tests/test_channels.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     1493 2023-04-05 15:55:57.000000 meggie-1.5.2/meggie/utilities/tests/test_events.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     1283 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/tests/test_filemanager.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      585 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/tests/test_measurement_info.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      573 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/tests/test_names.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      202 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/tests/test_plotting.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2330 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/threading.py
+-rw-r--r--   0 erpipehe (41746) users      (100)      160 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/uid.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2169 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/units.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     2108 2023-04-03 15:27:42.000000 meggie-1.5.2/meggie/utilities/validators.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.336139 meggie-1.5.2/meggie/utilities/widgets/
+-rw-r--r--   0 erpipehe (41746) users      (100)        0 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/widgets/__init__.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     3899 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/widgets/batchingWidgetMain.py
+-rw-r--r--   0 erpipehe (41746) users      (100)     5911 2021-09-08 08:30:55.000000 meggie-1.5.2/meggie/utilities/widgets/batchingWidgetUi.py
+drwxr-xr-x   0 erpipehe (41746) users      (100)        0 2023-08-03 10:00:42.235139 meggie-1.5.2/meggie.egg-info/
+-rw-r--r--   0 erpipehe (41746) users      (100)      414 2023-08-03 10:00:42.000000 meggie-1.5.2/meggie.egg-info/PKG-INFO
+-rw-r--r--   0 erpipehe (41746) users      (100)    10622 2023-08-03 10:00:42.000000 meggie-1.5.2/meggie.egg-info/SOURCES.txt
+-rw-r--r--   0 erpipehe (41746) users      (100)        1 2023-08-03 10:00:42.000000 meggie-1.5.2/meggie.egg-info/dependency_links.txt
+-rw-r--r--   0 erpipehe (41746) users      (100)       44 2023-08-03 10:00:42.000000 meggie-1.5.2/meggie.egg-info/entry_points.txt
+-rw-r--r--   0 erpipehe (41746) users      (100)        1 2022-10-18 08:25:51.000000 meggie-1.5.2/meggie.egg-info/not-zip-safe
+-rw-r--r--   0 erpipehe (41746) users      (100)        7 2023-08-03 10:00:42.000000 meggie-1.5.2/meggie.egg-info/top_level.txt
+-rw-r--r--   0 erpipehe (41746) users      (100)       38 2023-08-03 10:00:42.337139 meggie-1.5.2/setup.cfg
+-rw-r--r--   0 erpipehe (41746) users      (100)      603 2023-08-03 09:58:01.000000 meggie-1.5.2/setup.py
```

### Comparing `meggie-1.5.1/LICENSE` & `meggie-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/README.md` & `meggie-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/epochs_create/__init__.py` & `meggie-1.5.2/meggie/actions/epochs_create/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/epochs_create/controller/epoching.py` & `meggie-1.5.2/meggie/actions/epochs_create/controller/epoching.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogMain.py` & `meggie-1.5.2/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogUi.py` & `meggie-1.5.2/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/epochs_delete/__init__.py` & `meggie-1.5.2/meggie/actions/epochs_delete/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/epochs_delete_from_all/__init__.py` & `meggie-1.5.2/meggie/actions/epochs_delete_from_all/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/epochs_info/__init__.py` & `meggie-1.5.2/meggie/actions/epochs_info/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/epochs_plot/__init__.py` & `meggie-1.5.2/meggie/actions/epochs_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/epochs_plot_image/__init__.py` & `meggie-1.5.2/meggie/actions/epochs_plot_image/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/evoked_create/__init__.py` & `meggie-1.5.2/meggie/actions/evoked_create/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/evoked_delete/__init__.py` & `meggie-1.5.2/meggie/actions/evoked_delete/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/evoked_delete_from_all/__init__.py` & `meggie-1.5.2/meggie/actions/evoked_delete_from_all/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/evoked_group_average/__init__.py` & `meggie-1.5.2/meggie/actions/evoked_group_average/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/evoked_group_average/controller/evoked.py` & `meggie-1.5.2/meggie/actions/evoked_group_average/controller/evoked.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/evoked_info/__init__.py` & `meggie-1.5.2/meggie/actions/evoked_info/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/evoked_plot/__init__.py` & `meggie-1.5.2/meggie/actions/evoked_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/evoked_plot/controller/evoked.py` & `meggie-1.5.2/meggie/actions/evoked_plot/controller/evoked.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/evoked_plot_topomap/__init__.py` & `meggie-1.5.2/meggie/actions/evoked_plot_topomap/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogMain.py` & `meggie-1.5.2/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogUi.py` & `meggie-1.5.2/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/evoked_save/__init__.py` & `meggie-1.5.2/meggie/actions/evoked_save/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/evoked_save/controller/evoked.py` & `meggie-1.5.2/meggie/actions/evoked_save/controller/evoked.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_event_info/__init__.py` & `meggie-1.5.2/meggie/actions/raw_event_info/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_events_from_annotations/__init__.py` & `meggie-1.5.2/meggie/actions/raw_events_from_annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogMain.py` & `meggie-1.5.2/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogUi.py` & `meggie-1.5.2/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_filter/__init__.py` & `meggie-1.5.2/meggie/actions/raw_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_filter/controller/filter.py` & `meggie-1.5.2/meggie/actions/raw_filter/controller/filter.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_filter/dialogs/filterDialogMain.py` & `meggie-1.5.2/meggie/actions/raw_filter/dialogs/filterDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_filter/dialogs/filterDialogUi.py` & `meggie-1.5.2/meggie/actions/raw_filter/dialogs/filterDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_ica/__init__.py` & `meggie-1.5.2/meggie/actions/raw_ica/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_ica/controller/ica.py` & `meggie-1.5.2/meggie/actions/raw_ica/controller/ica.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_ica/dialogs/icaDialogMain.py` & `meggie-1.5.2/meggie/actions/raw_ica/dialogs/icaDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_ica/dialogs/icaDialogUi.py` & `meggie-1.5.2/meggie/actions/raw_ica/dialogs/icaDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_measurement_info/__init__.py` & `meggie-1.5.2/meggie/actions/raw_measurement_info/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_montage/__init__.py` & `meggie-1.5.2/meggie/actions/raw_montage/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_montage/dialogs/montageDialogMain.py` & `meggie-1.5.2/meggie/actions/raw_montage/dialogs/montageDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_montage/dialogs/montageDialogUi.py` & `meggie-1.5.2/meggie/actions/raw_montage/dialogs/montageDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_plot/__init__.py` & `meggie-1.5.2/meggie/actions/raw_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_plot_projections/__init__.py` & `meggie-1.5.2/meggie/actions/raw_plot_projections/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_rereference/__init__.py` & `meggie-1.5.2/meggie/actions/raw_rereference/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,21 +22,18 @@
     @subject_action
     def handler(self, subject, params):
         """
         """
         @threaded
         def rereference_fun():
             raw = subject.get_raw()
-            if params['selection'] == 'Use average':
-                raw.set_eeg_reference(ref_channels='average', 
-                                      projection=False)
-            elif params['selection'] == '':
-                raise Exception('Empty selection')
-            else:
-                raw.set_eeg_reference(ref_channels=[selection])
+            raw = raw.set_eeg_reference(
+                ref_channels=params['selection'],
+                projection=False,
+            )
 
         rereference_fun(do_meanwhile=self.window.update_ui)
         subject.rereferenced = True
         subject.save()
 
     def run(self):
         rereference_dialog = RereferencingDialog(
```

### Comparing `meggie-1.5.1/meggie/actions/raw_rereference/dialogs/rereferencingDialogMain.py` & `meggie-1.5.2/meggie/actions/raw_rereference/dialogs/rereferencingDialogMain.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,16 +30,17 @@
         sfreq = raw.info['sfreq']
 
         # fill the combobox
         picks = mne.pick_types(raw.info, eeg=True, meg=False, eog=True)
         ch_names = [ch_name for ch_idx, ch_name in
                     enumerate(raw.info['ch_names']) if ch_idx in picks]
 
+        self.ui.listWidgetChannels.clear()
         for ch_name in ch_names:
-            self.ui.comboBoxChannel.addItem(ch_name)
+            self.ui.listWidgetChannels.addItem(ch_name)
 
         self.batching_widget = BatchingWidget(
             experiment_getter=self._experiment_getter,
             parent=self,
             container=self.ui.groupBoxBatching,
             geometry=self.ui.batchingWidgetPlaceholder.geometry())
         self.ui.gridLayoutBatching.addWidget(self.batching_widget, 0, 0, 1, 1)
@@ -47,30 +48,43 @@
     def _experiment_getter(self):
         return self.experiment
 
     def accept(self):
         experiment = self.experiment
         subject = experiment.active_subject
 
-        selection = self.ui.comboBoxChannel.currentText()
+        if self.ui.radioButtonUseAverage.isChecked():
+            selection = "average"
+        else:
+            selection = [
+                item.text() for item in
+                self.ui.listWidgetChannels.selectedItems()
+            ]
 
         try:
             params = {'selection': selection}
             self.handler(subject, params)
             experiment.save_experiment_settings()
         except Exception as exc:
             exc_messagebox(self.parent, exc)
             return
 
         self.parent.initialize_ui()
         self.close()
 
     def acceptBatch(self):
         experiment = self.experiment
-        selection = self.ui.comboBoxChannel.currentText()
+
+        if self.ui.radioButtonUseAverage.isChecked():
+            selection = "average"
+        else:
+            selection = [
+                item.text() for item in
+                self.ui.listWidgetChannels.selectedItems()
+            ]
 
         selected_subject_names = self.batching_widget.selected_subjects
 
         for name, subject in experiment.subjects.items():
             if name in selected_subject_names:
                 try:
                     params = {'selection': selection}
```

### Comparing `meggie-1.5.1/meggie/actions/raw_rereference/dialogs/rereferencingDialogUi.py` & `meggie-1.5.2/meggie/utilities/dialogs/simpleDialogUi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,99 @@
-# -*- coding: utf-8 -*-
+""" UI layout for simple dialog
+"""
+from PyQt5 import QtCore
+from PyQt5 import QtGui
+from PyQt5 import QtWidgets
+
+class Ui_SimpleDialog(object):
+    """ Contains layout of very simple reusable dialog
+    """
+    def setupUi(self, dialog):
+        dialog.setObjectName("CreateEvokedDialog")
+        dialog.resize(364, 530)
+
+        self.gridLayout = QtWidgets.QGridLayout(dialog)
+        self.gridLayout.setObjectName("gridLayout")
 
-# Form implementation generated from reading ui file 'rereferencingDialogUi.ui'
-#
-# Created by: PyQt5 UI code generator 5.9.2
-#
-# WARNING! All changes made in this file will be lost!
-
-from PyQt5 import QtCore, QtGui, QtWidgets
-
-class Ui_rereferencingDialog(object):
-    def setupUi(self, rereferencingDialog):
-        rereferencingDialog.setObjectName("rereferencingDialog")
-        rereferencingDialog.resize(423, 498)
-        self.gridLayout_2 = QtWidgets.QGridLayout(rereferencingDialog)
-        self.gridLayout_2.setObjectName("gridLayout_2")
-        self.horizontalLayout = QtWidgets.QHBoxLayout()
-        self.horizontalLayout.setObjectName("horizontalLayout")
         spacerItem = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
-        self.horizontalLayout.addItem(spacerItem)
-        self.pushButtonCancel = QtWidgets.QPushButton(rereferencingDialog)
+
+        self.horizontalLayoutButtons = QtWidgets.QHBoxLayout()
+        self.horizontalLayoutButtons.setObjectName("horizontalLayoutButtons")
+        self.horizontalLayoutButtons.addItem(spacerItem)
+
+        self.pushButtonCancel = QtWidgets.QPushButton(dialog)
         self.pushButtonCancel.setObjectName("pushButtonCancel")
-        self.horizontalLayout.addWidget(self.pushButtonCancel)
-        self.pushButtonBatch = QtWidgets.QPushButton(rereferencingDialog)
+        self.horizontalLayoutButtons.addWidget(self.pushButtonCancel)
+
+        self.pushButtonBatch = QtWidgets.QPushButton(dialog)
         self.pushButtonBatch.setObjectName("pushButtonBatch")
-        self.horizontalLayout.addWidget(self.pushButtonBatch)
-        self.pushButtonApply = QtWidgets.QPushButton(rereferencingDialog)
+        self.horizontalLayoutButtons.addWidget(self.pushButtonBatch)
+
+        self.pushButtonApply = QtWidgets.QPushButton(dialog)
         self.pushButtonApply.setObjectName("pushButtonApply")
-        self.horizontalLayout.addWidget(self.pushButtonApply)
-        self.gridLayout_2.addLayout(self.horizontalLayout, 1, 0, 1, 1)
-        self.scrollArea = QtWidgets.QScrollArea(rereferencingDialog)
+        self.horizontalLayoutButtons.addWidget(self.pushButtonApply)
+
+        self.gridLayout.addLayout(self.horizontalLayoutButtons, 2, 0, 1, 1)
+
+        self.scrollArea = QtWidgets.QScrollArea(dialog)
         self.scrollArea.setWidgetResizable(True)
         self.scrollArea.setObjectName("scrollArea")
+
         self.scrollAreaWidgetContents = QtWidgets.QWidget()
-        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 403, 447))
+        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 344, 479))
         self.scrollAreaWidgetContents.setObjectName("scrollAreaWidgetContents")
-        self.gridLayout = QtWidgets.QGridLayout(self.scrollAreaWidgetContents)
-        self.gridLayout.setObjectName("gridLayout")
-        self.groupBoxRereference = QtWidgets.QGroupBox(self.scrollAreaWidgetContents)
-        self.groupBoxRereference.setObjectName("groupBoxRereference")
-        self.formLayout_2 = QtWidgets.QFormLayout(self.groupBoxRereference)
-        self.formLayout_2.setObjectName("formLayout_2")
-        self.labelSelectChannel = QtWidgets.QLabel(self.groupBoxRereference)
-        self.labelSelectChannel.setObjectName("labelSelectChannel")
-        self.formLayout_2.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.labelSelectChannel)
-        self.comboBoxChannel = QtWidgets.QComboBox(self.groupBoxRereference)
-        self.comboBoxChannel.setMinimumSize(QtCore.QSize(120, 0))
-        self.comboBoxChannel.setObjectName("comboBoxChannel")
-        self.comboBoxChannel.addItem("")
-        self.formLayout_2.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.comboBoxChannel)
-        self.gridLayout.addWidget(self.groupBoxRereference, 0, 0, 1, 1)
-        spacerItem1 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.gridLayout.addItem(spacerItem1, 2, 0, 1, 1)
+
+        self.gridLayoutScrollArea = QtWidgets.QGridLayout(self.scrollAreaWidgetContents)
+        self.gridLayoutScrollArea.setObjectName("gridLayoutScrollArea")
+
         self.groupBoxBatching = QtWidgets.QGroupBox(self.scrollAreaWidgetContents)
         self.groupBoxBatching.setObjectName("groupBoxBatching")
+        self.gridLayoutScrollArea.addWidget(self.groupBoxBatching, 1, 0, 1, 1)
+
         self.gridLayoutBatching = QtWidgets.QGridLayout(self.groupBoxBatching)
+        self.gridLayoutBatching.setContentsMargins(9, 9, 9, 9)
         self.gridLayoutBatching.setObjectName("gridLayoutBatching")
+
         self.batchingWidgetPlaceholder = QtWidgets.QWidget(self.groupBoxBatching)
         self.batchingWidgetPlaceholder.setMinimumSize(QtCore.QSize(300, 300))
         self.batchingWidgetPlaceholder.setObjectName("batchingWidgetPlaceholder")
         self.gridLayoutBatching.addWidget(self.batchingWidgetPlaceholder, 0, 0, 1, 1)
-        self.gridLayout.addWidget(self.groupBoxBatching, 1, 0, 1, 1)
+
+        self.groupBoxInfo = QtWidgets.QGroupBox(self.scrollAreaWidgetContents)
+        self.groupBoxInfo.setObjectName("groupBoxInfo")
+
+        self.formLayout = QtWidgets.QFormLayout(self.groupBoxInfo)
+        self.formLayout.setObjectName("formLayout")
+
+        self.labelName = QtWidgets.QLabel(self.groupBoxInfo)
+        self.labelName.setObjectName("labelName")
+        self.formLayout.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.labelName)
+
+        self.lineEditName = QtWidgets.QLineEdit(self.groupBoxInfo)
+        self.lineEditName.setObjectName("lineEditName")
+        self.formLayout.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.lineEditName)
+
+        self.gridLayoutScrollArea.addWidget(self.groupBoxInfo, 0, 0, 1, 1)
+
+        spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.gridLayoutScrollArea.addItem(spacerItem, 2, 0, 1, 1)
+
         self.scrollArea.setWidget(self.scrollAreaWidgetContents)
-        self.gridLayout_2.addWidget(self.scrollArea, 0, 0, 1, 1)
+        self.gridLayout.addWidget(self.scrollArea, 0, 0, 1, 1)
+
+        self.retranslateUi(dialog)
 
-        self.retranslateUi(rereferencingDialog)
-        self.pushButtonCancel.clicked.connect(rereferencingDialog.reject)
-        self.pushButtonApply.clicked.connect(rereferencingDialog.accept)
-        self.pushButtonBatch.clicked.connect(rereferencingDialog.acceptBatch)
-        QtCore.QMetaObject.connectSlotsByName(rereferencingDialog)
+        self.pushButtonCancel.clicked.connect(dialog.close)
+        self.pushButtonApply.clicked.connect(dialog.accept)
+        self.pushButtonBatch.clicked.connect(dialog.acceptBatch)
+        QtCore.QMetaObject.connectSlotsByName(dialog)
 
-    def retranslateUi(self, rereferencingDialog):
+    def retranslateUi(self, dialog):
         _translate = QtCore.QCoreApplication.translate
-        rereferencingDialog.setWindowTitle(_translate("rereferencingDialog", "Meggie - Rereferencing"))
-        self.pushButtonCancel.setText(_translate("rereferencingDialog", "Cancel"))
-        self.pushButtonBatch.setText(_translate("rereferencingDialog", "Batch"))
-        self.pushButtonApply.setText(_translate("rereferencingDialog", "Apply"))
-        self.groupBoxRereference.setTitle(_translate("rereferencingDialog", "Rereferencing options"))
-        self.labelSelectChannel.setText(_translate("rereferencingDialog", "Select channel:"))
-        self.comboBoxChannel.setCurrentText(_translate("rereferencingDialog", "Use average"))
-        self.comboBoxChannel.setItemText(0, _translate("rereferencingDialog", "Use average"))
-        self.groupBoxBatching.setTitle(_translate("rereferencingDialog", "Batching"))
+        dialog.setWindowTitle(_translate("SimpleDialog", "Meggie - Simple dialog"))
+        self.pushButtonCancel.setText(_translate("SimpleDialog", "Cancel"))
+        self.pushButtonBatch.setText(_translate("SimpleDialog", "Batch"))
+        self.pushButtonApply.setText(_translate("SimpleDialog", "Apply"))
+        self.groupBoxBatching.setTitle(_translate("SimpleDialog", "Batching"))
+        self.groupBoxInfo.setTitle(_translate("SimpleDialog", "Info"))
+        self.labelName.setText(_translate("SimpleDialog", "Name:"))
```

### Comparing `meggie-1.5.1/meggie/actions/raw_resample/__init__.py` & `meggie-1.5.2/meggie/actions/raw_resample/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_resample/dialogs/resamplingDialogMain.py` & `meggie-1.5.2/meggie/actions/raw_resample/dialogs/resamplingDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/raw_resample/dialogs/resamplingDialogUi.py` & `meggie-1.5.2/meggie/actions/raw_resample/dialogs/resamplingDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/spectrum_create/__init__.py` & `meggie-1.5.2/meggie/actions/spectrum_create/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/spectrum_create/controller/spectrum.py` & `meggie-1.5.2/meggie/actions/spectrum_create/controller/spectrum.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/spectrum_delete/__init__.py` & `meggie-1.5.2/meggie/actions/spectrum_delete/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/spectrum_delete_from_all/__init__.py` & `meggie-1.5.2/meggie/actions/spectrum_delete_from_all/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/spectrum_group_average/__init__.py` & `meggie-1.5.2/meggie/actions/spectrum_group_average/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/spectrum_group_average/controller/spectrum.py` & `meggie-1.5.2/meggie/actions/spectrum_group_average/controller/spectrum.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/spectrum_info/__init__.py` & `meggie-1.5.2/meggie/actions/spectrum_info/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/spectrum_plot/__init__.py` & `meggie-1.5.2/meggie/actions/spectrum_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/spectrum_plot/controller/spectrum.py` & `meggie-1.5.2/meggie/actions/spectrum_plot/controller/spectrum.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/spectrum_save/__init__.py` & `meggie-1.5.2/meggie/actions/spectrum_save/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/spectrum_save/controller/spectrum.py` & `meggie-1.5.2/meggie/actions/spectrum_save/controller/spectrum.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_create/__init__.py` & `meggie-1.5.2/meggie/actions/tfr_create/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_create/controller/tfr.py` & `meggie-1.5.2/meggie/actions/tfr_create/controller/tfr.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_create/dialogs/TFRDialogMain.py` & `meggie-1.5.2/meggie/actions/tfr_create/dialogs/TFRDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_create/dialogs/TFRDialogUi.py` & `meggie-1.5.2/meggie/actions/tfr_create/dialogs/TFRDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_delete/__init__.py` & `meggie-1.5.2/meggie/actions/tfr_delete/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_delete_from_all/__init__.py` & `meggie-1.5.2/meggie/actions/tfr_delete_from_all/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_group_average/__init__.py` & `meggie-1.5.2/meggie/actions/tfr_group_average/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_group_average/controller/tfr.py` & `meggie-1.5.2/meggie/actions/tfr_group_average/controller/tfr.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_info/__init__.py` & `meggie-1.5.2/meggie/actions/tfr_info/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_plot/__init__.py` & `meggie-1.5.2/meggie/actions/tfr_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_plot/controller/tfr.py` & `meggie-1.5.2/meggie/actions/tfr_plot/controller/tfr.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_plot_tse/__init__.py` & `meggie-1.5.2/meggie/actions/tfr_plot_tse/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_plot_tse/controller/tfr.py` & `meggie-1.5.2/meggie/actions/tfr_plot_tse/controller/tfr.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_save/__init__.py` & `meggie-1.5.2/meggie/actions/tfr_save/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_save/controller/tfr.py` & `meggie-1.5.2/meggie/actions/tfr_save/controller/tfr.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_save_tse/__init__.py` & `meggie-1.5.2/meggie/actions/tfr_save_tse/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/actions/tfr_save_tse/controller/tfr.py` & `meggie-1.5.2/meggie/actions/tfr_save_tse/controller/tfr.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/configuration.json` & `meggie-1.5.2/meggie/configuration.json`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/datatypes/epochs/epochs.py` & `meggie-1.5.2/meggie/datatypes/epochs/epochs.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/datatypes/epochs/tests/test_epochs.py` & `meggie-1.5.2/meggie/datatypes/epochs/tests/test_epochs.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/datatypes/evoked/evoked.py` & `meggie-1.5.2/meggie/datatypes/evoked/evoked.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/datatypes/evoked/tests/test_evoked.py` & `meggie-1.5.2/meggie/datatypes/evoked/tests/test_evoked.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/datatypes/spectrum/spectrum.py` & `meggie-1.5.2/meggie/datatypes/spectrum/spectrum.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/datatypes/spectrum/tests/test_spectrum.py` & `meggie-1.5.2/meggie/datatypes/spectrum/tests/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/datatypes/tfr/tests/test_tfr.py` & `meggie-1.5.2/meggie/datatypes/tfr/tests/test_tfr.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/datatypes/tfr/tfr.py` & `meggie-1.5.2/meggie/datatypes/tfr/tfr.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/experiment.py` & `meggie-1.5.2/meggie/experiment.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainWindowMain.py` & `meggie-1.5.2/meggie/mainWindowMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainWindowUi.py` & `meggie-1.5.2/meggie/mainWindowUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/aboutDialogMain.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/aboutDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/aboutDialogUi.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/aboutDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/actionDialogMain.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/actionDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/actionDialogUi.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/actionDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/activePluginsDialogMain.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/activePluginsDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/activePluginsDialogUi.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/activePluginsDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/addSubjectDialogMain.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/addSubjectDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/addSubjectDialogUi.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/addSubjectDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/channelGroupsDialogMain.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/channelGroupsDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/channelGroupsDialogUi.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/channelGroupsDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/createExperimentDialogMain.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/createExperimentDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/createExperimentDialogUi.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/createExperimentDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/pipelineDialogMain.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/pipelineDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/pipelineDialogUi.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/pipelineDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/preferencesDialogMain.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/preferencesDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dialogs/preferencesDialogUi.py` & `meggie-1.5.2/meggie/mainwindow/dialogs/preferencesDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/dynamic.py` & `meggie-1.5.2/meggie/mainwindow/dynamic.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/mainwindow/preferences.py` & `meggie-1.5.2/meggie/mainwindow/preferences.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/run.py` & `meggie-1.5.2/meggie/run.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/subject.py` & `meggie-1.5.2/meggie/subject.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/tests/test_experiment_and_subject.py` & `meggie-1.5.2/meggie/tests/test_experiment_and_subject.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/channels.py` & `meggie-1.5.2/meggie/utilities/channels.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/compare.py` & `meggie-1.5.2/meggie/utilities/compare.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/datatype.py` & `meggie-1.5.2/meggie/utilities/datatype.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/debug.py` & `meggie-1.5.2/meggie/utilities/debug.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/TFROutputOptionsMain.py` & `meggie-1.5.2/meggie/utilities/dialogs/TFROutputOptionsMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/TFROutputOptionsUi.py` & `meggie-1.5.2/meggie/utilities/dialogs/TFROutputOptionsUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/bitSelectionDialogMain.py` & `meggie-1.5.2/meggie/utilities/dialogs/bitSelectionDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/bitSelectionDialogUi.py` & `meggie-1.5.2/meggie/utilities/dialogs/bitSelectionDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/groupSelectionDialogMain.py` & `meggie-1.5.2/meggie/utilities/dialogs/groupSelectionDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/groupSelectionDialogUi.py` & `meggie-1.5.2/meggie/utilities/dialogs/groupSelectionDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/outputOptionsMain.py` & `meggie-1.5.2/meggie/utilities/dialogs/outputOptionsMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/outputOptionsUi.py` & `meggie-1.5.2/meggie/utilities/dialogs/outputOptionsUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogMain.py` & `meggie-1.5.2/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogUi.py` & `meggie-1.5.2/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/powerSpectrumDialogMain.py` & `meggie-1.5.2/meggie/utilities/dialogs/powerSpectrumDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/powerSpectrumDialogUi.py` & `meggie-1.5.2/meggie/utilities/dialogs/powerSpectrumDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/shortMessageBoxMain.py` & `meggie-1.5.2/meggie/utilities/dialogs/shortMessageBoxMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/shortMessageBoxUi.py` & `meggie-1.5.2/meggie/utilities/dialogs/shortMessageBoxUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/shortQuestionBoxMain.py` & `meggie-1.5.2/meggie/utilities/dialogs/shortQuestionBoxMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/shortQuestionBoxUi.py` & `meggie-1.5.2/meggie/utilities/dialogs/shortQuestionBoxUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/simpleDialogMain.py` & `meggie-1.5.2/meggie/utilities/dialogs/simpleDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/singleChannelDialogMain.py` & `meggie-1.5.2/meggie/utilities/dialogs/singleChannelDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/dialogs/singleChannelDialogUi.py` & `meggie-1.5.2/meggie/utilities/dialogs/singleChannelDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/events.py` & `meggie-1.5.2/meggie/utilities/events.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/filemanager.py` & `meggie-1.5.2/meggie/utilities/filemanager.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/formats.py` & `meggie-1.5.2/meggie/utilities/formats.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/generate_experiments.py` & `meggie-1.5.2/meggie/utilities/generate_experiments.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/measurement_info.py` & `meggie-1.5.2/meggie/utilities/measurement_info.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/messaging.py` & `meggie-1.5.2/meggie/utilities/messaging.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/names.py` & `meggie-1.5.2/meggie/utilities/names.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/plotting.py` & `meggie-1.5.2/meggie/utilities/plotting.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/tests/test_channels.py` & `meggie-1.5.2/meggie/utilities/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/tests/test_events.py` & `meggie-1.5.2/meggie/utilities/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/tests/test_filemanager.py` & `meggie-1.5.2/meggie/utilities/tests/test_filemanager.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/tests/test_measurement_info.py` & `meggie-1.5.2/meggie/utilities/tests/test_measurement_info.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/tests/test_names.py` & `meggie-1.5.2/meggie/utilities/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/threading.py` & `meggie-1.5.2/meggie/utilities/threading.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/units.py` & `meggie-1.5.2/meggie/utilities/units.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/validators.py` & `meggie-1.5.2/meggie/utilities/validators.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/widgets/batchingWidgetMain.py` & `meggie-1.5.2/meggie/utilities/widgets/batchingWidgetMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie/utilities/widgets/batchingWidgetUi.py` & `meggie-1.5.2/meggie/utilities/widgets/batchingWidgetUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/meggie.egg-info/SOURCES.txt` & `meggie-1.5.2/meggie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meggie-1.5.1/setup.py` & `meggie-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 description = "User-friendly graphical user interface to do M/EEG analysis"
 
 setup(
     name='meggie',
-    version='1.5.1',
+    version='1.5.2',
     description=description,
     long_description=description,
     long_description_content_type="text/plain",
     author='CIBR',
     author_email='erkka.heinila@jyu.fi',
     url='https://github.com/cibr-jyu/meggie',
     license='BSD',
```

