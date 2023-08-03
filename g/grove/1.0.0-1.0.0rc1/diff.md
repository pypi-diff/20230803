# Comparing `tmp/grove-1.0.0.tar.gz` & `tmp/grove-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grove-1.0.0.tar", last modified: Thu Aug  3 15:08:07 2023, max compression
+gzip compressed data, was "grove-1.0.0rc1.tar", last modified: Wed Feb 15 18:57:42 2023, max compression
```

## Comparing `grove-1.0.0.tar` & `grove-1.0.0rc1.tar`

### file list

```diff
@@ -1,419 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.399429 grove-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.355425 grove-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 15:07:45.000000 grove-1.0.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.355425 grove-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-03 15:07:45.000000 grove-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-03 15:07:45.000000 grove-1.0.0/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-03 15:07:45.000000 grove-1.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-08-03 15:07:45.000000 grove-1.0.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.355425 grove-1.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-03 15:07:45.000000 grove-1.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-03 15:07:45.000000 grove-1.0.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-03 15:07:45.000000 grove-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-03 15:07:45.000000 grove-1.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-08-03 15:08:07.399429 grove-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-08-03 15:07:45.000000 grove-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-03 15:07:45.000000 grove-1.0.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.355425 grove-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 15:07:45.000000 grove-1.0.0/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.355425 grove-1.0.0/docs/_generated/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:07:45.000000 grove-1.0.0/docs/_generated/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-03 15:07:45.000000 grove-1.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-03 15:07:45.000000 grove-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-08-03 15:07:45.000000 grove-1.0.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-03 15:07:45.000000 grove-1.0.0/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-03 15:07:45.000000 grove-1.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-08-03 15:07:45.000000 grove-1.0.0/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-03 15:07:45.000000 grove-1.0.0/docs/grove.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-08-03 15:07:45.000000 grove-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-08-03 15:07:45.000000 grove-1.0.0/docs/internals.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-03 15:07:45.000000 grove-1.0.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-08-03 15:07:45.000000 grove-1.0.0/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.359426 grove-1.0.0/docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-03 15:07:45.000000 grove-1.0.0/docs/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    51212 2023-08-03 15:07:45.000000 grove-1.0.0/docs/static/flow.png
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-08-03 15:07:45.000000 grove-1.0.0/docs/static/grove-logo-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-08-03 15:07:45.000000 grove-1.0.0/docs/static/grove-logo-small-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    19248 2023-08-03 15:07:45.000000 grove-1.0.0/docs/static/grove-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (123)    23315 2023-08-03 15:07:45.000000 grove-1.0.0/docs/static/grove-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    73194 2023-08-03 15:07:45.000000 grove-1.0.0/docs/static/grove-support-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    78562 2023-08-03 15:07:45.000000 grove-1.0.0/docs/static/grove-support.png
--rw-r--r--   0 runner    (1001) docker     (123)    53548 2023-08-03 15:07:45.000000 grove-1.0.0/docs/static/grove.png
--rw-r--r--   0 runner    (1001) docker     (123)    41033 2023-08-03 15:07:45.000000 grove-1.0.0/docs/static/plugin_structure.png
--rw-r--r--   0 runner    (1001) docker     (123)    69230 2023-08-03 15:07:45.000000 grove-1.0.0/docs/static/pointers.png
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-03 15:07:45.000000 grove-1.0.0/docs/style.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.359426 grove-1.0.0/grove/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-03 15:07:45.000000 grove-1.0.0/grove/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-03 15:07:45.000000 grove-1.0.0/grove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.359426 grove-1.0.0/grove/caches/
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-03 15:07:45.000000 grove-1.0.0/grove/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-08-03 15:07:45.000000 grove-1.0.0/grove/caches/aws_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-08-03 15:07:45.000000 grove-1.0.0/grove/caches/local_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.363426 grove-1.0.0/grove/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-03 15:07:45.000000 grove-1.0.0/grove/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-08-03 15:07:45.000000 grove-1.0.0/grove/configs/aws_ssm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-08-03 15:07:45.000000 grove-1.0.0/grove/configs/local_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.363426 grove-1.0.0/grove/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)    37612 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.363426 grove-1.0.0/grove/connectors/atlassian/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/atlassian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/atlassian/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/atlassian/audit_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.363426 grove-1.0.0/grove/connectors/github/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/github/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/github/audit_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.363426 grove-1.0.0/grove/connectors/gsuite/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/gsuite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/gsuite/activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/gsuite/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.363426 grove-1.0.0/grove/connectors/local/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/local/heartbeat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.363426 grove-1.0.0/grove/connectors/okta/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/okta/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/okta/system_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.363426 grove-1.0.0/grove/connectors/onepassword/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/onepassword/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/onepassword/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/onepassword/events_audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/onepassword/events_itemusages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/onepassword/events_signinattempts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.363426 grove-1.0.0/grove/connectors/oomnitza/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/oomnitza/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/oomnitza/activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/oomnitza/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.363426 grove-1.0.0/grove/connectors/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/pagerduty/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/pagerduty/audit_records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.363426 grove-1.0.0/grove/connectors/sf/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/sf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/sf/event_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.367426 grove-1.0.0/grove/connectors/sfmc/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/sfmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/sfmc/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/sfmc/audit_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/sfmc/security_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.367426 grove-1.0.0/grove/connectors/slack/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/slack/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/slack/audit_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.367426 grove-1.0.0/grove/connectors/tfc/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/tfc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/tfc/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/tfc/audit_trails.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.367426 grove-1.0.0/grove/connectors/tines/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/tines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/tines/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/tines/audit_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.367426 grove-1.0.0/grove/connectors/torq/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/torq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/torq/activity_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/torq/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/torq/audit_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.367426 grove-1.0.0/grove/connectors/twilio/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/twilio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/twilio/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/twilio/monitor_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.367426 grove-1.0.0/grove/connectors/workday/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/workday/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/workday/activity_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/workday/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.367426 grove-1.0.0/grove/connectors/zoom/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/zoom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/zoom/activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/zoom/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-03 15:07:45.000000 grove-1.0.0/grove/connectors/zoom/operationlogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-08-03 15:07:45.000000 grove-1.0.0/grove/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.371427 grove-1.0.0/grove/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-03 15:07:45.000000 grove-1.0.0/grove/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-08-03 15:07:45.000000 grove-1.0.0/grove/entrypoints/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-08-03 15:07:45.000000 grove-1.0.0/grove/entrypoints/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-03 15:07:45.000000 grove-1.0.0/grove/entrypoints/local_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-03 15:07:45.000000 grove-1.0.0/grove/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.371427 grove-1.0.0/grove/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 15:07:45.000000 grove-1.0.0/grove/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-08-03 15:07:45.000000 grove-1.0.0/grove/helpers/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-08-03 15:07:45.000000 grove-1.0.0/grove/helpers/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-08-03 15:07:45.000000 grove-1.0.0/grove/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-08-03 15:07:45.000000 grove-1.0.0/grove/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.371427 grove-1.0.0/grove/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-08-03 15:07:45.000000 grove-1.0.0/grove/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-08-03 15:07:45.000000 grove-1.0.0/grove/outputs/aws_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-08-03 15:07:45.000000 grove-1.0.0/grove/outputs/local_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-03 15:07:45.000000 grove-1.0.0/grove/outputs/local_stdout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.371427 grove-1.0.0/grove/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-03 15:07:45.000000 grove-1.0.0/grove/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-08-03 15:07:45.000000 grove-1.0.0/grove/processors/extract_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-08-03 15:07:45.000000 grove-1.0.0/grove/processors/filter_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-03 15:07:45.000000 grove-1.0.0/grove/processors/split_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.371427 grove-1.0.0/grove/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 15:07:45.000000 grove-1.0.0/grove/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-03 15:07:45.000000 grove-1.0.0/grove/secrets/aws_ssm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-08-03 15:07:45.000000 grove-1.0.0/grove/secrets/hashicorp_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-03 15:07:45.000000 grove-1.0.0/grove/secrets/local_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-03 15:07:45.000000 grove-1.0.0/grove/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.359426 grove-1.0.0/grove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-08-03 15:08:07.000000 grove-1.0.0/grove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-08-03 15:08:07.000000 grove-1.0.0/grove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:08:07.000000 grove-1.0.0/grove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-03 15:08:07.000000 grove-1.0.0/grove.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-03 15:08:07.000000 grove-1.0.0/grove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 15:08:07.000000 grove-1.0.0/grove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-08-03 15:07:45.000000 grove-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:08:07.399429 grove-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.371427 grove-1.0.0/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-03 15:07:45.000000 grove-1.0.0/templates/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.371427 grove-1.0.0/templates/code/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.371427 grove-1.0.0/templates/code/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/hooks/post_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.371427 grove-1.0.0/templates/code/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/scripts/run_cookiecutter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.335424 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/tests/test_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/example_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-03 15:07:45.000000 grove-1.0.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.339424 grove-1.0.0/templates/configuration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/configuration/1password/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/1password/events_audit.json
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/1password/events_itemusages.json
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/1password/events_signinattempts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/configuration/atlassian/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/atlassian/audit_events.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/configuration/github/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/github/enterprise_audit_log.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/github/orgs_audit_log.json
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/github/self-hosted_orgs_audit_log.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/configuration/gsuite/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/gsuite/activities.json
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/gsuite/alerts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/configuration/okta/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/okta/preview_system_log.json
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/okta/system_log.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/configuration/oomnitza/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/oomnitza/activities.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/configuration/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/pagerduty/audit_records.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/configuration/salesforce/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/salesforce/event_log.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.375427 grove-1.0.0/templates/configuration/slack/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/slack/audit_logs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.379428 grove-1.0.0/templates/configuration/tfc/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/tfc/audit_trails.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.379428 grove-1.0.0/templates/configuration/tines/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/tines/audit_logs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.379428 grove-1.0.0/templates/configuration/torq/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/torq/activity_logs.json
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/torq/audit_logs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.379428 grove-1.0.0/templates/configuration/twilio/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/twilio/messages.json
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/twilio/monitor_events.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.379428 grove-1.0.0/templates/configuration/workday/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/workday/activity_logging.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.379428 grove-1.0.0/templates/configuration/zoom/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/zoom/activities.json
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-03 15:07:45.000000 grove-1.0.0/templates/configuration/zoom/operationlogs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.343424 grove-1.0.0/templates/deployment/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.379428 grove-1.0.0/templates/deployment/local-quick-start/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/local-quick-start/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.379428 grove-1.0.0/templates/deployment/local-quick-start/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/local-quick-start/connectors/local_heartbeat.json
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/local-quick-start/test_entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.379428 grove-1.0.0/templates/deployment/terraform-aws-ecs/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/terraform-aws-ecs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.343424 grove-1.0.0/templates/deployment/terraform-aws-ecs/connectors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.379428 grove-1.0.0/templates/deployment/terraform-aws-ecs/connectors/local_heartbeat/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/terraform-aws-ecs/connectors/local_heartbeat/local_heartbeat.json
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/terraform-aws-ecs/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.343424 grove-1.0.0/templates/deployment/terraform-aws-ecs/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.379428 grove-1.0.0/templates/deployment/terraform-aws-ecs/modules/grove/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/terraform-aws-ecs/modules/grove/cloudwatch.tf
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/terraform-aws-ecs/modules/grove/compute.tf
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/terraform-aws-ecs/modules/grove/dynamodb.tf
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/terraform-aws-ecs/modules/grove/iam.tf
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/terraform-aws-ecs/modules/grove/network.tf
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/terraform-aws-ecs/modules/grove/output.tf
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/terraform-aws-ecs/modules/grove/s3.tf
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/terraform-aws-ecs/modules/grove/variables.tf
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/terraform-aws-ecs/output.tf
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/terraform-aws-ecs/providers.tf
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-03 15:07:45.000000 grove-1.0.0/templates/deployment/terraform-aws-ecs/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.387428 grove-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 15:07:45.000000 grove-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.387428 grove-1.0.0/tests/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 15:07:45.000000 grove-1.0.0/tests/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-03 15:07:45.000000 grove-1.0.0/tests/connectors/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.351425 grove-1.0.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.343424 grove-1.0.0/tests/fixtures/atlassian/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.387428 grove-1.0.0/tests/fixtures/atlassian/event_audit/
--rw-r--r--   0 runner    (1001) docker     (123)    76068 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/atlassian/event_audit/001.json
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/atlassian/event_audit/002.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.343424 grove-1.0.0/tests/fixtures/github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.387428 grove-1.0.0/tests/fixtures/github/audit/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/github/audit/001.json
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/github/audit/002.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.343424 grove-1.0.0/tests/fixtures/grove/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.387428 grove-1.0.0/tests/fixtures/grove/chronological/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/grove/chronological/001.json
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/grove/chronological/002.json
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/grove/chronological/003.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.387428 grove-1.0.0/tests/fixtures/grove/reverse_chronological/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/grove/reverse_chronological/001.json
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/grove/reverse_chronological/002.json
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/grove/reverse_chronological/003.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.343424 grove-1.0.0/tests/fixtures/gsuite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.391429 grove-1.0.0/tests/fixtures/gsuite/activities/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/gsuite/activities/001.json
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/gsuite/activities/002.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.391429 grove-1.0.0/tests/fixtures/gsuite/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/gsuite/alerts/001.json
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/gsuite/alerts/002.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.347425 grove-1.0.0/tests/fixtures/okta/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.391429 grove-1.0.0/tests/fixtures/okta/system_log/
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/okta/system_log/001.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/okta/system_log/002.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.347425 grove-1.0.0/tests/fixtures/onepassword/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.391429 grove-1.0.0/tests/fixtures/onepassword/events_audit/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/onepassword/events_audit/001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/onepassword/events_audit/002.json
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/onepassword/events_audit/003.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.391429 grove-1.0.0/tests/fixtures/onepassword/events_itemusages/
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/onepassword/events_itemusages/001.json
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/onepassword/events_itemusages/002.json
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/onepassword/events_itemusages/003.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.391429 grove-1.0.0/tests/fixtures/onepassword/events_signinattempts/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/onepassword/events_signinattempts/001.json
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/onepassword/events_signinattempts/002.json
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/onepassword/events_signinattempts/003.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.347425 grove-1.0.0/tests/fixtures/oomnitza/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.391429 grove-1.0.0/tests/fixtures/oomnitza/activities/
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/oomnitza/activities/001.json
--rw-r--r--   0 runner    (1001) docker     (123)    77536 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/oomnitza/activities/002.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/oomnitza/activities/003.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.347425 grove-1.0.0/tests/fixtures/pagerduty/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.391429 grove-1.0.0/tests/fixtures/pagerduty/audit_records/
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/pagerduty/audit_records/001.json
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/pagerduty/audit_records/002.json
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/pagerduty/audit_records/003.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.347425 grove-1.0.0/tests/fixtures/sf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.391429 grove-1.0.0/tests/fixtures/sf/event_log/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/sf/event_log/001.csv
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/sf/event_log/001.json
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/sf/event_log/error.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/sf/event_log/login.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.347425 grove-1.0.0/tests/fixtures/sfmc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.395429 grove-1.0.0/tests/fixtures/sfmc/audit_events/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/sfmc/audit_events/001.json
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/sfmc/audit_events/002.json
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/sfmc/audit_events/003.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.395429 grove-1.0.0/tests/fixtures/sfmc/security_events/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/sfmc/security_events/001.json
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/sfmc/security_events/002.json
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/sfmc/security_events/003.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.347425 grove-1.0.0/tests/fixtures/slack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.395429 grove-1.0.0/tests/fixtures/slack/audit/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/slack/audit/001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/slack/audit/002.json
--rw-r--r--   0 runner    (1001) docker     (123)    20726 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/slack/audit/003.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.347425 grove-1.0.0/tests/fixtures/tfc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.395429 grove-1.0.0/tests/fixtures/tfc/audit_trails/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/tfc/audit_trails/001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/tfc/audit_trails/002.json
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/tfc/audit_trails/003.json
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/tfc/audit_trails/004.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.347425 grove-1.0.0/tests/fixtures/tines/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.395429 grove-1.0.0/tests/fixtures/tines/audit_logs/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/tines/audit_logs/001.json
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/tines/audit_logs/002.json
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/tines/audit_logs/003.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.351425 grove-1.0.0/tests/fixtures/torq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.395429 grove-1.0.0/tests/fixtures/torq/activity/
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/torq/activity/001.json
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/torq/activity/002.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.395429 grove-1.0.0/tests/fixtures/torq/audit/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/torq/audit/001.json
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/torq/audit/002.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.395429 grove-1.0.0/tests/fixtures/torq/client/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/torq/client/001.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.351425 grove-1.0.0/tests/fixtures/workday/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.395429 grove-1.0.0/tests/fixtures/workday/activity_logging/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/workday/activity_logging/001.json
--rw-r--r--   0 runner    (1001) docker     (123)    39041 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/workday/activity_logging/002.json
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/workday/activity_logging/003.json
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/workday/activity_logging/004.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/workday/activity_logging/005.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.351425 grove-1.0.0/tests/fixtures/zoom/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.395429 grove-1.0.0/tests/fixtures/zoom/activities/
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/zoom/activities/001.json
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/zoom/activities/002.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.399429 grove-1.0.0/tests/fixtures/zoom/client/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/zoom/client/001.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.399429 grove-1.0.0/tests/fixtures/zoom/operation/
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/zoom/operation/001.json
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-03 15:07:45.000000 grove-1.0.0/tests/fixtures/zoom/operation/002.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:08:07.399429 grove-1.0.0/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-03 15:07:45.000000 grove-1.0.0/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-03 15:07:45.000000 grove-1.0.0/tests/mocks/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_caches_local_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_configs_aws_ssm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_atlassian_audit_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_deduplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_github_audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_github_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_gsuite_activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_gsuite_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_okta_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_okta_system_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_onepassword_events_audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_onepassword_events_itemusages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_onepassword_events_signinattempts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_oomnitza_activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_pagerduty_audit_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_sf_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_sfmc_audit_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_sfmc_security_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_slack_audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_tfc_audit_trails.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_tines_audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_torq_activity_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_torq_audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_torq_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_workday_activity_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_zoom_activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_zoom_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_connectors_zoom_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_e2e_grove_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_helpers_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_outputs_aws_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_outputs_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_processors_extract_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_processors_filter_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_processors_split_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_secrets_hashicorp_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-03 15:07:45.000000 grove-1.0.0/tests/test_secrets_local_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.610627 grove-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-02-15 18:57:34.000000 grove-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-02-15 18:57:42.610627 grove-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-02-15 18:57:34.000000 grove-1.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.598627 grove-1.0.0rc1/grove/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.598627 grove-1.0.0rc1/grove/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/caches/aws_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/caches/local_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.598627 grove-1.0.0rc1/grove/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/configs/aws_ssm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/configs/local_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.598627 grove-1.0.0rc1/grove/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)    33601 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.598627 grove-1.0.0rc1/grove/connectors/atlassian/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/atlassian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/atlassian/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/atlassian/audit_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.598627 grove-1.0.0rc1/grove/connectors/github/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/github/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/github/audit_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.598627 grove-1.0.0rc1/grove/connectors/gsuite/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/gsuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/gsuite/activities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/gsuite/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.598627 grove-1.0.0rc1/grove/connectors/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/local/heartbeat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.598627 grove-1.0.0rc1/grove/connectors/okta/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/okta/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/okta/system_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.602627 grove-1.0.0rc1/grove/connectors/onepassword/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/onepassword/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/onepassword/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/onepassword/events_itemusages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/onepassword/events_signinattempts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.602627 grove-1.0.0rc1/grove/connectors/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/pagerduty/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/pagerduty/audit_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.602627 grove-1.0.0rc1/grove/connectors/sf/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/sf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/sf/event_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.602627 grove-1.0.0rc1/grove/connectors/sfmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/sfmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/sfmc/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/sfmc/audit_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/sfmc/security_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.602627 grove-1.0.0rc1/grove/connectors/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/slack/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/slack/audit_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.602627 grove-1.0.0rc1/grove/connectors/tfc/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/tfc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/tfc/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/tfc/audit_trails.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.602627 grove-1.0.0rc1/grove/connectors/torq/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/torq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/torq/activity_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/torq/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/torq/audit_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.602627 grove-1.0.0rc1/grove/connectors/twilio/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/twilio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/twilio/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/twilio/monitor_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.602627 grove-1.0.0rc1/grove/connectors/workday/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/workday/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/workday/activity_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/workday/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.602627 grove-1.0.0rc1/grove/connectors/zoom/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/zoom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/zoom/activities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/zoom/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/connectors/zoom/operationlogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.606627 grove-1.0.0rc1/grove/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/entrypoints/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/entrypoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/entrypoints/local_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.606627 grove-1.0.0rc1/grove/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/helpers/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/helpers/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.606627 grove-1.0.0rc1/grove/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/outputs/aws_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/outputs/local_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/outputs/local_stdout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.606627 grove-1.0.0rc1/grove/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/secrets/aws_ssm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-02-15 18:57:34.000000 grove-1.0.0rc1/grove/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.598627 grove-1.0.0rc1/grove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-02-15 18:57:42.000000 grove-1.0.0rc1/grove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-02-15 18:57:42.000000 grove-1.0.0rc1/grove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 18:57:42.000000 grove-1.0.0rc1/grove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-02-15 18:57:42.000000 grove-1.0.0rc1/grove.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-15 18:57:42.000000 grove-1.0.0rc1/grove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-15 18:57:42.000000 grove-1.0.0rc1/grove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-02-15 18:57:42.610627 grove-1.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-02-15 18:57:34.000000 grove-1.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:57:42.610627 grove-1.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_caches_local_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_configs_aws_ssm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_atlassian_audit_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_deduplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_github_audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_github_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_gsuite_activities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_gsuite_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_okta_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_okta_system_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_onepassword_events_itemusages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_onepassword_events_signinattempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_pagerduty_audit_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_sf_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_sfmc_audit_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_sfmc_security_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_slack_audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_tfc_audit_trails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_torq_activity_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_torq_audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_torq_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_workday_activity_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_zoom_activities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_zoom_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_connectors_zoom_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_e2e_grove_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_outputs_aws_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-02-15 18:57:34.000000 grove-1.0.0rc1/tests/test_outputs_base.py
```

### Comparing `grove-1.0.0/LICENSE` & `grove-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/PKG-INFO` & `grove-1.0.0rc1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,60 @@
 Metadata-Version: 2.1
 Name: grove
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: A Software as a Service (SaaS) log collection framework.
 Author: HashiCorp Security (TDR)
-License: MPL-2.0
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Natural Language :: English
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
-<p align="center">
-    <br /><br />
-    <picture>
-      <source media="(prefers-color-scheme: dark)" srcset="docs/static/grove-logo-small-light.png?raw=True">
-      <source media="(prefers-color-scheme: light)" srcset="docs/static/grove-logo-small.png?raw=True">
-      <img src="docs/static/grove-logo-small.png?raw=True" alt="Grove logo">
-    </picture>
-    <br /><br />
-</p>
+## Grove
+
+> Grove is not an official HashiCorp project.
 
 Grove is a Software as a Service (SaaS) log collection framework, designed to support
 collection of logs from services which do not natively support log streaming.
 
 Grove enables teams to collect security related events from their vendors in a reliable
 and consistent way. This data may then be stored and analyzed with a team's _existing_
 tooling in order to support threat detection and compliance programmes.
 
 Out of the box, Grove provides:
 
-* 🪵 Reliable and periodic collection of logs.
+* 🪵 Reliable and periodic log collection of logs.
 * ☁️ Support a large number of widely used SaaS applications and services.
 * 🧱 Plugin based "connectors" to enable support for new applications and services.
 * 🧳 "Bring your own" caching, output, configuration, and secrets backends.
 
 Grove was created and is currently maintained by the HashiCorp security team.
 
 **Please note**: While this is not an official HashiCorp project, security is still very
 important to us! If you have found a potential security issue with Grove, please contact
 us via email at security@hashicorp.com, rather than filing a GitHub issue.
 
 ### Supported Sources
 
-<p align="center">
-    <br /><br />
-    <picture>
-      <source media="(prefers-color-scheme: dark)" srcset="docs/static/grove-support-light.png?raw=True">
-      <source media="(prefers-color-scheme: light)" srcset="docs/static/grove-support.png?raw=True">
-      <img src="docs/static/grove-support.png?raw=True" alt="Overview of supported services, also listed below" >
-    </picture>
-    <br />
-</p>
-
 Currently the following log sources are supported by Grove out of the box. If a source
 isn't listed here, support can be added by creating a custom connector!
 
 * Atlassian audit events (e.g. Confluence, Jira)
 * GitHub audit logs
 * GSuite alerts
 * GSuite activity logs
 * Okta system logs
-* Oomnitza activity logs
 * 1Password sign-in attempt logs
 * 1Password item usage event logs
-* 1Password audit logs
 * PagerDuty audit records
 * SalesForce Cloud event logs
 * SalesForce Marketing Cloud audit event logs
 * SalesForce Marketing Cloud security event logs
 * Slack audit logs
-* Tines audit logs
 * Terraform Cloud audit trails
 * Torq activity logs
 * Torq audit logs
 * Twilio monitor events
 * Twilio message logs
 * Workday activity logs
 * Zoom activity logs
```

### Comparing `grove-1.0.0/README.md` & `grove-1.0.0rc1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,48 @@
-<p align="center">
-    <br /><br />
-    <picture>
-      <source media="(prefers-color-scheme: dark)" srcset="docs/static/grove-logo-small-light.png?raw=True">
-      <source media="(prefers-color-scheme: light)" srcset="docs/static/grove-logo-small.png?raw=True">
-      <img src="docs/static/grove-logo-small.png?raw=True" alt="Grove logo">
-    </picture>
-    <br /><br />
-</p>
+## Grove
+
+> Grove is not an official HashiCorp project.
 
 Grove is a Software as a Service (SaaS) log collection framework, designed to support
 collection of logs from services which do not natively support log streaming.
 
 Grove enables teams to collect security related events from their vendors in a reliable
 and consistent way. This data may then be stored and analyzed with a team's _existing_
 tooling in order to support threat detection and compliance programmes.
 
 Out of the box, Grove provides:
 
-* 🪵 Reliable and periodic collection of logs.
+* 🪵 Reliable and periodic log collection of logs.
 * ☁️ Support a large number of widely used SaaS applications and services.
 * 🧱 Plugin based "connectors" to enable support for new applications and services.
 * 🧳 "Bring your own" caching, output, configuration, and secrets backends.
 
 Grove was created and is currently maintained by the HashiCorp security team.
 
 **Please note**: While this is not an official HashiCorp project, security is still very
 important to us! If you have found a potential security issue with Grove, please contact
 us via email at security@hashicorp.com, rather than filing a GitHub issue.
 
 ### Supported Sources
 
-<p align="center">
-    <br /><br />
-    <picture>
-      <source media="(prefers-color-scheme: dark)" srcset="docs/static/grove-support-light.png?raw=True">
-      <source media="(prefers-color-scheme: light)" srcset="docs/static/grove-support.png?raw=True">
-      <img src="docs/static/grove-support.png?raw=True" alt="Overview of supported services, also listed below" >
-    </picture>
-    <br />
-</p>
-
 Currently the following log sources are supported by Grove out of the box. If a source
 isn't listed here, support can be added by creating a custom connector!
 
 * Atlassian audit events (e.g. Confluence, Jira)
 * GitHub audit logs
 * GSuite alerts
 * GSuite activity logs
 * Okta system logs
-* Oomnitza activity logs
 * 1Password sign-in attempt logs
 * 1Password item usage event logs
-* 1Password audit logs
 * PagerDuty audit records
 * SalesForce Cloud event logs
 * SalesForce Marketing Cloud audit event logs
 * SalesForce Marketing Cloud security event logs
 * Slack audit logs
-* Tines audit logs
 * Terraform Cloud audit trails
 * Torq activity logs
 * Torq audit logs
 * Twilio monitor events
 * Twilio message logs
 * Workday activity logs
 * Zoom activity logs
```

### Comparing `grove-1.0.0/grove/caches/__init__.py` & `grove-1.0.0rc1/grove/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/caches/aws_dynamodb.py` & `grove-1.0.0rc1/grove/caches/aws_dynamodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,20 +29,18 @@
     """
 
     table: str = Field(
         default="grove",
         description="The name of the AWS DynamoDB table to use for the cache.",
     )
     url: Optional[str] = Field(
-        description="An optional URL to use when connecting to AWS DynamoDB.",
-        default=None,
+        description="An optional URL to use when connecting to AWS DynamoDB."
     )
     assume_role_arn: Optional[str] = Field(
-        description="An optional AWS role to assume when authenticating with AWS.",
-        default=None,
+        description="An optional AWS role to assume when authenticating with AWS."
     )
     table_region: Optional[str] = Field(
         description="The region that the DynamoDB table exists in (default us-east-1)",
         default=os.environ.get("AWS_REGION", "us-east-1"),
     )
 
     class Config:
```

### Comparing `grove-1.0.0/grove/caches/local_memory.py` & `grove-1.0.0rc1/grove/caches/local_memory.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/configs/__init__.py` & `grove-1.0.0rc1/grove/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/configs/aws_ssm.py` & `grove-1.0.0rc1/grove/configs/aws_ssm.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
     """
 
     prefix: Optional[str] = Field(
         default="/grove/connectors/",
         description="A prefix to added to the beginning of all parameter store paths.",
     )
     assume_role_arn: Optional[str] = Field(
-        description="An optional AWS role to assume when authenticating with AWS.",
-        default=None,
+        description="An optional AWS role to assume when authenticating with AWS."
     )
     ssm_region: Optional[str] = Field(
         description="The region that the parameter store exists in (default us-east-1)",
         default=os.environ.get("AWS_REGION", "us-east-1"),
     )
 
     class Config:
```

### Comparing `grove-1.0.0/grove/configs/local_file.py` & `grove-1.0.0rc1/grove/configs/local_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     """A configuration handler to read configuration documents from local files."""
 
     def __init__(self):
         self.logger = logging.getLogger(__name__)
 
         # Wrap validation errors to keep them in the Grove exception hierarchy.
         try:
-            self.config = Configuration()  # type: ignore
+            self.config = Configuration()
         except ValidationError as err:
             raise ConfigurationException(parsing.validation_error(err))
 
     def get(self, id: str = "") -> List[ConnectorConfig]:
         """Get and return one or more connector configuration objects from local files.
 
         :param id: Not used.
```

### Comparing `grove-1.0.0/grove/connectors/__init__.py` & `grove-1.0.0rc1/grove/connectors/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import abc
 import datetime
 import hashlib
 import json
 import logging
 import os
 from typing import Any, Dict, List, Optional
+from grove.__about__ import __version__
 
 import jmespath
 
-from grove.__about__ import __version__
 from grove.constants import (
     CACHE_KEY_LOCK,
     CACHE_KEY_POINTER,
     CACHE_KEY_POINTER_NEXT,
     CACHE_KEY_POINTER_PREV,
     CACHE_KEY_SEEN,
     CACHE_KEY_WINDOW_END,
@@ -29,28 +29,25 @@
     DEFAULT_OUTPUT_HANDLER,
     ENV_GROVE_CACHE_HANDLER,
     ENV_GROVE_LOCK_DURATION,
     ENV_GROVE_OUTPUT_HANDLER,
     LOCK_DATE_FORMAT,
     PLUGIN_GROUP_CACHE,
     PLUGIN_GROUP_OUTPUT,
-    PLUGIN_GROUP_PROCESSOR,
     REVERSE_CHRONOLOGICAL,
 )
 from grove.exceptions import (
     AccessException,
     ConcurrencyException,
-    ConfigurationException,
     DataFormatException,
     GroveException,
     NotFoundException,
-    ProcessorError,
 )
-from grove.helpers import parsing, plugin
-from grove.models import ConnectorConfig, OutputStream
+from grove.helpers import plugin
+from grove.models import ConnectorConfig
 
 
 class BaseConnector:
     NAME = "base"
     POINTER_PATH = "NOT_SET"
     LOG_ORDER = REVERSE_CHRONOLOGICAL
 
@@ -77,70 +74,50 @@
         self.log_context = {
             "operation": self.operation,
             "connector": self.__class__.__module__,
             "identity": self.identity,
         }
 
         # Let the caller handle exceptions from failure to load handlers directly.
-        self._cache = plugin.load_handler(
-            os.environ.get(ENV_GROVE_CACHE_HANDLER, DEFAULT_CACHE_HANDLER),
-            PLUGIN_GROUP_CACHE,
-        )
         self._output = plugin.load_handler(
             os.environ.get(ENV_GROVE_OUTPUT_HANDLER, DEFAULT_OUTPUT_HANDLER),
             PLUGIN_GROUP_OUTPUT,
         )
-        self._output.setup()
-
-        # Processors are only setup once for each connector instance.
-        self._processors = {}
-
-        for processor in self.configuration.processors:
-            try:
-                self._processors[processor.name] = plugin.load_handler(
-                    processor.processor,
-                    PLUGIN_GROUP_PROCESSOR,
-                    processor,
-                )
-            except ConfigurationException as err:
-                raise ProcessorError(
-                    f"Failed to initialise processor '{processor.name}' "
-                    f"({processor.processor}). {err}",
-                )
+        self._cache = plugin.load_handler(
+            os.environ.get(ENV_GROVE_CACHE_HANDLER, DEFAULT_CACHE_HANDLER),
+            PLUGIN_GROUP_CACHE,
+        )
 
         # The time that our current lock expires, if we have one.
         self._lock_expiry: Optional[datetime.datetime] = None
 
         try:
             self._lock_duration = int(
                 os.environ.get(ENV_GROVE_LOCK_DURATION, DEFAULT_LOCK_DURATION)
             )
         except ValueError as err:
             self.logger.warning(
                 f"Lock duration ('{ENV_GROVE_LOCK_DURATION}') must be a number.",
-                extra={"exception": err, **self.log_context},
+                extra={"exception": err},
             )
 
         # Determines if the start of a 'window' has been passed during a collection.
         # This is used to track windows which span multiple pages of results and is only
         # applicable for logs collected in reverse chronological order.
         self._window_passed = False
         self._window_start = str()
         self._window_end = str()
 
+        # Tracks the total number of saved log entries.
+        self._saved = 0
+
         # Paginated / chunked data needs an incrementing identifier to keep things
         # orderly.
         self._part = 0
 
-        # Track the number of output logs by the configured output destination stream.
-        # This allows statistics to be generated on deduplication, splitting, etc.
-        self._saved = {}
-        for descriptor, _ in self.configuration.outputs.items():
-            self._saved[descriptor] = 0
-
         # Tracks hashes of unique log entries, keyed by their pointer value.
         self._hashes: Dict[str, set[str]] = {}
 
         # Pointers track the last collected record in order for collection to continue
         # at the correct place between runs. A "next" pointer is only applicable for
         # logs collected in reverse chronological order.
         self._pointer = str()
@@ -164,15 +141,15 @@
             )
 
         # Perform collection.
         try:
             self.collect()
         except GroveException as err:
             self.logger.error(
-                "Connector was unable to complete collection successfully.",
+                "Connector was unable to collect logs.",
                 extra={"exception": err, **self.log_context},
             )
             self.unlock()
             return
 
         # Call the correct post run method.
         if self.LOG_ORDER == CHRONOLOGICAL:
@@ -182,18 +159,17 @@
             self._run_reverse_chronological()
 
         # TODO: The use of a context manager for lock management would be best.
         self.unlock()
 
     def _run_chronological(self):
         """Performs chronological specific post collection operations."""
-        # TODO: Move to processor.
         try:
             self.logger.debug(
-                "Saving deduplication hashes to cache.",
+                "Saving deduplication hashes to cache",
                 extra=self.log_context,
             )
             self.save_hashes()
         except AccessException as err:
             self.logger.error(
                 "Failed to save hashes to cache.",
                 extra={"exception": err, **self.log_context},
@@ -213,15 +189,15 @@
             self.logger.error(
                 "Connector failed to save pointer, cannot continue.",
                 extra={"exception": err, **self.log_context},
             )
             return
         except NotFoundException:
             self.logger.debug(
-                "Skipping pointer swap and clean-up as there is no next-pointer.",
+                "Skipping pointer swap and clean-up as there is no next-pointer",
                 extra={**self.log_context},
             )
             return
 
         # If the collection complete without error delete the window locations and
         # the next pointer from cache, if set.
         try:
@@ -244,15 +220,14 @@
         except AccessException as err:
             self.logger.error(
                 "Failed to clean up windows and next pointer from cache.",
                 extra={"exception": err, **self.log_context},
             )
             return
 
-        # TODO: Move to processor.
         try:
             self.logger.debug(
                 "Saving deduplication hashes to cache",
                 extra=self.log_context,
             )
             self.save_hashes()
         except AccessException as err:
@@ -263,127 +238,82 @@
             return
 
     @abc.abstractmethod
     def collect(self):
         """Provides a stub for a connector to initiate a collection."""
         pass
 
-    def process_and_write(self, entries: List[Any]):
-        """Write log entries them to the configured output handler.
+    def save(self, candidates: List[Any]):
+        """Saves log candidates, and updates the pointer in the cache.
 
-        :param entries: List of log entries to process.
-        """
-        # Allow failures to bubble all the way up and fail the run. If processing fails
-        # we want to defer collection, to allow retry later. We always pass a copy of
-        # the entries to prevent accidental overwriting of the collected raw data by
-        # a processor.
-        processed = self.process(entries)
-
-        for descriptor, stream in self.configuration.outputs.items():
-            # Ensure the output uses the correct stream.
-            to_save = entries
-            if stream == OutputStream.processed:
-                to_save = processed
-
-            number_of_entries = len(to_save)
-            if number_of_entries < 1:
-                self.logger.info(
-                    "No log entries to output for stream, skipping.",
-                    extra={
-                        "stream": stream,
-                        "descriptor": descriptor,
-                        **self.log_context,
-                    },
-                )
-                continue
-
-            try:
-                self._output.submit(
-                    data=self._output.serialize(
-                        data=to_save,
-                        metadata=self.metadata(),
-                    ),
-                    part=self._part,
-                    operation=self.operation,
-                    connector=self.NAME,
-                    identity=self.identity,
-                    descriptor=descriptor,
-                )
+        :param candidates: List of log candidates to save.
 
-                # Update counters.
-                self._saved[descriptor] += number_of_entries
+        :raises GroveException: The LOG_ORDER defined by the Connector is not valid.
 
-                self.logger.info(
-                    "Log submitted successfully to output.",
-                    extra={
-                        "part": self._part,
-                        "stream": stream,
-                        "descriptor": descriptor,
-                        "entries": number_of_entries,
-                        **self.log_context,
-                    },
-                )
-            except AccessException as err:
-                self.logger.error(
-                    "Failed to write logs to output, cannot continue.",
-                    extra={
-                        "part": self._part,
-                        "exception": err,
-                        "stream": stream,
-                        "descriptor": descriptor,
-                        **self.log_context,
-                    },
-                )
-                raise
-
-    def save(self, entries: List[Any]):
-        """Saves log entries, and updates the pointer in the cache.
-
-        :param entries: List of log entries to save.
+        :return: A count of entries saved.
         """
-        # TODO: Move deduplication into a processor.
-        entries = self.deduplicate_by_hash(entries)
+        entries = self.deduplicate_by_hash(candidates)
 
         if len(entries) < 1:
             self.logger.warning(
                 "No log entries to save, skipping.", extra=self.log_context
             )
             return
 
         # Always refresh our lock while saving. This allows us to grab a new lock for
         # every page of data to try and prevent our lock expiring before we've performed
         # a full collection.
-        #
-        # Unlock is not called here, as it's performed by the caller.
         self.lock()
 
         if self.LOG_ORDER == CHRONOLOGICAL:
-            self._save_chronological(entries)
+            return self._save_chronological(entries)
 
         if self.LOG_ORDER == REVERSE_CHRONOLOGICAL:
-            self._save_reverse_chronological(entries)
+            return self._save_reverse_chronological(entries)
 
-        self.finalize()
+        # Fall through for anything not supported / incorrectly specified.
+        raise GroveException(f"Connector LOG_ORDER '{self.LOG_ORDER}' is not valid.")
 
-    def _save_chronological(self, entries: List[Any]):
+    def _save_chronological(self, candidates: List[Any]):
         """Saves log entries when retrieved logs are in chronological order.
 
-        :param entries: List of log entries to save.
+        :param candidates: List of log entries to save.
         """
-        # Pointers are extracted prior to processing as processing may modify the
-        # structure, or remove entries entirely.
-        newest = jmespath.search(self.POINTER_PATH, entries[-1])
+        newest = jmespath.search(self.POINTER_PATH, candidates[-1])
+
         if newest is None:
-            raise GroveException(
-                f"Pointer path ({self.POINTER_PATH}) was not found in returned logs."
+            self.logger.error(
+                "Pointer path was not found in returned logs, cannot continue.",
+                extra={"pointer_path": self.POINTER_PATH, **self.log_context},
             )
+            return
 
-        # Exceptions are allowed to bubble up here to ensure connectors exit on error,
-        # rather than silently dropping batches of log entries.
-        self.process_and_write(entries)
+        # Generate metadata for the candidate log entries, and save to the output
+        # handler.
+        try:
+            self._output.submit(
+                data=self._output.serialize(
+                    data=candidates,
+                    metadata=self.metadata(),
+                ),
+                part=self._part,
+                operation=self.operation,
+                connector=self.NAME,
+                identity=self.identity,
+            )
+            self.logger.info(
+                "Log submitted successfully to output.",
+                extra={"part": self._part, **self.log_context},
+            )
+        except AccessException as err:
+            self.logger.error(
+                "Failed to write logs to output, cannot continue.",
+                extra={"exception": err, **self.log_context},
+            )
+            return
 
         # Once uploaded, then update the pointer. NOTE: There is an opportunity for
         # issues to occur between the output and pointer update which would lead to
         # duplicate data.
         try:
             self.pointer = newest
             self.logger.info(
@@ -391,18 +321,19 @@
                 extra={"pointer": newest, **self.log_context},
             )
         except AccessException as err:
             self.logger.error(
                 "Failed to save pointer to cache, cannot continue.",
                 extra={"exception": err, **self.log_context},
             )
-            raise
+            return
 
-        # Get ready for the next batch of candidate log entries (if required).
+        # Get ready for the next block of candidate log entries (if required).
         self._part += 1
+        self._saved += len(candidates)
 
     def _save_reverse_chronological(self, candidates: List[Any]):  # noqa: C901
         """Save log entries when logs are in reverse chronological order.
 
         Data returned in reverse chronological order is more complicated to handle,
         as the data may be paginated, and the execution environment "unreliable". This
         results in more operations are against the cache.
@@ -413,17 +344,19 @@
         :param candidates: List of log entries to save.
         """
         entries = []
         oldest = jmespath.search(self.POINTER_PATH, candidates[-1])
         newest = jmespath.search(self.POINTER_PATH, candidates[0])
 
         if oldest is None or newest is None:
-            raise GroveException(
-                f"Pointer path ({self.POINTER_PATH}) was not found in returned logs."
+            self.logger.error(
+                "Pointer path was not found in logs entry, cannot continue.",
+                extra={"pointer_path": self.POINTER_PATH, **self.log_context},
             )
+            return
 
         # If a window start is in the cache then a previous collection is incomplete.
         # We'll skip entries until we find our window, and then only collect entries
         # which are ON AND AFTER the end of the window. Any skipped entries will be
         # fetched by subsequent collections.
         incomplete_collection = False
 
@@ -434,17 +367,19 @@
             pass
 
         if incomplete_collection:
             for entry in candidates:
                 current_pointer = jmespath.search(self.POINTER_PATH, entry)
 
                 if current_pointer is None:
-                    raise GroveException(
-                        f"Pointer path ({self.POINTER_PATH}) not found in log entry."
+                    self.logger.error(
+                        "Pointer path was not found in logs entry, cannot continue.",
+                        extra={"pointer_path": self.POINTER_PATH, **self.log_context},
                     )
+                    return
 
                 # We need to track FROM the window end, inclusive, to ensure that we
                 # don't miss any logs. This is required in cases where the timestamp
                 # granularity from the upstream API is only seconds (as always, we
                 # prefer duplicates to missing logs).
                 #
                 # TODO: There is a condition here were duplicates are not considered.
@@ -470,20 +405,40 @@
             self.window_start = newest
             self.window_end = oldest
             self.pointer_next = newest
 
         if len(entries) < 1:
             return
 
-        # Exceptions are allowed to bubble up here to ensure connectors exit on error,
-        # rather than silently dropping batches of log entries.
-        self.process_and_write(entries)
+        # Generate metadata for the entries, and save to the output handler.
+        try:
+            self._output.submit(
+                data=self._output.serialize(
+                    data=entries,
+                    metadata=self.metadata(),
+                ),
+                part=self._part,
+                operation=self.operation,
+                connector=self.NAME,
+                identity=self.identity,
+            )
+            self.logger.info(
+                "Log submitted successfully to output.",
+                extra={"part": self._part, **self.log_context},
+            )
+        except AccessException as err:
+            self.logger.error(
+                "Failed to write logs to output, cannot continue.",
+                extra={"exception": err, **self.log_context},
+            )
+            return
 
         # Get ready for the next block of entries (if required).
         self._part += 1
+        self._saved += len(entries)
 
         # Save the new window geometry to cache but only AFTER data is saved, and only
         # save the window start when it's updated.
         if not incomplete_collection:
             self.save_window_start()
 
         self.save_window_end()
@@ -607,163 +562,110 @@
             entries.append(candidate)
 
         # Update known in-memory hashes to include our new entries.
         self.hashes = {**old_hashes, **new_hashes}
 
         return entries
 
-    def deduplicate_by_pointer(self, entries: List[Any]):
+    def deduplicate_by_pointer(self, candidates: List[Any]):
         """Deduplicate log entries by pointer values.
 
         Deduplicates records which occur before or after a pointer on the current
         page - depending on whether log entries are in chronological or reverse
         chronological order. This enables deduplication of log events within the same
         page of results, and is intended to solve for cases where a provider's filters
         are not as granular as the pointer value.
 
         For example, some provider's only allow filtering on a date (YYYY-MM-DD) while
         returning log entries with timestamps that have millisecond precision.
 
-        :param entries: A list of log entries to deduplicate.
+        :param candidates: A list of log entries to deduplicate.
 
         :return: A deduplicated list of log entries.
         """
         if self.LOG_ORDER == CHRONOLOGICAL:
-            return self._deduplicate_by_pointer_chronological(entries)
+            return self._deduplicate_by_pointer_chronological(candidates)
 
         if self.LOG_ORDER == REVERSE_CHRONOLOGICAL:
-            return self._deduplicate_by_pointer_reverse_chronological(entries)
+            return self._deduplicate_by_pointer_reverse_chronological(candidates)
 
-    def _deduplicate_by_pointer_chronological(self, entries: List[Any]):
+    def _deduplicate_by_pointer_chronological(self, candidates: List[Any]):
         """Deduplicates chronological log entries by their pointer.
 
-        :param entries: A list of log entries to deduplicate.
+        :param candidates: A list of log entries to deduplicate.
 
         :return: A deduplicated list of log entries.
         """
-        results = []
+        entries = []
         pointer_passed = False
 
-        for candidate in entries:
+        for candidate in candidates:
             candidate_pointer = str(jmespath.search(self.POINTER_PATH, candidate))
 
             if candidate_pointer == self.pointer:
                 pointer_passed = True
 
             # Only track chronological records on and after the pointer.
             if pointer_passed:
-                results.append(candidate)
+                entries.append(candidate)
 
         # If we never encountered the pointer, don't filter the records at all. This may
         # cause some duplicates if the pointer is on a subsequent page, but we always
         # prefer duplicates in these cases.
         if not pointer_passed:
-            results = entries
+            entries = candidates
 
-        return results
+        return entries
 
-    def _deduplicate_by_pointer_reverse_chronological(self, entries: List[Any]):
+    def _deduplicate_by_pointer_reverse_chronological(self, candidates: List[Any]):
         """Deduplicates reverse chronological log entries by their pointer.
 
-        :param entries: A list of log entries to deduplicate.
+        :param candidates: A list of log entries to deduplicate.
 
         :return: A deduplicated list of log entries.
         """
-        results = []
+        entries = []
         pointer_found = False
         pointer_passed = False
 
-        for candidate in entries:
+        for candidate in candidates:
             candidate_pointer = jmespath.search(self.POINTER_PATH, candidate)
 
             if candidate_pointer == self.pointer:
                 pointer_found = True
 
             if pointer_found and candidate_pointer != self.pointer:
                 pointer_passed = True
                 break
 
             if not pointer_passed:
-                results.append(candidate)
+                entries.append(candidate)
 
         # If we never encountered the pointer, don't filter the records at all. This may
         # cause some duplicates if the pointer is on a subsequent page, but we always
         # prefer duplicates in these cases.
         if not pointer_passed:
-            results = entries
-
-        return results
-
-    def process(self, entries: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
-        """Process log entries prior to saving.
-
-        :param entries: A list of log entries to process.
-
-        :return: A processed list of log entries.
-        """
-        # Shortcut where there are no processors configured.
-        if len(self._processors) < 1:
-            return []
-
-        # As processors can modify the number of entries, we need to loop over them
-        # multiple times.
-        processed = parsing.quick_copy(entries)
+            entries = candidates
 
-        for name, processor in self._processors.items():
-            for index, _ in enumerate(processed):
-                try:
-                    processed[index:index] = processor.process(processed.pop(index))
-                except Exception as err:
-                    raise ProcessorError(
-                        f"Processor '{name}' ({processor}) failed during "
-                        f" processing. {err}"
-                    )
-
-        return processed
-
-    def finalize(self):
-        """Performs final steps after each save operation has complete."""
-
-        # Finalize all processors.
-        for name, processor in self._processors.items():
-            # Once again this exception handler is exceptionally (!) broad, to ensure
-            # that any unhandled exception, including from downstream libraries, are
-            # caught and handled consistently (except for BaseException derived).
-            try:
-                processor.finalize()
-            except Exception as err:
-                # As this runs after saving data and pointers, all we can really do is
-                # log this and continue.
-                self.logger.error(
-                    "Processor failed during finalization.",
-                    extra={
-                        "identity": name,
-                        "processor": processor,
-                        "exception": err,
-                        **self.log_context,
-                    },
-                )
+        return entries
 
     @property
     def hashes(self) -> Dict[str, set[str]]:
         """Return hashes for the most recently seen log entries.
 
         :return: A dictionary of log entry hashes, keyed by their pointer.
         """
         default: Dict[str, set[str]] = {}
         if self._hashes:
             return self._hashes
 
         try:
             self._hashes[self.pointer] = set(
                 json.loads(
-                    self._cache.get(
-                        self.cache_key(CACHE_KEY_SEEN),
-                        self.operation,
-                    )
+                    self._cache.get(self.cache_key(CACHE_KEY_SEEN), self.operation)
                 )
             )
         except (TypeError, json.decoder.JSONDecodeError) as err:
             self.logger.warning(
                 "Deduplication hashes in the cache appear to be malformed, ignoring.",
                 extra={"exception": err, **self.log_context},
             )
@@ -1040,8 +942,7 @@
         except DataFormatException:
             raise ConcurrencyException(
                 "Could not delete lock, the lock no longer appears to be ours."
             )
 
         # Bye-bye lock.
         self._lock_expiry = None
-        self._lock_expiry = None
```

### Comparing `grove-1.0.0/grove/connectors/atlassian/api.py` & `grove-1.0.0rc1/grove/connectors/atlassian/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/connectors/atlassian/audit_events.py` & `grove-1.0.0rc1/grove/connectors/atlassian/audit_events.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/connectors/github/api.py` & `grove-1.0.0rc1/grove/connectors/github/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,16 @@
         """
         while True:
             try:
                 response = requests.get(url, headers=self.headers, params=params)
                 response.raise_for_status()
                 break
             except requests.exceptions.RequestException as err:
-                # 403s OR 429s are used with a header to indicate rate-limit exceeded.
-                if int(getattr(err.response, "status_code", 0)) not in [403, 429]:
+                # 403s are used with a header to indicate rate-limit exceeded.
+                if getattr(err.response, "status_code", None) != 403:
                     raise RequestFailedException(err)
 
                 if err.response.headers.get("X-RateLimit-Remaining") != "0":
                     raise RequestFailedException(err)
 
                 # Retry on rate-limit, but only if requested.
                 self.logger.warning("Rate-limit was exceeded during request")
```

### Comparing `grove-1.0.0/grove/connectors/github/audit_log.py` & `grove-1.0.0rc1/grove/connectors/github/audit_log.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,56 +18,24 @@
     LOG_ORDER = CHRONOLOGICAL
 
     # Double quoting is required so that jmespath understands that @timestamp is the
     # field to be extracted - due to the special character at the start ('@').
     POINTER_PATH = '"@timestamp"'
 
     @property
-    def delay(self):
-        """Defines the amount of time to delay collection of logs (in minutes).
-
-        This is used to allow time for logs to become 'consistent' before they are
-        collected. This is required as Github backfills log entries but unfortunately do
-        not provide any guidance around 'lag' time, or guarantees on availability and
-        delivery.
-
-        As a result of these constraints, this value is configurable to allow operators
-        to preference consistency over speed of delivery, and vice versa. For example,
-        a delay of 20 would instruct Grove to only collect logs after they are at least
-        20 minutes old.
-
-        This defaults to 0 (no delay).
-
-        :return: The "delay" component of the connector configuration.
-        """
-        try:
-            candidate = self.configuration.delay
-        except AttributeError:
-            return 0
-
-        try:
-            candidate = int(candidate)
-        except ValueError as err:
-            raise ConfigurationException(
-                f"Configured 'delay' is not valid. Value must be an integer. {err}"
-            )
-
-        return candidate
-
-    @property
     def scope(self):
         """Fetches the configured Github scope.
 
         This is used to control whether the connector should collect logs for a Github
         enterprise, or an organisation. This defaults to "orgs".
 
         :return: The "scope" component of the connector configuration.
         """
         try:
-            candidate = self.configuration.scope
+            candidate = self.configuration.scope  # type: ignore
         except AttributeError:
             return "orgs"
 
         # Check that this style of account is supported.
         SUPPORTED = ["enterprises", "orgs"]
 
         if candidate.lower() not in SUPPORTED:
@@ -80,15 +48,15 @@
     @property
     def fqdn(self):
         """Fetches the configured Github API FQDN, or the default (SaaS).
 
         :return: The "fqdn" component of the connector configuration.
         """
         try:
-            return self.configuration.fqdn
+            return self.configuration.fqdn  # type: ignore
         except AttributeError:
             return "api.github.com"
 
     def collect(self):
         """Collects all logs from the GitHub Audit API.
 
         This will first check whether there are any pointers cached to indicate previous
@@ -113,34 +81,22 @@
             # doesn't appear to support millisecond granularity in filters.
             self.pointer = str(
                 int((datetime.now(timezone.utc) - timedelta(days=7)).timestamp() * 1000)
             )
 
         # Transform the pointer into an ISO8601 compatible date and construct the search
         # phrase.
-        start = datetime.utcfromtimestamp(int(self.pointer) / 1000)
-        end = datetime.utcnow() - timedelta(minutes=self.delay)
+        start = datetime.utcfromtimestamp(int(self.pointer) / 1000).strftime(
+            DATESTAMP_FORMAT
+        )
 
         # Get log data from the upstream API, paging as required.
         while True:
-            if end <= start:
-                self.logger.debug(
-                    "Collection end time is prior to start, skipping.",
-                    extra={
-                        "start": start.strftime(DATESTAMP_FORMAT),
-                        "end": end.strftime(DATESTAMP_FORMAT),
-                    },
-                )
-                break
-
             log = client.get_audit_log(
-                phrase=(
-                    f"created:>={start.strftime(DATESTAMP_FORMAT)} "
-                    f"created:<={end.strftime(DATESTAMP_FORMAT)}"
-                ),
+                phrase=f"created:>={start}",
                 include=self.operation,
                 cursor=cursor,
             )
 
             # Save this batch of log entries.
             self.save(log.entries)
```

### Comparing `grove-1.0.0/grove/connectors/gsuite/activities.py` & `grove-1.0.0rc1/grove/connectors/gsuite/activities.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,75 +7,36 @@
 from datetime import datetime, timedelta
 
 import google_auth_httplib2
 import httplib2
 from google.auth.exceptions import GoogleAuthError
 from google.oauth2 import service_account
 from googleapiclient.discovery import build
-from googleapiclient.errors import Error as GACError
+from googleapiclient.errors import Error
 
 from grove.connectors import BaseConnector
 from grove.constants import REVERSE_CHRONOLOGICAL
 from grove.exceptions import (
     ConfigurationException,
     NotFoundException,
     RequestFailedException,
 )
 
 # This connector is only interested in the GSuite Reports API.
 SCOPES = ["https://www.googleapis.com/auth/admin.reports.audit.readonly"]
 
-
-def as_rfc3339(date: datetime) -> str:
-    """Formats an input date into RFC3339 format.
-
-    :param date: The input datetime object to convert to RFC3339 format.
-
-    :return: An RFC 3339 format date as a string.
-    """
-    return date.isoformat(sep="T", timespec="milliseconds") + "Z"
+# Use consistent flags when formatting via isoformat() on datetime objects.
+ISO_FORMAT_FLAGS = {"sep": "T", "timespec": "milliseconds"}
 
 
 class Connector(BaseConnector):
     NAME = "gsuite_activities"
     POINTER_PATH = "id.time"
     LOG_ORDER = REVERSE_CHRONOLOGICAL
 
-    @property
-    def delay(self):
-        """Defines the amount of time to delay collection of logs (in minutes).
-
-        This is used to allow time for logs to become 'consistent' before they are
-        collected. Google backfill log entries based on their published lag guidelines.
-        As a result of this, collection of events within this lag window may result in
-        missed events.
-
-        As a result of these constraints, this value is configurable to allow operators
-        to preference consistency over speed of delivery, and vice versa. For example,
-        a delay of 20 would instruct Grove to only collect logs after they are at least
-        20 minutes old.
-
-        This defaults to 0 (no delay).
-
-        :return: The "delay" component of the connector configuration.
-        """
-        try:
-            candidate = self.configuration.delay
-        except AttributeError:
-            return 0
-
-        try:
-            candidate = int(candidate)
-        except ValueError as err:
-            raise ConfigurationException(
-                f"Configured 'delay' is not valid. Value must be an integer. {err}"
-            )
-
-        return candidate
-
     def collect(self):
         """Collects activities from the Google GSuite Reports API.
 
         As the Google APIs use OAuth 2.0 2LO ('two-legged OAuth') which contains a
         number of fields inside of a JSON 'service account file' the key and identity
         are treated a little differently in this connector.
 
@@ -99,94 +60,74 @@
 
         # If no pointer is stored then a previous run hasn't been performed, so set the
         # pointer to a week ago. In the case of the GSuite reports API the pointer is
         # the value of the id.time field from the latest record retrieved from the API.
         try:
             _ = self.pointer
         except NotFoundException:
-            self.pointer = as_rfc3339(datetime.utcnow() - timedelta(days=7))
+            # Sorry about the + 'Z' here. It turns out, if you pass the API a startTime
+            # with a timezone in '+00:00' format, which is permitted according to API
+            # validation, filtering seems to break and just return you ALL data
+            # available. Cool.
+            self.pointer = (datetime.utcnow() - timedelta(days=7)).isoformat(
+                **ISO_FORMAT_FLAGS
+            ) + "Z"
 
         # Page over all activities since the last pointer.
         more_requests = True
 
         with build("admin", "reports_v1", http=http) as service:
             while more_requests:
-                # Transform the dates back to native to allow timedelta and comparison.
-                start = datetime.fromisoformat(self.pointer.replace("Z", ""))
-                end = datetime.utcnow() - timedelta(minutes=self.delay)
-
-                if end <= start:
-                    self.logger.debug(
-                        "Collection end time is prior to start, skipping.",
-                        extra={
-                            "start": as_rfc3339(start),
-                            "end": as_rfc3339(end),
-                            **self.log_context,
-                        },
-                    )
-                    break
-
+                self.logger.debug(
+                    "Requesting GSuite activity list.",
+                    extra={"operation": self.operation},
+                )
                 if cursor:
                     self.logger.debug(
-                        "Using pageToken as cursor to request next page of activities.",
-                        extra={"cursor": cursor, **self.log_context},
+                        "Using pageToken as cursor to request next page of results",
+                        extra={"cursor": cursor},
                     )
                     request = service.activities().list(
                         userKey="all",
                         applicationName=self.operation,
-                        startTime=as_rfc3339(start),
-                        endTime=as_rfc3339(end),
+                        startTime=self.pointer,
                         pageToken=cursor,
                     )
                 else:
                     self.logger.debug(
-                        "Using startTime from pointer to request activity list.",
-                        extra={
-                            "start": as_rfc3339(start),
-                            "end": as_rfc3339(end),
-                            **self.log_context,
-                        },
+                        "Using startTime from pointer", extra={"pointer": self.pointer}
                     )
                     request = service.activities().list(
                         userKey="all",
-                        startTime=as_rfc3339(start),
-                        endTime=as_rfc3339(end),
+                        startTime=self.pointer,
                         applicationName=self.operation,
                     )
 
                 # As both the _entries and activities objects are Lists, we can extend
                 # them in order to support appending more data on any subsequent
                 # iterations (due to paging).
                 try:
                     results = request.execute()
                     activities = results.get("items", [])
 
                     self.logger.debug(
-                        "Got activities from the GSuite API.",
-                        extra={
-                            "count": len(activities),
-                            **self.log_context,
-                        },
+                        "Got activities from the GSuite API",
+                        extra={"count": len(activities)},
                     )
                     self.save(activities)
-                except (GoogleAuthError, GACError) as err:
+                except (GoogleAuthError, Error) as err:
                     raise RequestFailedException(f"Request to GSuite API failed: {err}")
 
                 # Determine whether we're still paging.
                 if "nextPageToken" not in results:
-                    self.logger.debug(
-                        "No nextPageToken, finishing collection.",
-                        extra=self.log_context,
-                    )
+                    self.logger.debug("No nextPageToken, finishing collection.")
                     more_requests = False
                     break
 
-                self.logger.debug(
-                    "nextPageToken is present, paging.", extra=self.log_context
-                )
+                self.logger.debug("nextPageToken is present in response, paging.")
                 cursor = results["nextPageToken"]
                 more_requests = True
 
     def get_http_transport(self):
         """Creates an HTTP object for use by the Google API Client.
 
         :return: An httplib2.Http object for use with the Google API client.
```

### Comparing `grove-1.0.0/grove/connectors/gsuite/alerts.py` & `grove-1.0.0rc1/grove/connectors/gsuite/alerts.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/connectors/local/heartbeat.py` & `grove-1.0.0rc1/grove/connectors/local/heartbeat.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,26 +21,26 @@
     @property
     def count(self):
         """Fetches the count of heartbeat messages to emit from the configuration.
 
         :return: The number of heartbeat messages to emit.
         """
         try:
-            return int(self.configuration.count)
+            return int(self.configuration.count)  # type: ignore
         except (AttributeError, ValueError):
             return 5
 
     @property
     def interval(self):
         """Fetches the interval to emit a heartbeat message from the configuration.
 
         :return: The heartbeat interval, in seconds.
         """
         try:
-            return int(self.configuration.interval)
+            return int(self.configuration.interval)  # type: ignore
         except (AttributeError, ValueError):
             return 1
 
     def collect(self):
         """Generates test log entries at the configured interval."""
         try:
             _ = self.pointer
```

### Comparing `grove-1.0.0/grove/connectors/okta/api.py` & `grove-1.0.0rc1/grove/connectors/okta/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/connectors/okta/system_log.py` & `grove-1.0.0rc1/grove/connectors/okta/system_log.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         This field is used to allow configuration of collection of log data from
         specific Okta domains, including okta-emea.com, and oktapreview.com. This must
         not include the customer name / organisation name.  The default is 'okta.com'.
 
         :return: The "domain" portion of the connector's configuration.
         """
         try:
-            return self.configuration.domain
+            return self.configuration.domain  # type: ignore
         except AttributeError:
             return "okta.com"
 
     def collect(self):
         """Collects all logs from the Okta Audit API.
 
         This will first check whether there are any pointers cached to indicate previous
```

### Comparing `grove-1.0.0/grove/connectors/onepassword/api.py` & `grove-1.0.0rc1/grove/connectors/onepassword/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,23 +145,7 @@
         :param start_time: The ISO Format timestamp to query logs since.
 
         :return: AuditLogEntries object containing a pagination cursor, and log entries.
         """
         return self.get_events(
             event_type="itemusages", cursor=cursor, start_time=start_time
         )
-
-    def get_auditevents(
-        self,
-        cursor: Optional[str] = None,
-        start_time: Optional[str] = None,
-    ) -> AuditLogEntries:
-        """Fetches a list of actions performed by members of a 1Password account.
-
-        :param cursor: Cursor to use when fetching results. Supersedes other parameters.
-        :param start_time: The ISO Format timestamp to query logs since.
-
-        :return: AuditLogEntries object containing a pagination cursor, and log entries.
-        """
-        return self.get_events(
-            event_type="auditevents", cursor=cursor, start_time=start_time
-        )
```

### Comparing `grove-1.0.0/grove/connectors/onepassword/events_audit.py` & `grove-1.0.0rc1/grove/connectors/onepassword/events_signinattempts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
-"""1Password Audit event log connector for Grove."""
+"""1Password Signin Attempt event log connector for Grove."""
 
 import datetime
 
-from grove.connectors import BaseConnector
 from grove.connectors.onepassword.api import Client
+from grove.connectors import BaseConnector
 from grove.constants import CHRONOLOGICAL
 from grove.exceptions import NotFoundException
 
 
 class Connector(BaseConnector):
-    NAME = "onepassword_events_audit"
+    NAME = "onepassword_events_signinattempts"
     POINTER_PATH = "timestamp"
     LOG_ORDER = CHRONOLOGICAL
 
     def collect(self):
-        """Collects all logs from the 1Password audit event log API.
+        """Collects all logs from the 1Password signin event log API.
 
         This will first check whether there are any pointers cached to indicate previous
         collections. If not, the last week of data will be collected.
         """
         client = Client(token=self.key)
         cursor = None
 
@@ -32,15 +32,15 @@
             _ = self.pointer
         except NotFoundException:
             week_ago = datetime.datetime.now() - datetime.timedelta(days=7)
             self.pointer = (week_ago).astimezone().replace(microsecond=0).isoformat()
 
         # Get log data from the upstream API, paging as required.
         while True:
-            log = client.get_auditevents(start_time=self.pointer, cursor=cursor)
+            log = client.get_signinattempts(start_time=self.pointer, cursor=cursor)
 
             # Save this batch of log entries.
             self.save(log.entries)
 
             # Check if we need to continue paging.
             cursor = log.cursor
             if cursor is None:
```

### Comparing `grove-1.0.0/grove/connectors/onepassword/events_itemusages.py` & `grove-1.0.0rc1/grove/connectors/onepassword/events_itemusages.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/connectors/onepassword/events_signinattempts.py` & `grove-1.0.0rc1/grove/connectors/tfc/audit_trails.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
-"""1Password Signin Attempt event log connector for Grove."""
+"""Terraform Cloud audit trails connector for Grove."""
 
-import datetime
+from datetime import datetime, timedelta
 
-from grove.connectors.onepassword.api import Client
 from grove.connectors import BaseConnector
-from grove.constants import CHRONOLOGICAL
+from grove.connectors.tfc.api import Client
+from grove.constants import REVERSE_CHRONOLOGICAL
 from grove.exceptions import NotFoundException
 
 
 class Connector(BaseConnector):
-    NAME = "onepassword_events_signinattempts"
+    NAME = "tfc_audit_trails"
     POINTER_PATH = "timestamp"
-    LOG_ORDER = CHRONOLOGICAL
+    LOG_ORDER = REVERSE_CHRONOLOGICAL
 
     def collect(self):
-        """Collects all logs from the 1Password signin event log API.
+        """Collects TFC audit trail from the TFC audit-trails API.
+
+        https://www.terraform.io/docs/cloud/api/audit-trails.html
 
         This will first check whether there are any pointers cached to indicate previous
         collections. If not, the last week of data will be collected.
         """
         client = Client(token=self.key)
-        cursor = None
+        cursor = 1
 
         # If no pointer is stored then a previous run hasn't been performed, so set the
-        # pointer to a week ago. In the case of the 1Password API this is an ISO
-        # timestamp in a field called "timestamp".
+        # pointer to a week ago. In the case of the TFC audit API the pointer is the
+        # value of the "timestamp" field from the latest record retrieved from the
+        # API - which is in ISO8601 Format.
         try:
             _ = self.pointer
         except NotFoundException:
-            week_ago = datetime.datetime.now() - datetime.timedelta(days=7)
-            self.pointer = (week_ago).astimezone().replace(microsecond=0).isoformat()
+            self.pointer = (datetime.utcnow() - timedelta(days=7)).isoformat()
 
-        # Get log data from the upstream API, paging as required.
+        # Get log data from the upstream API.
         while True:
-            log = client.get_signinattempts(start_time=self.pointer, cursor=cursor)
+            log = client.get_trails(since=self.pointer, cursor=cursor)
 
             # Save this batch of log entries.
             self.save(log.entries)
 
             # Check if we need to continue paging.
-            cursor = log.cursor
-            if cursor is None:
+            cursor = log.cursor  # type: ignore
+            if not cursor:
                 break
```

### Comparing `grove-1.0.0/grove/connectors/oomnitza/activities.py` & `grove-1.0.0rc1/grove/connectors/slack/audit_logs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,47 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
-"""Oomnitza Activities connector for Grove."""
-import time
+"""Slack Audit connector for Grove."""
+
 from datetime import datetime, timedelta
 
 from grove.connectors import BaseConnector
-from grove.connectors.oomnitza.api import Client
+from grove.connectors.slack.api import Client
 from grove.constants import REVERSE_CHRONOLOGICAL
 from grove.exceptions import NotFoundException
 
 
 class Connector(BaseConnector):
-    NAME = "oomnitza_activities"
-    POINTER_PATH = "timestamp"
+    NAME = "slack_audit_logs"
+    POINTER_PATH = "date_create"
     LOG_ORDER = REVERSE_CHRONOLOGICAL
 
     def collect(self):
-        """Collects Oomnitza activities from the Oomnitza API.
+        """Collects all logs from the Slack Audit API.
 
         This will first check whether there are any pointers cached to indicate previous
         collections. If not, the last week of data will be collected.
         """
-        client = Client(token=self.key, identity=self.identity)
-
-        # Set cursor
-        cursor = 0
+        client = Client(token=self.key)
+        cursor = None
 
         # If no pointer is stored then a previous run hasn't been performed, so set the
-        # pointer to 2 days ago. In the case of the Oomnitza activities API the pointer
-        # is the value of the "timestamp" field from the latest record retrieved from
-        # the API - which is in epoch. The Oomnitza API doesnt account for milliseconds.
-        now = datetime.fromtimestamp(time.time()).strftime("%s")
-
+        # pointer to a week ago. In the case of the Slack audit API the pointer is the
+        # value of the "date_create" field from the latest record retrieved from the
+        # API - which is in seconds since epoch ("Unix Time") format.
         try:
             _ = self.pointer
         except NotFoundException:
-            self.pointer = (
-                datetime.fromtimestamp(time.time()) - timedelta(days=2)
-            ).strftime("%s")
+            self.pointer = (datetime.utcnow() - timedelta(days=7)).strftime("%s")
 
-        # Get log data from the upstream API. A "start_date" and "end_date" datetime
-        # query parameters are required.
+        # Page over data using the cursor, saving returned data page by page.
         while True:
-            log = client.get_activites(
-                start_date=self.pointer, end_date=now, cursor=cursor
-            )
+            log = client.get_logs(oldest=self.pointer, cursor=cursor)
 
             # Save this batch of log entries.
             self.save(log.entries)
 
             # Check if we need to continue paging.
-            cursor = log.cursor  # type: ignore
-            if not cursor:
+            cursor = log.cursor
+            if cursor is None:
                 break
```

### Comparing `grove-1.0.0/grove/connectors/oomnitza/api.py` & `grove-1.0.0rc1/grove/connectors/tfc/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,103 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
-"""Oomnitza API client."""
+"""Terraform Cloud audit trail API client.
+
+The official TFC SDK does not currently support the Audit API, so interactions need
+to be handled manually.
+"""
 
 import logging
+import time
 from typing import Dict, Optional
 
 import requests
 
-from grove.exceptions import RequestFailedException
+from grove.exceptions import RateLimitException, RequestFailedException
 from grove.types import AuditLogEntries, HTTPResponse
 
-API_BASE_URI = "https://{identity}.oomnitza.com"
-API_PAGE_SIZE = 200
+API_BASE_URI = "https://app.terraform.io/api/v2"
 
 
 class Client:
     def __init__(
         self,
-        identity: Optional[str] = None,
         token: Optional[str] = None,
-    ):
+        retry: Optional[bool] = True,
+    ) -> None:
         """Setup a new client.
 
-        :param identity: The name of the Oomnitza organisation.
-        :param token: The Oomnitza API token.
+        :param token: The TFC API Bearer token.
+        :param retry: Whether to automatically retry if recoverable errors are
+            encountered, such as rate-limiting.
         """
+        self.retry = retry
         self.logger = logging.getLogger(__name__)
         self.headers = {
-            "content-type": "application/json",
+            "Accept": "application/json",
+            "Authorization": f"Bearer {token}",
         }
-        if token:
-            self.headers["Authorization2"] = token
-
-        # We need to push the identity into the URI, so we'll keep track of this.
-        self._api_base_uri = API_BASE_URI.format(identity=identity)
 
     def _get(
         self,
         url: str,
         params: Optional[Dict[str, Optional[str]]] = None,
     ) -> HTTPResponse:
         """A GET wrapper to handle retries for the caller.
 
         :param url: URL to perform the HTTP GET against.
         :param params: HTTP parameters to add to the request.
 
+        :raises RateLimitException: A rate limit was encountered.
         :raises RequestFailedException: An HTTP request failed.
 
         :return: HTTP Response object containing the headers and body of a response.
         """
-        try:
-            response = requests.get(url, headers=self.headers, params=params)
-            response.raise_for_status()
-        except requests.exceptions.RequestException as err:
-            raise RequestFailedException(err)
+        while True:
+            try:
+                response = requests.get(url, headers=self.headers, params=params)
+                response.raise_for_status()
+                break
+            except requests.exceptions.RequestException as err:
+                # Retry on rate-limit, but only if requested.
+                if getattr(err.response, "status_code", None) == 429:
+                    self.logger.warning("Rate-limit was exceeded during request")
+                    if self.retry:
+                        time.sleep(1)
+                        continue
+                    else:
+                        raise RateLimitException(err)
+
+                raise RequestFailedException(err)
 
         return HTTPResponse(headers=response.headers, body=response.json())
 
-    def get_activites(
+    def get_trails(
         self,
-        cursor: int = 0,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        since: Optional[str] = None,
+        cursor: Optional[int] = 1,
+        page_size: Optional[str] = None,
     ) -> AuditLogEntries:
-        """Fetches a list of signing attempt logs.
+        """Fetches a list of audit logs which match the provided filters.
 
-        :param cursor: Cursor to use when fetching results.
-        :param start_date: The earliest date an event represented as an epoch value.
-        :param end_date: The latest date an event represented as an epoch value.
+        :param since: The ISO8601 format of the most recent event to include (inclusive).
+        :param cursor: The page to fetch. If omitted, endpoint returns first page.
+        :param page_size: Number of audit events per page. Defaults to 1000.
 
-        :return: AuditLogEntries object containing a pagination cursor, and log entries.
+        :return: AuditLogEntries object containing a pagination cursor, and log
+            entries.
         """
-        url = f"{self._api_base_uri}/api/v3/activities"
-
+        # See psf/requests issue #2651 for why we can happily pass in None values
+        # and not have the request key added to the URI.
         result = self._get(
-            url,
+            f"{API_BASE_URI}/organization/audit-trail",
             params={
-                "start_date": start_date,
-                "end_date": end_date,
-                "limit": str(API_PAGE_SIZE),
-                "skip": str(cursor),
+                "since": since,
+                "page[number]": str(cursor),
+                "page[size]": page_size,
             },
         )
-        # Keep paging until we run out of results.
-        data = result.body
-
-        if len(data) == API_PAGE_SIZE:
-            cursor += API_PAGE_SIZE
-        else:
-            cursor = 0
+        cursor = result.body.get("pagination", {}).get("next_page", 0)
 
         # Return the cursor and the results to allow the caller to page as required.
-        return AuditLogEntries(cursor=cursor, entries=data)  # type: ignore
+        return AuditLogEntries(cursor=cursor, entries=result.body.get("data", []))
```

### Comparing `grove-1.0.0/grove/connectors/pagerduty/api.py` & `grove-1.0.0rc1/grove/connectors/pagerduty/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/connectors/pagerduty/audit_records.py` & `grove-1.0.0rc1/grove/connectors/pagerduty/audit_records.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/connectors/sf/event_log.py` & `grove-1.0.0rc1/grove/connectors/sf/event_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         """Fetches the SalesForce token from the configuration.
 
         This is required as this is a third authentication element required by SF.
 
         :return: The "token" portion of the connector's configuration.
         """
         try:
-            return self.configuration.token
+            return self.configuration.token  # type: ignore
         except AttributeError:
             return None
 
     def collect(self):  # noqa: C901
         """Collects EventLogs from the SF Cloud API.
 
         This will first check whether there are any pointers cached to indicate previous
```

### Comparing `grove-1.0.0/grove/connectors/sfmc/api.py` & `grove-1.0.0rc1/grove/connectors/sfmc/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/connectors/sfmc/audit_events.py` & `grove-1.0.0rc1/grove/connectors/sfmc/audit_events.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/connectors/sfmc/security_events.py` & `grove-1.0.0rc1/grove/connectors/sfmc/security_events.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/connectors/slack/api.py` & `grove-1.0.0rc1/grove/connectors/slack/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/connectors/slack/audit_logs.py` & `grove-1.0.0rc1/grove/connectors/torq/audit_logs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
-"""Slack Audit connector for Grove."""
+"""Torq audit log connector for Grove."""
 
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 
 from grove.connectors import BaseConnector
-from grove.connectors.slack.api import Client
+from grove.connectors.torq.api import Client
 from grove.constants import REVERSE_CHRONOLOGICAL
 from grove.exceptions import NotFoundException
 
 
 class Connector(BaseConnector):
-    NAME = "slack_audit_logs"
-    POINTER_PATH = "date_create"
+    NAME = "torq_audit_logs"
+    POINTER_PATH = "timestamp"
     LOG_ORDER = REVERSE_CHRONOLOGICAL
 
     def collect(self):
-        """Collects all logs from the Slack Audit API.
+        """Collects all audit logs from the Torq API.
 
         This will first check whether there are any pointers cached to indicate previous
-        collections. If not, the last week of data will be collected.
+        collections. If not, a 7 day look-back of data will be collected.
         """
-        client = Client(token=self.key)
+        client = Client(identity=self.identity, key=self.key)
         cursor = None
 
         # If no pointer is stored then a previous run hasn't been performed, so set the
-        # pointer to a week ago. In the case of the Slack audit API the pointer is the
-        # value of the "date_create" field from the latest record retrieved from the
-        # API - which is in seconds since epoch ("Unix Time") format.
+        # pointer to 7-days ago.
         try:
             _ = self.pointer
         except NotFoundException:
-            self.pointer = (datetime.utcnow() - timedelta(days=7)).strftime("%s")
+            self.pointer = (datetime.now(timezone.utc) - timedelta(days=7)).isoformat()
 
-        # Page over data using the cursor, saving returned data page by page.
         while True:
-            log = client.get_logs(oldest=self.pointer, cursor=cursor)
+            log = client.get_audit_logs(start_time=self.pointer, cursor=cursor)
 
             # Save this batch of log entries.
             self.save(log.entries)
 
             # Check if we need to continue paging.
             cursor = log.cursor
             if cursor is None:
```

### Comparing `grove-1.0.0/grove/connectors/torq/activity_logs.py` & `grove-1.0.0rc1/grove/connectors/torq/activity_logs.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/connectors/torq/api.py` & `grove-1.0.0rc1/grove/connectors/torq/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,16 +140,16 @@
         result_field: str,
         start_time: Optional[str] = None,
         limit: Optional[int] = API_PAGE_SIZE,
         cursor: Optional[str] = None,
     ) -> AuditLogEntries:
         """Fetches a list of logs from Torq which match the provided filters.
 
-        :param start_time: The required date and time of the earliest log entry. Start
-            times are in RFC3339 format, for example, 2022-03-09T08:40:18.490771179Z.
+        :param start_time: The required date and time of the earliest log entry.
+            Timestamps are in RFC 3339 format, for example, 2022-03-09T08:40:18.490771179Z.
         :param result_field: The key name for the list of logs in the returned json.
         :param to_date: The required date and time in UTC of the latest log entry.
         :param limit: The maximum number of items to include in a single response.
         :param cursor: The cursor to use when paging.
 
         :return: AuditLogEntries object containing a pagination cursor, and log entries.
         """
@@ -174,16 +174,16 @@
         return AuditLogEntries(cursor=cursor, entries=data)
 
     def get_audit_logs(
         self, start_time: Optional[str] = None, cursor: Optional[str] = None
     ) -> AuditLogEntries:
         """Fetches a list of audit logs from Torq which match the provided filters.
 
-        :param start_time: The required date and time of the earliest log entry. Start
-            times are in RFC 3339 format, for example, 2022-03-09T08:40:18.490771179Z.
+        :param start_time: The required date and time of the earliest log entry.
+            Timestamps are in RFC 3339 format, for example, 2022-03-09T08:40:18.490771179Z.
         :param to_date: The required date and time in UTC of the latest log entry.
         :param cursor: The cursor to use when paging.
 
         :return: AuditLogEntries object containing a pagination cursor, and log entries.
         """
         return self.get_logs(
             endpoint="v1alpha/audit_logs",
@@ -193,16 +193,16 @@
         )
 
     def get_activity_logs(
         self, start_time: Optional[str] = None, cursor: Optional[str] = None
     ) -> AuditLogEntries:
         """Fetches a list of activity logs from Torq which match the provided filters.
 
-        :param start_time: The required date and time of the earliest log entry. Start
-            times are in RFC 3339 format, for example, 2022-03-09T08:40:18.490771179Z.
+        :param start_time: The required date and time of the earliest log entry.
+            Timestamps are in RFC 3339 format, for example, 2022-03-09T08:40:18.490771179Z.
         :param to_date: The required date and time in UTC of the latest log entry.
         :param cursor: The cursor to use when paging.
 
         :return: AuditLogEntries object containing a pagination cursor, and log entries.
         """
         return self.get_logs(
             endpoint="v1alpha/activity_logs",
```

### Comparing `grove-1.0.0/grove/connectors/twilio/messages.py` & `grove-1.0.0rc1/grove/connectors/twilio/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
         This is required as this is a third authentication element required by Twilio
         when using API authentication.
 
         :return: The value of the 'secret' field from the configuration.
         """
         try:
-            return self.configuration.secret
+            return self.configuration.secret  # type: ignore
         except AttributeError:
             return None
 
     @lru_cache(maxsize=512)  # noqa: B019
     def _carrier_lookup(self, number: str):
         """Performs a Carrier lookup via the Twilio API.
```

### Comparing `grove-1.0.0/grove/connectors/twilio/monitor_events.py` & `grove-1.0.0rc1/grove/connectors/twilio/monitor_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         This is required as this is a third authentication element required by Twilio
         when using API authentication.
 
         :return: The value of the 'secret' field from the configuration.
         """
         try:
-            return self.configuration.secret
+            return self.configuration.secret  # type: ignore
         except AttributeError:
             return None
 
     def collect(self):
         """Collects all events from the Twilio Monitor Event API.
 
         This will first check whether there are any pointers cached to indicate previous
```

### Comparing `grove-1.0.0/grove/connectors/workday/activity_logging.py` & `grove-1.0.0rc1/grove/connectors/workday/activity_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,41 +24,41 @@
 
         This is required as this is the url required by WD for authentication and API
         usage.
 
         :return: The "base_url" portion of the connector's configuration.
         """
         try:
-            return self.configuration.base_url
+            return self.configuration.base_url  # type: ignore
         except AttributeError:
             return None
 
     @property
     def client_id(self):
         """Fetches the Workday Client ID from the configuration.
 
         This is required as this is an additional authentication element required by WD.
 
         :return: The "client_id" portion of the connector's configuration.
         """
         try:
-            return self.configuration.client_id
+            return self.configuration.client_id  # type: ignore
         except AttributeError:
             return None
 
     @property
     def client_secret(self):
         """Fetches the Workday Client Secret from the configuration.
 
         This is required as this is an additional authentication element required by WD.
 
         :return: The "client_secret" portion of the connector's configuration.
         """
         try:
-            return self.configuration.client_secret
+            return self.configuration.client_secret  # type: ignore
         except AttributeError:
             return None
 
     def collect(self):
         """Collects all logs from the Workday Audit API.
 
         This will first check whether there are any pointers cached to indicate previous
@@ -88,17 +88,15 @@
                 DATESTAMP_FORMAT
             )
 
         # Get log data from the upstream API. A "from" and "to" datetime query
         # parameters are required.
         while True:
             log = client.get_activity_logging(
-                from_date=self.pointer,
-                to_date=now,
-                cursor=cursor,
+                from_date=self.pointer, to_date=now, cursor=cursor
             )
 
             # Save this batch of log entries.
             self.save(log.entries)
 
             # Check if we need to continue paging.
             cursor = log.cursor  # type: ignore
```

### Comparing `grove-1.0.0/grove/connectors/workday/api.py` & `grove-1.0.0rc1/grove/connectors/workday/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/connectors/zoom/activities.py` & `grove-1.0.0rc1/grove/connectors/zoom/activities.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     @property
     def client_id(self):
         """Fetches the Zoom ClientID from the configuration.
 
         This is required as this is a third authentication element required by Zoom.
         """
         try:
-            return self.configuration.client_id
+            return self.configuration.client_id  # type: ignore
         except AttributeError:
             return None
 
     def collect(self):
         """Collects all logs from the Zoom Activity API."""
         client = api.Client(
             identity=self.identity,
```

### Comparing `grove-1.0.0/grove/connectors/zoom/api.py` & `grove-1.0.0rc1/grove/connectors/zoom/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
 """Zoom API client.
 
-As the Python Zoom client does not currently support Audit API, this client has been
-created in the interim.
+As the Python Zoom client does not currently support Audit API, this client has been created in
+the interim.
 """
 
 import base64
 import logging
 import time
 from typing import Any, Dict, Optional
 
@@ -147,17 +147,17 @@
         :param from_date: The required date of the earliest log entry.
         :param to_date: The required date of the latest log entry.
         :param limit: The maximum number of items to include in a single response.
         :param cursor: The 'next_page_token' returned from a request.
 
         :return: AuditLogEntries object containing a pagination cursor, and log entries.
         """
-        # The endpoint returns the same total value of results regardless of the limit
-        # and offset parameters. The pagination parameters determine the amount of
-        # content in the data[] array.
+        # The endpoint returns the same total value of results regardless of the limit and
+        # offset parameters. The pagination parameters determine the amount of content
+        # in the data[] array.
 
         result = self._get(
             f"{API_BASE_URI}/{endpoint}",
             params={
                 "from": from_date,
                 "to": to_date,
                 "next_page_token": cursor,
```

### Comparing `grove-1.0.0/grove/connectors/zoom/operationlogs.py` & `grove-1.0.0rc1/grove/connectors/zoom/operationlogs.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     @property
     def client_id(self):
         """Fetches the Zoom ClientID from the configuration.
 
         This is required as this is a third authentication element required by Zoom.
         """
         try:
-            return self.configuration.client_id
+            return self.configuration.client_id  # type: ignore
         except AttributeError:
             return None
 
     def collect(self):
         """Collects all logs from the Zoom Activity API."""
         client = api.Client(
             identity=self.identity,
```

### Comparing `grove-1.0.0/grove/constants.py` & `grove-1.0.0rc1/grove/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 ENV_GROVE_WORKER_COUNT = "GROVE_WORKER_COUNT"
 ENV_GROVE_LOCK_DURATION = "GROVE_LOCK_DURATION"
 
 # Plugin groups (setuptools entrypoints).
 PLUGIN_GROUP_CACHE = "grove.caches"
 PLUGIN_GROUP_OUTPUT = "grove.outputs"
 PLUGIN_GROUP_CONFIG = "grove.configs"
-PLUGIN_GROUP_PROCESSOR = "grove.processors"
 PLUGIN_GROUP_SECRET = "grove.secrets"  # noqa: S105
 PLUGIN_GROUP_CONNECTOR = "grove.connectors"
 
 # Define defines for unset environment variables.
 DEFAULT_CACHE_HANDLER = "local_memory"
 DEFAULT_OUTPUT_HANDLER = "local_stdout"
 DEFAULT_CONFIG_HANDLER = "local_file"
```

### Comparing `grove-1.0.0/grove/entrypoints/aws_lambda.py` & `grove-1.0.0rc1/grove/entrypoints/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/entrypoints/base.py` & `grove-1.0.0rc1/grove/entrypoints/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
 """Provides functions used between entrypoints."""
 
 import os
-import sys
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from typing import Any, Dict, List
 
 from aws_lambda_powertools import Logger
 
 from grove.constants import (
     DEFAULT_CONFIG_HANDLER,
@@ -74,35 +73,31 @@
 
     This function should be called from various wrappers in order to execute Grove when
     running under the respective runtime. This is in order to enable use in serverless,
     containerised, virtualised, and "bare metal" environments.
 
     :param context: Contextual information relating to the current runtime.
     """
-    logger = Logger(
-        "grove",
-        logger_formatter=GroveFormatter(context),
-        stream=sys.stderr,
-    )
+    logger = Logger("grove", logger_formatter=GroveFormatter(context))
     logger.info("Grove started")
 
     # Attempt to load connector configuration, failure to do so is not recoverable.
     try:
         configurations = configure()
     except GroveException as err:
-        logger.critical(
+        logger.fatal(
             "Failed to initialise configuration handler", extra={"exception": err}
         )
         return
 
     # Allow users to optionally configure the number of worker threads.
     try:
         workers = int(os.environ.get(ENV_GROVE_WORKER_COUNT, DEFAULT_WORKER_COUNT))
     except ValueError as err:
-        logger.critical(
+        logger.fatal(
             f"Worker count ('{ENV_GROVE_WORKER_COUNT}') must be a number.",
             extra={"exception": err},
         )
         return
 
     # All connectors will be executed in their own thread, up to the maximum configured
     # workers specified by the worker count.
```

### Comparing `grove-1.0.0/grove/entrypoints/local_process.py` & `grove-1.0.0rc1/grove/entrypoints/local_process.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/exceptions.py` & `grove-1.0.0rc1/grove/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class ConnectorMissingException(GroveException):
     """Indicates that a requested connector was not found."""
 
 
 class ConcurrencyException(GroveException):
-    """Indicates that Grove may be running in another location concurrently."""
+    """Indidates that Grove may be running in another location concurrently."""
 
 
 class NotImplementedException(GroveException):
     """Indicates that the requested functionality has not been implemented."""
 
 
 class NotFoundException(GroveException):
@@ -38,11 +38,7 @@
 
 class AccessException(GroveException):
     """Indicates an issue occurred while attempting to access the requested resource."""
 
 
 class DataFormatException(GroveException):
     """Indicates an issue occurred while attempting to process data."""
-
-
-class ProcessorError(GroveException):
-    """Indicates that an error occurred when setting up or calling a processor."""
```

### Comparing `grove-1.0.0/grove/helpers/plugin.py` & `grove-1.0.0rc1/grove/helpers/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,20 +31,19 @@
             return candidate
 
     raise ConfigurationException(
         f"Requested handler could not be found with name '{name}' (group '{group}')"
     )
 
 
-def load_handler(name: str, group: str, *args: Any, **kwargs: Any) -> Any:
+def load_handler(name: str, group: str) -> Any:
     """Attempts to locate and load the requested plugin handler.
 
     This is a convenience method which wrappers the lookup operation, and performs the
-    load and instantiation required to hydrate a 'real' handler. Any additional
-    arguments passed to load_handler are pass through to the handler during creation.
+    load and instantiation required to hydrate a 'real' handler.
 
     :param name: The name of the handler to load (e.g. 'aws_ssm').
     :param group: The group the handler belongs to (e.g. 'grove.outputs').
     """
     cls = lookup_handler(name, group).load()
 
-    return cls(*args, **kwargs)
+    return cls()
```

### Comparing `grove-1.0.0/grove/logging.py` & `grove-1.0.0rc1/grove/logging.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/models.py` & `grove-1.0.0rc1/grove/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
 """Data models used throughout Grove."""
 
 import base64
 import binascii
-from enum import Enum
-from typing import Dict, List
+from typing import Dict
 
 from pydantic import BaseModel, Extra, Field, root_validator, validator
 
 from grove.constants import OPERATION_DEFAULT
 from grove.exceptions import DataFormatException
 
 
@@ -33,44 +32,16 @@
     except binascii.Error as err:
         raise DataFormatException(f"Unable to base64 decode data, {err}")
 
     # More formats may be supported later.
     raise DataFormatException(f"Unknown encoding method '{encoding}'")
 
 
-class ProcessorConfig(BaseModel, extra=Extra.allow):
-    """A processor configuration object.
-
-    A processor configuration object represents information used by processors to
-    perform some set of operations on log entries. This base configuration object
-    is bare-bones as processors may define their own required configuration fields.
-    """
-
-    # Name is an arbitrary name administrators can provide to processors to enable
-    # better tracking and identification of processors.
-    name: str
-
-    # Processor defines the processor which should be run. This must match the plugin
-    # entrypoint name.
-    processor: str
-
-
-class OutputStream(str, Enum):
-    """Defines supported output 'streams'.
-
-    This is used to allow routing of original / raw collected data differently to
-    post processed data.
-    """
-
-    raw = "raw"
-    processed = "processed"
-
-
 class ConnectorConfig(BaseModel, extra=Extra.allow):
-    """Defines the connector configuration structure.
+    """A connector configuration object.
 
     A configuration object represents information which Grove uses to call a given
     connector. All connectors must have at least a name, key, identity, and connector
     defined.
 
     Connector configuration objects support the addition of arbitrary fields to enable
     service specific authentication and configuration concerns to be defined. This is
@@ -98,27 +69,14 @@
     # binary data or nested JSON.
     encoding: Dict[str, str] = Field({})
 
     # Operations allow connectors and users to filter which 'type' of events to collect
     # from API endpoints which allow filtering records to return.
     operation: str = Field(OPERATION_DEFAULT)
 
-    # Processors allow processing of data during collection.
-    processors: List[ProcessorConfig] = Field([])
-
-    # Outputs allows specification of what type of data to output, and with what
-    # descriptor. By default, any processed logs will be output with a descriptor of
-    # 'processed', and raw logs with a descriptor of 'logs'.
-    outputs: Dict[str, OutputStream] = Field(
-        {
-            "logs": OutputStream.raw,
-            "processed": OutputStream.processed,
-        }
-    )
-
     @validator("key")
     def _validate_key_or_secret(cls, value, values, field):  # noqa: B902
         """Ensures that 'key' is set directly or a reference is present in 'secrets'.
 
         This is used to ensure that a key is always set, whether directly, or will be
         fetched from the configured secrets backend at runtime (as indicated by an entry
         in the secrets field).
```

### Comparing `grove-1.0.0/grove/outputs/aws_s3.py` & `grove-1.0.0rc1/grove/outputs/aws_s3.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,112 +1,92 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
 """Grove AWS S3 output handler."""
 
 import datetime
+import logging
 import os
 from typing import Optional
 
 from boto3.session import Session
 from botocore.exceptions import BotoCoreError, ClientError
-from pydantic import Field
+from pydantic import BaseSettings, Field, ValidationError
 
 from grove.constants import DATESTAMP_FORMAT
-from grove.exceptions import AccessException
+from grove.exceptions import AccessException, ConfigurationException
+from grove.helpers import parsing
 from grove.outputs import BaseOutput
 
 OBJECT_KEY = (
-    "{descriptor}{connector}/{identity}/{year}/{month}/{day}/"
-    "{operation}-{datestamp}.{part}{kind}"
+    "logs/{connector}/{identity}/{year}/{month}/{day}/"
+    "{operation}-{datestamp}.{part}.json.gz"
 )
 
 
-class Handler(BaseOutput):
-    """This output handler allows Grove to write collected logs to an AWS S3 bucket."""
-
-    class Configuration(BaseOutput.Configuration):
-        """Defines environment variables used to configure the AWS S3 handler.
+class Configuration(BaseSettings):
+    """Defines environment variables used to configure the AWS S3 handler.
 
-        This should also include any appropriate default values for fields which are not
-        required.
+    This should also include any appropriate default values for fields which are not
+    required.
+    """
+
+    bucket: str = Field(
+        description="The name of the S3 bucket to output logs to.",
+    )
+    assume_role_arn: Optional[str] = Field(
+        description="An optional AWS role to assume when authenticating with AWS."
+    )
+    bucket_region: Optional[str] = Field(
+        description="The region that S3 the bucket exists in (default us-east-1)",
+        default=os.environ.get("AWS_REGION", "us-east-1"),
+    )
+
+    class Config:
+        """Allow environment variable override of configuration fields.
+
+        This also enforce a prefix for all environment variables for this handler. As
+        an example the field `bucket` would be set using the environment variable
+        `GROVE_OUTPUT_AWS_S3_BUCKET`.
         """
 
-        bucket: str = Field(
-            description="The name of the S3 bucket to output logs to.",
-        )
-        aws_access_key_id: Optional[str] = Field(
-            description="An optional AWS access key to use when authenticating",
-            default=os.environ.get("AWS_ACCESS_KEY_ID"),
-        )
-        aws_secret_access_key: Optional[str] = Field(
-            description="An optional AWS secret key to use when authenticating",
-            default=os.environ.get("AWS_SECRET_ACCESS_KEY"),
-        )
-        aws_session_token: Optional[str] = Field(
-            description="An optional AWS session token to use when authenticating",
-            default=os.environ.get("AWS_SESSION_TOKEN"),
-        )
-        assume_role_arn: Optional[str] = Field(
-            description="An optional AWS role to assume when authenticating with AWS.",
-            default=None,
-        )
-        bucket_region: Optional[str] = Field(
-            description="The region that S3 the bucket exists in (default us-east-1)",
-            default=os.environ.get("AWS_REGION", "us-east-1"),
-        )
-
-        class Config:
-            """Allow environment variable override of configuration fields.
-
-            This also enforce a prefix for all environment variables for this handler.
-            As an example the field `bucket` would be set using the environment variable
-            `GROVE_OUTPUT_AWS_S3_BUCKET`.
-            """
+        env_prefix = "GROVE_OUTPUT_AWS_S3_"
+        case_insensitive = True
 
-            env_prefix = "GROVE_OUTPUT_AWS_S3_"
-            case_insensitive = True
 
-    def setup(self):
+class Handler(BaseOutput):
+    """This output handler allows Grove to write collected logs to an AWS S3 bucket."""
+
+    def __init__(self):
         """Sets up access to S3.
 
         This handler also attempt to assume a configured role in order to allow
         cross-account use - if required.
 
         :raises ConfigurationException: There was an issue with configuration.
         :raises AccessException: An issue occurred when accessing S3.
         """
-        # Explicit calls to session are mostly used to allow mocks during testing.
-        session = Session()
+        self.logger = logging.getLogger(__name__)
 
-        # Only add in optional arguments if configured.
-        client_kwargs = {}
-
-        if self.config.aws_access_key_id:
-            client_kwargs["aws_access_key_id"] = self.config.aws_access_key_id
-            client_kwargs["aws_secret_access_key"] = self.config.aws_secret_access_key
+        # Wrap validation errors to keep them in the Grove exception hierarchy.
+        try:
+            self.config = Configuration()
+        except ValidationError as err:
+            raise ConfigurationException(parsing.validation_error(err))
 
-        if self.config.aws_session_token:
-            client_kwargs["aws_session_token"] = self.config.aws_session_token
+        # Explicit calls to session are mostly used to allow mocks during testing.
+        session = Session()
 
         # If a role was specified, ensure we assume it and use STS tokens to interact
         # with S3.
         try:
             if not self.config.assume_role_arn:
-                self.s3 = session.client(
-                    "s3",
-                    region_name=self.config.bucket_region,
-                    **client_kwargs,
-                )
+                self.s3 = session.client("s3", region_name=self.config.bucket_region)
             else:
-                sts = session.client(
-                    "sts",
-                    region_name=self.config.bucket_region,
-                    **client_kwargs,
-                )
+                sts = session.client("sts")
                 role = sts.assume_role(
                     RoleArn=self.config.assume_role_arn,
                     RoleSessionName="GroveOutputWriter",
                 )
                 self.s3 = session.client(
                     "s3",
                     region_name=self.config.bucket_region,
@@ -120,50 +100,39 @@
     def submit(
         self,
         data: bytes,
         connector: str,
         identity: str,
         operation: str,
         part: int = 0,
-        kind: Optional[str] = ".json.gz",
-        descriptor: Optional[str] = "logs/",
     ):
         """Persists captured data to an S3 compatible object store.
 
         :param data: Log data to write to S3.
         :param connector: Name of the connector which retrieved the data.
         :param identity: Identity the collected data was collect for.
         :param operation: Operation the collected logs are associated with.
         :param part: Number indicating which part of the same log stream this file
             contains data for. This is used to indicate that the logs are from the same
             collection, but have been broken into smaller files for downstream
             processing.
-        :param kind: An optional file suffix to use for objects written.
-        :param descriptor: An optional path to append to the beginning of the output
-            S3 key.
 
         :raises AccessException: An issue occurred when accessing S3.
         """
-        # Append a trailing slash to the descriptor if set - to form a path.
-        if descriptor and not descriptor.endswith("/"):
-            descriptor = f"{descriptor}/"
-
         try:
             datestamp = datetime.datetime.utcnow()
             self.s3.put_object(
                 Body=data,
                 Bucket=self.config.bucket,
                 Key=OBJECT_KEY.format(
                     part=part,
                     connector=connector,
                     identity=identity,
                     operation=operation,
                     year=datestamp.strftime("%Y"),
                     month=datestamp.strftime("%m"),
                     day=datestamp.strftime("%d"),
                     datestamp=datestamp.strftime(DATESTAMP_FORMAT),
-                    descriptor=descriptor,
-                    kind=kind,
                 ),
             )
         except ClientError as err:
             raise AccessException(f"Unable to write object to AWS S3: {err}")
```

### Comparing `grove-1.0.0/grove/outputs/local_file.py` & `grove-1.0.0rc1/grove/outputs/local_file.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,70 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
 """Grove local file path output handler."""
 
 import datetime
+import logging
 import os
-from typing import Optional
 
-from pydantic import Field
+from pydantic import BaseSettings, Field, ValidationError
 
 from grove.constants import DATESTAMP_FORMAT
-from grove.exceptions import AccessException
+from grove.exceptions import AccessException, ConfigurationException
+from grove.helpers import parsing
 from grove.outputs import BaseOutput
 
 OBJECT_PATH = (
-    "{descriptor}{connector}/{identity}/{year}/{month}/{day}/"
-    "{operation}-{datestamp}.{part}{kind}"
+    "logs/{connector}/{identity}/{year}/{month}/{day}/"
+    "{operation}-{datestamp}.{part}.json.gz"
 )
 
 
-class Handler(BaseOutput):
-    class Configuration(BaseOutput.Configuration):
-        """Defines environment variables used to configure the local file handler.
+class Configuration(BaseSettings):
+    """Defines environment variables used to configure the local file handler.
 
-        This should also include any appropriate default values for fields which are not
-        required.
+    This should also include any appropriate default values for fields which are not
+    required.
+    """
+
+    path: str = Field(
+        description="The path to the directory to write collected logs to.",
+    )
+
+    class Config:
+        """Allow environment variable override of configuration fields.
+
+        This also enforce a prefix for all environment variables for this handler. As
+        an example the field `path` would be set using the environment variable
+        `GROVE_OUTPUT_LOCAL_FILE_PATH`.
         """
 
-        path: str = Field(
-            description="The path to the directory to write collected logs to.",
-        )
-
-        class Config:
-            """Allow environment variable override of configuration fields.
-
-            This also enforce a prefix for all environment variables for this handler.
-            As an example the field `path` would be set using the environment variable
-            `GROVE_OUTPUT_LOCAL_FILE_PATH`.
-            """
+        env_prefix = "GROVE_OUTPUT_LOCAL_FILE_"
+        case_insensitive = True
 
-            env_prefix = "GROVE_OUTPUT_LOCAL_FILE_"
-            case_insensitive = True
 
-    def setup(self):
+class Handler(BaseOutput):
+    def __init__(self):
         """Set up access to local filesystem path.
 
         This also checks that an output directory is configured, and it is initially
         accessible and writable.
 
-        :raises AccessException: There was an issue accessing to the provided file path.
+        :raises ConfigurationException: There was an issue with output configuration.
+        :raises AccessException: There was an issue accessing to the specified file path.
         """
+        self.logger = logging.getLogger(__name__)
+
+        # Wrap validation errors to keep them in the Grove exception hierarchy.
+        try:
+            self.config = Configuration()
+        except ValidationError as err:
+            raise ConfigurationException(parsing.validation_error(err))
+
         # Perform a spot check to see if the directory is writable now. Although this
         # can change, we'd like to bail before we collect any data if it's a simple
         # permissions related misconfiguration.
         if not os.path.isdir(self.config.path):
             raise AccessException(
                 f"Configured output path '{self.config.path}' does not exist."
             )
@@ -66,52 +77,41 @@
     def submit(
         self,
         data: bytes,
         connector: str,
         identity: str,
         operation: str,
         part: int = 0,
-        kind: Optional[str] = ".json.gz",
-        descriptor: Optional[str] = "logs/",
     ):
         """Persists captured data to a local file path.
 
         :param data: Log data to write.
         :param connector: Name of the connector which retrieved the data.
         :param identity: Identity the collected data was collect for.
         :param operation: Operation the collected logs are associated with.
         :param part: Number indicating which part of the same log stream this file
             contains data for. This is used to indicate that the logs are from the same
             collection, but have been broken into smaller files for downstream
             processing.
-        :param kind: An optional file suffix to use for files written.
-        :param descriptor: An optional path to append to the beginning of the output
-            file path.
 
         :raises AccessException: An issue occurred when writing data.
         """
-        # Append a trailing slash to the descriptor if set - to form a path.
-        if descriptor and not descriptor.endswith("/"):
-            descriptor = f"{descriptor}/"
-
         # Each log file is output under a particular hierarchy to assist with sharding
         # and ingestion / finding of log data.
         datestamp = datetime.datetime.utcnow()
 
         filename = OBJECT_PATH.format(
             part=part,
             connector=connector,
             identity=identity,
             operation=operation,
             year=datestamp.strftime("%Y"),
             month=datestamp.strftime("%m"),
             day=datestamp.strftime("%d"),
             datestamp=datestamp.strftime(DATESTAMP_FORMAT),
-            kind=kind,
-            descriptor=descriptor,
         )
 
         # Quick and dirty directory traversal check.
         destination = os.path.abspath(
             os.path.join(self.config.path, os.path.dirname(filename))
         )
```

### Comparing `grove-1.0.0/grove/outputs/local_stdout.py` & `grove-1.0.0rc1/grove/outputs/local_stdout.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,62 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
 """Grove stdout output handler."""
 
 import datetime
 import json
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List
 
 from grove.constants import DATESTAMP_FORMAT, GROVE_METADATA_KEY
 from grove.exceptions import DataFormatException
 from grove.outputs import BaseOutput
 
 
 class Handler(BaseOutput):
     def submit(
         self,
         data: bytes,
         connector: str,
         identity: str,
         operation: str,
         part: int = 0,
-        kind: Optional[str] = "json",
-        descriptor: Optional[str] = "raw",
     ):
         """Print captured data to stdout.
 
         :param data: Log data to write.
         :param connector: Name of the connector which retrieved the data.
         :param identity: Identity the collected data was collect for.
         :param operation: Operation the collected logs are associated with.
         :param part: Number indicating which part of the same log stream this file
             contains data for. This is used to indicate that the logs are from the same
             collection, but have been broken into smaller files for downstream
             processing.
-        :param kind: The format of the data being output.
-        :param descriptor: An arbitrary descriptor to identify the data being output.
-
         """
         datestamp = datetime.datetime.utcnow()
 
-        for entry in data.decode("utf-8").splitlines():
-            print(
-                json.dumps(
-                    {
-                        "part": part,
-                        "kind": kind,
-                        "descriptor": descriptor,
-                        "connector": connector,
-                        "identity": identity,
-                        "operation": operation,
-                        "datestamp": datestamp.strftime(DATESTAMP_FORMAT),
-                        "message": json.loads(entry),
-                    }
-                ),
-                flush=True,
-            )
+        print(
+            json.dumps(
+                {
+                    "part": part,
+                    "connector": connector,
+                    "identity": identity,
+                    "operation": operation,
+                    "datestamp": datestamp.strftime(DATESTAMP_FORMAT),
+                    "message": json.loads(data.decode("utf-8")),
+                }
+            ),
+            flush=True,
+        )
 
-    def serialize(self, data: List[Any], metadata: Dict[str, Any] = {}) -> bytes:
+    def serialize(self, data: List[Any], metadata: Dict[str, Any]) -> bytes:
         """Serialize data to a standard format (NDJSON).
 
         :param data: A list of log entries to serialize to JSON.
-        :param metadata: Metadata to append to each log entry before serialization. If
-            not specified no metadata will be added.
+        :param metadata: Metadata to append to JSON before serialisation.
 
         :return: Log data serialized as NDJSON.
 
         :raises DataFormatException: Cannot serialize the input to JSON.
         """
         candidate = []
```

### Comparing `grove-1.0.0/grove/secrets/__init__.py` & `grove-1.0.0rc1/grove/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove/secrets/aws_ssm.py` & `grove-1.0.0rc1/grove/secrets/aws_ssm.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,15 @@
     """Defines environment variables used to configure the AWS SSM handler.
 
     This should also include any appropriate default values for fields which are not
     required.
     """
 
     assume_role_arn: Optional[str] = Field(
-        description="An optional AWS role to assume when authenticating with AWS.",
-        default=None,
+        description="An optional AWS role to assume when authenticating with AWS."
     )
     ssm_region: Optional[str] = Field(
         description="The region that the parameter store exists in (default us-east-1)",
         default=os.environ.get("AWS_REGION", "us-east-1"),
     )
 
     class Config:
```

### Comparing `grove-1.0.0/grove/types.py` & `grove-1.0.0rc1/grove/types.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/grove.egg-info/PKG-INFO` & `grove-1.0.0rc1/grove.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,60 @@
 Metadata-Version: 2.1
 Name: grove
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: A Software as a Service (SaaS) log collection framework.
 Author: HashiCorp Security (TDR)
-License: MPL-2.0
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Natural Language :: English
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
-<p align="center">
-    <br /><br />
-    <picture>
-      <source media="(prefers-color-scheme: dark)" srcset="docs/static/grove-logo-small-light.png?raw=True">
-      <source media="(prefers-color-scheme: light)" srcset="docs/static/grove-logo-small.png?raw=True">
-      <img src="docs/static/grove-logo-small.png?raw=True" alt="Grove logo">
-    </picture>
-    <br /><br />
-</p>
+## Grove
+
+> Grove is not an official HashiCorp project.
 
 Grove is a Software as a Service (SaaS) log collection framework, designed to support
 collection of logs from services which do not natively support log streaming.
 
 Grove enables teams to collect security related events from their vendors in a reliable
 and consistent way. This data may then be stored and analyzed with a team's _existing_
 tooling in order to support threat detection and compliance programmes.
 
 Out of the box, Grove provides:
 
-* 🪵 Reliable and periodic collection of logs.
+* 🪵 Reliable and periodic log collection of logs.
 * ☁️ Support a large number of widely used SaaS applications and services.
 * 🧱 Plugin based "connectors" to enable support for new applications and services.
 * 🧳 "Bring your own" caching, output, configuration, and secrets backends.
 
 Grove was created and is currently maintained by the HashiCorp security team.
 
 **Please note**: While this is not an official HashiCorp project, security is still very
 important to us! If you have found a potential security issue with Grove, please contact
 us via email at security@hashicorp.com, rather than filing a GitHub issue.
 
 ### Supported Sources
 
-<p align="center">
-    <br /><br />
-    <picture>
-      <source media="(prefers-color-scheme: dark)" srcset="docs/static/grove-support-light.png?raw=True">
-      <source media="(prefers-color-scheme: light)" srcset="docs/static/grove-support.png?raw=True">
-      <img src="docs/static/grove-support.png?raw=True" alt="Overview of supported services, also listed below" >
-    </picture>
-    <br />
-</p>
-
 Currently the following log sources are supported by Grove out of the box. If a source
 isn't listed here, support can be added by creating a custom connector!
 
 * Atlassian audit events (e.g. Confluence, Jira)
 * GitHub audit logs
 * GSuite alerts
 * GSuite activity logs
 * Okta system logs
-* Oomnitza activity logs
 * 1Password sign-in attempt logs
 * 1Password item usage event logs
-* 1Password audit logs
 * PagerDuty audit records
 * SalesForce Cloud event logs
 * SalesForce Marketing Cloud audit event logs
 * SalesForce Marketing Cloud security event logs
 * Slack audit logs
-* Tines audit logs
 * Terraform Cloud audit trails
 * Torq activity logs
 * Torq audit logs
 * Twilio monitor events
 * Twilio message logs
 * Workday activity logs
 * Zoom activity logs
```

### Comparing `grove-1.0.0/grove.egg-info/entry_points.txt` & `grove-1.0.0rc1/grove.egg-info/entry_points.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,25 +12,22 @@
 [grove.connectors]
 atlassian_audit_events = grove.connectors.atlassian.audit_events:Connector
 github_audit_log = grove.connectors.github.audit_log:Connector
 gsuite_activities = grove.connectors.gsuite.activities:Connector
 gsuite_alerts = grove.connectors.gsuite.alerts:Connector
 local_heartbeat = grove.connectors.local.heartbeat:Connector
 okta_system_log = grove.connectors.okta.system_log:Connector
-onepassword_events_audit = grove.connectors.onepassword.events_audit:Connector
 onepassword_events_itemusages = grove.connectors.onepassword.events_itemusages:Connector
 onepassword_events_signinattempts = grove.connectors.onepassword.events_signinattempts:Connector
-oomnitza_activities = grove.connectors.oomnitza.activities:Connector
 pagerduty_audit_records = grove.connectors.pagerduty.audit_records:Connector
 sf_event_log = grove.connectors.sf.event_log:Connector
 sfmc_audit_events = grove.connectors.sfmc.audit_events:Connector
 sfmc_security_events = grove.connectors.sfmc.security_events:Connector
 slack_audit_logs = grove.connectors.slack.audit_logs:Connector
 tfc_audit_trails = grove.connectors.tfc.audit_trails:Connector
-tines_audit_logs = grove.connectors.tines.audit_logs:Connector
 torq_activity_logs = grove.connectors.torq.activity_logs:Connector
 torq_audit_logs = grove.connectors.torq.audit_logs:Connector
 twilio_messages = grove.connectors.twilio.messages:Connector
 twilio_monitor_events = grove.connectors.twilio.monitor_events:Connector
 workday_activity_logging = grove.connectors.workday.activity_logging:Connector
 zoom_activities = grove.connectors.zoom.activities:Connector
 zoom_operationlogs = grove.connectors.zoom.operationlogs:Connector
@@ -40,16 +37,9 @@
 local_process = grove.entrypoints.local_process:entrypoint
 
 [grove.outputs]
 aws_s3 = grove.outputs.aws_s3:Handler
 local_file = grove.outputs.local_file:Handler
 local_stdout = grove.outputs.local_stdout:Handler
 
-[grove.processors]
-extract_paths = grove.processors.extract_paths:Handler
-filter_paths = grove.processors.filter_paths:Handler
-split_path = grove.processors.split_path:Handler
-
 [grove.secrets]
 aws_ssm = grove.secrets.aws_ssm:Handler
-hashicorp_vault = grove.secrets.hashicorp_vault:Handler
-local_file = grove.secrets.local_file:Handler
```

### Comparing `grove-1.0.0/tests/test_caches_local_memory.py` & `grove-1.0.0rc1/tests/test_caches_local_memory.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/tests/test_configs_aws_ssm.py` & `grove-1.0.0rc1/tests/test_configs_aws_ssm.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/tests/test_connectors_atlassian_audit_events.py` & `grove-1.0.0rc1/tests/test_connectors_atlassian_audit_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
 
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 31)
+        self.assertEqual(self.connector._saved, 31)
         self.assertEqual(self.connector.pointer, "2022-05-12T19:13:13Z")
 
     @responses.activate
     def test_collect_no_pagination(self):
         """Ensure collection without pagination is working as expected."""
         responses.add(
             responses.GET,
@@ -86,9 +86,9 @@
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
 
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 1)
+        self.assertEqual(self.connector._saved, 1)
         self.assertEqual(self.connector.pointer, "2022-05-12T19:13:13Z")
```

### Comparing `grove-1.0.0/tests/test_connectors_base.py` & `grove-1.0.0rc1/tests/test_connectors_base.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/tests/test_connectors_deduplicate.py` & `grove-1.0.0rc1/tests/test_connectors_deduplicate.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,35 +57,35 @@
         for file in ["001.json", "002.json", "003.json"]:
             self.add_response(
                 path=os.path.join(self.dir, f"fixtures/grove/chronological/{file}")
             )
 
         # Run a full collection first and ensure all is as we expect.
         first_collection.run()
-        self.assertEqual(first_collection._saved["logs"], 7)
+        self.assertEqual(first_collection._saved, 7)
         self.assertEqual(first_collection.pointer, "7")
 
         # Perform a collection with the latest pointer, and ensure no new records are
         # saved - as they're duplicates. This simulates a "return logs inclusive of the
         # current pointer" operation.
         second_collection = Connector(config=config, context=context)
 
         # In-memory cache does not support locking as it's only intended for local
         # "one-shot" execution, and development use. As a result, we have to currently
-        # alias one to the other to simulate this.
+        # clone the state of one cache to the other to simulate this.
         #
         # TODO: Remove the need for this, as it's going to cause confusion in future.
         second_collection._cache._data = first_collection._cache._data
 
         self.add_response(
             path=os.path.join(self.dir, "fixtures/grove/chronological/003.json")
         )
 
         second_collection.run()
-        self.assertEqual(second_collection._saved["logs"], 0)
+        self.assertEqual(second_collection._saved, 0)
         self.assertEqual(second_collection.pointer, "7")
 
     @responses.activate
     @patch("grove.helpers.plugin.load_handler", mocks.load_handler)
     def test_deduplication_reverse_chronological(self):
         """Ensure deduplication works as expected for reverse chronological data."""
         config = ConnectorConfig(
@@ -97,42 +97,40 @@
         context = {
             "runtime": "test_harness",
             "runtime_id": "NA",
         }
 
         # Hot patch the connector to work in reverse chronological order.
         first_collection = Connector(config=config, context=context)
-
-        # This is very naughty.
         first_collection.LOG_ORDER = constants.REVERSE_CHRONOLOGICAL
 
         # Load all simulated responses in order.
         for file in ["001.json", "002.json"]:
             self.add_response(
                 path=os.path.join(
                     self.dir, f"fixtures/grove/reverse_chronological/{file}"
                 )
             )
 
         # Run a full collection first and ensure all is as we expect.
         first_collection.run()
-        self.assertEqual(first_collection._saved["logs"], 7)
+        self.assertEqual(first_collection._saved, 7)
         self.assertEqual(first_collection.pointer, "7")
 
         # Perform a collection with the latest pointer, and ensure that only new records
         # are returned.
         second_collection = Connector(config=config, context=context)
 
         # In-memory cache does not support locking as it's only intended for local
         # "one-shot" execution, and development use. As a result, we have to currently
-        # alias the state of one cache to the other to simulate this.
+        # clone the state of one cache to the other to simulate this.
         #
         # TODO: Remove the need for this, as it's going to cause confusion in future.
         second_collection._cache._data = first_collection._cache._data
 
         self.add_response(
             path=os.path.join(self.dir, "fixtures/grove/reverse_chronological/003.json")
         )
 
         second_collection.run()
-        self.assertEqual(second_collection._saved["logs"], 1)
+        self.assertEqual(second_collection._saved, 1)
         self.assertEqual(second_collection.pointer, "7")
```

### Comparing `grove-1.0.0/tests/test_connectors_github_audit.py` & `grove-1.0.0rc1/tests/test_connectors_github_audit.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             context={
                 "runtime": "test_harness",
                 "runtime_id": "NA",
             },
         )
 
     @responses.activate
-    def test_client_rate_limit_403(self):
+    def test_client_rate_limit(self):
         """Ensure ratelimit waiting is working as expected."""
         # Rate limit the first request.
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=403,
             content_type="application/json",
@@ -68,50 +68,14 @@
         # Ensure we sleep appropriately on rate-limit. This takes advantage of the retry
         # logic sleeping for one second if the ratelimit-reset header is in the past.
         with patch("time.sleep", return_value=None) as mock_sleep:
             self.connector.run()
             mock_sleep.assert_called_with(1)
 
     @responses.activate
-    def test_client_rate_limit_429(self):
-        """Ensure ratelimit waiting is working as expected."""
-        # Rate limit the first request.
-        responses.add(
-            responses.GET,
-            re.compile(r"https://.*"),
-            status=429,
-            content_type="application/json",
-            body=bytes(),
-            headers={
-                "X-RateLimit-Remaining": "0",
-                "x-ratelimit-reset": "0",  # Unix-time, so definitely in the past :)
-            },
-        )
-
-        # Succeed on the second.
-        responses.add(
-            responses.GET,
-            re.compile(r"https://.*"),
-            status=200,
-            content_type="application/json",
-            body=bytes(
-                open(
-                    os.path.join(self.dir, "fixtures/github/audit/001.json"), "r"
-                ).read(),
-                "utf-8",
-            ),
-        )
-
-        # Ensure we sleep appropriately on rate-limit. This takes advantage of the retry
-        # logic sleeping for one second if the ratelimit-reset header is in the past.
-        with patch("time.sleep", return_value=None) as mock_sleep:
-            self.connector.run()
-            mock_sleep.assert_called_with(1)
-
-    @responses.activate
     def test_collect_no_pagination(self):
         """Ensure collection without pagination is working as expected."""
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
@@ -121,9 +85,9 @@
                 ).read(),
                 "utf-8",
             ),
         )
 
         # Ensure the correct number of value are returned, and the pointer properly set.
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 2)
+        self.assertEqual(self.connector._saved, 2)
         self.assertEqual(self.connector.pointer, "1625045793361")
```

### Comparing `grove-1.0.0/tests/test_connectors_github_client.py` & `grove-1.0.0rc1/tests/test_connectors_github_client.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/tests/test_connectors_gsuite_activities.py` & `grove-1.0.0rc1/tests/test_connectors_gsuite_activities.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,9 +61,9 @@
                         "r",
                     ).read(),
                 ),
             ],
         )
         self.connector.run()
 
-        self.assertEqual(self.connector._saved["logs"], 2)
+        self.assertEqual(self.connector._saved, 2)
         self.assertEqual(self.connector.pointer, "2021-10-27T23:59:31.657Z")
```

### Comparing `grove-1.0.0/tests/test_connectors_gsuite_alerts.py` & `grove-1.0.0rc1/tests/test_connectors_gsuite_alerts.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,9 +59,9 @@
                         os.path.join(self.dir, "fixtures/gsuite/alerts/002.json"),
                         "r",
                     ).read(),
                 ),
             ],
         )
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 2)
+        self.assertEqual(self.connector._saved, 2)
         self.assertEqual(self.connector.pointer, "2021-04-03T14:05:39.950458Z")
```

### Comparing `grove-1.0.0/tests/test_connectors_lock.py` & `grove-1.0.0rc1/tests/test_connectors_lock.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/tests/test_connectors_okta_client.py` & `grove-1.0.0rc1/tests/test_connectors_okta_client.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/tests/test_connectors_okta_system_log.py` & `grove-1.0.0rc1/tests/test_connectors_okta_system_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                     os.path.join(self.dir, "fixtures/okta/system_log/001.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
         # Ensure only a single value is returned, and the pointer is properly set.
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 1)
+        self.assertEqual(self.connector._saved, 1)
         self.assertEqual(self.connector.pointer, "2021-06-24T00:04:08.123Z")
 
     @responses.activate
     def test_collect_no_results(self):
         """Ensure break occurs when there is no results returned."""
         responses.add(
             responses.GET,
```

### Comparing `grove-1.0.0/tests/test_connectors_onepassword_events_audit.py` & `grove-1.0.0rc1/tests/test_connectors_onepassword_events_itemusages.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
-"""Implements unit tests for the 1Password Audit Events collector."""
+"""Implements unit tests for the 1Password Event Item Usage collector."""
 
 import os
 import re
 import unittest
 from unittest.mock import patch
 
 import responses
 
-from grove.connectors.onepassword.events_audit import Connector
+from grove.connectors.onepassword.events_itemusages import Connector
 from grove.models import ConnectorConfig
 from tests import mocks
 
 
 class OnePasswordItemUsageEventTestCase(unittest.TestCase):
-    """Implements unit tests for the 1Password Audit Events collector."""
+    """Implements unit tests for the 1Password Item Usage Event collector."""
 
     @patch("grove.helpers.plugin.load_handler", mocks.load_handler)
     def setUp(self):
         """Ensure the application is setup for testing."""
         self.dir = os.path.dirname(os.path.abspath(__file__))
         self.connector = Connector(
             config=ConnectorConfig(
@@ -52,15 +52,15 @@
             responses.POST,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
                     os.path.join(
-                        self.dir, "fixtures/onepassword/events_audit/001.json"
+                        self.dir, "fixtures/onepassword/events_itemusages/001.json"
                     ),
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
 
@@ -76,39 +76,39 @@
             responses.POST,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
                     os.path.join(
-                        self.dir, "fixtures/onepassword/events_audit/001.json"
+                        self.dir, "fixtures/onepassword/events_itemusages/001.json"
                     ),
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
 
         # Ensure only a single value is returned, and the pointer is properly set.
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 3)
-        self.assertEqual(self.connector.pointer, "2023-03-15T16:50:50-03:00")
+        self.assertEqual(self.connector._saved, 3)
+        self.assertEqual(self.connector.pointer, "2020-06-11T16:42:55-03:00")
 
     @responses.activate
     def test_collect_pagination(self):
         """Ensure collection with pagination is working as expected."""
         responses.add(
             responses.POST,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
                     os.path.join(
-                        self.dir, "fixtures/onepassword/events_audit/002.json"
+                        self.dir, "fixtures/onepassword/events_itemusages/002.json"
                     ),
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
 
@@ -116,19 +116,19 @@
             responses.POST,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
                     os.path.join(
-                        self.dir, "fixtures/onepassword/events_audit/003.json"
+                        self.dir, "fixtures/onepassword/events_itemusages/003.json"
                     ),
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
 
         # Ensure only a single value is returned, and the pointer is properly set.
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 1)
-        self.assertEqual(self.connector.pointer, "2023-03-15T16:33:50-03:00")
+        self.assertEqual(self.connector._saved, 2)
+        self.assertEqual(self.connector.pointer, "2020-06-11T16:52:55-03:00")
```

### Comparing `grove-1.0.0/tests/test_connectors_onepassword_events_itemusages.py` & `grove-1.0.0rc1/tests/test_connectors_pagerduty_audit_records.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,134 +1,130 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
-"""Implements unit tests for the 1Password Event Item Usage collector."""
+"""Implements tests for the PagerDuty audit records collector."""
 
 import os
 import re
 import unittest
 from unittest.mock import patch
 
 import responses
 
-from grove.connectors.onepassword.events_itemusages import Connector
+from grove.connectors.pagerduty.audit_records import Connector
 from grove.models import ConnectorConfig
 from tests import mocks
 
 
-class OnePasswordItemUsageEventTestCase(unittest.TestCase):
-    """Implements unit tests for the 1Password Item Usage Event collector."""
+class PagerDutyAuditTestCase(unittest.TestCase):
+    """Implements tests for the PagerDuty audit records collector."""
 
     @patch("grove.helpers.plugin.load_handler", mocks.load_handler)
     def setUp(self):
         """Ensure the application is setup for testing."""
         self.dir = os.path.dirname(os.path.abspath(__file__))
         self.connector = Connector(
             config=ConnectorConfig(
-                identity="examplecorp",
-                key="0123456789",
-                name="examplecorp",
+                identity="1FEEDFEED1",
+                key="token",
+                name="test",
                 connector="test",
             ),
             context={
                 "runtime": "test_harness",
                 "runtime_id": "NA",
             },
         )
 
     @responses.activate
-    def test_client_rate_limit(self):
-        """Ensure ratelimit waiting is working as expected."""
+    def test_collect_rate_limit(self):
+        """Ensure rate-limit retires are working as expected."""
         # Rate limit the first request.
         responses.add(
-            responses.POST,
+            responses.GET,
             re.compile(r"https://.*"),
             status=429,
             content_type="application/json",
             body=bytes(),
         )
 
         # Succeed on the second.
         responses.add(
-            responses.POST,
+            responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(
-                        self.dir, "fixtures/onepassword/events_itemusages/001.json"
-                    ),
+                    os.path.join(self.dir, "fixtures/pagerduty/audit_records/003.json"),
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
 
-        # Ensure we sleep appropriately on rate-limit.
+        # Ensure time.sleep is called with the correct value in response to a
+        # rate-limit.
         with patch("time.sleep", return_value=None) as mock_sleep:
             self.connector.run()
             mock_sleep.assert_called_with(1)
 
     @responses.activate
-    def test_collect_no_pagination(self):
-        """Ensure collection without pagination is working as expected."""
+    def test_collect_pagination(self):
+        """Ensure pagination is working as expected."""
+        # Succeed with a cursor returned (to indicate paging is required).
         responses.add(
-            responses.POST,
+            responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(
-                        self.dir, "fixtures/onepassword/events_itemusages/001.json"
-                    ),
+                    os.path.join(self.dir, "fixtures/pagerduty/audit_records/001.json"),
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
 
-        # Ensure only a single value is returned, and the pointer is properly set.
-        self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 3)
-        self.assertEqual(self.connector.pointer, "2020-06-11T16:42:55-03:00")
-
-    @responses.activate
-    def test_collect_pagination(self):
-        """Ensure collection with pagination is working as expected."""
+        # The last "page" returns an empty cursor.
         responses.add(
-            responses.POST,
+            responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(
-                        self.dir, "fixtures/onepassword/events_itemusages/002.json"
-                    ),
+                    os.path.join(self.dir, "fixtures/pagerduty/audit_records/002.json"),
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
 
+        # Check the pointer matches the latest execution_time value, and that the
+        # expected number of logs were returned.
+        self.connector.run()
+        self.assertEqual(self.connector._saved, 5)
+        self.assertEqual(self.connector.pointer, "2021-09-08T18:03:32.120Z")
+
+    @responses.activate
+    def test_collect_no_pagination(self):
+        """Ensure collection without pagination is working as expected."""
         responses.add(
-            responses.POST,
+            responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(
-                        self.dir, "fixtures/onepassword/events_itemusages/003.json"
-                    ),
+                    os.path.join(self.dir, "fixtures/pagerduty/audit_records/003.json"),
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
 
-        # Ensure only a single value is returned, and the pointer is properly set.
+        # Set the chunk size large enough that no chunking is required.
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 2)
-        self.assertEqual(self.connector.pointer, "2020-06-11T16:52:55-03:00")
+        self.assertEqual(self.connector._saved, 4)
+        self.assertEqual(self.connector.pointer, "2021-09-08T18:05:45.120Z")
```

### Comparing `grove-1.0.0/tests/test_connectors_onepassword_events_signinattempts.py` & `grove-1.0.0rc1/tests/test_connectors_onepassword_events_signinattempts.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 ).read(),
                 "utf-8",
             ),
         )
 
         # Ensure only a single value is returned, and the pointer is properly set.
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 2)
+        self.assertEqual(self.connector._saved, 2)
         self.assertEqual(self.connector.pointer, "2021-03-01T16:42:50-03:00")
 
     @responses.activate
     def test_collect_pagination(self):
         """Ensure collection with pagination is working as expected."""
         responses.add(
             responses.POST,
@@ -126,9 +126,9 @@
                 ).read(),
                 "utf-8",
             ),
         )
 
         # Ensure only a single value is returned, and the pointer is properly set.
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 2)
+        self.assertEqual(self.connector._saved, 2)
         self.assertEqual(self.connector.pointer, "2021-03-01T16:42:50-03:00")
```

### Comparing `grove-1.0.0/tests/test_connectors_oomnitza_activities.py` & `grove-1.0.0rc1/tests/test_connectors_slack_audit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,115 +1,126 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
-"""Implements unit tests for the Oomnitza Audit collector."""
+"""Implements integration tests for the Slack Audit collector."""
 
 import os
 import re
 import unittest
 from unittest.mock import patch
 
 import responses
 
-from grove.connectors.oomnitza.activities import Connector
+from grove.connectors.slack.audit_logs import Connector
 from grove.models import ConnectorConfig
 from tests import mocks
 
 
-class OomnitzaAuditTestCase(unittest.TestCase):
-    """Implements unit tests for the Oomnitza Activities collector."""
+class SlackAuditTestCase(unittest.TestCase):
+    """Implements integration tests for the Slack Audit collector."""
 
     @patch("grove.helpers.plugin.load_handler", mocks.load_handler)
     def setUp(self):
         """Ensure the application is setup for testing."""
         self.dir = os.path.dirname(os.path.abspath(__file__))
         self.connector = Connector(
             config=ConnectorConfig(
-                identity="corp",
-                key="testkey",
-                name="corp",
+                identity="1FEEDFEED1",
+                key="token",
+                name="test",
                 connector="test",
             ),
             context={
                 "runtime": "test_harness",
                 "runtime_id": "NA",
             },
         )
 
     @responses.activate
-    def test_collect_pagination(self):
-        """Ensure pagination is working as expected."""
+    def test_collect_rate_limit(self):
+        """Ensure rate-limit retires are working as expected."""
+        # Rate limit the first request.
+        responses.add(
+            responses.GET,
+            re.compile(r"https://.*"),
+            status=429,
+            content_type="application/json",
+            body=bytes(),
+            headers={
+                "Retry-After": "66",
+            },
+        )
+
+        # Succeed on the second.
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/oomnitza/activities/002.json"),
-                    "r",
+                    os.path.join(self.dir, "fixtures/slack/audit/002.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
 
-        # The last "page" returns an empty cursor.
+        # Ensure time.sleep is called with the correct value in response to a
+        # rate-limit.
+        with patch("time.sleep", return_value=None) as mock_sleep:
+            self.connector.run()
+            mock_sleep.assert_called_with(66)
+
+    @responses.activate
+    def test_collect_pagination(self):
+        """Ensure pagination is working as expected."""
+        # Succeed with a cursor returned (to indicate paging is required).
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/oomnitza/activities/001.json"),
-                    "r",
+                    os.path.join(self.dir, "fixtures/slack/audit/001.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
 
-        # Check the pointer matches the latest execution_time value, and that the
-        # expected number of logs were returned.
-        self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 205)
-        self.assertEqual(self.connector.pointer, "1682538024")
-
-    @responses.activate
-    def test_collect_no_pagination(self):
-        """Ensure collection without pagination is working as expected."""
+        # The last "page" returns an empty cursor.
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/oomnitza/activities/001.json"),
-                    "r",
+                    os.path.join(self.dir, "fixtures/slack/audit/002.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
 
-        # Ensure only a single value is returned, and the pointer is properly set.
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 5)
-        self.assertEqual(self.connector.pointer, "1680895957")
+        self.assertEqual(self.connector._saved, 2)
+        self.assertEqual(self.connector.pointer, "1521214344")
 
     @responses.activate
-    def test_collect_no_results(self):
-        """Ensure break accurs when there is no results returned."""
+    def test_collect_no_pagination(self):
+        """Ensure collection without pagination is working as expected."""
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/oomnitza/activities/003.json"),
-                    "r",
+                    os.path.join(self.dir, "fixtures/slack/audit/003.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
+
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 0)
+        self.assertEqual(self.connector._saved, 19)
+        self.assertEqual(self.connector.pointer, "1521214944")
```

### Comparing `grove-1.0.0/tests/test_connectors_pagerduty_audit_records.py` & `grove-1.0.0rc1/tests/test_connectors_zoom_operation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,125 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
-"""Implements tests for the PagerDuty audit records collector."""
+"""Implements unit tests for the Zoom Operation Log collector."""
 
 import os
 import re
 import unittest
 from unittest.mock import patch
 
 import responses
+from responses import matchers
 
-from grove.connectors.pagerduty.audit_records import Connector
+from grove.connectors.zoom.operationlogs import Connector
 from grove.models import ConnectorConfig
 from tests import mocks
 
 
-class PagerDutyAuditTestCase(unittest.TestCase):
-    """Implements tests for the PagerDuty audit records collector."""
+class ZoomOperationLogsTestCase(unittest.TestCase):
+    """Implements unit tests for the Zoom Operation Logs collector."""
 
     @patch("grove.helpers.plugin.load_handler", mocks.load_handler)
     def setUp(self):
         """Ensure the application is setup for testing."""
         self.dir = os.path.dirname(os.path.abspath(__file__))
         self.connector = Connector(
             config=ConnectorConfig(
-                identity="1FEEDFEED1",
-                key="token",
+                identity="client_id",
+                key="test_key",
                 name="test",
                 connector="test",
             ),
             context={
                 "runtime": "test_harness",
                 "runtime_id": "NA",
             },
         )
 
     @responses.activate
-    def test_collect_rate_limit(self):
-        """Ensure rate-limit retires are working as expected."""
-        # Rate limit the first request.
+    def test_collect_pagination(self):
+        """Ensure pagination is working as expected."""
+        # set bearer token
         responses.add(
-            responses.GET,
-            re.compile(r"https://.*"),
-            status=429,
-            content_type="application/json",
-            body=bytes(),
-        )
-
-        # Succeed on the second.
-        responses.add(
-            responses.GET,
+            responses.POST,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/pagerduty/audit_records/003.json"),
+                    os.path.join(self.dir, "fixtures/zoom/client/001.json"),
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
-
-        # Ensure time.sleep is called with the correct value in response to a
-        # rate-limit.
-        with patch("time.sleep", return_value=None) as mock_sleep:
-            self.connector.run()
-            mock_sleep.assert_called_with(1)
-
-    @responses.activate
-    def test_collect_pagination(self):
-        """Ensure pagination is working as expected."""
-        # Succeed with a cursor returned (to indicate paging is required).
+        # first page has a cursor to the next page
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/pagerduty/audit_records/001.json"),
-                    "r",
+                    os.path.join(self.dir, "fixtures/zoom/operation/001.json"), "r"
                 ).read(),
                 "utf-8",
             ),
+            match=[matchers.header_matcher({"Authorization": "Bearer testtoken"})],
         )
 
-        # The last "page" returns an empty cursor.
+        # The last page returns no cursor.
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/pagerduty/audit_records/002.json"),
-                    "r",
+                    os.path.join(self.dir, "fixtures/zoom/operation/002.json"), "r"
                 ).read(),
                 "utf-8",
             ),
+            match=[matchers.header_matcher({"Authorization": "Bearer testtoken"})],
         )
 
-        # Check the pointer matches the latest execution_time value, and that the
-        # expected number of logs were returned.
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 5)
-        self.assertEqual(self.connector.pointer, "2021-09-08T18:03:32.120Z")
+        self.assertEqual(self.connector._saved, 31)
+        self.assertEqual(self.connector.pointer, "2022-08-23T14:46:17Z")
 
     @responses.activate
     def test_collect_no_pagination(self):
         """Ensure collection without pagination is working as expected."""
+        # set bearer token
         responses.add(
-            responses.GET,
+            responses.POST,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/pagerduty/audit_records/003.json"),
+                    os.path.join(self.dir, "fixtures/zoom/client/001.json"),
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
 
-        # Set the chunk size large enough that no chunking is required.
+        # add one entry result with no cursor
+        responses.add(
+            responses.GET,
+            re.compile(r"https://.*"),
+            status=200,
+            content_type="application/json",
+            body=bytes(
+                open(
+                    os.path.join(self.dir, "fixtures/zoom/operation/002.json"), "r"
+                ).read(),
+                "utf-8",
+            ),
+            match=[matchers.header_matcher({"Authorization": "Bearer testtoken"})],
+        )
+
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 4)
-        self.assertEqual(self.connector.pointer, "2021-09-08T18:05:45.120Z")
+        self.assertEqual(self.connector._saved, 1)
+        self.assertEqual(self.connector.pointer, "2022-08-23T14:46:17Z")
```

### Comparing `grove-1.0.0/tests/test_connectors_sf_event_log.py` & `grove-1.0.0rc1/tests/test_connectors_sf_event_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,9 +111,9 @@
             body=log_response,
             content_type="text/csv",
         )
 
         # Check the pointer matches the latest value, and that the expected number of
         # logs were returned.
         self.connector.collect()
-        self.assertEqual(self.connector._saved["logs"], 2)
+        self.assertEqual(self.connector._saved, 2)
         self.assertEqual(self.connector.pointer, "2038-01-19T03:00:00.000Z")
```

### Comparing `grove-1.0.0/tests/test_connectors_sfmc_audit_events.py` & `grove-1.0.0rc1/tests/test_connectors_sfmc_audit_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 "utf-8",
             ),
         )
 
         # Check the pointer matches the latest value, and that the expected number of
         # logs were returned.
         self.connector.collect()
-        self.assertEqual(self.connector._saved["logs"], 2)
+        self.assertEqual(self.connector._saved, 2)
         self.assertEqual(self.connector.pointer, "2019-01-02T12:00:00.00")
 
     @responses.activate
     def test_collect_no_pagination(self):
         """Ensure collection without pagination is working as expected."""
         responses.add(
             responses.GET,
@@ -85,9 +85,9 @@
                     os.path.join(self.dir, "fixtures/sfmc/audit_events/003.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
 
         self.connector.collect()
-        self.assertEqual(self.connector._saved["logs"], 7)
+        self.assertEqual(self.connector._saved, 7)
         self.assertEqual(self.connector.pointer, "2019-01-07T12:00:00.00")
```

### Comparing `grove-1.0.0/tests/test_connectors_sfmc_security_events.py` & `grove-1.0.0rc1/tests/test_connectors_sfmc_security_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
 
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 2)
+        self.assertEqual(self.connector._saved, 2)
         self.assertEqual(self.connector.pointer, "2019-01-02T12:00:00.00")
 
     @responses.activate
     def test_collect_no_pagination(self):
         """Ensure collection without pagination is working as expected."""
         responses.add(
             responses.GET,
@@ -86,9 +86,9 @@
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
 
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 7)
+        self.assertEqual(self.connector._saved, 7)
         self.assertEqual(self.connector.pointer, "2019-01-07T12:00:00.00")
```

### Comparing `grove-1.0.0/tests/test_connectors_slack_audit.py` & `grove-1.0.0rc1/tests/test_connectors_tfc_audit_trails.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
-"""Implements integration tests for the Slack Audit collector."""
+"""Implements integration tests for the TFC Audit collector."""
 
 import os
 import re
 import unittest
 from unittest.mock import patch
 
 import responses
 
-from grove.connectors.slack.audit_logs import Connector
+from grove.connectors.tfc.audit_trails import Connector
 from grove.models import ConnectorConfig
 from tests import mocks
 
 
-class SlackAuditTestCase(unittest.TestCase):
-    """Implements integration tests for the Slack Audit collector."""
+class TFCAuditTestCase(unittest.TestCase):
+    """Implements integration tests for the TFC Audit collector."""
 
     @patch("grove.helpers.plugin.load_handler", mocks.load_handler)
     def setUp(self):
         """Ensure the application is setup for testing."""
         self.dir = os.path.dirname(os.path.abspath(__file__))
         self.connector = Connector(
             config=ConnectorConfig(
@@ -41,86 +41,83 @@
         # Rate limit the first request.
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=429,
             content_type="application/json",
             body=bytes(),
-            headers={
-                "Retry-After": "66",
-            },
         )
 
         # Succeed on the second.
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/slack/audit/002.json"), "r"
+                    os.path.join(self.dir, "fixtures/tfc/audit_trails/002.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
 
         # Ensure time.sleep is called with the correct value in response to a
         # rate-limit.
         with patch("time.sleep", return_value=None) as mock_sleep:
             self.connector.run()
-            mock_sleep.assert_called_with(66)
+            mock_sleep.assert_called_with(1)
 
     @responses.activate
     def test_collect_pagination(self):
         """Ensure pagination is working as expected."""
         # Succeed with a cursor returned (to indicate paging is required).
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/slack/audit/001.json"), "r"
+                    os.path.join(self.dir, "fixtures/tfc/audit_trails/001.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
 
         # The last "page" returns an empty cursor.
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/slack/audit/002.json"), "r"
+                    os.path.join(self.dir, "fixtures/tfc/audit_trails/002.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
 
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 2)
-        self.assertEqual(self.connector.pointer, "1521214344")
+        self.assertEqual(self.connector._saved, 3)
+        self.assertEqual(self.connector.pointer, "2020-06-30T17:52:46.000Z")
 
     @responses.activate
     def test_collect_no_pagination(self):
         """Ensure collection without pagination is working as expected."""
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/slack/audit/003.json"), "r"
+                    os.path.join(self.dir, "fixtures/tfc/audit_trails/003.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
 
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 19)
-        self.assertEqual(self.connector.pointer, "1521214944")
+        self.assertEqual(self.connector._saved, 5)
+        self.assertEqual(self.connector.pointer, "2020-06-30T17:52:46.000Z")
```

### Comparing `grove-1.0.0/tests/test_connectors_tines_audit_logs.py` & `grove-1.0.0rc1/tests/test_connectors_zoom_activities.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,125 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
-"""Implements integration tests for the Tines Audit Log collector."""
+"""Implements unit tests for the Zoom Activity Log collector."""
 
 import os
 import re
 import unittest
 from unittest.mock import patch
 
 import responses
+from responses import matchers
 
-from grove.connectors.tines.audit_logs import Connector
+from grove.connectors.zoom.activities import Connector
 from grove.models import ConnectorConfig
 from tests import mocks
 
 
-class TinesAuditTestCase(unittest.TestCase):
-    """Implements integration tests for the Tines Audit collector."""
+class ZoomActivitiesTestCase(unittest.TestCase):
+    """Implements unit tests for the Zoom Activity Logs collector."""
 
     @patch("grove.helpers.plugin.load_handler", mocks.load_handler)
     def setUp(self):
         """Ensure the application is setup for testing."""
         self.dir = os.path.dirname(os.path.abspath(__file__))
         self.connector = Connector(
             config=ConnectorConfig(
-                identity="1FEEDFEED1",
-                key="token",
+                identity="client_id",
+                key="test_key",
                 name="test",
                 connector="test",
             ),
             context={
                 "runtime": "test_harness",
                 "runtime_id": "NA",
             },
         )
 
     @responses.activate
     def test_collect_pagination(self):
         """Ensure pagination is working as expected."""
-        # Succeed with a cursor returned (to indicate paging is required).
+        # set bearer token
+        responses.add(
+            responses.POST,
+            re.compile(r"https://.*"),
+            status=200,
+            content_type="application/json",
+            body=bytes(
+                open(
+                    os.path.join(self.dir, "fixtures/zoom/client/001.json"),
+                    "r",
+                ).read(),
+                "utf-8",
+            ),
+        )
+        # first page has a cursor to the next page
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/tines/audit_logs/001.json"), "r"
+                    os.path.join(self.dir, "fixtures/zoom/activities/001.json"), "r"
                 ).read(),
                 "utf-8",
             ),
+            match=[matchers.header_matcher({"Authorization": "Bearer testtoken"})],
         )
 
-        # The last "page" returns an empty cursor.
+        # The last page returns no cursor.
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/tines/audit_logs/002.json"), "r"
+                    os.path.join(self.dir, "fixtures/zoom/activities/002.json"), "r"
                 ).read(),
                 "utf-8",
             ),
+            match=[matchers.header_matcher({"Authorization": "Bearer testtoken"})],
         )
 
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 2)
-        self.assertEqual(self.connector.pointer, "2023-07-21T14:21:30Z")
+        self.assertEqual(self.connector._saved, 31)
+        self.assertEqual(self.connector.pointer, "2022-08-23T14:45:54Z")
 
     @responses.activate
     def test_collect_no_pagination(self):
         """Ensure collection without pagination is working as expected."""
+        # set bearer token
+        responses.add(
+            responses.POST,
+            re.compile(r"https://.*"),
+            status=200,
+            content_type="application/json",
+            body=bytes(
+                open(
+                    os.path.join(self.dir, "fixtures/zoom/client/001.json"),
+                    "r",
+                ).read(),
+                "utf-8",
+            ),
+        )
+
+        # add one entry result with no cursor
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/tines/audit_logs/003.json"), "r"
+                    os.path.join(self.dir, "fixtures/zoom/activities/002.json"), "r"
                 ).read(),
                 "utf-8",
             ),
+            match=[matchers.header_matcher({"Authorization": "Bearer testtoken"})],
         )
 
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 2)
-        self.assertEqual(self.connector.pointer, "2023-07-21T10:32:37Z")
+        self.assertEqual(self.connector._saved, 1)
+        self.assertEqual(self.connector.pointer, "2022-08-23T14:45:54Z")
```

### Comparing `grove-1.0.0/tests/test_connectors_torq_activity_logs.py` & `grove-1.0.0rc1/tests/test_connectors_torq_activity_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                 matchers.header_matcher(
                     {"Authorization": f"Bearer aaaaaaaa-aaaa-aaaa-aaaa-aaaaaaaaaaaa"}
                 )
             ],
         )
 
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 2)
+        self.assertEqual(self.connector._saved, 2)
         # it's reverse chronological so the earlier timestamp should be recorded
         self.assertEqual(self.connector.pointer, "2022-06-24T18:15:07.380622Z")
 
     @responses.activate
     def test_collect_no_pagination(self):
         """Ensure collection without pagination is working as expected."""
         # set bearer token
@@ -130,9 +130,9 @@
                 matchers.header_matcher(
                     {"Authorization": f"Bearer aaaaaaaa-aaaa-aaaa-aaaa-aaaaaaaaaaaa"}
                 )
             ],
         )
 
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 1)
+        self.assertEqual(self.connector._saved, 1)
         self.assertEqual(self.connector.pointer, "2022-06-24T18:15:06.380622Z")
```

### Comparing `grove-1.0.0/tests/test_connectors_torq_audit_logs.py` & `grove-1.0.0rc1/tests/test_connectors_torq_audit_logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                 matchers.header_matcher(
                     {"Authorization": f"Bearer aaaaaaaa-aaaa-aaaa-aaaa-aaaaaaaaaaaa"}
                 )
             ],
         )
 
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 4)
+        self.assertEqual(self.connector._saved, 4)
         # it's reverse chronological so the earlier timestamp should be recorded
         self.assertEqual(self.connector.pointer, "2022-06-27T11:35:10.681687Z")
 
     @responses.activate
     def test_collect_no_pagination(self):
         """Ensure collection without pagination is working as expected."""
         # set bearer token
@@ -130,9 +130,9 @@
                 matchers.header_matcher(
                     {"Authorization": f"Bearer aaaaaaaa-aaaa-aaaa-aaaa-aaaaaaaaaaaa"}
                 )
             ],
         )
 
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 1)
+        self.assertEqual(self.connector._saved, 1)
         self.assertEqual(self.connector.pointer, "2022-06-07T11:35:11.681687Z")
```

### Comparing `grove-1.0.0/tests/test_connectors_torq_clients.py` & `grove-1.0.0rc1/tests/test_connectors_torq_clients.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/tests/test_connectors_workday_activity_logging.py` & `grove-1.0.0rc1/tests/test_connectors_workday_activity_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,15 @@
                 "utf-8",
             ),
         )
 
         # Check the pointer matches the latest execution_time value, and that the
         # expected number of logs were returned.
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 113)
+        self.assertEqual(self.connector._saved, 113)
         self.assertEqual(self.connector.pointer, "2021-10-12T23:50:09.752Z")
 
     @responses.activate
     def test_collect_no_pagination(self):
         """Ensure collection without pagination is working as expected."""
         # Get bearer token
         responses.add(
@@ -230,15 +230,15 @@
                 ).read(),
                 "utf-8",
             ),
         )
 
         # Ensure only a single value is returned, and the pointer is properly set.
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 13)
+        self.assertEqual(self.connector._saved, 13)
         self.assertEqual(self.connector.pointer, "2021-10-12T23:50:09.752Z")
 
     @responses.activate
     def test_collect_no_results(self):
         """Ensure break accurs when there is no results returned."""
         # Get bearer token
         responses.add(
@@ -268,8 +268,8 @@
                     ),
                     "r",
                 ).read(),
                 "utf-8",
             ),
         )
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 0)
+        self.assertEqual(self.connector._saved, 0)
```

### Comparing `grove-1.0.0/tests/test_connectors_zoom_client.py` & `grove-1.0.0rc1/tests/test_connectors_zoom_client.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/tests/test_e2e_grove_cli.py` & `grove-1.0.0rc1/tests/test_e2e_grove_cli.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/tests/test_outputs_aws_s3.py` & `grove-1.0.0rc1/tests/test_outputs_aws_s3.py`

 * *Files identical despite different names*

### Comparing `grove-1.0.0/tests/test_outputs_base.py` & `grove-1.0.0rc1/tests/test_outputs_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 
 from grove.outputs import BaseOutput
 
 
 # Required as BaseOutput is an ABC, so without defining submit we will not be able to
 # instantiate it to validate methods on the base class.
 class TestOutput(BaseOutput):
-    __test__ = False
-
     def submit(self, *args, **kwargs):
         pass
 
 
 class BaseOutputTestCase(unittest.TestCase):
     """Implements tests for the base output handler."""
```

