# Comparing `tmp/sbcli-3.tar.gz` & `tmp/sbcli-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\HP\PycharmProjects\ultra_repo\ultra\api\dist\.tmp-3jd2g4qz\sbcli-3.tar", last modified: Wed Jul 19 14:44:19 2023, max compression
+gzip compressed data, was "C:\Users\HP\PycharmProjects\ultra_repo\ultra\api\dist\.tmp-636hp240\sbcli-3.1.tar", last modified: Thu Aug  3 20:58:41 2023, max compression
```

## Comparing `sbcli-3.tar` & `sbcli-3.1.tar`

### file list

```diff
@@ -1,56 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 14:44:19.770799 sbcli-3/
--rw-rw-rw-   0        0        0    43374 2023-07-19 14:44:19.769799 sbcli-3/PKG-INFO
--rw-rw-rw-   0        0        0    43124 2023-07-13 15:17:09.000000 sbcli-3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 14:44:19.691009 sbcli-3/management/
--rw-rw-rw-   0        0        0        0 2021-10-27 21:58:56.000000 sbcli-3/management/__init__.py
--rw-rw-rw-   0        0        0    51657 2023-07-19 14:29:48.000000 sbcli-3/management/cli.py
--rw-rw-rw-   0        0        0     6893 2023-07-11 13:47:18.000000 sbcli-3/management/cluster_ops.py
--rw-rw-rw-   0        0        0     5264 2023-03-06 15:46:56.000000 sbcli-3/management/compute_node_ops.py
--rw-rw-rw-   0        0        0      755 2023-07-06 18:09:38.000000 sbcli-3/management/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-19 14:44:19.700982 sbcli-3/management/controllers/
--rw-rw-rw-   0        0        0        0 2023-03-06 16:32:43.000000 sbcli-3/management/controllers/__init__.py
--rw-rw-rw-   0        0        0      955 2023-06-27 12:09:06.000000 sbcli-3/management/controllers/cluster_lifecycle.py
--rw-rw-rw-   0        0        0     8787 2023-06-27 12:04:07.000000 sbcli-3/management/controllers/device_lifecycle.py
--rw-rw-rw-   0        0        0    16507 2023-07-13 17:10:28.000000 sbcli-3/management/controllers/lvol_controller.py
--rw-rw-rw-   0        0        0    13889 2023-06-27 12:01:46.000000 sbcli-3/management/controllers/node_lifecycle.py
--rw-rw-rw-   0        0        0     9473 2023-06-29 12:54:01.000000 sbcli-3/management/controllers/pool_controller.py
--rw-rw-rw-   0        0        0     5773 2023-07-13 17:28:28.000000 sbcli-3/management/kv_store.py
--rw-rw-rw-   0        0        0     3578 2023-05-22 22:51:19.000000 sbcli-3/management/mgmt_node_ops.py
-drwxrwxrwx   0        0        0        0 2023-07-19 14:44:19.721932 sbcli-3/management/models/
--rw-rw-rw-   0        0        0        0 2021-10-28 14:11:47.000000 sbcli-3/management/models/__init__.py
--rw-rw-rw-   0        0        0     4681 2023-07-13 17:24:37.000000 sbcli-3/management/models/base_model.py
--rw-rw-rw-   0        0        0     1815 2023-07-11 12:10:41.000000 sbcli-3/management/models/cluster.py
--rw-rw-rw-   0        0        0      943 2023-02-08 22:16:26.000000 sbcli-3/management/models/compute_node.py
--rw-rw-rw-   0        0        0     3019 2023-07-13 18:37:17.000000 sbcli-3/management/models/device_stat.py
--rw-rw-rw-   0        0        0     1251 2023-05-09 17:37:12.000000 sbcli-3/management/models/global_settings.py
--rw-rw-rw-   0        0        0      830 2023-07-03 20:33:53.000000 sbcli-3/management/models/iface.py
--rw-rw-rw-   0        0        0      620 2023-05-22 22:52:24.000000 sbcli-3/management/models/mgmt_node.py
--rw-rw-rw-   0        0        0     1451 2023-06-28 16:43:11.000000 sbcli-3/management/models/nvme_device.py
--rw-rw-rw-   0        0        0     1690 2023-06-29 12:54:01.000000 sbcli-3/management/models/pool.py
--rw-rw-rw-   0        0        0     3364 2023-06-28 16:58:39.000000 sbcli-3/management/models/storage_node.py
--rw-rw-rw-   0        0        0      966 2023-02-16 22:27:55.000000 sbcli-3/management/pci_utils.py
--rw-rw-rw-   0        0        0    11574 2023-06-28 16:43:12.000000 sbcli-3/management/rpc_client.py
-drwxrwxrwx   0        0        0        0 2023-07-19 14:44:19.735889 sbcli-3/management/services/
--rw-rw-rw-   0        0        0     5008 2023-07-12 16:29:01.000000 sbcli-3/management/services/__init__.py
--rw-rw-rw-   0        0        0     1865 2021-12-22 20:16:04.000000 sbcli-3/management/services/device_monitor.py
--rw-rw-rw-   0        0        0     3515 2023-07-13 19:22:01.000000 sbcli-3/management/services/device_stat_collector.py
--rw-rw-rw-   0        0        0     3185 2023-07-13 19:22:01.000000 sbcli-3/management/services/lvol_stat_collector.py
--rw-rw-rw-   0        0        0     3012 2023-06-27 11:52:17.000000 sbcli-3/management/services/mgmt_node_monitor.py
--rw-rw-rw-   0        0        0     2153 2022-01-11 22:20:04.000000 sbcli-3/management/services/node_monitor.py
--rw-rw-rw-   0        0        0     2445 2023-07-03 20:33:53.000000 sbcli-3/management/services/port_stat_collector.py
--rw-rw-rw-   0        0        0     3999 2022-01-14 19:44:44.000000 sbcli-3/management/services/stat_collector.py
--rw-rw-rw-   0        0        0      288 2023-02-16 23:53:54.000000 sbcli-3/management/shell_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-19 14:44:19.737883 sbcli-3/management/spdk_installer/
--rw-rw-rw-   0        0        0      747 2023-03-02 14:29:22.000000 sbcli-3/management/spdk_installer/__init__.py
--rw-rw-rw-   0        0        0    53543 2023-07-13 19:39:33.000000 sbcli-3/management/storage_node_ops.py
--rw-rw-rw-   0        0        0     1784 2023-07-03 20:29:53.000000 sbcli-3/management/utils.py
--rw-rw-rw-   0        0        0       86 2023-07-19 14:06:48.000000 sbcli-3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-19 14:44:19.767824 sbcli-3/sbcli.egg-info/
--rw-rw-rw-   0        0        0    43374 2023-07-19 14:44:19.000000 sbcli-3/sbcli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1455 2023-07-19 14:44:19.000000 sbcli-3/sbcli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 14:44:19.000000 sbcli-3/sbcli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-19 14:44:19.000000 sbcli-3/sbcli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       61 2023-07-19 14:44:19.000000 sbcli-3/sbcli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-19 14:44:19.000000 sbcli-3/sbcli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 14:44:19.771798 sbcli-3/setup.cfg
--rw-rw-rw-   0        0        0      780 2023-07-19 14:44:02.000000 sbcli-3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:58:41.157622 sbcli-3.1/
+-rw-rw-rw-   0        0        0    43356 2023-08-03 20:58:41.156626 sbcli-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    43124 2023-07-13 15:17:09.000000 sbcli-3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 20:58:40.953168 sbcli-3.1/management/
+-rw-rw-rw-   0        0        0        0 2021-10-27 21:58:56.000000 sbcli-3.1/management/__init__.py
+-rw-rw-rw-   0        0        0    54198 2023-08-03 20:32:22.000000 sbcli-3.1/management/cli.py
+-rw-rw-rw-   0        0        0    12261 2023-08-03 20:32:22.000000 sbcli-3.1/management/cluster_ops.py
+-rw-rw-rw-   0        0        0     5264 2023-03-06 15:46:56.000000 sbcli-3.1/management/compute_node_ops.py
+-rw-rw-rw-   0        0        0      795 2023-08-03 20:21:48.000000 sbcli-3.1/management/constants.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:58:41.010017 sbcli-3.1/management/controllers/
+-rw-rw-rw-   0        0        0        0 2023-03-06 16:32:43.000000 sbcli-3.1/management/controllers/__init__.py
+-rw-rw-rw-   0        0        0     7584 2023-08-01 03:53:15.000000 sbcli-3.1/management/controllers/cluster_events.py
+-rw-rw-rw-   0        0        0      955 2023-06-27 12:09:06.000000 sbcli-3.1/management/controllers/cluster_lifecycle.py
+-rw-rw-rw-   0        0        0     8787 2023-06-27 12:04:07.000000 sbcli-3.1/management/controllers/device_lifecycle.py
+-rw-rw-rw-   0        0        0     1019 2023-08-01 03:44:27.000000 sbcli-3.1/management/controllers/events_controller.py
+-rw-rw-rw-   0        0        0    16507 2023-07-13 17:10:28.000000 sbcli-3.1/management/controllers/lvol_controller.py
+-rw-rw-rw-   0        0        0     3578 2023-08-01 03:53:15.000000 sbcli-3.1/management/controllers/mgmt_events.py
+-rw-rw-rw-   0        0        0    13889 2023-06-27 12:01:46.000000 sbcli-3.1/management/controllers/node_lifecycle.py
+-rw-rw-rw-   0        0        0     9473 2023-06-29 12:54:01.000000 sbcli-3.1/management/controllers/pool_controller.py
+-rw-rw-rw-   0        0        0    36931 2023-08-01 03:53:15.000000 sbcli-3.1/management/controllers/storage_events.py
+-rw-rw-rw-   0        0        0     5834 2023-08-03 20:21:48.000000 sbcli-3.1/management/kv_store.py
+-rw-rw-rw-   0        0        0     3649 2023-08-03 20:21:48.000000 sbcli-3.1/management/mgmt_node_ops.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:58:41.058886 sbcli-3.1/management/models/
+-rw-rw-rw-   0        0        0        0 2021-10-28 14:11:47.000000 sbcli-3.1/management/models/__init__.py
+-rw-rw-rw-   0        0        0     4681 2023-07-13 17:24:37.000000 sbcli-3.1/management/models/base_model.py
+-rw-rw-rw-   0        0        0     1871 2023-08-03 20:21:48.000000 sbcli-3.1/management/models/cluster.py
+-rw-rw-rw-   0        0        0      943 2023-02-08 22:16:26.000000 sbcli-3.1/management/models/compute_node.py
+-rw-rw-rw-   0        0        0     3019 2023-07-13 18:37:17.000000 sbcli-3.1/management/models/device_stat.py
+-rw-rw-rw-   0        0        0     1140 2023-08-03 20:21:48.000000 sbcli-3.1/management/models/events.py
+-rw-rw-rw-   0        0        0     1251 2023-05-09 17:37:12.000000 sbcli-3.1/management/models/global_settings.py
+-rw-rw-rw-   0        0        0      830 2023-07-03 20:33:53.000000 sbcli-3.1/management/models/iface.py
+-rw-rw-rw-   0        0        0      673 2023-08-03 20:21:48.000000 sbcli-3.1/management/models/mgmt_node.py
+-rw-rw-rw-   0        0        0     1451 2023-06-28 16:43:11.000000 sbcli-3.1/management/models/nvme_device.py
+-rw-rw-rw-   0        0        0     1690 2023-06-29 12:54:01.000000 sbcli-3.1/management/models/pool.py
+-rw-rw-rw-   0        0        0     3364 2023-06-28 16:58:39.000000 sbcli-3.1/management/models/storage_node.py
+-rw-rw-rw-   0        0        0      966 2023-02-16 22:27:55.000000 sbcli-3.1/management/pci_utils.py
+-rw-rw-rw-   0        0        0    11574 2023-06-28 16:43:12.000000 sbcli-3.1/management/rpc_client.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:58:41.069857 sbcli-3.1/management/scripts/
+-rw-rw-rw-   0        0        0     1050 2023-08-03 20:21:48.000000 sbcli-3.1/management/scripts/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-08-03 20:21:48.000000 sbcli-3.1/management/scripts/db_config_single.sh
+-rw-rw-rw-   0        0        0      310 2023-08-03 20:21:48.000000 sbcli-3.1/management/scripts/deploy_stack.sh
+-rw-rw-rw-   0        0        0     1125 2023-08-03 20:21:48.000000 sbcli-3.1/management/scripts/install_deps.sh
+-rw-rw-rw-   0        0        0        0 2023-08-03 20:21:48.000000 sbcli-3.1/management/scripts/prepare_mgmt.sh
+-rw-rw-rw-   0        0        0       62 2023-08-03 20:21:48.000000 sbcli-3.1/management/scripts/set_db_config.sh
+drwxrwxrwx   0        0        0        0 2023-08-03 20:58:41.123712 sbcli-3.1/management/services/
+-rw-rw-rw-   0        0        0     5008 2023-07-12 16:29:01.000000 sbcli-3.1/management/services/__init__.py
+-rw-rw-rw-   0        0        0     1865 2021-12-22 20:16:04.000000 sbcli-3.1/management/services/device_monitor.py
+-rw-rw-rw-   0        0        0     3517 2023-08-01 03:53:15.000000 sbcli-3.1/management/services/device_stat_collector.py
+-rw-rw-rw-   0        0        0     3185 2023-07-13 19:22:01.000000 sbcli-3.1/management/services/lvol_stat_collector.py
+-rw-rw-rw-   0        0        0     3012 2023-06-27 11:52:17.000000 sbcli-3.1/management/services/mgmt_node_monitor.py
+-rw-rw-rw-   0        0        0     2153 2022-01-11 22:20:04.000000 sbcli-3.1/management/services/node_monitor.py
+-rw-rw-rw-   0        0        0     2445 2023-07-03 20:33:53.000000 sbcli-3.1/management/services/port_stat_collector.py
+-rw-rw-rw-   0        0        0     3999 2022-01-14 19:44:44.000000 sbcli-3.1/management/services/stat_collector.py
+-rw-rw-rw-   0        0        0      288 2023-02-16 23:53:54.000000 sbcli-3.1/management/shell_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:58:41.126705 sbcli-3.1/management/spdk_installer/
+-rw-rw-rw-   0        0        0      747 2023-03-02 14:29:22.000000 sbcli-3.1/management/spdk_installer/__init__.py
+-rw-rw-rw-   0        0        0    53543 2023-07-13 19:39:33.000000 sbcli-3.1/management/storage_node_ops.py
+-rw-rw-rw-   0        0        0     2061 2023-08-03 20:24:10.000000 sbcli-3.1/management/utils.py
+-rw-rw-rw-   0        0        0       86 2023-07-19 14:06:48.000000 sbcli-3.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-03 20:58:41.154631 sbcli-3.1/sbcli.egg-info/
+-rw-rw-rw-   0        0        0    43356 2023-08-03 20:58:40.000000 sbcli-3.1/sbcli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1858 2023-08-03 20:58:40.000000 sbcli-3.1/sbcli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 20:58:40.000000 sbcli-3.1/sbcli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-08-03 20:58:40.000000 sbcli-3.1/sbcli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-08-03 20:58:40.000000 sbcli-3.1/sbcli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-03 20:58:40.000000 sbcli-3.1/sbcli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 20:58:41.157622 sbcli-3.1/setup.cfg
+-rw-rw-rw-   0        0        0      819 2023-08-03 20:54:24.000000 sbcli-3.1/setup.py
```

### Comparing `sbcli-3/PKG-INFO` & `sbcli-3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sbcli
-Version: 3
+Version: 3.1
 Summary: CLI for managing SimplyBlock cluster
-Home-page: https://github.com/simplyblock-io/ultra
+Home-page: https://github.com/
 Author: Hamdy Khader
 Author-email: hamdy.khader@gmail.com
 Description-Content-Type: text/markdown
 
 
 # Simply Block
 [![Docker Image CI](https://github.com/simplyblock-io/ultra/actions/workflows/docker-image.yml/badge.svg?branch=main)](https://github.com/simplyblock-io/ultra/actions/workflows/docker-image.yml)
```

### Comparing `sbcli-3/README.md` & `sbcli-3.1/README.md`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/cli.py` & `sbcli-3.1/management/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,42 @@
         sub_command.add_argument("--iSCSI", help='The cluster supports iscsi LUNs in addition to nvmeof volumes',
                                  required=False, action='store_true')
         sub_command.add_argument("--CLI_PASS", help='Password for CLI SSH connection', required=False)
 
         # show cluster list
         sub_command = self.add_sub_command(subparser, 'list', 'Show clusters list')
 
+        # cluster create
+        sub_command = self.add_sub_command(subparser, 'create', 'Create an new cluster with this node as mgmt')
+        sub_command.add_argument(
+            "--blk_size", help='The block size in bytes', type=int,  choices=[512, 4096], default=512)
+        sub_command.add_argument(
+            "--page_size_in_blocks", help='The size of a data page in logical blocks', type=int, default=512)
+
+        sub_command.add_argument(
+            "--ha_type", help='Can be "single" for single node clusters or  "HA", which requires at least 3 nodes',
+            choices=["single", "ha"], default='single')
+        sub_command.add_argument(
+            "--tls", help='TCP/IP transport security can be turned on and off. '
+                          'If turned on, both hosts and storage nodes must '
+                          'authenticate the connection via TLS certificates',
+            choices=["on", "off"], default='off')
+        sub_command.add_argument(
+            "--auth-hosts-only", help='if turned on, hosts must be explicitely added to the '
+                                      'cluster to be able to connect to any NVMEoF subsystem in the cluster',
+            choices=["on", "off"], default='off')
+
+        sub_command.add_argument("NQN", help='cluster NQN subsystem')
+        sub_command.add_argument("--CLI_PASS", help='Password for CLI SSH connection', required=False)
+
+        # join cluster
+        sub_command = self.add_sub_command(subparser, 'join', 'join cluster')
+        sub_command.add_argument("cluster_ip", help='the cluster IP address')
+        sub_command.add_argument("cluster_id", help='the cluster UUID')
+
         # show cluster info
         sub_command = self.add_sub_command(
             subparser, 'status', 'Show cluster status')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
 
         sub_command = self.add_sub_command(
             subparser, 'suspend', 'Suspend cluster. The cluster will stop processing all IO. '
@@ -628,14 +656,18 @@
         elif args.command == 'cluster':
             sub_command = args_dict[args.command]
             if sub_command in ["add-dev-model", "rm-dev-model", "add-host-auth",
                                "rm-host-auth", "set-log-level", "get-event-log"]:
                 ret = "Not Implemented!"
             elif sub_command == 'init':
                 ret = self.cluster_init(args)
+            elif sub_command == 'create':
+                ret = self.cluster_create(args)
+            elif sub_command == 'join':
+                ret = self.cluster_join(args)
             elif sub_command == 'status':
                 cluster_id = args.cluster_id
                 ret = cluster_ops.show_cluster(cluster_id)
             elif sub_command == 'list':
                 ret = cluster_ops.list()
             elif sub_command == 'suspend':
                 cluster_id = args.cluster_id
@@ -845,14 +877,33 @@
         CLI_PASS = args.CLI_PASS
 
         # TODO: Validate the inputs
         return cluster_ops.add_cluster(
             blk_size, page_size_in_blocks, model_ids, ha_type, tls,
             auth_hosts_only, dhchap, NQN, iSCSI, CLI_PASS)
 
+    def cluster_create(self, args):
+        page_size_in_blocks = args.page_size_in_blocks
+        blk_size = args.blk_size
+        ha_type = args.ha_type
+        tls = args.tls == 'on'
+        auth_hosts_only = args.auth_hosts_only == 'on'
+        NQN = args.NQN
+        CLI_PASS = args.CLI_PASS
+
+        # TODO: Validate the inputs
+        return cluster_ops.create_cluster(
+            blk_size, page_size_in_blocks , ha_type, tls,
+            auth_hosts_only, NQN , CLI_PASS)
+
+    def cluster_join(self, args):
+        cluster_id = args.cluster_id
+        cluster_ip = args.cluster_ip
+        return cluster_ops.join_cluster(cluster_ip, cluster_id)
+
     def query_yes_no(self, question, default="yes"):
         """Ask a yes/no question via raw_input() and return their answer.
 
         "question" is a string that is presented to the user.
         "default" is the presumed answer if the user just hits <Enter>.
                 It must be "yes" (the default), "no" or None (meaning
                 an answer is required of the user).
```

### Comparing `sbcli-3/management/cluster_ops.py` & `sbcli-3.1/management/controllers/cluster_events.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import time
 import uuid
 
 import docker
 
 from management import utils
+from management.controllers import events_controller as ec
 from management.kv_store import DBController
 from management.models.cluster import Cluster
 from management.models.device_stat import DeviceStat
 
 logger = logging.getLogger()
 db_controller = DBController()
 
@@ -61,27 +62,46 @@
 
 def suspend_cluster(cl_id):
     cls = db_controller.get_clusters(id=cl_id)
     if not cls:
         logger.error(f"Cluster not found {cl_id}")
         return False
     cl = cls[0]
+    old_status = cl.status
     cl.status = Cluster.STATUS_SUSPENDED
     cl.write_to_db(db_controller.kv_store)
+
+    ec.log_event_cluster(
+        cluster_id=cl.get_id(),
+        domain=ec.DOMAIN_CLUSTER,
+        event=ec.EVENT_STATUS_CHANGE,
+        db_object=cl,
+        caused_by=ec.CAUSED_BY_CLI,
+        message=f"Cluster status changed from {old_status} to {Cluster.STATUS_SUSPENDED}")
+
     return "Done"
 
 
 def unsuspend_cluster(cl_id):
     cls = db_controller.get_clusters(id=cl_id)
     if not cls:
         logger.error(f"Cluster not found {cl_id}")
         return False
     cl = cls[0]
+    old_status = cl.status
     cl.status = Cluster.STATUS_ACTIVE
     cl.write_to_db(db_controller.kv_store)
+    ec.log_event_cluster(
+        cluster_id=cl.get_id(),
+        domain=ec.DOMAIN_CLUSTER,
+        event=ec.EVENT_STATUS_CHANGE,
+        db_object=cl,
+        caused_by=ec.CAUSED_BY_CLI,
+        message=f"Cluster status changed from {old_status} to {Cluster.STATUS_ACTIVE}")
+
     return "Done"
 
 
 def list():
     cls = db_controller.get_clusters()
     st = db_controller.get_storage_nodes()
     mt = db_controller.get_mgmt_nodes()
```

### Comparing `sbcli-3/management/compute_node_ops.py` & `sbcli-3.1/management/compute_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/constants.py` & `sbcli-3.1/management/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 KVD_DB_FILE_PATH = '/etc/foundationdb/fdb.cluster'
 SPK_DIR = '/home/ec2-user/spdk'
 RPC_HTTP_PROXY_PORT = 8080
 LOG_LEVEL = logging.INFO
 
 FILE_DIR = os.path.dirname(os.path.realpath(__file__))
 INSTALL_DIR = os.path.dirname(FILE_DIR)
+TOP_DIR = os.path.dirname(INSTALL_DIR)
 
 NODE_MONITOR_INTERVAL_SEC = 5
 DEVICE_MONITOR_INTERVAL_SEC = 5
 STAT_COLLECTOR_INTERVAL_SEC = 60*5  # 5 minutes
 LVOL_STAT_COLLECTOR_INTERVAL_SEC = 2
 DEV_STAT_COLLECTOR_INTERVAL_SEC = 2
 PROT_STAT_COLLECTOR_INTERVAL_SEC = 2
```

### Comparing `sbcli-3/management/controllers/cluster_lifecycle.py` & `sbcli-3.1/management/controllers/cluster_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/controllers/device_lifecycle.py` & `sbcli-3.1/management/controllers/device_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/controllers/lvol_controller.py` & `sbcli-3.1/management/controllers/lvol_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/controllers/node_lifecycle.py` & `sbcli-3.1/management/controllers/node_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/controllers/pool_controller.py` & `sbcli-3.1/management/controllers/pool_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/kv_store.py` & `sbcli-3.1/management/kv_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,20 @@
 from management.models.storage_node import StorageNode, LVol
 
 logger = logging.getLogger()
 
 
 class KVStore:
     def __init__(self):
-        fdb.api_version(constants.KVD_DB_VERSION)
-        self.db = fdb.open(constants.KVD_DB_FILE_PATH)
-        self.db.options.set_transaction_timeout(3000)
+        try:
+            fdb.api_version(constants.KVD_DB_VERSION)
+            self.db = fdb.open(constants.KVD_DB_FILE_PATH)
+            self.db.options.set_transaction_timeout(3000)
+        except:
+            pass
 
     def set(self, key, value):
         self.db.set(key, value)
         return
 
     def rm(self, key):
         self.db.clear(key)
```

### Comparing `sbcli-3/management/mgmt_node_ops.py` & `sbcli-3.1/management/controllers/mgmt_events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/models/base_model.py` & `sbcli-3.1/management/models/base_model.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/models/cluster.py` & `sbcli-3.1/management/models/cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         "ha_type": {"type": str, 'default': "single"},
         "tls": {"type": bool, 'default': False},
         "auth_hosts_only": {"type": bool, 'default': False},
         "nqn": {"type": str, 'default': ""},
         "iscsi": {"type": str, 'default': ""},
         "dhchap": {"type": str, "default": ""},
         "cli_pass": {"type": str, "default": ""},
+        "db_connection": {"type": str, "default": ""},
         "cluster_status": {"type": str, "default": ""},
         "updated_at": {"type": str, "default": ""},
     }
 
     def __init__(self, data=None):
         super(Cluster, self).__init__()
         self.set_attrs(self.attributes, data)
```

### Comparing `sbcli-3/management/models/compute_node.py` & `sbcli-3.1/management/models/compute_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/models/device_stat.py` & `sbcli-3.1/management/models/device_stat.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/models/global_settings.py` & `sbcli-3.1/management/models/global_settings.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/models/iface.py` & `sbcli-3.1/management/models/iface.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/models/mgmt_node.py` & `sbcli-3.1/management/models/mgmt_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
     attributes = {
         "baseboard_sn": {"type": str, 'default': ""},
         "system_uuid": {"type": str, 'default': ""},
         "hostname": {"type": str, 'default': ""},
         "status": {"type": str, 'default': ""},
         "docker_ip_port": {"type": str, 'default': ""},
+        "cluster_id": {"type": str, 'default': ""},
     }
 
     def __init__(self, data=None):
         super(MgmtNode, self).__init__()
         self.set_attrs(self.attributes, data)
         self.object_type = "object"
```

### Comparing `sbcli-3/management/models/nvme_device.py` & `sbcli-3.1/management/models/nvme_device.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/models/pool.py` & `sbcli-3.1/management/models/pool.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/models/storage_node.py` & `sbcli-3.1/management/models/storage_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/pci_utils.py` & `sbcli-3.1/management/pci_utils.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/rpc_client.py` & `sbcli-3.1/management/rpc_client.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/services/__init__.py` & `sbcli-3.1/management/services/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/services/device_monitor.py` & `sbcli-3.1/management/services/device_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/services/device_stat_collector.py` & `sbcli-3.1/management/services/device_stat_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
             "read_iops": int((stats['num_read_ops'] - last_stat.stats['num_read_ops']) / (now - last_stat.date)),
             "write_bytes_per_sec": int(
                 (stats['bytes_written'] - last_stat.stats['bytes_written']) / (now - last_stat.date)),
             "write_iops": int((stats['num_write_ops'] - last_stat.stats['num_write_ops']) / (now - last_stat.date)),
             "unmapped_bytes_per_sec": int(
                 (stats['bytes_unmapped'] - last_stat.stats['bytes_unmapped']) / (now - last_stat.date)),
         })
+
     else:
         logger.warning("last record not found")
 
     stat_obj = DeviceStat(data=data)
     stat_obj.write_to_db(db_store)
     return
```

### Comparing `sbcli-3/management/services/lvol_stat_collector.py` & `sbcli-3.1/management/services/lvol_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/services/mgmt_node_monitor.py` & `sbcli-3.1/management/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/services/node_monitor.py` & `sbcli-3.1/management/services/node_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/services/port_stat_collector.py` & `sbcli-3.1/management/services/port_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/services/stat_collector.py` & `sbcli-3.1/management/services/stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/spdk_installer/__init__.py` & `sbcli-3.1/management/spdk_installer/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/storage_node_ops.py` & `sbcli-3.1/management/storage_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-3/management/utils.py` & `sbcli-3.1/management/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # coding=utf-8
 import logging
 import os
+import random
+import string
 
 from management import shell_utils
 from prettytable import PrettyTable
 
 logger = logging.getLogger()
 
 
@@ -29,14 +31,19 @@
 
 
 def get_hostname():
     out, _, _ = shell_utils.run_command("hostname -s")
     return out
 
 
+def get_ips():
+    out, _, _ = shell_utils.run_command("hostname -I")
+    return out
+
+
 def print_table(data: list):
     if data:
         x = PrettyTable(field_names=data[0].keys())
         x.align = 'l'
         for node_data in data:
             row = []
             for key in node_data:
@@ -61,7 +68,12 @@
         return '{0:.1f} KB'.format(B / KB)
     elif MB <= B < GB:
         return '{0:.1f} MB'.format(B / MB)
     elif GB <= B < TB:
         return '{0:.1f} GB'.format(B / GB)
     elif TB <= B:
         return '{0:.1f} TB'.format(B / TB)
+
+
+def generate_string(length):
+    return ''.join(random.SystemRandom().choice(
+        string.ascii_letters + string.digits) for _ in range(length))
```

### Comparing `sbcli-3/sbcli.egg-info/PKG-INFO` & `sbcli-3.1/sbcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sbcli
-Version: 3
+Version: 3.1
 Summary: CLI for managing SimplyBlock cluster
-Home-page: https://github.com/simplyblock-io/ultra
+Home-page: https://github.com/
 Author: Hamdy Khader
 Author-email: hamdy.khader@gmail.com
 Description-Content-Type: text/markdown
 
 
 # Simply Block
 [![Docker Image CI](https://github.com/simplyblock-io/ultra/actions/workflows/docker-image.yml/badge.svg?branch=main)](https://github.com/simplyblock-io/ultra/actions/workflows/docker-image.yml)
```

### Comparing `sbcli-3/sbcli.egg-info/SOURCES.txt` & `sbcli-3.1/sbcli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,30 +10,41 @@
 management/mgmt_node_ops.py
 management/pci_utils.py
 management/rpc_client.py
 management/shell_utils.py
 management/storage_node_ops.py
 management/utils.py
 management/controllers/__init__.py
+management/controllers/cluster_events.py
 management/controllers/cluster_lifecycle.py
 management/controllers/device_lifecycle.py
+management/controllers/events_controller.py
 management/controllers/lvol_controller.py
+management/controllers/mgmt_events.py
 management/controllers/node_lifecycle.py
 management/controllers/pool_controller.py
+management/controllers/storage_events.py
 management/models/__init__.py
 management/models/base_model.py
 management/models/cluster.py
 management/models/compute_node.py
 management/models/device_stat.py
+management/models/events.py
 management/models/global_settings.py
 management/models/iface.py
 management/models/mgmt_node.py
 management/models/nvme_device.py
 management/models/pool.py
 management/models/storage_node.py
+management/scripts/__init__.py
+management/scripts/db_config_single.sh
+management/scripts/deploy_stack.sh
+management/scripts/install_deps.sh
+management/scripts/prepare_mgmt.sh
+management/scripts/set_db_config.sh
 management/services/__init__.py
 management/services/device_monitor.py
 management/services/device_stat_collector.py
 management/services/lvol_stat_collector.py
 management/services/mgmt_node_monitor.py
 management/services/node_monitor.py
 management/services/port_stat_collector.py
```

### Comparing `sbcli-3/setup.py` & `sbcli-3.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sbcli',
-    version='3',
+    version='3.1',
     packages=find_packages(),
-    url='https://github.com/simplyblock-io/ultra',
+    url='https://github.com/',
     author='Hamdy Khader',
     author_email='hamdy.khader@gmail.com',
     description='CLI for managing SimplyBlock cluster',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "foundationdb",
         "requests",
-        "numpy",
         "typing",
         "prettytable",
         "docker",
         "psutil",
     ],
     entry_points={
         'console_scripts': [
             'sbcli=management.cli:__main__',
         ]
-    }
+    },
+    include_package_data=True,
+    package_data={'': ['scripts/*.sh']},
 )
```

