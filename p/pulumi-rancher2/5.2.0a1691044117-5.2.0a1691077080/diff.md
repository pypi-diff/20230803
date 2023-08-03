# Comparing `tmp/pulumi_rancher2-5.2.0a1691044117.tar.gz` & `tmp/pulumi_rancher2-5.2.0a1691077080.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rancher2-5.2.0a1691044117.tar", last modified: Thu Aug  3 06:45:50 2023, max compression
+gzip compressed data, was "pulumi_rancher2-5.2.0a1691077080.tar", last modified: Thu Aug  3 15:43:46 2023, max compression
```

## Comparing `pulumi_rancher2-5.2.0a1691044117.tar` & `pulumi_rancher2-5.2.0a1691077080.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:45:50.313352 pulumi_rancher2-5.2.0a1691044117/
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-08-03 06:45:50.313352 pulumi_rancher2-5.2.0a1691044117/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:45:50.309352 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/
--rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1331725 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    81934 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/active_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    40919 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    39478 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/app_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    81893 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_active_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_adfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    74864 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_free_ipa.py
--rw-r--r--   0 runner    (1001) docker     (123)    26284 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_github.py
--rw-r--r--   0 runner    (1001) docker     (123)    37428 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_keycloak.py
--rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_okta.py
--rw-r--r--   0 runner    (1001) docker     (123)    74951 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_open_ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)    36725 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_ping.py
--rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    32734 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    34681 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    45103 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)   154396 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    25128 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    39686 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    25349 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_alter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    35202 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_alter_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    24092 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    25480 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    31455 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    25028 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    53172 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:45:50.313352 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    32293 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/custom_user_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    24961 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cluster_alter_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cluster_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_global_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_node_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_node_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    29150 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_principal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_role_tempalte.py
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_role_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/global_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/global_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    47168 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/machine_config_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    41496 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/node_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    31694 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/node_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    82407 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/node_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)  1650650 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    77219 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    37627 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    37710 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/role_tempalte.py
--rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/role_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    28125 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:45:50.313352 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-08-03 06:45:50.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-08-03 06:45:50.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:45:50.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:45:50.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 06:45:50.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 06:45:50.000000 pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:45:50.313352 pulumi_rancher2-5.2.0a1691044117/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-03 06:45:49.000000 pulumi_rancher2-5.2.0a1691044117/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:43:46.586376 pulumi_rancher2-5.2.0a1691077080/
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-08-03 15:43:46.586376 pulumi_rancher2-5.2.0a1691077080/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:43:46.582376 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1337305 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81934 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/active_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40919 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39478 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/app_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81893 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_active_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_adfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74864 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_free_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26284 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37428 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74951 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_open_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37231 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32734 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34681 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45068 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158431 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25128 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39686 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25349 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_alter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35202 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_alter_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24092 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25487 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31462 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25030 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51694 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:43:46.586376 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32293 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/custom_user_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25468 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cluster_alter_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cluster_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_global_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_node_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29585 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_principal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_role_tempalte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_role_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/global_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/global_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18960 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47177 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/machine_config_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41496 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31708 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82423 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/node_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1656094 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77219 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37627 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37710 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21370 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/role_tempalte.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/role_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28125 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:43:46.582376 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:43:46.586376 pulumi_rancher2-5.2.0a1691077080/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-03 15:43:46.000000 pulumi_rancher2-5.2.0a1691077080/setup.py
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/PKG-INFO` & `pulumi_rancher2-5.2.0a1691077080/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rancher2
-Version: 5.2.0a1691044117
+Version: 5.2.0a1691077080
 Summary: A Pulumi package for creating and managing rancher2 resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi rancher2
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/README.md` & `pulumi_rancher2-5.2.0a1691077080/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/__init__.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/_inputs.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1426,14 +1426,17 @@
 
     @property
     @pulumi.getter
     def tag(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Use `tags` argument instead as []string
         """
+        warnings.warn("""Use tags argument instead as []string""", DeprecationWarning)
+        pulumi.log.warn("""tag is deprecated: Use tags argument instead as []string""")
+
         return pulumi.get(self, "tag")
 
     @tag.setter
     def tag(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "tag", value)
 
     @property
@@ -2735,42 +2738,56 @@
 
 @pulumi.input_type
 class ClusterClusterAgentDeploymentCustomizationArgs:
     def __init__(__self__, *,
                  append_tolerations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationAppendTolerationArgs']]]] = None,
                  override_affinity: Optional[pulumi.Input[str]] = None,
                  override_resource_requirements: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]] = None):
+        """
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationAppendTolerationArgs']]] append_tolerations: User defined tolerations to append to agent (list)
+        :param pulumi.Input[str] override_affinity: User defined affinity to override default agent affinity (string)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs']]] override_resource_requirements: User defined resource requirements to set on the agent (list)
+        """
         if append_tolerations is not None:
             pulumi.set(__self__, "append_tolerations", append_tolerations)
         if override_affinity is not None:
             pulumi.set(__self__, "override_affinity", override_affinity)
         if override_resource_requirements is not None:
             pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
 
     @property
     @pulumi.getter(name="appendTolerations")
     def append_tolerations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationAppendTolerationArgs']]]]:
+        """
+        User defined tolerations to append to agent (list)
+        """
         return pulumi.get(self, "append_tolerations")
 
     @append_tolerations.setter
     def append_tolerations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationAppendTolerationArgs']]]]):
         pulumi.set(self, "append_tolerations", value)
 
     @property
     @pulumi.getter(name="overrideAffinity")
     def override_affinity(self) -> Optional[pulumi.Input[str]]:
+        """
+        User defined affinity to override default agent affinity (string)
+        """
         return pulumi.get(self, "override_affinity")
 
     @override_affinity.setter
     def override_affinity(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "override_affinity", value)
 
     @property
     @pulumi.getter(name="overrideResourceRequirements")
     def override_resource_requirements(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]:
+        """
+        User defined resource requirements to set on the agent (list)
+        """
         return pulumi.get(self, "override_resource_requirements")
 
     @override_resource_requirements.setter
     def override_resource_requirements(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]):
         pulumi.set(self, "override_resource_requirements", value)
 
 
@@ -2780,17 +2797,17 @@
                  key: pulumi.Input[str],
                  effect: Optional[pulumi.Input[str]] = None,
                  operator: Optional[pulumi.Input[str]] = None,
                  seconds: Optional[pulumi.Input[int]] = None,
                  value: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] key: The toleration key (string)
-        :param pulumi.Input[str] effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
-        :param pulumi.Input[str] operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
-        :param pulumi.Input[int] seconds: The toleration seconds (int)
+        :param pulumi.Input[str] effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param pulumi.Input[str] operator: The toleration operator (string)
+        :param pulumi.Input[int] seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param pulumi.Input[str] value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -2811,39 +2828,39 @@
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[pulumi.Input[str]]:
         """
-        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @effect.setter
     def effect(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "effect", value)
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[pulumi.Input[str]]:
         """
-        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[pulumi.Input[int]]:
         """
-        The toleration seconds (int)
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
         """
         return pulumi.get(self, "seconds")
 
     @seconds.setter
     def seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "seconds", value)
 
@@ -2863,53 +2880,71 @@
 @pulumi.input_type
 class ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs:
     def __init__(__self__, *,
                  cpu_limit: Optional[pulumi.Input[str]] = None,
                  cpu_request: Optional[pulumi.Input[str]] = None,
                  memory_limit: Optional[pulumi.Input[str]] = None,
                  memory_request: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] cpu_limit: The maximum CPU limit for agent (string)
+        :param pulumi.Input[str] cpu_request: The minimum CPU required for agent (string)
+        :param pulumi.Input[str] memory_limit: The maximum memory limit for agent (string)
+        :param pulumi.Input[str] memory_request: The minimum memory required for agent (string)
+        """
         if cpu_limit is not None:
             pulumi.set(__self__, "cpu_limit", cpu_limit)
         if cpu_request is not None:
             pulumi.set(__self__, "cpu_request", cpu_request)
         if memory_limit is not None:
             pulumi.set(__self__, "memory_limit", memory_limit)
         if memory_request is not None:
             pulumi.set(__self__, "memory_request", memory_request)
 
     @property
     @pulumi.getter(name="cpuLimit")
     def cpu_limit(self) -> Optional[pulumi.Input[str]]:
+        """
+        The maximum CPU limit for agent (string)
+        """
         return pulumi.get(self, "cpu_limit")
 
     @cpu_limit.setter
     def cpu_limit(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cpu_limit", value)
 
     @property
     @pulumi.getter(name="cpuRequest")
     def cpu_request(self) -> Optional[pulumi.Input[str]]:
+        """
+        The minimum CPU required for agent (string)
+        """
         return pulumi.get(self, "cpu_request")
 
     @cpu_request.setter
     def cpu_request(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cpu_request", value)
 
     @property
     @pulumi.getter(name="memoryLimit")
     def memory_limit(self) -> Optional[pulumi.Input[str]]:
+        """
+        The maximum memory limit for agent (string)
+        """
         return pulumi.get(self, "memory_limit")
 
     @memory_limit.setter
     def memory_limit(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "memory_limit", value)
 
     @property
     @pulumi.getter(name="memoryRequest")
     def memory_request(self) -> Optional[pulumi.Input[str]]:
+        """
+        The minimum memory required for agent (string)
+        """
         return pulumi.get(self, "memory_request")
 
     @memory_request.setter
     def memory_request(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "memory_request", value)
 
 
@@ -3370,17 +3405,17 @@
                  virtual_network: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] access_key: Access key for S3 service (string)
         :param pulumi.Input[str] kubernetes_version: K8s version to deploy. Default: `Rancher default` (string) (Note - if rke_config is set at cluster_template, kubernetes_version must be set to the active cluster version so Rancher can clone the RKE template)
         :param pulumi.Input[str] secret_key: Secret key for S3 service (string)
         :param pulumi.Input[str] ami: AMI ID to use for the worker nodes instead of the default (string)
         :param pulumi.Input[bool] associate_worker_node_public_ip: Associate public ip EKS worker nodes. Default `true` (bool)
-        :param pulumi.Input[int] desired_nodes: The desired number of worker nodes. Just for Rancher v2.3.x and above. Default `3` (int)
+        :param pulumi.Input[int] desired_nodes: The desired number of worker nodes. For Rancher v2.3.x and above. Default `3` (int)
         :param pulumi.Input[str] instance_type: The type of machine to use for worker nodes. Default `t2.medium` (string)
-        :param pulumi.Input[str] key_pair_name: Allow user to specify key name to use. Just for Rancher v2.2.7 and above (string)
+        :param pulumi.Input[str] key_pair_name: Allow user to specify key name to use. For Rancher v2.2.7 and above (string)
         :param pulumi.Input[int] maximum_nodes: The maximum number of worker nodes. Default `3` (int)
         :param pulumi.Input[int] minimum_nodes: The minimum number of worker nodes. Default `1` (int)
         :param pulumi.Input[int] node_volume_size: The volume size for each node. Default `20` (int)
         :param pulumi.Input[str] region: (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: List of security groups to use for the cluster. If it's not specified Rancher will create a new security group (list)
         :param pulumi.Input[str] service_role: The service role to use to perform the cluster operations in AWS. If it's not specified Rancher will create a new service role (string)
         :param pulumi.Input[str] session_token: A session token to use with the client key and secret if applicable (string)
@@ -3484,15 +3519,15 @@
     def associate_worker_node_public_ip(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "associate_worker_node_public_ip", value)
 
     @property
     @pulumi.getter(name="desiredNodes")
     def desired_nodes(self) -> Optional[pulumi.Input[int]]:
         """
-        The desired number of worker nodes. Just for Rancher v2.3.x and above. Default `3` (int)
+        The desired number of worker nodes. For Rancher v2.3.x and above. Default `3` (int)
         """
         return pulumi.get(self, "desired_nodes")
 
     @desired_nodes.setter
     def desired_nodes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "desired_nodes", value)
 
@@ -3517,15 +3552,15 @@
     def instance_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_type", value)
 
     @property
     @pulumi.getter(name="keyPairName")
     def key_pair_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Allow user to specify key name to use. Just for Rancher v2.2.7 and above (string)
+        Allow user to specify key name to use. For Rancher v2.2.7 and above (string)
         """
         return pulumi.get(self, "key_pair_name")
 
     @key_pair_name.setter
     def key_pair_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_pair_name", value)
 
@@ -4282,42 +4317,56 @@
 
 @pulumi.input_type
 class ClusterFleetAgentDeploymentCustomizationArgs:
     def __init__(__self__, *,
                  append_tolerations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationAppendTolerationArgs']]]] = None,
                  override_affinity: Optional[pulumi.Input[str]] = None,
                  override_resource_requirements: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]] = None):
+        """
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationAppendTolerationArgs']]] append_tolerations: User defined tolerations to append to agent (list)
+        :param pulumi.Input[str] override_affinity: User defined affinity to override default agent affinity (string)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirementArgs']]] override_resource_requirements: User defined resource requirements to set on the agent (list)
+        """
         if append_tolerations is not None:
             pulumi.set(__self__, "append_tolerations", append_tolerations)
         if override_affinity is not None:
             pulumi.set(__self__, "override_affinity", override_affinity)
         if override_resource_requirements is not None:
             pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
 
     @property
     @pulumi.getter(name="appendTolerations")
     def append_tolerations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationAppendTolerationArgs']]]]:
+        """
+        User defined tolerations to append to agent (list)
+        """
         return pulumi.get(self, "append_tolerations")
 
     @append_tolerations.setter
     def append_tolerations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationAppendTolerationArgs']]]]):
         pulumi.set(self, "append_tolerations", value)
 
     @property
     @pulumi.getter(name="overrideAffinity")
     def override_affinity(self) -> Optional[pulumi.Input[str]]:
+        """
+        User defined affinity to override default agent affinity (string)
+        """
         return pulumi.get(self, "override_affinity")
 
     @override_affinity.setter
     def override_affinity(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "override_affinity", value)
 
     @property
     @pulumi.getter(name="overrideResourceRequirements")
     def override_resource_requirements(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]:
+        """
+        User defined resource requirements to set on the agent (list)
+        """
         return pulumi.get(self, "override_resource_requirements")
 
     @override_resource_requirements.setter
     def override_resource_requirements(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]):
         pulumi.set(self, "override_resource_requirements", value)
 
 
@@ -4327,17 +4376,17 @@
                  key: pulumi.Input[str],
                  effect: Optional[pulumi.Input[str]] = None,
                  operator: Optional[pulumi.Input[str]] = None,
                  seconds: Optional[pulumi.Input[int]] = None,
                  value: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] key: The toleration key (string)
-        :param pulumi.Input[str] effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
-        :param pulumi.Input[str] operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
-        :param pulumi.Input[int] seconds: The toleration seconds (int)
+        :param pulumi.Input[str] effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param pulumi.Input[str] operator: The toleration operator (string)
+        :param pulumi.Input[int] seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param pulumi.Input[str] value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -4358,39 +4407,39 @@
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[pulumi.Input[str]]:
         """
-        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @effect.setter
     def effect(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "effect", value)
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[pulumi.Input[str]]:
         """
-        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[pulumi.Input[int]]:
         """
-        The toleration seconds (int)
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
         """
         return pulumi.get(self, "seconds")
 
     @seconds.setter
     def seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "seconds", value)
 
@@ -4410,53 +4459,71 @@
 @pulumi.input_type
 class ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirementArgs:
     def __init__(__self__, *,
                  cpu_limit: Optional[pulumi.Input[str]] = None,
                  cpu_request: Optional[pulumi.Input[str]] = None,
                  memory_limit: Optional[pulumi.Input[str]] = None,
                  memory_request: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] cpu_limit: The maximum CPU limit for agent (string)
+        :param pulumi.Input[str] cpu_request: The minimum CPU required for agent (string)
+        :param pulumi.Input[str] memory_limit: The maximum memory limit for agent (string)
+        :param pulumi.Input[str] memory_request: The minimum memory required for agent (string)
+        """
         if cpu_limit is not None:
             pulumi.set(__self__, "cpu_limit", cpu_limit)
         if cpu_request is not None:
             pulumi.set(__self__, "cpu_request", cpu_request)
         if memory_limit is not None:
             pulumi.set(__self__, "memory_limit", memory_limit)
         if memory_request is not None:
             pulumi.set(__self__, "memory_request", memory_request)
 
     @property
     @pulumi.getter(name="cpuLimit")
     def cpu_limit(self) -> Optional[pulumi.Input[str]]:
+        """
+        The maximum CPU limit for agent (string)
+        """
         return pulumi.get(self, "cpu_limit")
 
     @cpu_limit.setter
     def cpu_limit(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cpu_limit", value)
 
     @property
     @pulumi.getter(name="cpuRequest")
     def cpu_request(self) -> Optional[pulumi.Input[str]]:
+        """
+        The minimum CPU required for agent (string)
+        """
         return pulumi.get(self, "cpu_request")
 
     @cpu_request.setter
     def cpu_request(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cpu_request", value)
 
     @property
     @pulumi.getter(name="memoryLimit")
     def memory_limit(self) -> Optional[pulumi.Input[str]]:
+        """
+        The maximum memory limit for agent (string)
+        """
         return pulumi.get(self, "memory_limit")
 
     @memory_limit.setter
     def memory_limit(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "memory_limit", value)
 
     @property
     @pulumi.getter(name="memoryRequest")
     def memory_request(self) -> Optional[pulumi.Input[str]]:
+        """
+        The minimum memory required for agent (string)
+        """
         return pulumi.get(self, "memory_request")
 
     @memory_request.setter
     def memory_request(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "memory_request", value)
 
 
@@ -6276,27 +6343,27 @@
 @pulumi.input_type
 class ClusterGkeConfigV2NodePoolConfigTaintArgs:
     def __init__(__self__, *,
                  effect: pulumi.Input[str],
                  key: pulumi.Input[str],
                  value: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        :param pulumi.Input[str] effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
         :param pulumi.Input[str] key: The toleration key (string)
         :param pulumi.Input[str] value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "effect", effect)
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def effect(self) -> pulumi.Input[str]:
         """
-        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @effect.setter
     def effect(self, value: pulumi.Input[str]):
         pulumi.set(self, "effect", value)
 
@@ -6572,18 +6639,18 @@
         :param pulumi.Input[str] private_key_contents: The private API key file contents for the specified user, in PEM format (string)
         :param pulumi.Input[str] region: (string)
         :param pulumi.Input[str] tenancy_id: The OCID of the tenancy in which to create resources (string)
         :param pulumi.Input[str] user_ocid: The OCID of a user who has access to the tenancy/compartment (string)
         :param pulumi.Input[int] custom_boot_volume_size: Optional custom boot volume size (GB) for all nodes. If you specify 0, it will apply the default according to the `node_image` specified. Default `0` (int)
         :param pulumi.Input[str] description: The description for Cluster (string)
         :param pulumi.Input[bool] enable_kubernetes_dashboard: Whether to enable the Kubernetes dashboard. Default `false` (bool)
-        :param pulumi.Input[bool] enable_private_control_plane: Specifies whether Kubernetes API endpoint is a private IP only accessible from within the VCN. Default `false` Just for Rancher v2.5.10 or above (bool)
+        :param pulumi.Input[bool] enable_private_control_plane: Specifies whether Kubernetes API endpoint is a private IP only accessible from within the VCN. Default `false` for Rancher v2.5.10 and above (bool)
         :param pulumi.Input[bool] enable_private_nodes: Whether nodes have internal IP address only. Default `false` (bool)
         :param pulumi.Input[int] flex_ocpus: Specifies number of OCPUs for nodes (requires flexible shape specified with `node_shape`) (int)
-        :param pulumi.Input[str] kms_key_id: The OCID of a KMS vault master key used to encrypt secrets at rest. See [here](https://docs.oracle.com/en-us/iaas/Content/ContEng/Tasks/contengencryptingdata.htm) for help creating a vault and master encryption key. Just for Rancher v2.5.9 or above (string)
+        :param pulumi.Input[str] kms_key_id: The OCID of a KMS vault master key used to encrypt secrets at rest. See [here](https://docs.oracle.com/en-us/iaas/Content/ContEng/Tasks/contengencryptingdata.htm) for help creating a vault and master encryption key. For Rancher v2.5.9 and above (string)
         :param pulumi.Input[int] limit_node_count: The maximum number of worker nodes. Can limit `quantity_per_subnet`. Default `0` (no limit) (int)
         :param pulumi.Input[str] load_balancer_subnet_name1: The name of the first existing subnet to use for Kubernetes services / LB. `vcn_name` is also required when specifying an existing subnet. (string)
         :param pulumi.Input[str] load_balancer_subnet_name2: The name of a second existing subnet to use for Kubernetes services / LB. A second subnet is only required when it is AD-specific (non-regional) (string)
         :param pulumi.Input[str] node_pool_dns_domain_name: Name for DNS domain of node pool subnet. Default `nodedns` (string)
         :param pulumi.Input[str] node_pool_subnet_name: Name for node pool subnet. Default `nodedns` (string)
         :param pulumi.Input[str] node_public_key_contents: The contents of the SSH public key file to use for the nodes (string)
         :param pulumi.Input[str] pod_cidr: A CIDR notation IP range from which to assign Kubernetes Pod IPs when \\"network plugin\\" is specified in \\"kubenet\\". Default `172.244.0.0/16` (string)
@@ -6797,15 +6864,15 @@
     def enable_kubernetes_dashboard(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_kubernetes_dashboard", value)
 
     @property
     @pulumi.getter(name="enablePrivateControlPlane")
     def enable_private_control_plane(self) -> Optional[pulumi.Input[bool]]:
         """
-        Specifies whether Kubernetes API endpoint is a private IP only accessible from within the VCN. Default `false` Just for Rancher v2.5.10 or above (bool)
+        Specifies whether Kubernetes API endpoint is a private IP only accessible from within the VCN. Default `false` for Rancher v2.5.10 and above (bool)
         """
         return pulumi.get(self, "enable_private_control_plane")
 
     @enable_private_control_plane.setter
     def enable_private_control_plane(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_private_control_plane", value)
 
@@ -6833,15 +6900,15 @@
     def flex_ocpus(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "flex_ocpus", value)
 
     @property
     @pulumi.getter(name="kmsKeyId")
     def kms_key_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The OCID of a KMS vault master key used to encrypt secrets at rest. See [here](https://docs.oracle.com/en-us/iaas/Content/ContEng/Tasks/contengencryptingdata.htm) for help creating a vault and master encryption key. Just for Rancher v2.5.9 or above (string)
+        The OCID of a KMS vault master key used to encrypt secrets at rest. See [here](https://docs.oracle.com/en-us/iaas/Content/ContEng/Tasks/contengencryptingdata.htm) for help creating a vault and master encryption key. For Rancher v2.5.9 and above (string)
         """
         return pulumi.get(self, "kms_key_id")
 
     @kms_key_id.setter
     def kms_key_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kms_key_id", value)
 
@@ -7178,15 +7245,15 @@
         :param pulumi.Input[int] addon_job_timeout: Duration in seconds of addon job (int)
         :param pulumi.Input[str] addons: Addons descripton to deploy on RKE cluster.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] addons_includes: Addons yaml manifests to deploy on RKE cluster (list)
         :param pulumi.Input['ClusterRkeConfigAuthenticationArgs'] authentication: Kubernetes cluster authentication (list maxitems:1)
         :param pulumi.Input['ClusterRkeConfigAuthorizationArgs'] authorization: Kubernetes cluster authorization (list maxitems:1)
         :param pulumi.Input['ClusterRkeConfigBastionHostArgs'] bastion_host: RKE bastion host (list maxitems:1)
         :param pulumi.Input['ClusterRkeConfigCloudProviderArgs'] cloud_provider: RKE cloud provider [rke-cloud-providers](https://rancher.com/docs/rke/v0.1.x/en/config-options/cloud-providers/) (list maxitems:1)
-        :param pulumi.Input['ClusterRkeConfigDnsArgs'] dns: RKE dns add-on. Just for Rancher v2.2.x (list maxitems:1)
+        :param pulumi.Input['ClusterRkeConfigDnsArgs'] dns: RKE dns add-on. For Rancher v2.2.x (list maxitems:1)
         :param pulumi.Input[bool] enable_cri_dockerd: Enable/disable using cri-dockerd. Deafult: `false` [enable_cri_dockerd](https://rancher.com/docs/rke/latest/en/config-options/#cri-dockerd) (bool)
         :param pulumi.Input[bool] ignore_docker_version: Ignore docker version. Default `true` (bool)
         :param pulumi.Input['ClusterRkeConfigIngressArgs'] ingress: Kubernetes ingress configuration (list maxitems:1)
         :param pulumi.Input[str] kubernetes_version: K8s version to deploy. Default: `Rancher default` (string) (Note - if rke_config is set at cluster_template, kubernetes_version must be set to the active cluster version so Rancher can clone the RKE template)
         :param pulumi.Input['ClusterRkeConfigMonitoringArgs'] monitoring: Kubernetes cluster monitoring (list maxitems:1)
         :param pulumi.Input['ClusterRkeConfigNetworkArgs'] network: Kubernetes cluster networking (list maxitems:1)
         :param pulumi.Input[Sequence[pulumi.Input['ClusterRkeConfigNodeArgs']]] nodes: RKE cluster nodes (list)
@@ -7330,15 +7397,15 @@
     def cloud_provider(self, value: Optional[pulumi.Input['ClusterRkeConfigCloudProviderArgs']]):
         pulumi.set(self, "cloud_provider", value)
 
     @property
     @pulumi.getter
     def dns(self) -> Optional[pulumi.Input['ClusterRkeConfigDnsArgs']]:
         """
-        RKE dns add-on. Just for Rancher v2.2.x (list maxitems:1)
+        RKE dns add-on. For Rancher v2.2.x (list maxitems:1)
         """
         return pulumi.get(self, "dns")
 
     @dns.setter
     def dns(self, value: Optional[pulumi.Input['ClusterRkeConfigDnsArgs']]):
         pulumi.set(self, "dns", value)
 
@@ -9830,17 +9897,17 @@
                  key: pulumi.Input[str],
                  effect: Optional[pulumi.Input[str]] = None,
                  operator: Optional[pulumi.Input[str]] = None,
                  seconds: Optional[pulumi.Input[int]] = None,
                  value: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] key: The toleration key (string)
-        :param pulumi.Input[str] effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
-        :param pulumi.Input[str] operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
-        :param pulumi.Input[int] seconds: The toleration seconds (int)
+        :param pulumi.Input[str] effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param pulumi.Input[str] operator: The toleration operator (string)
+        :param pulumi.Input[int] seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param pulumi.Input[str] value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -9861,39 +9928,39 @@
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[pulumi.Input[str]]:
         """
-        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @effect.setter
     def effect(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "effect", value)
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[pulumi.Input[str]]:
         """
-        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[pulumi.Input[int]]:
         """
-        The toleration seconds (int)
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
         """
         return pulumi.get(self, "seconds")
 
     @seconds.setter
     def seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "seconds", value)
 
@@ -10177,17 +10244,17 @@
                  key: pulumi.Input[str],
                  effect: Optional[pulumi.Input[str]] = None,
                  operator: Optional[pulumi.Input[str]] = None,
                  seconds: Optional[pulumi.Input[int]] = None,
                  value: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] key: The toleration key (string)
-        :param pulumi.Input[str] effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
-        :param pulumi.Input[str] operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
-        :param pulumi.Input[int] seconds: The toleration seconds (int)
+        :param pulumi.Input[str] effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param pulumi.Input[str] operator: The toleration operator (string)
+        :param pulumi.Input[int] seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param pulumi.Input[str] value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -10208,39 +10275,39 @@
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[pulumi.Input[str]]:
         """
-        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @effect.setter
     def effect(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "effect", value)
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[pulumi.Input[str]]:
         """
-        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[pulumi.Input[int]]:
         """
-        The toleration seconds (int)
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
         """
         return pulumi.get(self, "seconds")
 
     @seconds.setter
     def seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "seconds", value)
 
@@ -10428,17 +10495,17 @@
                  key: pulumi.Input[str],
                  effect: Optional[pulumi.Input[str]] = None,
                  operator: Optional[pulumi.Input[str]] = None,
                  seconds: Optional[pulumi.Input[int]] = None,
                  value: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] key: The toleration key (string)
-        :param pulumi.Input[str] effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
-        :param pulumi.Input[str] operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
-        :param pulumi.Input[int] seconds: The toleration seconds (int)
+        :param pulumi.Input[str] effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param pulumi.Input[str] operator: The toleration operator (string)
+        :param pulumi.Input[int] seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param pulumi.Input[str] value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -10459,39 +10526,39 @@
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[pulumi.Input[str]]:
         """
-        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @effect.setter
     def effect(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "effect", value)
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[pulumi.Input[str]]:
         """
-        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[pulumi.Input[int]]:
         """
-        The toleration seconds (int)
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
         """
         return pulumi.get(self, "seconds")
 
     @seconds.setter
     def seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "seconds", value)
 
@@ -11983,17 +12050,17 @@
                  key: pulumi.Input[str],
                  effect: Optional[pulumi.Input[str]] = None,
                  operator: Optional[pulumi.Input[str]] = None,
                  seconds: Optional[pulumi.Input[int]] = None,
                  value: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] key: The toleration key (string)
-        :param pulumi.Input[str] effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
-        :param pulumi.Input[str] operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
-        :param pulumi.Input[int] seconds: The toleration seconds (int)
+        :param pulumi.Input[str] effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param pulumi.Input[str] operator: The toleration operator (string)
+        :param pulumi.Input[int] seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param pulumi.Input[str] value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -12014,39 +12081,39 @@
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[pulumi.Input[str]]:
         """
-        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @effect.setter
     def effect(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "effect", value)
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[pulumi.Input[str]]:
         """
-        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[pulumi.Input[int]]:
         """
-        The toleration seconds (int)
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
         """
         return pulumi.get(self, "seconds")
 
     @seconds.setter
     def seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "seconds", value)
 
@@ -12540,29 +12607,29 @@
                  image: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  retention: Optional[pulumi.Input[str]] = None,
                  snapshot: Optional[pulumi.Input[bool]] = None,
                  uid: Optional[pulumi.Input[int]] = None):
         """
-        :param pulumi.Input['ClusterRkeConfigServicesEtcdBackupConfigArgs'] backup_config: Backup options for etcd service. Just for Rancher v2.2.x (list maxitems:1)
+        :param pulumi.Input['ClusterRkeConfigServicesEtcdBackupConfigArgs'] backup_config: Backup options for etcd service. For Rancher v2.2.x (list maxitems:1)
         :param pulumi.Input[str] ca_cert: TLS CA certificate for etcd service (string)
         :param pulumi.Input[str] cert: TLS certificate for etcd service (string)
         :param pulumi.Input[str] creation: Creation option for etcd service (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] external_urls: External urls for etcd service (list)
         :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for RKE Ingress (map)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds for etcd service (list)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra environment for etcd service (list)
-        :param pulumi.Input[int] gid: Etcd service GID. Default: `0`. For Rancher v2.3.x or above (int)
+        :param pulumi.Input[int] gid: Etcd service GID. Default: `0`. For Rancher v2.3.x and above (int)
         :param pulumi.Input[str] image: Docker image for etcd service (string)
         :param pulumi.Input[str] key: The toleration key (string)
         :param pulumi.Input[str] path: Path for etcd service (string)
         :param pulumi.Input[str] retention: Retention option for etcd service (string)
         :param pulumi.Input[bool] snapshot: Snapshot option for etcd service (bool)
-        :param pulumi.Input[int] uid: Etcd service UID. Default: `0`. For Rancher v2.3.x or above (int)
+        :param pulumi.Input[int] uid: Etcd service UID. Default: `0`. For Rancher v2.3.x and above (int)
         """
         if backup_config is not None:
             pulumi.set(__self__, "backup_config", backup_config)
         if ca_cert is not None:
             pulumi.set(__self__, "ca_cert", ca_cert)
         if cert is not None:
             pulumi.set(__self__, "cert", cert)
@@ -12591,15 +12658,15 @@
         if uid is not None:
             pulumi.set(__self__, "uid", uid)
 
     @property
     @pulumi.getter(name="backupConfig")
     def backup_config(self) -> Optional[pulumi.Input['ClusterRkeConfigServicesEtcdBackupConfigArgs']]:
         """
-        Backup options for etcd service. Just for Rancher v2.2.x (list maxitems:1)
+        Backup options for etcd service. For Rancher v2.2.x (list maxitems:1)
         """
         return pulumi.get(self, "backup_config")
 
     @backup_config.setter
     def backup_config(self, value: Optional[pulumi.Input['ClusterRkeConfigServicesEtcdBackupConfigArgs']]):
         pulumi.set(self, "backup_config", value)
 
@@ -12687,15 +12754,15 @@
     def extra_envs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_envs", value)
 
     @property
     @pulumi.getter
     def gid(self) -> Optional[pulumi.Input[int]]:
         """
-        Etcd service GID. Default: `0`. For Rancher v2.3.x or above (int)
+        Etcd service GID. Default: `0`. For Rancher v2.3.x and above (int)
         """
         return pulumi.get(self, "gid")
 
     @gid.setter
     def gid(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "gid", value)
 
@@ -12759,15 +12826,15 @@
     def snapshot(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "snapshot", value)
 
     @property
     @pulumi.getter
     def uid(self) -> Optional[pulumi.Input[int]]:
         """
-        Etcd service UID. Default: `0`. For Rancher v2.3.x or above (int)
+        Etcd service UID. Default: `0`. For Rancher v2.3.x and above (int)
         """
         return pulumi.get(self, "uid")
 
     @uid.setter
     def uid(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "uid", value)
 
@@ -12783,15 +12850,15 @@
                  timeout: Optional[pulumi.Input[int]] = None):
         """
         :param pulumi.Input[bool] enabled: Enable etcd backup (bool)
         :param pulumi.Input[int] interval_hours: Interval hours for etcd backup. Default `12` (int)
         :param pulumi.Input[int] retention: Retention option for etcd service (string)
         :param pulumi.Input['ClusterRkeConfigServicesEtcdBackupConfigS3BackupConfigArgs'] s3_backup_config: S3 config options for etcd backup (list maxitems:1)
         :param pulumi.Input[bool] safe_timestamp: Safe timestamp for etcd backup. Default: `false` (bool)
-        :param pulumi.Input[int] timeout: Timeout in seconds for etcd backup. Default: `300`. Just for Rancher v2.5.6 and above (int)
+        :param pulumi.Input[int] timeout: Timeout in seconds for etcd backup. Default: `300`. For Rancher v2.5.6 and above (int)
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if interval_hours is not None:
             pulumi.set(__self__, "interval_hours", interval_hours)
         if retention is not None:
             pulumi.set(__self__, "retention", retention)
@@ -12862,15 +12929,15 @@
     def safe_timestamp(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "safe_timestamp", value)
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[pulumi.Input[int]]:
         """
-        Timeout in seconds for etcd backup. Default: `300`. Just for Rancher v2.5.6 and above (int)
+        Timeout in seconds for etcd backup. Default: `300`. For Rancher v2.5.6 and above (int)
         """
         return pulumi.get(self, "timeout")
 
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout", value)
 
@@ -13250,26 +13317,14 @@
 class ClusterRkeConfigServicesKubeApiAdmissionConfigurationPluginArgs:
     def __init__(__self__, *,
                  configuration: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] configuration: Plugin configuration. (string) Ex:
-               
-               ```python
-               import pulumi
-               ```
-               configuration = <<EOF
-               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
-               kind: Configuration
-               limits:
-               - type: Server
-               burst: 35000
-               qps: 6000
-               EOF
         :param pulumi.Input[str] name: The name of the Cluster (string)
         :param pulumi.Input[str] path: Path for etcd service (string)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -13277,26 +13332,14 @@
             pulumi.set(__self__, "path", path)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[pulumi.Input[str]]:
         """
         Plugin configuration. (string) Ex:
-
-        ```python
-        import pulumi
-        ```
-        configuration = <<EOF
-        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
-        kind: Configuration
-        limits:
-        - type: Server
-        burst: 35000
-        qps: 6000
-        EOF
         """
         return pulumi.get(self, "configuration")
 
     @configuration.setter
     def configuration(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "configuration", value)
 
@@ -13328,50 +13371,26 @@
 @pulumi.input_type
 class ClusterRkeConfigServicesKubeApiAuditLogArgs:
     def __init__(__self__, *,
                  configuration: Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs']] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs'] configuration: Plugin configuration. (string) Ex:
-               
-               ```python
-               import pulumi
-               ```
-               configuration = <<EOF
-               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
-               kind: Configuration
-               limits:
-               - type: Server
-               burst: 35000
-               qps: 6000
-               EOF
         :param pulumi.Input[bool] enabled: Enable etcd backup (bool)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs']]:
         """
         Plugin configuration. (string) Ex:
-
-        ```python
-        import pulumi
-        ```
-        configuration = <<EOF
-        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
-        kind: Configuration
-        limits:
-        - type: Server
-        burst: 35000
-        qps: 6000
-        EOF
         """
         return pulumi.get(self, "configuration")
 
     @configuration.setter
     def configuration(self, value: Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs']]):
         pulumi.set(self, "configuration", value)
 
@@ -13494,50 +13513,26 @@
 @pulumi.input_type
 class ClusterRkeConfigServicesKubeApiEventRateLimitArgs:
     def __init__(__self__, *,
                  configuration: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input[str] configuration: Plugin configuration. (string) Ex:
-               
-               ```python
-               import pulumi
-               ```
-               configuration = <<EOF
-               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
-               kind: Configuration
-               limits:
-               - type: Server
-               burst: 35000
-               qps: 6000
-               EOF
         :param pulumi.Input[bool] enabled: Enable etcd backup (bool)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[pulumi.Input[str]]:
         """
         Plugin configuration. (string) Ex:
-
-        ```python
-        import pulumi
-        ```
-        configuration = <<EOF
-        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
-        kind: Configuration
-        limits:
-        - type: Server
-        burst: 35000
-        qps: 6000
-        EOF
         """
         return pulumi.get(self, "configuration")
 
     @configuration.setter
     def configuration(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "configuration", value)
 
@@ -14077,15 +14072,15 @@
                  ignore_daemon_sets: Optional[pulumi.Input[bool]] = None,
                  timeout: Optional[pulumi.Input[int]] = None):
         """
         :param pulumi.Input[bool] delete_local_data: Delete RKE node local data. Default: `false` (bool)
         :param pulumi.Input[bool] force: Force RKE node drain. Default: `false` (bool)
         :param pulumi.Input[int] grace_period: RKE node drain grace period. Default: `-1` (int)
         :param pulumi.Input[bool] ignore_daemon_sets: Ignore RKE daemon sets. Default: `true` (bool)
-        :param pulumi.Input[int] timeout: Timeout in seconds for etcd backup. Default: `300`. Just for Rancher v2.5.6 and above (int)
+        :param pulumi.Input[int] timeout: Timeout in seconds for etcd backup. Default: `300`. For Rancher v2.5.6 and above (int)
         """
         if delete_local_data is not None:
             pulumi.set(__self__, "delete_local_data", delete_local_data)
         if force is not None:
             pulumi.set(__self__, "force", force)
         if grace_period is not None:
             pulumi.set(__self__, "grace_period", grace_period)
@@ -14142,15 +14137,15 @@
     def ignore_daemon_sets(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ignore_daemon_sets", value)
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[pulumi.Input[int]]:
         """
-        Timeout in seconds for etcd backup. Default: `300`. Just for Rancher v2.5.6 and above (int)
+        Timeout in seconds for etcd backup. Default: `300`. For Rancher v2.5.6 and above (int)
         """
         return pulumi.get(self, "timeout")
 
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout", value)
 
@@ -20186,42 +20181,56 @@
 
 @pulumi.input_type
 class ClusterV2ClusterAgentDeploymentCustomizationArgs:
     def __init__(__self__, *,
                  append_tolerations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationAppendTolerationArgs']]]] = None,
                  override_affinity: Optional[pulumi.Input[str]] = None,
                  override_resource_requirements: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]] = None):
+        """
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationAppendTolerationArgs']]] append_tolerations: User defined tolerations to append to agent (list)
+        :param pulumi.Input[str] override_affinity: User defined affinity to override default agent affinity (string)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs']]] override_resource_requirements: User defined resource requirements to set on the agent (list)
+        """
         if append_tolerations is not None:
             pulumi.set(__self__, "append_tolerations", append_tolerations)
         if override_affinity is not None:
             pulumi.set(__self__, "override_affinity", override_affinity)
         if override_resource_requirements is not None:
             pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
 
     @property
     @pulumi.getter(name="appendTolerations")
     def append_tolerations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationAppendTolerationArgs']]]]:
+        """
+        User defined tolerations to append to agent (list)
+        """
         return pulumi.get(self, "append_tolerations")
 
     @append_tolerations.setter
     def append_tolerations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationAppendTolerationArgs']]]]):
         pulumi.set(self, "append_tolerations", value)
 
     @property
     @pulumi.getter(name="overrideAffinity")
     def override_affinity(self) -> Optional[pulumi.Input[str]]:
+        """
+        User defined affinity to override default agent affinity (string)
+        """
         return pulumi.get(self, "override_affinity")
 
     @override_affinity.setter
     def override_affinity(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "override_affinity", value)
 
     @property
     @pulumi.getter(name="overrideResourceRequirements")
     def override_resource_requirements(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]:
+        """
+        User defined resource requirements to set on the agent (list)
+        """
         return pulumi.get(self, "override_resource_requirements")
 
     @override_resource_requirements.setter
     def override_resource_requirements(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]):
         pulumi.set(self, "override_resource_requirements", value)
 
 
@@ -20230,17 +20239,18 @@
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  effect: Optional[pulumi.Input[str]] = None,
                  operator: Optional[pulumi.Input[str]] = None,
                  seconds: Optional[pulumi.Input[int]] = None,
                  value: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] key: The taint key (string)
-        :param pulumi.Input[str] effect: The taint effect. Default: `\\"NoExecute\\"` (string)
-        :param pulumi.Input[str] operator: Machine selector label match expressions operator (string)
+        :param pulumi.Input[str] key: The toleration key (string)
+        :param pulumi.Input[str] effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param pulumi.Input[str] operator: The toleration operator (string)
+        :param pulumi.Input[int] seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param pulumi.Input[str] value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -20249,49 +20259,52 @@
         if value is not None:
             pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Input[str]:
         """
-        The taint key (string)
+        The toleration key (string)
         """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[pulumi.Input[str]]:
         """
-        The taint effect. Default: `\\"NoExecute\\"` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @effect.setter
     def effect(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "effect", value)
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[pulumi.Input[str]]:
         """
-        Machine selector label match expressions operator (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[pulumi.Input[int]]:
+        """
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
+        """
         return pulumi.get(self, "seconds")
 
     @seconds.setter
     def seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "seconds", value)
 
     @property
@@ -20310,53 +20323,71 @@
 @pulumi.input_type
 class ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs:
     def __init__(__self__, *,
                  cpu_limit: Optional[pulumi.Input[str]] = None,
                  cpu_request: Optional[pulumi.Input[str]] = None,
                  memory_limit: Optional[pulumi.Input[str]] = None,
                  memory_request: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] cpu_limit: The maximum CPU limit for agent (string)
+        :param pulumi.Input[str] cpu_request: The minimum CPU required for agent (string)
+        :param pulumi.Input[str] memory_limit: The maximum memory limit for agent (string)
+        :param pulumi.Input[str] memory_request: The minimum memory required for agent (string)
+        """
         if cpu_limit is not None:
             pulumi.set(__self__, "cpu_limit", cpu_limit)
         if cpu_request is not None:
             pulumi.set(__self__, "cpu_request", cpu_request)
         if memory_limit is not None:
             pulumi.set(__self__, "memory_limit", memory_limit)
         if memory_request is not None:
             pulumi.set(__self__, "memory_request", memory_request)
 
     @property
     @pulumi.getter(name="cpuLimit")
     def cpu_limit(self) -> Optional[pulumi.Input[str]]:
+        """
+        The maximum CPU limit for agent (string)
+        """
         return pulumi.get(self, "cpu_limit")
 
     @cpu_limit.setter
     def cpu_limit(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cpu_limit", value)
 
     @property
     @pulumi.getter(name="cpuRequest")
     def cpu_request(self) -> Optional[pulumi.Input[str]]:
+        """
+        The minimum CPU required for agent (string)
+        """
         return pulumi.get(self, "cpu_request")
 
     @cpu_request.setter
     def cpu_request(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cpu_request", value)
 
     @property
     @pulumi.getter(name="memoryLimit")
     def memory_limit(self) -> Optional[pulumi.Input[str]]:
+        """
+        The maximum memory limit for agent (string)
+        """
         return pulumi.get(self, "memory_limit")
 
     @memory_limit.setter
     def memory_limit(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "memory_limit", value)
 
     @property
     @pulumi.getter(name="memoryRequest")
     def memory_request(self) -> Optional[pulumi.Input[str]]:
+        """
+        The minimum memory required for agent (string)
+        """
         return pulumi.get(self, "memory_request")
 
     @memory_request.setter
     def memory_request(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "memory_request", value)
 
 
@@ -20577,42 +20608,56 @@
 
 @pulumi.input_type
 class ClusterV2FleetAgentDeploymentCustomizationArgs:
     def __init__(__self__, *,
                  append_tolerations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationAppendTolerationArgs']]]] = None,
                  override_affinity: Optional[pulumi.Input[str]] = None,
                  override_resource_requirements: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]] = None):
+        """
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationAppendTolerationArgs']]] append_tolerations: User defined tolerations to append to agent (list)
+        :param pulumi.Input[str] override_affinity: User defined affinity to override default agent affinity (string)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirementArgs']]] override_resource_requirements: User defined resource requirements to set on the agent (list)
+        """
         if append_tolerations is not None:
             pulumi.set(__self__, "append_tolerations", append_tolerations)
         if override_affinity is not None:
             pulumi.set(__self__, "override_affinity", override_affinity)
         if override_resource_requirements is not None:
             pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
 
     @property
     @pulumi.getter(name="appendTolerations")
     def append_tolerations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationAppendTolerationArgs']]]]:
+        """
+        User defined tolerations to append to agent (list)
+        """
         return pulumi.get(self, "append_tolerations")
 
     @append_tolerations.setter
     def append_tolerations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationAppendTolerationArgs']]]]):
         pulumi.set(self, "append_tolerations", value)
 
     @property
     @pulumi.getter(name="overrideAffinity")
     def override_affinity(self) -> Optional[pulumi.Input[str]]:
+        """
+        User defined affinity to override default agent affinity (string)
+        """
         return pulumi.get(self, "override_affinity")
 
     @override_affinity.setter
     def override_affinity(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "override_affinity", value)
 
     @property
     @pulumi.getter(name="overrideResourceRequirements")
     def override_resource_requirements(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]:
+        """
+        User defined resource requirements to set on the agent (list)
+        """
         return pulumi.get(self, "override_resource_requirements")
 
     @override_resource_requirements.setter
     def override_resource_requirements(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]):
         pulumi.set(self, "override_resource_requirements", value)
 
 
@@ -20621,17 +20666,18 @@
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  effect: Optional[pulumi.Input[str]] = None,
                  operator: Optional[pulumi.Input[str]] = None,
                  seconds: Optional[pulumi.Input[int]] = None,
                  value: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] key: The taint key (string)
-        :param pulumi.Input[str] effect: The taint effect. Default: `\\"NoExecute\\"` (string)
-        :param pulumi.Input[str] operator: Machine selector label match expressions operator (string)
+        :param pulumi.Input[str] key: The toleration key (string)
+        :param pulumi.Input[str] effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param pulumi.Input[str] operator: The toleration operator (string)
+        :param pulumi.Input[int] seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param pulumi.Input[str] value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -20640,49 +20686,52 @@
         if value is not None:
             pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Input[str]:
         """
-        The taint key (string)
+        The toleration key (string)
         """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[pulumi.Input[str]]:
         """
-        The taint effect. Default: `\\"NoExecute\\"` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @effect.setter
     def effect(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "effect", value)
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[pulumi.Input[str]]:
         """
-        Machine selector label match expressions operator (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[pulumi.Input[int]]:
+        """
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
+        """
         return pulumi.get(self, "seconds")
 
     @seconds.setter
     def seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "seconds", value)
 
     @property
@@ -20701,53 +20750,71 @@
 @pulumi.input_type
 class ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirementArgs:
     def __init__(__self__, *,
                  cpu_limit: Optional[pulumi.Input[str]] = None,
                  cpu_request: Optional[pulumi.Input[str]] = None,
                  memory_limit: Optional[pulumi.Input[str]] = None,
                  memory_request: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] cpu_limit: The maximum CPU limit for agent (string)
+        :param pulumi.Input[str] cpu_request: The minimum CPU required for agent (string)
+        :param pulumi.Input[str] memory_limit: The maximum memory limit for agent (string)
+        :param pulumi.Input[str] memory_request: The minimum memory required for agent (string)
+        """
         if cpu_limit is not None:
             pulumi.set(__self__, "cpu_limit", cpu_limit)
         if cpu_request is not None:
             pulumi.set(__self__, "cpu_request", cpu_request)
         if memory_limit is not None:
             pulumi.set(__self__, "memory_limit", memory_limit)
         if memory_request is not None:
             pulumi.set(__self__, "memory_request", memory_request)
 
     @property
     @pulumi.getter(name="cpuLimit")
     def cpu_limit(self) -> Optional[pulumi.Input[str]]:
+        """
+        The maximum CPU limit for agent (string)
+        """
         return pulumi.get(self, "cpu_limit")
 
     @cpu_limit.setter
     def cpu_limit(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cpu_limit", value)
 
     @property
     @pulumi.getter(name="cpuRequest")
     def cpu_request(self) -> Optional[pulumi.Input[str]]:
+        """
+        The minimum CPU required for agent (string)
+        """
         return pulumi.get(self, "cpu_request")
 
     @cpu_request.setter
     def cpu_request(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cpu_request", value)
 
     @property
     @pulumi.getter(name="memoryLimit")
     def memory_limit(self) -> Optional[pulumi.Input[str]]:
+        """
+        The maximum memory limit for agent (string)
+        """
         return pulumi.get(self, "memory_limit")
 
     @memory_limit.setter
     def memory_limit(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "memory_limit", value)
 
     @property
     @pulumi.getter(name="memoryRequest")
     def memory_request(self) -> Optional[pulumi.Input[str]]:
+        """
+        The minimum memory required for agent (string)
+        """
         return pulumi.get(self, "memory_request")
 
     @memory_request.setter
     def memory_request(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "memory_request", value)
 
 
@@ -20928,14 +20995,17 @@
 
     @property
     @pulumi.getter(name="localAuthEndpoint")
     def local_auth_endpoint(self) -> Optional[pulumi.Input['ClusterV2RkeConfigLocalAuthEndpointArgs']]:
         """
         Cluster V2 local auth endpoint (list maxitems:1)
         """
+        warnings.warn("""Use rancher2_cluster_v2.local_auth_endpoint instead""", DeprecationWarning)
+        pulumi.log.warn("""local_auth_endpoint is deprecated: Use rancher2_cluster_v2.local_auth_endpoint instead""")
+
         return pulumi.get(self, "local_auth_endpoint")
 
     @local_auth_endpoint.setter
     def local_auth_endpoint(self, value: Optional[pulumi.Input['ClusterV2RkeConfigLocalAuthEndpointArgs']]):
         pulumi.set(self, "local_auth_endpoint", value)
 
     @property
@@ -21755,28 +21825,28 @@
 @pulumi.input_type
 class ClusterV2RkeConfigMachinePoolTaintArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  value: pulumi.Input[str],
                  effect: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] key: The taint key (string)
+        :param pulumi.Input[str] key: The toleration key (string)
         :param pulumi.Input[str] value: Rancher agent env var value (string)
-        :param pulumi.Input[str] effect: The taint effect. Default: `\\"NoExecute\\"` (string)
+        :param pulumi.Input[str] effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "value", value)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Input[str]:
         """
-        The taint key (string)
+        The toleration key (string)
         """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
@@ -21792,15 +21862,15 @@
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[pulumi.Input[str]]:
         """
-        The taint effect. Default: `\\"NoExecute\\"` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @effect.setter
     def effect(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "effect", value)
 
@@ -21886,42 +21956,42 @@
 @pulumi.input_type
 class ClusterV2RkeConfigMachineSelectorConfigMachineLabelSelectorMatchExpressionArgs:
     def __init__(__self__, *,
                  key: Optional[pulumi.Input[str]] = None,
                  operator: Optional[pulumi.Input[str]] = None,
                  values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        :param pulumi.Input[str] key: The taint key (string)
-        :param pulumi.Input[str] operator: Machine selector label match expressions operator (string)
+        :param pulumi.Input[str] key: The toleration key (string)
+        :param pulumi.Input[str] operator: The toleration operator (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] values: Machine selector label match expressions values (List string)
         """
         if key is not None:
             pulumi.set(__self__, "key", key)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
         if values is not None:
             pulumi.set(__self__, "values", values)
 
     @property
     @pulumi.getter
     def key(self) -> Optional[pulumi.Input[str]]:
         """
-        The taint key (string)
+        The toleration key (string)
         """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[pulumi.Input[str]]:
         """
-        Machine selector label match expressions operator (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "operator", value)
 
@@ -23609,22 +23679,22 @@
                  vnet: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] availability_set: Azure Availability Set to place the virtual machine into. Default `docker-machine` (string)
         :param pulumi.Input[str] availability_zone: OpenStack availability zone (string)
         :param pulumi.Input[str] client_id: Azure Service Principal Account ID. Mandatory on Rancher v2.0.x and v2.1.x. Use `CloudCredential` from Rancher v2.2.x (string)
         :param pulumi.Input[str] client_secret: Azure Service Principal Account password. Mandatory on Rancher v2.0.x and v2.1.x. Use `CloudCredential` from Rancher v2.2.x (string)
         :param pulumi.Input[str] custom_data: Path to file with custom-data (string)
-        :param pulumi.Input[str] disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        :param pulumi.Input[str] disk_size: Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         :param pulumi.Input[str] dns: A unique DNS label for the public IP adddress (string)
         :param pulumi.Input[str] docker_port: Port number for Docker engine. Default `2376` (string)
         :param pulumi.Input[str] environment: Azure environment (e.g. AzurePublicCloud, AzureChinaCloud). Default `AzurePublicCloud` (string)
         :param pulumi.Input[str] fault_domain_count: Fault domain count to use for availability set. Default `3` (string)
         :param pulumi.Input[str] image: Azure virtual machine OS image. Default `canonical:UbuntuServer:18.04-LTS:latest` (string)
         :param pulumi.Input[str] location: Azure region to create the virtual machine. Default `westus` (string)
-        :param pulumi.Input[bool] managed_disks: Configures VM and availability set for managed disks. Just for Rancher v2.3.x and above. Default `false` (bool)
+        :param pulumi.Input[bool] managed_disks: Configures VM and availability set for managed disks. For Rancher v2.3.x and above. Default `false` (bool)
         :param pulumi.Input[bool] no_public_ip: Do not create a public IP address for the machine. Default `false` (bool)
         :param pulumi.Input[str] nsg: Azure Network Security Group to assign this node to (accepts either a name or resource ID, default is to create a new NSG for each machine). Default `docker-machine-nsg` (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] open_ports: Make the specified port number accessible from the Internet. (list)
         :param pulumi.Input[bool] private_address_only: Only use a private IP address. Default `false` (bool)
         :param pulumi.Input[str] private_ip_address: Specify a static private IP address for the machine. (string)
         :param pulumi.Input[str] resource_group: Azure Resource Group name (will be created if missing). Default `docker-machine` (string)
         :param pulumi.Input[str] size: Size for Azure Virtual Machine. Default `Standard_A2` (string)
@@ -23776,15 +23846,15 @@
     def custom_data(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_data", value)
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[pulumi.Input[str]]:
         """
-        Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         """
         return pulumi.get(self, "disk_size")
 
     @disk_size.setter
     def disk_size(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_size", value)
 
@@ -23860,15 +23930,15 @@
     def location(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "location", value)
 
     @property
     @pulumi.getter(name="managedDisks")
     def managed_disks(self) -> Optional[pulumi.Input[bool]]:
         """
-        Configures VM and availability set for managed disks. Just for Rancher v2.3.x and above. Default `false` (bool)
+        Configures VM and availability set for managed disks. For Rancher v2.3.x and above. Default `false` (bool)
         """
         return pulumi.get(self, "managed_disks")
 
     @managed_disks.setter
     def managed_disks(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "managed_disks", value)
 
@@ -24349,24 +24419,24 @@
                  vm_affinity: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] ssh_user: Set the name of the ssh user (string)
         :param pulumi.Input[str] vm_namespace: Virtual machine namespace e.g. `default` (string)
         :param pulumi.Input[str] cpu_count: CPU count, Default `2` (string)
         :param pulumi.Input[str] disk_bus: Use `disk_info` instead
         :param pulumi.Input[str] disk_info: A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
-        :param pulumi.Input[str] disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        :param pulumi.Input[str] disk_size: Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         :param pulumi.Input[str] image_name: Use `disk_info` instead
         :param pulumi.Input[str] memory_size: Memory size (in GiB), Default `4` (string)
         :param pulumi.Input[str] network_data: NetworkData content of cloud-init, base64 is supported (string)
         :param pulumi.Input[str] network_info: A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
         :param pulumi.Input[str] network_model: Use `network_info` instead
         :param pulumi.Input[str] network_name: Use `network_info` instead
         :param pulumi.Input[str] ssh_password: SSH password (string)
         :param pulumi.Input[str] user_data: UserData content of cloud-init, base64 is supported. If the image does not contain the qemu-guest-agent package, you must install and start qemu-guest-agent using userdata (string)
-        :param pulumi.Input[str] vm_affinity: Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 or above (string)
+        :param pulumi.Input[str] vm_affinity: Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 and above (string)
         """
         pulumi.set(__self__, "ssh_user", ssh_user)
         pulumi.set(__self__, "vm_namespace", vm_namespace)
         if cpu_count is not None:
             pulumi.set(__self__, "cpu_count", cpu_count)
         if disk_bus is not None:
             warnings.warn("""Use disk_info instead""", DeprecationWarning)
@@ -24446,14 +24516,17 @@
 
     @property
     @pulumi.getter(name="diskBus")
     def disk_bus(self) -> Optional[pulumi.Input[str]]:
         """
         Use `disk_info` instead
         """
+        warnings.warn("""Use disk_info instead""", DeprecationWarning)
+        pulumi.log.warn("""disk_bus is deprecated: Use disk_info instead""")
+
         return pulumi.get(self, "disk_bus")
 
     @disk_bus.setter
     def disk_bus(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_bus", value)
 
     @property
@@ -24468,28 +24541,34 @@
     def disk_info(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_info", value)
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[pulumi.Input[str]]:
         """
-        Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         """
+        warnings.warn("""Use disk_info instead""", DeprecationWarning)
+        pulumi.log.warn("""disk_size is deprecated: Use disk_info instead""")
+
         return pulumi.get(self, "disk_size")
 
     @disk_size.setter
     def disk_size(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_size", value)
 
     @property
     @pulumi.getter(name="imageName")
     def image_name(self) -> Optional[pulumi.Input[str]]:
         """
         Use `disk_info` instead
         """
+        warnings.warn("""Use disk_info instead""", DeprecationWarning)
+        pulumi.log.warn("""image_name is deprecated: Use disk_info instead""")
+
         return pulumi.get(self, "image_name")
 
     @image_name.setter
     def image_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image_name", value)
 
     @property
@@ -24530,26 +24609,32 @@
 
     @property
     @pulumi.getter(name="networkModel")
     def network_model(self) -> Optional[pulumi.Input[str]]:
         """
         Use `network_info` instead
         """
+        warnings.warn("""Use network_info instead""", DeprecationWarning)
+        pulumi.log.warn("""network_model is deprecated: Use network_info instead""")
+
         return pulumi.get(self, "network_model")
 
     @network_model.setter
     def network_model(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_model", value)
 
     @property
     @pulumi.getter(name="networkName")
     def network_name(self) -> Optional[pulumi.Input[str]]:
         """
         Use `network_info` instead
         """
+        warnings.warn("""Use network_info instead""", DeprecationWarning)
+        pulumi.log.warn("""network_name is deprecated: Use network_info instead""")
+
         return pulumi.get(self, "network_name")
 
     @network_name.setter
     def network_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_name", value)
 
     @property
@@ -24576,15 +24661,15 @@
     def user_data(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_data", value)
 
     @property
     @pulumi.getter(name="vmAffinity")
     def vm_affinity(self) -> Optional[pulumi.Input[str]]:
         """
-        Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 or above (string)
+        Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 and above (string)
         """
         return pulumi.get(self, "vm_affinity")
 
     @vm_affinity.setter
     def vm_affinity(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vm_affinity", value)
 
@@ -24932,16 +25017,16 @@
         :param pulumi.Input[str] tenant_id: Azure Tenant ID (string)
         :param pulumi.Input[str] tenant_name: OpenStack tenant name. Conflicts with `tenant_id` (string)
         :param pulumi.Input[str] user_data_file: File containing an openstack userdata script (string)
         :param pulumi.Input[str] user_domain_id: OpenStack user domain id. Conflicts with `user_domain_name` (string)
         :param pulumi.Input[str] user_domain_name: OpenStack user domain name. Conflicts with `user_domain_id` (string)
         :param pulumi.Input[str] username: OpenStack username (string)
         :param pulumi.Input[str] volume_device_path: OpenStack volume device path (attaching). Applicable only when `boot_from_volume` is `true`. Omit for auto `/dev/vdb`. (string)
-               > **Note**: `Required+` denotes that either the _name or _id is required but you cannot use both.
-               > **Note**: `Required++` denotes that either the _name or _id is required unless `application_credential_id` is defined.
+               > **Note:**: `Required+` denotes that either the _name or _id is required but you cannot use both.
+               > **Note:**: `Required++` denotes that either the _name or _id is required unless `application_credential_id` is defined.
         :param pulumi.Input[str] volume_id: OpenStack volume id of existing volume. Applicable only when `boot_from_volume` is `true` (string)
         :param pulumi.Input[str] volume_name: OpenStack volume name of existing volume. Applicable only when `boot_from_volume` is `true` (string)
         :param pulumi.Input[str] volume_size: OpenStack volume size (GiB). Required when `boot_from_volume` is `true` (string)
         :param pulumi.Input[str] volume_type: Amazon EBS volume type. Default `gp2` (string)
         """
         pulumi.set(__self__, "auth_url", auth_url)
         pulumi.set(__self__, "availability_zone", availability_zone)
@@ -25470,16 +25555,16 @@
         pulumi.set(self, "username", value)
 
     @property
     @pulumi.getter(name="volumeDevicePath")
     def volume_device_path(self) -> Optional[pulumi.Input[str]]:
         """
         OpenStack volume device path (attaching). Applicable only when `boot_from_volume` is `true`. Omit for auto `/dev/vdb`. (string)
-        > **Note**: `Required+` denotes that either the _name or _id is required but you cannot use both.
-        > **Note**: `Required++` denotes that either the _name or _id is required unless `application_credential_id` is defined.
+        > **Note:**: `Required+` denotes that either the _name or _id is required but you cannot use both.
+        > **Note:**: `Required++` denotes that either the _name or _id is required unless `application_credential_id` is defined.
         """
         return pulumi.get(self, "volume_device_path")
 
     @volume_device_path.setter
     def volume_device_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "volume_device_path", value)
 
@@ -25575,15 +25660,15 @@
         :param pulumi.Input[str] content_library: If you choose to clone from a content library template specify the name of the library (string)
         :param pulumi.Input[str] cpu_count: CPU count, Default `2` (string)
         :param pulumi.Input[str] creation_type: Creation type when creating a new virtual machine. Supported values: vm, template, library, legacy. Default `legacy` (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_attributes: vSphere custom attributes, format key/value e.g. `200=my custom value` (List)
         :param pulumi.Input[str] datacenter: vSphere datacenter for docker VM (string)
         :param pulumi.Input[str] datastore: vSphere datastore for docker VM (string)
         :param pulumi.Input[str] datastore_cluster: vSphere datastore cluster for virtual machine (string)
-        :param pulumi.Input[str] disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        :param pulumi.Input[str] disk_size: Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         :param pulumi.Input[str] folder: vSphere folder for the docker VM. This folder must already exist in the datacenter (string)
         :param pulumi.Input[str] hostsystem: vSphere compute resource where the docker VM will be instantiated. This can be omitted if using a cluster with DRS (string)
         :param pulumi.Input[str] memory_size: Memory size (in GiB), Default `4` (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] networks: vSphere network where the docker VM will be attached (list)
         :param pulumi.Input[str] password: OpenStack password. Mandatory on Rancher v2.0.x and v2.1.x. Use `CloudCredential` from Rancher v2.2.x (string)
         :param pulumi.Input[str] pool: vSphere resource pool for docker VM (string)
         :param pulumi.Input[str] ssh_password: SSH password (string)
@@ -25806,15 +25891,15 @@
     def datastore_cluster(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_cluster", value)
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[pulumi.Input[str]]:
         """
-        Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         """
         return pulumi.get(self, "disk_size")
 
     @disk_size.setter
     def disk_size(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_size", value)
 
@@ -26723,15 +26808,15 @@
         :param pulumi.Input[str] spot_price: AWS spot instance bid price (in dollar). Default `0.50` (string)
         :param pulumi.Input[str] ssh_user: Set the name of the ssh user (string)
         :param pulumi.Input[str] tags: AWS Tags (e.g. key1,value1,key2,value2) (string)
         :param pulumi.Input[bool] use_ebs_optimized_instance: Create an EBS optimized instance. Default `false` (bool)
         :param pulumi.Input[bool] use_private_address: Force the usage of private IP address. Default `false` (bool)
         :param pulumi.Input[str] userdata: Path to file with cloud-init user data (string)
                
-               > **Note**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
+               > **Note:**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
         :param pulumi.Input[str] volume_type: Amazon EBS volume type. Default `gp2` (string)
         """
         pulumi.set(__self__, "ami", ami)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "security_groups", security_groups)
         pulumi.set(__self__, "subnet_id", subnet_id)
         pulumi.set(__self__, "vpc_id", vpc_id)
@@ -27190,15 +27275,15 @@
 
     @property
     @pulumi.getter
     def userdata(self) -> Optional[pulumi.Input[str]]:
         """
         Path to file with cloud-init user data (string)
 
-        > **Note**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
+        > **Note:**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
         """
         return pulumi.get(self, "userdata")
 
     @userdata.setter
     def userdata(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "userdata", value)
 
@@ -27252,26 +27337,26 @@
                  vnet: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] availability_set: Azure Availability Set to place the virtual machine into. Default `docker-machine` (string)
         :param pulumi.Input[str] availability_zone: OpenStack availability zone (string)
         :param pulumi.Input[str] client_id: Azure Service Principal Account ID. Mandatory on Rancher v2.0.x and v2.1.x. Use `CloudCredential` from Rancher v2.2.x (string)
         :param pulumi.Input[str] client_secret: Azure Service Principal Account password. Mandatory on Rancher v2.0.x and v2.1.x. Use `CloudCredential` from Rancher v2.2.x (string)
         :param pulumi.Input[str] custom_data: Path to file with custom-data (string)
-        :param pulumi.Input[str] disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        :param pulumi.Input[str] disk_size: Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         :param pulumi.Input[str] dns: A unique DNS label for the public IP adddress (string)
         :param pulumi.Input[str] docker_port: Port number for Docker engine. Default `2376` (string)
         :param pulumi.Input[str] environment: Azure environment (e.g. AzurePublicCloud, AzureChinaCloud). Default `AzurePublicCloud` (string)
         :param pulumi.Input[str] fault_domain_count: Fault domain count to use for availability set. Default `3` (string)
         :param pulumi.Input[str] image: Azure virtual machine OS image. Default `canonical:UbuntuServer:18.04-LTS:latest` (string)
         :param pulumi.Input[str] location: Azure region to create the virtual machine. Default `westus` (string)
-        :param pulumi.Input[bool] managed_disks: Configures VM and availability set for managed disks. Just for Rancher v2.3.x and above. Default `false` (bool)
+        :param pulumi.Input[bool] managed_disks: Configures VM and availability set for managed disks. For Rancher v2.3.x and above. Default `false` (bool)
         :param pulumi.Input[bool] no_public_ip: Do not create a public IP address for the machine. Default `false` (bool)
         :param pulumi.Input[str] nsg: Azure Network Security Group to assign this node to (accepts either a name or resource ID, default is to create a new NSG for each machine). Default `docker-machine-nsg` (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] open_ports: Make the specified port number accessible from the Internet. (list)
-        :param pulumi.Input[str] plan: Azure marketplace purchase plan for Azure Virtual Machine. Format is `<publisher>:<product>:<plan>`. Just for Rancher v2.6.3 and above. (string)
+        :param pulumi.Input[str] plan: Azure marketplace purchase plan for Azure Virtual Machine. Format is `<publisher>:<product>:<plan>`. For Rancher v2.6.3 and above. (string)
         :param pulumi.Input[str] private_ip_address: Specify a static private IP address for the machine. (string)
         :param pulumi.Input[str] resource_group: Azure Resource Group name (will be created if missing). Default `docker-machine` (string)
         :param pulumi.Input[str] size: Size for Azure Virtual Machine. Default `Standard_A2` (string)
         :param pulumi.Input[str] ssh_user: Set the name of the ssh user (string)
         :param pulumi.Input[bool] static_public_ip: Assign a static public IP address to the machine. Default `false` (bool)
         :param pulumi.Input[str] storage_type: Type of Storage Account to host the OS Disk for the machine. Default `Standard_LRS` (string)
         :param pulumi.Input[str] subnet: Azure Subnet Name to be used within the Virtual Network. Default `docker-machine` (string)
@@ -27416,15 +27501,15 @@
     def custom_data(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_data", value)
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[pulumi.Input[str]]:
         """
-        Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         """
         return pulumi.get(self, "disk_size")
 
     @disk_size.setter
     def disk_size(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_size", value)
 
@@ -27500,15 +27585,15 @@
     def location(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "location", value)
 
     @property
     @pulumi.getter(name="managedDisks")
     def managed_disks(self) -> Optional[pulumi.Input[bool]]:
         """
-        Configures VM and availability set for managed disks. Just for Rancher v2.3.x and above. Default `false` (bool)
+        Configures VM and availability set for managed disks. For Rancher v2.3.x and above. Default `false` (bool)
         """
         return pulumi.get(self, "managed_disks")
 
     @managed_disks.setter
     def managed_disks(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "managed_disks", value)
 
@@ -27548,15 +27633,15 @@
     def open_ports(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "open_ports", value)
 
     @property
     @pulumi.getter
     def plan(self) -> Optional[pulumi.Input[str]]:
         """
-        Azure marketplace purchase plan for Azure Virtual Machine. Format is `<publisher>:<product>:<plan>`. Just for Rancher v2.6.3 and above. (string)
+        Azure marketplace purchase plan for Azure Virtual Machine. Format is `<publisher>:<product>:<plan>`. For Rancher v2.6.3 and above. (string)
         """
         return pulumi.get(self, "plan")
 
     @plan.setter
     def plan(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plan", value)
 
@@ -27755,15 +27840,15 @@
         :param pulumi.Input[str] ssh_key_fingerprint: SSH key fingerprint (string)
         :param pulumi.Input[str] ssh_key_path: SSH private key path (string)
         :param pulumi.Input[str] ssh_port: SSH port. Default `22` (string)
         :param pulumi.Input[str] ssh_user: Set the name of the ssh user (string)
         :param pulumi.Input[str] tags: AWS Tags (e.g. key1,value1,key2,value2) (string)
         :param pulumi.Input[str] userdata: Path to file with cloud-init user data (string)
                
-               > **Note**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
+               > **Note:**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
         """
         if access_token is not None:
             pulumi.set(__self__, "access_token", access_token)
         if backups is not None:
             pulumi.set(__self__, "backups", backups)
         if image is not None:
             pulumi.set(__self__, "image", image)
@@ -27948,15 +28033,15 @@
 
     @property
     @pulumi.getter
     def userdata(self) -> Optional[pulumi.Input[str]]:
         """
         Path to file with cloud-init user data (string)
 
-        > **Note**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
+        > **Note:**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
         """
         return pulumi.get(self, "userdata")
 
     @userdata.setter
     def userdata(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "userdata", value)
 
@@ -27981,24 +28066,24 @@
                  vm_affinity: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] ssh_user: Set the name of the ssh user (string)
         :param pulumi.Input[str] vm_namespace: Virtual machine namespace e.g. `default` (string)
         :param pulumi.Input[str] cpu_count: CPU count, Default `2` (string)
         :param pulumi.Input[str] disk_bus: Use `disk_info` instead
         :param pulumi.Input[str] disk_info: A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
-        :param pulumi.Input[str] disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        :param pulumi.Input[str] disk_size: Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         :param pulumi.Input[str] image_name: Use `disk_info` instead
         :param pulumi.Input[str] memory_size: Memory size (in GiB), Default `4` (string)
         :param pulumi.Input[str] network_data: NetworkData content of cloud-init, base64 is supported (string)
         :param pulumi.Input[str] network_info: A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
         :param pulumi.Input[str] network_model: Use `network_info` instead
         :param pulumi.Input[str] network_name: Use `network_info` instead
         :param pulumi.Input[str] ssh_password: SSH password (string)
         :param pulumi.Input[str] user_data: UserData content of cloud-init, base64 is supported. If the image does not contain the qemu-guest-agent package, you must install and start qemu-guest-agent using userdata (string)
-        :param pulumi.Input[str] vm_affinity: Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 or above (string)
+        :param pulumi.Input[str] vm_affinity: Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 and above (string)
         """
         pulumi.set(__self__, "ssh_user", ssh_user)
         pulumi.set(__self__, "vm_namespace", vm_namespace)
         if cpu_count is not None:
             pulumi.set(__self__, "cpu_count", cpu_count)
         if disk_bus is not None:
             warnings.warn("""Use disk_info instead""", DeprecationWarning)
@@ -28078,14 +28163,17 @@
 
     @property
     @pulumi.getter(name="diskBus")
     def disk_bus(self) -> Optional[pulumi.Input[str]]:
         """
         Use `disk_info` instead
         """
+        warnings.warn("""Use disk_info instead""", DeprecationWarning)
+        pulumi.log.warn("""disk_bus is deprecated: Use disk_info instead""")
+
         return pulumi.get(self, "disk_bus")
 
     @disk_bus.setter
     def disk_bus(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_bus", value)
 
     @property
@@ -28100,28 +28188,34 @@
     def disk_info(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_info", value)
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[pulumi.Input[str]]:
         """
-        Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         """
+        warnings.warn("""Use disk_info instead""", DeprecationWarning)
+        pulumi.log.warn("""disk_size is deprecated: Use disk_info instead""")
+
         return pulumi.get(self, "disk_size")
 
     @disk_size.setter
     def disk_size(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_size", value)
 
     @property
     @pulumi.getter(name="imageName")
     def image_name(self) -> Optional[pulumi.Input[str]]:
         """
         Use `disk_info` instead
         """
+        warnings.warn("""Use disk_info instead""", DeprecationWarning)
+        pulumi.log.warn("""image_name is deprecated: Use disk_info instead""")
+
         return pulumi.get(self, "image_name")
 
     @image_name.setter
     def image_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image_name", value)
 
     @property
@@ -28162,26 +28256,32 @@
 
     @property
     @pulumi.getter(name="networkModel")
     def network_model(self) -> Optional[pulumi.Input[str]]:
         """
         Use `network_info` instead
         """
+        warnings.warn("""Use network_info instead""", DeprecationWarning)
+        pulumi.log.warn("""network_model is deprecated: Use network_info instead""")
+
         return pulumi.get(self, "network_model")
 
     @network_model.setter
     def network_model(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_model", value)
 
     @property
     @pulumi.getter(name="networkName")
     def network_name(self) -> Optional[pulumi.Input[str]]:
         """
         Use `network_info` instead
         """
+        warnings.warn("""Use network_info instead""", DeprecationWarning)
+        pulumi.log.warn("""network_name is deprecated: Use network_info instead""")
+
         return pulumi.get(self, "network_name")
 
     @network_name.setter
     def network_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_name", value)
 
     @property
@@ -28208,15 +28308,15 @@
     def user_data(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_data", value)
 
     @property
     @pulumi.getter(name="vmAffinity")
     def vm_affinity(self) -> Optional[pulumi.Input[str]]:
         """
-        Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 or above (string)
+        Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 and above (string)
         """
         return pulumi.get(self, "vm_affinity")
 
     @vm_affinity.setter
     def vm_affinity(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vm_affinity", value)
 
@@ -28239,15 +28339,15 @@
         :param pulumi.Input[str] networks: Comma-separated list of network IDs or names which should be attached to the server private network interface (string)
         :param pulumi.Input[Mapping[str, Any]] server_labels: Map of the labels which will be assigned to the server. This argument is only available on [Hetzner Docker Node Driver:v3.6.0](https://github.com/JonasProgrammer/docker-machine-driver-hetzner/releases/tag/3.6.0) and above (map)
         :param pulumi.Input[str] server_location: Hetzner Cloud datacenter. Default `nbg1` (string)
         :param pulumi.Input[str] server_type: Hetzner Cloud server type. Default `cx11` (string)
         :param pulumi.Input[bool] use_private_network: Use private network. Default `false` (bool)
         :param pulumi.Input[str] userdata: Path to file with cloud-init user data (string)
                
-               > **Note**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
+               > **Note:**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
         :param pulumi.Input[str] volumes: Comma-separated list of volume IDs or names which should be attached to the server (string)
         """
         pulumi.set(__self__, "api_token", api_token)
         if image is not None:
             pulumi.set(__self__, "image", image)
         if networks is not None:
             pulumi.set(__self__, "networks", networks)
@@ -28350,15 +28450,15 @@
 
     @property
     @pulumi.getter
     def userdata(self) -> Optional[pulumi.Input[str]]:
         """
         Path to file with cloud-init user data (string)
 
-        > **Note**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
+        > **Note:**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
         """
         return pulumi.get(self, "userdata")
 
     @userdata.setter
     def userdata(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "userdata", value)
 
@@ -28746,15 +28846,15 @@
         :param pulumi.Input[str] network_name: Use `network_info` instead
         :param pulumi.Input[str] network_owner: Opennebula user ID of the Network to connect the machine to (string)
         :param pulumi.Input[str] ssh_user: Set the name of the ssh user (string)
         :param pulumi.Input[str] template_id: Opennebula template ID to use. Conflicts with `template_name` (string)
         :param pulumi.Input[str] template_name: Name of the Opennbula template to use. Conflicts with `template_id` (string)
         :param pulumi.Input[str] vcpu: VCPUs for the VM (string)
                
-               > **Note**: `Required*` denotes that one of image_name / image_id or template_name / template_id is required but you cannot combine them.
+               > **Note:**: `Required*` denotes that one of image_name / image_id or template_name / template_id is required but you cannot combine them.
         """
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "user", user)
         pulumi.set(__self__, "xml_rpc_url", xml_rpc_url)
         if b2d_size is not None:
             pulumi.set(__self__, "b2d_size", b2d_size)
         if cpu is not None:
@@ -29006,15 +29106,15 @@
 
     @property
     @pulumi.getter
     def vcpu(self) -> Optional[pulumi.Input[str]]:
         """
         VCPUs for the VM (string)
 
-        > **Note**: `Required*` denotes that one of image_name / image_id or template_name / template_id is required but you cannot combine them.
+        > **Note:**: `Required*` denotes that one of image_name / image_id or template_name / template_id is required but you cannot combine them.
         """
         return pulumi.get(self, "vcpu")
 
     @vcpu.setter
     def vcpu(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vcpu", value)
 
@@ -29092,17 +29192,17 @@
         :param pulumi.Input[str] ssh_user: Set the name of the ssh user (string)
         :param pulumi.Input[str] tenant_id: OpenStack tenant id. Conflicts with `tenant_name` (string)
         :param pulumi.Input[str] tenant_name: OpenStack tenant name. Conflicts with `tenant_id` (string)
         :param pulumi.Input[str] user_data_file: File containing an openstack userdata script (string)
         :param pulumi.Input[str] username: OpenStack username (string)
         :param pulumi.Input[str] volume_device_path: OpenStack volume device path (attaching). Applicable only when `boot_from_volume` is `true`. Omit for auto `/dev/vdb`. (string)
                
-               > **Note**: `Required*` denotes that either the _name or _id is required but you cannot use both.
+               > **Note:**: `Required*` denotes that either the _name or _id is required but you cannot use both.
                
-               > **Note**: `Required**` denotes that either the _name or _id is required unless `application_credential_id` is defined.
+               > **Note:**: `Required**` denotes that either the _name or _id is required unless `application_credential_id` is defined.
         :param pulumi.Input[str] volume_id: OpenStack volume id of existing volume. Applicable only when `boot_from_volume` is `true` (string)
         :param pulumi.Input[str] volume_name: OpenStack volume name of existing volume. Applicable only when `boot_from_volume` is `true` (string)
         :param pulumi.Input[str] volume_size: OpenStack volume size (GiB). Required when `boot_from_volume` is `true` (string)
         :param pulumi.Input[str] volume_type: Amazon EBS volume type. Default `gp2` (string)
         """
         pulumi.set(__self__, "auth_url", auth_url)
         pulumi.set(__self__, "availability_zone", availability_zone)
@@ -29576,17 +29676,17 @@
 
     @property
     @pulumi.getter(name="volumeDevicePath")
     def volume_device_path(self) -> Optional[pulumi.Input[str]]:
         """
         OpenStack volume device path (attaching). Applicable only when `boot_from_volume` is `true`. Omit for auto `/dev/vdb`. (string)
 
-        > **Note**: `Required*` denotes that either the _name or _id is required but you cannot use both.
+        > **Note:**: `Required*` denotes that either the _name or _id is required but you cannot use both.
 
-        > **Note**: `Required**` denotes that either the _name or _id is required unless `application_credential_id` is defined.
+        > **Note:**: `Required**` denotes that either the _name or _id is required unless `application_credential_id` is defined.
         """
         return pulumi.get(self, "volume_device_path")
 
     @volume_device_path.setter
     def volume_device_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "volume_device_path", value)
 
@@ -29863,15 +29963,15 @@
         :param pulumi.Input[str] content_library: If you choose to clone from a content library template specify the name of the library. From Rancher v2.3.3 (string)
         :param pulumi.Input[str] cpu_count: CPU count, Default `2` (string)
         :param pulumi.Input[str] creation_type: Creation type when creating a new virtual machine. Supported values: vm, template, library, legacy. Default `legacy`. From Rancher v2.3.3 (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_attributes: vSphere custom attributes, format key/value e.g. `200=my custom value`. From Rancher v2.3.3 (List)
         :param pulumi.Input[str] datacenter: vSphere datacenter for docker VM (string)
         :param pulumi.Input[str] datastore: vSphere datastore for docker VM (string)
         :param pulumi.Input[str] datastore_cluster: vSphere datastore cluster for virtual machine. From Rancher v2.3.3 (string)
-        :param pulumi.Input[str] disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        :param pulumi.Input[str] disk_size: Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         :param pulumi.Input[str] folder: vSphere folder for the docker VM. This folder must already exist in the datacenter (string)
         :param pulumi.Input[str] hostsystem: vSphere compute resource where the docker VM will be instantiated. This can be omitted if using a cluster with DRS (string)
         :param pulumi.Input[str] memory_size: Memory size (in GiB), Default `4` (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] networks: vSphere network where the docker VM will be attached (list)
         :param pulumi.Input[str] password: Set the password for the XML-RPC API authentication (string)
         :param pulumi.Input[str] pool: vSphere resource pool for docker VM (string)
         :param pulumi.Input[str] ssh_password: SSH password (string)
@@ -30094,15 +30194,15 @@
     def datastore_cluster(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_cluster", value)
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[pulumi.Input[str]]:
         """
-        Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         """
         return pulumi.get(self, "disk_size")
 
     @disk_size.setter
     def disk_size(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_size", value)
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/_utilities.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/active_directory.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/active_directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/app.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/app_v2.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/app_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_active_directory.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_active_directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_adfs.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_adfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_azure_ad.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_free_ipa.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_free_ipa.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_github.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_keycloak.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_keycloak.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_okta.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_okta.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_open_ldap.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_open_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/auth_config_ping.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/auth_config_ping.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         :param pulumi.Input[str] sp_key: Ping SP key (string)
         :param pulumi.Input[str] uid_field: Ping UID field (string)
         :param pulumi.Input[str] user_name_field: Ping user name field (string)
         :param pulumi.Input[str] access_mode: Access mode for auth. `required`, `restricted`, `unrestricted` are supported. Default `unrestricted` (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_principal_ids: Allowed principal ids for auth. Required if `access_mode` is `required` or `restricted`. Ex: `ping_user://<USER_ID>`  `ping_group://<GROUP_ID>` (list)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations of the resource (map)
         :param pulumi.Input[bool] enabled: Enable auth config provider. Default `true` (bool)
+        :param pulumi.Input[str] entity_id_field: Ping entity ID field (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels of the resource (map)
         """
         pulumi.set(__self__, "display_name_field", display_name_field)
         pulumi.set(__self__, "groups_field", groups_field)
         pulumi.set(__self__, "idp_metadata_content", idp_metadata_content)
         pulumi.set(__self__, "rancher_api_host", rancher_api_host)
         pulumi.set(__self__, "sp_cert", sp_cert)
@@ -208,14 +209,17 @@
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter(name="entityIdField")
     def entity_id_field(self) -> Optional[pulumi.Input[str]]:
+        """
+        Ping entity ID field (string)
+        """
         return pulumi.get(self, "entity_id_field")
 
     @entity_id_field.setter
     def entity_id_field(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "entity_id_field", value)
 
     @property
@@ -253,14 +257,15 @@
         """
         Input properties used for looking up and filtering AuthConfigPing resources.
         :param pulumi.Input[str] access_mode: Access mode for auth. `required`, `restricted`, `unrestricted` are supported. Default `unrestricted` (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_principal_ids: Allowed principal ids for auth. Required if `access_mode` is `required` or `restricted`. Ex: `ping_user://<USER_ID>`  `ping_group://<GROUP_ID>` (list)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations of the resource (map)
         :param pulumi.Input[str] display_name_field: Ping display name field (string)
         :param pulumi.Input[bool] enabled: Enable auth config provider. Default `true` (bool)
+        :param pulumi.Input[str] entity_id_field: Ping entity ID field (string)
         :param pulumi.Input[str] groups_field: Ping group field (string)
         :param pulumi.Input[str] idp_metadata_content: Ping IDP metadata content (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels of the resource (map)
         :param pulumi.Input[str] name: (Computed) The name of the resource (string)
         :param pulumi.Input[str] rancher_api_host: Rancher URL. URL scheme needs to be specified, `https://<RANCHER_API_HOST>` (string)
         :param pulumi.Input[str] sp_cert: Ping SP cert (string)
         :param pulumi.Input[str] sp_key: Ping SP key (string)
@@ -360,14 +365,17 @@
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter(name="entityIdField")
     def entity_id_field(self) -> Optional[pulumi.Input[str]]:
+        """
+        Ping entity ID field (string)
+        """
         return pulumi.get(self, "entity_id_field")
 
     @entity_id_field.setter
     def entity_id_field(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "entity_id_field", value)
 
     @property
@@ -537,14 +545,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_mode: Access mode for auth. `required`, `restricted`, `unrestricted` are supported. Default `unrestricted` (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_principal_ids: Allowed principal ids for auth. Required if `access_mode` is `required` or `restricted`. Ex: `ping_user://<USER_ID>`  `ping_group://<GROUP_ID>` (list)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations of the resource (map)
         :param pulumi.Input[str] display_name_field: Ping display name field (string)
         :param pulumi.Input[bool] enabled: Enable auth config provider. Default `true` (bool)
+        :param pulumi.Input[str] entity_id_field: Ping entity ID field (string)
         :param pulumi.Input[str] groups_field: Ping group field (string)
         :param pulumi.Input[str] idp_metadata_content: Ping IDP metadata content (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels of the resource (map)
         :param pulumi.Input[str] rancher_api_host: Rancher URL. URL scheme needs to be specified, `https://<RANCHER_API_HOST>` (string)
         :param pulumi.Input[str] sp_cert: Ping SP cert (string)
         :param pulumi.Input[str] sp_key: Ping SP key (string)
         :param pulumi.Input[str] uid_field: Ping UID field (string)
@@ -685,14 +694,15 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_mode: Access mode for auth. `required`, `restricted`, `unrestricted` are supported. Default `unrestricted` (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_principal_ids: Allowed principal ids for auth. Required if `access_mode` is `required` or `restricted`. Ex: `ping_user://<USER_ID>`  `ping_group://<GROUP_ID>` (list)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations of the resource (map)
         :param pulumi.Input[str] display_name_field: Ping display name field (string)
         :param pulumi.Input[bool] enabled: Enable auth config provider. Default `true` (bool)
+        :param pulumi.Input[str] entity_id_field: Ping entity ID field (string)
         :param pulumi.Input[str] groups_field: Ping group field (string)
         :param pulumi.Input[str] idp_metadata_content: Ping IDP metadata content (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels of the resource (map)
         :param pulumi.Input[str] name: (Computed) The name of the resource (string)
         :param pulumi.Input[str] rancher_api_host: Rancher URL. URL scheme needs to be specified, `https://<RANCHER_API_HOST>` (string)
         :param pulumi.Input[str] sp_cert: Ping SP cert (string)
         :param pulumi.Input[str] sp_key: Ping SP key (string)
@@ -761,14 +771,17 @@
         Enable auth config provider. Default `true` (bool)
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="entityIdField")
     def entity_id_field(self) -> pulumi.Output[Optional[str]]:
+        """
+        Ping entity ID field (string)
+        """
         return pulumi.get(self, "entity_id_field")
 
     @property
     @pulumi.getter(name="groupsField")
     def groups_field(self) -> pulumi.Output[str]:
         """
         Ping group field (string)
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/bootstrap.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/catalog.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/catalog_v2.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/certificate.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cloud_credential.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cloud_credential.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         :param pulumi.Input['CloudCredentialDigitaloceanCredentialConfigArgs'] digitalocean_credential_config: DigitalOcean config for the Cloud Credential (list maxitems:1)
         :param pulumi.Input['CloudCredentialGoogleCredentialConfigArgs'] google_credential_config: Google config for the Cloud Credential (list maxitems:1)
         :param pulumi.Input['CloudCredentialHarvesterCredentialConfigArgs'] harvester_credential_config: Harvester config for the Cloud Credential (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Cloud Credential object (map)
         :param pulumi.Input['CloudCredentialLinodeCredentialConfigArgs'] linode_credential_config: Linode config for the Cloud Credential (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Cloud Credential (string)
         :param pulumi.Input['CloudCredentialOpenstackCredentialConfigArgs'] openstack_credential_config: OpenStack config for the Cloud Credential (list maxitems:1)
-        :param pulumi.Input['CloudCredentialS3CredentialConfigArgs'] s3_credential_config: S3 config for the Cloud Credential. Just for Rancher 2.6.0 and above (list maxitems:1)
+        :param pulumi.Input['CloudCredentialS3CredentialConfigArgs'] s3_credential_config: S3 config for the Cloud Credential. For Rancher 2.6.0 and above (list maxitems:1)
         :param pulumi.Input['CloudCredentialVsphereCredentialConfigArgs'] vsphere_credential_config: vSphere config for the Cloud Credential (list maxitems:1)
         """
         if amazonec2_credential_config is not None:
             pulumi.set(__self__, "amazonec2_credential_config", amazonec2_credential_config)
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
         if azure_credential_config is not None:
@@ -204,15 +204,15 @@
     def openstack_credential_config(self, value: Optional[pulumi.Input['CloudCredentialOpenstackCredentialConfigArgs']]):
         pulumi.set(self, "openstack_credential_config", value)
 
     @property
     @pulumi.getter(name="s3CredentialConfig")
     def s3_credential_config(self) -> Optional[pulumi.Input['CloudCredentialS3CredentialConfigArgs']]:
         """
-        S3 config for the Cloud Credential. Just for Rancher 2.6.0 and above (list maxitems:1)
+        S3 config for the Cloud Credential. For Rancher 2.6.0 and above (list maxitems:1)
         """
         return pulumi.get(self, "s3_credential_config")
 
     @s3_credential_config.setter
     def s3_credential_config(self, value: Optional[pulumi.Input['CloudCredentialS3CredentialConfigArgs']]):
         pulumi.set(self, "s3_credential_config", value)
 
@@ -256,15 +256,15 @@
         :param pulumi.Input[str] driver: (Computed) The driver of the Cloud Credential (string)
         :param pulumi.Input['CloudCredentialGoogleCredentialConfigArgs'] google_credential_config: Google config for the Cloud Credential (list maxitems:1)
         :param pulumi.Input['CloudCredentialHarvesterCredentialConfigArgs'] harvester_credential_config: Harvester config for the Cloud Credential (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Cloud Credential object (map)
         :param pulumi.Input['CloudCredentialLinodeCredentialConfigArgs'] linode_credential_config: Linode config for the Cloud Credential (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Cloud Credential (string)
         :param pulumi.Input['CloudCredentialOpenstackCredentialConfigArgs'] openstack_credential_config: OpenStack config for the Cloud Credential (list maxitems:1)
-        :param pulumi.Input['CloudCredentialS3CredentialConfigArgs'] s3_credential_config: S3 config for the Cloud Credential. Just for Rancher 2.6.0 and above (list maxitems:1)
+        :param pulumi.Input['CloudCredentialS3CredentialConfigArgs'] s3_credential_config: S3 config for the Cloud Credential. For Rancher 2.6.0 and above (list maxitems:1)
         :param pulumi.Input['CloudCredentialVsphereCredentialConfigArgs'] vsphere_credential_config: vSphere config for the Cloud Credential (list maxitems:1)
         """
         if amazonec2_credential_config is not None:
             pulumi.set(__self__, "amazonec2_credential_config", amazonec2_credential_config)
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
         if azure_credential_config is not None:
@@ -436,15 +436,15 @@
     def openstack_credential_config(self, value: Optional[pulumi.Input['CloudCredentialOpenstackCredentialConfigArgs']]):
         pulumi.set(self, "openstack_credential_config", value)
 
     @property
     @pulumi.getter(name="s3CredentialConfig")
     def s3_credential_config(self) -> Optional[pulumi.Input['CloudCredentialS3CredentialConfigArgs']]:
         """
-        S3 config for the Cloud Credential. Just for Rancher 2.6.0 and above (list maxitems:1)
+        S3 config for the Cloud Credential. For Rancher 2.6.0 and above (list maxitems:1)
         """
         return pulumi.get(self, "s3_credential_config")
 
     @s3_credential_config.setter
     def s3_credential_config(self, value: Optional[pulumi.Input['CloudCredentialS3CredentialConfigArgs']]):
         pulumi.set(self, "s3_credential_config", value)
 
@@ -532,15 +532,15 @@
         :param pulumi.Input[pulumi.InputType['CloudCredentialDigitaloceanCredentialConfigArgs']] digitalocean_credential_config: DigitalOcean config for the Cloud Credential (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['CloudCredentialGoogleCredentialConfigArgs']] google_credential_config: Google config for the Cloud Credential (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['CloudCredentialHarvesterCredentialConfigArgs']] harvester_credential_config: Harvester config for the Cloud Credential (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Cloud Credential object (map)
         :param pulumi.Input[pulumi.InputType['CloudCredentialLinodeCredentialConfigArgs']] linode_credential_config: Linode config for the Cloud Credential (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Cloud Credential (string)
         :param pulumi.Input[pulumi.InputType['CloudCredentialOpenstackCredentialConfigArgs']] openstack_credential_config: OpenStack config for the Cloud Credential (list maxitems:1)
-        :param pulumi.Input[pulumi.InputType['CloudCredentialS3CredentialConfigArgs']] s3_credential_config: S3 config for the Cloud Credential. Just for Rancher 2.6.0 and above (list maxitems:1)
+        :param pulumi.Input[pulumi.InputType['CloudCredentialS3CredentialConfigArgs']] s3_credential_config: S3 config for the Cloud Credential. For Rancher 2.6.0 and above (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['CloudCredentialVsphereCredentialConfigArgs']] vsphere_credential_config: vSphere config for the Cloud Credential (list maxitems:1)
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[CloudCredentialArgs] = None,
@@ -678,15 +678,15 @@
         :param pulumi.Input[str] driver: (Computed) The driver of the Cloud Credential (string)
         :param pulumi.Input[pulumi.InputType['CloudCredentialGoogleCredentialConfigArgs']] google_credential_config: Google config for the Cloud Credential (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['CloudCredentialHarvesterCredentialConfigArgs']] harvester_credential_config: Harvester config for the Cloud Credential (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Cloud Credential object (map)
         :param pulumi.Input[pulumi.InputType['CloudCredentialLinodeCredentialConfigArgs']] linode_credential_config: Linode config for the Cloud Credential (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Cloud Credential (string)
         :param pulumi.Input[pulumi.InputType['CloudCredentialOpenstackCredentialConfigArgs']] openstack_credential_config: OpenStack config for the Cloud Credential (list maxitems:1)
-        :param pulumi.Input[pulumi.InputType['CloudCredentialS3CredentialConfigArgs']] s3_credential_config: S3 config for the Cloud Credential. Just for Rancher 2.6.0 and above (list maxitems:1)
+        :param pulumi.Input[pulumi.InputType['CloudCredentialS3CredentialConfigArgs']] s3_credential_config: S3 config for the Cloud Credential. For Rancher 2.6.0 and above (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['CloudCredentialVsphereCredentialConfigArgs']] vsphere_credential_config: vSphere config for the Cloud Credential (list maxitems:1)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _CloudCredentialState.__new__(_CloudCredentialState)
 
         __props__.__dict__["amazonec2_credential_config"] = amazonec2_credential_config
@@ -801,15 +801,15 @@
         """
         return pulumi.get(self, "openstack_credential_config")
 
     @property
     @pulumi.getter(name="s3CredentialConfig")
     def s3_credential_config(self) -> pulumi.Output[Optional['outputs.CloudCredentialS3CredentialConfig']]:
         """
-        S3 config for the Cloud Credential. Just for Rancher 2.6.0 and above (list maxitems:1)
+        S3 config for the Cloud Credential. For Rancher 2.6.0 and above (list maxitems:1)
         """
         return pulumi.get(self, "s3_credential_config")
 
     @property
     @pulumi.getter(name="vsphereCredentialConfig")
     def vsphere_credential_config(self) -> pulumi.Output[Optional['outputs.CloudCredentialVsphereCredentialConfig']]:
         """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,41 +48,41 @@
                  name: Optional[pulumi.Input[str]] = None,
                  oke_config: Optional[pulumi.Input['ClusterOkeConfigArgs']] = None,
                  rke2_config: Optional[pulumi.Input['ClusterRke2ConfigArgs']] = None,
                  rke_config: Optional[pulumi.Input['ClusterRkeConfigArgs']] = None,
                  windows_prefered_cluster: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Cluster resource.
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterAgentEnvVarArgs']]] agent_env_vars: Optional Agent Env Vars for Rancher agent. Just for Rancher v2.5.6 and above (list)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterAgentEnvVarArgs']]] agent_env_vars: Optional Agent Env Vars for Rancher agent. For Rancher v2.5.6 and above (list)
         :param pulumi.Input['ClusterAksConfigArgs'] aks_config: The Azure AKS configuration for `aks` Clusters. Conflicts with `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input['ClusterAksConfigV2Args'] aks_config_v2: The Azure AKS v2 configuration for creating/import `aks` Clusters. Conflicts with `aks_config`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster (map)
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]] cluster_agent_deployment_customizations: Optional customization for cluster agent
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]] cluster_agent_deployment_customizations: Optional customization for cluster agent. For Rancher v2.7.5 and above (list)
         :param pulumi.Input['ClusterClusterAuthEndpointArgs'] cluster_auth_endpoint: Enabling the [local cluster authorized endpoint](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#local-cluster-auth-endpoint) allows direct communication with the cluster, bypassing the Rancher API proxy. (list maxitems:1)
         :param pulumi.Input['ClusterClusterMonitoringInputArgs'] cluster_monitoring_input: Cluster monitoring config. Any parameter defined in [rancher-monitoring charts](https://github.com/rancher/system-charts/tree/dev/charts/rancher-monitoring) could be configured  (list maxitems:1)
-        :param pulumi.Input['ClusterClusterTemplateAnswersArgs'] cluster_template_answers: Cluster template answers. Just for Rancher v2.3.x and above (list maxitems:1)
-        :param pulumi.Input[str] cluster_template_id: Cluster template ID. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterClusterTemplateQuestionArgs']]] cluster_template_questions: Cluster template questions. Just for Rancher v2.3.x and above (list)
-        :param pulumi.Input[str] cluster_template_revision_id: Cluster template revision ID. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster default pod security admission configuration template name
+        :param pulumi.Input['ClusterClusterTemplateAnswersArgs'] cluster_template_answers: Cluster template answers. For Rancher v2.3.x and above (list maxitems:1)
+        :param pulumi.Input[str] cluster_template_id: Cluster template ID. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterClusterTemplateQuestionArgs']]] cluster_template_questions: Cluster template questions. For Rancher v2.3.x and above (list)
+        :param pulumi.Input[str] cluster_template_revision_id: Cluster template revision ID. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster default pod security admission configuration template name (string)
         :param pulumi.Input[str] default_pod_security_policy_template_id: [Default pod security policy template id](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#pod-security-policy-support) (string)
         :param pulumi.Input[str] description: The description for Cluster (string)
-        :param pulumi.Input[str] desired_agent_image: Desired agent image. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[str] desired_auth_image: Desired auth image. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[str] docker_root_dir: Desired auth image. Just for Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] desired_agent_image: Desired agent image. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] desired_auth_image: Desired auth image. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] docker_root_dir: Desired auth image. For Rancher v2.3.x and above (string)
         :param pulumi.Input[str] driver: (Computed) The driver used for the Cluster. `imported`, `azurekubernetesservice`, `amazonelasticcontainerservice`, `googlekubernetesengine` and `rancherKubernetesEngine` are supported (string)
         :param pulumi.Input['ClusterEksConfigArgs'] eks_config: The Amazon EKS configuration for `eks` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
-        :param pulumi.Input['ClusterEksConfigV2Args'] eks_config_v2: The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x or above (list maxitems:1)
+        :param pulumi.Input['ClusterEksConfigV2Args'] eks_config_v2: The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x and above (list maxitems:1)
         :param pulumi.Input[bool] enable_cluster_alerting: Enable built-in cluster alerting (bool)
         :param pulumi.Input[bool] enable_cluster_monitoring: Enable built-in cluster monitoring (bool)
         :param pulumi.Input[bool] enable_network_policy: Enable project network isolation (bool)
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]] fleet_agent_deployment_customizations: Optional customization for fleet agent
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]] fleet_agent_deployment_customizations: Optional customization for fleet agent. For Rancher v2.7.5 and above (list)
         :param pulumi.Input[str] fleet_workspace_name: Fleet workspace name (string)
         :param pulumi.Input['ClusterGkeConfigArgs'] gke_config: The Google GKE configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config_v2`, `oke_config`, `k3s_config` and `rke_config` (list maxitems:1)
-        :param pulumi.Input['ClusterGkeConfigV2Args'] gke_config_v2: The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 or above (list maxitems:1)
+        :param pulumi.Input['ClusterGkeConfigV2Args'] gke_config_v2: The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 and above (list maxitems:1)
         :param pulumi.Input['ClusterK3sConfigArgs'] k3s_config: The K3S configuration for `k3s` imported Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster (map)
         :param pulumi.Input[str] name: The name of the Cluster (string)
         :param pulumi.Input['ClusterOkeConfigArgs'] oke_config: The Oracle OKE configuration for `oke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input['ClusterRke2ConfigArgs'] rke2_config: The RKE2 configuration for `rke2` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `gke_config`, `oke_config`, `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input['ClusterRkeConfigArgs'] rke_config: The RKE configuration for `rke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` and `k3s_config` (list maxitems:1)
         :param pulumi.Input[bool] windows_prefered_cluster: Windows preferred cluster. Default: `false` (bool)
@@ -156,15 +156,15 @@
         if windows_prefered_cluster is not None:
             pulumi.set(__self__, "windows_prefered_cluster", windows_prefered_cluster)
 
     @property
     @pulumi.getter(name="agentEnvVars")
     def agent_env_vars(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterAgentEnvVarArgs']]]]:
         """
-        Optional Agent Env Vars for Rancher agent. Just for Rancher v2.5.6 and above (list)
+        Optional Agent Env Vars for Rancher agent. For Rancher v2.5.6 and above (list)
         """
         return pulumi.get(self, "agent_env_vars")
 
     @agent_env_vars.setter
     def agent_env_vars(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterAgentEnvVarArgs']]]]):
         pulumi.set(self, "agent_env_vars", value)
 
@@ -204,15 +204,15 @@
     def annotations(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "annotations", value)
 
     @property
     @pulumi.getter(name="clusterAgentDeploymentCustomizations")
     def cluster_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]]]:
         """
-        Optional customization for cluster agent
+        Optional customization for cluster agent. For Rancher v2.7.5 and above (list)
         """
         return pulumi.get(self, "cluster_agent_deployment_customizations")
 
     @cluster_agent_deployment_customizations.setter
     def cluster_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]]]):
         pulumi.set(self, "cluster_agent_deployment_customizations", value)
 
@@ -240,63 +240,63 @@
     def cluster_monitoring_input(self, value: Optional[pulumi.Input['ClusterClusterMonitoringInputArgs']]):
         pulumi.set(self, "cluster_monitoring_input", value)
 
     @property
     @pulumi.getter(name="clusterTemplateAnswers")
     def cluster_template_answers(self) -> Optional[pulumi.Input['ClusterClusterTemplateAnswersArgs']]:
         """
-        Cluster template answers. Just for Rancher v2.3.x and above (list maxitems:1)
+        Cluster template answers. For Rancher v2.3.x and above (list maxitems:1)
         """
         return pulumi.get(self, "cluster_template_answers")
 
     @cluster_template_answers.setter
     def cluster_template_answers(self, value: Optional[pulumi.Input['ClusterClusterTemplateAnswersArgs']]):
         pulumi.set(self, "cluster_template_answers", value)
 
     @property
     @pulumi.getter(name="clusterTemplateId")
     def cluster_template_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster template ID. Just for Rancher v2.3.x and above (string)
+        Cluster template ID. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "cluster_template_id")
 
     @cluster_template_id.setter
     def cluster_template_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_template_id", value)
 
     @property
     @pulumi.getter(name="clusterTemplateQuestions")
     def cluster_template_questions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterTemplateQuestionArgs']]]]:
         """
-        Cluster template questions. Just for Rancher v2.3.x and above (list)
+        Cluster template questions. For Rancher v2.3.x and above (list)
         """
         return pulumi.get(self, "cluster_template_questions")
 
     @cluster_template_questions.setter
     def cluster_template_questions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterTemplateQuestionArgs']]]]):
         pulumi.set(self, "cluster_template_questions", value)
 
     @property
     @pulumi.getter(name="clusterTemplateRevisionId")
     def cluster_template_revision_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster template revision ID. Just for Rancher v2.3.x and above (string)
+        Cluster template revision ID. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "cluster_template_revision_id")
 
     @cluster_template_revision_id.setter
     def cluster_template_revision_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_template_revision_id", value)
 
     @property
     @pulumi.getter(name="defaultPodSecurityAdmissionConfigurationTemplateName")
     def default_pod_security_admission_configuration_template_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster default pod security admission configuration template name
+        Cluster default pod security admission configuration template name (string)
         """
         return pulumi.get(self, "default_pod_security_admission_configuration_template_name")
 
     @default_pod_security_admission_configuration_template_name.setter
     def default_pod_security_admission_configuration_template_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_pod_security_admission_configuration_template_name", value)
 
@@ -324,39 +324,39 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="desiredAgentImage")
     def desired_agent_image(self) -> Optional[pulumi.Input[str]]:
         """
-        Desired agent image. Just for Rancher v2.3.x and above (string)
+        Desired agent image. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "desired_agent_image")
 
     @desired_agent_image.setter
     def desired_agent_image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "desired_agent_image", value)
 
     @property
     @pulumi.getter(name="desiredAuthImage")
     def desired_auth_image(self) -> Optional[pulumi.Input[str]]:
         """
-        Desired auth image. Just for Rancher v2.3.x and above (string)
+        Desired auth image. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "desired_auth_image")
 
     @desired_auth_image.setter
     def desired_auth_image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "desired_auth_image", value)
 
     @property
     @pulumi.getter(name="dockerRootDir")
     def docker_root_dir(self) -> Optional[pulumi.Input[str]]:
         """
-        Desired auth image. Just for Rancher v2.3.x and above (string)
+        Desired auth image. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "docker_root_dir")
 
     @docker_root_dir.setter
     def docker_root_dir(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "docker_root_dir", value)
 
@@ -384,15 +384,15 @@
     def eks_config(self, value: Optional[pulumi.Input['ClusterEksConfigArgs']]):
         pulumi.set(self, "eks_config", value)
 
     @property
     @pulumi.getter(name="eksConfigV2")
     def eks_config_v2(self) -> Optional[pulumi.Input['ClusterEksConfigV2Args']]:
         """
-        The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x or above (list maxitems:1)
+        The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x and above (list maxitems:1)
         """
         return pulumi.get(self, "eks_config_v2")
 
     @eks_config_v2.setter
     def eks_config_v2(self, value: Optional[pulumi.Input['ClusterEksConfigV2Args']]):
         pulumi.set(self, "eks_config_v2", value)
 
@@ -432,15 +432,15 @@
     def enable_network_policy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_network_policy", value)
 
     @property
     @pulumi.getter(name="fleetAgentDeploymentCustomizations")
     def fleet_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]]]:
         """
-        Optional customization for fleet agent
+        Optional customization for fleet agent. For Rancher v2.7.5 and above (list)
         """
         return pulumi.get(self, "fleet_agent_deployment_customizations")
 
     @fleet_agent_deployment_customizations.setter
     def fleet_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]]]):
         pulumi.set(self, "fleet_agent_deployment_customizations", value)
 
@@ -468,15 +468,15 @@
     def gke_config(self, value: Optional[pulumi.Input['ClusterGkeConfigArgs']]):
         pulumi.set(self, "gke_config", value)
 
     @property
     @pulumi.getter(name="gkeConfigV2")
     def gke_config_v2(self) -> Optional[pulumi.Input['ClusterGkeConfigV2Args']]:
         """
-        The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 or above (list maxitems:1)
+        The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 and above (list maxitems:1)
         """
         return pulumi.get(self, "gke_config_v2")
 
     @gke_config_v2.setter
     def gke_config_v2(self, value: Optional[pulumi.Input['ClusterGkeConfigV2Args']]):
         pulumi.set(self, "gke_config_v2", value)
 
@@ -607,46 +607,46 @@
                  oke_config: Optional[pulumi.Input['ClusterOkeConfigArgs']] = None,
                  rke2_config: Optional[pulumi.Input['ClusterRke2ConfigArgs']] = None,
                  rke_config: Optional[pulumi.Input['ClusterRkeConfigArgs']] = None,
                  system_project_id: Optional[pulumi.Input[str]] = None,
                  windows_prefered_cluster: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering Cluster resources.
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterAgentEnvVarArgs']]] agent_env_vars: Optional Agent Env Vars for Rancher agent. Just for Rancher v2.5.6 and above (list)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterAgentEnvVarArgs']]] agent_env_vars: Optional Agent Env Vars for Rancher agent. For Rancher v2.5.6 and above (list)
         :param pulumi.Input['ClusterAksConfigArgs'] aks_config: The Azure AKS configuration for `aks` Clusters. Conflicts with `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input['ClusterAksConfigV2Args'] aks_config_v2: The Azure AKS v2 configuration for creating/import `aks` Clusters. Conflicts with `aks_config`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster (map)
         :param pulumi.Input[str] ca_cert: TLS CA certificate for etcd service (string)
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]] cluster_agent_deployment_customizations: Optional customization for cluster agent
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]] cluster_agent_deployment_customizations: Optional customization for cluster agent. For Rancher v2.7.5 and above (list)
         :param pulumi.Input['ClusterClusterAuthEndpointArgs'] cluster_auth_endpoint: Enabling the [local cluster authorized endpoint](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#local-cluster-auth-endpoint) allows direct communication with the cluster, bypassing the Rancher API proxy. (list maxitems:1)
         :param pulumi.Input['ClusterClusterMonitoringInputArgs'] cluster_monitoring_input: Cluster monitoring config. Any parameter defined in [rancher-monitoring charts](https://github.com/rancher/system-charts/tree/dev/charts/rancher-monitoring) could be configured  (list maxitems:1)
         :param pulumi.Input['ClusterClusterRegistrationTokenArgs'] cluster_registration_token: (Computed) Cluster Registration Token generated for the cluster (list maxitems:1)
-        :param pulumi.Input['ClusterClusterTemplateAnswersArgs'] cluster_template_answers: Cluster template answers. Just for Rancher v2.3.x and above (list maxitems:1)
-        :param pulumi.Input[str] cluster_template_id: Cluster template ID. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterClusterTemplateQuestionArgs']]] cluster_template_questions: Cluster template questions. Just for Rancher v2.3.x and above (list)
-        :param pulumi.Input[str] cluster_template_revision_id: Cluster template revision ID. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster default pod security admission configuration template name
+        :param pulumi.Input['ClusterClusterTemplateAnswersArgs'] cluster_template_answers: Cluster template answers. For Rancher v2.3.x and above (list maxitems:1)
+        :param pulumi.Input[str] cluster_template_id: Cluster template ID. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterClusterTemplateQuestionArgs']]] cluster_template_questions: Cluster template questions. For Rancher v2.3.x and above (list)
+        :param pulumi.Input[str] cluster_template_revision_id: Cluster template revision ID. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster default pod security admission configuration template name (string)
         :param pulumi.Input[str] default_pod_security_policy_template_id: [Default pod security policy template id](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#pod-security-policy-support) (string)
         :param pulumi.Input[str] default_project_id: (Computed) Default project ID for the cluster (string)
         :param pulumi.Input[str] description: The description for Cluster (string)
-        :param pulumi.Input[str] desired_agent_image: Desired agent image. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[str] desired_auth_image: Desired auth image. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[str] docker_root_dir: Desired auth image. Just for Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] desired_agent_image: Desired agent image. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] desired_auth_image: Desired auth image. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] docker_root_dir: Desired auth image. For Rancher v2.3.x and above (string)
         :param pulumi.Input[str] driver: (Computed) The driver used for the Cluster. `imported`, `azurekubernetesservice`, `amazonelasticcontainerservice`, `googlekubernetesengine` and `rancherKubernetesEngine` are supported (string)
         :param pulumi.Input['ClusterEksConfigArgs'] eks_config: The Amazon EKS configuration for `eks` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
-        :param pulumi.Input['ClusterEksConfigV2Args'] eks_config_v2: The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x or above (list maxitems:1)
+        :param pulumi.Input['ClusterEksConfigV2Args'] eks_config_v2: The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x and above (list maxitems:1)
         :param pulumi.Input[bool] enable_cluster_alerting: Enable built-in cluster alerting (bool)
         :param pulumi.Input[bool] enable_cluster_istio: Deploy istio on `system` project and `istio-system` namespace, using App resource instead. See above example.
         :param pulumi.Input[bool] enable_cluster_monitoring: Enable built-in cluster monitoring (bool)
         :param pulumi.Input[bool] enable_network_policy: Enable project network isolation (bool)
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]] fleet_agent_deployment_customizations: Optional customization for fleet agent
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]] fleet_agent_deployment_customizations: Optional customization for fleet agent. For Rancher v2.7.5 and above (list)
         :param pulumi.Input[str] fleet_workspace_name: Fleet workspace name (string)
         :param pulumi.Input['ClusterGkeConfigArgs'] gke_config: The Google GKE configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config_v2`, `oke_config`, `k3s_config` and `rke_config` (list maxitems:1)
-        :param pulumi.Input['ClusterGkeConfigV2Args'] gke_config_v2: The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 or above (list maxitems:1)
-        :param pulumi.Input[bool] istio_enabled: (Computed) Is istio enabled at cluster? Just for Rancher v2.3.x and above (bool)
+        :param pulumi.Input['ClusterGkeConfigV2Args'] gke_config_v2: The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 and above (list maxitems:1)
+        :param pulumi.Input[bool] istio_enabled: (Computed) Is istio enabled at cluster? For Rancher v2.3.x and above (bool)
         :param pulumi.Input['ClusterK3sConfigArgs'] k3s_config: The K3S configuration for `k3s` imported Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[str] kube_config: (Computed/Sensitive) Kube Config generated for the cluster. Note: For Rancher 2.6.0 and above, when the cluster has `cluster_auth_endpoint` enabled, the kube_config will not be available until the cluster is `connected` (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster (map)
         :param pulumi.Input[str] name: The name of the Cluster (string)
         :param pulumi.Input['ClusterOkeConfigArgs'] oke_config: The Oracle OKE configuration for `oke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input['ClusterRke2ConfigArgs'] rke2_config: The RKE2 configuration for `rke2` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `gke_config`, `oke_config`, `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input['ClusterRkeConfigArgs'] rke_config: The RKE configuration for `rke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` and `k3s_config` (list maxitems:1)
@@ -739,15 +739,15 @@
         if windows_prefered_cluster is not None:
             pulumi.set(__self__, "windows_prefered_cluster", windows_prefered_cluster)
 
     @property
     @pulumi.getter(name="agentEnvVars")
     def agent_env_vars(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterAgentEnvVarArgs']]]]:
         """
-        Optional Agent Env Vars for Rancher agent. Just for Rancher v2.5.6 and above (list)
+        Optional Agent Env Vars for Rancher agent. For Rancher v2.5.6 and above (list)
         """
         return pulumi.get(self, "agent_env_vars")
 
     @agent_env_vars.setter
     def agent_env_vars(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterAgentEnvVarArgs']]]]):
         pulumi.set(self, "agent_env_vars", value)
 
@@ -799,15 +799,15 @@
     def ca_cert(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ca_cert", value)
 
     @property
     @pulumi.getter(name="clusterAgentDeploymentCustomizations")
     def cluster_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]]]:
         """
-        Optional customization for cluster agent
+        Optional customization for cluster agent. For Rancher v2.7.5 and above (list)
         """
         return pulumi.get(self, "cluster_agent_deployment_customizations")
 
     @cluster_agent_deployment_customizations.setter
     def cluster_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]]]):
         pulumi.set(self, "cluster_agent_deployment_customizations", value)
 
@@ -847,63 +847,63 @@
     def cluster_registration_token(self, value: Optional[pulumi.Input['ClusterClusterRegistrationTokenArgs']]):
         pulumi.set(self, "cluster_registration_token", value)
 
     @property
     @pulumi.getter(name="clusterTemplateAnswers")
     def cluster_template_answers(self) -> Optional[pulumi.Input['ClusterClusterTemplateAnswersArgs']]:
         """
-        Cluster template answers. Just for Rancher v2.3.x and above (list maxitems:1)
+        Cluster template answers. For Rancher v2.3.x and above (list maxitems:1)
         """
         return pulumi.get(self, "cluster_template_answers")
 
     @cluster_template_answers.setter
     def cluster_template_answers(self, value: Optional[pulumi.Input['ClusterClusterTemplateAnswersArgs']]):
         pulumi.set(self, "cluster_template_answers", value)
 
     @property
     @pulumi.getter(name="clusterTemplateId")
     def cluster_template_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster template ID. Just for Rancher v2.3.x and above (string)
+        Cluster template ID. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "cluster_template_id")
 
     @cluster_template_id.setter
     def cluster_template_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_template_id", value)
 
     @property
     @pulumi.getter(name="clusterTemplateQuestions")
     def cluster_template_questions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterTemplateQuestionArgs']]]]:
         """
-        Cluster template questions. Just for Rancher v2.3.x and above (list)
+        Cluster template questions. For Rancher v2.3.x and above (list)
         """
         return pulumi.get(self, "cluster_template_questions")
 
     @cluster_template_questions.setter
     def cluster_template_questions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterTemplateQuestionArgs']]]]):
         pulumi.set(self, "cluster_template_questions", value)
 
     @property
     @pulumi.getter(name="clusterTemplateRevisionId")
     def cluster_template_revision_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster template revision ID. Just for Rancher v2.3.x and above (string)
+        Cluster template revision ID. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "cluster_template_revision_id")
 
     @cluster_template_revision_id.setter
     def cluster_template_revision_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_template_revision_id", value)
 
     @property
     @pulumi.getter(name="defaultPodSecurityAdmissionConfigurationTemplateName")
     def default_pod_security_admission_configuration_template_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster default pod security admission configuration template name
+        Cluster default pod security admission configuration template name (string)
         """
         return pulumi.get(self, "default_pod_security_admission_configuration_template_name")
 
     @default_pod_security_admission_configuration_template_name.setter
     def default_pod_security_admission_configuration_template_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_pod_security_admission_configuration_template_name", value)
 
@@ -943,39 +943,39 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="desiredAgentImage")
     def desired_agent_image(self) -> Optional[pulumi.Input[str]]:
         """
-        Desired agent image. Just for Rancher v2.3.x and above (string)
+        Desired agent image. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "desired_agent_image")
 
     @desired_agent_image.setter
     def desired_agent_image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "desired_agent_image", value)
 
     @property
     @pulumi.getter(name="desiredAuthImage")
     def desired_auth_image(self) -> Optional[pulumi.Input[str]]:
         """
-        Desired auth image. Just for Rancher v2.3.x and above (string)
+        Desired auth image. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "desired_auth_image")
 
     @desired_auth_image.setter
     def desired_auth_image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "desired_auth_image", value)
 
     @property
     @pulumi.getter(name="dockerRootDir")
     def docker_root_dir(self) -> Optional[pulumi.Input[str]]:
         """
-        Desired auth image. Just for Rancher v2.3.x and above (string)
+        Desired auth image. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "docker_root_dir")
 
     @docker_root_dir.setter
     def docker_root_dir(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "docker_root_dir", value)
 
@@ -1003,15 +1003,15 @@
     def eks_config(self, value: Optional[pulumi.Input['ClusterEksConfigArgs']]):
         pulumi.set(self, "eks_config", value)
 
     @property
     @pulumi.getter(name="eksConfigV2")
     def eks_config_v2(self) -> Optional[pulumi.Input['ClusterEksConfigV2Args']]:
         """
-        The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x or above (list maxitems:1)
+        The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x and above (list maxitems:1)
         """
         return pulumi.get(self, "eks_config_v2")
 
     @eks_config_v2.setter
     def eks_config_v2(self, value: Optional[pulumi.Input['ClusterEksConfigV2Args']]):
         pulumi.set(self, "eks_config_v2", value)
 
@@ -1029,14 +1029,17 @@
 
     @property
     @pulumi.getter(name="enableClusterIstio")
     def enable_cluster_istio(self) -> Optional[pulumi.Input[bool]]:
         """
         Deploy istio on `system` project and `istio-system` namespace, using App resource instead. See above example.
         """
+        warnings.warn("""Deploy istio using rancher2_app resource instead""", DeprecationWarning)
+        pulumi.log.warn("""enable_cluster_istio is deprecated: Deploy istio using rancher2_app resource instead""")
+
         return pulumi.get(self, "enable_cluster_istio")
 
     @enable_cluster_istio.setter
     def enable_cluster_istio(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_cluster_istio", value)
 
     @property
@@ -1063,15 +1066,15 @@
     def enable_network_policy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_network_policy", value)
 
     @property
     @pulumi.getter(name="fleetAgentDeploymentCustomizations")
     def fleet_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]]]:
         """
-        Optional customization for fleet agent
+        Optional customization for fleet agent. For Rancher v2.7.5 and above (list)
         """
         return pulumi.get(self, "fleet_agent_deployment_customizations")
 
     @fleet_agent_deployment_customizations.setter
     def fleet_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]]]):
         pulumi.set(self, "fleet_agent_deployment_customizations", value)
 
@@ -1099,27 +1102,27 @@
     def gke_config(self, value: Optional[pulumi.Input['ClusterGkeConfigArgs']]):
         pulumi.set(self, "gke_config", value)
 
     @property
     @pulumi.getter(name="gkeConfigV2")
     def gke_config_v2(self) -> Optional[pulumi.Input['ClusterGkeConfigV2Args']]:
         """
-        The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 or above (list maxitems:1)
+        The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 and above (list maxitems:1)
         """
         return pulumi.get(self, "gke_config_v2")
 
     @gke_config_v2.setter
     def gke_config_v2(self, value: Optional[pulumi.Input['ClusterGkeConfigV2Args']]):
         pulumi.set(self, "gke_config_v2", value)
 
     @property
     @pulumi.getter(name="istioEnabled")
     def istio_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Computed) Is istio enabled at cluster? Just for Rancher v2.3.x and above (bool)
+        (Computed) Is istio enabled at cluster? For Rancher v2.3.x and above (bool)
         """
         return pulumi.get(self, "istio_enabled")
 
     @istio_enabled.setter
     def istio_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "istio_enabled", value)
 
@@ -1276,15 +1279,15 @@
         Provides a Rancher v2 Cluster resource. This can be used to create Clusters for Rancher v2 environments and retrieve their information.
 
         ## Example Usage
 
         **Note optional/computed arguments** If any `optional/computed` argument of this resource is defined by the user, removing it from tf file will NOT reset its value. To reset it, let its definition at tf file as empty/false object. Ex: `enable_cluster_monitoring = false`, `cloud_provider {}`, `name = ""`
         ### Creating Rancher v2 RKE cluster enabling and customizing monitoring
 
-        **Note** Cluster monitoring version `0.2.0` or above, can't be enabled until cluster is fully deployed as [`kubeVersion`](https://github.com/rancher/system-charts/blob/52be656700468904b9bf15c3f39cd7112e1f8c9b/charts/rancher-monitoring/v0.2.0/Chart.yaml#L12) requirement has been introduced to helm chart
+        **Note** Cluster monitoring version `0.2.0` and above, can't be enabled until cluster is fully deployed as [`kubeVersion`](https://github.com/rancher/system-charts/blob/52be656700468904b9bf15c3f39cd7112e1f8c9b/charts/rancher-monitoring/v0.2.0/Chart.yaml#L12) requirement has been introduced to helm chart
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 RKE Cluster
         foo_custom = rancher2.Cluster("foo-custom",
@@ -1448,15 +1451,15 @@
             hostname_prefix="foo-cluster-0",
             node_template_id=foo_node_template.id,
             quantity=3,
             control_plane=True,
             etcd=True,
             worker=True)
         ```
-        ### Creating Rancher v2 RKE cluster from template. For Rancher v2.3.x or above.
+        ### Creating Rancher v2 RKE cluster from template. For Rancher v2.3.x and above.
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 cluster template
         foo_cluster_template = rancher2.ClusterTemplate("fooClusterTemplate",
@@ -1483,15 +1486,15 @@
             )],
             description="Test cluster template v2")
         # Create a new rancher2 RKE Cluster from template
         foo_cluster = rancher2.Cluster("fooCluster",
             cluster_template_id=foo_cluster_template.id,
             cluster_template_revision_id=foo_cluster_template.template_revisions[0].id)
         ```
-        ### Creating Rancher v2 RKE cluster with upgrade strategy. For Rancher v2.4.x or above.
+        ### Creating Rancher v2 RKE cluster with upgrade strategy. For Rancher v2.4.x and above.
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         foo = rancher2.Cluster("foo",
             description="Terraform custom cluster",
@@ -1532,15 +1535,59 @@
                 ),
                 upgrade_strategy=rancher2.ClusterRkeConfigUpgradeStrategyArgs(
                     drain=True,
                     max_unavailable_worker="20%",
                 ),
             ))
         ```
-        ### Importing EKS cluster to Rancher v2, using `eks_config_v2`. For Rancher v2.5.x or above.
+        ### Creating Rancher v2 RKE cluster with cluster agent customization. For Rancher v2.7.5 and above.
+
+        ```python
+        import pulumi
+        import pulumi_rancher2 as rancher2
+
+        foo = rancher2.Cluster("foo",
+            cluster_agent_deployment_customizations=[rancher2.ClusterClusterAgentDeploymentCustomizationArgs(
+                append_tolerations=[rancher2.ClusterClusterAgentDeploymentCustomizationAppendTolerationArgs(
+                    effect="NoSchedule",
+                    key="tolerate/control-plane",
+                    value="true",
+                )],
+                override_affinity=\"\"\"{
+          "nodeAffinity": {
+            "requiredDuringSchedulingIgnoredDuringExecution": {
+              "nodeSelectorTerms": [{
+                "matchExpressions": [{
+                  "key": "not.this/nodepool",
+                  "operator": "In",
+                  "values": [
+                    "true"
+                  ]
+                }]
+              }]
+            }
+          }
+        }
+
+        \"\"\",
+                override_resource_requirements=[rancher2.ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs(
+                    cpu_limit="800",
+                    cpu_request="500",
+                    memory_limit="800",
+                    memory_request="500",
+                )],
+            )],
+            description="Terraform cluster with agent customization",
+            rke_config=rancher2.ClusterRkeConfigArgs(
+                network=rancher2.ClusterRkeConfigNetworkArgs(
+                    plugin="canal",
+                ),
+            ))
+        ```
+        ### Importing EKS cluster to Rancher v2, using `eks_config_v2`. For Rancher v2.5.x and above.
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         foo_cloud_credential = rancher2.CloudCredential("fooCloudCredential",
             description="foo test",
@@ -1553,15 +1600,15 @@
             eks_config_v2=rancher2.ClusterEksConfigV2Args(
                 cloud_credential_id=foo_cloud_credential.id,
                 name="<CLUSTER_NAME>",
                 region="<EKS_REGION>",
                 imported=True,
             ))
         ```
-        ### Creating EKS cluster from Rancher v2, using `eks_config_v2`. For Rancher v2.5.x or above.
+        ### Creating EKS cluster from Rancher v2, using `eks_config_v2`. For Rancher v2.5.x and above.
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         foo_cloud_credential = rancher2.CloudCredential("fooCloudCredential",
             description="foo test",
@@ -1594,15 +1641,15 @@
                         node_role="arn:aws:iam::role/test-NodeInstanceRole",
                     ),
                 ],
                 private_access=True,
                 public_access=False,
             ))
         ```
-        ### Creating EKS cluster from Rancher v2, using `eks_config_v2` and launch template. For Rancher v2.5.6 or above.
+        ### Creating EKS cluster from Rancher v2, using `eks_config_v2` and launch template. For Rancher v2.5.6 and above.
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         foo_cloud_credential = rancher2.CloudCredential("fooCloudCredential",
             description="foo test",
@@ -1629,15 +1676,15 @@
                         version=1,
                     )],
                 )],
                 private_access=True,
                 public_access=True,
             ))
         ```
-        ### Creating AKS cluster from Rancher v2, using `aks_config_v2`. For Rancher v2.6.0 or above.
+        ### Creating AKS cluster from Rancher v2, using `aks_config_v2`. For Rancher v2.6.0 and above.
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         foo_aks = rancher2.CloudCredential("foo-aks", azure_credential_config=rancher2.CloudCredentialAzureCredentialConfigArgs(
             client_id="<CLIENT_ID>",
@@ -1696,41 +1743,41 @@
 
         ```sh
          $ pulumi import rancher2:index/cluster:Cluster foo &lt;CLUSTER_ID&gt;
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterAgentEnvVarArgs']]]] agent_env_vars: Optional Agent Env Vars for Rancher agent. Just for Rancher v2.5.6 and above (list)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterAgentEnvVarArgs']]]] agent_env_vars: Optional Agent Env Vars for Rancher agent. For Rancher v2.5.6 and above (list)
         :param pulumi.Input[pulumi.InputType['ClusterAksConfigArgs']] aks_config: The Azure AKS configuration for `aks` Clusters. Conflicts with `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterAksConfigV2Args']] aks_config_v2: The Azure AKS v2 configuration for creating/import `aks` Clusters. Conflicts with `aks_config`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster (map)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterAgentDeploymentCustomizationArgs']]]] cluster_agent_deployment_customizations: Optional customization for cluster agent
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterAgentDeploymentCustomizationArgs']]]] cluster_agent_deployment_customizations: Optional customization for cluster agent. For Rancher v2.7.5 and above (list)
         :param pulumi.Input[pulumi.InputType['ClusterClusterAuthEndpointArgs']] cluster_auth_endpoint: Enabling the [local cluster authorized endpoint](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#local-cluster-auth-endpoint) allows direct communication with the cluster, bypassing the Rancher API proxy. (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterClusterMonitoringInputArgs']] cluster_monitoring_input: Cluster monitoring config. Any parameter defined in [rancher-monitoring charts](https://github.com/rancher/system-charts/tree/dev/charts/rancher-monitoring) could be configured  (list maxitems:1)
-        :param pulumi.Input[pulumi.InputType['ClusterClusterTemplateAnswersArgs']] cluster_template_answers: Cluster template answers. Just for Rancher v2.3.x and above (list maxitems:1)
-        :param pulumi.Input[str] cluster_template_id: Cluster template ID. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterTemplateQuestionArgs']]]] cluster_template_questions: Cluster template questions. Just for Rancher v2.3.x and above (list)
-        :param pulumi.Input[str] cluster_template_revision_id: Cluster template revision ID. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster default pod security admission configuration template name
+        :param pulumi.Input[pulumi.InputType['ClusterClusterTemplateAnswersArgs']] cluster_template_answers: Cluster template answers. For Rancher v2.3.x and above (list maxitems:1)
+        :param pulumi.Input[str] cluster_template_id: Cluster template ID. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterTemplateQuestionArgs']]]] cluster_template_questions: Cluster template questions. For Rancher v2.3.x and above (list)
+        :param pulumi.Input[str] cluster_template_revision_id: Cluster template revision ID. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster default pod security admission configuration template name (string)
         :param pulumi.Input[str] default_pod_security_policy_template_id: [Default pod security policy template id](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#pod-security-policy-support) (string)
         :param pulumi.Input[str] description: The description for Cluster (string)
-        :param pulumi.Input[str] desired_agent_image: Desired agent image. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[str] desired_auth_image: Desired auth image. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[str] docker_root_dir: Desired auth image. Just for Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] desired_agent_image: Desired agent image. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] desired_auth_image: Desired auth image. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] docker_root_dir: Desired auth image. For Rancher v2.3.x and above (string)
         :param pulumi.Input[str] driver: (Computed) The driver used for the Cluster. `imported`, `azurekubernetesservice`, `amazonelasticcontainerservice`, `googlekubernetesengine` and `rancherKubernetesEngine` are supported (string)
         :param pulumi.Input[pulumi.InputType['ClusterEksConfigArgs']] eks_config: The Amazon EKS configuration for `eks` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
-        :param pulumi.Input[pulumi.InputType['ClusterEksConfigV2Args']] eks_config_v2: The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x or above (list maxitems:1)
+        :param pulumi.Input[pulumi.InputType['ClusterEksConfigV2Args']] eks_config_v2: The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x and above (list maxitems:1)
         :param pulumi.Input[bool] enable_cluster_alerting: Enable built-in cluster alerting (bool)
         :param pulumi.Input[bool] enable_cluster_monitoring: Enable built-in cluster monitoring (bool)
         :param pulumi.Input[bool] enable_network_policy: Enable project network isolation (bool)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterFleetAgentDeploymentCustomizationArgs']]]] fleet_agent_deployment_customizations: Optional customization for fleet agent
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterFleetAgentDeploymentCustomizationArgs']]]] fleet_agent_deployment_customizations: Optional customization for fleet agent. For Rancher v2.7.5 and above (list)
         :param pulumi.Input[str] fleet_workspace_name: Fleet workspace name (string)
         :param pulumi.Input[pulumi.InputType['ClusterGkeConfigArgs']] gke_config: The Google GKE configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config_v2`, `oke_config`, `k3s_config` and `rke_config` (list maxitems:1)
-        :param pulumi.Input[pulumi.InputType['ClusterGkeConfigV2Args']] gke_config_v2: The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 or above (list maxitems:1)
+        :param pulumi.Input[pulumi.InputType['ClusterGkeConfigV2Args']] gke_config_v2: The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 and above (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterK3sConfigArgs']] k3s_config: The K3S configuration for `k3s` imported Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster (map)
         :param pulumi.Input[str] name: The name of the Cluster (string)
         :param pulumi.Input[pulumi.InputType['ClusterOkeConfigArgs']] oke_config: The Oracle OKE configuration for `oke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterRke2ConfigArgs']] rke2_config: The RKE2 configuration for `rke2` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `gke_config`, `oke_config`, `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterRkeConfigArgs']] rke_config: The RKE configuration for `rke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` and `k3s_config` (list maxitems:1)
         :param pulumi.Input[bool] windows_prefered_cluster: Windows preferred cluster. Default: `false` (bool)
@@ -1745,15 +1792,15 @@
         Provides a Rancher v2 Cluster resource. This can be used to create Clusters for Rancher v2 environments and retrieve their information.
 
         ## Example Usage
 
         **Note optional/computed arguments** If any `optional/computed` argument of this resource is defined by the user, removing it from tf file will NOT reset its value. To reset it, let its definition at tf file as empty/false object. Ex: `enable_cluster_monitoring = false`, `cloud_provider {}`, `name = ""`
         ### Creating Rancher v2 RKE cluster enabling and customizing monitoring
 
-        **Note** Cluster monitoring version `0.2.0` or above, can't be enabled until cluster is fully deployed as [`kubeVersion`](https://github.com/rancher/system-charts/blob/52be656700468904b9bf15c3f39cd7112e1f8c9b/charts/rancher-monitoring/v0.2.0/Chart.yaml#L12) requirement has been introduced to helm chart
+        **Note** Cluster monitoring version `0.2.0` and above, can't be enabled until cluster is fully deployed as [`kubeVersion`](https://github.com/rancher/system-charts/blob/52be656700468904b9bf15c3f39cd7112e1f8c9b/charts/rancher-monitoring/v0.2.0/Chart.yaml#L12) requirement has been introduced to helm chart
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 RKE Cluster
         foo_custom = rancher2.Cluster("foo-custom",
@@ -1917,15 +1964,15 @@
             hostname_prefix="foo-cluster-0",
             node_template_id=foo_node_template.id,
             quantity=3,
             control_plane=True,
             etcd=True,
             worker=True)
         ```
-        ### Creating Rancher v2 RKE cluster from template. For Rancher v2.3.x or above.
+        ### Creating Rancher v2 RKE cluster from template. For Rancher v2.3.x and above.
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 cluster template
         foo_cluster_template = rancher2.ClusterTemplate("fooClusterTemplate",
@@ -1952,15 +1999,15 @@
             )],
             description="Test cluster template v2")
         # Create a new rancher2 RKE Cluster from template
         foo_cluster = rancher2.Cluster("fooCluster",
             cluster_template_id=foo_cluster_template.id,
             cluster_template_revision_id=foo_cluster_template.template_revisions[0].id)
         ```
-        ### Creating Rancher v2 RKE cluster with upgrade strategy. For Rancher v2.4.x or above.
+        ### Creating Rancher v2 RKE cluster with upgrade strategy. For Rancher v2.4.x and above.
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         foo = rancher2.Cluster("foo",
             description="Terraform custom cluster",
@@ -2001,15 +2048,59 @@
                 ),
                 upgrade_strategy=rancher2.ClusterRkeConfigUpgradeStrategyArgs(
                     drain=True,
                     max_unavailable_worker="20%",
                 ),
             ))
         ```
-        ### Importing EKS cluster to Rancher v2, using `eks_config_v2`. For Rancher v2.5.x or above.
+        ### Creating Rancher v2 RKE cluster with cluster agent customization. For Rancher v2.7.5 and above.
+
+        ```python
+        import pulumi
+        import pulumi_rancher2 as rancher2
+
+        foo = rancher2.Cluster("foo",
+            cluster_agent_deployment_customizations=[rancher2.ClusterClusterAgentDeploymentCustomizationArgs(
+                append_tolerations=[rancher2.ClusterClusterAgentDeploymentCustomizationAppendTolerationArgs(
+                    effect="NoSchedule",
+                    key="tolerate/control-plane",
+                    value="true",
+                )],
+                override_affinity=\"\"\"{
+          "nodeAffinity": {
+            "requiredDuringSchedulingIgnoredDuringExecution": {
+              "nodeSelectorTerms": [{
+                "matchExpressions": [{
+                  "key": "not.this/nodepool",
+                  "operator": "In",
+                  "values": [
+                    "true"
+                  ]
+                }]
+              }]
+            }
+          }
+        }
+
+        \"\"\",
+                override_resource_requirements=[rancher2.ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs(
+                    cpu_limit="800",
+                    cpu_request="500",
+                    memory_limit="800",
+                    memory_request="500",
+                )],
+            )],
+            description="Terraform cluster with agent customization",
+            rke_config=rancher2.ClusterRkeConfigArgs(
+                network=rancher2.ClusterRkeConfigNetworkArgs(
+                    plugin="canal",
+                ),
+            ))
+        ```
+        ### Importing EKS cluster to Rancher v2, using `eks_config_v2`. For Rancher v2.5.x and above.
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         foo_cloud_credential = rancher2.CloudCredential("fooCloudCredential",
             description="foo test",
@@ -2022,15 +2113,15 @@
             eks_config_v2=rancher2.ClusterEksConfigV2Args(
                 cloud_credential_id=foo_cloud_credential.id,
                 name="<CLUSTER_NAME>",
                 region="<EKS_REGION>",
                 imported=True,
             ))
         ```
-        ### Creating EKS cluster from Rancher v2, using `eks_config_v2`. For Rancher v2.5.x or above.
+        ### Creating EKS cluster from Rancher v2, using `eks_config_v2`. For Rancher v2.5.x and above.
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         foo_cloud_credential = rancher2.CloudCredential("fooCloudCredential",
             description="foo test",
@@ -2063,15 +2154,15 @@
                         node_role="arn:aws:iam::role/test-NodeInstanceRole",
                     ),
                 ],
                 private_access=True,
                 public_access=False,
             ))
         ```
-        ### Creating EKS cluster from Rancher v2, using `eks_config_v2` and launch template. For Rancher v2.5.6 or above.
+        ### Creating EKS cluster from Rancher v2, using `eks_config_v2` and launch template. For Rancher v2.5.6 and above.
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         foo_cloud_credential = rancher2.CloudCredential("fooCloudCredential",
             description="foo test",
@@ -2098,15 +2189,15 @@
                         version=1,
                     )],
                 )],
                 private_access=True,
                 public_access=True,
             ))
         ```
-        ### Creating AKS cluster from Rancher v2, using `aks_config_v2`. For Rancher v2.6.0 or above.
+        ### Creating AKS cluster from Rancher v2, using `aks_config_v2`. For Rancher v2.6.0 and above.
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         foo_aks = rancher2.CloudCredential("foo-aks", azure_credential_config=rancher2.CloudCredentialAzureCredentialConfigArgs(
             client_id="<CLIENT_ID>",
@@ -2322,46 +2413,46 @@
         """
         Get an existing Cluster resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterAgentEnvVarArgs']]]] agent_env_vars: Optional Agent Env Vars for Rancher agent. Just for Rancher v2.5.6 and above (list)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterAgentEnvVarArgs']]]] agent_env_vars: Optional Agent Env Vars for Rancher agent. For Rancher v2.5.6 and above (list)
         :param pulumi.Input[pulumi.InputType['ClusterAksConfigArgs']] aks_config: The Azure AKS configuration for `aks` Clusters. Conflicts with `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterAksConfigV2Args']] aks_config_v2: The Azure AKS v2 configuration for creating/import `aks` Clusters. Conflicts with `aks_config`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster (map)
         :param pulumi.Input[str] ca_cert: TLS CA certificate for etcd service (string)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterAgentDeploymentCustomizationArgs']]]] cluster_agent_deployment_customizations: Optional customization for cluster agent
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterAgentDeploymentCustomizationArgs']]]] cluster_agent_deployment_customizations: Optional customization for cluster agent. For Rancher v2.7.5 and above (list)
         :param pulumi.Input[pulumi.InputType['ClusterClusterAuthEndpointArgs']] cluster_auth_endpoint: Enabling the [local cluster authorized endpoint](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#local-cluster-auth-endpoint) allows direct communication with the cluster, bypassing the Rancher API proxy. (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterClusterMonitoringInputArgs']] cluster_monitoring_input: Cluster monitoring config. Any parameter defined in [rancher-monitoring charts](https://github.com/rancher/system-charts/tree/dev/charts/rancher-monitoring) could be configured  (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterClusterRegistrationTokenArgs']] cluster_registration_token: (Computed) Cluster Registration Token generated for the cluster (list maxitems:1)
-        :param pulumi.Input[pulumi.InputType['ClusterClusterTemplateAnswersArgs']] cluster_template_answers: Cluster template answers. Just for Rancher v2.3.x and above (list maxitems:1)
-        :param pulumi.Input[str] cluster_template_id: Cluster template ID. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterTemplateQuestionArgs']]]] cluster_template_questions: Cluster template questions. Just for Rancher v2.3.x and above (list)
-        :param pulumi.Input[str] cluster_template_revision_id: Cluster template revision ID. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster default pod security admission configuration template name
+        :param pulumi.Input[pulumi.InputType['ClusterClusterTemplateAnswersArgs']] cluster_template_answers: Cluster template answers. For Rancher v2.3.x and above (list maxitems:1)
+        :param pulumi.Input[str] cluster_template_id: Cluster template ID. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterTemplateQuestionArgs']]]] cluster_template_questions: Cluster template questions. For Rancher v2.3.x and above (list)
+        :param pulumi.Input[str] cluster_template_revision_id: Cluster template revision ID. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster default pod security admission configuration template name (string)
         :param pulumi.Input[str] default_pod_security_policy_template_id: [Default pod security policy template id](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#pod-security-policy-support) (string)
         :param pulumi.Input[str] default_project_id: (Computed) Default project ID for the cluster (string)
         :param pulumi.Input[str] description: The description for Cluster (string)
-        :param pulumi.Input[str] desired_agent_image: Desired agent image. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[str] desired_auth_image: Desired auth image. Just for Rancher v2.3.x and above (string)
-        :param pulumi.Input[str] docker_root_dir: Desired auth image. Just for Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] desired_agent_image: Desired agent image. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] desired_auth_image: Desired auth image. For Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] docker_root_dir: Desired auth image. For Rancher v2.3.x and above (string)
         :param pulumi.Input[str] driver: (Computed) The driver used for the Cluster. `imported`, `azurekubernetesservice`, `amazonelasticcontainerservice`, `googlekubernetesengine` and `rancherKubernetesEngine` are supported (string)
         :param pulumi.Input[pulumi.InputType['ClusterEksConfigArgs']] eks_config: The Amazon EKS configuration for `eks` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
-        :param pulumi.Input[pulumi.InputType['ClusterEksConfigV2Args']] eks_config_v2: The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x or above (list maxitems:1)
+        :param pulumi.Input[pulumi.InputType['ClusterEksConfigV2Args']] eks_config_v2: The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x and above (list maxitems:1)
         :param pulumi.Input[bool] enable_cluster_alerting: Enable built-in cluster alerting (bool)
         :param pulumi.Input[bool] enable_cluster_istio: Deploy istio on `system` project and `istio-system` namespace, using App resource instead. See above example.
         :param pulumi.Input[bool] enable_cluster_monitoring: Enable built-in cluster monitoring (bool)
         :param pulumi.Input[bool] enable_network_policy: Enable project network isolation (bool)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterFleetAgentDeploymentCustomizationArgs']]]] fleet_agent_deployment_customizations: Optional customization for fleet agent
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterFleetAgentDeploymentCustomizationArgs']]]] fleet_agent_deployment_customizations: Optional customization for fleet agent. For Rancher v2.7.5 and above (list)
         :param pulumi.Input[str] fleet_workspace_name: Fleet workspace name (string)
         :param pulumi.Input[pulumi.InputType['ClusterGkeConfigArgs']] gke_config: The Google GKE configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config_v2`, `oke_config`, `k3s_config` and `rke_config` (list maxitems:1)
-        :param pulumi.Input[pulumi.InputType['ClusterGkeConfigV2Args']] gke_config_v2: The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 or above (list maxitems:1)
-        :param pulumi.Input[bool] istio_enabled: (Computed) Is istio enabled at cluster? Just for Rancher v2.3.x and above (bool)
+        :param pulumi.Input[pulumi.InputType['ClusterGkeConfigV2Args']] gke_config_v2: The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 and above (list maxitems:1)
+        :param pulumi.Input[bool] istio_enabled: (Computed) Is istio enabled at cluster? For Rancher v2.3.x and above (bool)
         :param pulumi.Input[pulumi.InputType['ClusterK3sConfigArgs']] k3s_config: The K3S configuration for `k3s` imported Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[str] kube_config: (Computed/Sensitive) Kube Config generated for the cluster. Note: For Rancher 2.6.0 and above, when the cluster has `cluster_auth_endpoint` enabled, the kube_config will not be available until the cluster is `connected` (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster (map)
         :param pulumi.Input[str] name: The name of the Cluster (string)
         :param pulumi.Input[pulumi.InputType['ClusterOkeConfigArgs']] oke_config: The Oracle OKE configuration for `oke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterRke2ConfigArgs']] rke2_config: The RKE2 configuration for `rke2` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `gke_config`, `oke_config`, `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterRkeConfigArgs']] rke_config: The RKE configuration for `rke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` and `k3s_config` (list maxitems:1)
@@ -2415,15 +2506,15 @@
         __props__.__dict__["windows_prefered_cluster"] = windows_prefered_cluster
         return Cluster(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="agentEnvVars")
     def agent_env_vars(self) -> pulumi.Output[Optional[Sequence['outputs.ClusterAgentEnvVar']]]:
         """
-        Optional Agent Env Vars for Rancher agent. Just for Rancher v2.5.6 and above (list)
+        Optional Agent Env Vars for Rancher agent. For Rancher v2.5.6 and above (list)
         """
         return pulumi.get(self, "agent_env_vars")
 
     @property
     @pulumi.getter(name="aksConfig")
     def aks_config(self) -> pulumi.Output[Optional['outputs.ClusterAksConfig']]:
         """
@@ -2455,15 +2546,15 @@
         """
         return pulumi.get(self, "ca_cert")
 
     @property
     @pulumi.getter(name="clusterAgentDeploymentCustomizations")
     def cluster_agent_deployment_customizations(self) -> pulumi.Output[Optional[Sequence['outputs.ClusterClusterAgentDeploymentCustomization']]]:
         """
-        Optional customization for cluster agent
+        Optional customization for cluster agent. For Rancher v2.7.5 and above (list)
         """
         return pulumi.get(self, "cluster_agent_deployment_customizations")
 
     @property
     @pulumi.getter(name="clusterAuthEndpoint")
     def cluster_auth_endpoint(self) -> pulumi.Output['outputs.ClusterClusterAuthEndpoint']:
         """
@@ -2487,47 +2578,47 @@
         """
         return pulumi.get(self, "cluster_registration_token")
 
     @property
     @pulumi.getter(name="clusterTemplateAnswers")
     def cluster_template_answers(self) -> pulumi.Output['outputs.ClusterClusterTemplateAnswers']:
         """
-        Cluster template answers. Just for Rancher v2.3.x and above (list maxitems:1)
+        Cluster template answers. For Rancher v2.3.x and above (list maxitems:1)
         """
         return pulumi.get(self, "cluster_template_answers")
 
     @property
     @pulumi.getter(name="clusterTemplateId")
     def cluster_template_id(self) -> pulumi.Output[Optional[str]]:
         """
-        Cluster template ID. Just for Rancher v2.3.x and above (string)
+        Cluster template ID. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "cluster_template_id")
 
     @property
     @pulumi.getter(name="clusterTemplateQuestions")
     def cluster_template_questions(self) -> pulumi.Output[Sequence['outputs.ClusterClusterTemplateQuestion']]:
         """
-        Cluster template questions. Just for Rancher v2.3.x and above (list)
+        Cluster template questions. For Rancher v2.3.x and above (list)
         """
         return pulumi.get(self, "cluster_template_questions")
 
     @property
     @pulumi.getter(name="clusterTemplateRevisionId")
     def cluster_template_revision_id(self) -> pulumi.Output[Optional[str]]:
         """
-        Cluster template revision ID. Just for Rancher v2.3.x and above (string)
+        Cluster template revision ID. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "cluster_template_revision_id")
 
     @property
     @pulumi.getter(name="defaultPodSecurityAdmissionConfigurationTemplateName")
     def default_pod_security_admission_configuration_template_name(self) -> pulumi.Output[str]:
         """
-        Cluster default pod security admission configuration template name
+        Cluster default pod security admission configuration template name (string)
         """
         return pulumi.get(self, "default_pod_security_admission_configuration_template_name")
 
     @property
     @pulumi.getter(name="defaultPodSecurityPolicyTemplateId")
     def default_pod_security_policy_template_id(self) -> pulumi.Output[str]:
         """
@@ -2551,31 +2642,31 @@
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="desiredAgentImage")
     def desired_agent_image(self) -> pulumi.Output[str]:
         """
-        Desired agent image. Just for Rancher v2.3.x and above (string)
+        Desired agent image. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "desired_agent_image")
 
     @property
     @pulumi.getter(name="desiredAuthImage")
     def desired_auth_image(self) -> pulumi.Output[str]:
         """
-        Desired auth image. Just for Rancher v2.3.x and above (string)
+        Desired auth image. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "desired_auth_image")
 
     @property
     @pulumi.getter(name="dockerRootDir")
     def docker_root_dir(self) -> pulumi.Output[str]:
         """
-        Desired auth image. Just for Rancher v2.3.x and above (string)
+        Desired auth image. For Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "docker_root_dir")
 
     @property
     @pulumi.getter
     def driver(self) -> pulumi.Output[str]:
         """
@@ -2591,15 +2682,15 @@
         """
         return pulumi.get(self, "eks_config")
 
     @property
     @pulumi.getter(name="eksConfigV2")
     def eks_config_v2(self) -> pulumi.Output['outputs.ClusterEksConfigV2']:
         """
-        The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x or above (list maxitems:1)
+        The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x and above (list maxitems:1)
         """
         return pulumi.get(self, "eks_config_v2")
 
     @property
     @pulumi.getter(name="enableClusterAlerting")
     def enable_cluster_alerting(self) -> pulumi.Output[bool]:
         """
@@ -2609,14 +2700,17 @@
 
     @property
     @pulumi.getter(name="enableClusterIstio")
     def enable_cluster_istio(self) -> pulumi.Output[bool]:
         """
         Deploy istio on `system` project and `istio-system` namespace, using App resource instead. See above example.
         """
+        warnings.warn("""Deploy istio using rancher2_app resource instead""", DeprecationWarning)
+        pulumi.log.warn("""enable_cluster_istio is deprecated: Deploy istio using rancher2_app resource instead""")
+
         return pulumi.get(self, "enable_cluster_istio")
 
     @property
     @pulumi.getter(name="enableClusterMonitoring")
     def enable_cluster_monitoring(self) -> pulumi.Output[bool]:
         """
         Enable built-in cluster monitoring (bool)
@@ -2631,15 +2725,15 @@
         """
         return pulumi.get(self, "enable_network_policy")
 
     @property
     @pulumi.getter(name="fleetAgentDeploymentCustomizations")
     def fleet_agent_deployment_customizations(self) -> pulumi.Output[Optional[Sequence['outputs.ClusterFleetAgentDeploymentCustomization']]]:
         """
-        Optional customization for fleet agent
+        Optional customization for fleet agent. For Rancher v2.7.5 and above (list)
         """
         return pulumi.get(self, "fleet_agent_deployment_customizations")
 
     @property
     @pulumi.getter(name="fleetWorkspaceName")
     def fleet_workspace_name(self) -> pulumi.Output[str]:
         """
@@ -2655,23 +2749,23 @@
         """
         return pulumi.get(self, "gke_config")
 
     @property
     @pulumi.getter(name="gkeConfigV2")
     def gke_config_v2(self) -> pulumi.Output[Optional['outputs.ClusterGkeConfigV2']]:
         """
-        The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 or above (list maxitems:1)
+        The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 and above (list maxitems:1)
         """
         return pulumi.get(self, "gke_config_v2")
 
     @property
     @pulumi.getter(name="istioEnabled")
     def istio_enabled(self) -> pulumi.Output[bool]:
         """
-        (Computed) Is istio enabled at cluster? Just for Rancher v2.3.x and above (bool)
+        (Computed) Is istio enabled at cluster? For Rancher v2.3.x and above (bool)
         """
         return pulumi.get(self, "istio_enabled")
 
     @property
     @pulumi.getter(name="k3sConfig")
     def k3s_config(self) -> pulumi.Output['outputs.ClusterK3sConfig']:
         """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_alert_group.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_alert_rule.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_alter_group.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_alter_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_alter_rule.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_alter_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_driver.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_role_template_binding.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_role_template_binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         :param pulumi.Input[str] cluster_id: The cluster id where bind cluster role template binding (string)
         :param pulumi.Input[str] role_template_id: The role template id from create cluster role template binding (string)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for cluster role template binding (map)
         :param pulumi.Input[str] group_id: The group ID to assign cluster role template binding (string)
         :param pulumi.Input[str] group_principal_id: The group_principal ID to assign cluster role template binding (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for cluster role template binding (map)
                
-               **Note** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
+               **Note:** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
         :param pulumi.Input[str] name: The name of the cluster role template binding (string)
         :param pulumi.Input[str] user_id: The user ID to assign cluster role template binding (string)
         :param pulumi.Input[str] user_principal_id: The user_principal ID to assign cluster role template binding (string)
         """
         pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "role_template_id", role_template_id)
         if annotations is not None:
@@ -116,15 +116,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Labels for cluster role template binding (map)
 
-        **Note** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
+        **Note:** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "labels", value)
 
@@ -181,15 +181,15 @@
         Input properties used for looking up and filtering ClusterRoleTemplateBinding resources.
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for cluster role template binding (map)
         :param pulumi.Input[str] cluster_id: The cluster id where bind cluster role template binding (string)
         :param pulumi.Input[str] group_id: The group ID to assign cluster role template binding (string)
         :param pulumi.Input[str] group_principal_id: The group_principal ID to assign cluster role template binding (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for cluster role template binding (map)
                
-               **Note** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
+               **Note:** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
         :param pulumi.Input[str] name: The name of the cluster role template binding (string)
         :param pulumi.Input[str] role_template_id: The role template id from create cluster role template binding (string)
         :param pulumi.Input[str] user_id: The user ID to assign cluster role template binding (string)
         :param pulumi.Input[str] user_principal_id: The user_principal ID to assign cluster role template binding (string)
         """
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
@@ -260,15 +260,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Labels for cluster role template binding (map)
 
-        **Note** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
+        **Note:** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "labels", value)
 
@@ -364,15 +364,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for cluster role template binding (map)
         :param pulumi.Input[str] cluster_id: The cluster id where bind cluster role template binding (string)
         :param pulumi.Input[str] group_id: The group ID to assign cluster role template binding (string)
         :param pulumi.Input[str] group_principal_id: The group_principal ID to assign cluster role template binding (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for cluster role template binding (map)
                
-               **Note** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
+               **Note:** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
         :param pulumi.Input[str] name: The name of the cluster role template binding (string)
         :param pulumi.Input[str] role_template_id: The role template id from create cluster role template binding (string)
         :param pulumi.Input[str] user_id: The user ID to assign cluster role template binding (string)
         :param pulumi.Input[str] user_principal_id: The user_principal ID to assign cluster role template binding (string)
         """
         ...
     @overload
@@ -478,15 +478,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for cluster role template binding (map)
         :param pulumi.Input[str] cluster_id: The cluster id where bind cluster role template binding (string)
         :param pulumi.Input[str] group_id: The group ID to assign cluster role template binding (string)
         :param pulumi.Input[str] group_principal_id: The group_principal ID to assign cluster role template binding (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for cluster role template binding (map)
                
-               **Note** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
+               **Note:** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
         :param pulumi.Input[str] name: The name of the cluster role template binding (string)
         :param pulumi.Input[str] role_template_id: The role template id from create cluster role template binding (string)
         :param pulumi.Input[str] user_id: The user ID to assign cluster role template binding (string)
         :param pulumi.Input[str] user_principal_id: The user_principal ID to assign cluster role template binding (string)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -537,15 +537,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> pulumi.Output[Mapping[str, Any]]:
         """
         Labels for cluster role template binding (map)
 
-        **Note** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
+        **Note:** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_sync.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                  wait_monitoring: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ClusterSync resource.
         :param pulumi.Input[str] cluster_id: The cluster ID that is syncing (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] node_pool_ids: The node pool IDs used by the cluster id (list)
         :param pulumi.Input[int] state_confirm: Wait until active status is confirmed a number of times (wait interval of 5s). Default: `1` means no confirmation (int)
                
-               **Note** `state_confirm` would be useful, if you have troubles for creating/updating custom clusters that eventually are reaching `active` state before they are fully installed. For example: setting `state_confirm = 2` will assure that the cluster has been in `active` state for at least 5 seconds, `state_confirm = 3` assure at least 10 seconds, etc
+               **Note:** `state_confirm` would be useful, if you have troubles for creating/updating custom clusters that eventually are reaching `active` state before they are fully installed. For example: setting `state_confirm = 2` will assure that the cluster has been in `active` state for at least 5 seconds, `state_confirm = 3` assure at least 10 seconds, etc
         :param pulumi.Input[bool] wait_alerting: Wait until alerting is up and running. Default: `false` (bool)
         :param pulumi.Input[bool] wait_catalogs: Wait until all catalogs are downloaded and active. Default: `false` (bool)
         :param pulumi.Input[bool] wait_monitoring: Wait until monitoring is up and running. Default: `false` (bool)
         """
         pulumi.set(__self__, "cluster_id", cluster_id)
         if node_pool_ids is not None:
             pulumi.set(__self__, "node_pool_ids", node_pool_ids)
@@ -74,15 +74,15 @@
 
     @property
     @pulumi.getter(name="stateConfirm")
     def state_confirm(self) -> Optional[pulumi.Input[int]]:
         """
         Wait until active status is confirmed a number of times (wait interval of 5s). Default: `1` means no confirmation (int)
 
-        **Note** `state_confirm` would be useful, if you have troubles for creating/updating custom clusters that eventually are reaching `active` state before they are fully installed. For example: setting `state_confirm = 2` will assure that the cluster has been in `active` state for at least 5 seconds, `state_confirm = 3` assure at least 10 seconds, etc
+        **Note:** `state_confirm` would be useful, if you have troubles for creating/updating custom clusters that eventually are reaching `active` state before they are fully installed. For example: setting `state_confirm = 2` will assure that the cluster has been in `active` state for at least 5 seconds, `state_confirm = 3` assure at least 10 seconds, etc
         """
         return pulumi.get(self, "state_confirm")
 
     @state_confirm.setter
     def state_confirm(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "state_confirm", value)
 
@@ -151,15 +151,15 @@
         :param pulumi.Input[str] cluster_id: The cluster ID that is syncing (string)
         :param pulumi.Input[str] default_project_id: (Computed) Default project ID for the cluster sync (string)
         :param pulumi.Input[str] kube_config: (Computed/Sensitive) Kube Config generated for the cluster sync (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] node_pool_ids: The node pool IDs used by the cluster id (list)
         :param pulumi.Input[Sequence[pulumi.Input['ClusterSyncNodeArgs']]] nodes: (Computed) The cluster nodes (list).
         :param pulumi.Input[int] state_confirm: Wait until active status is confirmed a number of times (wait interval of 5s). Default: `1` means no confirmation (int)
                
-               **Note** `state_confirm` would be useful, if you have troubles for creating/updating custom clusters that eventually are reaching `active` state before they are fully installed. For example: setting `state_confirm = 2` will assure that the cluster has been in `active` state for at least 5 seconds, `state_confirm = 3` assure at least 10 seconds, etc
+               **Note:** `state_confirm` would be useful, if you have troubles for creating/updating custom clusters that eventually are reaching `active` state before they are fully installed. For example: setting `state_confirm = 2` will assure that the cluster has been in `active` state for at least 5 seconds, `state_confirm = 3` assure at least 10 seconds, etc
         :param pulumi.Input[str] system_project_id: (Computed) System project ID for the cluster sync (string)
         :param pulumi.Input[bool] wait_alerting: Wait until alerting is up and running. Default: `false` (bool)
         :param pulumi.Input[bool] wait_catalogs: Wait until all catalogs are downloaded and active. Default: `false` (bool)
         :param pulumi.Input[bool] wait_monitoring: Wait until monitoring is up and running. Default: `false` (bool)
         """
         if cluster_id is not None:
             pulumi.set(__self__, "cluster_id", cluster_id)
@@ -246,15 +246,15 @@
 
     @property
     @pulumi.getter(name="stateConfirm")
     def state_confirm(self) -> Optional[pulumi.Input[int]]:
         """
         Wait until active status is confirmed a number of times (wait interval of 5s). Default: `1` means no confirmation (int)
 
-        **Note** `state_confirm` would be useful, if you have troubles for creating/updating custom clusters that eventually are reaching `active` state before they are fully installed. For example: setting `state_confirm = 2` will assure that the cluster has been in `active` state for at least 5 seconds, `state_confirm = 3` assure at least 10 seconds, etc
+        **Note:** `state_confirm` would be useful, if you have troubles for creating/updating custom clusters that eventually are reaching `active` state before they are fully installed. For example: setting `state_confirm = 2` will assure that the cluster has been in `active` state for at least 5 seconds, `state_confirm = 3` assure at least 10 seconds, etc
         """
         return pulumi.get(self, "state_confirm")
 
     @state_confirm.setter
     def state_confirm(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "state_confirm", value)
 
@@ -396,15 +396,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: The cluster ID that is syncing (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] node_pool_ids: The node pool IDs used by the cluster id (list)
         :param pulumi.Input[int] state_confirm: Wait until active status is confirmed a number of times (wait interval of 5s). Default: `1` means no confirmation (int)
                
-               **Note** `state_confirm` would be useful, if you have troubles for creating/updating custom clusters that eventually are reaching `active` state before they are fully installed. For example: setting `state_confirm = 2` will assure that the cluster has been in `active` state for at least 5 seconds, `state_confirm = 3` assure at least 10 seconds, etc
+               **Note:** `state_confirm` would be useful, if you have troubles for creating/updating custom clusters that eventually are reaching `active` state before they are fully installed. For example: setting `state_confirm = 2` will assure that the cluster has been in `active` state for at least 5 seconds, `state_confirm = 3` assure at least 10 seconds, etc
         :param pulumi.Input[bool] wait_alerting: Wait until alerting is up and running. Default: `false` (bool)
         :param pulumi.Input[bool] wait_catalogs: Wait until all catalogs are downloaded and active. Default: `false` (bool)
         :param pulumi.Input[bool] wait_monitoring: Wait until monitoring is up and running. Default: `false` (bool)
         """
         ...
     @overload
     def __init__(__self__,
@@ -553,15 +553,15 @@
         :param pulumi.Input[str] cluster_id: The cluster ID that is syncing (string)
         :param pulumi.Input[str] default_project_id: (Computed) Default project ID for the cluster sync (string)
         :param pulumi.Input[str] kube_config: (Computed/Sensitive) Kube Config generated for the cluster sync (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] node_pool_ids: The node pool IDs used by the cluster id (list)
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterSyncNodeArgs']]]] nodes: (Computed) The cluster nodes (list).
         :param pulumi.Input[int] state_confirm: Wait until active status is confirmed a number of times (wait interval of 5s). Default: `1` means no confirmation (int)
                
-               **Note** `state_confirm` would be useful, if you have troubles for creating/updating custom clusters that eventually are reaching `active` state before they are fully installed. For example: setting `state_confirm = 2` will assure that the cluster has been in `active` state for at least 5 seconds, `state_confirm = 3` assure at least 10 seconds, etc
+               **Note:** `state_confirm` would be useful, if you have troubles for creating/updating custom clusters that eventually are reaching `active` state before they are fully installed. For example: setting `state_confirm = 2` will assure that the cluster has been in `active` state for at least 5 seconds, `state_confirm = 3` assure at least 10 seconds, etc
         :param pulumi.Input[str] system_project_id: (Computed) System project ID for the cluster sync (string)
         :param pulumi.Input[bool] wait_alerting: Wait until alerting is up and running. Default: `false` (bool)
         :param pulumi.Input[bool] wait_catalogs: Wait until all catalogs are downloaded and active. Default: `false` (bool)
         :param pulumi.Input[bool] wait_monitoring: Wait until monitoring is up and running. Default: `false` (bool)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -622,15 +622,15 @@
 
     @property
     @pulumi.getter(name="stateConfirm")
     def state_confirm(self) -> pulumi.Output[Optional[int]]:
         """
         Wait until active status is confirmed a number of times (wait interval of 5s). Default: `1` means no confirmation (int)
 
-        **Note** `state_confirm` would be useful, if you have troubles for creating/updating custom clusters that eventually are reaching `active` state before they are fully installed. For example: setting `state_confirm = 2` will assure that the cluster has been in `active` state for at least 5 seconds, `state_confirm = 3` assure at least 10 seconds, etc
+        **Note:** `state_confirm` would be useful, if you have troubles for creating/updating custom clusters that eventually are reaching `active` state before they are fully installed. For example: setting `state_confirm = 2` will assure that the cluster has been in `active` state for at least 5 seconds, `state_confirm = 3` assure at least 10 seconds, etc
         """
         return pulumi.get(self, "state_confirm")
 
     @property
     @pulumi.getter
     def synced(self) -> pulumi.Output[Optional[bool]]:
         return pulumi.get(self, "synced")
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_template.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
                     ),
                 ),
                 default=True,
                 name="V1",
             )])
         ```
 
-        Creating Rancher v2 RKE cluster template with upgrade strategy. For Rancher v2.4.x or above.
+        Creating Rancher v2 RKE cluster template with upgrade strategy. For Rancher v2.4.x and above.
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Cluster Template
         foo = rancher2.ClusterTemplate("foo",
@@ -378,15 +378,15 @@
                     ),
                 ),
                 default=True,
                 name="V1",
             )])
         ```
 
-        Creating Rancher v2 RKE cluster template with upgrade strategy. For Rancher v2.4.x or above.
+        Creating Rancher v2 RKE cluster template with upgrade strategy. For Rancher v2.4.x and above.
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Cluster Template
         foo = rancher2.ClusterTemplate("foo",
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/cluster_v2.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/cluster_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,20 +33,20 @@
                  rke_config: Optional[pulumi.Input['ClusterV2RkeConfigArgs']] = None):
         """
         The set of arguments for constructing a ClusterV2 resource.
         :param pulumi.Input[str] kubernetes_version: The kubernetes version of the Cluster v2 (list maxitems:1)
         :param pulumi.Input[Sequence[pulumi.Input['ClusterV2AgentEnvVarArgs']]] agent_env_vars: Optional Agent Env Vars for Rancher agent (list)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster V2 (map)
         :param pulumi.Input[str] cloud_credential_secret_name: Cluster V2 cloud credential secret name (string)
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]] cluster_agent_deployment_customizations: Optional customization for cluster agent
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]] cluster_agent_deployment_customizations: Optional customization for cluster agent (list)
         :param pulumi.Input[str] default_cluster_role_for_project_members: Cluster V2 default cluster role for project members (string)
         :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster V2 default pod security admission configuration template name (string)
         :param pulumi.Input[str] default_pod_security_policy_template_name: Cluster V2 default pod security policy template name (string)
         :param pulumi.Input[bool] enable_network_policy: Enable k8s network policy at Cluster V2 (bool)
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]] fleet_agent_deployment_customizations: Optional customization for fleet agent
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]] fleet_agent_deployment_customizations: Optional customization for fleet agent (list)
         :param pulumi.Input[str] fleet_namespace: The fleet namespace of the Cluster v2. Default: `\\"fleet-default\\"` (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster V2 (map)
         :param pulumi.Input['ClusterV2LocalAuthEndpointArgs'] local_auth_endpoint: Cluster V2 local auth endpoint (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Cluster v2 (string)
         :param pulumi.Input['ClusterV2RkeConfigArgs'] rke_config: The RKE configuration for `k3s` and `rke2` Clusters v2. (list maxitems:1)
         """
         pulumi.set(__self__, "kubernetes_version", kubernetes_version)
@@ -127,15 +127,15 @@
     def cloud_credential_secret_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cloud_credential_secret_name", value)
 
     @property
     @pulumi.getter(name="clusterAgentDeploymentCustomizations")
     def cluster_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]]:
         """
-        Optional customization for cluster agent
+        Optional customization for cluster agent (list)
         """
         return pulumi.get(self, "cluster_agent_deployment_customizations")
 
     @cluster_agent_deployment_customizations.setter
     def cluster_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]]):
         pulumi.set(self, "cluster_agent_deployment_customizations", value)
 
@@ -187,15 +187,15 @@
     def enable_network_policy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_network_policy", value)
 
     @property
     @pulumi.getter(name="fleetAgentDeploymentCustomizations")
     def fleet_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]]]:
         """
-        Optional customization for fleet agent
+        Optional customization for fleet agent (list)
         """
         return pulumi.get(self, "fleet_agent_deployment_customizations")
 
     @fleet_agent_deployment_customizations.setter
     def fleet_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]]]):
         pulumi.set(self, "fleet_agent_deployment_customizations", value)
 
@@ -283,22 +283,22 @@
                  resource_version: Optional[pulumi.Input[str]] = None,
                  rke_config: Optional[pulumi.Input['ClusterV2RkeConfigArgs']] = None):
         """
         Input properties used for looking up and filtering ClusterV2 resources.
         :param pulumi.Input[Sequence[pulumi.Input['ClusterV2AgentEnvVarArgs']]] agent_env_vars: Optional Agent Env Vars for Rancher agent (list)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster V2 (map)
         :param pulumi.Input[str] cloud_credential_secret_name: Cluster V2 cloud credential secret name (string)
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]] cluster_agent_deployment_customizations: Optional customization for cluster agent
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]] cluster_agent_deployment_customizations: Optional customization for cluster agent (list)
         :param pulumi.Input['ClusterV2ClusterRegistrationTokenArgs'] cluster_registration_token: (Computed/Sensitive) Cluster Registration Token generated for the cluster v2 (list maxitems:1)
         :param pulumi.Input[str] cluster_v1_id: (Computed) Cluster v1 id for cluster v2. (e.g to be used with `rancher2_sync`) (string)
         :param pulumi.Input[str] default_cluster_role_for_project_members: Cluster V2 default cluster role for project members (string)
         :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster V2 default pod security admission configuration template name (string)
         :param pulumi.Input[str] default_pod_security_policy_template_name: Cluster V2 default pod security policy template name (string)
         :param pulumi.Input[bool] enable_network_policy: Enable k8s network policy at Cluster V2 (bool)
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]] fleet_agent_deployment_customizations: Optional customization for fleet agent
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]] fleet_agent_deployment_customizations: Optional customization for fleet agent (list)
         :param pulumi.Input[str] fleet_namespace: The fleet namespace of the Cluster v2. Default: `\\"fleet-default\\"` (string)
         :param pulumi.Input[str] kube_config: (Computed/Sensitive) Kube Config generated for the cluster v2. Note: When the cluster has `local_auth_endpoint` enabled, the kube_config will not be available until the cluster is `connected` (string)
         :param pulumi.Input[str] kubernetes_version: The kubernetes version of the Cluster v2 (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster V2 (map)
         :param pulumi.Input['ClusterV2LocalAuthEndpointArgs'] local_auth_endpoint: Cluster V2 local auth endpoint (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Cluster v2 (string)
         :param pulumi.Input[str] resource_version: (Computed) Cluster v2 k8s resource version (string)
@@ -379,15 +379,15 @@
     def cloud_credential_secret_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cloud_credential_secret_name", value)
 
     @property
     @pulumi.getter(name="clusterAgentDeploymentCustomizations")
     def cluster_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]]:
         """
-        Optional customization for cluster agent
+        Optional customization for cluster agent (list)
         """
         return pulumi.get(self, "cluster_agent_deployment_customizations")
 
     @cluster_agent_deployment_customizations.setter
     def cluster_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]]):
         pulumi.set(self, "cluster_agent_deployment_customizations", value)
 
@@ -463,15 +463,15 @@
     def enable_network_policy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_network_policy", value)
 
     @property
     @pulumi.getter(name="fleetAgentDeploymentCustomizations")
     def fleet_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]]]:
         """
-        Optional customization for fleet agent
+        Optional customization for fleet agent (list)
         """
         return pulumi.get(self, "fleet_agent_deployment_customizations")
 
     @fleet_agent_deployment_customizations.setter
     def fleet_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]]]):
         pulumi.set(self, "fleet_agent_deployment_customizations", value)
 
@@ -590,85 +590,47 @@
                  kubernetes_version: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  local_auth_endpoint: Optional[pulumi.Input[pulumi.InputType['ClusterV2LocalAuthEndpointArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  rke_config: Optional[pulumi.Input[pulumi.InputType['ClusterV2RkeConfigArgs']]] = None,
                  __props__=None):
         """
-        Provides a Rancher v2 Cluster v2 resource. This can be used to create RKE2 and K3S Clusters for Rancher v2 environments and retrieve their information. This resource is available from Rancher v2.6.0 and above.
-
-        ## Example Usage
-        ### Creating Rancher v2 custom cluster v2
-
-        ```python
-        import pulumi
-        import pulumi_rancher2 as rancher2
-
-        # Create a new rancher v2 K3S custom Cluster v2
-        foo = rancher2.ClusterV2("foo",
-            default_cluster_role_for_project_members="user",
-            enable_network_policy=False,
-            fleet_namespace="fleet-ns",
-            kubernetes_version="v1.21.4+k3s1")
-        ```
-
-        **Note** Once created, get the node command from `rancher2_cluster_v2.foo.cluster_registration_token`
-
         ## Import
 
         Clusters v2 can be imported using the Rancher Cluster v2 ID, that is in the form &lt;FLEET_NAMESPACE&gt;/&lt;CLUSTER_NAME&gt;
 
         ```sh
          $ pulumi import rancher2:index/clusterV2:ClusterV2 foo &lt;FLEET_NAMESPACE&gt;/&lt;CLUSTER_NAME&gt;
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2AgentEnvVarArgs']]]] agent_env_vars: Optional Agent Env Vars for Rancher agent (list)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster V2 (map)
         :param pulumi.Input[str] cloud_credential_secret_name: Cluster V2 cloud credential secret name (string)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]] cluster_agent_deployment_customizations: Optional customization for cluster agent
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]] cluster_agent_deployment_customizations: Optional customization for cluster agent (list)
         :param pulumi.Input[str] default_cluster_role_for_project_members: Cluster V2 default cluster role for project members (string)
         :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster V2 default pod security admission configuration template name (string)
         :param pulumi.Input[str] default_pod_security_policy_template_name: Cluster V2 default pod security policy template name (string)
         :param pulumi.Input[bool] enable_network_policy: Enable k8s network policy at Cluster V2 (bool)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2FleetAgentDeploymentCustomizationArgs']]]] fleet_agent_deployment_customizations: Optional customization for fleet agent
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2FleetAgentDeploymentCustomizationArgs']]]] fleet_agent_deployment_customizations: Optional customization for fleet agent (list)
         :param pulumi.Input[str] fleet_namespace: The fleet namespace of the Cluster v2. Default: `\\"fleet-default\\"` (string)
         :param pulumi.Input[str] kubernetes_version: The kubernetes version of the Cluster v2 (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster V2 (map)
         :param pulumi.Input[pulumi.InputType['ClusterV2LocalAuthEndpointArgs']] local_auth_endpoint: Cluster V2 local auth endpoint (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Cluster v2 (string)
         :param pulumi.Input[pulumi.InputType['ClusterV2RkeConfigArgs']] rke_config: The RKE configuration for `k3s` and `rke2` Clusters v2. (list maxitems:1)
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ClusterV2Args,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Provides a Rancher v2 Cluster v2 resource. This can be used to create RKE2 and K3S Clusters for Rancher v2 environments and retrieve their information. This resource is available from Rancher v2.6.0 and above.
-
-        ## Example Usage
-        ### Creating Rancher v2 custom cluster v2
-
-        ```python
-        import pulumi
-        import pulumi_rancher2 as rancher2
-
-        # Create a new rancher v2 K3S custom Cluster v2
-        foo = rancher2.ClusterV2("foo",
-            default_cluster_role_for_project_members="user",
-            enable_network_policy=False,
-            fleet_namespace="fleet-ns",
-            kubernetes_version="v1.21.4+k3s1")
-        ```
-
-        **Note** Once created, get the node command from `rancher2_cluster_v2.foo.cluster_registration_token`
-
         ## Import
 
         Clusters v2 can be imported using the Rancher Cluster v2 ID, that is in the form &lt;FLEET_NAMESPACE&gt;/&lt;CLUSTER_NAME&gt;
 
         ```sh
          $ pulumi import rancher2:index/clusterV2:ClusterV2 foo &lt;FLEET_NAMESPACE&gt;/&lt;CLUSTER_NAME&gt;
         ```
@@ -770,22 +732,22 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2AgentEnvVarArgs']]]] agent_env_vars: Optional Agent Env Vars for Rancher agent (list)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster V2 (map)
         :param pulumi.Input[str] cloud_credential_secret_name: Cluster V2 cloud credential secret name (string)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]] cluster_agent_deployment_customizations: Optional customization for cluster agent
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]] cluster_agent_deployment_customizations: Optional customization for cluster agent (list)
         :param pulumi.Input[pulumi.InputType['ClusterV2ClusterRegistrationTokenArgs']] cluster_registration_token: (Computed/Sensitive) Cluster Registration Token generated for the cluster v2 (list maxitems:1)
         :param pulumi.Input[str] cluster_v1_id: (Computed) Cluster v1 id for cluster v2. (e.g to be used with `rancher2_sync`) (string)
         :param pulumi.Input[str] default_cluster_role_for_project_members: Cluster V2 default cluster role for project members (string)
         :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster V2 default pod security admission configuration template name (string)
         :param pulumi.Input[str] default_pod_security_policy_template_name: Cluster V2 default pod security policy template name (string)
         :param pulumi.Input[bool] enable_network_policy: Enable k8s network policy at Cluster V2 (bool)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2FleetAgentDeploymentCustomizationArgs']]]] fleet_agent_deployment_customizations: Optional customization for fleet agent
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2FleetAgentDeploymentCustomizationArgs']]]] fleet_agent_deployment_customizations: Optional customization for fleet agent (list)
         :param pulumi.Input[str] fleet_namespace: The fleet namespace of the Cluster v2. Default: `\\"fleet-default\\"` (string)
         :param pulumi.Input[str] kube_config: (Computed/Sensitive) Kube Config generated for the cluster v2. Note: When the cluster has `local_auth_endpoint` enabled, the kube_config will not be available until the cluster is `connected` (string)
         :param pulumi.Input[str] kubernetes_version: The kubernetes version of the Cluster v2 (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster V2 (map)
         :param pulumi.Input[pulumi.InputType['ClusterV2LocalAuthEndpointArgs']] local_auth_endpoint: Cluster V2 local auth endpoint (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Cluster v2 (string)
         :param pulumi.Input[str] resource_version: (Computed) Cluster v2 k8s resource version (string)
@@ -840,15 +802,15 @@
         """
         return pulumi.get(self, "cloud_credential_secret_name")
 
     @property
     @pulumi.getter(name="clusterAgentDeploymentCustomizations")
     def cluster_agent_deployment_customizations(self) -> pulumi.Output[Optional[Sequence['outputs.ClusterV2ClusterAgentDeploymentCustomization']]]:
         """
-        Optional customization for cluster agent
+        Optional customization for cluster agent (list)
         """
         return pulumi.get(self, "cluster_agent_deployment_customizations")
 
     @property
     @pulumi.getter(name="clusterRegistrationToken")
     def cluster_registration_token(self) -> pulumi.Output['outputs.ClusterV2ClusterRegistrationToken']:
         """
@@ -896,15 +858,15 @@
         """
         return pulumi.get(self, "enable_network_policy")
 
     @property
     @pulumi.getter(name="fleetAgentDeploymentCustomizations")
     def fleet_agent_deployment_customizations(self) -> pulumi.Output[Optional[Sequence['outputs.ClusterV2FleetAgentDeploymentCustomization']]]:
         """
-        Optional customization for fleet agent
+        Optional customization for fleet agent (list)
         """
         return pulumi.get(self, "fleet_agent_deployment_customizations")
 
     @property
     @pulumi.getter(name="fleetNamespace")
     def fleet_namespace(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/config/vars.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/config_map_v2.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/custom_user_token.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/custom_user_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/etcd_backup.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/etcd_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/feature.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         """
         Provides a Rancher v2 Feature resource. This can be used to enable/disable [experimental features](https://rancher.com/docs/rancher/v2.x/en/installation/resources/feature-flags/) for Rancher v2 environments.
 
         Experimental features already exist at Rancher v2.5.x systems, so they can just be updated:
         * On create, provider will read Feature from Rancher and update its value. It will return an error if feature doesn't exist
         * On destroy, provider will not delete feature from Rancher, just from tfstate
 
-        **Note** Some Rancher features as `fleet`, may force a Rancher reboot once updated. The provider will wait until Rancher is rebooted. If you are modifying more than one feature in a row, and any of them requires a Rancher reboot, `pulumi up` may fail on first run. Run `pulumi up` again should work fine.
+        **Note:** Some Rancher features as `fleet`, may force a Rancher reboot once updated. The provider will wait until Rancher is rebooted. If you are modifying more than one feature in a row, and any of them requires a Rancher reboot, `pulumi up` may fail on first run. Run `pulumi up` again should work fine.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
@@ -200,15 +200,15 @@
         """
         Provides a Rancher v2 Feature resource. This can be used to enable/disable [experimental features](https://rancher.com/docs/rancher/v2.x/en/installation/resources/feature-flags/) for Rancher v2 environments.
 
         Experimental features already exist at Rancher v2.5.x systems, so they can just be updated:
         * On create, provider will read Feature from Rancher and update its value. It will return an error if feature doesn't exist
         * On destroy, provider will not delete feature from Rancher, just from tfstate
 
-        **Note** Some Rancher features as `fleet`, may force a Rancher reboot once updated. The provider will wait until Rancher is rebooted. If you are modifying more than one feature in a row, and any of them requires a Rancher reboot, `pulumi up` may fail on first run. Run `pulumi up` again should work fine.
+        **Note:** Some Rancher features as `fleet`, may force a Rancher reboot once updated. The provider will wait until Rancher is rebooted. If you are modifying more than one feature in a row, and any of them requires a Rancher reboot, `pulumi up` may fail on first run. Run `pulumi up` again should work fine.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_app.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -221,28 +221,28 @@
     __args__['name'] = name
     __args__['projectId'] = project_id
     __args__['targetNamespace'] = target_namespace
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getApp:getApp', __args__, opts=opts, typ=GetAppResult).value
 
     return AwaitableGetAppResult(
-        annotations=__ret__.annotations,
-        answers=__ret__.answers,
-        catalog_name=__ret__.catalog_name,
-        description=__ret__.description,
-        external_id=__ret__.external_id,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        project_id=__ret__.project_id,
-        revision_id=__ret__.revision_id,
-        target_namespace=__ret__.target_namespace,
-        template_name=__ret__.template_name,
-        template_version=__ret__.template_version,
-        values_yaml=__ret__.values_yaml)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        answers=pulumi.get(__ret__, 'answers'),
+        catalog_name=pulumi.get(__ret__, 'catalog_name'),
+        description=pulumi.get(__ret__, 'description'),
+        external_id=pulumi.get(__ret__, 'external_id'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        revision_id=pulumi.get(__ret__, 'revision_id'),
+        target_namespace=pulumi.get(__ret__, 'target_namespace'),
+        template_name=pulumi.get(__ret__, 'template_name'),
+        template_version=pulumi.get(__ret__, 'template_version'),
+        values_yaml=pulumi.get(__ret__, 'values_yaml'))
 
 
 @_utilities.lift_output_func(get_app)
 def get_app_output(annotations: Optional[pulumi.Input[Optional[Mapping[str, Any]]]] = None,
                    name: Optional[pulumi.Input[str]] = None,
                    project_id: Optional[pulumi.Input[str]] = None,
                    target_namespace: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_catalog.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_catalog.py`

 * *Files 15% similar despite different names*

```diff
@@ -216,28 +216,28 @@
     __args__ = dict()
     __args__['name'] = name
     __args__['scope'] = scope
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getCatalog:getCatalog', __args__, opts=opts, typ=GetCatalogResult).value
 
     return AwaitableGetCatalogResult(
-        annotations=__ret__.annotations,
-        branch=__ret__.branch,
-        cluster_id=__ret__.cluster_id,
-        description=__ret__.description,
-        id=__ret__.id,
-        kind=__ret__.kind,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        password=__ret__.password,
-        project_id=__ret__.project_id,
-        scope=__ret__.scope,
-        url=__ret__.url,
-        username=__ret__.username,
-        version=__ret__.version)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        branch=pulumi.get(__ret__, 'branch'),
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        kind=pulumi.get(__ret__, 'kind'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        password=pulumi.get(__ret__, 'password'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        scope=pulumi.get(__ret__, 'scope'),
+        url=pulumi.get(__ret__, 'url'),
+        username=pulumi.get(__ret__, 'username'),
+        version=pulumi.get(__ret__, 'version'))
 
 
 @_utilities.lift_output_func(get_catalog)
 def get_catalog_output(name: Optional[pulumi.Input[str]] = None,
                        scope: Optional[pulumi.Input[Optional[str]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCatalogResult]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_catalog_v2.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_catalog_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,30 +231,30 @@
     __args__ = dict()
     __args__['clusterId'] = cluster_id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getCatalogV2:getCatalogV2', __args__, opts=opts, typ=GetCatalogV2Result).value
 
     return AwaitableGetCatalogV2Result(
-        annotations=__ret__.annotations,
-        ca_bundle=__ret__.ca_bundle,
-        cluster_id=__ret__.cluster_id,
-        enabled=__ret__.enabled,
-        git_branch=__ret__.git_branch,
-        git_repo=__ret__.git_repo,
-        id=__ret__.id,
-        insecure=__ret__.insecure,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        resource_version=__ret__.resource_version,
-        secret_name=__ret__.secret_name,
-        secret_namespace=__ret__.secret_namespace,
-        service_account=__ret__.service_account,
-        service_account_namespace=__ret__.service_account_namespace,
-        url=__ret__.url)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        ca_bundle=pulumi.get(__ret__, 'ca_bundle'),
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        enabled=pulumi.get(__ret__, 'enabled'),
+        git_branch=pulumi.get(__ret__, 'git_branch'),
+        git_repo=pulumi.get(__ret__, 'git_repo'),
+        id=pulumi.get(__ret__, 'id'),
+        insecure=pulumi.get(__ret__, 'insecure'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        resource_version=pulumi.get(__ret__, 'resource_version'),
+        secret_name=pulumi.get(__ret__, 'secret_name'),
+        secret_namespace=pulumi.get(__ret__, 'secret_namespace'),
+        service_account=pulumi.get(__ret__, 'service_account'),
+        service_account_namespace=pulumi.get(__ret__, 'service_account_namespace'),
+        url=pulumi.get(__ret__, 'url'))
 
 
 @_utilities.lift_output_func(get_catalog_v2)
 def get_catalog_v2_output(cluster_id: Optional[pulumi.Input[str]] = None,
                           name: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCatalogV2Result]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_certificate.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_certificate.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,22 +158,22 @@
     __args__['name'] = name
     __args__['namespaceId'] = namespace_id
     __args__['projectId'] = project_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getCertificate:getCertificate', __args__, opts=opts, typ=GetCertificateResult).value
 
     return AwaitableGetCertificateResult(
-        annotations=__ret__.annotations,
-        certs=__ret__.certs,
-        description=__ret__.description,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        namespace_id=__ret__.namespace_id,
-        project_id=__ret__.project_id)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        certs=pulumi.get(__ret__, 'certs'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        namespace_id=pulumi.get(__ret__, 'namespace_id'),
+        project_id=pulumi.get(__ret__, 'project_id'))
 
 
 @_utilities.lift_output_func(get_certificate)
 def get_certificate_output(name: Optional[pulumi.Input[str]] = None,
                            namespace_id: Optional[pulumi.Input[Optional[str]]] = None,
                            project_id: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCertificateResult]:
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cloud_credential.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cloud_credential.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,18 +96,18 @@
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getCloudCredential:getCloudCredential', __args__, opts=opts, typ=GetCloudCredentialResult).value
 
     return AwaitableGetCloudCredentialResult(
-        annotations=__ret__.annotations,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'))
 
 
 @_utilities.lift_output_func(get_cloud_credential)
 def get_cloud_credential_output(name: Optional[pulumi.Input[str]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCloudCredentialResult]:
     """
     Use this data source to retrieve information about a Rancher v2 Cloud Credential.
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cluster.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             raise TypeError("Expected argument 'system_project_id' to be a str")
         pulumi.set(__self__, "system_project_id", system_project_id)
 
     @property
     @pulumi.getter(name="agentEnvVars")
     def agent_env_vars(self) -> Sequence[str]:
         """
-        (Computed) Optional Agent Env Vars for Rancher agent. Just for Rancher v2.5.6 and above (list)
+        (Computed) Optional Agent Env Vars for Rancher agent. For Rancher v2.5.6 and above (list)
         """
         return pulumi.get(self, "agent_env_vars")
 
     @property
     @pulumi.getter(name="aksConfig")
     def aks_config(self) -> 'outputs.GetClusterAksConfigResult':
         """
@@ -267,15 +267,15 @@
         """
         return pulumi.get(self, "eks_config")
 
     @property
     @pulumi.getter(name="eksConfigV2")
     def eks_config_v2(self) -> 'outputs.GetClusterEksConfigV2Result':
         """
-        (Computed) The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.x or above (list maxitems:1)
+        (Computed) The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.x and above (list maxitems:1)
         """
         return pulumi.get(self, "eks_config_v2")
 
     @property
     @pulumi.getter(name="enableClusterAlerting")
     def enable_cluster_alerting(self) -> bool:
         return pulumi.get(self, "enable_cluster_alerting")
@@ -312,15 +312,15 @@
         """
         return pulumi.get(self, "gke_config")
 
     @property
     @pulumi.getter(name="gkeConfigV2")
     def gke_config_v2(self) -> 'outputs.GetClusterGkeConfigV2Result':
         """
-        (Computed) The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 or above (list maxitems:1)
+        (Computed) The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 and above (list maxitems:1)
         """
         return pulumi.get(self, "gke_config_v2")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
@@ -453,48 +453,48 @@
     __args__ = dict()
     __args__['defaultPodSecurityAdmissionConfigurationTemplateName'] = default_pod_security_admission_configuration_template_name
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getCluster:getCluster', __args__, opts=opts, typ=GetClusterResult).value
 
     return AwaitableGetClusterResult(
-        agent_env_vars=__ret__.agent_env_vars,
-        aks_config=__ret__.aks_config,
-        aks_config_v2=__ret__.aks_config_v2,
-        annotations=__ret__.annotations,
-        ca_cert=__ret__.ca_cert,
-        cluster_auth_endpoint=__ret__.cluster_auth_endpoint,
-        cluster_monitoring_input=__ret__.cluster_monitoring_input,
-        cluster_registration_token=__ret__.cluster_registration_token,
-        cluster_template_answers=__ret__.cluster_template_answers,
-        cluster_template_id=__ret__.cluster_template_id,
-        cluster_template_questions=__ret__.cluster_template_questions,
-        cluster_template_revision_id=__ret__.cluster_template_revision_id,
-        default_pod_security_admission_configuration_template_name=__ret__.default_pod_security_admission_configuration_template_name,
-        default_pod_security_policy_template_id=__ret__.default_pod_security_policy_template_id,
-        default_project_id=__ret__.default_project_id,
-        description=__ret__.description,
-        driver=__ret__.driver,
-        eks_config=__ret__.eks_config,
-        eks_config_v2=__ret__.eks_config_v2,
-        enable_cluster_alerting=__ret__.enable_cluster_alerting,
-        enable_cluster_monitoring=__ret__.enable_cluster_monitoring,
-        enable_network_policy=__ret__.enable_network_policy,
-        fleet_workspace_name=__ret__.fleet_workspace_name,
-        gke_config=__ret__.gke_config,
-        gke_config_v2=__ret__.gke_config_v2,
-        id=__ret__.id,
-        k3s_config=__ret__.k3s_config,
-        kube_config=__ret__.kube_config,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        oke_config=__ret__.oke_config,
-        rke2_config=__ret__.rke2_config,
-        rke_config=__ret__.rke_config,
-        system_project_id=__ret__.system_project_id)
+        agent_env_vars=pulumi.get(__ret__, 'agent_env_vars'),
+        aks_config=pulumi.get(__ret__, 'aks_config'),
+        aks_config_v2=pulumi.get(__ret__, 'aks_config_v2'),
+        annotations=pulumi.get(__ret__, 'annotations'),
+        ca_cert=pulumi.get(__ret__, 'ca_cert'),
+        cluster_auth_endpoint=pulumi.get(__ret__, 'cluster_auth_endpoint'),
+        cluster_monitoring_input=pulumi.get(__ret__, 'cluster_monitoring_input'),
+        cluster_registration_token=pulumi.get(__ret__, 'cluster_registration_token'),
+        cluster_template_answers=pulumi.get(__ret__, 'cluster_template_answers'),
+        cluster_template_id=pulumi.get(__ret__, 'cluster_template_id'),
+        cluster_template_questions=pulumi.get(__ret__, 'cluster_template_questions'),
+        cluster_template_revision_id=pulumi.get(__ret__, 'cluster_template_revision_id'),
+        default_pod_security_admission_configuration_template_name=pulumi.get(__ret__, 'default_pod_security_admission_configuration_template_name'),
+        default_pod_security_policy_template_id=pulumi.get(__ret__, 'default_pod_security_policy_template_id'),
+        default_project_id=pulumi.get(__ret__, 'default_project_id'),
+        description=pulumi.get(__ret__, 'description'),
+        driver=pulumi.get(__ret__, 'driver'),
+        eks_config=pulumi.get(__ret__, 'eks_config'),
+        eks_config_v2=pulumi.get(__ret__, 'eks_config_v2'),
+        enable_cluster_alerting=pulumi.get(__ret__, 'enable_cluster_alerting'),
+        enable_cluster_monitoring=pulumi.get(__ret__, 'enable_cluster_monitoring'),
+        enable_network_policy=pulumi.get(__ret__, 'enable_network_policy'),
+        fleet_workspace_name=pulumi.get(__ret__, 'fleet_workspace_name'),
+        gke_config=pulumi.get(__ret__, 'gke_config'),
+        gke_config_v2=pulumi.get(__ret__, 'gke_config_v2'),
+        id=pulumi.get(__ret__, 'id'),
+        k3s_config=pulumi.get(__ret__, 'k3s_config'),
+        kube_config=pulumi.get(__ret__, 'kube_config'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        oke_config=pulumi.get(__ret__, 'oke_config'),
+        rke2_config=pulumi.get(__ret__, 'rke2_config'),
+        rke_config=pulumi.get(__ret__, 'rke_config'),
+        system_project_id=pulumi.get(__ret__, 'system_project_id'))
 
 
 @_utilities.lift_output_func(get_cluster)
 def get_cluster_output(default_pod_security_admission_configuration_template_name: Optional[pulumi.Input[Optional[str]]] = None,
                        name: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClusterResult]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cluster_alert_group.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cluster_alert_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -170,24 +170,24 @@
     __args__ = dict()
     __args__['clusterId'] = cluster_id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getClusterAlertGroup:getClusterAlertGroup', __args__, opts=opts, typ=GetClusterAlertGroupResult).value
 
     return AwaitableGetClusterAlertGroupResult(
-        annotations=__ret__.annotations,
-        cluster_id=__ret__.cluster_id,
-        description=__ret__.description,
-        group_interval_seconds=__ret__.group_interval_seconds,
-        group_wait_seconds=__ret__.group_wait_seconds,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        recipients=__ret__.recipients,
-        repeat_interval_seconds=__ret__.repeat_interval_seconds)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        description=pulumi.get(__ret__, 'description'),
+        group_interval_seconds=pulumi.get(__ret__, 'group_interval_seconds'),
+        group_wait_seconds=pulumi.get(__ret__, 'group_wait_seconds'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        recipients=pulumi.get(__ret__, 'recipients'),
+        repeat_interval_seconds=pulumi.get(__ret__, 'repeat_interval_seconds'))
 
 
 @_utilities.lift_output_func(get_cluster_alert_group)
 def get_cluster_alert_group_output(cluster_id: Optional[pulumi.Input[str]] = None,
                                    name: Optional[pulumi.Input[str]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClusterAlertGroupResult]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cluster_alter_rule.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cluster_alter_rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -233,29 +233,29 @@
     __args__['clusterId'] = cluster_id
     __args__['labels'] = labels
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getClusterAlterRule:getClusterAlterRule', __args__, opts=opts, typ=GetClusterAlterRuleResult).value
 
     return AwaitableGetClusterAlterRuleResult(
-        annotations=__ret__.annotations,
-        cluster_id=__ret__.cluster_id,
-        event_rule=__ret__.event_rule,
-        group_id=__ret__.group_id,
-        group_interval_seconds=__ret__.group_interval_seconds,
-        group_wait_seconds=__ret__.group_wait_seconds,
-        id=__ret__.id,
-        inherited=__ret__.inherited,
-        labels=__ret__.labels,
-        metric_rule=__ret__.metric_rule,
-        name=__ret__.name,
-        node_rule=__ret__.node_rule,
-        repeat_interval_seconds=__ret__.repeat_interval_seconds,
-        severity=__ret__.severity,
-        system_service_rule=__ret__.system_service_rule)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        event_rule=pulumi.get(__ret__, 'event_rule'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        group_interval_seconds=pulumi.get(__ret__, 'group_interval_seconds'),
+        group_wait_seconds=pulumi.get(__ret__, 'group_wait_seconds'),
+        id=pulumi.get(__ret__, 'id'),
+        inherited=pulumi.get(__ret__, 'inherited'),
+        labels=pulumi.get(__ret__, 'labels'),
+        metric_rule=pulumi.get(__ret__, 'metric_rule'),
+        name=pulumi.get(__ret__, 'name'),
+        node_rule=pulumi.get(__ret__, 'node_rule'),
+        repeat_interval_seconds=pulumi.get(__ret__, 'repeat_interval_seconds'),
+        severity=pulumi.get(__ret__, 'severity'),
+        system_service_rule=pulumi.get(__ret__, 'system_service_rule'))
 
 
 @_utilities.lift_output_func(get_cluster_alter_rule)
 def get_cluster_alter_rule_output(cluster_id: Optional[pulumi.Input[str]] = None,
                                   labels: Optional[pulumi.Input[Optional[Mapping[str, Any]]]] = None,
                                   name: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClusterAlterRuleResult]:
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cluster_driver.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cluster_driver.py`

 * *Files 11% similar despite different names*

```diff
@@ -180,25 +180,25 @@
     __args__ = dict()
     __args__['name'] = name
     __args__['url'] = url
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getClusterDriver:getClusterDriver', __args__, opts=opts, typ=GetClusterDriverResult).value
 
     return AwaitableGetClusterDriverResult(
-        active=__ret__.active,
-        actual_url=__ret__.actual_url,
-        annotations=__ret__.annotations,
-        builtin=__ret__.builtin,
-        checksum=__ret__.checksum,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        ui_url=__ret__.ui_url,
-        url=__ret__.url,
-        whitelist_domains=__ret__.whitelist_domains)
+        active=pulumi.get(__ret__, 'active'),
+        actual_url=pulumi.get(__ret__, 'actual_url'),
+        annotations=pulumi.get(__ret__, 'annotations'),
+        builtin=pulumi.get(__ret__, 'builtin'),
+        checksum=pulumi.get(__ret__, 'checksum'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        ui_url=pulumi.get(__ret__, 'ui_url'),
+        url=pulumi.get(__ret__, 'url'),
+        whitelist_domains=pulumi.get(__ret__, 'whitelist_domains'))
 
 
 @_utilities.lift_output_func(get_cluster_driver)
 def get_cluster_driver_output(name: Optional[pulumi.Input[str]] = None,
                               url: Optional[pulumi.Input[Optional[str]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClusterDriverResult]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cluster_role_template_binding.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cluster_role_template_binding.py`

 * *Files 8% similar despite different names*

```diff
@@ -169,24 +169,24 @@
     __args__['clusterId'] = cluster_id
     __args__['name'] = name
     __args__['roleTemplateId'] = role_template_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getClusterRoleTemplateBinding:getClusterRoleTemplateBinding', __args__, opts=opts, typ=GetClusterRoleTemplateBindingResult).value
 
     return AwaitableGetClusterRoleTemplateBindingResult(
-        annotations=__ret__.annotations,
-        cluster_id=__ret__.cluster_id,
-        group_id=__ret__.group_id,
-        group_principal_id=__ret__.group_principal_id,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        role_template_id=__ret__.role_template_id,
-        user_id=__ret__.user_id,
-        user_principal_id=__ret__.user_principal_id)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        group_principal_id=pulumi.get(__ret__, 'group_principal_id'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        role_template_id=pulumi.get(__ret__, 'role_template_id'),
+        user_id=pulumi.get(__ret__, 'user_id'),
+        user_principal_id=pulumi.get(__ret__, 'user_principal_id'))
 
 
 @_utilities.lift_output_func(get_cluster_role_template_binding)
 def get_cluster_role_template_binding_output(cluster_id: Optional[pulumi.Input[str]] = None,
                                              name: Optional[pulumi.Input[str]] = None,
                                              role_template_id: Optional[pulumi.Input[Optional[str]]] = None,
                                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClusterRoleTemplateBindingResult]:
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cluster_template.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cluster_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -152,22 +152,22 @@
     __args__['description'] = description
     __args__['labels'] = labels
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getClusterTemplate:getClusterTemplate', __args__, opts=opts, typ=GetClusterTemplateResult).value
 
     return AwaitableGetClusterTemplateResult(
-        annotations=__ret__.annotations,
-        default_revision_id=__ret__.default_revision_id,
-        description=__ret__.description,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        members=__ret__.members,
-        name=__ret__.name,
-        template_revisions=__ret__.template_revisions)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        default_revision_id=pulumi.get(__ret__, 'default_revision_id'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        members=pulumi.get(__ret__, 'members'),
+        name=pulumi.get(__ret__, 'name'),
+        template_revisions=pulumi.get(__ret__, 'template_revisions'))
 
 
 @_utilities.lift_output_func(get_cluster_template)
 def get_cluster_template_output(annotations: Optional[pulumi.Input[Optional[Mapping[str, Any]]]] = None,
                                 description: Optional[pulumi.Input[Optional[str]]] = None,
                                 labels: Optional[pulumi.Input[Optional[Mapping[str, Any]]]] = None,
                                 name: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_cluster_v2.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_cluster_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -248,31 +248,31 @@
     __args__ = dict()
     __args__['fleetNamespace'] = fleet_namespace
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getClusterV2:getClusterV2', __args__, opts=opts, typ=GetClusterV2Result).value
 
     return AwaitableGetClusterV2Result(
-        agent_env_vars=__ret__.agent_env_vars,
-        annotations=__ret__.annotations,
-        cloud_credential_secret_name=__ret__.cloud_credential_secret_name,
-        cluster_registration_token=__ret__.cluster_registration_token,
-        cluster_v1_id=__ret__.cluster_v1_id,
-        default_cluster_role_for_project_members=__ret__.default_cluster_role_for_project_members,
-        default_pod_security_admission_configuration_template_name=__ret__.default_pod_security_admission_configuration_template_name,
-        default_pod_security_policy_template_name=__ret__.default_pod_security_policy_template_name,
-        enable_network_policy=__ret__.enable_network_policy,
-        fleet_namespace=__ret__.fleet_namespace,
-        id=__ret__.id,
-        kube_config=__ret__.kube_config,
-        kubernetes_version=__ret__.kubernetes_version,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        resource_version=__ret__.resource_version,
-        rke_config=__ret__.rke_config)
+        agent_env_vars=pulumi.get(__ret__, 'agent_env_vars'),
+        annotations=pulumi.get(__ret__, 'annotations'),
+        cloud_credential_secret_name=pulumi.get(__ret__, 'cloud_credential_secret_name'),
+        cluster_registration_token=pulumi.get(__ret__, 'cluster_registration_token'),
+        cluster_v1_id=pulumi.get(__ret__, 'cluster_v1_id'),
+        default_cluster_role_for_project_members=pulumi.get(__ret__, 'default_cluster_role_for_project_members'),
+        default_pod_security_admission_configuration_template_name=pulumi.get(__ret__, 'default_pod_security_admission_configuration_template_name'),
+        default_pod_security_policy_template_name=pulumi.get(__ret__, 'default_pod_security_policy_template_name'),
+        enable_network_policy=pulumi.get(__ret__, 'enable_network_policy'),
+        fleet_namespace=pulumi.get(__ret__, 'fleet_namespace'),
+        id=pulumi.get(__ret__, 'id'),
+        kube_config=pulumi.get(__ret__, 'kube_config'),
+        kubernetes_version=pulumi.get(__ret__, 'kubernetes_version'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        resource_version=pulumi.get(__ret__, 'resource_version'),
+        rke_config=pulumi.get(__ret__, 'rke_config'))
 
 
 @_utilities.lift_output_func(get_cluster_v2)
 def get_cluster_v2_output(fleet_namespace: Optional[pulumi.Input[Optional[str]]] = None,
                           name: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClusterV2Result]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_config_map_v2.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_config_map_v2.py`

 * *Files 7% similar despite different names*

```diff
@@ -147,23 +147,23 @@
     __args__['clusterId'] = cluster_id
     __args__['name'] = name
     __args__['namespace'] = namespace
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getConfigMapV2:getConfigMapV2', __args__, opts=opts, typ=GetConfigMapV2Result).value
 
     return AwaitableGetConfigMapV2Result(
-        annotations=__ret__.annotations,
-        cluster_id=__ret__.cluster_id,
-        data=__ret__.data,
-        id=__ret__.id,
-        immutable=__ret__.immutable,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        namespace=__ret__.namespace,
-        resource_version=__ret__.resource_version)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        data=pulumi.get(__ret__, 'data'),
+        id=pulumi.get(__ret__, 'id'),
+        immutable=pulumi.get(__ret__, 'immutable'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        namespace=pulumi.get(__ret__, 'namespace'),
+        resource_version=pulumi.get(__ret__, 'resource_version'))
 
 
 @_utilities.lift_output_func(get_config_map_v2)
 def get_config_map_v2_output(cluster_id: Optional[pulumi.Input[str]] = None,
                              name: Optional[pulumi.Input[str]] = None,
                              namespace: Optional[pulumi.Input[Optional[str]]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetConfigMapV2Result]:
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_etcd_backup.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_etcd_backup.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,23 +158,23 @@
     __args__ = dict()
     __args__['clusterId'] = cluster_id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getEtcdBackup:getEtcdBackup', __args__, opts=opts, typ=GetEtcdBackupResult).value
 
     return AwaitableGetEtcdBackupResult(
-        annotations=__ret__.annotations,
-        backup_config=__ret__.backup_config,
-        cluster_id=__ret__.cluster_id,
-        filename=__ret__.filename,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        manual=__ret__.manual,
-        name=__ret__.name,
-        namespace_id=__ret__.namespace_id)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        backup_config=pulumi.get(__ret__, 'backup_config'),
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        filename=pulumi.get(__ret__, 'filename'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        manual=pulumi.get(__ret__, 'manual'),
+        name=pulumi.get(__ret__, 'name'),
+        namespace_id=pulumi.get(__ret__, 'namespace_id'))
 
 
 @_utilities.lift_output_func(get_etcd_backup)
 def get_etcd_backup_output(cluster_id: Optional[pulumi.Input[str]] = None,
                            name: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEtcdBackupResult]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_global_dns_provider.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_global_dns_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -145,23 +145,23 @@
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getGlobalDnsProvider:getGlobalDnsProvider', __args__, opts=opts, typ=GetGlobalDnsProviderResult).value
 
     return AwaitableGetGlobalDnsProviderResult(
-        alidns_config=__ret__.alidns_config,
-        annotations=__ret__.annotations,
-        cloudflare_config=__ret__.cloudflare_config,
-        dns_provider=__ret__.dns_provider,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        root_domain=__ret__.root_domain,
-        route53_config=__ret__.route53_config)
+        alidns_config=pulumi.get(__ret__, 'alidns_config'),
+        annotations=pulumi.get(__ret__, 'annotations'),
+        cloudflare_config=pulumi.get(__ret__, 'cloudflare_config'),
+        dns_provider=pulumi.get(__ret__, 'dns_provider'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        root_domain=pulumi.get(__ret__, 'root_domain'),
+        route53_config=pulumi.get(__ret__, 'route53_config'))
 
 
 @_utilities.lift_output_func(get_global_dns_provider)
 def get_global_dns_provider_output(name: Optional[pulumi.Input[str]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGlobalDnsProviderResult]:
     """
     Provides a Rancher V2 Global DNS Provider data source. Use this data source to retrieve information about a Rancher v2 global DNS provider
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_global_role.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_global_role.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,22 +145,22 @@
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getGlobalRole:getGlobalRole', __args__, opts=opts, typ=GetGlobalRoleResult).value
 
     return AwaitableGetGlobalRoleResult(
-        annotations=__ret__.annotations,
-        builtin=__ret__.builtin,
-        description=__ret__.description,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        new_user_default=__ret__.new_user_default,
-        rules=__ret__.rules)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        builtin=pulumi.get(__ret__, 'builtin'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        new_user_default=pulumi.get(__ret__, 'new_user_default'),
+        rules=pulumi.get(__ret__, 'rules'))
 
 
 @_utilities.lift_output_func(get_global_role)
 def get_global_role_output(name: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGlobalRoleResult]:
     """
     Use this data source to retrieve information about a Rancher v2 global role resource.
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_global_role_binding.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_global_role_binding.py`

 * *Files 7% similar despite different names*

```diff
@@ -133,21 +133,21 @@
     __args__ = dict()
     __args__['globalRoleId'] = global_role_id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getGlobalRoleBinding:getGlobalRoleBinding', __args__, opts=opts, typ=GetGlobalRoleBindingResult).value
 
     return AwaitableGetGlobalRoleBindingResult(
-        annotations=__ret__.annotations,
-        global_role_id=__ret__.global_role_id,
-        group_principal_id=__ret__.group_principal_id,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        user_id=__ret__.user_id)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        global_role_id=pulumi.get(__ret__, 'global_role_id'),
+        group_principal_id=pulumi.get(__ret__, 'group_principal_id'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        user_id=pulumi.get(__ret__, 'user_id'))
 
 
 @_utilities.lift_output_func(get_global_role_binding)
 def get_global_role_binding_output(global_role_id: Optional[pulumi.Input[Optional[str]]] = None,
                                    name: Optional[pulumi.Input[str]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGlobalRoleBindingResult]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_multi_cluster_app.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_multi_cluster_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -229,29 +229,29 @@
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getMultiClusterApp:getMultiClusterApp', __args__, opts=opts, typ=GetMultiClusterAppResult).value
 
     return AwaitableGetMultiClusterAppResult(
-        annotations=__ret__.annotations,
-        answers=__ret__.answers,
-        catalog_name=__ret__.catalog_name,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        members=__ret__.members,
-        name=__ret__.name,
-        revision_history_limit=__ret__.revision_history_limit,
-        revision_id=__ret__.revision_id,
-        roles=__ret__.roles,
-        targets=__ret__.targets,
-        template_name=__ret__.template_name,
-        template_version=__ret__.template_version,
-        template_version_id=__ret__.template_version_id,
-        upgrade_strategies=__ret__.upgrade_strategies)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        answers=pulumi.get(__ret__, 'answers'),
+        catalog_name=pulumi.get(__ret__, 'catalog_name'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        members=pulumi.get(__ret__, 'members'),
+        name=pulumi.get(__ret__, 'name'),
+        revision_history_limit=pulumi.get(__ret__, 'revision_history_limit'),
+        revision_id=pulumi.get(__ret__, 'revision_id'),
+        roles=pulumi.get(__ret__, 'roles'),
+        targets=pulumi.get(__ret__, 'targets'),
+        template_name=pulumi.get(__ret__, 'template_name'),
+        template_version=pulumi.get(__ret__, 'template_version'),
+        template_version_id=pulumi.get(__ret__, 'template_version_id'),
+        upgrade_strategies=pulumi.get(__ret__, 'upgrade_strategies'))
 
 
 @_utilities.lift_output_func(get_multi_cluster_app)
 def get_multi_cluster_app_output(name: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMultiClusterAppResult]:
     """
     Use this data source to retrieve information about a Rancher v2 multi cluster app.
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_namespace.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_namespace.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,22 +146,22 @@
     __args__ = dict()
     __args__['name'] = name
     __args__['projectId'] = project_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getNamespace:getNamespace', __args__, opts=opts, typ=GetNamespaceResult).value
 
     return AwaitableGetNamespaceResult(
-        annotations=__ret__.annotations,
-        container_resource_limit=__ret__.container_resource_limit,
-        description=__ret__.description,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        project_id=__ret__.project_id,
-        resource_quota=__ret__.resource_quota)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        container_resource_limit=pulumi.get(__ret__, 'container_resource_limit'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        resource_quota=pulumi.get(__ret__, 'resource_quota'))
 
 
 @_utilities.lift_output_func(get_namespace)
 def get_namespace_output(name: Optional[pulumi.Input[str]] = None,
                          project_id: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNamespaceResult]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_node_driver.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_node_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -192,26 +192,26 @@
     __args__ = dict()
     __args__['name'] = name
     __args__['url'] = url
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getNodeDriver:getNodeDriver', __args__, opts=opts, typ=GetNodeDriverResult).value
 
     return AwaitableGetNodeDriverResult(
-        active=__ret__.active,
-        annotations=__ret__.annotations,
-        builtin=__ret__.builtin,
-        checksum=__ret__.checksum,
-        description=__ret__.description,
-        external_id=__ret__.external_id,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        ui_url=__ret__.ui_url,
-        url=__ret__.url,
-        whitelist_domains=__ret__.whitelist_domains)
+        active=pulumi.get(__ret__, 'active'),
+        annotations=pulumi.get(__ret__, 'annotations'),
+        builtin=pulumi.get(__ret__, 'builtin'),
+        checksum=pulumi.get(__ret__, 'checksum'),
+        description=pulumi.get(__ret__, 'description'),
+        external_id=pulumi.get(__ret__, 'external_id'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        ui_url=pulumi.get(__ret__, 'ui_url'),
+        url=pulumi.get(__ret__, 'url'),
+        whitelist_domains=pulumi.get(__ret__, 'whitelist_domains'))
 
 
 @_utilities.lift_output_func(get_node_driver)
 def get_node_driver_output(name: Optional[pulumi.Input[str]] = None,
                            url: Optional[pulumi.Input[Optional[str]]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNodeDriverResult]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_node_pool.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_node_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -206,27 +206,27 @@
     __args__['clusterId'] = cluster_id
     __args__['name'] = name
     __args__['nodeTemplateId'] = node_template_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getNodePool:getNodePool', __args__, opts=opts, typ=GetNodePoolResult).value
 
     return AwaitableGetNodePoolResult(
-        annotations=__ret__.annotations,
-        cluster_id=__ret__.cluster_id,
-        control_plane=__ret__.control_plane,
-        delete_not_ready_after_secs=__ret__.delete_not_ready_after_secs,
-        etcd=__ret__.etcd,
-        hostname_prefix=__ret__.hostname_prefix,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        node_taints=__ret__.node_taints,
-        node_template_id=__ret__.node_template_id,
-        quantity=__ret__.quantity,
-        worker=__ret__.worker)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        control_plane=pulumi.get(__ret__, 'control_plane'),
+        delete_not_ready_after_secs=pulumi.get(__ret__, 'delete_not_ready_after_secs'),
+        etcd=pulumi.get(__ret__, 'etcd'),
+        hostname_prefix=pulumi.get(__ret__, 'hostname_prefix'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        node_taints=pulumi.get(__ret__, 'node_taints'),
+        node_template_id=pulumi.get(__ret__, 'node_template_id'),
+        quantity=pulumi.get(__ret__, 'quantity'),
+        worker=pulumi.get(__ret__, 'worker'))
 
 
 @_utilities.lift_output_func(get_node_pool)
 def get_node_pool_output(cluster_id: Optional[pulumi.Input[str]] = None,
                          name: Optional[pulumi.Input[str]] = None,
                          node_template_id: Optional[pulumi.Input[Optional[str]]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNodePoolResult]:
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_node_template.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_node_template.py`

 * *Files 17% similar despite different names*

```diff
@@ -244,30 +244,30 @@
     __args__ = dict()
     __args__['name'] = name
     __args__['useInternalIpAddress'] = use_internal_ip_address
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getNodeTemplate:getNodeTemplate', __args__, opts=opts, typ=GetNodeTemplateResult).value
 
     return AwaitableGetNodeTemplateResult(
-        annotations=__ret__.annotations,
-        cloud_credential_id=__ret__.cloud_credential_id,
-        description=__ret__.description,
-        driver=__ret__.driver,
-        engine_env=__ret__.engine_env,
-        engine_insecure_registries=__ret__.engine_insecure_registries,
-        engine_install_url=__ret__.engine_install_url,
-        engine_label=__ret__.engine_label,
-        engine_opt=__ret__.engine_opt,
-        engine_registry_mirrors=__ret__.engine_registry_mirrors,
-        engine_storage_driver=__ret__.engine_storage_driver,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        node_taints=__ret__.node_taints,
-        use_internal_ip_address=__ret__.use_internal_ip_address)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        cloud_credential_id=pulumi.get(__ret__, 'cloud_credential_id'),
+        description=pulumi.get(__ret__, 'description'),
+        driver=pulumi.get(__ret__, 'driver'),
+        engine_env=pulumi.get(__ret__, 'engine_env'),
+        engine_insecure_registries=pulumi.get(__ret__, 'engine_insecure_registries'),
+        engine_install_url=pulumi.get(__ret__, 'engine_install_url'),
+        engine_label=pulumi.get(__ret__, 'engine_label'),
+        engine_opt=pulumi.get(__ret__, 'engine_opt'),
+        engine_registry_mirrors=pulumi.get(__ret__, 'engine_registry_mirrors'),
+        engine_storage_driver=pulumi.get(__ret__, 'engine_storage_driver'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        node_taints=pulumi.get(__ret__, 'node_taints'),
+        use_internal_ip_address=pulumi.get(__ret__, 'use_internal_ip_address'))
 
 
 @_utilities.lift_output_func(get_node_template)
 def get_node_template_output(name: Optional[pulumi.Input[str]] = None,
                              use_internal_ip_address: Optional[pulumi.Input[Optional[bool]]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNodeTemplateResult]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_notifier.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -213,27 +213,27 @@
     __args__['dingtalkConfig'] = dingtalk_config
     __args__['msteamsConfig'] = msteams_config
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getNotifier:getNotifier', __args__, opts=opts, typ=GetNotifierResult).value
 
     return AwaitableGetNotifierResult(
-        annotations=__ret__.annotations,
-        cluster_id=__ret__.cluster_id,
-        description=__ret__.description,
-        dingtalk_config=__ret__.dingtalk_config,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        msteams_config=__ret__.msteams_config,
-        name=__ret__.name,
-        pagerduty_config=__ret__.pagerduty_config,
-        slack_config=__ret__.slack_config,
-        smtp_config=__ret__.smtp_config,
-        webhook_config=__ret__.webhook_config,
-        wechat_config=__ret__.wechat_config)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        description=pulumi.get(__ret__, 'description'),
+        dingtalk_config=pulumi.get(__ret__, 'dingtalk_config'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        msteams_config=pulumi.get(__ret__, 'msteams_config'),
+        name=pulumi.get(__ret__, 'name'),
+        pagerduty_config=pulumi.get(__ret__, 'pagerduty_config'),
+        slack_config=pulumi.get(__ret__, 'slack_config'),
+        smtp_config=pulumi.get(__ret__, 'smtp_config'),
+        webhook_config=pulumi.get(__ret__, 'webhook_config'),
+        wechat_config=pulumi.get(__ret__, 'wechat_config'))
 
 
 @_utilities.lift_output_func(get_notifier)
 def get_notifier_output(cluster_id: Optional[pulumi.Input[str]] = None,
                         dingtalk_config: Optional[pulumi.Input[Optional[pulumi.InputType['GetNotifierDingtalkConfigArgs']]]] = None,
                         msteams_config: Optional[pulumi.Input[Optional[pulumi.InputType['GetNotifierMsteamsConfigArgs']]]] = None,
                         name: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_pod_security_policy_template.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_pod_security_policy_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -397,43 +397,43 @@
     __args__['seLinux'] = se_linux
     __args__['supplementalGroup'] = supplemental_group
     __args__['volumes'] = volumes
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getPodSecurityPolicyTemplate:getPodSecurityPolicyTemplate', __args__, opts=opts, typ=GetPodSecurityPolicyTemplateResult).value
 
     return AwaitableGetPodSecurityPolicyTemplateResult(
-        allow_privilege_escalation=__ret__.allow_privilege_escalation,
-        allowed_capabilities=__ret__.allowed_capabilities,
-        allowed_csi_drivers=__ret__.allowed_csi_drivers,
-        allowed_flex_volumes=__ret__.allowed_flex_volumes,
-        allowed_host_paths=__ret__.allowed_host_paths,
-        allowed_proc_mount_types=__ret__.allowed_proc_mount_types,
-        allowed_unsafe_sysctls=__ret__.allowed_unsafe_sysctls,
-        annotations=__ret__.annotations,
-        default_add_capabilities=__ret__.default_add_capabilities,
-        default_allow_privilege_escalation=__ret__.default_allow_privilege_escalation,
-        description=__ret__.description,
-        forbidden_sysctls=__ret__.forbidden_sysctls,
-        fs_group=__ret__.fs_group,
-        host_ipc=__ret__.host_ipc,
-        host_network=__ret__.host_network,
-        host_pid=__ret__.host_pid,
-        host_ports=__ret__.host_ports,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        privileged=__ret__.privileged,
-        read_only_root_filesystem=__ret__.read_only_root_filesystem,
-        required_drop_capabilities=__ret__.required_drop_capabilities,
-        run_as_group=__ret__.run_as_group,
-        run_as_user=__ret__.run_as_user,
-        runtime_class=__ret__.runtime_class,
-        se_linux=__ret__.se_linux,
-        supplemental_group=__ret__.supplemental_group,
-        volumes=__ret__.volumes)
+        allow_privilege_escalation=pulumi.get(__ret__, 'allow_privilege_escalation'),
+        allowed_capabilities=pulumi.get(__ret__, 'allowed_capabilities'),
+        allowed_csi_drivers=pulumi.get(__ret__, 'allowed_csi_drivers'),
+        allowed_flex_volumes=pulumi.get(__ret__, 'allowed_flex_volumes'),
+        allowed_host_paths=pulumi.get(__ret__, 'allowed_host_paths'),
+        allowed_proc_mount_types=pulumi.get(__ret__, 'allowed_proc_mount_types'),
+        allowed_unsafe_sysctls=pulumi.get(__ret__, 'allowed_unsafe_sysctls'),
+        annotations=pulumi.get(__ret__, 'annotations'),
+        default_add_capabilities=pulumi.get(__ret__, 'default_add_capabilities'),
+        default_allow_privilege_escalation=pulumi.get(__ret__, 'default_allow_privilege_escalation'),
+        description=pulumi.get(__ret__, 'description'),
+        forbidden_sysctls=pulumi.get(__ret__, 'forbidden_sysctls'),
+        fs_group=pulumi.get(__ret__, 'fs_group'),
+        host_ipc=pulumi.get(__ret__, 'host_ipc'),
+        host_network=pulumi.get(__ret__, 'host_network'),
+        host_pid=pulumi.get(__ret__, 'host_pid'),
+        host_ports=pulumi.get(__ret__, 'host_ports'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        privileged=pulumi.get(__ret__, 'privileged'),
+        read_only_root_filesystem=pulumi.get(__ret__, 'read_only_root_filesystem'),
+        required_drop_capabilities=pulumi.get(__ret__, 'required_drop_capabilities'),
+        run_as_group=pulumi.get(__ret__, 'run_as_group'),
+        run_as_user=pulumi.get(__ret__, 'run_as_user'),
+        runtime_class=pulumi.get(__ret__, 'runtime_class'),
+        se_linux=pulumi.get(__ret__, 'se_linux'),
+        supplemental_group=pulumi.get(__ret__, 'supplemental_group'),
+        volumes=pulumi.get(__ret__, 'volumes'))
 
 
 @_utilities.lift_output_func(get_pod_security_policy_template)
 def get_pod_security_policy_template_output(allow_privilege_escalation: Optional[pulumi.Input[Optional[bool]]] = None,
                                             allowed_capabilities: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                                             allowed_csi_drivers: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetPodSecurityPolicyTemplateAllowedCsiDriverArgs']]]]] = None,
                                             allowed_flex_volumes: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetPodSecurityPolicyTemplateAllowedFlexVolumeArgs']]]]] = None,
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_principal.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_principal.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,17 +84,17 @@
     __args__ = dict()
     __args__['name'] = name
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getPrincipal:getPrincipal', __args__, opts=opts, typ=GetPrincipalResult).value
 
     return AwaitableGetPrincipalResult(
-        id=__ret__.id,
-        name=__ret__.name,
-        type=__ret__.type)
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_principal)
 def get_principal_output(name: Optional[pulumi.Input[str]] = None,
                          type: Optional[pulumi.Input[Optional[str]]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPrincipalResult]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_project.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_project.py`

 * *Files 10% similar despite different names*

```diff
@@ -171,25 +171,25 @@
     __args__ = dict()
     __args__['clusterId'] = cluster_id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getProject:getProject', __args__, opts=opts, typ=GetProjectResult).value
 
     return AwaitableGetProjectResult(
-        annotations=__ret__.annotations,
-        cluster_id=__ret__.cluster_id,
-        container_resource_limit=__ret__.container_resource_limit,
-        description=__ret__.description,
-        enable_project_monitoring=__ret__.enable_project_monitoring,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        pod_security_policy_template_id=__ret__.pod_security_policy_template_id,
-        resource_quota=__ret__.resource_quota,
-        uuid=__ret__.uuid)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        container_resource_limit=pulumi.get(__ret__, 'container_resource_limit'),
+        description=pulumi.get(__ret__, 'description'),
+        enable_project_monitoring=pulumi.get(__ret__, 'enable_project_monitoring'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        pod_security_policy_template_id=pulumi.get(__ret__, 'pod_security_policy_template_id'),
+        resource_quota=pulumi.get(__ret__, 'resource_quota'),
+        uuid=pulumi.get(__ret__, 'uuid'))
 
 
 @_utilities.lift_output_func(get_project)
 def get_project_output(cluster_id: Optional[pulumi.Input[str]] = None,
                        name: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectResult]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_project_alert_group.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_project_alert_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -170,24 +170,24 @@
     __args__ = dict()
     __args__['name'] = name
     __args__['projectId'] = project_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getProjectAlertGroup:getProjectAlertGroup', __args__, opts=opts, typ=GetProjectAlertGroupResult).value
 
     return AwaitableGetProjectAlertGroupResult(
-        annotations=__ret__.annotations,
-        description=__ret__.description,
-        group_interval_seconds=__ret__.group_interval_seconds,
-        group_wait_seconds=__ret__.group_wait_seconds,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        project_id=__ret__.project_id,
-        recipients=__ret__.recipients,
-        repeat_interval_seconds=__ret__.repeat_interval_seconds)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        description=pulumi.get(__ret__, 'description'),
+        group_interval_seconds=pulumi.get(__ret__, 'group_interval_seconds'),
+        group_wait_seconds=pulumi.get(__ret__, 'group_wait_seconds'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        recipients=pulumi.get(__ret__, 'recipients'),
+        repeat_interval_seconds=pulumi.get(__ret__, 'repeat_interval_seconds'))
 
 
 @_utilities.lift_output_func(get_project_alert_group)
 def get_project_alert_group_output(name: Optional[pulumi.Input[str]] = None,
                                    project_id: Optional[pulumi.Input[str]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectAlertGroupResult]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_project_alert_rule.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_project_alert_rule.py`

 * *Files 13% similar despite different names*

```diff
@@ -221,28 +221,28 @@
     __args__['labels'] = labels
     __args__['name'] = name
     __args__['projectId'] = project_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getProjectAlertRule:getProjectAlertRule', __args__, opts=opts, typ=GetProjectAlertRuleResult).value
 
     return AwaitableGetProjectAlertRuleResult(
-        annotations=__ret__.annotations,
-        group_id=__ret__.group_id,
-        group_interval_seconds=__ret__.group_interval_seconds,
-        group_wait_seconds=__ret__.group_wait_seconds,
-        id=__ret__.id,
-        inherited=__ret__.inherited,
-        labels=__ret__.labels,
-        metric_rule=__ret__.metric_rule,
-        name=__ret__.name,
-        pod_rule=__ret__.pod_rule,
-        project_id=__ret__.project_id,
-        repeat_interval_seconds=__ret__.repeat_interval_seconds,
-        severity=__ret__.severity,
-        workload_rule=__ret__.workload_rule)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        group_interval_seconds=pulumi.get(__ret__, 'group_interval_seconds'),
+        group_wait_seconds=pulumi.get(__ret__, 'group_wait_seconds'),
+        id=pulumi.get(__ret__, 'id'),
+        inherited=pulumi.get(__ret__, 'inherited'),
+        labels=pulumi.get(__ret__, 'labels'),
+        metric_rule=pulumi.get(__ret__, 'metric_rule'),
+        name=pulumi.get(__ret__, 'name'),
+        pod_rule=pulumi.get(__ret__, 'pod_rule'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        repeat_interval_seconds=pulumi.get(__ret__, 'repeat_interval_seconds'),
+        severity=pulumi.get(__ret__, 'severity'),
+        workload_rule=pulumi.get(__ret__, 'workload_rule'))
 
 
 @_utilities.lift_output_func(get_project_alert_rule)
 def get_project_alert_rule_output(labels: Optional[pulumi.Input[Optional[Mapping[str, Any]]]] = None,
                                   name: Optional[pulumi.Input[str]] = None,
                                   project_id: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectAlertRuleResult]:
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_project_role_template_binding.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_project_role_template_binding.py`

 * *Files 10% similar despite different names*

```diff
@@ -169,24 +169,24 @@
     __args__['name'] = name
     __args__['projectId'] = project_id
     __args__['roleTemplateId'] = role_template_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getProjectRoleTemplateBinding:getProjectRoleTemplateBinding', __args__, opts=opts, typ=GetProjectRoleTemplateBindingResult).value
 
     return AwaitableGetProjectRoleTemplateBindingResult(
-        annotations=__ret__.annotations,
-        group_id=__ret__.group_id,
-        group_principal_id=__ret__.group_principal_id,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        project_id=__ret__.project_id,
-        role_template_id=__ret__.role_template_id,
-        user_id=__ret__.user_id,
-        user_principal_id=__ret__.user_principal_id)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        group_principal_id=pulumi.get(__ret__, 'group_principal_id'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        role_template_id=pulumi.get(__ret__, 'role_template_id'),
+        user_id=pulumi.get(__ret__, 'user_id'),
+        user_principal_id=pulumi.get(__ret__, 'user_principal_id'))
 
 
 @_utilities.lift_output_func(get_project_role_template_binding)
 def get_project_role_template_binding_output(name: Optional[pulumi.Input[str]] = None,
                                              project_id: Optional[pulumi.Input[str]] = None,
                                              role_template_id: Optional[pulumi.Input[Optional[str]]] = None,
                                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectRoleTemplateBindingResult]:
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_registry.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -159,22 +159,22 @@
     __args__['name'] = name
     __args__['namespaceId'] = namespace_id
     __args__['projectId'] = project_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getRegistry:getRegistry', __args__, opts=opts, typ=GetRegistryResult).value
 
     return AwaitableGetRegistryResult(
-        annotations=__ret__.annotations,
-        description=__ret__.description,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        namespace_id=__ret__.namespace_id,
-        project_id=__ret__.project_id,
-        registries=__ret__.registries)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        namespace_id=pulumi.get(__ret__, 'namespace_id'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        registries=pulumi.get(__ret__, 'registries'))
 
 
 @_utilities.lift_output_func(get_registry)
 def get_registry_output(name: Optional[pulumi.Input[str]] = None,
                         namespace_id: Optional[pulumi.Input[Optional[str]]] = None,
                         project_id: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRegistryResult]:
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_role_tempalte.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_role_tempalte.py`

 * *Files 5% similar despite different names*

```diff
@@ -220,28 +220,28 @@
     __args__ = dict()
     __args__['context'] = context
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getRoleTempalte:getRoleTempalte', __args__, opts=opts, typ=GetRoleTempalteResult).value
 
     return AwaitableGetRoleTempalteResult(
-        administrative=__ret__.administrative,
-        annotations=__ret__.annotations,
-        builtin=__ret__.builtin,
-        context=__ret__.context,
-        default_role=__ret__.default_role,
-        description=__ret__.description,
-        external=__ret__.external,
-        hidden=__ret__.hidden,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        locked=__ret__.locked,
-        name=__ret__.name,
-        role_template_ids=__ret__.role_template_ids,
-        rules=__ret__.rules)
+        administrative=pulumi.get(__ret__, 'administrative'),
+        annotations=pulumi.get(__ret__, 'annotations'),
+        builtin=pulumi.get(__ret__, 'builtin'),
+        context=pulumi.get(__ret__, 'context'),
+        default_role=pulumi.get(__ret__, 'default_role'),
+        description=pulumi.get(__ret__, 'description'),
+        external=pulumi.get(__ret__, 'external'),
+        hidden=pulumi.get(__ret__, 'hidden'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        locked=pulumi.get(__ret__, 'locked'),
+        name=pulumi.get(__ret__, 'name'),
+        role_template_ids=pulumi.get(__ret__, 'role_template_ids'),
+        rules=pulumi.get(__ret__, 'rules'))
 
 
 @_utilities.lift_output_func(get_role_tempalte)
 def get_role_tempalte_output(context: Optional[pulumi.Input[Optional[str]]] = None,
                              name: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRoleTempalteResult]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_role_template.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_role_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -217,28 +217,28 @@
     __args__ = dict()
     __args__['context'] = context
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getRoleTemplate:getRoleTemplate', __args__, opts=opts, typ=GetRoleTemplateResult).value
 
     return AwaitableGetRoleTemplateResult(
-        administrative=__ret__.administrative,
-        annotations=__ret__.annotations,
-        builtin=__ret__.builtin,
-        context=__ret__.context,
-        default_role=__ret__.default_role,
-        description=__ret__.description,
-        external=__ret__.external,
-        hidden=__ret__.hidden,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        locked=__ret__.locked,
-        name=__ret__.name,
-        role_template_ids=__ret__.role_template_ids,
-        rules=__ret__.rules)
+        administrative=pulumi.get(__ret__, 'administrative'),
+        annotations=pulumi.get(__ret__, 'annotations'),
+        builtin=pulumi.get(__ret__, 'builtin'),
+        context=pulumi.get(__ret__, 'context'),
+        default_role=pulumi.get(__ret__, 'default_role'),
+        description=pulumi.get(__ret__, 'description'),
+        external=pulumi.get(__ret__, 'external'),
+        hidden=pulumi.get(__ret__, 'hidden'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        locked=pulumi.get(__ret__, 'locked'),
+        name=pulumi.get(__ret__, 'name'),
+        role_template_ids=pulumi.get(__ret__, 'role_template_ids'),
+        rules=pulumi.get(__ret__, 'rules'))
 
 
 @_utilities.lift_output_func(get_role_template)
 def get_role_template_output(context: Optional[pulumi.Input[Optional[str]]] = None,
                              name: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRoleTemplateResult]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_secret.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_secret.py`

 * *Files 8% similar despite different names*

```diff
@@ -158,22 +158,22 @@
     __args__['name'] = name
     __args__['namespaceId'] = namespace_id
     __args__['projectId'] = project_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getSecret:getSecret', __args__, opts=opts, typ=GetSecretResult).value
 
     return AwaitableGetSecretResult(
-        annotations=__ret__.annotations,
-        data=__ret__.data,
-        description=__ret__.description,
-        id=__ret__.id,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        namespace_id=__ret__.namespace_id,
-        project_id=__ret__.project_id)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        data=pulumi.get(__ret__, 'data'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        namespace_id=pulumi.get(__ret__, 'namespace_id'),
+        project_id=pulumi.get(__ret__, 'project_id'))
 
 
 @_utilities.lift_output_func(get_secret)
 def get_secret_output(name: Optional[pulumi.Input[str]] = None,
                       namespace_id: Optional[pulumi.Input[Optional[str]]] = None,
                       project_id: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSecretResult]:
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_secret_v2.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_secret_v2.py`

 * *Files 10% similar despite different names*

```diff
@@ -159,24 +159,24 @@
     __args__['clusterId'] = cluster_id
     __args__['name'] = name
     __args__['namespace'] = namespace
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getSecretV2:getSecretV2', __args__, opts=opts, typ=GetSecretV2Result).value
 
     return AwaitableGetSecretV2Result(
-        annotations=__ret__.annotations,
-        cluster_id=__ret__.cluster_id,
-        data=__ret__.data,
-        id=__ret__.id,
-        immutable=__ret__.immutable,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        namespace=__ret__.namespace,
-        resource_version=__ret__.resource_version,
-        type=__ret__.type)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        data=pulumi.get(__ret__, 'data'),
+        id=pulumi.get(__ret__, 'id'),
+        immutable=pulumi.get(__ret__, 'immutable'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        namespace=pulumi.get(__ret__, 'namespace'),
+        resource_version=pulumi.get(__ret__, 'resource_version'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_secret_v2)
 def get_secret_v2_output(cluster_id: Optional[pulumi.Input[str]] = None,
                          name: Optional[pulumi.Input[str]] = None,
                          namespace: Optional[pulumi.Input[Optional[str]]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSecretV2Result]:
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_setting.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_setting.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,17 +84,17 @@
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getSetting:getSetting', __args__, opts=opts, typ=GetSettingResult).value
 
     return AwaitableGetSettingResult(
-        id=__ret__.id,
-        name=__ret__.name,
-        value=__ret__.value)
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        value=pulumi.get(__ret__, 'value'))
 
 
 @_utilities.lift_output_func(get_setting)
 def get_setting_output(name: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSettingResult]:
     """
     Use this data source to retrieve information about a Rancher v2 setting.
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_storage_class_v2.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_storage_class_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -183,26 +183,26 @@
     __args__ = dict()
     __args__['clusterId'] = cluster_id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getStorageClassV2:getStorageClassV2', __args__, opts=opts, typ=GetStorageClassV2Result).value
 
     return AwaitableGetStorageClassV2Result(
-        allow_volume_expansion=__ret__.allow_volume_expansion,
-        annotations=__ret__.annotations,
-        cluster_id=__ret__.cluster_id,
-        id=__ret__.id,
-        k8s_provisioner=__ret__.k8s_provisioner,
-        labels=__ret__.labels,
-        mount_options=__ret__.mount_options,
-        name=__ret__.name,
-        parameters=__ret__.parameters,
-        reclaim_policy=__ret__.reclaim_policy,
-        resource_version=__ret__.resource_version,
-        volume_binding_mode=__ret__.volume_binding_mode)
+        allow_volume_expansion=pulumi.get(__ret__, 'allow_volume_expansion'),
+        annotations=pulumi.get(__ret__, 'annotations'),
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        id=pulumi.get(__ret__, 'id'),
+        k8s_provisioner=pulumi.get(__ret__, 'k8s_provisioner'),
+        labels=pulumi.get(__ret__, 'labels'),
+        mount_options=pulumi.get(__ret__, 'mount_options'),
+        name=pulumi.get(__ret__, 'name'),
+        parameters=pulumi.get(__ret__, 'parameters'),
+        reclaim_policy=pulumi.get(__ret__, 'reclaim_policy'),
+        resource_version=pulumi.get(__ret__, 'resource_version'),
+        volume_binding_mode=pulumi.get(__ret__, 'volume_binding_mode'))
 
 
 @_utilities.lift_output_func(get_storage_class_v2)
 def get_storage_class_v2_output(cluster_id: Optional[pulumi.Input[str]] = None,
                                 name: Optional[pulumi.Input[str]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetStorageClassV2Result]:
     """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/get_user.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/get_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -147,22 +147,22 @@
     __args__['isExternal'] = is_external
     __args__['name'] = name
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getUser:getUser', __args__, opts=opts, typ=GetUserResult).value
 
     return AwaitableGetUserResult(
-        annotations=__ret__.annotations,
-        enabled=__ret__.enabled,
-        id=__ret__.id,
-        is_external=__ret__.is_external,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        principal_ids=__ret__.principal_ids,
-        username=__ret__.username)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        enabled=pulumi.get(__ret__, 'enabled'),
+        id=pulumi.get(__ret__, 'id'),
+        is_external=pulumi.get(__ret__, 'is_external'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        principal_ids=pulumi.get(__ret__, 'principal_ids'),
+        username=pulumi.get(__ret__, 'username'))
 
 
 @_utilities.lift_output_func(get_user)
 def get_user_output(is_external: Optional[pulumi.Input[Optional[bool]]] = None,
                     name: Optional[pulumi.Input[Optional[str]]] = None,
                     username: Optional[pulumi.Input[Optional[str]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserResult]:
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/global_dns.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/global_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/global_dns_provider.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/global_dns_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/global_role.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/global_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/global_role_binding.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/global_role_binding.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         """
         The set of arguments for constructing a GlobalRoleBinding resource.
         :param pulumi.Input[str] global_role_id: The role id from create global role binding (string)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for global role binding (map)
         :param pulumi.Input[str] group_principal_id: The group principal ID to assign global role binding (only works with external auth providers that support groups). Rancher v2.4.0 or higher is required (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for global role binding (map)
                
-               **Note** user `user_id` OR group `group_principal_id` must be defined
+               **Note:** user `user_id` OR group `group_principal_id` must be defined
         :param pulumi.Input[str] name: The name of the global role binding (string)
         :param pulumi.Input[str] user_id: The user ID to assign global role binding (string)
         """
         pulumi.set(__self__, "global_role_id", global_role_id)
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
         if group_principal_id is not None:
@@ -81,15 +81,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Labels for global role binding (map)
 
-        **Note** user `user_id` OR group `group_principal_id` must be defined
+        **Note:** user `user_id` OR group `group_principal_id` must be defined
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "labels", value)
 
@@ -130,15 +130,15 @@
         """
         Input properties used for looking up and filtering GlobalRoleBinding resources.
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for global role binding (map)
         :param pulumi.Input[str] global_role_id: The role id from create global role binding (string)
         :param pulumi.Input[str] group_principal_id: The group principal ID to assign global role binding (only works with external auth providers that support groups). Rancher v2.4.0 or higher is required (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for global role binding (map)
                
-               **Note** user `user_id` OR group `group_principal_id` must be defined
+               **Note:** user `user_id` OR group `group_principal_id` must be defined
         :param pulumi.Input[str] name: The name of the global role binding (string)
         :param pulumi.Input[str] user_id: The user ID to assign global role binding (string)
         """
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
         if global_role_id is not None:
             pulumi.set(__self__, "global_role_id", global_role_id)
@@ -189,15 +189,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Labels for global role binding (map)
 
-        **Note** user `user_id` OR group `group_principal_id` must be defined
+        **Note:** user `user_id` OR group `group_principal_id` must be defined
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "labels", value)
 
@@ -268,15 +268,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for global role binding (map)
         :param pulumi.Input[str] global_role_id: The role id from create global role binding (string)
         :param pulumi.Input[str] group_principal_id: The group principal ID to assign global role binding (only works with external auth providers that support groups). Rancher v2.4.0 or higher is required (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for global role binding (map)
                
-               **Note** user `user_id` OR group `group_principal_id` must be defined
+               **Note:** user `user_id` OR group `group_principal_id` must be defined
         :param pulumi.Input[str] name: The name of the global role binding (string)
         :param pulumi.Input[str] user_id: The user ID to assign global role binding (string)
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -371,15 +371,15 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for global role binding (map)
         :param pulumi.Input[str] global_role_id: The role id from create global role binding (string)
         :param pulumi.Input[str] group_principal_id: The group principal ID to assign global role binding (only works with external auth providers that support groups). Rancher v2.4.0 or higher is required (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for global role binding (map)
                
-               **Note** user `user_id` OR group `group_principal_id` must be defined
+               **Note:** user `user_id` OR group `group_principal_id` must be defined
         :param pulumi.Input[str] name: The name of the global role binding (string)
         :param pulumi.Input[str] user_id: The user ID to assign global role binding (string)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _GlobalRoleBindingState.__new__(_GlobalRoleBindingState)
 
@@ -417,15 +417,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> pulumi.Output[Mapping[str, Any]]:
         """
         Labels for global role binding (map)
 
-        **Note** user `user_id` OR group `group_principal_id` must be defined
+        **Note:** user `user_id` OR group `group_principal_id` must be defined
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/machine_config_v2.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/machine_config_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for Machine Config V2 object (map)
         :param pulumi.Input['MachineConfigV2AzureConfigArgs'] azure_config: Azure config for the Machine Config V2. Conflicts with `amazonec2_config`, `digitalocean_config`, `harvester_config`, `linode_config`, `openstack_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input['MachineConfigV2DigitaloceanConfigArgs'] digitalocean_config: Digitalocean config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `harvester_config`, `linode_config`, `openstack_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[str] fleet_namespace: Cluster V2 fleet namespace
         :param pulumi.Input['MachineConfigV2HarvesterConfigArgs'] harvester_config: Harvester config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `linode_config`, `openstack_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Machine Config V2 object (map)
                
-               **Note** `labels` and `node_taints` will be applied to nodes deployed using the Machine Config V2
+               **Note:** `labels` and `node_taints` will be applied to nodes deployed using the Machine Config V2
         :param pulumi.Input['MachineConfigV2LinodeConfigArgs'] linode_config: Linode config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `harvester_config`, `openstack_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input['MachineConfigV2OpenstackConfigArgs'] openstack_config: Openstack config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `harvester_config`, `linode_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input['MachineConfigV2VsphereConfigArgs'] vsphere_config: vSphere config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `harvester_config`, `linode_config` and `openstack_config` (list maxitems:1)
         """
         pulumi.set(__self__, "generate_name", generate_name)
         if amazonec2_config is not None:
             pulumi.set(__self__, "amazonec2_config", amazonec2_config)
@@ -151,15 +151,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Labels for Machine Config V2 object (map)
 
-        **Note** `labels` and `node_taints` will be applied to nodes deployed using the Machine Config V2
+        **Note:** `labels` and `node_taints` will be applied to nodes deployed using the Machine Config V2
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "labels", value)
 
@@ -225,15 +225,15 @@
         :param pulumi.Input['MachineConfigV2DigitaloceanConfigArgs'] digitalocean_config: Digitalocean config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `harvester_config`, `linode_config`, `openstack_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[str] fleet_namespace: Cluster V2 fleet namespace
         :param pulumi.Input[str] generate_name: Cluster V2 generate name. The pattern to generate machine config name. e.g  generate_name=\\"prod-pool1\\" will generate \\"nc-prod-pool1-?????\\" name computed at `name` attribute (string)
         :param pulumi.Input['MachineConfigV2HarvesterConfigArgs'] harvester_config: Harvester config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `linode_config`, `openstack_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[str] kind: (Computed) The machine config kind (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Machine Config V2 object (map)
                
-               **Note** `labels` and `node_taints` will be applied to nodes deployed using the Machine Config V2
+               **Note:** `labels` and `node_taints` will be applied to nodes deployed using the Machine Config V2
         :param pulumi.Input['MachineConfigV2LinodeConfigArgs'] linode_config: Linode config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `harvester_config`, `openstack_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[str] name: (Computed) The machine config name (string)
         :param pulumi.Input['MachineConfigV2OpenstackConfigArgs'] openstack_config: Openstack config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `harvester_config`, `linode_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[str] resource_version: (Computed) The machine config k8s resource version (string)
         :param pulumi.Input['MachineConfigV2VsphereConfigArgs'] vsphere_config: vSphere config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `harvester_config`, `linode_config` and `openstack_config` (list maxitems:1)
         """
         if amazonec2_config is not None:
@@ -363,15 +363,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Labels for Machine Config V2 object (map)
 
-        **Note** `labels` and `node_taints` will be applied to nodes deployed using the Machine Config V2
+        **Note:** `labels` and `node_taints` will be applied to nodes deployed using the Machine Config V2
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "labels", value)
 
@@ -454,15 +454,15 @@
                  vsphere_config: Optional[pulumi.Input[pulumi.InputType['MachineConfigV2VsphereConfigArgs']]] = None,
                  __props__=None):
         """
         Provides a Rancher v2 Machine config v2 resource. This can be used to create Machine Config v2 for Rancher v2 and retrieve their information. This resource is available from Rancher v2.6.0 and above.
 
         `amazonec2`, `azure`, `digitalocean`, `harvester`, `linode`, `openstack`, and `vsphere` cloud providers are supported for machine config V2
 
-        **Note** This resource is used by
+        **Note:** This resource is used by
 
         ## Example Usage
         ### Using the Harvester Node Driver
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
@@ -518,15 +518,15 @@
         :param pulumi.Input[pulumi.InputType['MachineConfigV2AzureConfigArgs']] azure_config: Azure config for the Machine Config V2. Conflicts with `amazonec2_config`, `digitalocean_config`, `harvester_config`, `linode_config`, `openstack_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['MachineConfigV2DigitaloceanConfigArgs']] digitalocean_config: Digitalocean config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `harvester_config`, `linode_config`, `openstack_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[str] fleet_namespace: Cluster V2 fleet namespace
         :param pulumi.Input[str] generate_name: Cluster V2 generate name. The pattern to generate machine config name. e.g  generate_name=\\"prod-pool1\\" will generate \\"nc-prod-pool1-?????\\" name computed at `name` attribute (string)
         :param pulumi.Input[pulumi.InputType['MachineConfigV2HarvesterConfigArgs']] harvester_config: Harvester config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `linode_config`, `openstack_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Machine Config V2 object (map)
                
-               **Note** `labels` and `node_taints` will be applied to nodes deployed using the Machine Config V2
+               **Note:** `labels` and `node_taints` will be applied to nodes deployed using the Machine Config V2
         :param pulumi.Input[pulumi.InputType['MachineConfigV2LinodeConfigArgs']] linode_config: Linode config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `harvester_config`, `openstack_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['MachineConfigV2OpenstackConfigArgs']] openstack_config: Openstack config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `harvester_config`, `linode_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['MachineConfigV2VsphereConfigArgs']] vsphere_config: vSphere config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `harvester_config`, `linode_config` and `openstack_config` (list maxitems:1)
         """
         ...
     @overload
     def __init__(__self__,
@@ -534,15 +534,15 @@
                  args: MachineConfigV2Args,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Rancher v2 Machine config v2 resource. This can be used to create Machine Config v2 for Rancher v2 and retrieve their information. This resource is available from Rancher v2.6.0 and above.
 
         `amazonec2`, `azure`, `digitalocean`, `harvester`, `linode`, `openstack`, and `vsphere` cloud providers are supported for machine config V2
 
-        **Note** This resource is used by
+        **Note:** This resource is used by
 
         ## Example Usage
         ### Using the Harvester Node Driver
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
@@ -679,15 +679,15 @@
         :param pulumi.Input[pulumi.InputType['MachineConfigV2DigitaloceanConfigArgs']] digitalocean_config: Digitalocean config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `harvester_config`, `linode_config`, `openstack_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[str] fleet_namespace: Cluster V2 fleet namespace
         :param pulumi.Input[str] generate_name: Cluster V2 generate name. The pattern to generate machine config name. e.g  generate_name=\\"prod-pool1\\" will generate \\"nc-prod-pool1-?????\\" name computed at `name` attribute (string)
         :param pulumi.Input[pulumi.InputType['MachineConfigV2HarvesterConfigArgs']] harvester_config: Harvester config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `linode_config`, `openstack_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[str] kind: (Computed) The machine config kind (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Machine Config V2 object (map)
                
-               **Note** `labels` and `node_taints` will be applied to nodes deployed using the Machine Config V2
+               **Note:** `labels` and `node_taints` will be applied to nodes deployed using the Machine Config V2
         :param pulumi.Input[pulumi.InputType['MachineConfigV2LinodeConfigArgs']] linode_config: Linode config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `harvester_config`, `openstack_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[str] name: (Computed) The machine config name (string)
         :param pulumi.Input[pulumi.InputType['MachineConfigV2OpenstackConfigArgs']] openstack_config: Openstack config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `harvester_config`, `linode_config` and `vsphere_config` (list maxitems:1)
         :param pulumi.Input[str] resource_version: (Computed) The machine config k8s resource version (string)
         :param pulumi.Input[pulumi.InputType['MachineConfigV2VsphereConfigArgs']] vsphere_config: vSphere config for the Machine Config V2. Conflicts with `amazonec2_config`, `azure_config`, `digitalocean_config`, `harvester_config`, `linode_config` and `openstack_config` (list maxitems:1)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -776,15 +776,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> pulumi.Output[Mapping[str, Any]]:
         """
         Labels for Machine Config V2 object (map)
 
-        **Note** `labels` and `node_taints` will be applied to nodes deployed using the Machine Config V2
+        **Note:** `labels` and `node_taints` will be applied to nodes deployed using the Machine Config V2
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter(name="linodeConfig")
     def linode_config(self) -> pulumi.Output[Optional['outputs.MachineConfigV2LinodeConfig']]:
         """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/multi_cluster_app.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/multi_cluster_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/namespace.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/node_driver.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/node_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/node_pool.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/node_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,20 +32,20 @@
         """
         The set of arguments for constructing a NodePool resource.
         :param pulumi.Input[str] cluster_id: The RKE cluster id to use Node Pool (string)
         :param pulumi.Input[str] hostname_prefix: The prefix for created nodes of the Node Pool (string)
         :param pulumi.Input[str] node_template_id: The Node Template ID to use for node creation (string)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for Node Pool object (map)
         :param pulumi.Input[bool] control_plane: RKE control plane role for created nodes (bool)
-        :param pulumi.Input[int] delete_not_ready_after_secs: Delete not ready node after secs. For Rancher v2.3.3 or above. Default `0` (int)
+        :param pulumi.Input[int] delete_not_ready_after_secs: Delete not ready node after secs. For Rancher v2.3.3 and above. Default `0` (int)
         :param pulumi.Input[bool] drain_before_delete: Drain nodes before delete. Default: `false` (bool)
         :param pulumi.Input[bool] etcd: RKE etcd role for created nodes (bool)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Node Pool object (map)
         :param pulumi.Input[str] name: The name of the Node Pool (string)
-        :param pulumi.Input[Sequence[pulumi.Input['NodePoolNodeTaintArgs']]] node_taints: Node taints. For Rancher v2.3.3 or above (List)
+        :param pulumi.Input[Sequence[pulumi.Input['NodePoolNodeTaintArgs']]] node_taints: Node taints. For Rancher v2.3.3 and above (List)
         :param pulumi.Input[int] quantity: The number of nodes to create on Node Pool. Default `1`. Only values >= 1 allowed (int)
         :param pulumi.Input[bool] worker: RKE role role for created nodes (bool)
         """
         pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "hostname_prefix", hostname_prefix)
         pulumi.set(__self__, "node_template_id", node_template_id)
         if annotations is not None:
@@ -129,15 +129,15 @@
     def control_plane(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "control_plane", value)
 
     @property
     @pulumi.getter(name="deleteNotReadyAfterSecs")
     def delete_not_ready_after_secs(self) -> Optional[pulumi.Input[int]]:
         """
-        Delete not ready node after secs. For Rancher v2.3.3 or above. Default `0` (int)
+        Delete not ready node after secs. For Rancher v2.3.3 and above. Default `0` (int)
         """
         return pulumi.get(self, "delete_not_ready_after_secs")
 
     @delete_not_ready_after_secs.setter
     def delete_not_ready_after_secs(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "delete_not_ready_after_secs", value)
 
@@ -189,15 +189,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="nodeTaints")
     def node_taints(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NodePoolNodeTaintArgs']]]]:
         """
-        Node taints. For Rancher v2.3.3 or above (List)
+        Node taints. For Rancher v2.3.3 and above (List)
         """
         return pulumi.get(self, "node_taints")
 
     @node_taints.setter
     def node_taints(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NodePoolNodeTaintArgs']]]]):
         pulumi.set(self, "node_taints", value)
 
@@ -243,21 +243,21 @@
                  quantity: Optional[pulumi.Input[int]] = None,
                  worker: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering NodePool resources.
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for Node Pool object (map)
         :param pulumi.Input[str] cluster_id: The RKE cluster id to use Node Pool (string)
         :param pulumi.Input[bool] control_plane: RKE control plane role for created nodes (bool)
-        :param pulumi.Input[int] delete_not_ready_after_secs: Delete not ready node after secs. For Rancher v2.3.3 or above. Default `0` (int)
+        :param pulumi.Input[int] delete_not_ready_after_secs: Delete not ready node after secs. For Rancher v2.3.3 and above. Default `0` (int)
         :param pulumi.Input[bool] drain_before_delete: Drain nodes before delete. Default: `false` (bool)
         :param pulumi.Input[bool] etcd: RKE etcd role for created nodes (bool)
         :param pulumi.Input[str] hostname_prefix: The prefix for created nodes of the Node Pool (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Node Pool object (map)
         :param pulumi.Input[str] name: The name of the Node Pool (string)
-        :param pulumi.Input[Sequence[pulumi.Input['NodePoolNodeTaintArgs']]] node_taints: Node taints. For Rancher v2.3.3 or above (List)
+        :param pulumi.Input[Sequence[pulumi.Input['NodePoolNodeTaintArgs']]] node_taints: Node taints. For Rancher v2.3.3 and above (List)
         :param pulumi.Input[str] node_template_id: The Node Template ID to use for node creation (string)
         :param pulumi.Input[int] quantity: The number of nodes to create on Node Pool. Default `1`. Only values >= 1 allowed (int)
         :param pulumi.Input[bool] worker: RKE role role for created nodes (bool)
         """
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
         if cluster_id is not None:
@@ -321,15 +321,15 @@
     def control_plane(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "control_plane", value)
 
     @property
     @pulumi.getter(name="deleteNotReadyAfterSecs")
     def delete_not_ready_after_secs(self) -> Optional[pulumi.Input[int]]:
         """
-        Delete not ready node after secs. For Rancher v2.3.3 or above. Default `0` (int)
+        Delete not ready node after secs. For Rancher v2.3.3 and above. Default `0` (int)
         """
         return pulumi.get(self, "delete_not_ready_after_secs")
 
     @delete_not_ready_after_secs.setter
     def delete_not_ready_after_secs(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "delete_not_ready_after_secs", value)
 
@@ -393,15 +393,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="nodeTaints")
     def node_taints(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NodePoolNodeTaintArgs']]]]:
         """
-        Node taints. For Rancher v2.3.3 or above (List)
+        Node taints. For Rancher v2.3.3 and above (List)
         """
         return pulumi.get(self, "node_taints")
 
     @node_taints.setter
     def node_taints(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NodePoolNodeTaintArgs']]]]):
         pulumi.set(self, "node_taints", value)
 
@@ -473,21 +473,21 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for Node Pool object (map)
         :param pulumi.Input[str] cluster_id: The RKE cluster id to use Node Pool (string)
         :param pulumi.Input[bool] control_plane: RKE control plane role for created nodes (bool)
-        :param pulumi.Input[int] delete_not_ready_after_secs: Delete not ready node after secs. For Rancher v2.3.3 or above. Default `0` (int)
+        :param pulumi.Input[int] delete_not_ready_after_secs: Delete not ready node after secs. For Rancher v2.3.3 and above. Default `0` (int)
         :param pulumi.Input[bool] drain_before_delete: Drain nodes before delete. Default: `false` (bool)
         :param pulumi.Input[bool] etcd: RKE etcd role for created nodes (bool)
         :param pulumi.Input[str] hostname_prefix: The prefix for created nodes of the Node Pool (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Node Pool object (map)
         :param pulumi.Input[str] name: The name of the Node Pool (string)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NodePoolNodeTaintArgs']]]] node_taints: Node taints. For Rancher v2.3.3 or above (List)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NodePoolNodeTaintArgs']]]] node_taints: Node taints. For Rancher v2.3.3 and above (List)
         :param pulumi.Input[str] node_template_id: The Node Template ID to use for node creation (string)
         :param pulumi.Input[int] quantity: The number of nodes to create on Node Pool. Default `1`. Only values >= 1 allowed (int)
         :param pulumi.Input[bool] worker: RKE role role for created nodes (bool)
         """
         ...
     @overload
     def __init__(__self__,
@@ -590,21 +590,21 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for Node Pool object (map)
         :param pulumi.Input[str] cluster_id: The RKE cluster id to use Node Pool (string)
         :param pulumi.Input[bool] control_plane: RKE control plane role for created nodes (bool)
-        :param pulumi.Input[int] delete_not_ready_after_secs: Delete not ready node after secs. For Rancher v2.3.3 or above. Default `0` (int)
+        :param pulumi.Input[int] delete_not_ready_after_secs: Delete not ready node after secs. For Rancher v2.3.3 and above. Default `0` (int)
         :param pulumi.Input[bool] drain_before_delete: Drain nodes before delete. Default: `false` (bool)
         :param pulumi.Input[bool] etcd: RKE etcd role for created nodes (bool)
         :param pulumi.Input[str] hostname_prefix: The prefix for created nodes of the Node Pool (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Node Pool object (map)
         :param pulumi.Input[str] name: The name of the Node Pool (string)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NodePoolNodeTaintArgs']]]] node_taints: Node taints. For Rancher v2.3.3 or above (List)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NodePoolNodeTaintArgs']]]] node_taints: Node taints. For Rancher v2.3.3 and above (List)
         :param pulumi.Input[str] node_template_id: The Node Template ID to use for node creation (string)
         :param pulumi.Input[int] quantity: The number of nodes to create on Node Pool. Default `1`. Only values >= 1 allowed (int)
         :param pulumi.Input[bool] worker: RKE role role for created nodes (bool)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _NodePoolState.__new__(_NodePoolState)
@@ -648,15 +648,15 @@
         """
         return pulumi.get(self, "control_plane")
 
     @property
     @pulumi.getter(name="deleteNotReadyAfterSecs")
     def delete_not_ready_after_secs(self) -> pulumi.Output[Optional[int]]:
         """
-        Delete not ready node after secs. For Rancher v2.3.3 or above. Default `0` (int)
+        Delete not ready node after secs. For Rancher v2.3.3 and above. Default `0` (int)
         """
         return pulumi.get(self, "delete_not_ready_after_secs")
 
     @property
     @pulumi.getter(name="drainBeforeDelete")
     def drain_before_delete(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -696,15 +696,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="nodeTaints")
     def node_taints(self) -> pulumi.Output[Optional[Sequence['outputs.NodePoolNodeTaint']]]:
         """
-        Node taints. For Rancher v2.3.3 or above (List)
+        Node taints. For Rancher v2.3.3 and above (List)
         """
         return pulumi.get(self, "node_taints")
 
     @property
     @pulumi.getter(name="nodeTemplateId")
     def node_template_id(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/node_template.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/node_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,18 +61,18 @@
         :param pulumi.Input[Mapping[str, Any]] engine_opt: Engine options for the node template (map)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] engine_registry_mirrors: Engine registry mirror for the node template (list)
         :param pulumi.Input[str] engine_storage_driver: Engine storage driver for the node template (string)
         :param pulumi.Input['NodeTemplateHarvesterConfigArgs'] harvester_config: Harvester config for the Node Template (list maxitems:1)
         :param pulumi.Input['NodeTemplateHetznerConfigArgs'] hetzner_config: Hetzner config for the Node Template (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Node Template object (map)
                
-               **Note** `labels` and `node_taints` will be applied to nodes deployed using the Node Template
+               **Note:** `labels` and `node_taints` will be applied to nodes deployed using the Node Template
         :param pulumi.Input['NodeTemplateLinodeConfigArgs'] linode_config: Linode config for the Node Template (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Node Template (string)
-        :param pulumi.Input[Sequence[pulumi.Input['NodeTemplateNodeTaintArgs']]] node_taints: Node taints. For Rancher v2.3.3 or above (List)
+        :param pulumi.Input[Sequence[pulumi.Input['NodeTemplateNodeTaintArgs']]] node_taints: Node taints. For Rancher v2.3.3 and above (List)
         :param pulumi.Input['NodeTemplateOpennebulaConfigArgs'] opennebula_config: Opennebula config for the Node Template (list maxitems:1)
         :param pulumi.Input['NodeTemplateOpenstackConfigArgs'] openstack_config: Openstack config for the Node Template (list maxitems:1)
         :param pulumi.Input['NodeTemplateOutscaleConfigArgs'] outscale_config: Outscale config for the Node Template (list maxitems:1)
         :param pulumi.Input[bool] use_internal_ip_address: Engine storage driver for the node template (bool)
         :param pulumi.Input['NodeTemplateVsphereConfigArgs'] vsphere_config: vSphere config for the Node Template (list maxitems:1)
         """
         if amazonec2_config is not None:
@@ -348,15 +348,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Labels for Node Template object (map)
 
-        **Note** `labels` and `node_taints` will be applied to nodes deployed using the Node Template
+        **Note:** `labels` and `node_taints` will be applied to nodes deployed using the Node Template
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "labels", value)
 
@@ -384,15 +384,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="nodeTaints")
     def node_taints(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NodeTemplateNodeTaintArgs']]]]:
         """
-        Node taints. For Rancher v2.3.3 or above (List)
+        Node taints. For Rancher v2.3.3 and above (List)
         """
         return pulumi.get(self, "node_taints")
 
     @node_taints.setter
     def node_taints(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NodeTemplateNodeTaintArgs']]]]):
         pulumi.set(self, "node_taints", value)
 
@@ -507,18 +507,18 @@
         :param pulumi.Input[Mapping[str, Any]] engine_opt: Engine options for the node template (map)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] engine_registry_mirrors: Engine registry mirror for the node template (list)
         :param pulumi.Input[str] engine_storage_driver: Engine storage driver for the node template (string)
         :param pulumi.Input['NodeTemplateHarvesterConfigArgs'] harvester_config: Harvester config for the Node Template (list maxitems:1)
         :param pulumi.Input['NodeTemplateHetznerConfigArgs'] hetzner_config: Hetzner config for the Node Template (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Node Template object (map)
                
-               **Note** `labels` and `node_taints` will be applied to nodes deployed using the Node Template
+               **Note:** `labels` and `node_taints` will be applied to nodes deployed using the Node Template
         :param pulumi.Input['NodeTemplateLinodeConfigArgs'] linode_config: Linode config for the Node Template (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Node Template (string)
-        :param pulumi.Input[Sequence[pulumi.Input['NodeTemplateNodeTaintArgs']]] node_taints: Node taints. For Rancher v2.3.3 or above (List)
+        :param pulumi.Input[Sequence[pulumi.Input['NodeTemplateNodeTaintArgs']]] node_taints: Node taints. For Rancher v2.3.3 and above (List)
         :param pulumi.Input['NodeTemplateOpennebulaConfigArgs'] opennebula_config: Opennebula config for the Node Template (list maxitems:1)
         :param pulumi.Input['NodeTemplateOpenstackConfigArgs'] openstack_config: Openstack config for the Node Template (list maxitems:1)
         :param pulumi.Input['NodeTemplateOutscaleConfigArgs'] outscale_config: Outscale config for the Node Template (list maxitems:1)
         :param pulumi.Input[bool] use_internal_ip_address: Engine storage driver for the node template (bool)
         :param pulumi.Input['NodeTemplateVsphereConfigArgs'] vsphere_config: vSphere config for the Node Template (list maxitems:1)
         """
         if amazonec2_config is not None:
@@ -808,15 +808,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Labels for Node Template object (map)
 
-        **Note** `labels` and `node_taints` will be applied to nodes deployed using the Node Template
+        **Note:** `labels` and `node_taints` will be applied to nodes deployed using the Node Template
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "labels", value)
 
@@ -844,15 +844,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="nodeTaints")
     def node_taints(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NodeTemplateNodeTaintArgs']]]]:
         """
-        Node taints. For Rancher v2.3.3 or above (List)
+        Node taints. For Rancher v2.3.3 and above (List)
         """
         return pulumi.get(self, "node_taints")
 
     @node_taints.setter
     def node_taints(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NodeTemplateNodeTaintArgs']]]]):
         pulumi.set(self, "node_taints", value)
 
@@ -951,15 +951,15 @@
                  vsphere_config: Optional[pulumi.Input[pulumi.InputType['NodeTemplateVsphereConfigArgs']]] = None,
                  __props__=None):
         """
         Provides a Rancher v2 Node Template resource. This can be used to create Node Template for Rancher v2 and retrieve their information.
 
         amazonec2, azure, digitalocean, harvester, linode, opennebula, openstack, outscale, hetzner and vsphere drivers are supported for node templates.
 
-        **Note** If you are upgrading to Rancher v2.3.3, please take a look to final section
+        **Note:** If you are upgrading to Rancher v2.3.3, please take a look to final section
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
@@ -1100,18 +1100,18 @@
         :param pulumi.Input[Mapping[str, Any]] engine_opt: Engine options for the node template (map)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] engine_registry_mirrors: Engine registry mirror for the node template (list)
         :param pulumi.Input[str] engine_storage_driver: Engine storage driver for the node template (string)
         :param pulumi.Input[pulumi.InputType['NodeTemplateHarvesterConfigArgs']] harvester_config: Harvester config for the Node Template (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['NodeTemplateHetznerConfigArgs']] hetzner_config: Hetzner config for the Node Template (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Node Template object (map)
                
-               **Note** `labels` and `node_taints` will be applied to nodes deployed using the Node Template
+               **Note:** `labels` and `node_taints` will be applied to nodes deployed using the Node Template
         :param pulumi.Input[pulumi.InputType['NodeTemplateLinodeConfigArgs']] linode_config: Linode config for the Node Template (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Node Template (string)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NodeTemplateNodeTaintArgs']]]] node_taints: Node taints. For Rancher v2.3.3 or above (List)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NodeTemplateNodeTaintArgs']]]] node_taints: Node taints. For Rancher v2.3.3 and above (List)
         :param pulumi.Input[pulumi.InputType['NodeTemplateOpennebulaConfigArgs']] opennebula_config: Opennebula config for the Node Template (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['NodeTemplateOpenstackConfigArgs']] openstack_config: Openstack config for the Node Template (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['NodeTemplateOutscaleConfigArgs']] outscale_config: Outscale config for the Node Template (list maxitems:1)
         :param pulumi.Input[bool] use_internal_ip_address: Engine storage driver for the node template (bool)
         :param pulumi.Input[pulumi.InputType['NodeTemplateVsphereConfigArgs']] vsphere_config: vSphere config for the Node Template (list maxitems:1)
         """
         ...
@@ -1121,15 +1121,15 @@
                  args: Optional[NodeTemplateArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Rancher v2 Node Template resource. This can be used to create Node Template for Rancher v2 and retrieve their information.
 
         amazonec2, azure, digitalocean, harvester, linode, opennebula, openstack, outscale, hetzner and vsphere drivers are supported for node templates.
 
-        **Note** If you are upgrading to Rancher v2.3.3, please take a look to final section
+        **Note:** If you are upgrading to Rancher v2.3.3, please take a look to final section
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
@@ -1395,18 +1395,18 @@
         :param pulumi.Input[Mapping[str, Any]] engine_opt: Engine options for the node template (map)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] engine_registry_mirrors: Engine registry mirror for the node template (list)
         :param pulumi.Input[str] engine_storage_driver: Engine storage driver for the node template (string)
         :param pulumi.Input[pulumi.InputType['NodeTemplateHarvesterConfigArgs']] harvester_config: Harvester config for the Node Template (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['NodeTemplateHetznerConfigArgs']] hetzner_config: Hetzner config for the Node Template (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for Node Template object (map)
                
-               **Note** `labels` and `node_taints` will be applied to nodes deployed using the Node Template
+               **Note:** `labels` and `node_taints` will be applied to nodes deployed using the Node Template
         :param pulumi.Input[pulumi.InputType['NodeTemplateLinodeConfigArgs']] linode_config: Linode config for the Node Template (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Node Template (string)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NodeTemplateNodeTaintArgs']]]] node_taints: Node taints. For Rancher v2.3.3 or above (List)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NodeTemplateNodeTaintArgs']]]] node_taints: Node taints. For Rancher v2.3.3 and above (List)
         :param pulumi.Input[pulumi.InputType['NodeTemplateOpennebulaConfigArgs']] opennebula_config: Opennebula config for the Node Template (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['NodeTemplateOpenstackConfigArgs']] openstack_config: Openstack config for the Node Template (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['NodeTemplateOutscaleConfigArgs']] outscale_config: Outscale config for the Node Template (list maxitems:1)
         :param pulumi.Input[bool] use_internal_ip_address: Engine storage driver for the node template (bool)
         :param pulumi.Input[pulumi.InputType['NodeTemplateVsphereConfigArgs']] vsphere_config: vSphere config for the Node Template (list maxitems:1)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -1597,15 +1597,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> pulumi.Output[Mapping[str, Any]]:
         """
         Labels for Node Template object (map)
 
-        **Note** `labels` and `node_taints` will be applied to nodes deployed using the Node Template
+        **Note:** `labels` and `node_taints` will be applied to nodes deployed using the Node Template
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter(name="linodeConfig")
     def linode_config(self) -> pulumi.Output[Optional['outputs.NodeTemplateLinodeConfig']]:
         """
@@ -1621,15 +1621,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="nodeTaints")
     def node_taints(self) -> pulumi.Output[Optional[Sequence['outputs.NodeTemplateNodeTaint']]]:
         """
-        Node taints. For Rancher v2.3.3 or above (List)
+        Node taints. For Rancher v2.3.3 and above (List)
         """
         return pulumi.get(self, "node_taints")
 
     @property
     @pulumi.getter(name="opennebulaConfig")
     def opennebula_config(self) -> pulumi.Output[Optional['outputs.NodeTemplateOpennebulaConfig']]:
         """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/notifier.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/notifier.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/outputs.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1608,14 +1608,17 @@
 
     @property
     @pulumi.getter
     def tag(self) -> Optional[Mapping[str, Any]]:
         """
         Use `tags` argument instead as []string
         """
+        warnings.warn("""Use tags argument instead as []string""", DeprecationWarning)
+        pulumi.log.warn("""tag is deprecated: Use tags argument instead as []string""")
+
         return pulumi.get(self, "tag")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Sequence[str]]:
         """
         Tags for Kubernetes cluster. For example, `["foo=bar","bar=foo"]` (list)
@@ -2870,50 +2873,64 @@
         ClusterClusterAgentDeploymentCustomization.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  append_tolerations: Optional[Sequence['outputs.ClusterClusterAgentDeploymentCustomizationAppendToleration']] = None,
                  override_affinity: Optional[str] = None,
                  override_resource_requirements: Optional[Sequence['outputs.ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirement']] = None):
+        """
+        :param Sequence['ClusterClusterAgentDeploymentCustomizationAppendTolerationArgs'] append_tolerations: User defined tolerations to append to agent (list)
+        :param str override_affinity: User defined affinity to override default agent affinity (string)
+        :param Sequence['ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs'] override_resource_requirements: User defined resource requirements to set on the agent (list)
+        """
         if append_tolerations is not None:
             pulumi.set(__self__, "append_tolerations", append_tolerations)
         if override_affinity is not None:
             pulumi.set(__self__, "override_affinity", override_affinity)
         if override_resource_requirements is not None:
             pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
 
     @property
     @pulumi.getter(name="appendTolerations")
     def append_tolerations(self) -> Optional[Sequence['outputs.ClusterClusterAgentDeploymentCustomizationAppendToleration']]:
+        """
+        User defined tolerations to append to agent (list)
+        """
         return pulumi.get(self, "append_tolerations")
 
     @property
     @pulumi.getter(name="overrideAffinity")
     def override_affinity(self) -> Optional[str]:
+        """
+        User defined affinity to override default agent affinity (string)
+        """
         return pulumi.get(self, "override_affinity")
 
     @property
     @pulumi.getter(name="overrideResourceRequirements")
     def override_resource_requirements(self) -> Optional[Sequence['outputs.ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirement']]:
+        """
+        User defined resource requirements to set on the agent (list)
+        """
         return pulumi.get(self, "override_resource_requirements")
 
 
 @pulumi.output_type
 class ClusterClusterAgentDeploymentCustomizationAppendToleration(dict):
     def __init__(__self__, *,
                  key: str,
                  effect: Optional[str] = None,
                  operator: Optional[str] = None,
                  seconds: Optional[int] = None,
                  value: Optional[str] = None):
         """
         :param str key: The toleration key (string)
-        :param str effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
-        :param str operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
-        :param int seconds: The toleration seconds (int)
+        :param str effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param str operator: The toleration operator (string)
+        :param int seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param str value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -2930,31 +2947,31 @@
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[str]:
         """
-        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[str]:
         """
-        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[int]:
         """
-        The toleration seconds (int)
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
         """
         return pulumi.get(self, "seconds")
 
     @property
     @pulumi.getter
     def value(self) -> Optional[str]:
         """
@@ -2989,41 +3006,59 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  cpu_limit: Optional[str] = None,
                  cpu_request: Optional[str] = None,
                  memory_limit: Optional[str] = None,
                  memory_request: Optional[str] = None):
+        """
+        :param str cpu_limit: The maximum CPU limit for agent (string)
+        :param str cpu_request: The minimum CPU required for agent (string)
+        :param str memory_limit: The maximum memory limit for agent (string)
+        :param str memory_request: The minimum memory required for agent (string)
+        """
         if cpu_limit is not None:
             pulumi.set(__self__, "cpu_limit", cpu_limit)
         if cpu_request is not None:
             pulumi.set(__self__, "cpu_request", cpu_request)
         if memory_limit is not None:
             pulumi.set(__self__, "memory_limit", memory_limit)
         if memory_request is not None:
             pulumi.set(__self__, "memory_request", memory_request)
 
     @property
     @pulumi.getter(name="cpuLimit")
     def cpu_limit(self) -> Optional[str]:
+        """
+        The maximum CPU limit for agent (string)
+        """
         return pulumi.get(self, "cpu_limit")
 
     @property
     @pulumi.getter(name="cpuRequest")
     def cpu_request(self) -> Optional[str]:
+        """
+        The minimum CPU required for agent (string)
+        """
         return pulumi.get(self, "cpu_request")
 
     @property
     @pulumi.getter(name="memoryLimit")
     def memory_limit(self) -> Optional[str]:
+        """
+        The maximum memory limit for agent (string)
+        """
         return pulumi.get(self, "memory_limit")
 
     @property
     @pulumi.getter(name="memoryRequest")
     def memory_request(self) -> Optional[str]:
+        """
+        The minimum memory required for agent (string)
+        """
         return pulumi.get(self, "memory_request")
 
 
 @pulumi.output_type
 class ClusterClusterAuthEndpoint(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3492,17 +3527,17 @@
                  virtual_network: Optional[str] = None):
         """
         :param str access_key: Access key for S3 service (string)
         :param str kubernetes_version: K8s version to deploy. Default: `Rancher default` (string) (Note - if rke_config is set at cluster_template, kubernetes_version must be set to the active cluster version so Rancher can clone the RKE template)
         :param str secret_key: Secret key for S3 service (string)
         :param str ami: AMI ID to use for the worker nodes instead of the default (string)
         :param bool associate_worker_node_public_ip: Associate public ip EKS worker nodes. Default `true` (bool)
-        :param int desired_nodes: The desired number of worker nodes. Just for Rancher v2.3.x and above. Default `3` (int)
+        :param int desired_nodes: The desired number of worker nodes. For Rancher v2.3.x and above. Default `3` (int)
         :param str instance_type: The type of machine to use for worker nodes. Default `t2.medium` (string)
-        :param str key_pair_name: Allow user to specify key name to use. Just for Rancher v2.2.7 and above (string)
+        :param str key_pair_name: Allow user to specify key name to use. For Rancher v2.2.7 and above (string)
         :param int maximum_nodes: The maximum number of worker nodes. Default `3` (int)
         :param int minimum_nodes: The minimum number of worker nodes. Default `1` (int)
         :param int node_volume_size: The volume size for each node. Default `20` (int)
         :param str region: (string)
         :param Sequence[str] security_groups: List of security groups to use for the cluster. If it's not specified Rancher will create a new security group (list)
         :param str service_role: The service role to use to perform the cluster operations in AWS. If it's not specified Rancher will create a new service role (string)
         :param str session_token: A session token to use with the client key and secret if applicable (string)
@@ -3586,15 +3621,15 @@
         """
         return pulumi.get(self, "associate_worker_node_public_ip")
 
     @property
     @pulumi.getter(name="desiredNodes")
     def desired_nodes(self) -> Optional[int]:
         """
-        The desired number of worker nodes. Just for Rancher v2.3.x and above. Default `3` (int)
+        The desired number of worker nodes. For Rancher v2.3.x and above. Default `3` (int)
         """
         return pulumi.get(self, "desired_nodes")
 
     @property
     @pulumi.getter(name="ebsEncryption")
     def ebs_encryption(self) -> Optional[bool]:
         return pulumi.get(self, "ebs_encryption")
@@ -3607,15 +3642,15 @@
         """
         return pulumi.get(self, "instance_type")
 
     @property
     @pulumi.getter(name="keyPairName")
     def key_pair_name(self) -> Optional[str]:
         """
-        Allow user to specify key name to use. Just for Rancher v2.2.7 and above (string)
+        Allow user to specify key name to use. For Rancher v2.2.7 and above (string)
         """
         return pulumi.get(self, "key_pair_name")
 
     @property
     @pulumi.getter(name="maximumNodes")
     def maximum_nodes(self) -> Optional[int]:
         """
@@ -4275,50 +4310,64 @@
         ClusterFleetAgentDeploymentCustomization.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  append_tolerations: Optional[Sequence['outputs.ClusterFleetAgentDeploymentCustomizationAppendToleration']] = None,
                  override_affinity: Optional[str] = None,
                  override_resource_requirements: Optional[Sequence['outputs.ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirement']] = None):
+        """
+        :param Sequence['ClusterFleetAgentDeploymentCustomizationAppendTolerationArgs'] append_tolerations: User defined tolerations to append to agent (list)
+        :param str override_affinity: User defined affinity to override default agent affinity (string)
+        :param Sequence['ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirementArgs'] override_resource_requirements: User defined resource requirements to set on the agent (list)
+        """
         if append_tolerations is not None:
             pulumi.set(__self__, "append_tolerations", append_tolerations)
         if override_affinity is not None:
             pulumi.set(__self__, "override_affinity", override_affinity)
         if override_resource_requirements is not None:
             pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
 
     @property
     @pulumi.getter(name="appendTolerations")
     def append_tolerations(self) -> Optional[Sequence['outputs.ClusterFleetAgentDeploymentCustomizationAppendToleration']]:
+        """
+        User defined tolerations to append to agent (list)
+        """
         return pulumi.get(self, "append_tolerations")
 
     @property
     @pulumi.getter(name="overrideAffinity")
     def override_affinity(self) -> Optional[str]:
+        """
+        User defined affinity to override default agent affinity (string)
+        """
         return pulumi.get(self, "override_affinity")
 
     @property
     @pulumi.getter(name="overrideResourceRequirements")
     def override_resource_requirements(self) -> Optional[Sequence['outputs.ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirement']]:
+        """
+        User defined resource requirements to set on the agent (list)
+        """
         return pulumi.get(self, "override_resource_requirements")
 
 
 @pulumi.output_type
 class ClusterFleetAgentDeploymentCustomizationAppendToleration(dict):
     def __init__(__self__, *,
                  key: str,
                  effect: Optional[str] = None,
                  operator: Optional[str] = None,
                  seconds: Optional[int] = None,
                  value: Optional[str] = None):
         """
         :param str key: The toleration key (string)
-        :param str effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
-        :param str operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
-        :param int seconds: The toleration seconds (int)
+        :param str effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param str operator: The toleration operator (string)
+        :param int seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param str value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -4335,31 +4384,31 @@
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[str]:
         """
-        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[str]:
         """
-        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[int]:
         """
-        The toleration seconds (int)
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
         """
         return pulumi.get(self, "seconds")
 
     @property
     @pulumi.getter
     def value(self) -> Optional[str]:
         """
@@ -4394,41 +4443,59 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  cpu_limit: Optional[str] = None,
                  cpu_request: Optional[str] = None,
                  memory_limit: Optional[str] = None,
                  memory_request: Optional[str] = None):
+        """
+        :param str cpu_limit: The maximum CPU limit for agent (string)
+        :param str cpu_request: The minimum CPU required for agent (string)
+        :param str memory_limit: The maximum memory limit for agent (string)
+        :param str memory_request: The minimum memory required for agent (string)
+        """
         if cpu_limit is not None:
             pulumi.set(__self__, "cpu_limit", cpu_limit)
         if cpu_request is not None:
             pulumi.set(__self__, "cpu_request", cpu_request)
         if memory_limit is not None:
             pulumi.set(__self__, "memory_limit", memory_limit)
         if memory_request is not None:
             pulumi.set(__self__, "memory_request", memory_request)
 
     @property
     @pulumi.getter(name="cpuLimit")
     def cpu_limit(self) -> Optional[str]:
+        """
+        The maximum CPU limit for agent (string)
+        """
         return pulumi.get(self, "cpu_limit")
 
     @property
     @pulumi.getter(name="cpuRequest")
     def cpu_request(self) -> Optional[str]:
+        """
+        The minimum CPU required for agent (string)
+        """
         return pulumi.get(self, "cpu_request")
 
     @property
     @pulumi.getter(name="memoryLimit")
     def memory_limit(self) -> Optional[str]:
+        """
+        The maximum memory limit for agent (string)
+        """
         return pulumi.get(self, "memory_limit")
 
     @property
     @pulumi.getter(name="memoryRequest")
     def memory_request(self) -> Optional[str]:
+        """
+        The minimum memory required for agent (string)
+        """
         return pulumi.get(self, "memory_request")
 
 
 @pulumi.output_type
 class ClusterGkeConfig(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -6099,27 +6166,27 @@
 @pulumi.output_type
 class ClusterGkeConfigV2NodePoolConfigTaint(dict):
     def __init__(__self__, *,
                  effect: str,
                  key: str,
                  value: str):
         """
-        :param str effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        :param str effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
         :param str key: The toleration key (string)
         :param str value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "effect", effect)
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def effect(self) -> str:
         """
-        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @property
     @pulumi.getter
     def key(self) -> str:
         """
@@ -6492,18 +6559,18 @@
         :param str private_key_contents: The private API key file contents for the specified user, in PEM format (string)
         :param str region: (string)
         :param str tenancy_id: The OCID of the tenancy in which to create resources (string)
         :param str user_ocid: The OCID of a user who has access to the tenancy/compartment (string)
         :param int custom_boot_volume_size: Optional custom boot volume size (GB) for all nodes. If you specify 0, it will apply the default according to the `node_image` specified. Default `0` (int)
         :param str description: The description for Cluster (string)
         :param bool enable_kubernetes_dashboard: Whether to enable the Kubernetes dashboard. Default `false` (bool)
-        :param bool enable_private_control_plane: Specifies whether Kubernetes API endpoint is a private IP only accessible from within the VCN. Default `false` Just for Rancher v2.5.10 or above (bool)
+        :param bool enable_private_control_plane: Specifies whether Kubernetes API endpoint is a private IP only accessible from within the VCN. Default `false` for Rancher v2.5.10 and above (bool)
         :param bool enable_private_nodes: Whether nodes have internal IP address only. Default `false` (bool)
         :param int flex_ocpus: Specifies number of OCPUs for nodes (requires flexible shape specified with `node_shape`) (int)
-        :param str kms_key_id: The OCID of a KMS vault master key used to encrypt secrets at rest. See [here](https://docs.oracle.com/en-us/iaas/Content/ContEng/Tasks/contengencryptingdata.htm) for help creating a vault and master encryption key. Just for Rancher v2.5.9 or above (string)
+        :param str kms_key_id: The OCID of a KMS vault master key used to encrypt secrets at rest. See [here](https://docs.oracle.com/en-us/iaas/Content/ContEng/Tasks/contengencryptingdata.htm) for help creating a vault and master encryption key. For Rancher v2.5.9 and above (string)
         :param int limit_node_count: The maximum number of worker nodes. Can limit `quantity_per_subnet`. Default `0` (no limit) (int)
         :param str load_balancer_subnet_name1: The name of the first existing subnet to use for Kubernetes services / LB. `vcn_name` is also required when specifying an existing subnet. (string)
         :param str load_balancer_subnet_name2: The name of a second existing subnet to use for Kubernetes services / LB. A second subnet is only required when it is AD-specific (non-regional) (string)
         :param str node_pool_dns_domain_name: Name for DNS domain of node pool subnet. Default `nodedns` (string)
         :param str node_pool_subnet_name: Name for node pool subnet. Default `nodedns` (string)
         :param str node_public_key_contents: The contents of the SSH public key file to use for the nodes (string)
         :param str pod_cidr: A CIDR notation IP range from which to assign Kubernetes Pod IPs when \\"network plugin\\" is specified in \\"kubenet\\". Default `172.244.0.0/16` (string)
@@ -6669,15 +6736,15 @@
         """
         return pulumi.get(self, "enable_kubernetes_dashboard")
 
     @property
     @pulumi.getter(name="enablePrivateControlPlane")
     def enable_private_control_plane(self) -> Optional[bool]:
         """
-        Specifies whether Kubernetes API endpoint is a private IP only accessible from within the VCN. Default `false` Just for Rancher v2.5.10 or above (bool)
+        Specifies whether Kubernetes API endpoint is a private IP only accessible from within the VCN. Default `false` for Rancher v2.5.10 and above (bool)
         """
         return pulumi.get(self, "enable_private_control_plane")
 
     @property
     @pulumi.getter(name="enablePrivateNodes")
     def enable_private_nodes(self) -> Optional[bool]:
         """
@@ -6693,15 +6760,15 @@
         """
         return pulumi.get(self, "flex_ocpus")
 
     @property
     @pulumi.getter(name="kmsKeyId")
     def kms_key_id(self) -> Optional[str]:
         """
-        The OCID of a KMS vault master key used to encrypt secrets at rest. See [here](https://docs.oracle.com/en-us/iaas/Content/ContEng/Tasks/contengencryptingdata.htm) for help creating a vault and master encryption key. Just for Rancher v2.5.9 or above (string)
+        The OCID of a KMS vault master key used to encrypt secrets at rest. See [here](https://docs.oracle.com/en-us/iaas/Content/ContEng/Tasks/contengencryptingdata.htm) for help creating a vault and master encryption key. For Rancher v2.5.9 and above (string)
         """
         return pulumi.get(self, "kms_key_id")
 
     @property
     @pulumi.getter(name="limitNodeCount")
     def limit_node_count(self) -> Optional[int]:
         """
@@ -7029,15 +7096,15 @@
         :param int addon_job_timeout: Duration in seconds of addon job (int)
         :param str addons: Addons descripton to deploy on RKE cluster.
         :param Sequence[str] addons_includes: Addons yaml manifests to deploy on RKE cluster (list)
         :param 'ClusterRkeConfigAuthenticationArgs' authentication: Kubernetes cluster authentication (list maxitems:1)
         :param 'ClusterRkeConfigAuthorizationArgs' authorization: Kubernetes cluster authorization (list maxitems:1)
         :param 'ClusterRkeConfigBastionHostArgs' bastion_host: RKE bastion host (list maxitems:1)
         :param 'ClusterRkeConfigCloudProviderArgs' cloud_provider: RKE cloud provider [rke-cloud-providers](https://rancher.com/docs/rke/v0.1.x/en/config-options/cloud-providers/) (list maxitems:1)
-        :param 'ClusterRkeConfigDnsArgs' dns: RKE dns add-on. Just for Rancher v2.2.x (list maxitems:1)
+        :param 'ClusterRkeConfigDnsArgs' dns: RKE dns add-on. For Rancher v2.2.x (list maxitems:1)
         :param bool enable_cri_dockerd: Enable/disable using cri-dockerd. Deafult: `false` [enable_cri_dockerd](https://rancher.com/docs/rke/latest/en/config-options/#cri-dockerd) (bool)
         :param bool ignore_docker_version: Ignore docker version. Default `true` (bool)
         :param 'ClusterRkeConfigIngressArgs' ingress: Kubernetes ingress configuration (list maxitems:1)
         :param str kubernetes_version: K8s version to deploy. Default: `Rancher default` (string) (Note - if rke_config is set at cluster_template, kubernetes_version must be set to the active cluster version so Rancher can clone the RKE template)
         :param 'ClusterRkeConfigMonitoringArgs' monitoring: Kubernetes cluster monitoring (list maxitems:1)
         :param 'ClusterRkeConfigNetworkArgs' network: Kubernetes cluster networking (list maxitems:1)
         :param Sequence['ClusterRkeConfigNodeArgs'] nodes: RKE cluster nodes (list)
@@ -7153,15 +7220,15 @@
         """
         return pulumi.get(self, "cloud_provider")
 
     @property
     @pulumi.getter
     def dns(self) -> Optional['outputs.ClusterRkeConfigDns']:
         """
-        RKE dns add-on. Just for Rancher v2.2.x (list maxitems:1)
+        RKE dns add-on. For Rancher v2.2.x (list maxitems:1)
         """
         return pulumi.get(self, "dns")
 
     @property
     @pulumi.getter(name="enableCriDockerd")
     def enable_cri_dockerd(self) -> Optional[bool]:
         """
@@ -9552,17 +9619,17 @@
                  key: str,
                  effect: Optional[str] = None,
                  operator: Optional[str] = None,
                  seconds: Optional[int] = None,
                  value: Optional[str] = None):
         """
         :param str key: The toleration key (string)
-        :param str effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
-        :param str operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
-        :param int seconds: The toleration seconds (int)
+        :param str effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param str operator: The toleration operator (string)
+        :param int seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param str value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -9579,31 +9646,31 @@
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[str]:
         """
-        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[str]:
         """
-        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[int]:
         """
-        The toleration seconds (int)
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
         """
         return pulumi.get(self, "seconds")
 
     @property
     @pulumi.getter
     def value(self) -> Optional[str]:
         """
@@ -9886,17 +9953,17 @@
                  key: str,
                  effect: Optional[str] = None,
                  operator: Optional[str] = None,
                  seconds: Optional[int] = None,
                  value: Optional[str] = None):
         """
         :param str key: The toleration key (string)
-        :param str effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
-        :param str operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
-        :param int seconds: The toleration seconds (int)
+        :param str effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param str operator: The toleration operator (string)
+        :param int seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param str value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -9913,31 +9980,31 @@
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[str]:
         """
-        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[str]:
         """
-        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[int]:
         """
-        The toleration seconds (int)
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
         """
         return pulumi.get(self, "seconds")
 
     @property
     @pulumi.getter
     def value(self) -> Optional[str]:
         """
@@ -10134,17 +10201,17 @@
                  key: str,
                  effect: Optional[str] = None,
                  operator: Optional[str] = None,
                  seconds: Optional[int] = None,
                  value: Optional[str] = None):
         """
         :param str key: The toleration key (string)
-        :param str effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
-        :param str operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
-        :param int seconds: The toleration seconds (int)
+        :param str effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param str operator: The toleration operator (string)
+        :param int seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param str value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -10161,31 +10228,31 @@
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[str]:
         """
-        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[str]:
         """
-        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[int]:
         """
-        The toleration seconds (int)
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
         """
         return pulumi.get(self, "seconds")
 
     @property
     @pulumi.getter
     def value(self) -> Optional[str]:
         """
@@ -11540,17 +11607,17 @@
                  key: str,
                  effect: Optional[str] = None,
                  operator: Optional[str] = None,
                  seconds: Optional[int] = None,
                  value: Optional[str] = None):
         """
         :param str key: The toleration key (string)
-        :param str effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
-        :param str operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
-        :param int seconds: The toleration seconds (int)
+        :param str effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param str operator: The toleration operator (string)
+        :param int seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param str value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -11567,31 +11634,31 @@
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[str]:
         """
-        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[str]:
         """
-        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[int]:
         """
-        The toleration seconds (int)
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
         """
         return pulumi.get(self, "seconds")
 
     @property
     @pulumi.getter
     def value(self) -> Optional[str]:
         """
@@ -12084,29 +12151,29 @@
                  image: Optional[str] = None,
                  key: Optional[str] = None,
                  path: Optional[str] = None,
                  retention: Optional[str] = None,
                  snapshot: Optional[bool] = None,
                  uid: Optional[int] = None):
         """
-        :param 'ClusterRkeConfigServicesEtcdBackupConfigArgs' backup_config: Backup options for etcd service. Just for Rancher v2.2.x (list maxitems:1)
+        :param 'ClusterRkeConfigServicesEtcdBackupConfigArgs' backup_config: Backup options for etcd service. For Rancher v2.2.x (list maxitems:1)
         :param str ca_cert: TLS CA certificate for etcd service (string)
         :param str cert: TLS certificate for etcd service (string)
         :param str creation: Creation option for etcd service (string)
         :param Sequence[str] external_urls: External urls for etcd service (list)
         :param Mapping[str, Any] extra_args: Extra arguments for RKE Ingress (map)
         :param Sequence[str] extra_binds: Extra binds for etcd service (list)
         :param Sequence[str] extra_envs: Extra environment for etcd service (list)
-        :param int gid: Etcd service GID. Default: `0`. For Rancher v2.3.x or above (int)
+        :param int gid: Etcd service GID. Default: `0`. For Rancher v2.3.x and above (int)
         :param str image: Docker image for etcd service (string)
         :param str key: The toleration key (string)
         :param str path: Path for etcd service (string)
         :param str retention: Retention option for etcd service (string)
         :param bool snapshot: Snapshot option for etcd service (bool)
-        :param int uid: Etcd service UID. Default: `0`. For Rancher v2.3.x or above (int)
+        :param int uid: Etcd service UID. Default: `0`. For Rancher v2.3.x and above (int)
         """
         if backup_config is not None:
             pulumi.set(__self__, "backup_config", backup_config)
         if ca_cert is not None:
             pulumi.set(__self__, "ca_cert", ca_cert)
         if cert is not None:
             pulumi.set(__self__, "cert", cert)
@@ -12135,15 +12202,15 @@
         if uid is not None:
             pulumi.set(__self__, "uid", uid)
 
     @property
     @pulumi.getter(name="backupConfig")
     def backup_config(self) -> Optional['outputs.ClusterRkeConfigServicesEtcdBackupConfig']:
         """
-        Backup options for etcd service. Just for Rancher v2.2.x (list maxitems:1)
+        Backup options for etcd service. For Rancher v2.2.x (list maxitems:1)
         """
         return pulumi.get(self, "backup_config")
 
     @property
     @pulumi.getter(name="caCert")
     def ca_cert(self) -> Optional[str]:
         """
@@ -12199,15 +12266,15 @@
         """
         return pulumi.get(self, "extra_envs")
 
     @property
     @pulumi.getter
     def gid(self) -> Optional[int]:
         """
-        Etcd service GID. Default: `0`. For Rancher v2.3.x or above (int)
+        Etcd service GID. Default: `0`. For Rancher v2.3.x and above (int)
         """
         return pulumi.get(self, "gid")
 
     @property
     @pulumi.getter
     def image(self) -> Optional[str]:
         """
@@ -12247,15 +12314,15 @@
         """
         return pulumi.get(self, "snapshot")
 
     @property
     @pulumi.getter
     def uid(self) -> Optional[int]:
         """
-        Etcd service UID. Default: `0`. For Rancher v2.3.x or above (int)
+        Etcd service UID. Default: `0`. For Rancher v2.3.x and above (int)
         """
         return pulumi.get(self, "uid")
 
 
 @pulumi.output_type
 class ClusterRkeConfigServicesEtcdBackupConfig(dict):
     @staticmethod
@@ -12288,15 +12355,15 @@
                  timeout: Optional[int] = None):
         """
         :param bool enabled: Enable etcd backup (bool)
         :param int interval_hours: Interval hours for etcd backup. Default `12` (int)
         :param int retention: Retention option for etcd service (string)
         :param 'ClusterRkeConfigServicesEtcdBackupConfigS3BackupConfigArgs' s3_backup_config: S3 config options for etcd backup (list maxitems:1)
         :param bool safe_timestamp: Safe timestamp for etcd backup. Default: `false` (bool)
-        :param int timeout: Timeout in seconds for etcd backup. Default: `300`. Just for Rancher v2.5.6 and above (int)
+        :param int timeout: Timeout in seconds for etcd backup. Default: `300`. For Rancher v2.5.6 and above (int)
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if interval_hours is not None:
             pulumi.set(__self__, "interval_hours", interval_hours)
         if retention is not None:
             pulumi.set(__self__, "retention", retention)
@@ -12347,15 +12414,15 @@
         """
         return pulumi.get(self, "safe_timestamp")
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[int]:
         """
-        Timeout in seconds for etcd backup. Default: `300`. Just for Rancher v2.5.6 and above (int)
+        Timeout in seconds for etcd backup. Default: `300`. For Rancher v2.5.6 and above (int)
         """
         return pulumi.get(self, "timeout")
 
 
 @pulumi.output_type
 class ClusterRkeConfigServicesEtcdBackupConfigS3BackupConfig(dict):
     @staticmethod
@@ -12720,26 +12787,14 @@
 class ClusterRkeConfigServicesKubeApiAdmissionConfigurationPlugin(dict):
     def __init__(__self__, *,
                  configuration: Optional[str] = None,
                  name: Optional[str] = None,
                  path: Optional[str] = None):
         """
         :param str configuration: Plugin configuration. (string) Ex:
-               
-               ```python
-               import pulumi
-               ```
-               configuration = <<EOF
-               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
-               kind: Configuration
-               limits:
-               - type: Server
-               burst: 35000
-               qps: 6000
-               EOF
         :param str name: The name of the Cluster (string)
         :param str path: Path for etcd service (string)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -12747,26 +12802,14 @@
             pulumi.set(__self__, "path", path)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[str]:
         """
         Plugin configuration. (string) Ex:
-
-        ```python
-        import pulumi
-        ```
-        configuration = <<EOF
-        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
-        kind: Configuration
-        limits:
-        - type: Server
-        burst: 35000
-        qps: 6000
-        EOF
         """
         return pulumi.get(self, "configuration")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
@@ -12786,50 +12829,26 @@
 @pulumi.output_type
 class ClusterRkeConfigServicesKubeApiAuditLog(dict):
     def __init__(__self__, *,
                  configuration: Optional['outputs.ClusterRkeConfigServicesKubeApiAuditLogConfiguration'] = None,
                  enabled: Optional[bool] = None):
         """
         :param 'ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs' configuration: Plugin configuration. (string) Ex:
-               
-               ```python
-               import pulumi
-               ```
-               configuration = <<EOF
-               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
-               kind: Configuration
-               limits:
-               - type: Server
-               burst: 35000
-               qps: 6000
-               EOF
         :param bool enabled: Enable etcd backup (bool)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional['outputs.ClusterRkeConfigServicesKubeApiAuditLogConfiguration']:
         """
         Plugin configuration. (string) Ex:
-
-        ```python
-        import pulumi
-        ```
-        configuration = <<EOF
-        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
-        kind: Configuration
-        limits:
-        - type: Server
-        burst: 35000
-        qps: 6000
-        EOF
         """
         return pulumi.get(self, "configuration")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         """
@@ -12941,50 +12960,26 @@
 @pulumi.output_type
 class ClusterRkeConfigServicesKubeApiEventRateLimit(dict):
     def __init__(__self__, *,
                  configuration: Optional[str] = None,
                  enabled: Optional[bool] = None):
         """
         :param str configuration: Plugin configuration. (string) Ex:
-               
-               ```python
-               import pulumi
-               ```
-               configuration = <<EOF
-               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
-               kind: Configuration
-               limits:
-               - type: Server
-               burst: 35000
-               qps: 6000
-               EOF
         :param bool enabled: Enable etcd backup (bool)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[str]:
         """
         Plugin configuration. (string) Ex:
-
-        ```python
-        import pulumi
-        ```
-        configuration = <<EOF
-        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
-        kind: Configuration
-        limits:
-        - type: Server
-        burst: 35000
-        qps: 6000
-        EOF
         """
         return pulumi.get(self, "configuration")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         """
@@ -13557,15 +13552,15 @@
                  ignore_daemon_sets: Optional[bool] = None,
                  timeout: Optional[int] = None):
         """
         :param bool delete_local_data: Delete RKE node local data. Default: `false` (bool)
         :param bool force: Force RKE node drain. Default: `false` (bool)
         :param int grace_period: RKE node drain grace period. Default: `-1` (int)
         :param bool ignore_daemon_sets: Ignore RKE daemon sets. Default: `true` (bool)
-        :param int timeout: Timeout in seconds for etcd backup. Default: `300`. Just for Rancher v2.5.6 and above (int)
+        :param int timeout: Timeout in seconds for etcd backup. Default: `300`. For Rancher v2.5.6 and above (int)
         """
         if delete_local_data is not None:
             pulumi.set(__self__, "delete_local_data", delete_local_data)
         if force is not None:
             pulumi.set(__self__, "force", force)
         if grace_period is not None:
             pulumi.set(__self__, "grace_period", grace_period)
@@ -13606,15 +13601,15 @@
         """
         return pulumi.get(self, "ignore_daemon_sets")
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[int]:
         """
-        Timeout in seconds for etcd backup. Default: `300`. Just for Rancher v2.5.6 and above (int)
+        Timeout in seconds for etcd backup. Default: `300`. For Rancher v2.5.6 and above (int)
         """
         return pulumi.get(self, "timeout")
 
 
 @pulumi.output_type
 class ClusterSyncNode(dict):
     @staticmethod
@@ -19252,49 +19247,64 @@
         ClusterV2ClusterAgentDeploymentCustomization.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  append_tolerations: Optional[Sequence['outputs.ClusterV2ClusterAgentDeploymentCustomizationAppendToleration']] = None,
                  override_affinity: Optional[str] = None,
                  override_resource_requirements: Optional[Sequence['outputs.ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirement']] = None):
+        """
+        :param Sequence['ClusterV2ClusterAgentDeploymentCustomizationAppendTolerationArgs'] append_tolerations: User defined tolerations to append to agent (list)
+        :param str override_affinity: User defined affinity to override default agent affinity (string)
+        :param Sequence['ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs'] override_resource_requirements: User defined resource requirements to set on the agent (list)
+        """
         if append_tolerations is not None:
             pulumi.set(__self__, "append_tolerations", append_tolerations)
         if override_affinity is not None:
             pulumi.set(__self__, "override_affinity", override_affinity)
         if override_resource_requirements is not None:
             pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
 
     @property
     @pulumi.getter(name="appendTolerations")
     def append_tolerations(self) -> Optional[Sequence['outputs.ClusterV2ClusterAgentDeploymentCustomizationAppendToleration']]:
+        """
+        User defined tolerations to append to agent (list)
+        """
         return pulumi.get(self, "append_tolerations")
 
     @property
     @pulumi.getter(name="overrideAffinity")
     def override_affinity(self) -> Optional[str]:
+        """
+        User defined affinity to override default agent affinity (string)
+        """
         return pulumi.get(self, "override_affinity")
 
     @property
     @pulumi.getter(name="overrideResourceRequirements")
     def override_resource_requirements(self) -> Optional[Sequence['outputs.ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirement']]:
+        """
+        User defined resource requirements to set on the agent (list)
+        """
         return pulumi.get(self, "override_resource_requirements")
 
 
 @pulumi.output_type
 class ClusterV2ClusterAgentDeploymentCustomizationAppendToleration(dict):
     def __init__(__self__, *,
                  key: str,
                  effect: Optional[str] = None,
                  operator: Optional[str] = None,
                  seconds: Optional[int] = None,
                  value: Optional[str] = None):
         """
-        :param str key: The taint key (string)
-        :param str effect: The taint effect. Default: `\\"NoExecute\\"` (string)
-        :param str operator: Machine selector label match expressions operator (string)
+        :param str key: The toleration key (string)
+        :param str effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param str operator: The toleration operator (string)
+        :param int seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param str value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -19303,37 +19313,40 @@
         if value is not None:
             pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def key(self) -> str:
         """
-        The taint key (string)
+        The toleration key (string)
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[str]:
         """
-        The taint effect. Default: `\\"NoExecute\\"` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[str]:
         """
-        Machine selector label match expressions operator (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[int]:
+        """
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
+        """
         return pulumi.get(self, "seconds")
 
     @property
     @pulumi.getter
     def value(self) -> Optional[str]:
         """
         Rancher agent env var value (string)
@@ -19367,41 +19380,59 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  cpu_limit: Optional[str] = None,
                  cpu_request: Optional[str] = None,
                  memory_limit: Optional[str] = None,
                  memory_request: Optional[str] = None):
+        """
+        :param str cpu_limit: The maximum CPU limit for agent (string)
+        :param str cpu_request: The minimum CPU required for agent (string)
+        :param str memory_limit: The maximum memory limit for agent (string)
+        :param str memory_request: The minimum memory required for agent (string)
+        """
         if cpu_limit is not None:
             pulumi.set(__self__, "cpu_limit", cpu_limit)
         if cpu_request is not None:
             pulumi.set(__self__, "cpu_request", cpu_request)
         if memory_limit is not None:
             pulumi.set(__self__, "memory_limit", memory_limit)
         if memory_request is not None:
             pulumi.set(__self__, "memory_request", memory_request)
 
     @property
     @pulumi.getter(name="cpuLimit")
     def cpu_limit(self) -> Optional[str]:
+        """
+        The maximum CPU limit for agent (string)
+        """
         return pulumi.get(self, "cpu_limit")
 
     @property
     @pulumi.getter(name="cpuRequest")
     def cpu_request(self) -> Optional[str]:
+        """
+        The minimum CPU required for agent (string)
+        """
         return pulumi.get(self, "cpu_request")
 
     @property
     @pulumi.getter(name="memoryLimit")
     def memory_limit(self) -> Optional[str]:
+        """
+        The maximum memory limit for agent (string)
+        """
         return pulumi.get(self, "memory_limit")
 
     @property
     @pulumi.getter(name="memoryRequest")
     def memory_request(self) -> Optional[str]:
+        """
+        The minimum memory required for agent (string)
+        """
         return pulumi.get(self, "memory_request")
 
 
 @pulumi.output_type
 class ClusterV2ClusterRegistrationToken(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -19616,49 +19647,64 @@
         ClusterV2FleetAgentDeploymentCustomization.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  append_tolerations: Optional[Sequence['outputs.ClusterV2FleetAgentDeploymentCustomizationAppendToleration']] = None,
                  override_affinity: Optional[str] = None,
                  override_resource_requirements: Optional[Sequence['outputs.ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirement']] = None):
+        """
+        :param Sequence['ClusterV2FleetAgentDeploymentCustomizationAppendTolerationArgs'] append_tolerations: User defined tolerations to append to agent (list)
+        :param str override_affinity: User defined affinity to override default agent affinity (string)
+        :param Sequence['ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirementArgs'] override_resource_requirements: User defined resource requirements to set on the agent (list)
+        """
         if append_tolerations is not None:
             pulumi.set(__self__, "append_tolerations", append_tolerations)
         if override_affinity is not None:
             pulumi.set(__self__, "override_affinity", override_affinity)
         if override_resource_requirements is not None:
             pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
 
     @property
     @pulumi.getter(name="appendTolerations")
     def append_tolerations(self) -> Optional[Sequence['outputs.ClusterV2FleetAgentDeploymentCustomizationAppendToleration']]:
+        """
+        User defined tolerations to append to agent (list)
+        """
         return pulumi.get(self, "append_tolerations")
 
     @property
     @pulumi.getter(name="overrideAffinity")
     def override_affinity(self) -> Optional[str]:
+        """
+        User defined affinity to override default agent affinity (string)
+        """
         return pulumi.get(self, "override_affinity")
 
     @property
     @pulumi.getter(name="overrideResourceRequirements")
     def override_resource_requirements(self) -> Optional[Sequence['outputs.ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirement']]:
+        """
+        User defined resource requirements to set on the agent (list)
+        """
         return pulumi.get(self, "override_resource_requirements")
 
 
 @pulumi.output_type
 class ClusterV2FleetAgentDeploymentCustomizationAppendToleration(dict):
     def __init__(__self__, *,
                  key: str,
                  effect: Optional[str] = None,
                  operator: Optional[str] = None,
                  seconds: Optional[int] = None,
                  value: Optional[str] = None):
         """
-        :param str key: The taint key (string)
-        :param str effect: The taint effect. Default: `\\"NoExecute\\"` (string)
-        :param str operator: Machine selector label match expressions operator (string)
+        :param str key: The toleration key (string)
+        :param str effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
+        :param str operator: The toleration operator (string)
+        :param int seconds: The number of seconds a pod will stay bound to a node with a matching taint (int)
         :param str value: Rancher agent env var value (string)
         """
         pulumi.set(__self__, "key", key)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
@@ -19667,37 +19713,40 @@
         if value is not None:
             pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def key(self) -> str:
         """
-        The taint key (string)
+        The toleration key (string)
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[str]:
         """
-        The taint effect. Default: `\\"NoExecute\\"` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[str]:
         """
-        Machine selector label match expressions operator (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def seconds(self) -> Optional[int]:
+        """
+        The number of seconds a pod will stay bound to a node with a matching taint (int)
+        """
         return pulumi.get(self, "seconds")
 
     @property
     @pulumi.getter
     def value(self) -> Optional[str]:
         """
         Rancher agent env var value (string)
@@ -19731,41 +19780,59 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  cpu_limit: Optional[str] = None,
                  cpu_request: Optional[str] = None,
                  memory_limit: Optional[str] = None,
                  memory_request: Optional[str] = None):
+        """
+        :param str cpu_limit: The maximum CPU limit for agent (string)
+        :param str cpu_request: The minimum CPU required for agent (string)
+        :param str memory_limit: The maximum memory limit for agent (string)
+        :param str memory_request: The minimum memory required for agent (string)
+        """
         if cpu_limit is not None:
             pulumi.set(__self__, "cpu_limit", cpu_limit)
         if cpu_request is not None:
             pulumi.set(__self__, "cpu_request", cpu_request)
         if memory_limit is not None:
             pulumi.set(__self__, "memory_limit", memory_limit)
         if memory_request is not None:
             pulumi.set(__self__, "memory_request", memory_request)
 
     @property
     @pulumi.getter(name="cpuLimit")
     def cpu_limit(self) -> Optional[str]:
+        """
+        The maximum CPU limit for agent (string)
+        """
         return pulumi.get(self, "cpu_limit")
 
     @property
     @pulumi.getter(name="cpuRequest")
     def cpu_request(self) -> Optional[str]:
+        """
+        The minimum CPU required for agent (string)
+        """
         return pulumi.get(self, "cpu_request")
 
     @property
     @pulumi.getter(name="memoryLimit")
     def memory_limit(self) -> Optional[str]:
+        """
+        The maximum memory limit for agent (string)
+        """
         return pulumi.get(self, "memory_limit")
 
     @property
     @pulumi.getter(name="memoryRequest")
     def memory_request(self) -> Optional[str]:
+        """
+        The minimum memory required for agent (string)
+        """
         return pulumi.get(self, "memory_request")
 
 
 @pulumi.output_type
 class ClusterV2LocalAuthEndpoint(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -19961,14 +20028,17 @@
 
     @property
     @pulumi.getter(name="localAuthEndpoint")
     def local_auth_endpoint(self) -> Optional['outputs.ClusterV2RkeConfigLocalAuthEndpoint']:
         """
         Cluster V2 local auth endpoint (list maxitems:1)
         """
+        warnings.warn("""Use rancher2_cluster_v2.local_auth_endpoint instead""", DeprecationWarning)
+        pulumi.log.warn("""local_auth_endpoint is deprecated: Use rancher2_cluster_v2.local_auth_endpoint instead""")
+
         return pulumi.get(self, "local_auth_endpoint")
 
     @property
     @pulumi.getter(name="machineGlobalConfig")
     def machine_global_config(self) -> Optional[str]:
         """
         Cluster V2 machine global config. Must be in YAML format (string)
@@ -20741,28 +20811,28 @@
 @pulumi.output_type
 class ClusterV2RkeConfigMachinePoolTaint(dict):
     def __init__(__self__, *,
                  key: str,
                  value: str,
                  effect: Optional[str] = None):
         """
-        :param str key: The taint key (string)
+        :param str key: The toleration key (string)
         :param str value: Rancher agent env var value (string)
-        :param str effect: The taint effect. Default: `\\"NoExecute\\"` (string)
+        :param str effect: The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "value", value)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
 
     @property
     @pulumi.getter
     def key(self) -> str:
         """
-        The taint key (string)
+        The toleration key (string)
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def value(self) -> str:
         """
@@ -20770,15 +20840,15 @@
         """
         return pulumi.get(self, "value")
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[str]:
         """
-        The taint effect. Default: `\\"NoExecute\\"` (string)
+        The toleration effect. Default: `\\"NoSchedule\\"` (string)
         """
         return pulumi.get(self, "effect")
 
 
 @pulumi.output_type
 class ClusterV2RkeConfigMachineSelectorConfig(dict):
     @staticmethod
@@ -20880,38 +20950,38 @@
 @pulumi.output_type
 class ClusterV2RkeConfigMachineSelectorConfigMachineLabelSelectorMatchExpression(dict):
     def __init__(__self__, *,
                  key: Optional[str] = None,
                  operator: Optional[str] = None,
                  values: Optional[Sequence[str]] = None):
         """
-        :param str key: The taint key (string)
-        :param str operator: Machine selector label match expressions operator (string)
+        :param str key: The toleration key (string)
+        :param str operator: The toleration operator (string)
         :param Sequence[str] values: Machine selector label match expressions values (List string)
         """
         if key is not None:
             pulumi.set(__self__, "key", key)
         if operator is not None:
             pulumi.set(__self__, "operator", operator)
         if values is not None:
             pulumi.set(__self__, "values", values)
 
     @property
     @pulumi.getter
     def key(self) -> Optional[str]:
         """
-        The taint key (string)
+        The toleration key (string)
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def operator(self) -> Optional[str]:
         """
-        Machine selector label match expressions operator (string)
+        The toleration operator (string)
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def values(self) -> Optional[Sequence[str]]:
         """
@@ -22559,22 +22629,22 @@
                  vnet: Optional[str] = None):
         """
         :param str availability_set: Azure Availability Set to place the virtual machine into. Default `docker-machine` (string)
         :param str availability_zone: OpenStack availability zone (string)
         :param str client_id: Azure Service Principal Account ID. Mandatory on Rancher v2.0.x and v2.1.x. Use `CloudCredential` from Rancher v2.2.x (string)
         :param str client_secret: Azure Service Principal Account password. Mandatory on Rancher v2.0.x and v2.1.x. Use `CloudCredential` from Rancher v2.2.x (string)
         :param str custom_data: Path to file with custom-data (string)
-        :param str disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        :param str disk_size: Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         :param str dns: A unique DNS label for the public IP adddress (string)
         :param str docker_port: Port number for Docker engine. Default `2376` (string)
         :param str environment: Azure environment (e.g. AzurePublicCloud, AzureChinaCloud). Default `AzurePublicCloud` (string)
         :param str fault_domain_count: Fault domain count to use for availability set. Default `3` (string)
         :param str image: Azure virtual machine OS image. Default `canonical:UbuntuServer:18.04-LTS:latest` (string)
         :param str location: Azure region to create the virtual machine. Default `westus` (string)
-        :param bool managed_disks: Configures VM and availability set for managed disks. Just for Rancher v2.3.x and above. Default `false` (bool)
+        :param bool managed_disks: Configures VM and availability set for managed disks. For Rancher v2.3.x and above. Default `false` (bool)
         :param bool no_public_ip: Do not create a public IP address for the machine. Default `false` (bool)
         :param str nsg: Azure Network Security Group to assign this node to (accepts either a name or resource ID, default is to create a new NSG for each machine). Default `docker-machine-nsg` (string)
         :param Sequence[str] open_ports: Make the specified port number accessible from the Internet. (list)
         :param bool private_address_only: Only use a private IP address. Default `false` (bool)
         :param str private_ip_address: Specify a static private IP address for the machine. (string)
         :param str resource_group: Azure Resource Group name (will be created if missing). Default `docker-machine` (string)
         :param str size: Size for Azure Virtual Machine. Default `Standard_A2` (string)
@@ -22702,15 +22772,15 @@
         """
         return pulumi.get(self, "custom_data")
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[str]:
         """
-        Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         """
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter
     def dns(self) -> Optional[str]:
         """
@@ -22758,15 +22828,15 @@
         """
         return pulumi.get(self, "location")
 
     @property
     @pulumi.getter(name="managedDisks")
     def managed_disks(self) -> Optional[bool]:
         """
-        Configures VM and availability set for managed disks. Just for Rancher v2.3.x and above. Default `false` (bool)
+        Configures VM and availability set for managed disks. For Rancher v2.3.x and above. Default `false` (bool)
         """
         return pulumi.get(self, "managed_disks")
 
     @property
     @pulumi.getter(name="noPublicIp")
     def no_public_ip(self) -> Optional[bool]:
         """
@@ -23183,24 +23253,24 @@
                  vm_affinity: Optional[str] = None):
         """
         :param str ssh_user: Set the name of the ssh user (string)
         :param str vm_namespace: Virtual machine namespace e.g. `default` (string)
         :param str cpu_count: CPU count, Default `2` (string)
         :param str disk_bus: Use `disk_info` instead
         :param str disk_info: A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
-        :param str disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        :param str disk_size: Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         :param str image_name: Use `disk_info` instead
         :param str memory_size: Memory size (in GiB), Default `4` (string)
         :param str network_data: NetworkData content of cloud-init, base64 is supported (string)
         :param str network_info: A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
         :param str network_model: Use `network_info` instead
         :param str network_name: Use `network_info` instead
         :param str ssh_password: SSH password (string)
         :param str user_data: UserData content of cloud-init, base64 is supported. If the image does not contain the qemu-guest-agent package, you must install and start qemu-guest-agent using userdata (string)
-        :param str vm_affinity: Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 or above (string)
+        :param str vm_affinity: Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 and above (string)
         """
         pulumi.set(__self__, "ssh_user", ssh_user)
         pulumi.set(__self__, "vm_namespace", vm_namespace)
         if cpu_count is not None:
             pulumi.set(__self__, "cpu_count", cpu_count)
         if disk_bus is not None:
             pulumi.set(__self__, "disk_bus", disk_bus)
@@ -23253,38 +23323,47 @@
 
     @property
     @pulumi.getter(name="diskBus")
     def disk_bus(self) -> Optional[str]:
         """
         Use `disk_info` instead
         """
+        warnings.warn("""Use disk_info instead""", DeprecationWarning)
+        pulumi.log.warn("""disk_bus is deprecated: Use disk_info instead""")
+
         return pulumi.get(self, "disk_bus")
 
     @property
     @pulumi.getter(name="diskInfo")
     def disk_info(self) -> Optional[str]:
         """
         A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
         """
         return pulumi.get(self, "disk_info")
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[str]:
         """
-        Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         """
+        warnings.warn("""Use disk_info instead""", DeprecationWarning)
+        pulumi.log.warn("""disk_size is deprecated: Use disk_info instead""")
+
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter(name="imageName")
     def image_name(self) -> Optional[str]:
         """
         Use `disk_info` instead
         """
+        warnings.warn("""Use disk_info instead""", DeprecationWarning)
+        pulumi.log.warn("""image_name is deprecated: Use disk_info instead""")
+
         return pulumi.get(self, "image_name")
 
     @property
     @pulumi.getter(name="memorySize")
     def memory_size(self) -> Optional[str]:
         """
         Memory size (in GiB), Default `4` (string)
@@ -23309,22 +23388,28 @@
 
     @property
     @pulumi.getter(name="networkModel")
     def network_model(self) -> Optional[str]:
         """
         Use `network_info` instead
         """
+        warnings.warn("""Use network_info instead""", DeprecationWarning)
+        pulumi.log.warn("""network_model is deprecated: Use network_info instead""")
+
         return pulumi.get(self, "network_model")
 
     @property
     @pulumi.getter(name="networkName")
     def network_name(self) -> Optional[str]:
         """
         Use `network_info` instead
         """
+        warnings.warn("""Use network_info instead""", DeprecationWarning)
+        pulumi.log.warn("""network_name is deprecated: Use network_info instead""")
+
         return pulumi.get(self, "network_name")
 
     @property
     @pulumi.getter(name="sshPassword")
     def ssh_password(self) -> Optional[str]:
         """
         SSH password (string)
@@ -23339,15 +23424,15 @@
         """
         return pulumi.get(self, "user_data")
 
     @property
     @pulumi.getter(name="vmAffinity")
     def vm_affinity(self) -> Optional[str]:
         """
-        Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 or above (string)
+        Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 and above (string)
         """
         return pulumi.get(self, "vm_affinity")
 
 
 @pulumi.output_type
 class MachineConfigV2LinodeConfig(dict):
     @staticmethod
@@ -23751,16 +23836,16 @@
         :param str tenant_id: Azure Tenant ID (string)
         :param str tenant_name: OpenStack tenant name. Conflicts with `tenant_id` (string)
         :param str user_data_file: File containing an openstack userdata script (string)
         :param str user_domain_id: OpenStack user domain id. Conflicts with `user_domain_name` (string)
         :param str user_domain_name: OpenStack user domain name. Conflicts with `user_domain_id` (string)
         :param str username: OpenStack username (string)
         :param str volume_device_path: OpenStack volume device path (attaching). Applicable only when `boot_from_volume` is `true`. Omit for auto `/dev/vdb`. (string)
-               > **Note**: `Required+` denotes that either the _name or _id is required but you cannot use both.
-               > **Note**: `Required++` denotes that either the _name or _id is required unless `application_credential_id` is defined.
+               > **Note:**: `Required+` denotes that either the _name or _id is required but you cannot use both.
+               > **Note:**: `Required++` denotes that either the _name or _id is required unless `application_credential_id` is defined.
         :param str volume_id: OpenStack volume id of existing volume. Applicable only when `boot_from_volume` is `true` (string)
         :param str volume_name: OpenStack volume name of existing volume. Applicable only when `boot_from_volume` is `true` (string)
         :param str volume_size: OpenStack volume size (GiB). Required when `boot_from_volume` is `true` (string)
         :param str volume_type: Amazon EBS volume type. Default `gp2` (string)
         """
         pulumi.set(__self__, "auth_url", auth_url)
         pulumi.set(__self__, "availability_zone", availability_zone)
@@ -24141,16 +24226,16 @@
         return pulumi.get(self, "username")
 
     @property
     @pulumi.getter(name="volumeDevicePath")
     def volume_device_path(self) -> Optional[str]:
         """
         OpenStack volume device path (attaching). Applicable only when `boot_from_volume` is `true`. Omit for auto `/dev/vdb`. (string)
-        > **Note**: `Required+` denotes that either the _name or _id is required but you cannot use both.
-        > **Note**: `Required++` denotes that either the _name or _id is required unless `application_credential_id` is defined.
+        > **Note:**: `Required+` denotes that either the _name or _id is required but you cannot use both.
+        > **Note:**: `Required++` denotes that either the _name or _id is required unless `application_credential_id` is defined.
         """
         return pulumi.get(self, "volume_device_path")
 
     @property
     @pulumi.getter(name="volumeId")
     def volume_id(self) -> Optional[str]:
         """
@@ -24279,15 +24364,15 @@
         :param str content_library: If you choose to clone from a content library template specify the name of the library (string)
         :param str cpu_count: CPU count, Default `2` (string)
         :param str creation_type: Creation type when creating a new virtual machine. Supported values: vm, template, library, legacy. Default `legacy` (string)
         :param Sequence[str] custom_attributes: vSphere custom attributes, format key/value e.g. `200=my custom value` (List)
         :param str datacenter: vSphere datacenter for docker VM (string)
         :param str datastore: vSphere datastore for docker VM (string)
         :param str datastore_cluster: vSphere datastore cluster for virtual machine (string)
-        :param str disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        :param str disk_size: Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         :param str folder: vSphere folder for the docker VM. This folder must already exist in the datacenter (string)
         :param str hostsystem: vSphere compute resource where the docker VM will be instantiated. This can be omitted if using a cluster with DRS (string)
         :param str memory_size: Memory size (in GiB), Default `4` (string)
         :param Sequence[str] networks: vSphere network where the docker VM will be attached (list)
         :param str password: OpenStack password. Mandatory on Rancher v2.0.x and v2.1.x. Use `CloudCredential` from Rancher v2.2.x (string)
         :param str pool: vSphere resource pool for docker VM (string)
         :param str ssh_password: SSH password (string)
@@ -24462,15 +24547,15 @@
         """
         return pulumi.get(self, "datastore_cluster")
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[str]:
         """
-        Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         """
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter
     def folder(self) -> Optional[str]:
         """
@@ -25402,15 +25487,15 @@
         :param str spot_price: AWS spot instance bid price (in dollar). Default `0.50` (string)
         :param str ssh_user: Set the name of the ssh user (string)
         :param str tags: AWS Tags (e.g. key1,value1,key2,value2) (string)
         :param bool use_ebs_optimized_instance: Create an EBS optimized instance. Default `false` (bool)
         :param bool use_private_address: Force the usage of private IP address. Default `false` (bool)
         :param str userdata: Path to file with cloud-init user data (string)
                
-               > **Note**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
+               > **Note:**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
         :param str volume_type: Amazon EBS volume type. Default `gp2` (string)
         """
         pulumi.set(__self__, "ami", ami)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "security_groups", security_groups)
         pulumi.set(__self__, "subnet_id", subnet_id)
         pulumi.set(__self__, "vpc_id", vpc_id)
@@ -25737,15 +25822,15 @@
 
     @property
     @pulumi.getter
     def userdata(self) -> Optional[str]:
         """
         Path to file with cloud-init user data (string)
 
-        > **Note**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
+        > **Note:**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
         """
         return pulumi.get(self, "userdata")
 
     @property
     @pulumi.getter(name="volumeType")
     def volume_type(self) -> Optional[str]:
         """
@@ -25850,26 +25935,26 @@
                  vnet: Optional[str] = None):
         """
         :param str availability_set: Azure Availability Set to place the virtual machine into. Default `docker-machine` (string)
         :param str availability_zone: OpenStack availability zone (string)
         :param str client_id: Azure Service Principal Account ID. Mandatory on Rancher v2.0.x and v2.1.x. Use `CloudCredential` from Rancher v2.2.x (string)
         :param str client_secret: Azure Service Principal Account password. Mandatory on Rancher v2.0.x and v2.1.x. Use `CloudCredential` from Rancher v2.2.x (string)
         :param str custom_data: Path to file with custom-data (string)
-        :param str disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        :param str disk_size: Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         :param str dns: A unique DNS label for the public IP adddress (string)
         :param str docker_port: Port number for Docker engine. Default `2376` (string)
         :param str environment: Azure environment (e.g. AzurePublicCloud, AzureChinaCloud). Default `AzurePublicCloud` (string)
         :param str fault_domain_count: Fault domain count to use for availability set. Default `3` (string)
         :param str image: Azure virtual machine OS image. Default `canonical:UbuntuServer:18.04-LTS:latest` (string)
         :param str location: Azure region to create the virtual machine. Default `westus` (string)
-        :param bool managed_disks: Configures VM and availability set for managed disks. Just for Rancher v2.3.x and above. Default `false` (bool)
+        :param bool managed_disks: Configures VM and availability set for managed disks. For Rancher v2.3.x and above. Default `false` (bool)
         :param bool no_public_ip: Do not create a public IP address for the machine. Default `false` (bool)
         :param str nsg: Azure Network Security Group to assign this node to (accepts either a name or resource ID, default is to create a new NSG for each machine). Default `docker-machine-nsg` (string)
         :param Sequence[str] open_ports: Make the specified port number accessible from the Internet. (list)
-        :param str plan: Azure marketplace purchase plan for Azure Virtual Machine. Format is `<publisher>:<product>:<plan>`. Just for Rancher v2.6.3 and above. (string)
+        :param str plan: Azure marketplace purchase plan for Azure Virtual Machine. Format is `<publisher>:<product>:<plan>`. For Rancher v2.6.3 and above. (string)
         :param str private_ip_address: Specify a static private IP address for the machine. (string)
         :param str resource_group: Azure Resource Group name (will be created if missing). Default `docker-machine` (string)
         :param str size: Size for Azure Virtual Machine. Default `Standard_A2` (string)
         :param str ssh_user: Set the name of the ssh user (string)
         :param bool static_public_ip: Assign a static public IP address to the machine. Default `false` (bool)
         :param str storage_type: Type of Storage Account to host the OS Disk for the machine. Default `Standard_LRS` (string)
         :param str subnet: Azure Subnet Name to be used within the Virtual Network. Default `docker-machine` (string)
@@ -25990,15 +26075,15 @@
         """
         return pulumi.get(self, "custom_data")
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[str]:
         """
-        Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         """
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter
     def dns(self) -> Optional[str]:
         """
@@ -26046,15 +26131,15 @@
         """
         return pulumi.get(self, "location")
 
     @property
     @pulumi.getter(name="managedDisks")
     def managed_disks(self) -> Optional[bool]:
         """
-        Configures VM and availability set for managed disks. Just for Rancher v2.3.x and above. Default `false` (bool)
+        Configures VM and availability set for managed disks. For Rancher v2.3.x and above. Default `false` (bool)
         """
         return pulumi.get(self, "managed_disks")
 
     @property
     @pulumi.getter(name="noPublicIp")
     def no_public_ip(self) -> Optional[bool]:
         """
@@ -26078,15 +26163,15 @@
         """
         return pulumi.get(self, "open_ports")
 
     @property
     @pulumi.getter
     def plan(self) -> Optional[str]:
         """
-        Azure marketplace purchase plan for Azure Virtual Machine. Format is `<publisher>:<product>:<plan>`. Just for Rancher v2.6.3 and above. (string)
+        Azure marketplace purchase plan for Azure Virtual Machine. Format is `<publisher>:<product>:<plan>`. For Rancher v2.6.3 and above. (string)
         """
         return pulumi.get(self, "plan")
 
     @property
     @pulumi.getter(name="privateIpAddress")
     def private_ip_address(self) -> Optional[str]:
         """
@@ -26252,15 +26337,15 @@
         :param str ssh_key_fingerprint: SSH key fingerprint (string)
         :param str ssh_key_path: SSH private key path (string)
         :param str ssh_port: SSH port. Default `22` (string)
         :param str ssh_user: Set the name of the ssh user (string)
         :param str tags: AWS Tags (e.g. key1,value1,key2,value2) (string)
         :param str userdata: Path to file with cloud-init user data (string)
                
-               > **Note**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
+               > **Note:**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
         """
         if access_token is not None:
             pulumi.set(__self__, "access_token", access_token)
         if backups is not None:
             pulumi.set(__self__, "backups", backups)
         if image is not None:
             pulumi.set(__self__, "image", image)
@@ -26393,15 +26478,15 @@
 
     @property
     @pulumi.getter
     def userdata(self) -> Optional[str]:
         """
         Path to file with cloud-init user data (string)
 
-        > **Note**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
+        > **Note:**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
         """
         return pulumi.get(self, "userdata")
 
 
 @pulumi.output_type
 class NodeTemplateHarvesterConfig(dict):
     @staticmethod
@@ -26467,24 +26552,24 @@
                  vm_affinity: Optional[str] = None):
         """
         :param str ssh_user: Set the name of the ssh user (string)
         :param str vm_namespace: Virtual machine namespace e.g. `default` (string)
         :param str cpu_count: CPU count, Default `2` (string)
         :param str disk_bus: Use `disk_info` instead
         :param str disk_info: A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
-        :param str disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        :param str disk_size: Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         :param str image_name: Use `disk_info` instead
         :param str memory_size: Memory size (in GiB), Default `4` (string)
         :param str network_data: NetworkData content of cloud-init, base64 is supported (string)
         :param str network_info: A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
         :param str network_model: Use `network_info` instead
         :param str network_name: Use `network_info` instead
         :param str ssh_password: SSH password (string)
         :param str user_data: UserData content of cloud-init, base64 is supported. If the image does not contain the qemu-guest-agent package, you must install and start qemu-guest-agent using userdata (string)
-        :param str vm_affinity: Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 or above (string)
+        :param str vm_affinity: Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 and above (string)
         """
         pulumi.set(__self__, "ssh_user", ssh_user)
         pulumi.set(__self__, "vm_namespace", vm_namespace)
         if cpu_count is not None:
             pulumi.set(__self__, "cpu_count", cpu_count)
         if disk_bus is not None:
             pulumi.set(__self__, "disk_bus", disk_bus)
@@ -26537,38 +26622,47 @@
 
     @property
     @pulumi.getter(name="diskBus")
     def disk_bus(self) -> Optional[str]:
         """
         Use `disk_info` instead
         """
+        warnings.warn("""Use disk_info instead""", DeprecationWarning)
+        pulumi.log.warn("""disk_bus is deprecated: Use disk_info instead""")
+
         return pulumi.get(self, "disk_bus")
 
     @property
     @pulumi.getter(name="diskInfo")
     def disk_info(self) -> Optional[str]:
         """
         A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
         """
         return pulumi.get(self, "disk_info")
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[str]:
         """
-        Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         """
+        warnings.warn("""Use disk_info instead""", DeprecationWarning)
+        pulumi.log.warn("""disk_size is deprecated: Use disk_info instead""")
+
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter(name="imageName")
     def image_name(self) -> Optional[str]:
         """
         Use `disk_info` instead
         """
+        warnings.warn("""Use disk_info instead""", DeprecationWarning)
+        pulumi.log.warn("""image_name is deprecated: Use disk_info instead""")
+
         return pulumi.get(self, "image_name")
 
     @property
     @pulumi.getter(name="memorySize")
     def memory_size(self) -> Optional[str]:
         """
         Memory size (in GiB), Default `4` (string)
@@ -26593,22 +26687,28 @@
 
     @property
     @pulumi.getter(name="networkModel")
     def network_model(self) -> Optional[str]:
         """
         Use `network_info` instead
         """
+        warnings.warn("""Use network_info instead""", DeprecationWarning)
+        pulumi.log.warn("""network_model is deprecated: Use network_info instead""")
+
         return pulumi.get(self, "network_model")
 
     @property
     @pulumi.getter(name="networkName")
     def network_name(self) -> Optional[str]:
         """
         Use `network_info` instead
         """
+        warnings.warn("""Use network_info instead""", DeprecationWarning)
+        pulumi.log.warn("""network_name is deprecated: Use network_info instead""")
+
         return pulumi.get(self, "network_name")
 
     @property
     @pulumi.getter(name="sshPassword")
     def ssh_password(self) -> Optional[str]:
         """
         SSH password (string)
@@ -26623,15 +26723,15 @@
         """
         return pulumi.get(self, "user_data")
 
     @property
     @pulumi.getter(name="vmAffinity")
     def vm_affinity(self) -> Optional[str]:
         """
-        Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 or above (string)
+        Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 and above (string)
         """
         return pulumi.get(self, "vm_affinity")
 
 
 @pulumi.output_type
 class NodeTemplateHetznerConfig(dict):
     @staticmethod
@@ -26675,15 +26775,15 @@
         :param str networks: Comma-separated list of network IDs or names which should be attached to the server private network interface (string)
         :param Mapping[str, Any] server_labels: Map of the labels which will be assigned to the server. This argument is only available on [Hetzner Docker Node Driver:v3.6.0](https://github.com/JonasProgrammer/docker-machine-driver-hetzner/releases/tag/3.6.0) and above (map)
         :param str server_location: Hetzner Cloud datacenter. Default `nbg1` (string)
         :param str server_type: Hetzner Cloud server type. Default `cx11` (string)
         :param bool use_private_network: Use private network. Default `false` (bool)
         :param str userdata: Path to file with cloud-init user data (string)
                
-               > **Note**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
+               > **Note:**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
         :param str volumes: Comma-separated list of volume IDs or names which should be attached to the server (string)
         """
         pulumi.set(__self__, "api_token", api_token)
         if image is not None:
             pulumi.set(__self__, "image", image)
         if networks is not None:
             pulumi.set(__self__, "networks", networks)
@@ -26758,15 +26858,15 @@
 
     @property
     @pulumi.getter
     def userdata(self) -> Optional[str]:
         """
         Path to file with cloud-init user data (string)
 
-        > **Note**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
+        > **Note:**: You need to install the Hetzner Docker Machine Driver first as shown as in the examples section.
         """
         return pulumi.get(self, "userdata")
 
     @property
     @pulumi.getter
     def volumes(self) -> Optional[str]:
         """
@@ -27161,15 +27261,15 @@
         :param str network_name: Use `network_info` instead
         :param str network_owner: Opennebula user ID of the Network to connect the machine to (string)
         :param str ssh_user: Set the name of the ssh user (string)
         :param str template_id: Opennebula template ID to use. Conflicts with `template_name` (string)
         :param str template_name: Name of the Opennbula template to use. Conflicts with `template_id` (string)
         :param str vcpu: VCPUs for the VM (string)
                
-               > **Note**: `Required*` denotes that one of image_name / image_id or template_name / template_id is required but you cannot combine them.
+               > **Note:**: `Required*` denotes that one of image_name / image_id or template_name / template_id is required but you cannot combine them.
         """
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "user", user)
         pulumi.set(__self__, "xml_rpc_url", xml_rpc_url)
         if b2d_size is not None:
             pulumi.set(__self__, "b2d_size", b2d_size)
         if cpu is not None:
@@ -27349,15 +27449,15 @@
 
     @property
     @pulumi.getter
     def vcpu(self) -> Optional[str]:
         """
         VCPUs for the VM (string)
 
-        > **Note**: `Required*` denotes that one of image_name / image_id or template_name / template_id is required but you cannot combine them.
+        > **Note:**: `Required*` denotes that one of image_name / image_id or template_name / template_id is required but you cannot combine them.
         """
         return pulumi.get(self, "vcpu")
 
 
 @pulumi.output_type
 class NodeTemplateOpenstackConfig(dict):
     @staticmethod
@@ -27512,17 +27612,17 @@
         :param str ssh_user: Set the name of the ssh user (string)
         :param str tenant_id: OpenStack tenant id. Conflicts with `tenant_name` (string)
         :param str tenant_name: OpenStack tenant name. Conflicts with `tenant_id` (string)
         :param str user_data_file: File containing an openstack userdata script (string)
         :param str username: OpenStack username (string)
         :param str volume_device_path: OpenStack volume device path (attaching). Applicable only when `boot_from_volume` is `true`. Omit for auto `/dev/vdb`. (string)
                
-               > **Note**: `Required*` denotes that either the _name or _id is required but you cannot use both.
+               > **Note:**: `Required*` denotes that either the _name or _id is required but you cannot use both.
                
-               > **Note**: `Required**` denotes that either the _name or _id is required unless `application_credential_id` is defined.
+               > **Note:**: `Required**` denotes that either the _name or _id is required unless `application_credential_id` is defined.
         :param str volume_id: OpenStack volume id of existing volume. Applicable only when `boot_from_volume` is `true` (string)
         :param str volume_name: OpenStack volume name of existing volume. Applicable only when `boot_from_volume` is `true` (string)
         :param str volume_size: OpenStack volume size (GiB). Required when `boot_from_volume` is `true` (string)
         :param str volume_type: Amazon EBS volume type. Default `gp2` (string)
         """
         pulumi.set(__self__, "auth_url", auth_url)
         pulumi.set(__self__, "availability_zone", availability_zone)
@@ -27864,17 +27964,17 @@
 
     @property
     @pulumi.getter(name="volumeDevicePath")
     def volume_device_path(self) -> Optional[str]:
         """
         OpenStack volume device path (attaching). Applicable only when `boot_from_volume` is `true`. Omit for auto `/dev/vdb`. (string)
 
-        > **Note**: `Required*` denotes that either the _name or _id is required but you cannot use both.
+        > **Note:**: `Required*` denotes that either the _name or _id is required but you cannot use both.
 
-        > **Note**: `Required**` denotes that either the _name or _id is required unless `application_credential_id` is defined.
+        > **Note:**: `Required**` denotes that either the _name or _id is required unless `application_credential_id` is defined.
         """
         return pulumi.get(self, "volume_device_path")
 
     @property
     @pulumi.getter(name="volumeId")
     def volume_id(self) -> Optional[str]:
         """
@@ -28175,15 +28275,15 @@
         :param str content_library: If you choose to clone from a content library template specify the name of the library. From Rancher v2.3.3 (string)
         :param str cpu_count: CPU count, Default `2` (string)
         :param str creation_type: Creation type when creating a new virtual machine. Supported values: vm, template, library, legacy. Default `legacy`. From Rancher v2.3.3 (string)
         :param Sequence[str] custom_attributes: vSphere custom attributes, format key/value e.g. `200=my custom value`. From Rancher v2.3.3 (List)
         :param str datacenter: vSphere datacenter for docker VM (string)
         :param str datastore: vSphere datastore for docker VM (string)
         :param str datastore_cluster: vSphere datastore cluster for virtual machine. From Rancher v2.3.3 (string)
-        :param str disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        :param str disk_size: Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         :param str folder: vSphere folder for the docker VM. This folder must already exist in the datacenter (string)
         :param str hostsystem: vSphere compute resource where the docker VM will be instantiated. This can be omitted if using a cluster with DRS (string)
         :param str memory_size: Memory size (in GiB), Default `4` (string)
         :param Sequence[str] networks: vSphere network where the docker VM will be attached (list)
         :param str password: Set the password for the XML-RPC API authentication (string)
         :param str pool: vSphere resource pool for docker VM (string)
         :param str ssh_password: SSH password (string)
@@ -28358,15 +28458,15 @@
         """
         return pulumi.get(self, "datastore_cluster")
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[str]:
         """
-        Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
+        Disk size if using managed disk. For Rancher v2.3.x and above. Default `30` (string)
         """
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter
     def folder(self) -> Optional[str]:
         """
@@ -30685,14 +30785,17 @@
     @pulumi.getter(name="subscriptionId")
     def subscription_id(self) -> str:
         return pulumi.get(self, "subscription_id")
 
     @property
     @pulumi.getter
     def tag(self) -> Mapping[str, Any]:
+        warnings.warn("""Use tags argument instead as []string""", DeprecationWarning)
+        pulumi.log.warn("""tag is deprecated: Use tags argument instead as []string""")
+
         return pulumi.get(self, "tag")
 
     @property
     @pulumi.getter
     def tags(self) -> Sequence[str]:
         return pulumi.get(self, "tags")
 
@@ -40657,14 +40760,17 @@
     @pulumi.getter(name="etcdSnapshotRestore")
     def etcd_snapshot_restore(self) -> Optional['outputs.GetClusterV2RkeConfigEtcdSnapshotRestoreResult']:
         return pulumi.get(self, "etcd_snapshot_restore")
 
     @property
     @pulumi.getter(name="localAuthEndpoint")
     def local_auth_endpoint(self) -> Optional['outputs.GetClusterV2RkeConfigLocalAuthEndpointResult']:
+        warnings.warn("""Use rancher2_cluster_v2.local_auth_endpoint instead""", DeprecationWarning)
+        pulumi.log.warn("""local_auth_endpoint is deprecated: Use rancher2_cluster_v2.local_auth_endpoint instead""")
+
         return pulumi.get(self, "local_auth_endpoint")
 
     @property
     @pulumi.getter(name="machineGlobalConfig")
     def machine_global_config(self) -> Optional[str]:
         return pulumi.get(self, "machine_global_config")
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/pod_security_policy_template.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/project.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/project_alert_group.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/project_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/project_alert_rule.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/project_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/project_role_template_binding.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/project_role_template_binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         :param pulumi.Input[str] project_id: The project id where bind project role template (string)
         :param pulumi.Input[str] role_template_id: The role template id from create project role template binding (string)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations of the resource (map)
         :param pulumi.Input[str] group_id: The group ID to assign project role template binding (string)
         :param pulumi.Input[str] group_principal_id: The group_principal ID to assign project role template binding (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels of the resource (map)
                
-               **Note** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
+               **Note:** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
         :param pulumi.Input[str] name: The name of the project role template binding (string)
         :param pulumi.Input[str] user_id: The user ID to assign project role template binding (string)
         :param pulumi.Input[str] user_principal_id: The user_principal ID to assign project role template binding (string)
         """
         pulumi.set(__self__, "project_id", project_id)
         pulumi.set(__self__, "role_template_id", role_template_id)
         if annotations is not None:
@@ -116,15 +116,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Labels of the resource (map)
 
-        **Note** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
+        **Note:** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "labels", value)
 
@@ -180,15 +180,15 @@
         """
         Input properties used for looking up and filtering ProjectRoleTemplateBinding resources.
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations of the resource (map)
         :param pulumi.Input[str] group_id: The group ID to assign project role template binding (string)
         :param pulumi.Input[str] group_principal_id: The group_principal ID to assign project role template binding (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels of the resource (map)
                
-               **Note** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
+               **Note:** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
         :param pulumi.Input[str] name: The name of the project role template binding (string)
         :param pulumi.Input[str] project_id: The project id where bind project role template (string)
         :param pulumi.Input[str] role_template_id: The role template id from create project role template binding (string)
         :param pulumi.Input[str] user_id: The user ID to assign project role template binding (string)
         :param pulumi.Input[str] user_principal_id: The user_principal ID to assign project role template binding (string)
         """
         if annotations is not None:
@@ -248,15 +248,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Labels of the resource (map)
 
-        **Note** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
+        **Note:** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "labels", value)
 
@@ -363,15 +363,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations of the resource (map)
         :param pulumi.Input[str] group_id: The group ID to assign project role template binding (string)
         :param pulumi.Input[str] group_principal_id: The group_principal ID to assign project role template binding (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels of the resource (map)
                
-               **Note** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
+               **Note:** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
         :param pulumi.Input[str] name: The name of the project role template binding (string)
         :param pulumi.Input[str] project_id: The project id where bind project role template (string)
         :param pulumi.Input[str] role_template_id: The role template id from create project role template binding (string)
         :param pulumi.Input[str] user_id: The user ID to assign project role template binding (string)
         :param pulumi.Input[str] user_principal_id: The user_principal ID to assign project role template binding (string)
         """
         ...
@@ -477,15 +477,15 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations of the resource (map)
         :param pulumi.Input[str] group_id: The group ID to assign project role template binding (string)
         :param pulumi.Input[str] group_principal_id: The group_principal ID to assign project role template binding (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels of the resource (map)
                
-               **Note** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
+               **Note:** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
         :param pulumi.Input[str] name: The name of the project role template binding (string)
         :param pulumi.Input[str] project_id: The project id where bind project role template (string)
         :param pulumi.Input[str] role_template_id: The role template id from create project role template binding (string)
         :param pulumi.Input[str] user_id: The user ID to assign project role template binding (string)
         :param pulumi.Input[str] user_principal_id: The user_principal ID to assign project role template binding (string)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -529,15 +529,15 @@
 
     @property
     @pulumi.getter
     def labels(self) -> pulumi.Output[Mapping[str, Any]]:
         """
         Labels of the resource (map)
 
-        **Note** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
+        **Note:** user `user_id | user_principal_id` OR group `group_id | group_principal_id` must be defined
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/provider.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,17 @@
 
     @property
     @pulumi.getter
     def retries(self) -> Optional[pulumi.Input[int]]:
         """
         Rancher connection retries
         """
+        warnings.warn("""Use timeout instead""", DeprecationWarning)
+        pulumi.log.warn("""retries is deprecated: Use timeout instead""")
+
         return pulumi.get(self, "retries")
 
     @retries.setter
     def retries(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "retries", value)
 
     @property
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/registry.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -261,19 +261,19 @@
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace_id: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  registries: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RegistryRegistryArgs']]]]] = None,
                  __props__=None):
         """
-        Provides a Rancher v2 Registry resource. This can be used to create docker registries for Rancher v2 environments and retrieve their information.
+        Provides a Rancher v2 Registry resource. This resource creates Kubernetes secrets with the type `kubernetes.io/dockerconfigjson` for authenticating against Docker registries for Rancher v2 environments and retrieving their information.
 
-        Depending of the availability, there are 2 types of Rancher v2 docker registries:
-        - Project registry: Available to all namespaces in the `project_id`
-        - Namespaced registry: Available to just `namespace_id` in the `project_id`
+        Depending on the availability, there are 2 types of Rancher v2 Docker registry resources:
+        - Project registry resource: Available to all namespaces in the `project_id`.
+        - Namespaced registry resource: Available to `namespace_id` in the `project_id`.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
@@ -327,19 +327,19 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: RegistryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Provides a Rancher v2 Registry resource. This can be used to create docker registries for Rancher v2 environments and retrieve their information.
+        Provides a Rancher v2 Registry resource. This resource creates Kubernetes secrets with the type `kubernetes.io/dockerconfigjson` for authenticating against Docker registries for Rancher v2 environments and retrieving their information.
 
-        Depending of the availability, there are 2 types of Rancher v2 docker registries:
-        - Project registry: Available to all namespaces in the `project_id`
-        - Namespaced registry: Available to just `namespace_id` in the `project_id`
+        Depending on the availability, there are 2 types of Rancher v2 Docker registry resources:
+        - Project registry resource: Available to all namespaces in the `project_id`.
+        - Namespaced registry resource: Available to `namespace_id` in the `project_id`.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/role_tempalte.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/role_tempalte.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/role_template.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/role_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/secret.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/secret_v2.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/setting.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/storage_class_v2.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/token.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2/user.py` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2.egg-info/PKG-INFO` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-rancher2
-Version: 5.2.0a1691044117
+Version: 5.2.0a1691077080
 Summary: A Pulumi package for creating and managing rancher2 resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi rancher2
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_rancher2-5.2.0a1691044117/pulumi_rancher2.egg-info/SOURCES.txt` & `pulumi_rancher2-5.2.0a1691077080/pulumi_rancher2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.2.0a1691044117/setup.py` & `pulumi_rancher2-5.2.0a1691077080/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.2.0a1691044117"
-PLUGIN_VERSION = "5.2.0-alpha.1691044117+78c389d7"
+VERSION = "5.2.0a1691077080"
+PLUGIN_VERSION = "5.2.0-alpha.1691077080+4d5a617b"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'rancher2', PLUGIN_VERSION])
         except OSError as error:
```

