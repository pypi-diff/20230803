# Comparing `tmp/pulumi_signalfx-6.1.0.tar.gz` & `tmp/pulumi_signalfx-6.2.0a1691044148.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_signalfx-6.1.0.tar", last modified: Wed Aug  2 17:24:10 2023, max compression
+gzip compressed data, was "pulumi_signalfx-6.2.0a1691044148.tar", last modified: Thu Aug  3 06:46:04 2023, max compression
```

## Comparing `pulumi_signalfx-6.1.0.tar` & `pulumi_signalfx-6.2.0a1691044148.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.815032 pulumi_signalfx-6.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-08-02 17:24:10.815032 pulumi_signalfx-6.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.811032 pulumi_signalfx-6.1.0/pulumi_signalfx/
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   140636 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/alert_muting_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.811032 pulumi_signalfx-6.1.0/pulumi_signalfx/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/aws/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19593 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/aws/external_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    81078 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/aws/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/aws/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/aws/token_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.811032 pulumi_signalfx-6.1.0/pulumi_signalfx/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/azure/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53922 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/azure/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/azure/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.811032 pulumi_signalfx-6.1.0/pulumi_signalfx/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    61578 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    36715 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/dashboard_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23028 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/data_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    63092 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/event_feed_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.815032 pulumi_signalfx-6.1.0/pulumi_signalfx/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/gcp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36033 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/gcp/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/gcp/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/get_dimension_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    42295 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/heatmap_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.815032 pulumi_signalfx-6.1.0/pulumi_signalfx/jira/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32032 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/jira/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    62676 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/list_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.815032 pulumi_signalfx-6.1.0/pulumi_signalfx/log/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/log/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/log/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/log/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    28449 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/log/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.815032 pulumi_signalfx-6.1.0/pulumi_signalfx/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/logs/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/logs/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28664 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/logs/view.py
--rw-r--r--   0 runner    (1001) docker     (123)    18758 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/metric_ruleset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.815032 pulumi_signalfx-6.1.0/pulumi_signalfx/opsgenie/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/opsgenie/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    23045 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/org_token.py
--rw-r--r--   0 runner    (1001) docker     (123)   127525 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.815032 pulumi_signalfx-6.1.0/pulumi_signalfx/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/pagerduty/get_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/pagerduty/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.815032 pulumi_signalfx-6.1.0/pulumi_signalfx/servicenow/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/servicenow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27661 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/servicenow/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/single_value_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.815032 pulumi_signalfx-6.1.0/pulumi_signalfx/slack/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/slack/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    31617 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/table_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    27565 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/text_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    80156 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/time_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.815032 pulumi_signalfx-6.1.0/pulumi_signalfx/victorops/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/victorops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/victorops/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx/webhook_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:24:10.811032 pulumi_signalfx-6.1.0/pulumi_signalfx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/pulumi_signalfx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:24:10.815032 pulumi_signalfx-6.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-02 17:24:10.000000 pulumi_signalfx-6.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.181064 pulumi_signalfx-6.2.0a1691044148/
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-08-03 06:46:04.181064 pulumi_signalfx-6.2.0a1691044148/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.173063 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   140636 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/alert_muting_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.173063 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/aws/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19593 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/aws/external_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81078 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/aws/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/aws/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/aws/token_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.177064 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/azure/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53922 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/azure/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/azure/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.177064 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61578 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36715 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/dashboard_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23028 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/data_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63092 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/event_feed_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.177064 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/gcp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36033 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/gcp/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/gcp/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/get_dimension_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42295 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/heatmap_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.177064 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/jira/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32032 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/jira/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62676 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/list_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.177064 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/log/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/log/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/log/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28449 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/log/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.177064 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/logs/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/logs/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28664 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/logs/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18758 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/metric_ruleset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.181064 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/opsgenie/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23045 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/org_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127525 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.181064 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/pagerduty/get_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/pagerduty/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.181064 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/servicenow/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/servicenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27661 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/servicenow/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/single_value_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.181064 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/slack/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31617 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/table_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27565 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/text_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80156 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/time_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.181064 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/victorops/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/victorops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/victorops/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/webhook_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:46:04.173063 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-08-03 06:46:04.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-08-03 06:46:04.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:46:04.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:46:04.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 06:46:04.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 06:46:04.000000 pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:46:04.181064 pulumi_signalfx-6.2.0a1691044148/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-03 06:46:03.000000 pulumi_signalfx-6.2.0a1691044148/setup.py
```

### Comparing `pulumi_signalfx-6.1.0/PKG-INFO` & `pulumi_signalfx-6.2.0a1691044148/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_signalfx
-Version: 6.1.0
+Version: 6.2.0a1691044148
 Summary: A Pulumi package for creating and managing SignalFx resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi signalfx
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_signalfx-6.1.0/README.md` & `pulumi_signalfx-6.2.0a1691044148/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/__init__.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/_inputs.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/_utilities.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/alert_muting_rule.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/alert_muting_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/aws/_inputs.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/aws/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/aws/external_integration.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/aws/external_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/aws/integration.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/aws/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/aws/outputs.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/aws/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/aws/token_integration.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/aws/token_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/azure/_inputs.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/azure/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/azure/integration.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/azure/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/azure/outputs.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/azure/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/config/vars.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/dashboard.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/dashboard_group.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/dashboard_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/data_link.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/data_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/detector.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/detector.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/event_feed_chart.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/event_feed_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/gcp/_inputs.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/gcp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/gcp/integration.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/gcp/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/gcp/outputs.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/gcp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/get_dimension_values.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/get_dimension_values.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/heatmap_chart.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/heatmap_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/jira/integration.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/jira/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/list_chart.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/list_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/log/_inputs.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/log/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/log/outputs.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/log/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/log/timeline.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/log/timeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/log/view.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/log/view.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/logs/_inputs.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/logs/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/logs/outputs.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/logs/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/logs/view.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/logs/view.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/metric_ruleset.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/metric_ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/opsgenie/integration.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/opsgenie/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/org_token.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/org_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/outputs.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/pagerduty/get_integration.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/pagerduty/get_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/pagerduty/integration.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/pagerduty/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/provider.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/servicenow/integration.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/servicenow/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/single_value_chart.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/single_value_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/slack/integration.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/slack/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/table_chart.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/table_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/team.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/text_chart.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/text_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/time_chart.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/time_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/victorops/integration.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/victorops/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx/webhook_integration.py` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx/webhook_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx.egg-info/PKG-INFO` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-signalfx
-Version: 6.1.0
+Version: 6.2.0a1691044148
 Summary: A Pulumi package for creating and managing SignalFx resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi signalfx
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_signalfx-6.1.0/pulumi_signalfx.egg-info/SOURCES.txt` & `pulumi_signalfx-6.2.0a1691044148/pulumi_signalfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.1.0/setup.py` & `pulumi_signalfx-6.2.0a1691044148/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.1.0"
-PLUGIN_VERSION = "6.1.0"
+VERSION = "6.2.0a1691044148"
+PLUGIN_VERSION = "6.2.0-alpha.1691044148+ddf0dc06"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'signalfx', PLUGIN_VERSION])
         except OSError as error:
```

