# Comparing `tmp/pulumi_wavefront-2.0.0a0.tar.gz` & `tmp/pulumi_wavefront-2.0.0a1690995516.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_wavefront-2.0.0a0.tar", last modified: Wed Aug  2 15:40:52 2023, max compression
+gzip compressed data, was "pulumi_wavefront-2.0.0a1690995516.tar", last modified: Wed Aug  2 17:03:41 2023, max compression
```

## Comparing `pulumi_wavefront-2.0.0a0.tar` & `pulumi_wavefront-2.0.0a1690995516.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:40:52.963550 pulumi_wavefront-2.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-02 15:40:52.963550 pulumi_wavefront-2.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:40:52.963550 pulumi_wavefront-2.0.0a0/pulumi_wavefront/
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78096 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    49247 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    36453 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/alert_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    46819 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_app_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_aws_external_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    30615 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_azure_activity_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    28833 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_cloud_trail.py
--rw-r--r--   0 runner    (1001) docker     (123)    36599 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_cloud_watch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24093 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29291 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_gcp_billing.py
--rw-r--r--   0 runner    (1001) docker     (123)    26214 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_new_relic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:40:52.963550 pulumi_wavefront-2.0.0a0/pulumi_wavefront/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/dashboard_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/external_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    16347 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_default_user_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    15861 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_derived_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_external_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_external_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_maintenance_window_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_metrics_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_user_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/ingestion_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    34484 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/metrics_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)   210614 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    18961 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/user_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:40:52.963550 pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:40:52.963550 pulumi_wavefront-2.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:03:41.357169 pulumi_wavefront-2.0.0a1690995516/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-08-02 17:03:41.357169 pulumi_wavefront-2.0.0a1690995516/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:03:41.353169 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78096 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49247 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36453 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/alert_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46819 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_app_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_aws_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30615 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_azure_activity_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28833 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_cloud_trail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36599 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_cloud_watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24093 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29291 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_gcp_billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26214 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_new_relic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:03:41.357169 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/dashboard_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/external_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16347 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_default_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15861 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_derived_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_external_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_external_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_maintenance_window_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_metrics_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/ingestion_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34484 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/metrics_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   210614 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18961 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/user_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:03:41.357169 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:03:41.357169 pulumi_wavefront-2.0.0a1690995516/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-02 17:03:41.000000 pulumi_wavefront-2.0.0a1690995516/setup.py
```

### Comparing `pulumi_wavefront-2.0.0a0/PKG-INFO` & `pulumi_wavefront-2.0.0a1690995516/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_wavefront
-Version: 2.0.0a0
+Version: 2.0.0a1690995516
 Summary: A Pulumi package for creating and managing wavefront cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-wavefront
 Keywords: pulumi wavefront
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_wavefront-2.0.0a0/README.md` & `pulumi_wavefront-2.0.0a1690995516/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/__init__.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/_inputs.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/_utilities.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/alert.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/alert.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/alert_target.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/alert_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_app_dynamics.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_app_dynamics.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_aws_external_id.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_aws_external_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_azure.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_azure.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_azure_activity_log.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_azure_activity_log.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_cloud_trail.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_cloud_trail.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_cloud_watch.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_cloud_watch.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_ec2.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_ec2.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_gcp.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_gcp.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_gcp_billing.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_gcp_billing.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_new_relic.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/cloud_integration_new_relic.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/config/vars.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/dashboard.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/dashboard_json.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/dashboard_json.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/derived_metric.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/derived_metric.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/event.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/event.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/external_link.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/external_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_alert.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_alert.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_alerts.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_alerts.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_dashboard.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_dashboards.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_dashboards.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_default_user_group.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_default_user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_derived_metric.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_derived_metric.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_derived_metrics.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_derived_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_event.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_event.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_events.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_events.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_external_link.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_external_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_external_links.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_external_links.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_maintenance_window.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_maintenance_window_all.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_maintenance_window_all.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_metrics_policy.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_metrics_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_role.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_roles.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_user.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_user_group.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_user_groups.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_users.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/ingestion_policy.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/ingestion_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/maintenance_window.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/metrics_policy.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/metrics_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/outputs.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/provider.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/role.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/service_account.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/user.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront/user_group.py` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront/user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/PKG-INFO` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-wavefront
-Version: 2.0.0a0
+Version: 2.0.0a1690995516
 Summary: A Pulumi package for creating and managing wavefront cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-wavefront
 Keywords: pulumi wavefront
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/SOURCES.txt` & `pulumi_wavefront-2.0.0a1690995516/pulumi_wavefront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-2.0.0a0/setup.py` & `pulumi_wavefront-2.0.0a1690995516/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.0.0a0"
-PLUGIN_VERSION = "2.0.0-alpha.0"
+VERSION = "2.0.0a1690995516"
+PLUGIN_VERSION = "2.0.0-alpha.1690995516+06f8f92d"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'wavefront', PLUGIN_VERSION])
         except OSError as error:
```

