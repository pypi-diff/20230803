# Comparing `tmp/madam-mam-0.7.0.tar.gz` & `tmp/madam_mam-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madam-mam-0.7.0.tar", max compression
+gzip compressed data, was "madam_mam-0.7.2.tar", max compression
```

## Comparing `madam-mam-0.7.0.tar` & `madam_mam-0.7.2.tar`

### file list

```diff
@@ -1,91 +1,90 @@
--rw-r--r--   0        0        0     5405 2021-11-24 14:06:58.888065 madam-mam-0.7.0/README.md
--rw-r--r--   0        0        0      725 2021-12-02 10:29:32.042062 madam-mam-0.7.0/madam/__init__.py
--rw-r--r--   0        0        0     1946 2021-12-02 10:01:46.624368 madam-mam-0.7.0/madam/__main__.py
--rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam-mam-0.7.0/madam/adapters/__init__.py
--rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam-mam-0.7.0/madam/adapters/agents/__init__.py
--rw-r--r--   0        0        0     5275 2021-11-03 09:04:25.275451 madam-mam-0.7.0/madam/adapters/agents/bash.py
--rw-r--r--   0        0        0     6979 2021-11-30 10:48:21.579676 madam-mam-0.7.0/madam/adapters/agents/concatenate.py
--rw-r--r--   0        0        0     5236 2021-11-03 09:04:25.279451 madam-mam-0.7.0/madam/adapters/agents/ffmpeg.py
--rw-r--r--   0        0        0     6446 2021-11-03 09:04:25.279451 madam-mam-0.7.0/madam/adapters/agents/imagemagick.py
--rw-r--r--   0        0        0     6639 2021-11-30 14:16:29.510932 madam-mam-0.7.0/madam/adapters/agents/mediainfo.py
--rw-r--r--   0        0        0     5354 2021-11-03 09:04:25.279451 madam-mam-0.7.0/madam/adapters/agents/melt.py
--rw-r--r--   0        0        0     5266 2021-11-03 09:04:25.279451 madam-mam-0.7.0/madam/adapters/agents/python.py
--rw-r--r--   0        0        0     5658 2021-11-30 10:53:59.056698 madam-mam-0.7.0/madam/adapters/agents/scanfolder.py
--rw-r--r--   0        0        0     7858 2021-11-30 13:56:34.503835 madam-mam-0.7.0/madam/adapters/agents/scenes.py
--rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam-mam-0.7.0/madam/adapters/bpmn/__init__.py
--rw-r--r--   0        0        0     2156 2021-07-02 15:46:26.474963 madam-mam-0.7.0/madam/adapters/bpmn/assets/BPMN20.xsd
--rw-r--r--   0        0        0     3973 2021-07-02 15:46:26.454963 madam-mam-0.7.0/madam/adapters/bpmn/assets/BPMNDI.xsd
--rw-r--r--   0        0        0     1314 2021-07-02 15:46:26.482963 madam-mam-0.7.0/madam/adapters/bpmn/assets/DC.xsd
--rw-r--r--   0        0        0     3440 2021-07-02 15:46:26.466963 madam-mam-0.7.0/madam/adapters/bpmn/assets/DI.xsd
--rw-r--r--   0        0        0    73472 2021-07-02 15:46:26.498963 madam-mam-0.7.0/madam/adapters/bpmn/assets/Semantic.xsd
--rw-r--r--   0        0        0     6354 2021-09-09 14:40:59.130653 madam-mam-0.7.0/madam/adapters/bpmn/engine.py
--rw-r--r--   0        0        0     5058 2021-11-02 14:00:09.027293 madam-mam-0.7.0/madam/adapters/bpmn/parser.py
--rw-r--r--   0        0        0     1431 2021-11-02 13:58:46.010733 madam-mam-0.7.0/madam/adapters/config.py
--rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam-mam-0.7.0/madam/adapters/interfaces/__init__.py
--rw-r--r--   0        0        0     1523 2021-09-06 10:05:01.061344 madam-mam-0.7.0/madam/adapters/interfaces/agents.py
--rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam-mam-0.7.0/madam/adapters/process/__init__.py
--rw-r--r--   0        0        0     6885 2021-11-02 15:58:06.871577 madam-mam-0.7.0/madam/adapters/process/applications.py
--rw-r--r--   0        0        0     5367 2021-08-05 12:54:38.821297 madam-mam-0.7.0/madam/adapters/process/docker_api.py
--rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam-mam-0.7.0/madam/adapters/repository/__init__.py
--rw-r--r--   0        0        0    10992 2021-11-02 13:57:22.102150 madam-mam-0.7.0/madam/adapters/repository/applications.py
--rw-r--r--   0        0        0      199 2021-08-17 14:49:51.308963 madam-mam-0.7.0/madam/adapters/repository/assets/migrations/00001.init_tables.rollback.sql
--rw-r--r--   0        0        0     4128 2021-09-30 15:18:08.368183 madam-mam-0.7.0/madam/adapters/repository/assets/migrations/00001.init_tables.sql
--rw-r--r--   0        0        0     8118 2021-11-02 13:57:22.186151 madam-mam-0.7.0/madam/adapters/repository/jobs.py
--rw-r--r--   0        0        0    10827 2021-11-02 14:11:37.027525 madam-mam-0.7.0/madam/adapters/repository/postgresql.py
--rw-r--r--   0        0        0     7287 2021-11-02 13:57:22.130150 madam-mam-0.7.0/madam/adapters/repository/timers.py
--rw-r--r--   0        0        0    11287 2021-11-30 09:06:53.107885 madam-mam-0.7.0/madam/adapters/repository/watchfolders.py
--rw-r--r--   0        0        0     6566 2021-11-02 13:57:22.118150 madam-mam-0.7.0/madam/adapters/repository/workflow_instances.py
--rw-r--r--   0        0        0     6293 2021-09-07 13:59:09.550655 madam-mam-0.7.0/madam/adapters/repository/workflows.py
--rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam-mam-0.7.0/madam/domains/__init__.py
--rw-r--r--   0        0        0     4754 2021-11-02 13:57:22.226151 madam-mam-0.7.0/madam/domains/agents.py
--rw-r--r--   0        0        0     4464 2021-12-02 10:01:46.544367 madam-mam-0.7.0/madam/domains/application.py
--rw-r--r--   0        0        0     8960 2021-11-02 14:52:21.673085 madam-mam-0.7.0/madam/domains/applications.py
--rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam-mam-0.7.0/madam/domains/entities/__init__.py
--rw-r--r--   0        0        0      968 2021-09-21 07:52:45.954757 madam-mam-0.7.0/madam/domains/entities/agent.py
--rw-r--r--   0        0        0     1918 2021-09-21 07:56:51.067682 madam-mam-0.7.0/madam/domains/entities/application.py
--rw-r--r--   0        0        0     1183 2021-09-10 12:54:16.706229 madam-mam-0.7.0/madam/domains/entities/constants.py
--rw-r--r--   0        0        0     3848 2021-09-09 12:30:16.631361 madam-mam-0.7.0/madam/domains/entities/events.py
--rw-r--r--   0        0        0     1342 2021-09-09 12:46:33.896690 madam-mam-0.7.0/madam/domains/entities/job.py
--rw-r--r--   0        0        0     1681 2021-11-25 14:02:58.022893 madam-mam-0.7.0/madam/domains/entities/runner.py
--rw-r--r--   0        0        0     1436 2021-09-09 12:48:23.413293 madam-mam-0.7.0/madam/domains/entities/timer.py
--rw-r--r--   0        0        0     1590 2021-09-09 12:48:23.401293 madam-mam-0.7.0/madam/domains/entities/watchfolder.py
--rw-r--r--   0        0        0     1658 2021-09-09 12:58:59.092727 madam-mam-0.7.0/madam/domains/entities/workflow.py
--rw-r--r--   0        0        0     1456 2021-09-09 12:58:50.500681 madam-mam-0.7.0/madam/domains/entities/workflow_instance.py
--rw-r--r--   0        0        0     3304 2021-11-02 13:54:04.000684 madam-mam-0.7.0/madam/domains/events.py
--rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam-mam-0.7.0/madam/domains/interfaces/__init__.py
--rw-r--r--   0        0        0     2061 2021-09-10 11:11:40.165959 madam-mam-0.7.0/madam/domains/interfaces/agents.py
--rw-r--r--   0        0        0     2813 2021-09-07 13:16:50.424799 madam-mam-0.7.0/madam/domains/interfaces/bpmn.py
--rw-r--r--   0        0        0      781 2021-09-09 12:31:14.623662 madam-mam-0.7.0/madam/domains/interfaces/events.py
--rw-r--r--   0        0        0      680 2021-11-02 14:39:23.740789 madam-mam-0.7.0/madam/domains/interfaces/process/__init__.py
--rw-r--r--   0        0        0     2199 2021-09-16 15:37:41.415958 madam-mam-0.7.0/madam/domains/interfaces/process/applications.py
--rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam-mam-0.7.0/madam/domains/interfaces/repository/__init__.py
--rw-r--r--   0        0        0     4015 2021-09-02 10:10:04.512531 madam-mam-0.7.0/madam/domains/interfaces/repository/applications.py
--rw-r--r--   0        0        0     1195 2021-08-31 09:13:18.642807 madam-mam-0.7.0/madam/domains/interfaces/repository/config.py
--rw-r--r--   0        0        0     3748 2021-09-02 10:10:04.184529 madam-mam-0.7.0/madam/domains/interfaces/repository/jobs.py
--rw-r--r--   0        0        0     3436 2021-09-02 10:10:04.384530 madam-mam-0.7.0/madam/domains/interfaces/repository/timers.py
--rw-r--r--   0        0        0     3194 2021-09-02 10:10:04.436530 madam-mam-0.7.0/madam/domains/interfaces/repository/watchfolders.py
--rw-r--r--   0        0        0     3288 2021-09-02 10:10:04.380530 madam-mam-0.7.0/madam/domains/interfaces/repository/workflow_instances.py
--rw-r--r--   0        0        0     3136 2021-09-02 10:10:04.428530 madam-mam-0.7.0/madam/domains/interfaces/repository/workflows.py
--rw-r--r--   0        0        0     6848 2021-09-09 10:10:38.218945 madam-mam-0.7.0/madam/domains/jobs.py
--rw-r--r--   0        0        0    11839 2021-11-25 14:06:56.200276 madam-mam-0.7.0/madam/domains/timers.py
--rw-r--r--   0        0        0    11923 2021-11-24 13:35:25.797373 madam-mam-0.7.0/madam/domains/watchfolders.py
--rw-r--r--   0        0        0    13305 2021-11-02 13:56:30.949785 madam-mam-0.7.0/madam/domains/workflow_instances.py
--rw-r--r--   0        0        0     7328 2021-09-09 09:43:22.520593 madam-mam-0.7.0/madam/domains/workflows.py
--rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam-mam-0.7.0/madam/libs/__init__.py
--rw-r--r--   0        0        0     2982 2021-11-18 13:48:06.767347 madam-mam-0.7.0/madam/libs/http.py
--rw-r--r--   0        0        0     3648 2021-09-08 16:03:21.676933 madam-mam-0.7.0/madam/libs/iso8601.py
--rw-r--r--   0        0        0     2482 2021-11-02 14:00:45.567534 madam-mam-0.7.0/madam/libs/serialize.py
--rw-r--r--   0        0        0     1390 2021-08-05 12:54:38.821297 madam-mam-0.7.0/madam/libs/timecode.py
--rw-r--r--   0        0        0      680 2021-11-02 14:39:24.032791 madam-mam-0.7.0/madam/slots/__init__.py
--rwxr-xr-x   0        0        0    50245 2021-12-02 10:01:46.608368 madam-mam-0.7.0/madam/slots/cli.py
--rw-r--r--   0        0        0      680 2021-11-02 14:39:24.312792 madam-mam-0.7.0/madam/slots/graphql/__init__.py
--rw-r--r--   0        0        0     3659 2021-11-02 13:56:30.973785 madam-mam-0.7.0/madam/slots/graphql/api.py
--rw-r--r--   0        0        0    10036 2021-11-19 15:09:43.154405 madam-mam-0.7.0/madam/slots/graphql/assets/schema.graphql
--rw-r--r--   0        0        0    17305 2021-11-19 15:09:43.154405 madam-mam-0.7.0/madam/slots/graphql/mutation.py
--rw-r--r--   0        0        0    15703 2021-11-19 15:09:43.154405 madam-mam-0.7.0/madam/slots/graphql/query.py
--rw-r--r--   0        0        0     1361 2021-09-09 12:21:44.244708 madam-mam-0.7.0/madam/slots/graphql/scalar.py
--rw-r--r--   0        0        0     2429 2021-12-02 10:01:46.560367 madam-mam-0.7.0/madam/slots/graphql/server.py
--rw-r--r--   0        0        0     2991 2021-11-19 15:09:43.154405 madam-mam-0.7.0/madam/slots/graphql/subscription.py
--rw-r--r--   0        0        0     1883 2021-12-02 10:29:31.922062 madam-mam-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7239 2021-12-02 10:29:59.843832 madam-mam-0.7.0/setup.py
--rw-r--r--   0        0        0     6614 2021-12-02 10:29:59.844730 madam-mam-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     5696 2023-08-03 10:18:39.415629 madam_mam-0.7.2/README.md
+-rw-r--r--   0        0        0      725 2023-08-03 09:46:49.042003 madam_mam-0.7.2/madam/__init__.py
+-rw-r--r--   0        0        0     1946 2023-01-17 17:48:35.571198 madam_mam-0.7.2/madam/__main__.py
+-rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam_mam-0.7.2/madam/adapters/__init__.py
+-rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam_mam-0.7.2/madam/adapters/agents/__init__.py
+-rw-r--r--   0        0        0     5292 2023-08-02 09:10:04.331649 madam_mam-0.7.2/madam/adapters/agents/bash.py
+-rw-r--r--   0        0        0     6971 2023-08-02 09:10:24.495741 madam_mam-0.7.2/madam/adapters/agents/concatenate.py
+-rw-r--r--   0        0        0     5253 2023-08-02 09:11:31.012045 madam_mam-0.7.2/madam/adapters/agents/ffmpeg.py
+-rw-r--r--   0        0        0     6463 2023-08-02 09:12:09.256221 madam_mam-0.7.2/madam/adapters/agents/imagemagick.py
+-rw-r--r--   0        0        0     6656 2023-08-02 09:12:29.008312 madam_mam-0.7.2/madam/adapters/agents/mediainfo.py
+-rw-r--r--   0        0        0     5371 2023-08-02 09:12:45.248387 madam_mam-0.7.2/madam/adapters/agents/melt.py
+-rw-r--r--   0        0        0     5283 2023-08-02 09:13:00.976459 madam_mam-0.7.2/madam/adapters/agents/python.py
+-rw-r--r--   0        0        0     5650 2023-08-02 09:13:14.484522 madam_mam-0.7.2/madam/adapters/agents/scanfolder.py
+-rw-r--r--   0        0        0     7850 2023-08-02 09:13:27.028580 madam_mam-0.7.2/madam/adapters/agents/scenes.py
+-rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam_mam-0.7.2/madam/adapters/bpmn/__init__.py
+-rw-r--r--   0        0        0     2156 2021-07-02 15:46:26.474963 madam_mam-0.7.2/madam/adapters/bpmn/assets/BPMN20.xsd
+-rw-r--r--   0        0        0     3973 2021-07-02 15:46:26.454963 madam_mam-0.7.2/madam/adapters/bpmn/assets/BPMNDI.xsd
+-rw-r--r--   0        0        0     1314 2021-07-02 15:46:26.482963 madam_mam-0.7.2/madam/adapters/bpmn/assets/DC.xsd
+-rw-r--r--   0        0        0     3440 2021-07-02 15:46:26.466963 madam_mam-0.7.2/madam/adapters/bpmn/assets/DI.xsd
+-rw-r--r--   0        0        0    73472 2021-07-02 15:46:26.498963 madam_mam-0.7.2/madam/adapters/bpmn/assets/Semantic.xsd
+-rw-r--r--   0        0        0     6354 2021-09-09 14:40:59.130653 madam_mam-0.7.2/madam/adapters/bpmn/engine.py
+-rw-r--r--   0        0        0     5058 2021-11-02 14:00:09.027293 madam_mam-0.7.2/madam/adapters/bpmn/parser.py
+-rw-r--r--   0        0        0     1431 2021-11-02 13:58:46.010733 madam_mam-0.7.2/madam/adapters/config.py
+-rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam_mam-0.7.2/madam/adapters/interfaces/__init__.py
+-rw-r--r--   0        0        0     1523 2021-09-06 10:05:01.061344 madam_mam-0.7.2/madam/adapters/interfaces/agents.py
+-rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam_mam-0.7.2/madam/adapters/process/__init__.py
+-rw-r--r--   0        0        0     6884 2023-08-02 09:47:16.479164 madam_mam-0.7.2/madam/adapters/process/applications.py
+-rw-r--r--   0        0        0     5366 2023-08-02 09:47:16.479164 madam_mam-0.7.2/madam/adapters/process/docker_api.py
+-rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam_mam-0.7.2/madam/adapters/repository/__init__.py
+-rw-r--r--   0        0        0    10992 2023-08-02 09:47:16.479164 madam_mam-0.7.2/madam/adapters/repository/applications.py
+-rw-r--r--   0        0        0      199 2021-08-17 14:49:51.308963 madam_mam-0.7.2/madam/adapters/repository/assets/migrations/00001.init_tables.rollback.sql
+-rw-r--r--   0        0        0     4128 2021-09-30 15:18:08.368183 madam_mam-0.7.2/madam/adapters/repository/assets/migrations/00001.init_tables.sql
+-rw-r--r--   0        0        0     8118 2023-08-02 09:47:16.479164 madam_mam-0.7.2/madam/adapters/repository/jobs.py
+-rw-r--r--   0        0        0    10829 2023-08-02 10:07:48.203249 madam_mam-0.7.2/madam/adapters/repository/postgresql.py
+-rw-r--r--   0        0        0     7287 2021-11-02 13:57:22.130150 madam_mam-0.7.2/madam/adapters/repository/timers.py
+-rw-r--r--   0        0        0    11287 2021-11-30 09:06:53.107885 madam_mam-0.7.2/madam/adapters/repository/watchfolders.py
+-rw-r--r--   0        0        0     6566 2021-11-02 13:57:22.118150 madam_mam-0.7.2/madam/adapters/repository/workflow_instances.py
+-rw-r--r--   0        0        0     6293 2021-09-07 13:59:09.550655 madam_mam-0.7.2/madam/adapters/repository/workflows.py
+-rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam_mam-0.7.2/madam/domains/__init__.py
+-rw-r--r--   0        0        0     4754 2021-11-02 13:57:22.226151 madam_mam-0.7.2/madam/domains/agents.py
+-rw-r--r--   0        0        0     4464 2021-12-02 10:01:46.544367 madam_mam-0.7.2/madam/domains/application.py
+-rw-r--r--   0        0        0     8960 2021-11-02 14:52:21.673085 madam_mam-0.7.2/madam/domains/applications.py
+-rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam_mam-0.7.2/madam/domains/entities/__init__.py
+-rw-r--r--   0        0        0      968 2021-09-21 07:52:45.954757 madam_mam-0.7.2/madam/domains/entities/agent.py
+-rw-r--r--   0        0        0     1918 2021-09-21 07:56:51.067682 madam_mam-0.7.2/madam/domains/entities/application.py
+-rw-r--r--   0        0        0     1183 2021-09-10 12:54:16.706229 madam_mam-0.7.2/madam/domains/entities/constants.py
+-rw-r--r--   0        0        0     3848 2021-09-09 12:30:16.631361 madam_mam-0.7.2/madam/domains/entities/events.py
+-rw-r--r--   0        0        0     1342 2021-09-09 12:46:33.896690 madam_mam-0.7.2/madam/domains/entities/job.py
+-rw-r--r--   0        0        0     1681 2021-11-25 14:02:58.022893 madam_mam-0.7.2/madam/domains/entities/runner.py
+-rw-r--r--   0        0        0     1436 2021-09-09 12:48:23.413293 madam_mam-0.7.2/madam/domains/entities/timer.py
+-rw-r--r--   0        0        0     1590 2021-09-09 12:48:23.401293 madam_mam-0.7.2/madam/domains/entities/watchfolder.py
+-rw-r--r--   0        0        0     1658 2021-09-09 12:58:59.092727 madam_mam-0.7.2/madam/domains/entities/workflow.py
+-rw-r--r--   0        0        0     1456 2021-09-09 12:58:50.500681 madam_mam-0.7.2/madam/domains/entities/workflow_instance.py
+-rw-r--r--   0        0        0     3304 2021-11-02 13:54:04.000684 madam_mam-0.7.2/madam/domains/events.py
+-rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam_mam-0.7.2/madam/domains/interfaces/__init__.py
+-rw-r--r--   0        0        0     2061 2021-09-10 11:11:40.165959 madam_mam-0.7.2/madam/domains/interfaces/agents.py
+-rw-r--r--   0        0        0     2813 2021-09-07 13:16:50.424799 madam_mam-0.7.2/madam/domains/interfaces/bpmn.py
+-rw-r--r--   0        0        0      781 2021-09-09 12:31:14.623662 madam_mam-0.7.2/madam/domains/interfaces/events.py
+-rw-r--r--   0        0        0      680 2021-11-02 14:39:23.740789 madam_mam-0.7.2/madam/domains/interfaces/process/__init__.py
+-rw-r--r--   0        0        0     2199 2021-09-16 15:37:41.415958 madam_mam-0.7.2/madam/domains/interfaces/process/applications.py
+-rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam_mam-0.7.2/madam/domains/interfaces/repository/__init__.py
+-rw-r--r--   0        0        0     4015 2021-09-02 10:10:04.512531 madam_mam-0.7.2/madam/domains/interfaces/repository/applications.py
+-rw-r--r--   0        0        0     1195 2021-08-31 09:13:18.642807 madam_mam-0.7.2/madam/domains/interfaces/repository/config.py
+-rw-r--r--   0        0        0     3748 2021-09-02 10:10:04.184529 madam_mam-0.7.2/madam/domains/interfaces/repository/jobs.py
+-rw-r--r--   0        0        0     3436 2021-09-02 10:10:04.384530 madam_mam-0.7.2/madam/domains/interfaces/repository/timers.py
+-rw-r--r--   0        0        0     3194 2021-09-02 10:10:04.436530 madam_mam-0.7.2/madam/domains/interfaces/repository/watchfolders.py
+-rw-r--r--   0        0        0     3288 2021-09-02 10:10:04.380530 madam_mam-0.7.2/madam/domains/interfaces/repository/workflow_instances.py
+-rw-r--r--   0        0        0     3136 2021-09-02 10:10:04.428530 madam_mam-0.7.2/madam/domains/interfaces/repository/workflows.py
+-rw-r--r--   0        0        0     6848 2021-09-09 10:10:38.218945 madam_mam-0.7.2/madam/domains/jobs.py
+-rw-r--r--   0        0        0    11839 2021-11-25 14:06:56.200276 madam_mam-0.7.2/madam/domains/timers.py
+-rw-r--r--   0        0        0    11923 2021-11-24 13:35:25.797373 madam_mam-0.7.2/madam/domains/watchfolders.py
+-rw-r--r--   0        0        0    13305 2021-11-02 13:56:30.949785 madam_mam-0.7.2/madam/domains/workflow_instances.py
+-rw-r--r--   0        0        0     7328 2021-09-09 09:43:22.520593 madam_mam-0.7.2/madam/domains/workflows.py
+-rw-r--r--   0        0        0      680 2021-11-23 14:25:51.549049 madam_mam-0.7.2/madam/libs/__init__.py
+-rw-r--r--   0        0        0     2923 2023-08-02 09:21:34.935674 madam_mam-0.7.2/madam/libs/http.py
+-rw-r--r--   0        0        0     3648 2021-09-08 16:03:21.676933 madam_mam-0.7.2/madam/libs/iso8601.py
+-rw-r--r--   0        0        0     2482 2021-11-02 14:00:45.567534 madam_mam-0.7.2/madam/libs/serialize.py
+-rw-r--r--   0        0        0     1390 2021-08-05 12:54:38.821297 madam_mam-0.7.2/madam/libs/timecode.py
+-rw-r--r--   0        0        0      680 2021-11-02 14:39:24.032791 madam_mam-0.7.2/madam/slots/__init__.py
+-rwxr-xr-x   0        0        0    50245 2023-08-02 10:05:44.270945 madam_mam-0.7.2/madam/slots/cli.py
+-rw-r--r--   0        0        0      680 2021-11-02 14:39:24.312792 madam_mam-0.7.2/madam/slots/graphql/__init__.py
+-rw-r--r--   0        0        0     3659 2021-11-02 13:56:30.973785 madam_mam-0.7.2/madam/slots/graphql/api.py
+-rw-r--r--   0        0        0    10036 2021-11-19 15:09:43.154405 madam_mam-0.7.2/madam/slots/graphql/assets/schema.graphql
+-rw-r--r--   0        0        0    17185 2023-08-02 09:19:11.897086 madam_mam-0.7.2/madam/slots/graphql/mutation.py
+-rw-r--r--   0        0        0    15583 2023-08-02 09:20:50.118910 madam_mam-0.7.2/madam/slots/graphql/query.py
+-rw-r--r--   0        0        0     1361 2021-09-09 12:21:44.244708 madam_mam-0.7.2/madam/slots/graphql/scalar.py
+-rw-r--r--   0        0        0     2429 2021-12-02 10:01:46.560367 madam_mam-0.7.2/madam/slots/graphql/server.py
+-rw-r--r--   0        0        0     2983 2023-08-02 09:21:07.491211 madam_mam-0.7.2/madam/slots/graphql/subscription.py
+-rw-r--r--   0        0        0     2446 2023-08-03 09:46:48.934003 madam_mam-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6956 1970-01-01 00:00:00.000000 madam_mam-0.7.2/PKG-INFO
```

### Comparing `madam-mam-0.7.0/README.md` & `madam_mam-0.7.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -102,14 +102,18 @@
 
     curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python
 
 Install Python dependencies:
 
     poetry install --no-root
 
+Copy `bin/pre-commit.sh` for pre-commmit git hooks:
+
+    cp bin/pre-commit.sh .git/hooks/pre-commit
+
 You can use the madam-cli dev command:
 
     ./bin/madam-cli
 
 Get `bin/madam-cli` bash shell completion:
 
     _MADAM_CLI_COMPLETE=source_bash bin/madam-cli > madam-cli-complete.sh
@@ -157,14 +161,19 @@
 
 ### Build MADAM python package and Docker image
 
     make build
 
 The wheel package will be build in the `dist` directory.
 
+Push docker image on private registry:
+
+    docker image tag madam:[version] registry_hostname:registry_port/madam:[version]
+    docker push registry_hostname:registry_port/madam:[version]
+
 ## Deploy MADAM as local docker container
 
 To deploy MADAM container on localhost:
 
     make deploy
 
 ## Check static type and code quality
```

#### html2text {}

```diff
@@ -33,35 +33,38 @@
 a the `madam` cli command available: madam or madam --help will display command
 usage. To have bash completion, you can type: _MADAM_COMPLETE=source_bash madam
 > madam-complete.sh sudo cp madam-complete.sh /etc/bash_completion.d/. For
 another shell, replace `source_bash` by `source_zsh` or `source_fish` ###
 Development environment Install [Poetry](https://python-poetry.org/) with the
 custom installer: curl -sSL https://raw.githubusercontent.com/python-poetry/
 poetry/master/get-poetry.py | python Install Python dependencies: poetry
-install --no-root You can use the madam-cli dev command: ./bin/madam-cli Get
-`bin/madam-cli` bash shell completion: _MADAM_CLI_COMPLETE=source_bash bin/
-madam-cli > madam-cli-complete.sh sudo cp madam-cli-complete.sh /etc/
-bash_completion.d/. For another shell, replace `source_bash` by `source_zsh` or
-`source_fish` ### Configuration Make a copy of the environment config example
-file: cp .env.example .env Edit `.env` to suit your needs, then: export $(grep
--v '^#' .env | xargs -d '\n') Make a copy of the Ansible inventory example
-file: cp hosts.yaml.example hosts.yaml Edit `hosts.yaml` to suit your needs.
-Make a copy of the MADAM config example file: cp madam.yaml.example madam.yaml
-Edit `madam.yaml` to suit your needs. Make a copy of the MADAM config example
-file for the test environment: cp madam_tests.yaml.example madam_tests.yaml
-Edit `madam_tests.yaml` to suit your needs. Make a copy of the MADAM config
-example file for the local deploy: cp madam_deploy.yaml.example
-madam_deploy.yaml Edit `madam_deploy.yaml` to suit your needs. ### Set and tag
-project version in Git ./bin/release.sh 1.0.0 ### Build MADAM python package
-and Docker image make build The wheel package will be build in the `dist`
-directory. ## Deploy MADAM as local docker container To deploy MADAM container
-on localhost: make deploy ## Check static type and code quality make check ##
-Run tests Run all [pytest](https://docs.pytest.org) tests with: make tests Run
-only some tests by using `bin/tests.sh`: bin/tests.sh tests/domains/
-test_workflows.py::test_create ## Database setup Set `DATABASE_URL` and
-`DATABASE_URL_TESTS` environment variable in `.env` file:
-DATABASE_URL=postgresql://postgres:xxxxx@hostname:5432/madam?sslmode=allow
-DATABASE_URL_TESTS=postgresql://postgres:xxxxx@hostname:5432/
-madam_tests?sslmode=allow ### Migrations scripts Add/Edit scripts in
+install --no-root Copy `bin/pre-commit.sh` for pre-commmit git hooks: cp bin/
+pre-commit.sh .git/hooks/pre-commit You can use the madam-cli dev command: ./
+bin/madam-cli Get `bin/madam-cli` bash shell completion:
+_MADAM_CLI_COMPLETE=source_bash bin/madam-cli > madam-cli-complete.sh sudo cp
+madam-cli-complete.sh /etc/bash_completion.d/. For another shell, replace
+`source_bash` by `source_zsh` or `source_fish` ### Configuration Make a copy of
+the environment config example file: cp .env.example .env Edit `.env` to suit
+your needs, then: export $(grep -v '^#' .env | xargs -d '\n') Make a copy of
+the Ansible inventory example file: cp hosts.yaml.example hosts.yaml Edit
+`hosts.yaml` to suit your needs. Make a copy of the MADAM config example file:
+cp madam.yaml.example madam.yaml Edit `madam.yaml` to suit your needs. Make a
+copy of the MADAM config example file for the test environment: cp
+madam_tests.yaml.example madam_tests.yaml Edit `madam_tests.yaml` to suit your
+needs. Make a copy of the MADAM config example file for the local deploy: cp
+madam_deploy.yaml.example madam_deploy.yaml Edit `madam_deploy.yaml` to suit
+your needs. ### Set and tag project version in Git ./bin/release.sh 1.0.0 ###
+Build MADAM python package and Docker image make build The wheel package will
+be build in the `dist` directory. Push docker image on private registry: docker
+image tag madam:[version] registry_hostname:registry_port/madam:[version]
+docker push registry_hostname:registry_port/madam:[version] ## Deploy MADAM as
+local docker container To deploy MADAM container on localhost: make deploy ##
+Check static type and code quality make check ## Run tests Run all [pytest]
+(https://docs.pytest.org) tests with: make tests Run only some tests by using
+`bin/tests.sh`: bin/tests.sh tests/domains/test_workflows.py::test_create ##
+Database setup Set `DATABASE_URL` and `DATABASE_URL_TESTS` environment variable
+in `.env` file: DATABASE_URL=postgresql://postgres:xxxxx@hostname:5432/
+madam?sslmode=allow DATABASE_URL_TESTS=postgresql://postgres:xxxxx@hostname:
+5432/madam_tests?sslmode=allow ### Migrations scripts Add/Edit scripts in
 `resources/migrations` directory: # version.name.[rollback].sql
 00001.init_tables.sql 00001.init_tables.rollback.sql ### Migrate commands make
 databases make databases_rollback make databases_list
```

### Comparing `madam-mam-0.7.0/madam/__init__.py` & `madam_mam-0.7.2/madam/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with MADAM.  If not, see <https://www.gnu.org/licenses/>.
 
 """
 Madam package
 """
-__version__ = "0.7.0"
+__version__ = "0.7.2"
```

### Comparing `madam-mam-0.7.0/madam/__main__.py` & `madam_mam-0.7.2/madam/__main__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/__init__.py` & `madam_mam-0.7.2/madam/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/agents/__init__.py` & `madam_mam-0.7.2/madam/adapters/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/agents/bash.py` & `madam_mam-0.7.2/madam/adapters/agents/bash.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,30 +65,31 @@
 
     def execute(self, context: adhesive.ExecutionToken) -> None:
         """
         Execute application bash with arguments provided
 
         Headers:
             arguments:  string with bash command or script path, parsed as a jinja2 string
-                        (workflow variables can be used with jinja2 tags, see https://jinja.palletsprojects.com/en/3.0.x/templates/#variables)
+                        (workflow variables can be used with jinja2 tags,
+                         see https://jinja.palletsprojects.com/en/3.0.x/templates/#variables)
 
             applications.bash.version: Optional[string] with version for bash label application
 
 
         Examples:
             arguments = "cp {{source}} {{destination}}"
             arguments = "{{script_path}}"
 
         :param context: Adhesive context instance
         :return:
         """
         # job tracking
-        workflow_instance = json.loads(
+        workflow_instance: WorkflowInstance = json.loads(
             context.data.madam["workflow_instance"], cls=WorkflowInstanceJSONDecoder
-        )  # type: WorkflowInstance
+        )
         job = self.jobs.create(
             workflow_instance,
             context.task.id,
             self.AGENT_TYPE,
             context.task.headers,
             context.task.input.as_dict(),
         )
```

### Comparing `madam-mam-0.7.0/madam/adapters/agents/concatenate.py` & `madam_mam-0.7.2/madam/adapters/agents/concatenate.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,17 @@
 
         Note : need to create a temporary playlist file from sources list in the destination directory
 
         :param context: Adhesive context instance
         :return:
         """
         # job tracking
-        workflow_instance = json.loads(
+        workflow_instance: WorkflowInstance = json.loads(
             context.data.madam["workflow_instance"], cls=WorkflowInstanceJSONDecoder
-        )  # type: WorkflowInstance
+        )
         job = self.jobs.create(
             workflow_instance,
             context.task.id,
             self.AGENT_TYPE,
             context.task.headers,
             context.task.input.as_dict(),
         )
```

### Comparing `madam-mam-0.7.0/madam/adapters/agents/ffmpeg.py` & `madam_mam-0.7.2/madam/adapters/agents/ffmpeg.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,27 +65,28 @@
 
     def execute(self, context: adhesive.ExecutionToken) -> None:
         """
         Execute application FFmpeg with arguments provided
 
         Headers:
             arguments:  string with FFmpeg arguments parsed as a jinja2 string
-                        (workflow variables can be used with jinja2 tags, see https://jinja.palletsprojects.com/en/3.0.x/templates/#variables)
+                        (workflow variables can be used with jinja2 tags,
+                         see https://jinja.palletsprojects.com/en/3.0.x/templates/#variables)
 
             applications.ffmpeg.version: Optional[string] with version for ffmpeg label application
 
         Example: arguments = "-y -i {{item}} {{destination}}"
 
         :param context: Adhesive context instance
         :return:
         """
         # job tracking
-        workflow_instance = json.loads(
+        workflow_instance: WorkflowInstance = json.loads(
             context.data.madam["workflow_instance"], cls=WorkflowInstanceJSONDecoder
-        )  # type: WorkflowInstance
+        )
         job = self.jobs.create(
             workflow_instance,
             context.task.id,
             self.AGENT_TYPE,
             context.task.headers,
             context.task.input.as_dict(),
         )
```

### Comparing `madam-mam-0.7.0/madam/adapters/agents/imagemagick.py` & `madam_mam-0.7.2/madam/adapters/agents/imagemagick.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,27 +90,28 @@
                         - conjure
                         - convert
                         - identify
                         - mogrify
                         - montage
 
             arguments:  string with ImageMagick arguments parsed as a jinja2 string
-                        (workflow variables can be used with jinja2 tags, see https://jinja.palletsprojects.com/en/3.0.x/templates/#variables)
+                        (workflow variables can be used with jinja2 tags,
+                         see https://jinja.palletsprojects.com/en/3.0.x/templates/#variables)
 
             applications.imagemagick.version: Optional[string] with version for imagemagick label application
 
         Example: arguments = "-size 100x100 {{source}} {{destination}}"
 
         :param context: Adhesive context instance
         :return:
         """
         # job tracking
-        workflow_instance = json.loads(
+        workflow_instance: WorkflowInstance = json.loads(
             context.data.madam["workflow_instance"], cls=WorkflowInstanceJSONDecoder
-        )  # type: WorkflowInstance
+        )
         job = self.jobs.create(
             workflow_instance,
             context.task.id,
             self.AGENT_TYPE,
             context.task.headers,
             context.task.input.as_dict(),
         )
```

### Comparing `madam-mam-0.7.0/madam/adapters/agents/mediainfo.py` & `madam_mam-0.7.2/madam/adapters/agents/mediainfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,28 +70,29 @@
         Execute application Mediainfo with arguments provided
 
         Output Variables:
             mediainfo: dict with mediainfo output
 
         Headers:
             arguments:  string with Mediainfo arguments parsed as a jinja2 string
-                        (workflow variables can be used with jinja2 tags, see https://jinja.palletsprojects.com/en/3.0.x/templates/#variables)
+                        (workflow variables can be used with jinja2 tags,
+                         see https://jinja.palletsprojects.com/en/3.0.x/templates/#variables)
                         --Output=? is useless as it will be overloaded by agent to --Output=JSON
 
             applications.mediainfo.version: Optional[string] with version for mediainfo label application
 
         Example: arguments = "-f {{item}}"
 
         :param context: Adhesive context instance
         :return:
         """
         # job tracking
-        workflow_instance = json.loads(
+        workflow_instance: WorkflowInstance = json.loads(
             context.data.madam["workflow_instance"], cls=WorkflowInstanceJSONDecoder
-        )  # type: WorkflowInstance
+        )
         job = self.jobs.create(
             workflow_instance,
             context.task.id,
             self.AGENT_TYPE,
             context.task.headers,
             context.task.input.as_dict(),
         )
```

### Comparing `madam-mam-0.7.0/madam/adapters/agents/melt.py` & `madam_mam-0.7.2/madam/adapters/agents/melt.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,27 +65,28 @@
 
     def execute(self, context: adhesive.ExecutionToken) -> None:
         """
         Execute application Melt (MLT toolkit) with arguments provided
 
         Headers:
             arguments:  string with Melt arguments parsed as a jinja2 string
-                        (workflow variables can be used with jinja2 tags, see https://jinja.palletsprojects.com/en/3.0.x/templates/#variables)
+                        (workflow variables can be used with jinja2 tags,
+                         see https://jinja.palletsprojects.com/en/3.0.x/templates/#variables)
 
             applications.melt.version: Optional[string] with version for melt label application
 
         Example: arguments = "{{source}} -consumer {{destination}}"
 
         :param context: Adhesive context instance
         :return:
         """
         # job tracking
-        workflow_instance = json.loads(
+        workflow_instance: WorkflowInstance = json.loads(
             context.data.madam["workflow_instance"], cls=WorkflowInstanceJSONDecoder
-        )  # type: WorkflowInstance
+        )
         job = self.jobs.create(
             workflow_instance,
             context.task.id,
             self.AGENT_TYPE,
             context.task.headers,
             context.task.input.as_dict(),
         )
```

### Comparing `madam-mam-0.7.0/madam/adapters/agents/python.py` & `madam_mam-0.7.2/madam/adapters/agents/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,27 +65,28 @@
 
     def execute(self, context: adhesive.ExecutionToken) -> None:
         """
         Execute application python with arguments provided
 
         Headers:
             arguments:  string with bash arguments parsed as a jinja2 string
-                        (workflow variables can be used with jinja2 tags, see https://jinja.palletsprojects.com/en/3.0.x/templates/#variables)
+                        (workflow variables can be used with jinja2 tags,
+                         see https://jinja.palletsprojects.com/en/3.0.x/templates/#variables)
 
             applications.python.version: Optional[string] with version for python label application
 
         Example: arguments = "/path/to/python_script.py {{source}} {{destination}}"
 
         :param context: Adhesive context instance
         :return:
         """
         # job tracking
-        workflow_instance = json.loads(
+        workflow_instance: WorkflowInstance = json.loads(
             context.data.madam["workflow_instance"], cls=WorkflowInstanceJSONDecoder
-        )  # type: WorkflowInstance
+        )
         job = self.jobs.create(
             workflow_instance,
             context.task.id,
             self.AGENT_TYPE,
             context.task.headers,
             context.task.input.as_dict(),
         )
```

### Comparing `madam-mam-0.7.0/madam/adapters/agents/scanfolder.py` & `madam_mam-0.7.2/madam/adapters/agents/scanfolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,17 @@
         Example: glob_mp4 = "*.mp4"
                  glob_video = "video_*.*"
 
         :param context: Adhesive context instance
         :return:
         """
         # job tracking
-        workflow_instance = json.loads(
+        workflow_instance: WorkflowInstance = json.loads(
             context.data.madam["workflow_instance"], cls=WorkflowInstanceJSONDecoder
-        )  # type: WorkflowInstance
+        )
         job = self.jobs.create(
             workflow_instance,
             context.task.id,
             self.AGENT_TYPE,
             context.task.headers,
             context.task.input.as_dict(),
         )
```

### Comparing `madam-mam-0.7.0/madam/adapters/agents/scenes.py` & `madam_mam-0.7.2/madam/adapters/agents/scenes.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,17 +87,17 @@
 
             applications.ffmpeg.version: Optional[string] with version for ffmpeg label application
 
         :param context: Adhesive context instance
         :return:
         """
         # job tracking
-        workflow_instance = json.loads(
+        workflow_instance: WorkflowInstance = json.loads(
             context.data.madam["workflow_instance"], cls=WorkflowInstanceJSONDecoder
-        )  # type: WorkflowInstance
+        )
         job = self.jobs.create(
             workflow_instance,
             context.task.id,
             self.AGENT_TYPE,
             context.task.headers,
             context.task.input.as_dict(),
         )
```

### Comparing `madam-mam-0.7.0/madam/adapters/bpmn/__init__.py` & `madam_mam-0.7.2/madam/adapters/bpmn/__init__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/bpmn/assets/BPMN20.xsd` & `madam_mam-0.7.2/madam/adapters/bpmn/assets/BPMN20.xsd`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/bpmn/assets/BPMNDI.xsd` & `madam_mam-0.7.2/madam/adapters/bpmn/assets/BPMNDI.xsd`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/bpmn/assets/DC.xsd` & `madam_mam-0.7.2/madam/adapters/bpmn/assets/DC.xsd`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/bpmn/assets/DI.xsd` & `madam_mam-0.7.2/madam/adapters/bpmn/assets/DI.xsd`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/bpmn/assets/Semantic.xsd` & `madam_mam-0.7.2/madam/adapters/bpmn/assets/Semantic.xsd`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/bpmn/engine.py` & `madam_mam-0.7.2/madam/adapters/bpmn/engine.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/bpmn/parser.py` & `madam_mam-0.7.2/madam/adapters/bpmn/parser.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/config.py` & `madam_mam-0.7.2/madam/adapters/config.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/interfaces/__init__.py` & `madam_mam-0.7.2/madam/adapters/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/interfaces/agents.py` & `madam_mam-0.7.2/madam/adapters/interfaces/agents.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/process/__init__.py` & `madam_mam-0.7.2/madam/adapters/process/__init__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/process/applications.py` & `madam_mam-0.7.2/madam/adapters/process/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # You should have received a copy of the GNU General Public License
 # along with MADAM.  If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 from typing import Optional
 
 from docker.errors import NotFound
-
 from madam.adapters.process import docker_api
 from madam.domains.entities.application import (
     STATUS_ABORTED,
     STATUS_COMPLETE,
     STATUS_CONTAINER_ERROR,
     STATUS_ERROR,
     Application,
```

### Comparing `madam-mam-0.7.0/madam/adapters/process/docker_api.py` & `madam_mam-0.7.2/madam/adapters/process/docker_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,16 @@
 Madam docker_api module
 """
 import logging
 import shlex
 from time import sleep, time
 from typing import Optional
 
-from docker.models.services import Service
-
 from docker import DockerClient, types
+from docker.models.services import Service
 
 DOCKER_TASK_STATE_COMPLETE = "complete"
 DOCKER_TASK_STATE_FAILED = "failed"
 DOCKER_TASK_STATE_REJECTED = "rejected"
 DOCKER_SERVICE_ABORTED = "aborted"
 
 WAIT_FOR_TASK_TO_START_TIMEOUT = 30
```

### Comparing `madam-mam-0.7.0/madam/adapters/repository/__init__.py` & `madam_mam-0.7.2/madam/adapters/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/repository/applications.py` & `madam_mam-0.7.2/madam/adapters/repository/applications.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/repository/assets/migrations/00001.init_tables.sql` & `madam_mam-0.7.2/madam/adapters/repository/assets/migrations/00001.init_tables.sql`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/repository/jobs.py` & `madam_mam-0.7.2/madam/adapters/repository/jobs.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/repository/postgresql.py` & `madam_mam-0.7.2/madam/adapters/repository/postgresql.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,16 @@
         :return:
         """
         migrations_path = str(
             Path(__file__).parent.parent.joinpath(DATABASE_MIGRATIONS_PATH).expanduser()
         )
         migrations = read_migrations(migrations_path)
         backend = get_backend(
-            "postgresql://{username}:{password}@{hostname}:{port}/{database}?sslmode={ssl_mode}".format(  # pylint: disable=consider-using-f-string
+            "postgresql://{username}:{password}@{hostname}:{port}\
+/{database}?sslmode={ssl_mode}".format(  # pylint: disable=consider-using-f-string
                 username=self.config["migrations"]["username"],
                 password=self.config["migrations"]["password"],
                 hostname=self.config["host"],
                 port=self.config["port"],
                 database=self.config["name"],
                 ssl_mode=self.config["ssl_mode"],
             )
```

### Comparing `madam-mam-0.7.0/madam/adapters/repository/timers.py` & `madam_mam-0.7.2/madam/adapters/repository/timers.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/repository/watchfolders.py` & `madam_mam-0.7.2/madam/adapters/repository/watchfolders.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/repository/workflow_instances.py` & `madam_mam-0.7.2/madam/adapters/repository/workflow_instances.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/adapters/repository/workflows.py` & `madam_mam-0.7.2/madam/adapters/repository/workflows.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/__init__.py` & `madam_mam-0.7.2/madam/domains/__init__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/agents.py` & `madam_mam-0.7.2/madam/domains/agents.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/application.py` & `madam_mam-0.7.2/madam/domains/application.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/applications.py` & `madam_mam-0.7.2/madam/domains/applications.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/entities/__init__.py` & `madam_mam-0.7.2/madam/domains/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/entities/agent.py` & `madam_mam-0.7.2/madam/domains/entities/agent.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/entities/application.py` & `madam_mam-0.7.2/madam/domains/entities/application.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/entities/constants.py` & `madam_mam-0.7.2/madam/domains/entities/constants.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/entities/events.py` & `madam_mam-0.7.2/madam/domains/entities/events.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/entities/job.py` & `madam_mam-0.7.2/madam/domains/entities/job.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/entities/runner.py` & `madam_mam-0.7.2/madam/domains/entities/runner.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/entities/timer.py` & `madam_mam-0.7.2/madam/domains/entities/timer.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/entities/watchfolder.py` & `madam_mam-0.7.2/madam/domains/entities/watchfolder.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/entities/workflow.py` & `madam_mam-0.7.2/madam/domains/entities/workflow.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/entities/workflow_instance.py` & `madam_mam-0.7.2/madam/domains/entities/workflow_instance.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/events.py` & `madam_mam-0.7.2/madam/domains/events.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/interfaces/__init__.py` & `madam_mam-0.7.2/madam/domains/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/interfaces/agents.py` & `madam_mam-0.7.2/madam/domains/interfaces/agents.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/interfaces/bpmn.py` & `madam_mam-0.7.2/madam/domains/interfaces/bpmn.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/interfaces/events.py` & `madam_mam-0.7.2/madam/domains/interfaces/events.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/interfaces/process/__init__.py` & `madam_mam-0.7.2/madam/domains/interfaces/process/__init__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/interfaces/process/applications.py` & `madam_mam-0.7.2/madam/domains/interfaces/process/applications.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/interfaces/repository/__init__.py` & `madam_mam-0.7.2/madam/domains/interfaces/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/interfaces/repository/applications.py` & `madam_mam-0.7.2/madam/domains/interfaces/repository/applications.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/interfaces/repository/config.py` & `madam_mam-0.7.2/madam/domains/interfaces/repository/config.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/interfaces/repository/jobs.py` & `madam_mam-0.7.2/madam/domains/interfaces/repository/jobs.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/interfaces/repository/timers.py` & `madam_mam-0.7.2/madam/domains/interfaces/repository/timers.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/interfaces/repository/watchfolders.py` & `madam_mam-0.7.2/madam/domains/interfaces/repository/watchfolders.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/interfaces/repository/workflow_instances.py` & `madam_mam-0.7.2/madam/domains/interfaces/repository/workflow_instances.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/interfaces/repository/workflows.py` & `madam_mam-0.7.2/madam/domains/interfaces/repository/workflows.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/jobs.py` & `madam_mam-0.7.2/madam/domains/jobs.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/timers.py` & `madam_mam-0.7.2/madam/domains/timers.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/watchfolders.py` & `madam_mam-0.7.2/madam/domains/watchfolders.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/workflow_instances.py` & `madam_mam-0.7.2/madam/domains/workflow_instances.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/domains/workflows.py` & `madam_mam-0.7.2/madam/domains/workflows.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/libs/__init__.py` & `madam_mam-0.7.2/madam/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/libs/http.py` & `madam_mam-0.7.2/madam/libs/http.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with MADAM.  If not, see <https://www.gnu.org/licenses/>.
 
 import copy
 import json
 import logging
-from http.client import HTTPResponse
 from typing import Any, Optional
 from urllib import parse, request
 
 # Response type constants
 RESPONSE_JSON = "json"
 RESPONSE_TEXT = "text"
 RESPONSE_HTTP = "http"
@@ -67,15 +66,15 @@
 
             # http header to send json body
             headers["Content-Type"] = "application/json"
 
         if len(headers) > 0:
             request_.headers = headers
 
-        with request.urlopen(request_, timeout=15) as response:  # type: HTTPResponse
+        with request.urlopen(request_, timeout=15) as response:
             if response.status != 200:
                 content = response.read().decode("utf-8")
                 raise ValueError(f"status code != 200 => {response.status} ({content})")
 
             # get response content
             return_response = copy.copy(response)
             content = response.read().decode("utf-8")
```

### Comparing `madam-mam-0.7.0/madam/libs/iso8601.py` & `madam_mam-0.7.2/madam/libs/iso8601.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/libs/serialize.py` & `madam_mam-0.7.2/madam/libs/serialize.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/libs/timecode.py` & `madam_mam-0.7.2/madam/libs/timecode.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/slots/__init__.py` & `madam_mam-0.7.2/madam/slots/__init__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/slots/cli.py` & `madam_mam-0.7.2/madam/slots/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,17 @@
     variables: Dict[str, Any] = {"content": content}
     response = query_endpoint(mutation, context.obj["endpoint"], variables)
 
     if response["data"]["createWorkflow"]["status"] is False:
         click.echo("error: " + response["data"]["createWorkflow"]["error"])
         return
     click.echo(
-        f'Workflow "{response["data"]["createWorkflow"]["workflow"]["name"]}" (id: {response["data"]["createWorkflow"]["workflow"]["id"]}) Version {response["data"]["createWorkflow"]["workflow"]["version"]} uploaded.'
+        f'Workflow "{response["data"]["createWorkflow"]["workflow"]["name"]}" \
+(id: {response["data"]["createWorkflow"]["workflow"]["id"]}) \
+Version {response["data"]["createWorkflow"]["workflow"]["version"]} uploaded.'
     )
 
 
 @workflow.command("list")
 @click.pass_context
 def workflow_list(context: Context):
     """
@@ -1190,15 +1192,16 @@
     """
     response = query_endpoint(mutation, context.obj["endpoint"], variables)
 
     if response["data"]["createWatchfolder"]["status"] is False:
         click.echo("error: " + response["data"]["createWatchfolder"]["error"])
         return
     click.echo(
-        f'Watchfolder ID={response["data"]["createWatchfolder"]["watchfolder"]["id"]} created for path {response["data"]["createWatchfolder"]["watchfolder"]["path"]}.'
+        f'Watchfolder ID={response["data"]["createWatchfolder"]["watchfolder"]["id"]} \
+created for path {response["data"]["createWatchfolder"]["watchfolder"]["path"]}.'
     )
 
 
 @watchfolder.command("update")
 @click.pass_context
 def watchfolder_update(context: Context):
     """
@@ -1281,15 +1284,16 @@
 
     response = query_endpoint(mutation, context.obj["endpoint"], variables)
 
     if response["data"]["updateWatchfolder"]["status"] is False:
         click.echo("error: " + response["data"]["updateWatchfolder"]["error"])
         return
     click.echo(
-        f'Watchfolder ID={response["data"]["updateWatchfolder"]["watchfolder"]["id"]} updated for path {response["data"]["updateWatchfolder"]["watchfolder"]["path"]}.'
+        f'Watchfolder ID={response["data"]["updateWatchfolder"]["watchfolder"]["id"]} \
+updated for path {response["data"]["updateWatchfolder"]["watchfolder"]["path"]}.'
     )
 
 
 @watchfolder.command("start")
 @click.argument("id", type=str)
 @click.pass_context
 def watchfolder_start(context: Context, id: str):  # pylint: disable=redefined-builtin
@@ -1705,15 +1709,15 @@
     GraphQL query or mutation request on endpoint
 
     :param query: GraphQL query string
     :param url: Endpoint url
     :param variables: Variables for the query (optional, default None)
     :return:
     """
-    payload = {"query": query}  # type: Dict[str, Union[str, dict]]
+    payload: Dict[str, Union[str, dict]] = {"query": query}
 
     if variables is not None:
         payload["variables"] = variables
 
     client = HTTPClient()
 
     try:
```

### Comparing `madam-mam-0.7.0/madam/slots/graphql/__init__.py` & `madam_mam-0.7.2/madam/slots/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/slots/graphql/api.py` & `madam_mam-0.7.2/madam/slots/graphql/api.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/slots/graphql/assets/schema.graphql` & `madam_mam-0.7.2/madam/slots/graphql/assets/schema.graphql`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/slots/graphql/mutation.py` & `madam_mam-0.7.2/madam/slots/graphql/mutation.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     Create workflow from BPMN XML content
 
     :param _: Parent
     :param info: Context
     :param content: BPMN XML content
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     try:
         workflow = application.workflows.create(content)
     except Exception as exception:
         return {"status": False, "error": str(exception)}
 
     return {"status": True, "workflow": workflow}
@@ -55,15 +55,15 @@
     Delete workflow
 
     :param _: Parent
     :param info: Context
     :param id: Workflow ID
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     try:
         workflow = application.workflows.read(id)
         application.workflows.delete(workflow)
     except Exception as exception:
         return {"status": False, "error": str(exception)}
 
@@ -84,15 +84,15 @@
     :param _: Parent
     :param info: Context
     :param id: Workflow ID
     :param version: Workflow version
     :param variables: Workflow initial variables
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     if variables is not None:
         variables_obj = json.loads(variables)
     else:
         variables_obj = variables
     try:
         result = application.workflows.start(id, version, variables_obj)
@@ -111,15 +111,15 @@
 
     :param _: Parent
     :param info: Context
     :param id: Workflow ID
     :param version: Workflow version
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     try:
         result = application.workflows.abort(id, version)
     except Exception as exception:
         return {"status": False, "error": str(exception)}
 
     return {"status": result}
@@ -133,15 +133,15 @@
     Abort workflow instance by ID
 
     :param _: Parent
     :param info: Context
     :param id: Workflow instance ID
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     workflow_instance = application.workflow_instances.read(UUID(id))
 
     try:
         application.workflow_instances.abort(workflow_instance)
     except Exception as exception:
         return {"status": False, "error": str(exception)}
 
@@ -156,15 +156,15 @@
     Delete workflow instance
 
     :param _: Parent
     :param info: Context
     :param id: Workflow instance ID
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     try:
         workflow_instance = application.workflow_instances.read(UUID(id))
     except Exception as exception:
         return {"status": False, "error": str(exception)}
 
     try:
         application.workflow_instances.delete(workflow_instance)
@@ -183,15 +183,15 @@
 
     :param _: Parent
     :param info: Context
     :param id: Workflow instance ID
     :param version: Workflow version
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     try:
         workflow = application.workflows.read(id, version)
     except Exception as exception:
         return {"status": False, "error": str(exception)}
 
     try:
         application.workflow_instances.abort_by_workflow(workflow)
@@ -210,15 +210,15 @@
 
     :param _: Parent
     :param info: Context
     :param id: Workflow instance ID
     :param version: Workflow version
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     try:
         workflow = application.workflows.read(id, version)
     except Exception as exception:
         return {"status": False, "error": str(exception)}
 
     try:
         application.workflow_instances.delete_by_workflow(workflow)
@@ -236,15 +236,15 @@
     Abort timer by ID
 
     :param _: Parent
     :param info: Context
     :param id: Timer ID
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     try:
         application.timers.abort(UUID(id))
     except Exception as exception:
         return {"status": False, "error": str(exception)}
 
     return {"status": True}
 
@@ -257,15 +257,15 @@
     Delete timer
 
     :param _: Parent
     :param info: Context
     :param id: Timer ID
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     try:
         timer = application.timers.read(UUID(id))
     except Exception as exception:
         return {"status": False, "error": str(exception)}
 
     try:
         application.timers.delete(timer)
@@ -307,15 +307,15 @@
     :param deleted_workflow: Workflow instance to start when a file is deleted (default=None)
     :param deleted_variables: Initial variables for deleted_workflow (default=None)
     :param added_items_key: Key to store added files list in workflow initial variables (default="watchfolder)
     :param modified_items_key: Key to store modified files list in workflow initial variables (default="watchfolder)
     :param deleted_items_key: Key to store deleted files list in workflow initial variables (default="watchfolder)
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     added_workflow_object = None
     modified_workflow_object = None
     deleted_workflow_object = None
     if added_workflow is not None:
         try:
             added_workflow_object = application.workflows.read(
                 added_workflow["id"],
@@ -401,15 +401,15 @@
     :param deleted_workflow: Workflow instance to start when a file is deleted (default=None)
     :param deleted_variables: Initial variables for deleted_workflow (default=None)
     :param added_items_key: Key to store added files list in workflow initial variables (default="watchfolder)
     :param modified_items_key: Key to store modified files list in workflow initial variables (default="watchfolder)
     :param deleted_items_key: Key to store deleted files list in workflow initial variables (default="watchfolder)
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     try:
         watchfolder = application.watchfolders.read(UUID(id))
     except Exception as exception:
         return {"status": False, "error": str(exception)}
 
     added_workflow_object = None
     modified_workflow_object = None
@@ -478,15 +478,15 @@
     Start watchfolder ID
 
     :param _: Parent
     :param info: Context
     :param id: Watchfolder ID
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     try:
         watchfolder = application.watchfolders.read(UUID(id))
         application.watchfolders.start(watchfolder)
     except Exception as exception:
         return {"status": False, "error": str(exception)}
 
@@ -503,15 +503,15 @@
     Stop watchfolder ID
 
     :param _: Parent
     :param info: Context
     :param id: Watchfolder ID
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     try:
         application.watchfolders.stop(UUID(id))
     except Exception as exception:
         print(exception)
         return {"status": False, "error": str(exception)}
 
@@ -528,15 +528,15 @@
     Delete watchfolder ID
 
     :param _: Parent
     :param info: Context
     :param id: Watchfolder ID
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     try:
         watchfolder = application.watchfolders.read(UUID(id))
         application.watchfolders.delete(watchfolder)
     except Exception as exception:
         return {"status": False, "error": str(exception)}
```

### Comparing `madam-mam-0.7.0/madam/slots/graphql/query.py` & `madam_mam-0.7.2/madam/slots/graphql/query.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,29 +58,29 @@
     """
     Get Madam version
 
     :param _: Parent
     :param info: Context
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     return application.get_version()
 
 
 @query.field("agents")
 def resolve_agents(_, info: GraphQLResolveInfo):
     """
     Get Madam agents list
 
     :param _: Parent
     :param info: Context
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     if info.field_nodes[0].selection_set is not None:
         fields_selection = info.field_nodes[0].selection_set.selections
 
         if len(fields_selection) == 1:
             field = fields_selection[
                 0
@@ -104,15 +104,15 @@
     Get Madam agent documentation
 
     :param _: Parent
     :param info: Context
     :param name: Agent's name
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     try:
         agent = application.agents.read(name)
     except ModuleNotFoundError:
         return None
 
     return None if agent is None else _agent_serializer(agent)
@@ -151,15 +151,15 @@
 
     :param _: Parent
     :param info: Context
     :param id: Workflow ID
     :param version: Workflow version
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     try:
         workflow = application.workflows.read(id, version)
     except Exception:
         return None
 
     return workflow
@@ -183,15 +183,15 @@
     :param offset: Offset in result
     :param limit: Max number of elements in result
     :param sort_column: Column to order by
     :param sort_ascending: Order by ascending if True
     :param last_version: Return only last version if True
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     result: List[Workflow] = []
 
     try:
         count = application.workflows.count(last_version)
     except Exception:
         return {"count": 0, "result": result}
 
@@ -216,15 +216,15 @@
     Get workflow instance from ID
 
     :param _: Parent
     :param info: Context
     :param id: Workflow instance ID
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     try:
         instance = application.workflow_instances.read(UUID(id))
     except Exception:
         return None
 
     return instance
@@ -250,15 +250,15 @@
     :param limit: Max number of elements in result
     :param sort_column: Column to order by
     :param sort_ascending: Order by ascending if True
     :param status: Instance status filter
     :param workflow: Parent Workflow filter as WorkflowInput {"id": str, ["version": Optional[int]]}
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     result: List[WorkflowInstance] = []
 
     version = (
         workflow["version"] if workflow is not None and "version" in workflow else None
     )
     workflow_ = None
 
@@ -294,15 +294,15 @@
     Get Timer from ID
 
     :param _: Parent
     :param info: Context
     :param id: Timer ID
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     try:
         timer = application.timers.read(UUID(id))
     except Exception:
         return None
 
     return timer
@@ -328,15 +328,15 @@
     :param limit: Max number of elements in result
     :param sort_column: Column to order by
     :param sort_ascending: Order by ascending if True
     :param status: Instance status filter
     :param workflow: Parent Workflow filter as WorkflowInput {"id": str, ["version": Optional[int]]}
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     result: List[Timer] = []
 
     version = (
         workflow["version"] if workflow is not None and "version" in workflow else None
     )
     workflow_ = None
 
@@ -372,15 +372,15 @@
     Get Job from ID
 
     :param _: Parent
     :param info: Context
     :param id: Job ID
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     try:
         job = application.jobs.read(UUID(id))
     except Exception:
         return None
 
     return job
@@ -406,15 +406,15 @@
     :param limit: Max number of elements in result
     :param sort_column: Column to order by
     :param sort_ascending: Order by ascending if True
     :param status: Instance status filter
     :param workflow_instance_id: Parent WorkflowInstance ID filter
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     result: List[Job] = []
     workflow_instance_uuid = (
         UUID(workflow_instance_id) if workflow_instance_id is not None else None
     )
 
     try:
         count = application.jobs.count(status, workflow_instance_uuid)
@@ -442,15 +442,15 @@
     Get Application from ID
 
     :param _: Parent
     :param info: Context
     :param id: Application ID
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     try:
         application_ = application.applications.read(UUID(id))
     except Exception:
         return None
 
     return application_
@@ -476,15 +476,15 @@
     :param limit: Max number of elements in result
     :param sort_column: Column to order by
     :param sort_ascending: Order by ascending if True
     :param status: Instance status filter
     :param job_id: Parent Job ID filter
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     result: List[Application] = []
     job_uuid = UUID(job_id) if job_id is not None else None
 
     try:
         count = application.applications.count(status, job_uuid)
     except Exception:
         return {"count": 0, "result": result}
@@ -510,15 +510,15 @@
     Get workflow from ID and version
 
     :param _: Parent
     :param info: Context
     :param id: Watchfolder ID
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
 
     try:
         watchfolder = application.watchfolders.read(UUID(id))
     except Exception:
         return None
 
     return watchfolder
@@ -544,15 +544,15 @@
     :param limit: Max number of elements in result
     :param sort_column: Column to order by
     :param sort_ascending: Order by ascending if True
     :param status: Watchfolder status filter
     :param workflow: Triggered Workflow filter as WorkflowInput {"id": str, ["version": Optional[int]]}
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     result: List[Watchfolder] = []
 
     version = (
         workflow["version"] if workflow is not None and "version" in workflow else None
     )
     workflow_ = None
```

### Comparing `madam-mam-0.7.0/madam/slots/graphql/scalar.py` & `madam_mam-0.7.2/madam/slots/graphql/scalar.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/slots/graphql/server.py` & `madam_mam-0.7.2/madam/slots/graphql/server.py`

 * *Files identical despite different names*

### Comparing `madam-mam-0.7.0/madam/slots/graphql/subscription.py` & `madam_mam-0.7.2/madam/slots/graphql/subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     """
     Push instance event object
 
     :param _: Parent
     :param info: Context
     :return:
     """
-    application = info.context["application"]  # type: MainApplication
+    application: MainApplication = info.context["application"]
     subscription_id = str(uuid.uuid4())
     application.graphql_api.subscriptions[subscription_id] = []
     try:
         while True:
             if len(application.graphql_api.subscriptions[subscription_id]) > 0:
                 event = application.graphql_api.subscriptions[subscription_id].pop(0)
                 yield event
```

### Comparing `madam-mam-0.7.0/setup.py` & `madam_mam-0.7.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,243 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: madam-mam
+Version: 0.7.2
+Summary: MADAM (TM) Multi Agent Digital Asset Manager - a MAM server for Docker Swarm to handle higly distributed media processes
+License: GPL-3.0-only
+Keywords: BPMN,workflow,media,assets,management,MAM,DAM,docker,swarm
+Author: Vincent Texier
+Author-email: vit@free.fr
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Jinja2 (>=3.0.1,<4.0.0)
+Requires-Dist: PyYAML (==5.1.2)
+Requires-Dist: adhesive-zeebe (>=2021.4.3,<2022.0.0)
+Requires-Dist: ariadne (>=0.13.0,<0.14.0)
+Requires-Dist: docker (>=6.1.0,<7.0.0)
+Requires-Dist: lxml (>=4.6.3,<5.0.0)
+Requires-Dist: psycopg2-binary (>=2.8.6,<3.0.0)
+Requires-Dist: python-sql (>=1.2.2,<2.0.0)
+Requires-Dist: rich (>=10.2.2,<11.0.0)
+Requires-Dist: timecode (>=1.3.1,<2.0.0)
+Requires-Dist: uvicorn (>=0.14.0,<0.15.0)
+Requires-Dist: watchgod (>=0.7,<0.8)
+Requires-Dist: yoyo-migrations (>=8.2.0,<9.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['madam',
- 'madam.adapters',
- 'madam.adapters.agents',
- 'madam.adapters.bpmn',
- 'madam.adapters.interfaces',
- 'madam.adapters.process',
- 'madam.adapters.repository',
- 'madam.domains',
- 'madam.domains.entities',
- 'madam.domains.interfaces',
- 'madam.domains.interfaces.process',
- 'madam.domains.interfaces.repository',
- 'madam.libs',
- 'madam.slots',
- 'madam.slots.graphql']
-
-package_data = \
-{'': ['*'],
- 'madam.adapters.bpmn': ['assets/*'],
- 'madam.adapters.repository': ['assets/migrations/*'],
- 'madam.slots.graphql': ['assets/*']}
-
-install_requires = \
-['Jinja2>=3.0.1,<4.0.0',
- 'PyYAML==5.1.2',
- 'adhesive-zeebe>=2021.4.3,<2022.0.0',
- 'ariadne>=0.13.0,<0.14.0',
- 'docker>=5.0.0,<6.0.0',
- 'lxml>=4.6.3,<5.0.0',
- 'psycopg2-binary>=2.8.6,<3.0.0',
- 'python-sql>=1.2.2,<2.0.0',
- 'rich>=10.2.2,<11.0.0',
- 'timecode>=1.3.1,<2.0.0',
- 'uvicorn>=0.14.0,<0.15.0',
- 'watchgod>=0.7,<0.8',
- 'yoyo-migrations>=7.3.2,<8.0.0']
-
-entry_points = \
-{'console_scripts': ['madam = madam.slots.cli:cli']}
-
-setup_kwargs = {
-    'name': 'madam-mam',
-    'version': '0.7.0',
-    'description': 'MADAM (TM) Multi Agent Digital Asset Manager - a MAM server for Docker Swarm to handle higly distributed media processes',
-    'long_description': '# MADAM\n\nMADAM is the Multi Agent Digital Asset Manager.\n\nIt provides a three-tier architecture platform to handle workflow processing in a distributed environment.\n\nIt uses Docker swarm to dispatch processes in a cluster of machines.\n\nIt is a free (as freedom) software written in Python.\n\n## Documentation\n\n[Link to the documentation](https://m5231.gitlab.io/documentation/)\n\n## Support\n\nIf you find this project useful and want to contribute, please submit issues, merge requests. If you use it regularly,\nyou can help by the author by a financial support.\n\n<script src="https://liberapay.com/vit/widgets/button.js"></script>\n<noscript><a href="https://liberapay.com/vit/donate"><img alt="Donate using Liberapay" src="https://liberapay.com/assets/widgets/donate.svg"></a></noscript>\n\n## Requirements\n\nYou will need [Camunda Modeler 4.11+](https://github.com/camunda/camunda-modeler/releases) to easily create\nZeebe BPMN XML workflows for MADAM.\n\n## Licensing\n\nMADAM is licensed under the [Gnu Public License Version 3](https://www.gnu.org/licenses/gpl-3.0.en.html).\n\nCamunda Modeler is licensed under [the MIT License (MIT)](https://mit-license.org/).\n\nAt its core, MADAM use [adhesive-zebe](https://github.com/vtexier/adhesive), a BPMN workflow python engine able to\nexecute Zeebe BPMN XML workflows. It is a fork of [adhesive](https://github.com/germaniumhq/adhesive) under\nthe original adhesive license that is [GNU Affero General Public License v3.0](https://www.gnu.org/licenses/agpl-3.0.en.html)\n\n## System environment setup\n\n1. [Install Docker](https://docs.docker.com/engine/install/).\n\n2. [Configure userns-remap](https://docs.docker.com/engine/security/userns-remap/) to map container user `root` to a\n   host non-root user.\n\n3. Configure the dev station as a [Docker Swarm Manager](https://docs.docker.com/engine/swarm/).\n\n4. Install a [Postgresql](https://www.postgresql.org/download/) database server.\n   \n_You can use the Ansible playbook provided to install PostgreSQL locally with Docker,\nafter configuring `hosts.yaml`:_\n\n    make environment\n\n### Python environment setup\n\n* It requires Python 3.8+.\n\n* [Pyenv](https://github.com/pyenv/pyenv) should be used to choose the right version of Python, without breaking the\n  default Python of the Operating System.\n\n* A Python virtual environment should be created in a `.venv` folder.\n\n```bash\n    pyenv install 3.8.0\n    pyenv shell 3.8.0\n    python -m venv .venv \n    source .venv/bin/activate`\n```\n\n### Installation/Update\n\nFrom PyPI:\n\nIn a Python virtualenv:\n\n    pip install -U madam-mam\n\nIn your user install directory:\n\n    pip install --user -U madam-mam\n\nYou should have a the `madam` cli command available:\n\n    madam\n\nor\n\n    madam --help\n\nwill display command usage.\n\nTo have bash completion, you can type:\n\n    _MADAM_COMPLETE=source_bash madam > madam-complete.sh\n    sudo cp madam-complete.sh /etc/bash_completion.d/.\n\nFor another shell, replace `source_bash` by `source_zsh` or `source_fish`\n\n### Development environment\n\nInstall [Poetry](https://python-poetry.org/) with the custom installer:\n\n    curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python\n\nInstall Python dependencies:\n\n    poetry install --no-root\n\nYou can use the madam-cli dev command:\n\n    ./bin/madam-cli\n\nGet `bin/madam-cli` bash shell completion:\n\n    _MADAM_CLI_COMPLETE=source_bash bin/madam-cli > madam-cli-complete.sh\n    sudo cp madam-cli-complete.sh /etc/bash_completion.d/.\n\nFor another shell, replace `source_bash` by `source_zsh` or `source_fish`\n\n### Configuration\n\nMake a copy of the environment config example file:\n\n    cp .env.example .env\n\nEdit `.env` to suit your needs, then:\n\n    export $(grep -v \'^#\' .env | xargs -d \'\\n\')\n\nMake a copy of the Ansible inventory example file:\n\n    cp hosts.yaml.example hosts.yaml\n\nEdit `hosts.yaml` to suit your needs.\n\nMake a copy of the MADAM config example file:\n\n    cp madam.yaml.example madam.yaml\n\nEdit `madam.yaml` to suit your needs.\n\nMake a copy of the MADAM config example file for the test environment:\n\n    cp madam_tests.yaml.example madam_tests.yaml\n\nEdit `madam_tests.yaml` to suit your needs.\n\nMake a copy of the MADAM config example file for the local deploy:\n\n    cp madam_deploy.yaml.example madam_deploy.yaml\n\nEdit `madam_deploy.yaml` to suit your needs.\n\n### Set and tag project version in Git\n\n    ./bin/release.sh 1.0.0\n\n### Build MADAM python package and Docker image\n\n    make build\n\nThe wheel package will be build in the `dist` directory.\n\n## Deploy MADAM as local docker container\n\nTo deploy MADAM container on localhost:\n\n    make deploy\n\n## Check static type and code quality\n\n    make check\n\n## Run tests\n\nRun all [pytest](https://docs.pytest.org) tests with:\n\n    make tests\n\nRun only some tests by using `bin/tests.sh`:\n\n    bin/tests.sh tests/domains/test_workflows.py::test_create\n\n## Database setup\n\nSet `DATABASE_URL` and `DATABASE_URL_TESTS` environment variable in `.env` file:\n\n    DATABASE_URL=postgresql://postgres:xxxxx@hostname:5432/madam?sslmode=allow\n    DATABASE_URL_TESTS=postgresql://postgres:xxxxx@hostname:5432/madam_tests?sslmode=allow\n\n### Migrations scripts\n\nAdd/Edit scripts in `resources/migrations` directory:\n\n    # version.name.[rollback].sql\n    00001.init_tables.sql\n    00001.init_tables.rollback.sql\n\n### Migrate commands\n\n    make databases\n    make databases_rollback\n    make databases_list\n',
-    'author': 'Vincent Texier',
-    'author_email': 'vit@free.fr',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+# MADAM
 
+MADAM is the Multi Agent Digital Asset Manager.
+
+It provides a three-tier architecture platform to handle workflow processing in a distributed environment.
+
+It uses Docker swarm to dispatch processes in a cluster of machines.
+
+It is a free (as freedom) software written in Python.
+
+## Documentation
+
+[Link to the documentation](https://m5231.gitlab.io/documentation/)
+
+## Support
+
+If you find this project useful and want to contribute, please submit issues, merge requests. If you use it regularly,
+you can help by the author by a financial support.
+
+<script src="https://liberapay.com/vit/widgets/button.js"></script>
+<noscript><a href="https://liberapay.com/vit/donate"><img alt="Donate using Liberapay" src="https://liberapay.com/assets/widgets/donate.svg"></a></noscript>
+
+## Requirements
+
+You will need [Camunda Modeler 4.11+](https://github.com/camunda/camunda-modeler/releases) to easily create
+Zeebe BPMN XML workflows for MADAM.
+
+## Licensing
+
+MADAM is licensed under the [Gnu Public License Version 3](https://www.gnu.org/licenses/gpl-3.0.en.html).
+
+Camunda Modeler is licensed under [the MIT License (MIT)](https://mit-license.org/).
+
+At its core, MADAM use [adhesive-zebe](https://github.com/vtexier/adhesive), a BPMN workflow python engine able to
+execute Zeebe BPMN XML workflows. It is a fork of [adhesive](https://github.com/germaniumhq/adhesive) under
+the original adhesive license that is [GNU Affero General Public License v3.0](https://www.gnu.org/licenses/agpl-3.0.en.html)
+
+## System environment setup
+
+1. [Install Docker](https://docs.docker.com/engine/install/).
+
+2. [Configure userns-remap](https://docs.docker.com/engine/security/userns-remap/) to map container user `root` to a
+   host non-root user.
+
+3. Configure the dev station as a [Docker Swarm Manager](https://docs.docker.com/engine/swarm/).
+
+4. Install a [Postgresql](https://www.postgresql.org/download/) database server.
+   
+_You can use the Ansible playbook provided to install PostgreSQL locally with Docker,
+after configuring `hosts.yaml`:_
+
+    make environment
+
+### Python environment setup
+
+* It requires Python 3.8+.
+
+* [Pyenv](https://github.com/pyenv/pyenv) should be used to choose the right version of Python, without breaking the
+  default Python of the Operating System.
+
+* A Python virtual environment should be created in a `.venv` folder.
+
+```bash
+    pyenv install 3.8.0
+    pyenv shell 3.8.0
+    python -m venv .venv 
+    source .venv/bin/activate`
+```
+
+### Installation/Update
+
+From PyPI:
+
+In a Python virtualenv:
+
+    pip install -U madam-mam
+
+In your user install directory:
+
+    pip install --user -U madam-mam
+
+You should have a the `madam` cli command available:
+
+    madam
+
+or
+
+    madam --help
+
+will display command usage.
+
+To have bash completion, you can type:
+
+    _MADAM_COMPLETE=source_bash madam > madam-complete.sh
+    sudo cp madam-complete.sh /etc/bash_completion.d/.
+
+For another shell, replace `source_bash` by `source_zsh` or `source_fish`
+
+### Development environment
+
+Install [Poetry](https://python-poetry.org/) with the custom installer:
+
+    curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python
+
+Install Python dependencies:
+
+    poetry install --no-root
+
+Copy `bin/pre-commit.sh` for pre-commmit git hooks:
+
+    cp bin/pre-commit.sh .git/hooks/pre-commit
+
+You can use the madam-cli dev command:
+
+    ./bin/madam-cli
+
+Get `bin/madam-cli` bash shell completion:
+
+    _MADAM_CLI_COMPLETE=source_bash bin/madam-cli > madam-cli-complete.sh
+    sudo cp madam-cli-complete.sh /etc/bash_completion.d/.
+
+For another shell, replace `source_bash` by `source_zsh` or `source_fish`
+
+### Configuration
+
+Make a copy of the environment config example file:
+
+    cp .env.example .env
+
+Edit `.env` to suit your needs, then:
+
+    export $(grep -v '^#' .env | xargs -d '\n')
+
+Make a copy of the Ansible inventory example file:
+
+    cp hosts.yaml.example hosts.yaml
+
+Edit `hosts.yaml` to suit your needs.
+
+Make a copy of the MADAM config example file:
+
+    cp madam.yaml.example madam.yaml
+
+Edit `madam.yaml` to suit your needs.
+
+Make a copy of the MADAM config example file for the test environment:
+
+    cp madam_tests.yaml.example madam_tests.yaml
+
+Edit `madam_tests.yaml` to suit your needs.
+
+Make a copy of the MADAM config example file for the local deploy:
+
+    cp madam_deploy.yaml.example madam_deploy.yaml
+
+Edit `madam_deploy.yaml` to suit your needs.
+
+### Set and tag project version in Git
+
+    ./bin/release.sh 1.0.0
+
+### Build MADAM python package and Docker image
+
+    make build
+
+The wheel package will be build in the `dist` directory.
+
+Push docker image on private registry:
+
+    docker image tag madam:[version] registry_hostname:registry_port/madam:[version]
+    docker push registry_hostname:registry_port/madam:[version]
+
+## Deploy MADAM as local docker container
+
+To deploy MADAM container on localhost:
+
+    make deploy
+
+## Check static type and code quality
+
+    make check
+
+## Run tests
+
+Run all [pytest](https://docs.pytest.org) tests with:
+
+    make tests
+
+Run only some tests by using `bin/tests.sh`:
+
+    bin/tests.sh tests/domains/test_workflows.py::test_create
+
+## Database setup
+
+Set `DATABASE_URL` and `DATABASE_URL_TESTS` environment variable in `.env` file:
+
+    DATABASE_URL=postgresql://postgres:xxxxx@hostname:5432/madam?sslmode=allow
+    DATABASE_URL_TESTS=postgresql://postgres:xxxxx@hostname:5432/madam_tests?sslmode=allow
+
+### Migrations scripts
+
+Add/Edit scripts in `resources/migrations` directory:
+
+    # version.name.[rollback].sql
+    00001.init_tables.sql
+    00001.init_tables.rollback.sql
+
+### Migrate commands
+
+    make databases
+    make databases_rollback
+    make databases_list
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,92 +1,87 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['madam',
-'madam.adapters', 'madam.adapters.agents', 'madam.adapters.bpmn',
-'madam.adapters.interfaces', 'madam.adapters.process',
-'madam.adapters.repository', 'madam.domains', 'madam.domains.entities',
-'madam.domains.interfaces', 'madam.domains.interfaces.process',
-'madam.domains.interfaces.repository', 'madam.libs', 'madam.slots',
-'madam.slots.graphql'] package_data = \ {'': ['*'], 'madam.adapters.bpmn':
-['assets/*'], 'madam.adapters.repository': ['assets/migrations/*'],
-'madam.slots.graphql': ['assets/*']} install_requires = \
-['Jinja2>=3.0.1,<4.0.0', 'PyYAML==5.1.2', 'adhesive-zeebe>=2021.4.3,<2022.0.0',
-'ariadne>=0.13.0,<0.14.0', 'docker>=5.0.0,<6.0.0', 'lxml>=4.6.3,<5.0.0',
-'psycopg2-binary>=2.8.6,<3.0.0', 'python-sql>=1.2.2,<2.0.0',
-'rich>=10.2.2,<11.0.0', 'timecode>=1.3.1,<2.0.0', 'uvicorn>=0.14.0,<0.15.0',
-'watchgod>=0.7,<0.8', 'yoyo-migrations>=7.3.2,<8.0.0'] entry_points = \
-{'console_scripts': ['madam = madam.slots.cli:cli']} setup_kwargs = { 'name':
-'madam-mam', 'version': '0.7.0', 'description': 'MADAM (TM) Multi Agent Digital
-Asset Manager - a MAM server for Docker Swarm to handle higly distributed media
-processes', 'long_description': '# MADAM\n\nMADAM is the Multi Agent Digital
-Asset Manager.\n\nIt provides a three-tier architecture platform to handle
-workflow processing in a distributed environment.\n\nIt uses Docker swarm to
-dispatch processes in a cluster of machines.\n\nIt is a free (as freedom)
-software written in Python.\n\n## Documentation\n\n[Link to the documentation]
-(https://m5231.gitlab.io/documentation/)\n\n## Support\n\nIf you find this
-project useful and want to contribute, please submit issues, merge requests. If
-you use it regularly,\nyou can help by the author by a financial support.\n\n
-\n[Donate_using_Liberapay]\n\n## Requirements\n\nYou will need [Camunda Modeler
-4.11+](https://github.com/camunda/camunda-modeler/releases) to easily
-create\nZeebe BPMN XML workflows for MADAM.\n\n## Licensing\n\nMADAM is
-licensed under the [Gnu Public License Version 3](https://www.gnu.org/licenses/
-gpl-3.0.en.html).\n\nCamunda Modeler is licensed under [the MIT License (MIT)]
-(https://mit-license.org/).\n\nAt its core, MADAM use [adhesive-zebe](https://
-github.com/vtexier/adhesive), a BPMN workflow python engine able to\nexecute
-Zeebe BPMN XML workflows. It is a fork of [adhesive](https://github.com/
-germaniumhq/adhesive) under\nthe original adhesive license that is [GNU Affero
-General Public License v3.0](https://www.gnu.org/licenses/agpl-
-3.0.en.html)\n\n## System environment setup\n\n1. [Install Docker](https://
-docs.docker.com/engine/install/).\n\n2. [Configure userns-remap](https://
-docs.docker.com/engine/security/userns-remap/) to map container user `root` to
-a\n host non-root user.\n\n3. Configure the dev station as a [Docker Swarm
-Manager](https://docs.docker.com/engine/swarm/).\n\n4. Install a [Postgresql]
-(https://www.postgresql.org/download/) database server.\n \n_You can use the
-Ansible playbook provided to install PostgreSQL locally with Docker,\nafter
-configuring `hosts.yaml`:_\n\n make environment\n\n### Python environment
-setup\n\n* It requires Python 3.8+.\n\n* [Pyenv](https://github.com/pyenv/
-pyenv) should be used to choose the right version of Python, without breaking
-the\n default Python of the Operating System.\n\n* A Python virtual environment
-should be created in a `.venv` folder.\n\n```bash\n pyenv install 3.8.0\n pyenv
-shell 3.8.0\n python -m venv .venv \n source .venv/bin/activate`\n```\n\n###
-Installation/Update\n\nFrom PyPI:\n\nIn a Python virtualenv:\n\n pip install -
-U madam-mam\n\nIn your user install directory:\n\n pip install --user -U madam-
-mam\n\nYou should have a the `madam` cli command available:\n\n madam\n\nor\n\n
-madam --help\n\nwill display command usage.\n\nTo have bash completion, you can
-type:\n\n _MADAM_COMPLETE=source_bash madam > madam-complete.sh\n sudo cp
-madam-complete.sh /etc/bash_completion.d/.\n\nFor another shell, replace
-`source_bash` by `source_zsh` or `source_fish`\n\n### Development
-environment\n\nInstall [Poetry](https://python-poetry.org/) with the custom
-installer:\n\n curl -sSL https://raw.githubusercontent.com/python-poetry/
-poetry/master/get-poetry.py | python\n\nInstall Python dependencies:\n\n poetry
-install --no-root\n\nYou can use the madam-cli dev command:\n\n ./bin/madam-
-cli\n\nGet `bin/madam-cli` bash shell completion:\n\n
-_MADAM_CLI_COMPLETE=source_bash bin/madam-cli > madam-cli-complete.sh\n sudo cp
-madam-cli-complete.sh /etc/bash_completion.d/.\n\nFor another shell, replace
-`source_bash` by `source_zsh` or `source_fish`\n\n### Configuration\n\nMake a
-copy of the environment config example file:\n\n cp .env.example .env\n\nEdit
-`.env` to suit your needs, then:\n\n export $(grep -v \'^#\' .env | xargs -
-d \'\\n\')\n\nMake a copy of the Ansible inventory example file:\n\n cp
-hosts.yaml.example hosts.yaml\n\nEdit `hosts.yaml` to suit your needs.\n\nMake
-a copy of the MADAM config example file:\n\n cp madam.yaml.example
-madam.yaml\n\nEdit `madam.yaml` to suit your needs.\n\nMake a copy of the MADAM
-config example file for the test environment:\n\n cp madam_tests.yaml.example
-madam_tests.yaml\n\nEdit `madam_tests.yaml` to suit your needs.\n\nMake a copy
-of the MADAM config example file for the local deploy:\n\n cp
-madam_deploy.yaml.example madam_deploy.yaml\n\nEdit `madam_deploy.yaml` to suit
-your needs.\n\n### Set and tag project version in Git\n\n ./bin/release.sh
-1.0.0\n\n### Build MADAM python package and Docker image\n\n make build\n\nThe
-wheel package will be build in the `dist` directory.\n\n## Deploy MADAM as
-local docker container\n\nTo deploy MADAM container on localhost:\n\n make
-deploy\n\n## Check static type and code quality\n\n make check\n\n## Run
-tests\n\nRun all [pytest](https://docs.pytest.org) tests with:\n\n make
-tests\n\nRun only some tests by using `bin/tests.sh`:\n\n bin/tests.sh tests/
-domains/test_workflows.py::test_create\n\n## Database setup\n\nSet
-`DATABASE_URL` and `DATABASE_URL_TESTS` environment variable in `.env` file:
-\n\n DATABASE_URL=postgresql://postgres:xxxxx@hostname:5432/
-madam?sslmode=allow\n DATABASE_URL_TESTS=postgresql://postgres:xxxxx@hostname:
-5432/madam_tests?sslmode=allow\n\n### Migrations scripts\n\nAdd/Edit scripts in
-`resources/migrations` directory:\n\n # version.name.[rollback].sql\n
-00001.init_tables.sql\n 00001.init_tables.rollback.sql\n\n### Migrate
-commands\n\n make databases\n make databases_rollback\n make databases_list\n',
-'author': 'Vincent Texier', 'author_email': 'vit@free.fr', 'maintainer': None,
-'maintainer_email': None, 'url': None, 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'entry_points':
-entry_points, 'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: madam-mam Version: 0.7.2 Summary: MADAM (TM) Multi
+Agent Digital Asset Manager - a MAM server for Docker Swarm to handle higly
+distributed media processes License: GPL-3.0-only Keywords:
+BPMN,workflow,media,assets,management,MAM,DAM,docker,swarm Author: Vincent
+Texier Author-email: vit@free.fr Requires-Python: >=3.8,<4.0 Classifier:
+License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: Jinja2 (>=3.0.1,<4.0.0) Requires-Dist: PyYAML
+(==5.1.2) Requires-Dist: adhesive-zeebe (>=2021.4.3,<2022.0.0) Requires-Dist:
+ariadne (>=0.13.0,<0.14.0) Requires-Dist: docker (>=6.1.0,<7.0.0) Requires-
+Dist: lxml (>=4.6.3,<5.0.0) Requires-Dist: psycopg2-binary (>=2.8.6,<3.0.0)
+Requires-Dist: python-sql (>=1.2.2,<2.0.0) Requires-Dist: rich
+(>=10.2.2,<11.0.0) Requires-Dist: timecode (>=1.3.1,<2.0.0) Requires-Dist:
+uvicorn (>=0.14.0,<0.15.0) Requires-Dist: watchgod (>=0.7,<0.8) Requires-Dist:
+yoyo-migrations (>=8.2.0,<9.0.0) Description-Content-Type: text/markdown #
+MADAM MADAM is the Multi Agent Digital Asset Manager. It provides a three-tier
+architecture platform to handle workflow processing in a distributed
+environment. It uses Docker swarm to dispatch processes in a cluster of
+machines. It is a free (as freedom) software written in Python. ##
+Documentation [Link to the documentation](https://m5231.gitlab.io/
+documentation/) ## Support If you find this project useful and want to
+contribute, please submit issues, merge requests. If you use it regularly, you
+can help by the author by a financial support.
+ [Donate_using_Liberapay] ## Requirements You will need [Camunda Modeler 4.11+]
+(https://github.com/camunda/camunda-modeler/releases) to easily create Zeebe
+BPMN XML workflows for MADAM. ## Licensing MADAM is licensed under the [Gnu
+Public License Version 3](https://www.gnu.org/licenses/gpl-3.0.en.html).
+Camunda Modeler is licensed under [the MIT License (MIT)](https://mit-
+license.org/). At its core, MADAM use [adhesive-zebe](https://github.com/
+vtexier/adhesive), a BPMN workflow python engine able to execute Zeebe BPMN XML
+workflows. It is a fork of [adhesive](https://github.com/germaniumhq/adhesive)
+under the original adhesive license that is [GNU Affero General Public License
+v3.0](https://www.gnu.org/licenses/agpl-3.0.en.html) ## System environment
+setup 1. [Install Docker](https://docs.docker.com/engine/install/). 2.
+[Configure userns-remap](https://docs.docker.com/engine/security/userns-remap/
+) to map container user `root` to a host non-root user. 3. Configure the dev
+station as a [Docker Swarm Manager](https://docs.docker.com/engine/swarm/). 4.
+Install a [Postgresql](https://www.postgresql.org/download/) database server.
+_You can use the Ansible playbook provided to install PostgreSQL locally with
+Docker, after configuring `hosts.yaml`:_ make environment ### Python
+environment setup * It requires Python 3.8+. * [Pyenv](https://github.com/
+pyenv/pyenv) should be used to choose the right version of Python, without
+breaking the default Python of the Operating System. * A Python virtual
+environment should be created in a `.venv` folder. ```bash pyenv install 3.8.0
+pyenv shell 3.8.0 python -m venv .venv source .venv/bin/activate` ``` ###
+Installation/Update From PyPI: In a Python virtualenv: pip install -U madam-mam
+In your user install directory: pip install --user -U madam-mam You should have
+a the `madam` cli command available: madam or madam --help will display command
+usage. To have bash completion, you can type: _MADAM_COMPLETE=source_bash madam
+> madam-complete.sh sudo cp madam-complete.sh /etc/bash_completion.d/. For
+another shell, replace `source_bash` by `source_zsh` or `source_fish` ###
+Development environment Install [Poetry](https://python-poetry.org/) with the
+custom installer: curl -sSL https://raw.githubusercontent.com/python-poetry/
+poetry/master/get-poetry.py | python Install Python dependencies: poetry
+install --no-root Copy `bin/pre-commit.sh` for pre-commmit git hooks: cp bin/
+pre-commit.sh .git/hooks/pre-commit You can use the madam-cli dev command: ./
+bin/madam-cli Get `bin/madam-cli` bash shell completion:
+_MADAM_CLI_COMPLETE=source_bash bin/madam-cli > madam-cli-complete.sh sudo cp
+madam-cli-complete.sh /etc/bash_completion.d/. For another shell, replace
+`source_bash` by `source_zsh` or `source_fish` ### Configuration Make a copy of
+the environment config example file: cp .env.example .env Edit `.env` to suit
+your needs, then: export $(grep -v '^#' .env | xargs -d '\n') Make a copy of
+the Ansible inventory example file: cp hosts.yaml.example hosts.yaml Edit
+`hosts.yaml` to suit your needs. Make a copy of the MADAM config example file:
+cp madam.yaml.example madam.yaml Edit `madam.yaml` to suit your needs. Make a
+copy of the MADAM config example file for the test environment: cp
+madam_tests.yaml.example madam_tests.yaml Edit `madam_tests.yaml` to suit your
+needs. Make a copy of the MADAM config example file for the local deploy: cp
+madam_deploy.yaml.example madam_deploy.yaml Edit `madam_deploy.yaml` to suit
+your needs. ### Set and tag project version in Git ./bin/release.sh 1.0.0 ###
+Build MADAM python package and Docker image make build The wheel package will
+be build in the `dist` directory. Push docker image on private registry: docker
+image tag madam:[version] registry_hostname:registry_port/madam:[version]
+docker push registry_hostname:registry_port/madam:[version] ## Deploy MADAM as
+local docker container To deploy MADAM container on localhost: make deploy ##
+Check static type and code quality make check ## Run tests Run all [pytest]
+(https://docs.pytest.org) tests with: make tests Run only some tests by using
+`bin/tests.sh`: bin/tests.sh tests/domains/test_workflows.py::test_create ##
+Database setup Set `DATABASE_URL` and `DATABASE_URL_TESTS` environment variable
+in `.env` file: DATABASE_URL=postgresql://postgres:xxxxx@hostname:5432/
+madam?sslmode=allow DATABASE_URL_TESTS=postgresql://postgres:xxxxx@hostname:
+5432/madam_tests?sslmode=allow ### Migrations scripts Add/Edit scripts in
+`resources/migrations` directory: # version.name.[rollback].sql
+00001.init_tables.sql 00001.init_tables.rollback.sql ### Migrate commands make
+databases make databases_rollback make databases_list
```

