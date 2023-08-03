# Comparing `tmp/hiddifypanel-8.0.0.dev7.tar.gz` & `tmp/hiddifypanel-8.0.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiddifypanel-8.0.0.dev7.tar", last modified: Thu Aug  3 11:29:57 2023, max compression
+gzip compressed data, was "hiddifypanel-8.0.0.dev8.tar", last modified: Thu Aug  3 12:15:28 2023, max compression
```

## Comparing `hiddifypanel-8.0.0.dev7.tar` & `hiddifypanel-8.0.0.dev8.tar`

### file list

```diff
@@ -1,822 +1,822 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:57.019985 hiddifypanel-8.0.0.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34997 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)    19807 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 11:29:57.019985 hiddifypanel-8.0.0.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.887985 hiddifypanel-8.0.0.dev7/hiddifypanel/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/Events.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.887985 hiddifypanel-8.0.0.dev7/hiddifypanel/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/drivers/abstract_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/drivers/singbox_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/drivers/ssh_liberty_bridge_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/drivers/user_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/drivers/xray_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.891985 hiddifypanel-8.0.0.dev7/hiddifypanel/models/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/models/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/models/child.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/models/config_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/models/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/models/parent_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/models/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/models/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.891985 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.891985 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/Actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/AdminstratorAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/Backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/ChildAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/ConfigAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/Dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/DomainAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/ProxyAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/QuickSetup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/SettingAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/Terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/UserAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/adminlte.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/commercial_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.895985 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/a.html
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/backup.html
--rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/base2.html
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/commercial_info.html
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/config.html
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/configfake.html
--rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/ltemaster.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.895985 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/model/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/model/admin_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/model/domain_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/model/user_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/parent_dash.html
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/proxy.html
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/quick_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/result.html
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/cf_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/clean_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.895985 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/ParentDomainAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/ProxyDetailsAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.895985 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/restapi/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/restapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/restapi/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/restapi/tgbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/restapi/tgmsg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.895985 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/telegrambot/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/telegrambot/DefaultResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/telegrambot/Usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/telegrambot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/telegrambot/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/telegrambot/information.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.895985 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/templates/configc.html
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/templates/parent_dash.html
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/custom_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    25093 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/hiddify.py
--rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/init_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.895985 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/link_maker.html
--rw-r--r--   0 runner    (1001) docker     (123)    19572 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/link_maker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.895985 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/all_configs copy.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/all_configs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/clash_config copy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/clash_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/clash_proxies copy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/clash_proxies.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.899985 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/all-configs.html
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/all-configs_old.html
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/android.html
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/base2.html
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/clash-links copy.html
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/clash-links.html
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/doh.html
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/index copy.html
--rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/index_old.html
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/ios copy.html
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/ios.html
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/multi.html
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/speedtest.html
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/telegram.html
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/usage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/windows.html
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/singbox_config.json
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.899985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/a.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.903985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)  1665614 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/adminlte.css
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/adminlte.fa.css
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/adminlte.rtl.css
--rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/bootstrap4-rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   163995 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/bootstrap5.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/custom-rtl.css
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)   101895 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (123)   278568 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/lte.old
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.907985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    92934 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Black.eot
--rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    53500 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Black.woff
--rw-r--r--   0 runner    (1001) docker     (123)    42308 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Black.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    91810 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Bold.eot
--rw-r--r--   0 runner    (1001) docker     (123)    91644 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    52676 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    41856 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   101090 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Light.eot
--rw-r--r--   0 runner    (1001) docker     (123)   100920 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    59988 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Light.woff
--rw-r--r--   0 runner    (1001) docker     (123)    48616 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Light.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   107842 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Medium.eot
--rw-r--r--   0 runner    (1001) docker     (123)   107668 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    63312 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Medium.woff
--rw-r--r--   0 runner    (1001) docker     (123)    51256 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Medium.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    90482 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Thin.eot
--rw-r--r--   0 runner    (1001) docker     (123)    90316 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    51884 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Thin.woff
--rw-r--r--   0 runner    (1001) docker     (123)    41344 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Thin.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    85354 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir.eot
--rw-r--r--   0 runner    (1001) docker     (123)    85192 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    47972 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir.woff
--rw-r--r--   0 runner    (1001) docker     (123)    38004 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.907985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/WhiteLogo.png
--rw-r--r--   0 runner    (1001) docker     (123)   103814 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   111125 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/hiddify-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    37408 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/hiddify.png
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/no_back_hiddify.png
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/pwa-icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.907985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/
--rw-r--r--   0 runner    (1001) docker     (123)    75224 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/ipad_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    85623 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/ipadpro1_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)   121021 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/ipadpro2_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    90886 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/ipadpro3_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    28231 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/iphone5_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/iphone6_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    68643 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/iphoneplus_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    69743 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/iphonex_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    45109 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/iphonexr_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    80648 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/iphonexsmax_splash.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.911985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   104260 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/adminlte.js
--rw-r--r--   0 runner    (1001) docker     (123)    49278 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/bootbox.all.js
--rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/bootbox.all.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    60406 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/custom-rtl.js
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/custom.js
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/demo.js
--rw-r--r--   0 runner    (1001) docker     (123)    89764 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/jquery-3.6.1.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/js.cookie.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    51465 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/moment.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19032 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/pwa-sw.js
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/pwa.js
--rw-r--r--   0 runner    (1001) docker     (123)    33168 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/qrcode.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.887985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.883985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.911985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)    37644 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (123)    28977 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   172839 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)   140421 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.915985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)   210612 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)    70808 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   122441 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)    58072 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.911985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap-slider/
--rw-r--r--   0 runner    (1001) docker     (123)    36164 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap-slider/bootstrap-slider.js
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap-slider/slider.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.911985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap-wysihtml5/
--rw-r--r--   0 runner    (1001) docker     (123)   566620 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js
--rw-r--r--   0 runner    (1001) docker     (123)   210932 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.883985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap4-editable/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.915985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap4-editable/css/
--rw-r--r--   0 runner    (1001) docker     (123)    21490 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap4-editable/css/bootstrap-editable.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.915985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap4-editable/img/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap4-editable/img/clear.png
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap4-editable/img/loading.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.915985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap4-editable/js/
--rw-r--r--   0 runner    (1001) docker     (123)   225176 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.js
--rw-r--r--   0 runner    (1001) docker     (123)    76077 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.915985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/chart.js/
--rw-r--r--   0 runner    (1001) docker     (123)   535484 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/chart.js/Chart.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   211133 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/chart.js/Chart.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   403941 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/chart.js/Chart.js
--rw-r--r--   0 runner    (1001) docker     (123)   159638 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/chart.js/Chart.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.915985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/chartjs-old/
--rw-r--r--   0 runner    (1001) docker     (123)   109613 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/chartjs-old/Chart.js
--rw-r--r--   0 runner    (1001) docker     (123)    52092 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/chartjs-old/Chart.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.919985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/
--rw-r--r--   0 runner    (1001) docker     (123)   433051 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/ckeditor.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.923985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ar.js
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ast.js
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/bg.js
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/cs.js
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/da.js
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/de.js
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/el.js
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/en-au.js
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/eo.js
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/es.js
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/et.js
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/eu.js
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/fi.js
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/fr.js
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/gl.js
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/gu.js
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/hr.js
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/hu.js
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/it.js
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ja.js
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/km.js
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/kn.js
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ko.js
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ku.js
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/nb.js
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ne.js
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/nl.js
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/oc.js
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/pl.js
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/pt-br.js
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/pt.js
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ro.js
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ru.js
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/si.js
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/sk.js
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/sq.js
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/sv.js
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/tr.js
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/tt.js
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ug.js
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/uk.js
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/zh-cn.js
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/zh.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.923985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.css
--rw-r--r--   0 runner    (1001) docker     (123)    33831 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.js
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.923985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/img/
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/img/alpha-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/img/alpha.png
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/img/hue-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/img/hue.png
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/img/saturation.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.923985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.css
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.883985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.923985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/AutoFill/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/AutoFill/Readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.923985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/dataTables.autoFill.css
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/dataTables.autoFill.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.923985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/filler.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.923985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/
--rw-r--r--   0 runner    (1001) docker     (123)    22645 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.js
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.923985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/License.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.923985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/dataTables.colReorder.css
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/dataTables.colReorder.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.923985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/insert.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/
--rw-r--r--   0 runner    (1001) docker     (123)    36311 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.js
--rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/License.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.css
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colvis.jqueryui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/
--rw-r--r--   0 runner    (1001) docker     (123)    27029 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.js
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/License.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.css
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/
--rw-r--r--   0 runner    (1001) docker     (123)    40932 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.js
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/Readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/dataTables.fixedHeader.css
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/dataTables.fixedHeader.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/
--rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.js
--rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/KeyTable/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/KeyTable/Readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/dataTables.keyTable.css
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/dataTables.keyTable.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/
--rw-r--r--   0 runner    (1001) docker     (123)    29477 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.js
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/License.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.css
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/responsive.bootstrap4.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/
--rw-r--r--   0 runner    (1001) docker     (123)    25098 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.js
--rw-r--r--   0 runner    (1001) docker     (123)    14589 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/responsive.bootstrap4.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/Readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.css
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.927985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/loading-background.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.931985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/
--rw-r--r--   0 runner    (1001) docker     (123)    37984 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.js
--rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.931985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.931985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.css
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.931985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection.png
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy.png
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv.png
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf.png
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print.png
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls.png
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls_hover.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.931985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/
--rw-r--r--   0 runner    (1001) docker     (123)    84578 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.js
--rw-r--r--   0 runner    (1001) docker     (123)    31850 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.931985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls.swf
--rw-r--r--   0 runner    (1001) docker     (123)    58846 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls_pdf.swf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.931985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/images/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/images/sort_asc.png
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/images/sort_asc_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/images/sort_both.png
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/images/sort_desc.png
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/images/sort_desc_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/jquery.dataTables.css
--rw-r--r--   0 runner    (1001) docker     (123)    86551 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/jquery.dataTables.js
--rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    86551 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/jquery.dataTables_themeroller.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.931985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/
--rw-r--r--   0 runner    (1001) docker     (123)    46838 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/bootstrap-datepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)    33745 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/datepicker3.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.935985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ar.js
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.az.js
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.bg.js
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ca.js
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cs.js
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cy.js
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.da.js
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.de.js
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.el.js
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.es.js
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.et.js
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fa.js
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fi.js
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fr.js
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.gl.js
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.he.js
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hr.js
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hu.js
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.id.js
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.is.js
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.it.js
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ja.js
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ka.js
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kk.js
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kr.js
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lt.js
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lv.js
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.mk.js
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ms.js
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nb.js
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl-BE.js
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl.js
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.no.js
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pl.js
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt.js
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ro.js
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs-latin.js
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs.js
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ru.js
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sk.js
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sl.js
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sq.js
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sv.js
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sw.js
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.th.js
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.tr.js
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ua.js
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.vi.js
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-CN.js
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-TW.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.935985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/daterangepicker/
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/daterangepicker/daterangepicker-bs3.css
--rw-r--r--   0 runner    (1001) docker     (123)    53679 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/daterangepicker/daterangepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)    99201 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/daterangepicker/moment.js
--rw-r--r--   0 runner    (1001) docker     (123)    34737 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/daterangepicker/moment.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.935985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fastclick/
--rw-r--r--   0 runner    (1001) docker     (123)    25965 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fastclick/fastclick.js
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fastclick/fastclick.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.947985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/
--rw-r--r--   0 runner    (1001) docker     (123)    41944 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/excanvas.js
--rw-r--r--   0 runner    (1001) docker     (123)    19314 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/excanvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.colorhelpers.js
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.colorhelpers.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.canvas.js
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.categories.js
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.categories.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.js
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.js
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.js
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.image.js
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.image.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   121627 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.js
--rw-r--r--   0 runner    (1001) docker     (123)    52300 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.navigate.js
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.navigate.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    23635 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.pie.js
--rw-r--r--   0 runner    (1001) docker     (123)    12024 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.pie.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.resize.js
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.resize.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.selection.js
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.selection.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.stack.js
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.stack.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.symbol.js
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.symbol.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.threshold.js
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.threshold.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.time.js
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.time.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.883985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.951985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/css/
--rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (123)    21778 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.951985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   134808 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.955985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fullcalendar/
--rw-r--r--   0 runner    (1001) docker     (123)    22515 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fullcalendar/fullcalendar.css
--rw-r--r--   0 runner    (1001) docker     (123)   279259 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fullcalendar/fullcalendar.js
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    84823 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fullcalendar/fullcalendar.print.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.955985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/all.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.963985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/_all.css
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/aero.css
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/aero.png
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/blue.css
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/blue.png
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/flat.css
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/flat.png
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/flat@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/green.css
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/green.png
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/grey.css
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/grey.png
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/orange.css
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/orange.png
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/pink.css
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/pink.png
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/purple.css
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/purple.png
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/red.css
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/red.png
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/yellow.css
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/yellow.png
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.963985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/futurico/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/futurico/futurico.css
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/futurico/futurico.png
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/futurico/futurico@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/icheck.js
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/icheck.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.967985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/
--rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/_all.css
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/aero.css
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/blue.css
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/green.css
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/grey.css
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/line.css
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/line.png
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/line@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/orange.css
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/pink.css
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/purple.css
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/red.css
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/yellow.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.975985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/_all.css
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/aero.css
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/aero.png
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/blue.css
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/blue.png
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/green.css
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/green.png
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/grey.css
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/grey.png
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/minimal.css
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/minimal.png
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/minimal@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/orange.css
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/orange.png
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/pink.css
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/pink.png
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/purple.css
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/purple.png
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/red.css
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/red.png
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/yellow.css
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/yellow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.975985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/polaris/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/polaris/polaris.css
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/polaris/polaris.png
--rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/polaris/polaris@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.987985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/
--rw-r--r--   0 runner    (1001) docker     (123)    15591 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/_all.css
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/aero.css
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/aero.png
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/blue.css
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/blue.png
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/green.css
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/green.png
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/grey.css
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/grey.png
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/orange.css
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/orange.png
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/pink.css
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/pink.png
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/purple.css
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/purple.png
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/red.css
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/red.png
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/square.css
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/square.png
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/square@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/yellow.css
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/yellow.png
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.991985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/
--rw-r--r--   0 runner    (1001) docker     (123)    22814 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/jquery.inputmask.date.extensions.js
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/jquery.inputmask.extensions.js
--rw-r--r--   0 runner    (1001) docker     (123)    90539 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/jquery.inputmask.js
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/jquery.inputmask.numeric.extensions.js
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/jquery.inputmask.phone.extensions.js
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/jquery.inputmask.regex.extensions.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.991985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/phone-codes/
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/phone-codes/phone-be.json
--rw-r--r--   0 runner    (1001) docker     (123)    39492 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/phone-codes/phone-codes.json
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/phone-codes/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.991985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ionslider/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.991985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ionslider/img/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ionslider/img/sprite-skin-flat.png
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ionslider/img/sprite-skin-nice.png
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.css
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinFlat.css
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinNice.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.991985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jQueryUI/
--rw-r--r--   0 runner    (1001) docker     (123)   470596 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jQueryUI/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)   240427 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jQueryUI/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.995985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/
--rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/core.js
--rw-r--r--   0 runner    (1001) docker     (123)   271751 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)    86927 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   132370 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/jquery.min.map
--rw-r--r--   0 runner    (1001) docker     (123)   218897 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/jquery.slim.js
--rw-r--r--   0 runner    (1001) docker     (123)    69917 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/jquery.slim.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   105346 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/jquery.slim.min.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.995985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jvectormap/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.css
--rw-r--r--   0 runner    (1001) docker     (123)    33323 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    95062 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-usa-en.js
--rw-r--r--   0 runner    (1001) docker     (123)   144313 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-world-mill-en.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.995985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/knob/
--rw-r--r--   0 runner    (1001) docker     (123)    26222 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/knob/jquery.knob.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.995985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/morris/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/morris/morris.css
--rw-r--r--   0 runner    (1001) docker     (123)    66046 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/morris/morris.js
--rw-r--r--   0 runner    (1001) docker     (123)    35652 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/morris/morris.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.995985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/pace/
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/pace/pace.css
--rw-r--r--   0 runner    (1001) docker     (123)    26566 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/pace/pace.js
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/pace/pace.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/pace/pace.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.999985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.999985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/esm/
--rw-r--r--   0 runner    (1001) docker     (123)    34601 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/esm/popper-utils.js
--rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/esm/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    84361 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/esm/popper.js
--rw-r--r--   0 runner    (1001) docker     (123)    20314 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/esm/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    32919 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/popper-utils.js
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    80829 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/popper.js
--rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.999985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/umd/
--rw-r--r--   0 runner    (1001) docker     (123)    35703 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/umd/popper-utils.js
--rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/umd/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    84615 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/umd/popper.js
--rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/umd/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:57.003985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:57.011985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/az.js
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/bg.js
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/cs.js
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/da.js
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/de.js
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/en.js
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/es.js
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/et.js
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/eu.js
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/fa.js
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/fi.js
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/fr.js
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/gl.js
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/he.js
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/hi.js
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/hr.js
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/hu.js
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/id.js
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/is.js
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/it.js
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/ko.js
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/lt.js
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/lv.js
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/mk.js
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/nb.js
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/nl.js
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/pl.js
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/pt.js
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/ro.js
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/ru.js
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/sk.js
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/sr.js
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/sv.js
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/th.js
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/tr.js
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/uk.js
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/vi.js
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/zh-CN.js
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/zh-TW.js
--rw-r--r--   0 runner    (1001) docker     (123)    17062 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/select2.css
--rw-r--r--   0 runner    (1001) docker     (123)   152250 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/select2.full.js
--rw-r--r--   0 runner    (1001) docker     (123)    71172 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/select2.full.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   132348 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/select2.js
--rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    62834 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/select2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:57.011985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/slimScroll/
--rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.js
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:57.011985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/sparkline/
--rw-r--r--   0 runner    (1001) docker     (123)   123446 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/sparkline/jquery.sparkline.js
--rw-r--r--   0 runner    (1001) docker     (123)    43247 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/sparkline/jquery.sparkline.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:57.011985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/timepicker/
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.css
--rw-r--r--   0 runner    (1001) docker     (123)    26014 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:57.015985 hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   186124 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   107656 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    62320 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    25236 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   397420 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150516 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:57.015985 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/a.html
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/admin-layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/admin.ht.old
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/donation.html
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/fake.html
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/flaskadmin-layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:57.015985 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/hiddify-flask-admin/
--rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/hiddify-flask-admin/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/lte-master.html
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/macros.html
--rw-r--r--   0 runner    (1001) docker     (123)    20817 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/master.html
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/templates/static.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.887985 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.887985 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:57.019985 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    56207 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)   153530 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.887985 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:57.019985 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    74896 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)   175386 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.887985 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:57.019985 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    57475 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)   151218 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.887985 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/zh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:57.019985 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    47481 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/zh/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)   146552 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/hiddifypanel/translations/zh/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:29:56.887985 hiddifypanel-8.0.0.dev7/hiddifypanel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 11:29:56.000000 hiddifypanel-8.0.0.dev7/hiddifypanel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38833 2023-08-03 11:29:56.000000 hiddifypanel-8.0.0.dev7/hiddifypanel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:29:56.000000 hiddifypanel-8.0.0.dev7/hiddifypanel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-03 11:29:56.000000 hiddifypanel-8.0.0.dev7/hiddifypanel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-03 11:29:56.000000 hiddifypanel-8.0.0.dev7/hiddifypanel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 11:29:56.000000 hiddifypanel-8.0.0.dev7/hiddifypanel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:29:57.019985 hiddifypanel-8.0.0.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-03 11:29:41.000000 hiddifypanel-8.0.0.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.109428 hiddifypanel-8.0.0.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    35103 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19807 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 12:15:28.109428 hiddifypanel-8.0.0.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.021426 hiddifypanel-8.0.0.dev8/hiddifypanel/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/Events.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.021426 hiddifypanel-8.0.0.dev8/hiddifypanel/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/drivers/abstract_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/drivers/singbox_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/drivers/ssh_liberty_bridge_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/drivers/user_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/drivers/xray_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.021426 hiddifypanel-8.0.0.dev8/hiddifypanel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/models/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/models/child.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/models/config_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/models/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/models/parent_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/models/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/models/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.025426 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.025426 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/Actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/AdminstratorAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/Backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/ChildAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/ConfigAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/Dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/DomainAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/ProxyAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/QuickSetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/SettingAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/Terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/UserAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/adminlte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/commercial_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.025426 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/a.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/backup.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/base2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/commercial_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/configfake.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/ltemaster.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.029426 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/model/admin_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/model/domain_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/model/user_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/parent_dash.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/proxy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/quick_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/result.html
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/cf_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/clean_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.029426 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/ParentDomainAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/ProxyDetailsAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.029426 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/restapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/restapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/restapi/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/restapi/tgbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/restapi/tgmsg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.029426 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/telegrambot/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/telegrambot/DefaultResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/telegrambot/Usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/telegrambot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/telegrambot/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/telegrambot/information.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.029426 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/templates/configc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/templates/parent_dash.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/custom_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25093 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/hiddify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/init_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.029426 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/link_maker.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19572 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/link_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.029426 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/all_configs copy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/all_configs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/clash_config copy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/clash_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/clash_proxies copy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/clash_proxies.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.033427 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/all-configs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/all-configs_old.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/android.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/base2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/clash-links copy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/clash-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/doh.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/index copy.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/index_old.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/ios copy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/ios.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/multi.html
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/speedtest.html
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/telegram.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/usage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/windows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/singbox_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.033427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/a.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.033427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)  1665614 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/adminlte.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/adminlte.fa.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/adminlte.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/bootstrap4-rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   163995 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/bootstrap5.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/custom-rtl.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)   101895 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)   278568 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/lte.old
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.037427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    92934 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Black.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    53500 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Black.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    42308 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Black.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    91810 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Bold.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    91644 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    52676 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    41856 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   101090 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Light.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   100920 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    59988 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Light.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    48616 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Light.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   107842 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Medium.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   107668 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    63312 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Medium.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    51256 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    90482 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Thin.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    90316 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    51884 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Thin.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    41344 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Thin.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    85354 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    85192 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    47972 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    38004 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.041427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/WhiteLogo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   103814 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   111125 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/hiddify-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37408 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/hiddify.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/no_back_hiddify.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/pwa-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.041427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/
+-rw-r--r--   0 runner    (1001) docker     (123)    75224 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/ipad_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85623 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/ipadpro1_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)   121021 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/ipadpro2_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90886 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/ipadpro3_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28231 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/iphone5_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/iphone6_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68643 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/iphoneplus_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    69743 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/iphonex_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45109 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/iphonexr_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80648 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/iphonexsmax_splash.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.045427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   104260 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/adminlte.js
+-rw-r--r--   0 runner    (1001) docker     (123)    49278 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/bootbox.all.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/bootbox.all.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    60406 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/custom-rtl.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/demo.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89764 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/jquery-3.6.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/js.cookie.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    51465 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/moment.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19032 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/pwa-sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/pwa.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33168 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/qrcode.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.017426 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.013426 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.045427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    37644 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28977 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   172839 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   140421 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.045427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   210612 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)    70808 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   122441 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)    58072 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.045427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap-slider/
+-rw-r--r--   0 runner    (1001) docker     (123)    36164 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap-slider/bootstrap-slider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap-slider/slider.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.045427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap-wysihtml5/
+-rw-r--r--   0 runner    (1001) docker     (123)   566620 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js
+-rw-r--r--   0 runner    (1001) docker     (123)   210932 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.017426 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap4-editable/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.045427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap4-editable/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    21490 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap4-editable/css/bootstrap-editable.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.049427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap4-editable/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap4-editable/img/clear.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap4-editable/img/loading.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.049427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap4-editable/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   225176 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.js
+-rw-r--r--   0 runner    (1001) docker     (123)    76077 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.049427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/chart.js/
+-rw-r--r--   0 runner    (1001) docker     (123)   535484 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/chart.js/Chart.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   211133 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/chart.js/Chart.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   403941 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/chart.js/Chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)   159638 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/chart.js/Chart.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.049427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/chartjs-old/
+-rw-r--r--   0 runner    (1001) docker     (123)   109613 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/chartjs-old/Chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52092 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/chartjs-old/Chart.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.049427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)   433051 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/ckeditor.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.053427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ar.js
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ast.js
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/bg.js
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/cs.js
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/da.js
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/de.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/el.js
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/en-au.js
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/eo.js
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/es.js
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/et.js
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/eu.js
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/fi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/fr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/gl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/gu.js
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/hr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/hu.js
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/it.js
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ja.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/km.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/kn.js
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ko.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ku.js
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/nb.js
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ne.js
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/nl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/oc.js
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/pl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/pt-br.js
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/pt.js
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ro.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ru.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/si.js
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/sk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/sq.js
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/sv.js
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/tr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/tt.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ug.js
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/uk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/zh-cn.js
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/zh.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.053427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.css
+-rw-r--r--   0 runner    (1001) docker     (123)    33831 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/img/alpha-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/img/alpha.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/img/hue-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/img/hue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/img/saturation.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.017426 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/AutoFill/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/AutoFill/Readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/dataTables.autoFill.css
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/dataTables.autoFill.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/filler.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    22645 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/License.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/dataTables.colReorder.css
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/dataTables.colReorder.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/insert.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    36311 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/License.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colvis.jqueryui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    27029 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/License.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.css
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.057427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    40932 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/Readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/dataTables.fixedHeader.css
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/dataTables.fixedHeader.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/KeyTable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/KeyTable/Readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/dataTables.keyTable.css
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/dataTables.keyTable.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    29477 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/License.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/responsive.bootstrap4.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    25098 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14589 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/responsive.bootstrap4.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/Readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.css
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/loading-background.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    37984 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls_hover.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.061427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    84578 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31850 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.065427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls.swf
+-rw-r--r--   0 runner    (1001) docker     (123)    58846 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls_pdf.swf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.065427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/images/sort_asc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/images/sort_asc_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/images/sort_both.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/images/sort_desc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/images/sort_desc_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/jquery.dataTables.css
+-rw-r--r--   0 runner    (1001) docker     (123)    86551 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/jquery.dataTables.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    86551 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/jquery.dataTables_themeroller.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.065427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/
+-rw-r--r--   0 runner    (1001) docker     (123)    46838 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/bootstrap-datepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33745 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/datepicker3.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.069427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ar.js
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.az.js
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.bg.js
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cs.js
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cy.js
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.da.js
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.de.js
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.el.js
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.es.js
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.et.js
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.gl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.he.js
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hu.js
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.id.js
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.is.js
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.it.js
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ja.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ka.js
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lt.js
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lv.js
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.mk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ms.js
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nb.js
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl-BE.js
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.no.js
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt.js
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ro.js
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs-latin.js
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs.js
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ru.js
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sq.js
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sv.js
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.th.js
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.tr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ua.js
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.vi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-CN.js
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-TW.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.069427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/daterangepicker/
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/daterangepicker/daterangepicker-bs3.css
+-rw-r--r--   0 runner    (1001) docker     (123)    53679 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/daterangepicker/daterangepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    99201 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/daterangepicker/moment.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34737 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/daterangepicker/moment.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.069427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fastclick/
+-rw-r--r--   0 runner    (1001) docker     (123)    25965 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fastclick/fastclick.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fastclick/fastclick.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.073428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/
+-rw-r--r--   0 runner    (1001) docker     (123)    41944 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/excanvas.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19314 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/excanvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.colorhelpers.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.colorhelpers.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.canvas.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.categories.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.categories.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.image.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.image.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   121627 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52300 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.navigate.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.navigate.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23635 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.pie.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12024 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.pie.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.resize.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.resize.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.selection.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.selection.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.stack.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.stack.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.symbol.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.symbol.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.threshold.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.threshold.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.time.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.time.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.017426 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.073428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21778 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.073428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   134808 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.073428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fullcalendar/
+-rw-r--r--   0 runner    (1001) docker     (123)    22515 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fullcalendar/fullcalendar.css
+-rw-r--r--   0 runner    (1001) docker     (123)   279259 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fullcalendar/fullcalendar.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    84823 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fullcalendar/fullcalendar.print.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.077427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/all.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.077427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/_all.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/aero.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/aero.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/blue.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/flat.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/flat.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/flat@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/green.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/green.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/grey.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/grey.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/orange.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/orange.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/pink.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/pink.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/purple.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/purple.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/red.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/red.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.077427 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/futurico/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/futurico/futurico.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/futurico/futurico.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/futurico/futurico@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/icheck.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/icheck.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.081428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/
+-rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/_all.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/aero.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/blue.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/green.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/grey.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/line.css
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/line.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/line@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/orange.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/pink.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/purple.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/red.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/yellow.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.085428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/_all.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/aero.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/aero.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/blue.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/green.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/green.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/grey.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/grey.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/minimal.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/minimal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/minimal@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/orange.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/orange.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/pink.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/pink.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/purple.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/purple.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/red.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/red.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.085428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/polaris/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/polaris/polaris.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/polaris/polaris.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/polaris/polaris@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.089428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/
+-rw-r--r--   0 runner    (1001) docker     (123)    15591 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/_all.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/aero.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/aero.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/blue.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/green.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/green.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/grey.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/grey.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/orange.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/orange.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/pink.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/pink.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/purple.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/purple.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/red.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/red.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/square.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/square.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/square@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.089428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/
+-rw-r--r--   0 runner    (1001) docker     (123)    22814 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/jquery.inputmask.date.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/jquery.inputmask.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (123)    90539 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/jquery.inputmask.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/jquery.inputmask.numeric.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/jquery.inputmask.phone.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/jquery.inputmask.regex.extensions.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.089428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/phone-codes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/phone-codes/phone-be.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39492 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/phone-codes/phone-codes.json
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/phone-codes/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.089428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ionslider/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.089428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ionslider/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ionslider/img/sprite-skin-flat.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ionslider/img/sprite-skin-nice.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinFlat.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinNice.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.089428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jQueryUI/
+-rw-r--r--   0 runner    (1001) docker     (123)   470596 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jQueryUI/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)   240427 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jQueryUI/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.093428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/core.js
+-rw-r--r--   0 runner    (1001) docker     (123)   271751 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86927 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   132370 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/jquery.min.map
+-rw-r--r--   0 runner    (1001) docker     (123)   218897 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/jquery.slim.js
+-rw-r--r--   0 runner    (1001) docker     (123)    69917 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/jquery.slim.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   105346 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/jquery.slim.min.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.093428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jvectormap/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.css
+-rw-r--r--   0 runner    (1001) docker     (123)    33323 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95062 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-usa-en.js
+-rw-r--r--   0 runner    (1001) docker     (123)   144313 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-world-mill-en.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.093428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/knob/
+-rw-r--r--   0 runner    (1001) docker     (123)    26222 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/knob/jquery.knob.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.093428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/morris/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/morris/morris.css
+-rw-r--r--   0 runner    (1001) docker     (123)    66046 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/morris/morris.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35652 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/morris/morris.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.093428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/pace/
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/pace/pace.css
+-rw-r--r--   0 runner    (1001) docker     (123)    26566 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/pace/pace.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/pace/pace.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/pace/pace.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.093428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.097428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/esm/
+-rw-r--r--   0 runner    (1001) docker     (123)    34601 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/esm/popper-utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/esm/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    84361 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/esm/popper.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20314 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/esm/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32919 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/popper-utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80829 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/popper.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.097428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/umd/
+-rw-r--r--   0 runner    (1001) docker     (123)    35703 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/umd/popper-utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/umd/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    84615 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/umd/popper.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/umd/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.097428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.101428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/az.js
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/bg.js
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/cs.js
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/da.js
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/de.js
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/en.js
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/es.js
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/et.js
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/eu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/fi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/fr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/gl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/he.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/hi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/hr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/hu.js
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/id.js
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/is.js
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/it.js
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/ko.js
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/lt.js
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/lv.js
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/mk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/nb.js
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/nl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/pl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/pt.js
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/ro.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/ru.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/sk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/sr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/sv.js
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/th.js
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/tr.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/uk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/vi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/zh-CN.js
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/zh-TW.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17062 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/select2.css
+-rw-r--r--   0 runner    (1001) docker     (123)   152250 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/select2.full.js
+-rw-r--r--   0 runner    (1001) docker     (123)    71172 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/select2.full.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   132348 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/select2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    62834 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/select2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.101428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/slimScroll/
+-rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.101428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/sparkline/
+-rw-r--r--   0 runner    (1001) docker     (123)   123446 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/sparkline/jquery.sparkline.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43247 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/sparkline/jquery.sparkline.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.101428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/timepicker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.css
+-rw-r--r--   0 runner    (1001) docker     (123)    26014 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.105428 hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   186124 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   107656 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    62320 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    25236 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   397420 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150516 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.105428 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/a.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/admin-layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/admin.ht.old
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/donation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/fake.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/flaskadmin-layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.105428 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/hiddify-flask-admin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/hiddify-flask-admin/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/lte-master.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20817 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/master.html
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/templates/static.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.021426 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.021426 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.105428 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    56207 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   153530 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.021426 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.105428 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    74896 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   175386 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.021426 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.105428 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    57475 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   151218 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.021426 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/zh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.105428 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    47481 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/zh/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   146552 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/hiddifypanel/translations/zh/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:15:28.021426 hiddifypanel-8.0.0.dev8/hiddifypanel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 12:15:27.000000 hiddifypanel-8.0.0.dev8/hiddifypanel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38833 2023-08-03 12:15:27.000000 hiddifypanel-8.0.0.dev8/hiddifypanel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:15:27.000000 hiddifypanel-8.0.0.dev8/hiddifypanel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-03 12:15:27.000000 hiddifypanel-8.0.0.dev8/hiddifypanel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-03 12:15:27.000000 hiddifypanel-8.0.0.dev8/hiddifypanel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 12:15:27.000000 hiddifypanel-8.0.0.dev8/hiddifypanel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:15:28.109428 hiddifypanel-8.0.0.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-03 12:15:11.000000 hiddifypanel-8.0.0.dev8/setup.py
```

### Comparing `hiddifypanel-8.0.0.dev7/HISTORY.md` & `hiddifypanel-8.0.0.dev8/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,28 @@
 
 * Add ssh server port. 
 
 * Add ssh user support. 
 
 #### Changes
 
+* Add restart on change ssh configs. 
+
+* Remove ssh key info. 
+
 * Disable caching. 
 
 #### Fix
 
+* Singbox. 
+
+* Bool. 
+
+* Remove client. 
+
 * Singbox error. 
 
 * Config issue. 
 
 * Bug. 
 
 * Bug.
```

### Comparing `hiddifypanel-8.0.0.dev7/LICENSE.md` & `hiddifypanel-8.0.0.dev8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/PKG-INFO` & `hiddifypanel-8.0.0.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiddifypanel
-Version: 8.0.0.dev7
+Version: 8.0.0.dev8
 Summary: hiddifypanel multi proxy panel
 Home-page: https://github.com/hiddify/hiddify-config/
 Author: hiddify
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `hiddifypanel-8.0.0.dev7/README.md` & `hiddifypanel-8.0.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/Events.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/Events.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/base.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/base.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/drivers/singbox_api.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/drivers/singbox_api.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/drivers/ssh_liberty_bridge_api.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/drivers/ssh_liberty_bridge_api.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/drivers/user_driver.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/drivers/user_driver.py`

 * *Files 25% similar despite different names*

```diff
@@ -24,7 +24,12 @@
         d += driver.get_enabled_users() or []
     return d
 
 
 def add_client(self, user):
     for driver in drivers:
         d += driver.add_client(user)
+
+
+def remove_client(self, user):
+    for driver in drivers:
+        d += driver.remove_client(user)
```

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/drivers/xray_api.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/drivers/xray_api.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/models/__init__.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/models/admin.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/models/admin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/models/child.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/models/child.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/models/config.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/models/config.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/models/config_enum.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/models/config_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,16 +139,16 @@
     @classmethod
     def _missing_(cls, value):
         return cls.not_found  # "key not found"
 
     def info(self):
         map = {
             self.ssh_server_redis_url: {'category': ConfigCategory.hidden},
-            self.ssh_server_port: {'category': ConfigCategory.ssh},
-            self.ssh_server_enable: {'category': ConfigCategory.ssh},
+            self.ssh_server_port: {'category': ConfigCategory.ssh, 'apply_mode': 'apply'},
+            self.ssh_server_enable: {'category': ConfigCategory.ssh, 'type': bool, 'apply_mode': 'apply'},
             self.core_type: {'category': ConfigCategory.advanced, 'apply_mode': 'apply'},
             self.dns_server: {'category': ConfigCategory.general, 'apply_mode': 'apply'},
             self.warp_enable: {'category': ConfigCategory.hidden, 'type': bool, 'apply_mode': 'restart'},
             self.warp_mode: {'category': ConfigCategory.warp, 'apply_mode': 'apply'},
             self.warp_plus_code: {'category': ConfigCategory.warp, 'apply_mode': 'apply'},
             self.restls1_2_domain: {'category': ConfigCategory.hidden},
             self.restls1_3_domain: {'category': ConfigCategory.hidden},
```

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/models/domain.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/models/domain.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/models/parent_domain.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/models/parent_domain.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/models/proxy.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/models/proxy.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/models/usage.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/models/usage.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/models/user.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/models/user.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/Actions.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/Actions.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/AdminstratorAdmin.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/AdminstratorAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/Backup.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/Backup.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/ChildAdmin.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/ChildAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/ConfigAdmin.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/ConfigAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/Dashboard.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/Dashboard.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/DomainAdmin.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/DomainAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/ProxyAdmin.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/ProxyAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/QuickSetup.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/QuickSetup.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/SettingAdmin.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/SettingAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/Terminal.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/Terminal.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/UserAdmin.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/UserAdmin.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     column_list = ["name", "UserLinks", "current_usage_GB", "remaining_days", "comment", 'last_online', 'mode', 'admin', "uuid"]
     form_extra_fields = {
         'reset_days': SwitchField(_("Reset package days")),
         'reset_usage': SwitchField(_("Reset package usage")),
         # 'disable_user': SwitchField(_("Disable User"))
     }
     list_template = 'model/user_list.html'
-    form_excluded_columns = ['monthly', 'telegram_id', 'last_online', 'expiry_time', 'last_reset_time', 'current_usage_GB', 'start_date', 'added_by', 'admin', 'details', 'max_ips']
+    form_excluded_columns = ['monthly', 'telegram_id', 'last_online', 'expiry_time', 'last_reset_time', 'current_usage_GB',
+                             'start_date', 'added_by', 'admin', 'details', 'max_ips', 'ed25519_private_key', 'ed25519_public_key']
     page_size = 50
     # edit_modal=True
     # create_modal=True
     # column_display_pk = True
     # can_export = True
     # form_overrides = dict(monthly=SwitchField)
     form_overrides = {
```

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/__init__.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/adminlte.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/adminlte.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/commercial_info.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/commercial_info.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/backup.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/backup.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/base.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/base.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/base2.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/base2.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/config.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/config.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/configfake.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/configfake.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/index.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/index.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/ltemaster.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/ltemaster.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/model/admin_list.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/model/admin_list.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/model/user_list.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/model/user_list.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/parent_dash.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/parent_dash.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/proxy.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/proxy.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/quick_setup.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/quick_setup.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin/templates/result.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin/templates/result.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/admin_2.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/admin_2.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/cf_api.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/cf_api.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/clean_ip.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/clean_ip.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/cli.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/cli.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/ParentDomainAdmin.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/ParentDomainAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/ProxyDetailsAdmin.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/ProxyDetailsAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/__init__.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/restapi/__init__.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/restapi/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/restapi/resources.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/restapi/resources.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/restapi/tgbot.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/restapi/tgbot.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/restapi/tgmsg.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/restapi/tgmsg.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/telegrambot/Usage.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/telegrambot/Usage.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/telegrambot/admin.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/telegrambot/admin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/telegrambot/information.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/telegrambot/information.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/templates/configc.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/templates/configc.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/commercial/templates/parent_dash.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/commercial/templates/parent_dash.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/common.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/common.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/custom_widgets.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/hiddify.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/hiddify.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/init_db.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/init_db.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/usage.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/usage.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/__init__.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/link_maker.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/link_maker.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/all_configs.txt` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/all_configs.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/clash_config copy.yml` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/clash_config copy.yml`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/clash_config.yml` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/clash_config.yml`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/clash_proxies copy.yml` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/clash_proxies copy.yml`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/clash_proxies.yml` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/clash_proxies.yml`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/all-configs.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/all-configs.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/all-configs_old.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/all-configs_old.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/android.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/android.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/base2.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/base2.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/clash-links copy.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/clash-links copy.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/clash-links.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/clash-links.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/index copy.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/index copy.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/index_old.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/index_old.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/ios copy.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/ios copy.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/ios.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/ios.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/multi.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/multi.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/speedtest.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/speedtest.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/telegram.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/telegram.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/usage.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/usage.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/home/windows.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/home/windows.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/templates/singbox_config.json` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/templates/singbox_config.json`

 * *Files 4% similar despite different names*

```diff
@@ -62,18 +62,18 @@
 			"sniff_override_destination": true
 		}
 	],
 	"outbounds": [
 		{
 			"type": "ssh",
 			"tag": "ssh-out",
-			"server": "$server_addr",
+			"server": "{{domains[0].domain}}",
 			"server_port": {{hconfigs[ConfigEnum.ssh_server_port]}},
 			"user": "{{user.uuid}}",
-			"private_key": "{{user.ed25519_private_key|replace('\n', '\\n')}}",
+			"private_key": "{{user.ed25519_private_key|replace('\n', '\\n')}}", #{{user.ed25519_public_key|replace('\n', '\\n')}}
 			"host_key": {{host_keys}},
 			"client_version": "{{ssh_client_version}}"
 		},
 		{
 			"type": "direct",
 			"tag": "direct-out"
 		},
```

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/panel/user/user.py` & `hiddifypanel-8.0.0.dev8/hiddifypanel/panel/user/user.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/a.txt` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/a.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/adminlte.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/adminlte.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/adminlte.fa.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/adminlte.fa.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/adminlte.rtl.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/adminlte.rtl.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/bootstrap.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/bootstrap4-rtl.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/bootstrap4-rtl.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/bootstrap5.rtl.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/bootstrap5.rtl.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/custom.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/font-awesome.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/css/lte.old` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/css/lte.old`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Black.eot` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Black.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Black.ttf` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Black.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Black.woff` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Black.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Black.woff2` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Black.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Bold.eot` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Bold.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Bold.ttf` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Bold.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Bold.woff` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Bold.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Bold.woff2` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Bold.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Light.eot` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Light.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Light.ttf` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Light.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Light.woff` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Light.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Light.woff2` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Light.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Medium.eot` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Medium.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Medium.ttf` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Medium.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Medium.woff` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Medium.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Medium.woff2` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Medium.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Thin.eot` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Thin.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Thin.ttf` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Thin.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Thin.woff` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Thin.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir-Thin.woff2` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir-Thin.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir.eot` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir.ttf` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir.woff` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/fonts/Vazir.woff2` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/fonts/Vazir.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/WhiteLogo.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/WhiteLogo.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/favicon.ico` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/hiddify-dark.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/hiddify-dark.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/hiddify.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/hiddify.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/no_back_hiddify.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/no_back_hiddify.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/pwa-icon.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/pwa-icon.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/ipad_splash.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/ipad_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/ipadpro1_splash.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/ipadpro1_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/ipadpro2_splash.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/ipadpro2_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/ipadpro3_splash.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/ipadpro3_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/iphone5_splash.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/iphone5_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/iphone6_splash.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/iphone6_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/iphoneplus_splash.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/iphoneplus_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/iphonex_splash.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/iphonex_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/iphonexr_splash.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/iphonexr_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/images/splash/iphonexsmax_splash.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/images/splash/iphonexsmax_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/adminlte.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/adminlte.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/bootbox.all.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/bootbox.all.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/bootbox.all.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/bootbox.all.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/bootstrap.bundle.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/bootstrap.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/custom-rtl.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/custom-rtl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/custom.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/custom.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/demo.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/demo.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/jquery-3.6.1.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/jquery-3.6.1.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/js.cookie.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/js.cookie.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/moment.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/moment.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/popper.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/pwa.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/pwa.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/js/qrcode.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/js/qrcode.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/css/bootstrap.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/css/bootstrap.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/js/bootstrap.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap/js/bootstrap.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap-slider/bootstrap-slider.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap-slider/bootstrap-slider.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap-slider/slider.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap-slider/slider.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap4-editable/css/bootstrap-editable.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap4-editable/css/bootstrap-editable.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap4-editable/img/loading.gif` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap4-editable/img/loading.gif`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/chart.js/Chart.bundle.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/chart.js/Chart.bundle.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/chart.js/Chart.bundle.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/chart.js/Chart.bundle.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/chart.js/Chart.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/chart.js/Chart.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/chart.js/Chart.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/chart.js/Chart.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/chartjs-old/Chart.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/chartjs-old/Chart.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/chartjs-old/Chart.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/chartjs-old/Chart.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/ckeditor.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/ckeditor.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ar.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ar.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ast.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ast.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/bg.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/bg.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/cs.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/cs.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/da.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/da.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/de.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/de.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/el.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/el.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/en-au.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/en-au.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/eo.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/eo.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/es.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/es.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/et.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/et.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/eu.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/eu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/fi.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/fi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/fr.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/fr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/gl.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/gl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/gu.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/gu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/hr.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/hr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/hu.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/hu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/it.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/it.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ja.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ja.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/km.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/km.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/kn.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/kn.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ko.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ko.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ku.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ku.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/nb.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/nb.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ne.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ne.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/nl.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/nl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/oc.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/oc.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/pl.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/pl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/pt-br.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/pt-br.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/pt.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/pt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ro.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ro.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ru.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ru.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/si.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/si.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/sk.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/sk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/sq.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/sq.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/sv.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/sv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/tr.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/tr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/tt.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/tt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/ug.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/ug.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/uk.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/uk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/zh-cn.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/zh-cn.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ckeditor/translations/zh.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ckeditor/translations/zh.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/img/alpha-horizontal.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/img/alpha-horizontal.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/img/alpha.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/img/alpha.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/img/hue-horizontal.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/img/hue-horizontal.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/img/hue.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/img/hue.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/colorpicker/img/saturation.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/colorpicker/img/saturation.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/AutoFill/Readme.txt` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/AutoFill/Readme.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/filler.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/filler.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/License.txt` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/License.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/Readme.md` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/Readme.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/insert.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/insert.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/License.txt` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/License.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/Readme.md` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/Readme.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colvis.jqueryui.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colvis.jqueryui.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/License.txt` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/License.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/Readme.md` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/Readme.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/Readme.txt` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/Readme.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/KeyTable/Readme.txt` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/KeyTable/Readme.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/License.txt` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/License.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.scss` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.scss`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/responsive.bootstrap4.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/responsive.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/responsive.bootstrap4.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/responsive.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/Readme.txt` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/Readme.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/loading-background.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/loading-background.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/Readme.md` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/Readme.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection_hover.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy_hover.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv_hover.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf_hover.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print_hover.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls_hover.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls.swf` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls.swf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls_pdf.swf` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls_pdf.swf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/jquery.dataTables.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/jquery.dataTables.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/jquery.dataTables.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datatables/jquery.dataTables_themeroller.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datatables/jquery.dataTables_themeroller.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/bootstrap-datepicker.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/datepicker3.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/datepicker3.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ar.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ar.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.az.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.az.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.bg.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.bg.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ca.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ca.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cs.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cs.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cy.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cy.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.da.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.da.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.de.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.de.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.el.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.el.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.es.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.es.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.et.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.et.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fa.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fa.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fi.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fr.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.gl.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.gl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.he.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.he.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hr.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hu.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.id.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.id.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.is.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.is.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.it.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.it.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ja.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ja.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ka.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ka.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kk.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kr.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lt.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lv.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.mk.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.mk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ms.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ms.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nb.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nb.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl-BE.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl-BE.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.no.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.no.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pl.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt-BR.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt-BR.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ro.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ro.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs-latin.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs-latin.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ru.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ru.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sk.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sl.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sq.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sq.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sv.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sw.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sw.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.th.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.th.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.tr.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.tr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ua.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ua.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.vi.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.vi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-CN.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-CN.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-TW.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-TW.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/daterangepicker/daterangepicker-bs3.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/daterangepicker/daterangepicker-bs3.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/daterangepicker/daterangepicker.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/daterangepicker/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/daterangepicker/moment.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/daterangepicker/moment.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/daterangepicker/moment.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/daterangepicker/moment.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fastclick/fastclick.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fastclick/fastclick.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fastclick/fastclick.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fastclick/fastclick.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/excanvas.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/excanvas.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/excanvas.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/excanvas.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.colorhelpers.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.colorhelpers.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.colorhelpers.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.colorhelpers.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.canvas.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.canvas.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.canvas.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.canvas.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.categories.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.categories.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.categories.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.categories.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.image.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.image.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.image.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.image.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.navigate.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.navigate.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.navigate.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.navigate.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.pie.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.pie.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.pie.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.pie.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.resize.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.resize.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.resize.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.resize.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.selection.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.selection.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.selection.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.selection.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.stack.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.stack.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.stack.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.stack.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.symbol.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.symbol.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.symbol.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.symbol.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.threshold.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.threshold.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.threshold.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.threshold.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.time.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.time.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/flot/jquery.flot.time.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/flot/jquery.flot.time.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css.map` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/css/font-awesome.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/fonts/FontAwesome.otf` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.eot` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.svg` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.ttf` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff2` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fullcalendar/fullcalendar.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fullcalendar/fullcalendar.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fullcalendar/fullcalendar.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fullcalendar/fullcalendar.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/fullcalendar/fullcalendar.print.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/fullcalendar/fullcalendar.print.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/all.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/_all.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/_all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/aero.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/aero.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/aero.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/aero.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/aero@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/aero@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/blue.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/blue.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/blue.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/blue.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/blue@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/blue@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/flat.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/flat.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/flat.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/flat.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/flat@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/flat@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/green.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/green.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/green.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/green.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/green@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/green@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/grey.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/grey.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/grey.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/grey.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/grey@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/grey@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/orange.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/orange.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/orange.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/orange.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/orange@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/orange@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/pink.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/pink.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/pink.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/pink.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/pink@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/pink@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/purple.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/purple.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/purple.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/purple.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/purple@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/purple@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/red.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/red.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/red.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/red.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/red@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/red@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/yellow.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/yellow.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/yellow.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/yellow.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/flat/yellow@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/flat/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/futurico/futurico.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/futurico/futurico.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/futurico/futurico.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/futurico/futurico.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/futurico/futurico@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/futurico/futurico@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/icheck.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/icheck.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/icheck.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/icheck.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/_all.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/_all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/aero.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/aero.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/blue.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/blue.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/green.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/green.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/grey.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/grey.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/line.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/line.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/line.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/line.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/line@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/line@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/orange.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/orange.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/pink.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/pink.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/purple.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/purple.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/red.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/red.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/line/yellow.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/line/yellow.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/_all.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/_all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/aero.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/aero.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/aero.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/aero.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/aero@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/aero@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/blue.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/blue.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/blue.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/blue.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/blue@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/blue@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/green.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/green.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/green.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/green.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/green@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/green@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/grey.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/grey.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/grey.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/grey.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/grey@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/grey@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/minimal.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/minimal.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/minimal.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/minimal.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/minimal@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/minimal@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/orange.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/orange.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/orange.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/orange.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/orange@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/orange@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/pink.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/pink.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/pink.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/pink.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/pink@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/pink@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/purple.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/purple.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/purple.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/purple.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/purple@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/purple@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/red.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/red.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/red.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/red.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/red@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/red@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/yellow.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/yellow.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/yellow.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/yellow.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/minimal/yellow@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/minimal/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/polaris/polaris.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/polaris/polaris.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/polaris/polaris.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/polaris/polaris.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/polaris/polaris@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/polaris/polaris@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/_all.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/_all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/aero.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/aero.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/aero.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/aero.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/aero@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/aero@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/blue.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/blue.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/blue.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/blue.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/blue@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/blue@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/green.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/green.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/green.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/green.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/green@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/green@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/grey.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/grey.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/grey.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/grey.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/grey@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/grey@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/orange.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/orange.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/orange.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/orange.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/orange@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/orange@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/pink.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/pink.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/pink.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/pink.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/pink@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/pink@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/purple.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/purple.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/purple.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/purple.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/purple@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/purple@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/red.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/red.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/red.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/red.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/red@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/red@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/square.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/square.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/square.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/square.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/square@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/square@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/yellow.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/yellow.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/yellow.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/yellow.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/iCheck/square/yellow@2x.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/iCheck/square/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/jquery.inputmask.date.extensions.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/jquery.inputmask.date.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/jquery.inputmask.extensions.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/jquery.inputmask.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/jquery.inputmask.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/jquery.inputmask.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/jquery.inputmask.numeric.extensions.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/jquery.inputmask.numeric.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/jquery.inputmask.phone.extensions.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/jquery.inputmask.phone.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/jquery.inputmask.regex.extensions.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/jquery.inputmask.regex.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/phone-codes/phone-be.json` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/phone-codes/phone-be.json`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/input-mask/phone-codes/phone-codes.json` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/input-mask/phone-codes/phone-codes.json`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ionslider/img/sprite-skin-nice.png` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ionslider/img/sprite-skin-nice.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinFlat.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinFlat.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinNice.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinNice.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jQueryUI/jquery-ui.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jQueryUI/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jQueryUI/jquery-ui.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jQueryUI/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/core.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/core.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/jquery.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/jquery.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/jquery.min.map` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/jquery.min.map`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/jquery.slim.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/jquery.slim.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/jquery.slim.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jquery/jquery.slim.min.map` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jquery/jquery.slim.min.map`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-usa-en.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-usa-en.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-world-mill-en.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-world-mill-en.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/knob/jquery.knob.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/knob/jquery.knob.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/morris/morris.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/morris/morris.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/morris/morris.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/morris/morris.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/pace/pace.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/pace/pace.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/pace/pace.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/pace/pace.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/pace/pace.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/pace/pace.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/pace/pace.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/pace/pace.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/esm/popper-utils.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/esm/popper-utils.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/esm/popper-utils.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/esm/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/esm/popper.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/esm/popper.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/esm/popper.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/esm/popper.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/popper-utils.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/popper-utils.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/popper-utils.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/popper.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/popper.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/popper.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/popper.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/umd/popper-utils.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/umd/popper-utils.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/umd/popper-utils.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/umd/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/umd/popper.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/umd/popper.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/popper/umd/popper.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/popper/umd/popper.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/az.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/az.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/bg.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/ca.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/cs.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/da.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/da.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/de.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/de.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/en.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/en.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/es.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/es.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/et.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/et.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/eu.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/fa.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/fi.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/fr.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/gl.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/he.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/he.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/hi.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/hr.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/hu.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/id.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/id.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/is.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/is.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/it.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/it.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/ko.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/lt.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/lv.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/mk.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/nb.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/nl.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/pl.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/pt-BR.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/pt.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/ro.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/ru.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/sk.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/sr.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/sv.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/th.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/th.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/tr.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/uk.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/vi.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/zh-CN.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/i18n/zh-TW.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/select2.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/select2.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/select2.full.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/select2.full.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/select2.full.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/select2.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/select2.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/select2.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/select2.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/select2/select2.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/select2/select2.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/sparkline/jquery.sparkline.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/sparkline/jquery.sparkline.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/sparkline/jquery.sparkline.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/sparkline/jquery.sparkline.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.css` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.js` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-brands-400.ttf` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-brands-400.woff2` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-regular-400.ttf` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-regular-400.woff2` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-solid-900.ttf` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-solid-900.woff2` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-v4compatibility.ttf` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/static/webfonts/fa-v4compatibility.woff2` & `hiddifypanel-8.0.0.dev8/hiddifypanel/static/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/templates/500.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/templates/500.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/templates/admin-layout.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/templates/admin-layout.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/templates/admin.ht.old` & `hiddifypanel-8.0.0.dev8/hiddifypanel/templates/admin.ht.old`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/templates/donation.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/templates/donation.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/templates/fake.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/templates/fake.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/templates/flaskadmin-layout.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/templates/flaskadmin-layout.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/templates/hiddify-flask-admin/list.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/templates/hiddify-flask-admin/list.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/templates/lte-master.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/templates/lte-master.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/templates/macros.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/templates/macros.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/templates/master.html` & `hiddifypanel-8.0.0.dev8/hiddifypanel/templates/master.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/translations/en/LC_MESSAGES/messages.mo` & `hiddifypanel-8.0.0.dev8/hiddifypanel/translations/en/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  HiddifyPanel\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-08-03 13:28+0200\n"
-"PO-Revision-Date: 2023-08-03 04:46-0500\n"
+"POT-Creation-Date: 2023-08-03 14:14+0200\n"
+"PO-Revision-Date: 2023-08-03 06:29-0500\n"
 "Last-Translator: hidden u\n"
 "Language: en_US\n"
 "Language-Team: English (USA)\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/translations/en/LC_MESSAGES/messages.po` & `hiddifypanel-8.0.0.dev8/hiddifypanel/translations/en/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: HiddifyPanel\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-08-03 13:28+0200\n"
-"PO-Revision-Date: 2023-08-03 04:46-0500\n"
+"POT-Creation-Date: 2023-08-03 14:14+0200\n"
+"PO-Revision-Date: 2023-08-03 06:29-0500\n"
 "Last-Translator: hidden u\n"
 "Language-Team: English (USA)\n"
 "Language: en_US\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
@@ -125,44 +125,44 @@
 msgid ""
 "Success! Please wait around 5 minutes to make sure everything is updated."
 msgstr ""
 "✔️ Success! Please Wait around 5 minutes to make sure everything is updated"
 
 # | msgid "Actions"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:56
-#: hiddifypanel/panel/admin/UserAdmin.py:71
+#: hiddifypanel/panel/admin/UserAdmin.py:72
 msgid "actions"
 msgstr "Actions"
 
 # | msgid "User Links"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:57
-#: hiddifypanel/panel/admin/UserAdmin.py:73
+#: hiddifypanel/panel/admin/UserAdmin.py:74
 msgid "user.user_links"
 msgstr "User Links"
 
 # | msgid "Name"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:58
-#: hiddifypanel/panel/admin/UserAdmin.py:72
+#: hiddifypanel/panel/admin/UserAdmin.py:73
 msgid "user.name"
 msgstr "Name"
 
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:59
-#: hiddifypanel/panel/admin/UserAdmin.py:76
+#: hiddifypanel/panel/admin/UserAdmin.py:77
 msgid "Mode"
 msgstr "Mode"
 
 # | msgid "UUID"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:60
-#: hiddifypanel/panel/admin/UserAdmin.py:82
+#: hiddifypanel/panel/admin/UserAdmin.py:83
 msgid "user.UUID"
 msgstr "UUID"
 
 # | msgid "📝 Note"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:61
-#: hiddifypanel/panel/admin/UserAdmin.py:83
+#: hiddifypanel/panel/admin/UserAdmin.py:84
 msgid "Note"
 msgstr "📝 Note"
 
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:62
 msgid "Max Active Users"
 msgstr "Max Active Users"
 
@@ -915,114 +915,114 @@
 
 # | msgid "⏳ Reset Package's Usage"
 #: hiddifypanel/panel/admin/UserAdmin.py:30
 msgid "Reset package usage"
 msgstr "⏳ Reset Package's Usage"
 
 # | msgid "⌛️ Usage Limit (GB)"
-#: hiddifypanel/panel/admin/UserAdmin.py:74
+#: hiddifypanel/panel/admin/UserAdmin.py:75
 msgid "user.usage_limit_GB"
 msgstr "⌛️ Usage Limit (GB)"
 
 # | msgid "Monthly"
-#: hiddifypanel/panel/admin/UserAdmin.py:75
+#: hiddifypanel/panel/admin/UserAdmin.py:76
 msgid "Reset every month"
 msgstr "Monthly"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:77
+#: hiddifypanel/panel/admin/UserAdmin.py:78
 msgid "Added by"
 msgstr "Added by"
 
 # | msgid "Current Usage (GB)"
-#: hiddifypanel/panel/admin/UserAdmin.py:78
+#: hiddifypanel/panel/admin/UserAdmin.py:79
 msgid "user.current_usage_GB"
 msgstr "Current Usage (GB)"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:79
+#: hiddifypanel/panel/admin/UserAdmin.py:80
 msgid "Start Date"
 msgstr "Start Date"
 
 # | msgid "Expire (Days)"
-#: hiddifypanel/panel/admin/UserAdmin.py:80
+#: hiddifypanel/panel/admin/UserAdmin.py:81
 msgid "user.expiry_time"
 msgstr "Expire (Days)"
 
 # | msgid "Last Usage Date Reset"
-#: hiddifypanel/panel/admin/UserAdmin.py:81
+#: hiddifypanel/panel/admin/UserAdmin.py:82
 msgid "user.last_reset_time"
 msgstr "Last Usage Date Reset"
 
 # | msgid "Last Connection"
-#: hiddifypanel/panel/admin/UserAdmin.py:84
+#: hiddifypanel/panel/admin/UserAdmin.py:85
 msgid "Last Online"
 msgstr "Last Connection"
 
 # | msgid "📆 Package Days"
-#: hiddifypanel/panel/admin/UserAdmin.py:85
+#: hiddifypanel/panel/admin/UserAdmin.py:86
 msgid "Package Days"
 msgstr "📆 Package Days"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:86
+#: hiddifypanel/panel/admin/UserAdmin.py:87
 msgid "Max IPs"
 msgstr "Max IPs"
 
 # | msgid "❇️ Enable"
-#: hiddifypanel/panel/admin/UserAdmin.py:87
+#: hiddifypanel/panel/admin/UserAdmin.py:88
 msgid "Enable"
 msgstr "❇️ Enable"
 
 # | msgid "You can add some text that Is only visible to you"
-#: hiddifypanel/panel/admin/UserAdmin.py:101
+#: hiddifypanel/panel/admin/UserAdmin.py:102
 msgid "Add some text that is only visible to you."
 msgstr "You can add some text that Is only visible to you"
 
 # | msgid ""
 # | "The user's Package Mode. should the usage reset every Month, Week, etc"
-#: hiddifypanel/panel/admin/UserAdmin.py:102
+#: hiddifypanel/panel/admin/UserAdmin.py:103
 msgid "Define the user mode. Should the usage reset every month?"
 msgstr ""
 "The user's Package Mode. should the usage reset every Month, Week, etc"
 
 # | msgid ""
 # | "If the monthly option is enabled, when this number reaches 30, the user "
 # | "usage will be reset (for weekly and daily this number is 7 and 1)"
-#: hiddifypanel/panel/admin/UserAdmin.py:103
+#: hiddifypanel/panel/admin/UserAdmin.py:104
 msgid ""
 "If monthly is enabled, the usage will be reset after 30 days from this date."
 msgstr ""
 "If the monthly option is enabled, when this number reaches 30, the user "
 "usage will be reset (for weekly and daily this number is 7 and 1)"
 
 # | msgid ""
 # | "Specify the starting date of the package. Leave empty to start from first
 # "
 # | "Connection."
-#: hiddifypanel/panel/admin/UserAdmin.py:104
+#: hiddifypanel/panel/admin/UserAdmin.py:105
 msgid ""
 "From when the user package will be started? Empty for start from first "
 "connection"
 msgstr ""
 "Specify the starting date of the package. Leave empty to start from first "
 "Connection."
 
 # | msgid "How Many Days Is This Package?"
-#: hiddifypanel/panel/admin/UserAdmin.py:105
+#: hiddifypanel/panel/admin/UserAdmin.py:106
 msgid "How many days this package should be available?"
 msgstr "How Many Days Is This Package?"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:207
+#: hiddifypanel/panel/admin/UserAdmin.py:208
 msgid "Package not started yet."
 msgstr "Package not started yet."
 
 # | msgid "Package Ends"
-#: hiddifypanel/panel/admin/UserAdmin.py:214
+#: hiddifypanel/panel/admin/UserAdmin.py:215
 msgid "Remaining: "
 msgstr "Package Ends"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:251
+#: hiddifypanel/panel/admin/UserAdmin.py:252
 #, python-format
 msgid ""
 "You have too much users! You can have only %(active)s active users and "
 "%(total)s users"
 msgstr ""
 "You have too much users! You can have only %(active)s active users and "
 "%(total)s users"
```

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/translations/fa/LC_MESSAGES/messages.mo` & `hiddifypanel-8.0.0.dev8/hiddifypanel/translations/fa/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  HiddifyPanel\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-08-03 13:28+0200\n"
-"PO-Revision-Date: 2023-08-03 04:46-0500\n"
+"POT-Creation-Date: 2023-08-03 14:14+0200\n"
+"PO-Revision-Date: 2023-08-03 06:29-0500\n"
 "Last-Translator: hidden u\n"
 "Language: fa\n"
 "Language-Team: Persian\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/translations/fa/LC_MESSAGES/messages.po` & `hiddifypanel-8.0.0.dev8/hiddifypanel/translations/fa/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 msgid ""
 msgstr ""
 "Project-Id-Version:  HiddifyPanel\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-08-03 13:28+0200\n"
-"PO-Revision-Date: 2023-08-03 04:46-0500\n"
+"POT-Creation-Date: 2023-08-03 14:14+0200\n"
+"PO-Revision-Date: 2023-08-03 06:29-0500\n"
 "Last-Translator: hidden u\n"
 "Language: fa\n"
 "Language-Team: Persian\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -127,44 +127,44 @@
 msgid "Success! Please wait around 5 minutes to make sure everything is updated."
 msgstr ""
 "✔️ موفقیت آمیز بود! لطفا برای اینکه مطمئن شوید بروزرسانی‌ها به درستی "
 "اعمال شده، حدود 5 دقیقه صبر کنید."
 
 # | msgid "Actions"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:56
-#: hiddifypanel/panel/admin/UserAdmin.py:71
+#: hiddifypanel/panel/admin/UserAdmin.py:72
 msgid "actions"
 msgstr "عملیات"
 
 # | msgid "User Links"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:57
-#: hiddifypanel/panel/admin/UserAdmin.py:73
+#: hiddifypanel/panel/admin/UserAdmin.py:74
 msgid "user.user_links"
 msgstr "لینک‌های کاربر"
 
 # | msgid "Name"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:58
-#: hiddifypanel/panel/admin/UserAdmin.py:72
+#: hiddifypanel/panel/admin/UserAdmin.py:73
 msgid "user.name"
 msgstr "نام"
 
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:59
-#: hiddifypanel/panel/admin/UserAdmin.py:76
+#: hiddifypanel/panel/admin/UserAdmin.py:77
 msgid "Mode"
 msgstr "حالت کاربر"
 
 # | msgid "UUID"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:60
-#: hiddifypanel/panel/admin/UserAdmin.py:82
+#: hiddifypanel/panel/admin/UserAdmin.py:83
 msgid "user.UUID"
 msgstr "UUID"
 
 # | msgid "📝 Note"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:61
-#: hiddifypanel/panel/admin/UserAdmin.py:83
+#: hiddifypanel/panel/admin/UserAdmin.py:84
 msgid "Note"
 msgstr "📝 یادداشت"
 
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:62
 #, fuzzy
 msgid "Max Active Users"
 msgstr "حداکثر کاربران فعال"
@@ -930,118 +930,118 @@
 
 # | msgid "⏳ Reset Package's Usage"
 #: hiddifypanel/panel/admin/UserAdmin.py:30
 msgid "Reset package usage"
 msgstr "⏳ ریست حجم مصرفی کاربر"
 
 # | msgid "⌛️ Usage Limit (GB)"
-#: hiddifypanel/panel/admin/UserAdmin.py:74
+#: hiddifypanel/panel/admin/UserAdmin.py:75
 msgid "user.usage_limit_GB"
 msgstr "⌛️ محدودیت حجم (گیگابایت)"
 
 # | msgid "Monthly"
-#: hiddifypanel/panel/admin/UserAdmin.py:75
+#: hiddifypanel/panel/admin/UserAdmin.py:76
 msgid "Reset every month"
 msgstr "ماهانه"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:77
+#: hiddifypanel/panel/admin/UserAdmin.py:78
 #, fuzzy
 msgid "Added by"
 msgstr "اضافه شده توسط"
 
 # | msgid "Current Usage (GB)"
-#: hiddifypanel/panel/admin/UserAdmin.py:78
+#: hiddifypanel/panel/admin/UserAdmin.py:79
 msgid "user.current_usage_GB"
 msgstr "حجم مصرفی (گیگابایت)"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:79
+#: hiddifypanel/panel/admin/UserAdmin.py:80
 msgid "Start Date"
 msgstr "زمان شروع"
 
 # | msgid "Expire (Days)"
-#: hiddifypanel/panel/admin/UserAdmin.py:80
+#: hiddifypanel/panel/admin/UserAdmin.py:81
 msgid "user.expiry_time"
 msgstr "انقضا (روز)"
 
 # | msgid "Last Usage Date Reset"
-#: hiddifypanel/panel/admin/UserAdmin.py:81
+#: hiddifypanel/panel/admin/UserAdmin.py:82
 msgid "user.last_reset_time"
 msgstr "آخرین زمان ریست شدن حجم (روز پیش)"
 
 # | msgid "Last Connection"
-#: hiddifypanel/panel/admin/UserAdmin.py:84
+#: hiddifypanel/panel/admin/UserAdmin.py:85
 msgid "Last Online"
 msgstr "آخرین اتصال"
 
 # | msgid "📆 Package Days"
-#: hiddifypanel/panel/admin/UserAdmin.py:85
+#: hiddifypanel/panel/admin/UserAdmin.py:86
 msgid "Package Days"
 msgstr "📆 تعداد روز بسته"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:86
+#: hiddifypanel/panel/admin/UserAdmin.py:87
 #, fuzzy
 msgid "Max IPs"
 msgstr "حداکثر IP"
 
 # | msgid "❇️ Enable"
-#: hiddifypanel/panel/admin/UserAdmin.py:87
+#: hiddifypanel/panel/admin/UserAdmin.py:88
 msgid "Enable"
 msgstr "❇️ فعال"
 
 # | msgid "You can add some text that Is only visible to you"
-#: hiddifypanel/panel/admin/UserAdmin.py:101
+#: hiddifypanel/panel/admin/UserAdmin.py:102
 msgid "Add some text that is only visible to you."
 msgstr ""
 "در این قسمت یادداشتی اضافه کنید. (این یادداشت فقط برای شما قابل نمایش "
 "است.)"
 
 # | msgid ""
 # | "The user's Package Mode. should the usage reset every Month, Week, etc"
-#: hiddifypanel/panel/admin/UserAdmin.py:102
+#: hiddifypanel/panel/admin/UserAdmin.py:103
 msgid "Define the user mode. Should the usage reset every month?"
 msgstr ""
 "حالت کاربر را تعریف کنید. کاربر غیرفعال (Disable) یا ریست حجم کاربر را "
 "مشخص کنید: (عدم ریست، ماهانه، هفتگی یا روزانه)"
 
 # | msgid ""
 # | "If the monthly option is enabled, when this number reaches 30, the user "
 # | "usage will be reset (for weekly and daily this number is 7 and 1)"
-#: hiddifypanel/panel/admin/UserAdmin.py:103
+#: hiddifypanel/panel/admin/UserAdmin.py:104
 msgid ""
 "If monthly is enabled, the usage will be reset after 30 days from this "
 "date."
 msgstr ""
 "اگر گزینه ماهانه فعال باشد، وقتی این عدد به ۳۰ برسد حجم کاربر ریست می‌شود"
 " (برای هفتگی و روزانه این عدد ۷ و ۱ است)"
 
 # | msgid ""
 # | "Specify the starting date of the package. Leave empty to start from first
 # "
 # | "Connection."
-#: hiddifypanel/panel/admin/UserAdmin.py:104
+#: hiddifypanel/panel/admin/UserAdmin.py:105
 msgid ""
 "From when the user package will be started? Empty for start from first "
 "connection"
 msgstr "از چه زمانی پکیج کاربر محاسبه شود؟ برای محاسبه از اولین اتصال خالی بگذارید"
 
 # | msgid "How Many Days Is This Package?"
-#: hiddifypanel/panel/admin/UserAdmin.py:105
+#: hiddifypanel/panel/admin/UserAdmin.py:106
 msgid "How many days this package should be available?"
 msgstr "این بسته چند روزه است؟"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:207
+#: hiddifypanel/panel/admin/UserAdmin.py:208
 msgid "Package not started yet."
 msgstr "بسته هنوز شروع نشده است."
 
 # | msgid "Package Ends"
-#: hiddifypanel/panel/admin/UserAdmin.py:214
+#: hiddifypanel/panel/admin/UserAdmin.py:215
 msgid "Remaining: "
 msgstr "زمان پایان بسته"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:251
+#: hiddifypanel/panel/admin/UserAdmin.py:252
 #, fuzzy, python-format
 msgid ""
 "You have too much users! You can have only %(active)s active users and "
 "%(total)s users"
 msgstr ""
 "شما کاربران زیادی دارید! شما می توانید تنها %(active)s کاربر فعال و "
 "%(total)s کاربر داشته باشید"
```

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/translations/pt/LC_MESSAGES/messages.mo` & `hiddifypanel-8.0.0.dev8/hiddifypanel/translations/pt/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  HiddifyPT\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-08-03 13:28+0200\n"
-"PO-Revision-Date: 2023-08-03 04:46-0500\n"
+"POT-Creation-Date: 2023-08-03 14:14+0200\n"
+"PO-Revision-Date: 2023-08-03 06:29-0500\n"
 "Last-Translator: lymanrudni\n"
 "Language: pt\n"
 "Language-Team: Portuguese\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/translations/pt/LC_MESSAGES/messages.po` & `hiddifypanel-8.0.0.dev8/hiddifypanel/translations/pt/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 msgid ""
 msgstr ""
 "Project-Id-Version:  HiddifyPT\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-08-03 13:28+0200\n"
-"PO-Revision-Date: 2023-08-03 04:46-0500\n"
+"POT-Creation-Date: 2023-08-03 14:14+0200\n"
+"PO-Revision-Date: 2023-08-03 06:29-0500\n"
 "Last-Translator: lymanrudni\n"
 "Language: pt\n"
 "Language-Team: Portuguese\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -141,48 +141,48 @@
 msgid "Success! Please wait around 5 minutes to make sure everything is updated."
 msgstr ""
 "✔️ Sucesso! Aguarde cerca de 5 minutos para garantir que tudo esteja "
 "atualizado"
 
 # | msgid "Actions"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:56
-#: hiddifypanel/panel/admin/UserAdmin.py:71
+#: hiddifypanel/panel/admin/UserAdmin.py:72
 #, fuzzy
 msgid "actions"
 msgstr "Ações"
 
 # | msgid "User Links"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:57
-#: hiddifypanel/panel/admin/UserAdmin.py:73
+#: hiddifypanel/panel/admin/UserAdmin.py:74
 #, fuzzy
 msgid "user.user_links"
 msgstr "Links de usuário"
 
 # | msgid "Name"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:58
-#: hiddifypanel/panel/admin/UserAdmin.py:72
+#: hiddifypanel/panel/admin/UserAdmin.py:73
 #, fuzzy
 msgid "user.name"
 msgstr "Nome"
 
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:59
-#: hiddifypanel/panel/admin/UserAdmin.py:76
+#: hiddifypanel/panel/admin/UserAdmin.py:77
 #, fuzzy
 msgid "Mode"
 msgstr "Modo"
 
 # | msgid "UUID"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:60
-#: hiddifypanel/panel/admin/UserAdmin.py:82
+#: hiddifypanel/panel/admin/UserAdmin.py:83
 msgid "user.UUID"
 msgstr "UUID"
 
 # | msgid "📝 Note"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:61
-#: hiddifypanel/panel/admin/UserAdmin.py:83
+#: hiddifypanel/panel/admin/UserAdmin.py:84
 #, fuzzy
 msgid "Note"
 msgstr "📝 Observação"
 
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:62
 #, fuzzy
 msgid "Max Active Users"
@@ -1027,129 +1027,129 @@
 # | msgid "⏳ Reset Package's Usage"
 #: hiddifypanel/panel/admin/UserAdmin.py:30
 #, fuzzy
 msgid "Reset package usage"
 msgstr "⏳ Redefinir o uso do pacote"
 
 # | msgid "⌛️ Usage Limit (GB)"
-#: hiddifypanel/panel/admin/UserAdmin.py:74
+#: hiddifypanel/panel/admin/UserAdmin.py:75
 #, fuzzy
 msgid "user.usage_limit_GB"
 msgstr "Limite de uso (GB)"
 
 # | msgid "Monthly"
-#: hiddifypanel/panel/admin/UserAdmin.py:75
+#: hiddifypanel/panel/admin/UserAdmin.py:76
 #, fuzzy
 msgid "Reset every month"
 msgstr "Por mês"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:77
+#: hiddifypanel/panel/admin/UserAdmin.py:78
 #, fuzzy
 msgid "Added by"
 msgstr "Adicionado por"
 
 # | msgid "Current Usage (GB)"
-#: hiddifypanel/panel/admin/UserAdmin.py:78
+#: hiddifypanel/panel/admin/UserAdmin.py:79
 #, fuzzy
 msgid "user.current_usage_GB"
 msgstr "Uso atual (GB)"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:79
+#: hiddifypanel/panel/admin/UserAdmin.py:80
 #, fuzzy
 msgid "Start Date"
 msgstr "Data de início"
 
 # | msgid "Expire (Days)"
-#: hiddifypanel/panel/admin/UserAdmin.py:80
+#: hiddifypanel/panel/admin/UserAdmin.py:81
 #, fuzzy
 msgid "user.expiry_time"
 msgstr "Expiração (dias)"
 
 # | msgid "Last Usage Date Reset"
-#: hiddifypanel/panel/admin/UserAdmin.py:81
+#: hiddifypanel/panel/admin/UserAdmin.py:82
 msgid "user.last_reset_time"
 msgstr "Redefinir para a última vez que ouve uso."
 
 # | msgid "Last Connection"
-#: hiddifypanel/panel/admin/UserAdmin.py:84
+#: hiddifypanel/panel/admin/UserAdmin.py:85
 msgid "Last Online"
 msgstr "Última vez online"
 
 # | msgid "📆 Package Days"
-#: hiddifypanel/panel/admin/UserAdmin.py:85
+#: hiddifypanel/panel/admin/UserAdmin.py:86
 msgid "Package Days"
 msgstr "Dias do pacote"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:86
+#: hiddifypanel/panel/admin/UserAdmin.py:87
 msgid "Max IPs"
 msgstr "Máximo de IPs"
 
 # | msgid "❇️ Enable"
-#: hiddifypanel/panel/admin/UserAdmin.py:87
+#: hiddifypanel/panel/admin/UserAdmin.py:88
 #, fuzzy
 msgid "Enable"
 msgstr "Habilitar"
 
 # | msgid "You can add some text that Is only visible to you"
-#: hiddifypanel/panel/admin/UserAdmin.py:101
+#: hiddifypanel/panel/admin/UserAdmin.py:102
 #, fuzzy
 msgid "Add some text that is only visible to you."
 msgstr "Você pode adicionar algum texto, será visível apenas para voce"
 
 # | msgid ""
 # | "The user's Package Mode. should the usage reset every Month, Week, etc"
-#: hiddifypanel/panel/admin/UserAdmin.py:102
+#: hiddifypanel/panel/admin/UserAdmin.py:103
 #, fuzzy
 msgid "Define the user mode. Should the usage reset every month?"
 msgstr ""
 "O modo de pacote do usuário. o uso deve ser redefinido a cada mês, semana"
 " etc."
 
 # | msgid ""
 # | "If the monthly option is enabled, when this number reaches 30, the user "
 # | "usage will be reset (for weekly and daily this number is 7 and 1)"
-#: hiddifypanel/panel/admin/UserAdmin.py:103
+#: hiddifypanel/panel/admin/UserAdmin.py:104
 msgid ""
 "If monthly is enabled, the usage will be reset after 30 days from this "
 "date."
 msgstr ""
 "Se a opção mensal estiver habilitada, quando esse número chegar a 30, o "
 "uso do usuário será zerado! (para semanal, e diário o número será  7 e 1)"
 
 # | msgid ""
 # | "Specify the starting date of the package. Leave empty to start from first
 # "
 # | "Connection."
-#: hiddifypanel/panel/admin/UserAdmin.py:104
+#: hiddifypanel/panel/admin/UserAdmin.py:105
 #, fuzzy
 msgid ""
 "From when the user package will be started? Empty for start from first "
 "connection"
 msgstr ""
 "Especifique a data de início do pacote. Deixe em branco para começar a "
 "partir da primeira conexão."
 
 # | msgid "How Many Days Is This Package?"
-#: hiddifypanel/panel/admin/UserAdmin.py:105
+#: hiddifypanel/panel/admin/UserAdmin.py:106
 #, fuzzy
 msgid "How many days this package should be available?"
 msgstr "Quantos dias é este pacote?"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:207
+#: hiddifypanel/panel/admin/UserAdmin.py:208
 #, fuzzy
 msgid "Package not started yet."
 msgstr "Pacote ainda não iniciado."
 
 # | msgid "Package Ends"
-#: hiddifypanel/panel/admin/UserAdmin.py:214
+#: hiddifypanel/panel/admin/UserAdmin.py:215
 #, fuzzy
 msgid "Remaining: "
 msgstr "O pacote termina em"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:251
+#: hiddifypanel/panel/admin/UserAdmin.py:252
 #, fuzzy, python-format
 msgid ""
 "You have too much users! You can have only %(active)s active users and "
 "%(total)s users"
 msgstr ""
 "Você tem muitos usuários! Você pode ter apenas %(active)s usuários ativos"
 " e %(total)s usuários"
```

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/translations/zh/LC_MESSAGES/messages.mo` & `hiddifypanel-8.0.0.dev8/hiddifypanel/translations/zh/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  HiddifyPanel\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-08-03 13:28+0200\n"
-"PO-Revision-Date: 2023-08-03 04:46-0500\n"
+"POT-Creation-Date: 2023-08-03 14:14+0200\n"
+"PO-Revision-Date: 2023-08-03 06:29-0500\n"
 "Last-Translator: hidden u\n"
 "Language: zh\n"
 "Language-Team: Chinese\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel/translations/zh/LC_MESSAGES/messages.po` & `hiddifypanel-8.0.0.dev8/hiddifypanel/translations/zh/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 msgid ""
 msgstr ""
 "Project-Id-Version:  HiddifyPanel\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-08-03 13:28+0200\n"
-"PO-Revision-Date: 2023-08-03 04:46-0500\n"
+"POT-Creation-Date: 2023-08-03 14:14+0200\n"
+"PO-Revision-Date: 2023-08-03 06:29-0500\n"
 "Last-Translator: hidden u\n"
 "Language: zh\n"
 "Language-Team: Chinese\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -124,45 +124,45 @@
 # updated"
 #: hiddifypanel/panel/admin/Actions.py:193
 msgid "Success! Please wait around 5 minutes to make sure everything is updated."
 msgstr "成功！ 请等待大约 5 分钟，以确保所有内容都已更新。"
 
 # | msgid "Actions"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:56
-#: hiddifypanel/panel/admin/UserAdmin.py:71
+#: hiddifypanel/panel/admin/UserAdmin.py:72
 msgid "actions"
 msgstr "动作"
 
 # | msgid "User Links"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:57
-#: hiddifypanel/panel/admin/UserAdmin.py:73
+#: hiddifypanel/panel/admin/UserAdmin.py:74
 msgid "user.user_links"
 msgstr "用户链接"
 
 # | msgid "Name"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:58
-#: hiddifypanel/panel/admin/UserAdmin.py:72
+#: hiddifypanel/panel/admin/UserAdmin.py:73
 msgid "user.name"
 msgstr "名称"
 
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:59
-#: hiddifypanel/panel/admin/UserAdmin.py:76
+#: hiddifypanel/panel/admin/UserAdmin.py:77
 #, fuzzy
 msgid "Mode"
 msgstr "模式"
 
 # | msgid "UUID"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:60
-#: hiddifypanel/panel/admin/UserAdmin.py:82
+#: hiddifypanel/panel/admin/UserAdmin.py:83
 msgid "user.UUID"
 msgstr "UUID"
 
 # | msgid "📝 Note"
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:61
-#: hiddifypanel/panel/admin/UserAdmin.py:83
+#: hiddifypanel/panel/admin/UserAdmin.py:84
 #, fuzzy
 msgid "Note"
 msgstr "笔记"
 
 #: hiddifypanel/panel/admin/AdminstratorAdmin.py:62
 #, fuzzy
 msgid "Max Active Users"
@@ -915,123 +915,123 @@
 # | msgid "⏳ Reset Package's Usage"
 #: hiddifypanel/panel/admin/UserAdmin.py:30
 #, fuzzy
 msgid "Reset package usage"
 msgstr "重置包的使用。"
 
 # | msgid "⌛️ Usage Limit (GB)"
-#: hiddifypanel/panel/admin/UserAdmin.py:74
+#: hiddifypanel/panel/admin/UserAdmin.py:75
 msgid "user.usage_limit_GB"
 msgstr "使用限制 (GB)"
 
 # | msgid "Monthly"
-#: hiddifypanel/panel/admin/UserAdmin.py:75
+#: hiddifypanel/panel/admin/UserAdmin.py:76
 msgid "Reset every month"
 msgstr "每月"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:77
+#: hiddifypanel/panel/admin/UserAdmin.py:78
 #, fuzzy
 msgid "Added by"
 msgstr "添加者"
 
 # | msgid "Current Usage (GB)"
-#: hiddifypanel/panel/admin/UserAdmin.py:78
+#: hiddifypanel/panel/admin/UserAdmin.py:79
 msgid "user.current_usage_GB"
 msgstr "当前使用量 (GB)"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:79
+#: hiddifypanel/panel/admin/UserAdmin.py:80
 #, fuzzy
 msgid "Start Date"
 msgstr "开始日期"
 
 # | msgid "Expire (Days)"
-#: hiddifypanel/panel/admin/UserAdmin.py:80
+#: hiddifypanel/panel/admin/UserAdmin.py:81
 msgid "user.expiry_time"
 msgstr "过期时间"
 
 # | msgid "Last Usage Date Reset"
-#: hiddifypanel/panel/admin/UserAdmin.py:81
+#: hiddifypanel/panel/admin/UserAdmin.py:82
 msgid "user.last_reset_time"
 msgstr "最后使用日期重置"
 
 # | msgid "Last Connection"
-#: hiddifypanel/panel/admin/UserAdmin.py:84
+#: hiddifypanel/panel/admin/UserAdmin.py:85
 #, fuzzy
 msgid "Last Online"
 msgstr "最后上线"
 
 # | msgid "📆 Package Days"
-#: hiddifypanel/panel/admin/UserAdmin.py:85
+#: hiddifypanel/panel/admin/UserAdmin.py:86
 #, fuzzy
 msgid "Package Days"
 msgstr "包天"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:86
+#: hiddifypanel/panel/admin/UserAdmin.py:87
 #, fuzzy
 msgid "Max IPs"
 msgstr "最大 IP"
 
 # | msgid "❇️ Enable"
-#: hiddifypanel/panel/admin/UserAdmin.py:87
+#: hiddifypanel/panel/admin/UserAdmin.py:88
 #, fuzzy
 msgid "Enable"
 msgstr "使能够"
 
 # | msgid "You can add some text that Is only visible to you"
-#: hiddifypanel/panel/admin/UserAdmin.py:101
+#: hiddifypanel/panel/admin/UserAdmin.py:102
 #, fuzzy
 msgid "Add some text that is only visible to you."
 msgstr "添加一些仅对您可见的文本。"
 
 # | msgid ""
 # | "The user's Package Mode. should the usage reset every Month, Week, etc"
-#: hiddifypanel/panel/admin/UserAdmin.py:102
+#: hiddifypanel/panel/admin/UserAdmin.py:103
 #, fuzzy
 msgid "Define the user mode. Should the usage reset every month?"
 msgstr "定义用户模式。应该每个月重置使用量吗？"
 
 # | msgid ""
 # | "If the monthly option is enabled, when this number reaches 30, the user "
 # | "usage will be reset (for weekly and daily this number is 7 and 1)"
-#: hiddifypanel/panel/admin/UserAdmin.py:103
+#: hiddifypanel/panel/admin/UserAdmin.py:104
 #, fuzzy
 msgid ""
 "If monthly is enabled, the usage will be reset after 30 days from this "
 "date."
 msgstr "如果启用每月选项，当这个数字达到 30 时，用户使用量将被重置（每周和每天这个数字是 7 和 1）"
 
 # | msgid ""
 # | "Specify the starting date of the package. Leave empty to start from first
 # "
 # | "Connection."
-#: hiddifypanel/panel/admin/UserAdmin.py:104
+#: hiddifypanel/panel/admin/UserAdmin.py:105
 #, fuzzy
 msgid ""
 "From when the user package will be started? Empty for start from first "
 "connection"
 msgstr "指定包的开始日期。留空以从第一个连接开始。"
 
 # | msgid "How Many Days Is This Package?"
-#: hiddifypanel/panel/admin/UserAdmin.py:105
+#: hiddifypanel/panel/admin/UserAdmin.py:106
 #, fuzzy
 msgid "How many days this package should be available?"
 msgstr "这个包裹有多少天？"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:207
+#: hiddifypanel/panel/admin/UserAdmin.py:208
 #, fuzzy
 msgid "Package not started yet."
 msgstr "套餐还没有开始。"
 
 # | msgid "Package Ends"
-#: hiddifypanel/panel/admin/UserAdmin.py:214
+#: hiddifypanel/panel/admin/UserAdmin.py:215
 #, fuzzy
 msgid "Remaining: "
 msgstr "包结束于"
 
-#: hiddifypanel/panel/admin/UserAdmin.py:251
+#: hiddifypanel/panel/admin/UserAdmin.py:252
 #, fuzzy, python-format
 msgid ""
 "You have too much users! You can have only %(active)s active users and "
 "%(total)s users"
 msgstr "你的用户太多了！您只能有 %(active)s 个活跃用户和 %(total)s 个用户"
 
 #: hiddifypanel/panel/admin/templates/backup.html:9
```

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel.egg-info/PKG-INFO` & `hiddifypanel-8.0.0.dev8/hiddifypanel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiddifypanel
-Version: 8.0.0.dev7
+Version: 8.0.0.dev8
 Summary: hiddifypanel multi proxy panel
 Home-page: https://github.com/hiddify/hiddify-config/
 Author: hiddify
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel.egg-info/SOURCES.txt` & `hiddifypanel-8.0.0.dev8/hiddifypanel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/hiddifypanel.egg-info/requires.txt` & `hiddifypanel-8.0.0.dev8/hiddifypanel.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-8.0.0.dev7/setup.py` & `hiddifypanel-8.0.0.dev8/setup.py`

 * *Files identical despite different names*

