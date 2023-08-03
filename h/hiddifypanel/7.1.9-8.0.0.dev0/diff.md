# Comparing `tmp/hiddifypanel-7.1.9.tar.gz` & `tmp/hiddifypanel-8.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiddifypanel-7.1.9.tar", last modified: Sun Jul 30 14:44:27 2023, max compression
+gzip compressed data, was "hiddifypanel-8.0.0.dev0.tar", last modified: Thu Aug  3 08:14:55 2023, max compression
```

## Comparing `hiddifypanel-7.1.9.tar` & `hiddifypanel-8.0.0.dev0.tar`

### file list

```diff
@@ -1,816 +1,822 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.284593 hiddifypanel-7.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34455 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)    19807 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-30 14:44:27.284593 hiddifypanel-7.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.200592 hiddifypanel-7.1.9/hiddifypanel/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/Events.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.200592 hiddifypanel-7.1.9/hiddifypanel/models/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/models/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/models/child.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/models/config_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/models/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/models/parent_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/models/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/models/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.200592 hiddifypanel-7.1.9/hiddifypanel/panel/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.204592 hiddifypanel-7.1.9/hiddifypanel/panel/admin/
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/Actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/AdminstratorAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/Backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/ChildAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/ConfigAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/Dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/DomainAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/ProxyAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/QuickSetup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/SettingAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/Terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)    14447 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/UserAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/adminlte.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/commercial_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.204592 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/a.html
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/backup.html
--rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/base2.html
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/commercial_info.html
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/config.html
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/configfake.html
--rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/ltemaster.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.204592 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/model/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/model/admin_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/model/domain_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/model/user_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/parent_dash.html
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/proxy.html
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/quick_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/result.html
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/admin_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/cf_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/clean_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.204592 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/ParentDomainAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/ProxyDetailsAdmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.204592 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/restapi/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/restapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/restapi/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/restapi/tgbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/restapi/tgmsg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.204592 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/telegrambot/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/telegrambot/DefaultResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/telegrambot/Usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/telegrambot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/telegrambot/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/telegrambot/information.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.204592 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/templates/configc.html
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/commercial/templates/parent_dash.html
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/custom_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    23761 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/hiddify.py
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/init_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.208592 hiddifypanel-7.1.9/hiddifypanel/panel/user/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/link_maker.html
--rw-r--r--   0 runner    (1001) docker     (123)    19568 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/link_maker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.208592 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/all_configs copy.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/all_configs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/clash_config copy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/clash_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/clash_proxies copy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/clash_proxies.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.208592 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/all-configs.html
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/all-configs_old.html
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/android.html
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/base2.html
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/clash-links copy.html
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/clash-links.html
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/doh.html
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/index copy.html
--rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/index_old.html
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/ios copy.html
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/ios.html
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/multi.html
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/speedtest.html
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/telegram.html
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/usage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/windows.html
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/panel/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/singbox_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.208592 hiddifypanel-7.1.9/hiddifypanel/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/a.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.212592 hiddifypanel-7.1.9/hiddifypanel/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)  1665614 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/css/adminlte.css
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/css/adminlte.fa.css
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/css/adminlte.rtl.css
--rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/css/bootstrap4-rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   163995 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/css/bootstrap5.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/css/custom-rtl.css
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)   101895 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (123)   278568 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/css/lte.old
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.216592 hiddifypanel-7.1.9/hiddifypanel/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    92934 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Black.eot
--rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    53500 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Black.woff
--rw-r--r--   0 runner    (1001) docker     (123)    42308 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Black.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    91810 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Bold.eot
--rw-r--r--   0 runner    (1001) docker     (123)    91644 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    52676 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    41856 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   101090 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Light.eot
--rw-r--r--   0 runner    (1001) docker     (123)   100920 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    59988 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Light.woff
--rw-r--r--   0 runner    (1001) docker     (123)    48616 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Light.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   107842 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Medium.eot
--rw-r--r--   0 runner    (1001) docker     (123)   107668 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    63312 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Medium.woff
--rw-r--r--   0 runner    (1001) docker     (123)    51256 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Medium.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    90482 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Thin.eot
--rw-r--r--   0 runner    (1001) docker     (123)    90316 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    51884 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Thin.woff
--rw-r--r--   0 runner    (1001) docker     (123)    41344 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Thin.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    85354 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir.eot
--rw-r--r--   0 runner    (1001) docker     (123)    85192 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    47972 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir.woff
--rw-r--r--   0 runner    (1001) docker     (123)    38004 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.216592 hiddifypanel-7.1.9/hiddifypanel/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/WhiteLogo.png
--rw-r--r--   0 runner    (1001) docker     (123)   103814 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   111125 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/hiddify-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    37408 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/hiddify.png
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/no_back_hiddify.png
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/pwa-icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.220592 hiddifypanel-7.1.9/hiddifypanel/static/images/splash/
--rw-r--r--   0 runner    (1001) docker     (123)    75224 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/splash/ipad_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    85623 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/splash/ipadpro1_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)   121021 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/splash/ipadpro2_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    90886 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/splash/ipadpro3_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    28231 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/splash/iphone5_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/splash/iphone6_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    68643 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/splash/iphoneplus_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    69743 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/splash/iphonex_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    45109 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/splash/iphonexr_splash.png
--rw-r--r--   0 runner    (1001) docker     (123)    80648 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/images/splash/iphonexsmax_splash.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.220592 hiddifypanel-7.1.9/hiddifypanel/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   104260 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/adminlte.js
--rw-r--r--   0 runner    (1001) docker     (123)    49278 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/bootbox.all.js
--rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/bootbox.all.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    60406 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/custom-rtl.js
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/custom.js
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/demo.js
--rw-r--r--   0 runner    (1001) docker     (123)    89764 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/jquery-3.6.1.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/js.cookie.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    51465 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/moment.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19032 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/pwa-sw.js
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/pwa.js
--rw-r--r--   0 runner    (1001) docker     (123)    33168 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/js/qrcode.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.196592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.192592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.224592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)    37644 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (123)    28977 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   172839 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)   140421 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.224592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)   210612 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)    70808 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   122441 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)    58072 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.220592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap-slider/
--rw-r--r--   0 runner    (1001) docker     (123)    36164 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap-slider/bootstrap-slider.js
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap-slider/slider.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.220592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap-wysihtml5/
--rw-r--r--   0 runner    (1001) docker     (123)   566620 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js
--rw-r--r--   0 runner    (1001) docker     (123)   210932 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.192592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap4-editable/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.224592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap4-editable/css/
--rw-r--r--   0 runner    (1001) docker     (123)    21490 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap4-editable/css/bootstrap-editable.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.224592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap4-editable/img/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap4-editable/img/clear.png
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap4-editable/img/loading.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.224592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap4-editable/js/
--rw-r--r--   0 runner    (1001) docker     (123)   225176 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.js
--rw-r--r--   0 runner    (1001) docker     (123)    76077 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.228592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/chart.js/
--rw-r--r--   0 runner    (1001) docker     (123)   535484 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/chart.js/Chart.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   211133 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/chart.js/Chart.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   403941 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/chart.js/Chart.js
--rw-r--r--   0 runner    (1001) docker     (123)   159638 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/chart.js/Chart.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.228592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/chartjs-old/
--rw-r--r--   0 runner    (1001) docker     (123)   109613 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/chartjs-old/Chart.js
--rw-r--r--   0 runner    (1001) docker     (123)    52092 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/chartjs-old/Chart.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.228592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/
--rw-r--r--   0 runner    (1001) docker     (123)   433051 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/ckeditor.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.232592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ar.js
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ast.js
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/bg.js
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/cs.js
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/da.js
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/de.js
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/el.js
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/en-au.js
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/eo.js
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/es.js
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/et.js
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/eu.js
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/fi.js
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/fr.js
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/gl.js
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/gu.js
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/hr.js
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/hu.js
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/it.js
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ja.js
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/km.js
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/kn.js
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ko.js
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ku.js
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/nb.js
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ne.js
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/nl.js
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/oc.js
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/pl.js
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/pt-br.js
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/pt.js
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ro.js
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ru.js
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/si.js
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/sk.js
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/sq.js
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/sv.js
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/tr.js
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/tt.js
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ug.js
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/uk.js
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/zh-cn.js
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/zh.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.232592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.css
--rw-r--r--   0 runner    (1001) docker     (123)    33831 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.js
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.232592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/img/
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/img/alpha-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/img/alpha.png
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/img/hue-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/img/hue.png
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/img/saturation.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.232592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.css
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.196592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.232592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/AutoFill/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/AutoFill/Readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.232592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/dataTables.autoFill.css
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/dataTables.autoFill.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/filler.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/
--rw-r--r--   0 runner    (1001) docker     (123)    22645 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.js
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/License.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/dataTables.colReorder.css
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/dataTables.colReorder.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/insert.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/
--rw-r--r--   0 runner    (1001) docker     (123)    36311 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.js
--rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/License.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.css
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colvis.jqueryui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/
--rw-r--r--   0 runner    (1001) docker     (123)    27029 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.js
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/License.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.css
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/
--rw-r--r--   0 runner    (1001) docker     (123)    40932 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.js
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/Readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/dataTables.fixedHeader.css
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/dataTables.fixedHeader.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/
--rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.js
--rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/KeyTable/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/KeyTable/Readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/dataTables.keyTable.css
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/dataTables.keyTable.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/
--rw-r--r--   0 runner    (1001) docker     (123)    29477 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.js
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/License.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.236592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.css
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/responsive.bootstrap4.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.240592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/
--rw-r--r--   0 runner    (1001) docker     (123)    25098 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.js
--rw-r--r--   0 runner    (1001) docker     (123)    14589 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/responsive.bootstrap4.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.240592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/Readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.240592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.css
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.240592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/loading-background.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.240592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/
--rw-r--r--   0 runner    (1001) docker     (123)    37984 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.js
--rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.240592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.240592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.css
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.240592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection.png
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy.png
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv.png
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf.png
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print.png
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls.png
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls_hover.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.240592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/
--rw-r--r--   0 runner    (1001) docker     (123)    84578 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.js
--rw-r--r--   0 runner    (1001) docker     (123)    31850 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.240592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls.swf
--rw-r--r--   0 runner    (1001) docker     (123)    58846 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls_pdf.swf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.240592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/images/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/images/sort_asc.png
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/images/sort_asc_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/images/sort_both.png
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/images/sort_desc.png
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/images/sort_desc_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/jquery.dataTables.css
--rw-r--r--   0 runner    (1001) docker     (123)    86551 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/jquery.dataTables.js
--rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    86551 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/jquery.dataTables_themeroller.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.240592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/
--rw-r--r--   0 runner    (1001) docker     (123)    46838 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/bootstrap-datepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)    33745 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/datepicker3.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.248592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ar.js
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.az.js
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.bg.js
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ca.js
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cs.js
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cy.js
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.da.js
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.de.js
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.el.js
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.es.js
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.et.js
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fa.js
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fi.js
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fr.js
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.gl.js
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.he.js
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hr.js
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hu.js
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.id.js
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.is.js
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.it.js
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ja.js
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ka.js
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kk.js
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kr.js
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lt.js
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lv.js
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.mk.js
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ms.js
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nb.js
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl-BE.js
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl.js
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.no.js
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pl.js
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt.js
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ro.js
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs-latin.js
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs.js
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ru.js
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sk.js
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sl.js
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sq.js
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sv.js
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sw.js
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.th.js
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.tr.js
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ua.js
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.vi.js
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-CN.js
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-TW.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.248592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/daterangepicker/
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/daterangepicker/daterangepicker-bs3.css
--rw-r--r--   0 runner    (1001) docker     (123)    53679 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/daterangepicker/daterangepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)    99201 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/daterangepicker/moment.js
--rw-r--r--   0 runner    (1001) docker     (123)    34737 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/daterangepicker/moment.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.248592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/fastclick/
--rw-r--r--   0 runner    (1001) docker     (123)    25965 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/fastclick/fastclick.js
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/fastclick/fastclick.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.252593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/
--rw-r--r--   0 runner    (1001) docker     (123)    41944 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/excanvas.js
--rw-r--r--   0 runner    (1001) docker     (123)    19314 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/excanvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.colorhelpers.js
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.colorhelpers.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.canvas.js
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.categories.js
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.categories.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.js
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.js
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.js
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.image.js
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.image.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   121627 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.js
--rw-r--r--   0 runner    (1001) docker     (123)    52300 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.navigate.js
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.navigate.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    23635 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.pie.js
--rw-r--r--   0 runner    (1001) docker     (123)    12024 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.pie.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.resize.js
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.resize.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.selection.js
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.selection.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.stack.js
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.stack.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.symbol.js
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.symbol.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.threshold.js
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.threshold.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.time.js
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.time.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.196592 hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.252593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/css/
--rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (123)    21778 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.252593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   134808 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.256593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/fullcalendar/
--rw-r--r--   0 runner    (1001) docker     (123)    22515 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/fullcalendar/fullcalendar.css
--rw-r--r--   0 runner    (1001) docker     (123)   279259 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/fullcalendar/fullcalendar.js
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    84823 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/fullcalendar/fullcalendar.print.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.256593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/all.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.256593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/_all.css
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/aero.css
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/aero.png
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/blue.css
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/blue.png
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/flat.css
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/flat.png
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/flat@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/green.css
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/green.png
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/grey.css
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/grey.png
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/orange.css
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/orange.png
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/pink.css
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/pink.png
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/purple.css
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/purple.png
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/red.css
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/red.png
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/yellow.css
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/yellow.png
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.260593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/futurico/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/futurico/futurico.css
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/futurico/futurico.png
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/futurico/futurico@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/icheck.js
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/icheck.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.260593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/
--rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/_all.css
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/aero.css
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/blue.css
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/green.css
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/grey.css
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/line.css
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/line.png
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/line@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/orange.css
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/pink.css
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/purple.css
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/red.css
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/yellow.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.264593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/_all.css
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/aero.css
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/aero.png
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/blue.css
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/blue.png
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/green.css
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/green.png
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/grey.css
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/grey.png
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/minimal.css
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/minimal.png
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/minimal@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/orange.css
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/orange.png
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/pink.css
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/pink.png
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/purple.css
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/purple.png
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/red.css
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/red.png
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/yellow.css
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/yellow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.264593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/polaris/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/polaris/polaris.css
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/polaris/polaris.png
--rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/polaris/polaris@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.264593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/
--rw-r--r--   0 runner    (1001) docker     (123)    15591 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/_all.css
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/aero.css
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/aero.png
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/blue.css
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/blue.png
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/green.css
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/green.png
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/grey.css
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/grey.png
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/orange.css
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/orange.png
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/pink.css
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/pink.png
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/purple.css
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/purple.png
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/red.css
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/red.png
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/square.css
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/square.png
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/square@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/yellow.css
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/yellow.png
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.268593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/
--rw-r--r--   0 runner    (1001) docker     (123)    22814 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/jquery.inputmask.date.extensions.js
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/jquery.inputmask.extensions.js
--rw-r--r--   0 runner    (1001) docker     (123)    90539 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/jquery.inputmask.js
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/jquery.inputmask.numeric.extensions.js
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/jquery.inputmask.phone.extensions.js
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/jquery.inputmask.regex.extensions.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.268593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/phone-codes/
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/phone-codes/phone-be.json
--rw-r--r--   0 runner    (1001) docker     (123)    39492 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/phone-codes/phone-codes.json
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/phone-codes/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.268593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ionslider/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.268593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ionslider/img/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ionslider/img/sprite-skin-flat.png
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ionslider/img/sprite-skin-nice.png
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.css
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinFlat.css
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinNice.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.268593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jQueryUI/
--rw-r--r--   0 runner    (1001) docker     (123)   470596 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jQueryUI/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)   240427 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jQueryUI/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.268593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/
--rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/core.js
--rw-r--r--   0 runner    (1001) docker     (123)   271751 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)    86927 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   132370 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/jquery.min.map
--rw-r--r--   0 runner    (1001) docker     (123)   218897 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/jquery.slim.js
--rw-r--r--   0 runner    (1001) docker     (123)    69917 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/jquery.slim.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   105346 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/jquery.slim.min.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.272593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jvectormap/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.css
--rw-r--r--   0 runner    (1001) docker     (123)    33323 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    95062 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-usa-en.js
--rw-r--r--   0 runner    (1001) docker     (123)   144313 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-world-mill-en.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.272593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/knob/
--rw-r--r--   0 runner    (1001) docker     (123)    26222 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/knob/jquery.knob.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.272593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/morris/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/morris/morris.css
--rw-r--r--   0 runner    (1001) docker     (123)    66046 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/morris/morris.js
--rw-r--r--   0 runner    (1001) docker     (123)    35652 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/morris/morris.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.272593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/pace/
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/pace/pace.css
--rw-r--r--   0 runner    (1001) docker     (123)    26566 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/pace/pace.js
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/pace/pace.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/pace/pace.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.272593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.272593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/esm/
--rw-r--r--   0 runner    (1001) docker     (123)    34601 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/esm/popper-utils.js
--rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/esm/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    84361 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/esm/popper.js
--rw-r--r--   0 runner    (1001) docker     (123)    20314 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/esm/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    32919 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/popper-utils.js
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    80829 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/popper.js
--rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.272593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/umd/
--rw-r--r--   0 runner    (1001) docker     (123)    35703 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/umd/popper-utils.js
--rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/umd/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    84615 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/umd/popper.js
--rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/umd/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.272593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.280593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/az.js
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/bg.js
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/cs.js
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/da.js
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/de.js
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/en.js
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/es.js
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/et.js
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/eu.js
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/fa.js
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/fi.js
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/fr.js
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/gl.js
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/he.js
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/hi.js
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/hr.js
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/hu.js
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/id.js
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/is.js
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/it.js
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/ko.js
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/lt.js
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/lv.js
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/mk.js
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/nb.js
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/nl.js
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/pl.js
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/pt.js
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/ro.js
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/ru.js
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/sk.js
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/sr.js
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/sv.js
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/th.js
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/tr.js
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/uk.js
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/vi.js
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/zh-CN.js
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/zh-TW.js
--rw-r--r--   0 runner    (1001) docker     (123)    17062 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/select2.css
--rw-r--r--   0 runner    (1001) docker     (123)   152250 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/select2.full.js
--rw-r--r--   0 runner    (1001) docker     (123)    71172 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/select2.full.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   132348 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/select2.js
--rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    62834 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/select2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.280593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/slimScroll/
--rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.js
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.280593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/sparkline/
--rw-r--r--   0 runner    (1001) docker     (123)   123446 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/sparkline/jquery.sparkline.js
--rw-r--r--   0 runner    (1001) docker     (123)    43247 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/sparkline/jquery.sparkline.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.280593 hiddifypanel-7.1.9/hiddifypanel/static/plugins/timepicker/
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.css
--rw-r--r--   0 runner    (1001) docker     (123)    26014 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.280593 hiddifypanel-7.1.9/hiddifypanel/static/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   186124 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   107656 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    62320 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    25236 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   397420 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150516 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.284593 hiddifypanel-7.1.9/hiddifypanel/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/templates/a.html
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/templates/admin-layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/templates/admin.ht.old
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/templates/donation.html
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/templates/fake.html
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/templates/flaskadmin-layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.284593 hiddifypanel-7.1.9/hiddifypanel/templates/hiddify-flask-admin/
--rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/templates/hiddify-flask-admin/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/templates/lte-master.html
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/templates/macros.html
--rw-r--r--   0 runner    (1001) docker     (123)    20817 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/templates/master.html
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/templates/static.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.196592 hiddifypanel-7.1.9/hiddifypanel/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.196592 hiddifypanel-7.1.9/hiddifypanel/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.284593 hiddifypanel-7.1.9/hiddifypanel/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    55521 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)   151878 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.196592 hiddifypanel-7.1.9/hiddifypanel/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.284593 hiddifypanel-7.1.9/hiddifypanel/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    74896 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)   174141 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.196592 hiddifypanel-7.1.9/hiddifypanel/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.284593 hiddifypanel-7.1.9/hiddifypanel/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    57475 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)   149973 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.196592 hiddifypanel-7.1.9/hiddifypanel/translations/zh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.284593 hiddifypanel-7.1.9/hiddifypanel/translations/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    47481 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/translations/zh/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)   145307 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/translations/zh/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/hiddifypanel/xray_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:44:27.200592 hiddifypanel-7.1.9/hiddifypanel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-30 14:44:27.000000 hiddifypanel-7.1.9/hiddifypanel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38618 2023-07-30 14:44:27.000000 hiddifypanel-7.1.9/hiddifypanel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 14:44:27.000000 hiddifypanel-7.1.9/hiddifypanel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-30 14:44:27.000000 hiddifypanel-7.1.9/hiddifypanel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-30 14:44:27.000000 hiddifypanel-7.1.9/hiddifypanel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-30 14:44:27.000000 hiddifypanel-7.1.9/hiddifypanel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 14:44:27.284593 hiddifypanel-7.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-30 14:44:14.000000 hiddifypanel-7.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.073526 hiddifypanel-8.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34914 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19807 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 08:14:55.073526 hiddifypanel-8.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.985524 hiddifypanel-8.0.0.dev0/hiddifypanel/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/Events.py
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.985524 hiddifypanel-8.0.0.dev0/hiddifypanel/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/drivers/abstract_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/drivers/singbox_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/drivers/ssh_liberty_bridge_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/drivers/user_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/drivers/xray_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.989524 hiddifypanel-8.0.0.dev0/hiddifypanel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/models/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/models/child.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/models/config_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/models/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/models/parent_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/models/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/models/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.989524 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.989524 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/Actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/AdminstratorAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/Backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/ChildAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/ConfigAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/Dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/DomainAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/ProxyAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/QuickSetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/SettingAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/Terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/UserAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/adminlte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/commercial_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.993524 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/a.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/backup.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/base2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/commercial_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/configfake.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/ltemaster.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.993524 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/model/admin_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/model/domain_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/model/user_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/parent_dash.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/proxy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/quick_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/result.html
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/cf_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/clean_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.993524 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/ParentDomainAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/ProxyDetailsAdmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.993524 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/restapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/restapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/restapi/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/restapi/tgbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/restapi/tgmsg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.993524 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/telegrambot/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/telegrambot/DefaultResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/telegrambot/Usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/telegrambot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/telegrambot/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/telegrambot/information.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.993524 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/templates/configc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/templates/parent_dash.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/custom_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/hiddify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17708 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/init_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.993524 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/link_maker.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19572 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/link_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.993524 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/all_configs copy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/all_configs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/clash_config copy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/clash_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/clash_proxies copy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/clash_proxies.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.997524 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/all-configs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/all-configs_old.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/android.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/base2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/clash-links copy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/clash-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/doh.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/index copy.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/index_old.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/ios copy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/ios.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/multi.html
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/speedtest.html
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/telegram.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/usage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/windows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/singbox_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.997524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/a.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.001524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)  1665614 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/adminlte.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/adminlte.fa.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/adminlte.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/bootstrap4-rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   163995 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/bootstrap5.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/custom-rtl.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)   101895 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)   278568 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/lte.old
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.005524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    92934 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Black.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    53500 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Black.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    42308 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Black.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    91810 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Bold.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    91644 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    52676 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    41856 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   101090 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Light.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   100920 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    59988 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Light.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    48616 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Light.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   107842 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Medium.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   107668 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    63312 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Medium.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    51256 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    90482 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Thin.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    90316 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    51884 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Thin.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    41344 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Thin.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    85354 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    85192 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    47972 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    38004 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.005524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/WhiteLogo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   103814 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   111125 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/hiddify-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37408 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/hiddify.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/no_back_hiddify.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/pwa-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.005524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/
+-rw-r--r--   0 runner    (1001) docker     (123)    75224 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/ipad_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85623 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/ipadpro1_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)   121021 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/ipadpro2_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90886 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/ipadpro3_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28231 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/iphone5_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/iphone6_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68643 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/iphoneplus_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    69743 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/iphonex_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45109 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/iphonexr_splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80648 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/iphonexsmax_splash.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.009524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   104260 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/adminlte.js
+-rw-r--r--   0 runner    (1001) docker     (123)    49278 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/bootbox.all.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/bootbox.all.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    60406 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/custom-rtl.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/demo.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89764 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/jquery-3.6.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/js.cookie.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    51465 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/moment.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19032 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/pwa-sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/pwa.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33168 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/qrcode.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.985524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.981523 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.013524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    37644 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28977 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   172839 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   140421 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.013524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   210612 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)    70808 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   122441 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)    58072 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.009524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap-slider/
+-rw-r--r--   0 runner    (1001) docker     (123)    36164 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap-slider/bootstrap-slider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap-slider/slider.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.009524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap-wysihtml5/
+-rw-r--r--   0 runner    (1001) docker     (123)   566620 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js
+-rw-r--r--   0 runner    (1001) docker     (123)   210932 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.981523 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap4-editable/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.013524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap4-editable/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    21490 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap4-editable/css/bootstrap-editable.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.013524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap4-editable/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap4-editable/img/clear.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap4-editable/img/loading.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.013524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap4-editable/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   225176 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.js
+-rw-r--r--   0 runner    (1001) docker     (123)    76077 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.017524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/chart.js/
+-rw-r--r--   0 runner    (1001) docker     (123)   535484 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/chart.js/Chart.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   211133 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/chart.js/Chart.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   403941 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/chart.js/Chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)   159638 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/chart.js/Chart.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.017524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/chartjs-old/
+-rw-r--r--   0 runner    (1001) docker     (123)   109613 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/chartjs-old/Chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52092 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/chartjs-old/Chart.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.017524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)   433051 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/ckeditor.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.021524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ar.js
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ast.js
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/bg.js
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/cs.js
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/da.js
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/de.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/el.js
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/en-au.js
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/eo.js
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/es.js
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/et.js
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/eu.js
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/fi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/fr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/gl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/gu.js
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/hr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/hu.js
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/it.js
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ja.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/km.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/kn.js
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ko.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ku.js
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/nb.js
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ne.js
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/nl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/oc.js
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/pl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/pt-br.js
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/pt.js
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ro.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ru.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/si.js
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/sk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/sq.js
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/sv.js
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/tr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/tt.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ug.js
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/uk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/zh-cn.js
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/zh.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.021524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.css
+-rw-r--r--   0 runner    (1001) docker     (123)    33831 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.021524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/img/alpha-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/img/alpha.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/img/hue-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/img/hue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/img/saturation.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.021524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.981523 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.021524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/AutoFill/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/AutoFill/Readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.021524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/dataTables.autoFill.css
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/AutoFill/css/dataTables.autoFill.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/filler.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    22645 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/License.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/dataTables.colReorder.css
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/css/dataTables.colReorder.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/insert.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    36311 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/License.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colvis.jqueryui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    27029 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/License.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.css
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    40932 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/Readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/dataTables.fixedHeader.css
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/css/dataTables.fixedHeader.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/KeyTable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/KeyTable/Readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/dataTables.keyTable.css
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/KeyTable/css/dataTables.keyTable.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    29477 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.025524 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/License.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.029525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/responsive.bootstrap4.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.029525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    25098 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14589 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/responsive.bootstrap4.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.029525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/Readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.029525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.css
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.029525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/loading-background.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.029525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    37984 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.029525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.029525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.029525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls_hover.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.029525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    84578 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31850 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.029525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls.swf
+-rw-r--r--   0 runner    (1001) docker     (123)    58846 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls_pdf.swf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.029525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/images/sort_asc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/images/sort_asc_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/images/sort_both.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/images/sort_desc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/images/sort_desc_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/jquery.dataTables.css
+-rw-r--r--   0 runner    (1001) docker     (123)    86551 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/jquery.dataTables.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    86551 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/jquery.dataTables_themeroller.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.029525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/
+-rw-r--r--   0 runner    (1001) docker     (123)    46838 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/bootstrap-datepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33745 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/datepicker3.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.037525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ar.js
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.az.js
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.bg.js
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cs.js
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cy.js
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.da.js
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.de.js
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.el.js
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.es.js
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.et.js
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.gl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.he.js
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hu.js
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.id.js
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.is.js
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.it.js
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ja.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ka.js
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lt.js
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lv.js
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.mk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ms.js
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nb.js
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl-BE.js
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.no.js
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt.js
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ro.js
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs-latin.js
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs.js
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ru.js
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sq.js
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sv.js
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.th.js
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.tr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ua.js
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.vi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-CN.js
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-TW.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.037525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/daterangepicker/
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/daterangepicker/daterangepicker-bs3.css
+-rw-r--r--   0 runner    (1001) docker     (123)    53679 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/daterangepicker/daterangepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    99201 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/daterangepicker/moment.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34737 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/daterangepicker/moment.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.037525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fastclick/
+-rw-r--r--   0 runner    (1001) docker     (123)    25965 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fastclick/fastclick.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fastclick/fastclick.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.041525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/
+-rw-r--r--   0 runner    (1001) docker     (123)    41944 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/excanvas.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19314 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/excanvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.colorhelpers.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.colorhelpers.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.canvas.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.categories.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.categories.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.image.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.image.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   121627 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52300 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.navigate.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.navigate.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23635 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.pie.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12024 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.pie.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.resize.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.resize.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.selection.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.selection.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.stack.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.stack.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.symbol.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.symbol.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.threshold.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.threshold.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.time.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.time.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.981523 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.041525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21778 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.041525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   134808 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.045525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fullcalendar/
+-rw-r--r--   0 runner    (1001) docker     (123)    22515 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fullcalendar/fullcalendar.css
+-rw-r--r--   0 runner    (1001) docker     (123)   279259 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fullcalendar/fullcalendar.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    84823 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fullcalendar/fullcalendar.print.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.045525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/all.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.045525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/_all.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/aero.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/aero.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/blue.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/flat.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/flat.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/flat@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/green.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/green.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/grey.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/grey.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/orange.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/orange.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/pink.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/pink.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/purple.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/purple.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/red.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/red.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.045525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/futurico/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/futurico/futurico.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/futurico/futurico.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/futurico/futurico@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/icheck.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/icheck.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.049525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/
+-rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/_all.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/aero.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/blue.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/green.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/grey.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/line.css
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/line.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/line@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/orange.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/pink.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/purple.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/red.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/yellow.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.053525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/_all.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/aero.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/aero.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/blue.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/green.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/green.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/grey.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/grey.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/minimal.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/minimal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/minimal@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/orange.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/orange.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/pink.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/pink.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/purple.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/purple.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/red.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/red.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.053525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/polaris/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/polaris/polaris.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/polaris/polaris.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/polaris/polaris@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.053525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/
+-rw-r--r--   0 runner    (1001) docker     (123)    15591 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/_all.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/aero.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/aero.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/blue.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/green.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/green.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/grey.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/grey.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/orange.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/orange.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/pink.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/pink.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/purple.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/purple.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/red.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/red.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/square.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/square.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/square@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.053525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/
+-rw-r--r--   0 runner    (1001) docker     (123)    22814 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/jquery.inputmask.date.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/jquery.inputmask.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (123)    90539 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/jquery.inputmask.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/jquery.inputmask.numeric.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/jquery.inputmask.phone.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/jquery.inputmask.regex.extensions.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.057525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/phone-codes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/phone-codes/phone-be.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39492 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/phone-codes/phone-codes.json
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/phone-codes/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.057525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ionslider/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.057525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ionslider/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ionslider/img/sprite-skin-flat.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ionslider/img/sprite-skin-nice.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinFlat.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinNice.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.057525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jQueryUI/
+-rw-r--r--   0 runner    (1001) docker     (123)   470596 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jQueryUI/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)   240427 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jQueryUI/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.057525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/core.js
+-rw-r--r--   0 runner    (1001) docker     (123)   271751 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86927 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   132370 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/jquery.min.map
+-rw-r--r--   0 runner    (1001) docker     (123)   218897 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/jquery.slim.js
+-rw-r--r--   0 runner    (1001) docker     (123)    69917 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/jquery.slim.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   105346 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/jquery.slim.min.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.057525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jvectormap/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.css
+-rw-r--r--   0 runner    (1001) docker     (123)    33323 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95062 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-usa-en.js
+-rw-r--r--   0 runner    (1001) docker     (123)   144313 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-world-mill-en.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.061525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/knob/
+-rw-r--r--   0 runner    (1001) docker     (123)    26222 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/knob/jquery.knob.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.061525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/morris/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/morris/morris.css
+-rw-r--r--   0 runner    (1001) docker     (123)    66046 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/morris/morris.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35652 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/morris/morris.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.061525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/pace/
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/pace/pace.css
+-rw-r--r--   0 runner    (1001) docker     (123)    26566 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/pace/pace.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/pace/pace.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/pace/pace.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.061525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.061525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/esm/
+-rw-r--r--   0 runner    (1001) docker     (123)    34601 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/esm/popper-utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/esm/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    84361 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/esm/popper.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20314 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/esm/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32919 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/popper-utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80829 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/popper.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.061525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/umd/
+-rw-r--r--   0 runner    (1001) docker     (123)    35703 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/umd/popper-utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/umd/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    84615 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/umd/popper.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/umd/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.065525 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.069526 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/az.js
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/bg.js
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/cs.js
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/da.js
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/de.js
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/en.js
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/es.js
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/et.js
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/eu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/fi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/fr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/gl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/he.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/hi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/hr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/hu.js
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/id.js
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/is.js
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/it.js
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/ko.js
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/lt.js
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/lv.js
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/mk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/nb.js
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/nl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/pl.js
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/pt.js
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/ro.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/ru.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/sk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/sr.js
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/sv.js
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/th.js
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/tr.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/uk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/vi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/zh-CN.js
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/zh-TW.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17062 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/select2.css
+-rw-r--r--   0 runner    (1001) docker     (123)   152250 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/select2.full.js
+-rw-r--r--   0 runner    (1001) docker     (123)    71172 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/select2.full.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   132348 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/select2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    62834 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/select2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.069526 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/slimScroll/
+-rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.069526 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/sparkline/
+-rw-r--r--   0 runner    (1001) docker     (123)   123446 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/sparkline/jquery.sparkline.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43247 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/sparkline/jquery.sparkline.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.069526 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/timepicker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.css
+-rw-r--r--   0 runner    (1001) docker     (123)    26014 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.069526 hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   186124 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   107656 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    62320 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    25236 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   397420 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150516 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.073526 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/a.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/admin-layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/admin.ht.old
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/donation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/fake.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/flaskadmin-layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.073526 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/hiddify-flask-admin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/hiddify-flask-admin/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/lte-master.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20817 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/master.html
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/templates/static.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.985524 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.985524 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.073526 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    56211 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   153354 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.985524 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.073526 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    74896 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   175272 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.985524 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.073526 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    57475 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   151104 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.985524 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/zh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:55.073526 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    47481 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/zh/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   146438 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/hiddifypanel/translations/zh/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:14:54.985524 hiddifypanel-8.0.0.dev0/hiddifypanel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 08:14:54.000000 hiddifypanel-8.0.0.dev0/hiddifypanel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38833 2023-08-03 08:14:54.000000 hiddifypanel-8.0.0.dev0/hiddifypanel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:14:54.000000 hiddifypanel-8.0.0.dev0/hiddifypanel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-03 08:14:54.000000 hiddifypanel-8.0.0.dev0/hiddifypanel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-03 08:14:54.000000 hiddifypanel-8.0.0.dev0/hiddifypanel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 08:14:54.000000 hiddifypanel-8.0.0.dev0/hiddifypanel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:14:55.073526 hiddifypanel-8.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-03 08:14:40.000000 hiddifypanel-8.0.0.dev0/setup.py
```

### Comparing `hiddifypanel-7.1.9/HISTORY.md` & `hiddifypanel-8.0.0.dev0/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,45 @@
 # Changelog
 
 
+## (unreleased)
+
+#### New
+
+* Add caching for speed up some process. 
+
+* Add singbox config. 
+
+* Add singbox config for ssh. 
+
+* Add ssh server port. 
+
+* Add ssh user support. 
+
+#### Changes
+
+* Disable caching. 
+
+#### Fix
+
+* Ssh liberty redis path. 
+
+#### Other
+
+* Merge branch 'main' of github.com:hiddify1/HiddifyPanel. 
+
+* Merge pull request #14 from randomguy-on-internet/patch-1. 
+  _clash GRPC bug_
+
+* Update link_maker.py. 
+
+* Update link_maker.py. 
+
+
+
 ## 7.1.9 (2023-07-30)
 
 #### Fix
 
 * Bugs.
```

### Comparing `hiddifypanel-7.1.9/LICENSE.md` & `hiddifypanel-8.0.0.dev0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/PKG-INFO` & `hiddifypanel-8.0.0.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiddifypanel
-Version: 7.1.9
+Version: 8.0.0.dev0
 Summary: hiddifypanel multi proxy panel
 Home-page: https://github.com/hiddify/hiddify-config/
 Author: hiddify
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `hiddifypanel-7.1.9/README.md` & `hiddifypanel-8.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/Events.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/Events.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/base.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import flask_bootstrap
 import hiddifypanel
 from dynaconf import FlaskDynaconf
 from flask import Flask, request, g
 from flask_babelex import Babel
 from hiddifypanel.panel.init_db import init_db
 import hiddifypanel
-from hiddifypanel.models import  *
+from hiddifypanel.models import *
 from dotenv import dotenv_values
 import os
-def create_app(cli=False,**config):
+
+
+def create_app(cli=False, **config):
     app = Flask(__name__, static_url_path="/<proxy_path>/static/", instance_relative_config=True)
 
-    for c,v in dotenv_values('app.cfg').items():
+    for c, v in dotenv_values('app.cfg').items():
         if v.isdecimal():
-            v= int(v)
+            v = int(v)
         else:
-            v=True if v.lower()=="true" else (False if v.lower()=="false" else v)
+            v = True if v.lower() == "true" else (False if v.lower() == "false" else v)
 
-        
-        app.config[c]=v
-        
+        app.config[c] = v
 
     app.jinja_env.line_statement_prefix = '%'
-    app.is_cli=cli
+    app.is_cli = cli
     flask_bootstrap.Bootstrap4(app)
-    
+
     hiddifypanel.panel.database.init_app(app)
     with app.app_context():
         init_db()
-        
 
     hiddifypanel.panel.common.init_app(app)
     hiddifypanel.panel.admin.init_app(app)
     hiddifypanel.panel.user.init_app(app)
     hiddifypanel.panel.commercial.init_app(app)
     hiddifypanel.panel.cli.init_app(app)
 
@@ -54,18 +53,22 @@
 
     from flask_wtf.csrf import CSRFProtect
 
     csrf = CSRFProtect(app)
 
     @app.before_request
     def check_csrf():
-        if "/admin/user/" in request.base_url: return
-        if "/admin/domain/" in request.base_url: return
-        if "/admin/actions/" in request.base_url: return
-        if "/api/v1/" in request.base_url: return
+        if "/admin/user/" in request.base_url:
+            return
+        if "/admin/domain/" in request.base_url:
+            return
+        if "/admin/actions/" in request.base_url:
+            return
+        if "/api/v1/" in request.base_url:
+            return
         csrf.protect()
 
     app.jinja_env.globals['get_locale'] = get_locale
     app.jinja_env.globals['version'] = hiddifypanel.__version__
 
     return app
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/models/__init__.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/models/admin.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/models/admin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/models/child.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/models/child.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/models/config.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/models/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# from hiddifypanel.cache import cache
 from sqlalchemy_serializer import SerializerMixin
 from flask import Flask
 from flask_sqlalchemy import SQLAlchemy
 from flask_admin import Admin
 from flask_admin.contrib.sqla import ModelView
 from wtforms import SelectMultipleField
 
@@ -44,14 +45,15 @@
         return {
             'key': d.key,
             'value': d.value,
             'child_unique_id': d.child.unique_id if d.child else ''
         }
 
 
+# @cache.cache()
 def hconfig(key: ConfigEnum, child_id=0):
     value = None
     try:
         str_conf = StrConfig.query.filter(StrConfig.key == key, StrConfig.child_id == child_id).first()
         if str_conf:
             value = str_conf.value
         else:
@@ -70,15 +72,15 @@
         print(f'{key} error!')
         raise
 
     return value
 
 
 def set_hconfig(key: ConfigEnum, value, child_id=0, commit=True):
-
+    hconfig.invalidate(key, child_id)
     if key.type() == bool:
         dbconf = BoolConfig.query.filter(BoolConfig.key == key, BoolConfig.child_id == child_id).first()
         if not dbconf:
             dbconf = BoolConfig(key=key, value=value, child_id=child_id)
             db.session.add(dbconf)
     else:
         dbconf = StrConfig.query.filter(StrConfig.key == key, StrConfig.child_id == child_id).first()
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/models/config_enum.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/models/config_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,29 +22,32 @@
     branding = auto()
     general = auto()
     proxies = auto()
     domain_fronting = auto()
     telegram = auto()
     http = auto()
     tls = auto()
-
+    ssh = auto()
     ssfaketls = auto()
     shadowtls = auto()
     restls = auto()
     tuic = auto()
     ssr = auto()
     kcp = auto()
     hidden = auto()
     advanced = auto()
     too_advanced = auto()
     warp = auto()
     reality = auto()
 
 
 class ConfigEnum(StrEnum):
+    ssh_server_redis_url = auto()
+    ssh_server_ports = auto()
+    ssh_server_enable = auto()
     first_setup = auto()
     core_type = auto()
     warp_enable = auto()
     warp_mode = auto()
     warp_plus_code = auto()
     dns_server = auto()
     reality_fallback_domain = auto()
@@ -135,14 +138,17 @@
     # cdn_forced_host=auto()
     @classmethod
     def _missing_(cls, value):
         return cls.not_found  # "key not found"
 
     def info(self):
         map = {
+            self.ssh_server_redis_url: {'category': ConfigCategory.hidden},
+            self.ssh_server_ports: {'category': ConfigCategory.ssh},
+            self.ssh_server_enable: {'category': ConfigCategory.ssh},
             self.core_type: {'category': ConfigCategory.advanced, 'apply_mode': 'apply'},
             self.dns_server: {'category': ConfigCategory.general, 'apply_mode': 'apply'},
             self.warp_enable: {'category': ConfigCategory.hidden, 'type': bool, 'apply_mode': 'restart'},
             self.warp_mode: {'category': ConfigCategory.warp, 'apply_mode': 'apply'},
             self.warp_plus_code: {'category': ConfigCategory.warp, 'apply_mode': 'apply'},
             self.restls1_2_domain: {'category': ConfigCategory.hidden},
             self.restls1_3_domain: {'category': ConfigCategory.hidden},
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/models/domain.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/models/domain.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/models/parent_domain.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/models/parent_domain.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/models/proxy.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/models/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     faketls = auto()
     shadowtls = auto()
     restls1_2 = auto()
     restls1_3 = auto()
     # h1=auto()
     WS = auto()
     tcp = auto()
+    ssh = auto()
 
 
 class ProxyCDN(StrEnum):
     CDN = auto()
     direct = auto()
     Fake = auto()
 
@@ -36,23 +37,25 @@
 class ProxyProto(StrEnum):
     vless = auto()
     trojan = auto()
     vmess = auto()
     ss = auto()
     v2ray = auto()
     ssr = auto()
+    ssh = auto()
 
 
 class ProxyL3(StrEnum):
     tls = auto()
     tls_h2 = auto()
     tls_h2_h1 = auto()
     reality = auto()
     http = auto()
     kcp = auto()
+    ssh = auto()
     # hysteria=auto()
 
 
 class Proxy(db.Model, SerializerMixin):
     id = db.Column(db.Integer, primary_key=True, autoincrement=True)
     child_id = db.Column(db.Integer, db.ForeignKey('child.id'), default=0)
     name = db.Column(db.String(200), nullable=False, unique=True)
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/models/usage.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/models/usage.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/models/user.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,17 @@
     last_reset_time = db.Column(db.Date, default=datetime.date.today())
     comment = db.Column(db.String(512))
     telegram_id = db.Column(db.String(512))
     added_by = db.Column(db.Integer, db.ForeignKey('admin_user.id'), default=0)
     max_ips = db.Column(db.Integer, default=1000, nullable=False)
     details = db.relationship('UserDetail', cascade="all,delete", backref='user',    lazy='dynamic',)
     enable = db.Column(db.Boolean, default=True, nullable=False)
+    ed25519_private_key=db.Column(db.String(100))
+    ed25519_public_key=db.Column(db.String(100))
+
 
     @property
     def remaining_days(self):
         return remaining_days(self)
 
     @property
     def is_active(self):
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/Actions.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/Actions.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/AdminstratorAdmin.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/AdminstratorAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/Backup.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/Backup.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/ChildAdmin.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/ChildAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/ConfigAdmin.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/ConfigAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/Dashboard.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/Dashboard.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/DomainAdmin.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/DomainAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/ProxyAdmin.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/ProxyAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/QuickSetup.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/QuickSetup.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/SettingAdmin.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/SettingAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/Terminal.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/Terminal.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/UserAdmin.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/UserAdmin.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from hiddifypanel.panel.database import db
 import datetime
 from hiddifypanel.models import *
 from flask import Markup, g, request, url_for, abort
 from wtforms.validators import Regexp, ValidationError
 import re
 import uuid
-from hiddifypanel import xray_api
+from hiddifypanel.drivers import user_driver
 from .adminlte import AdminLTEModelView
 # from gettext import gettext as _
 from flask_babelex import gettext as __
 from flask_babelex import lazy_gettext as _
 
 from wtforms.validators import NumberRange
 
@@ -191,15 +191,15 @@
         'last_online': _online_formatter,
         'admin': _admin_formatter
     }
 
     def on_model_delete(self, model):
         if len(User.query.all()) <= 1:
             raise ValidationError(f"at least one user should exist")
-        xray_api.remove_client(model.uuid)
+        user_driver.remove_client(model.uuid)
         # hiddify.flash_config_success()
 
     # def is_accessible(self):
     #     return g.is_admin
 
     def on_form_prefill(self, form, id=None):
         # print("================",form._obj.start_date)
@@ -247,15 +247,15 @@
         old_user = user_by_id(model.id)
         if not model.added_by:
             model.added_by = g.admin.id
         if not g.admin.can_have_more_users():
             raise ValidationError(_('You have too much users! You can have only %(active)s active users and %(total)s users',
                                   active=g.admin.max_active_users, total=g.admin.max_users))
         if old_user and old_user.uuid != model.uuid:
-            xray_api.remove_client(old_user.uuid)
+            user_driver.remove_client(old_user.uuid)
 
         # model.expiry_time=datetime.date.today()+datetime.timedelta(days=model.expiry_time)
 
         # if model.current_usage_GB < model.usage_limit_GB:
         #     xray_api.add_client(model.uuid)
         # else:
         #     xray_api.remove_client(model.uuid)
@@ -263,21 +263,21 @@
     # def is_accessible(self):
     #     return is_valid()
 
     def after_model_change(self, form, model, is_created):
 
         user = User.query.filter(User.uuid == model.uuid).first()
         if is_user_active(user):
-            xray_api.add_client(model.uuid)
+            user_driver.add_client(model.uuid)
         else:
-            xray_api.remove_client(model.uuid)
+            user_driver.remove_client(model.uuid)
         hiddify.quick_apply_users()
 
     def after_model_delete(self, model):
-        xray_api.remove_client(model.uuid)
+        user_driver.remove_client(model.uuid)
 
         hiddify.quick_apply_users()
 
     def get_list(self, page, sort_column, sort_desc, search, filters, *args, **kwargs):
         res = None
         # print('aaa',args, kwargs)
         if 'remaining_days' == sort_column:
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/__init__.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/adminlte.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/adminlte.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/commercial_info.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/commercial_info.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/backup.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/backup.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/base.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/base.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/base2.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/base2.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/config.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/config.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/configfake.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/configfake.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/index.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/index.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/ltemaster.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/ltemaster.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/model/admin_list.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/model/admin_list.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/model/user_list.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/model/user_list.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/parent_dash.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/parent_dash.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/proxy.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/proxy.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/quick_setup.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/quick_setup.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin/templates/result.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin/templates/result.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/admin_2.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/admin_2.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/cf_api.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/cf_api.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/clean_ip.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/clean_ip.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/cli.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/cli.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/commercial/ParentDomainAdmin.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/ParentDomainAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/commercial/ProxyDetailsAdmin.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/ProxyDetailsAdmin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/commercial/__init__.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/commercial/restapi/__init__.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/restapi/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/commercial/restapi/resources.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/restapi/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from flask import abort, jsonify, request
 from flask_restful import Resource
 # from flask_simplelogin import login_required
 import datetime
 from hiddifypanel.models import *
 from urllib.parse import urlparse
 from hiddifypanel.panel import hiddify
-from hiddifypanel import xray_api
+from hiddifypanel.drivers import user_driver
 # class AllResource(Resource):
 #     def get(self):
 #         return jsonify(
 #             hiddify.dump_db_to_dict()
 #         )
 
 
@@ -23,15 +23,15 @@
         return jsonify(
             [product.to_dict() for product in products]
         )
 
     def post(self):
         data = request.json
         hiddify.add_or_update_user(**data)
-        xray_api.add_client(data['uuid'])
+        user_driver.add_client(data['uuid'])
         hiddify.quick_apply_users()
 
         return jsonify({'status': 200, 'msg': 'ok'})
 
 
 class AdminUserResource(Resource):
     def get(self, uuid=None):
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/commercial/restapi/tgbot.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/restapi/tgbot.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/commercial/restapi/tgmsg.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/restapi/tgmsg.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/commercial/telegrambot/Usage.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/telegrambot/Usage.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/commercial/telegrambot/admin.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/telegrambot/admin.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/commercial/telegrambot/information.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/telegrambot/information.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/commercial/templates/configc.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/templates/configc.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/commercial/templates/parent_dash.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/commercial/templates/parent_dash.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/common.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/common.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/custom_widgets.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/custom_widgets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
+from flask_admin.contrib.sqla import ModelView
+from wtforms.widgets import TextArea
+from wtforms import TextAreaField
+from flask_bootstrap import SwitchField
+from wtforms.fields import StringField, IntegerField, SelectField
+from hiddifypanel.panel.hiddify import flash
+from hiddifypanel.panel import hiddify
+from flask_babelex import lazy_gettext as _
+from flask_babelex import gettext as __
 from flask_admin.contrib import sqla
 from hiddifypanel.panel.database import db
 import datetime
 from hiddifypanel.models import *
 from flask import Markup, g
 from wtforms.validators import Regexp, ValidationError
 import re
 import uuid
-from hiddifypanel import xray_api
+
 # from gettext import gettext as _
-from flask_babelex import gettext as __
-from flask_babelex import lazy_gettext as _
-from hiddifypanel.panel import hiddify
-from hiddifypanel.panel.hiddify import flash
-from wtforms.fields import StringField, IntegerField, SelectField
-from flask_bootstrap import SwitchField
-from wtforms import TextAreaField
-from wtforms.widgets import TextArea
-from flask_admin.contrib.sqla import ModelView
 
 
 class DaysLeftField(IntegerField):
     def process_data(self, value):
         if value is not None:
             days_left = (value - datetime.date.today()).days
             self.data = days_left
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/hiddify.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/hiddify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import socket
 from sqlalchemy.orm import Load
+import glob
+import json
 from babel.dates import format_timedelta as babel_format_timedelta
 from flask_babelex import gettext as __
 from flask_babelex import lazy_gettext as _
 from hiddifypanel.models import *
 from hiddifypanel.panel.database import db
 import datetime
-from flask import jsonify, g, url_for, Markup, abort
+from flask import jsonify, g, url_for, Markup, abort, current_app
 from flask import flash as flask_flash
 from wtforms.validators import ValidationError
 import requests
 # from hiddifypanel.panel.admin.Actions import Actions
 import string
 import random
 from babel.dates import format_timedelta as babel_format_timedelta
@@ -663,7 +665,27 @@
     output = subprocess.check_output(cmd, shell=True, text=True)
     # Extract the private and public keys from the output
     private_key = output.split("Private key: ")[1].split("\n")[0]
     public_key = output.split("Public key: ")[1].split("\n")[0]
 
     # Return the keys as a tuple
     return {"private_key": private_key, "public_key": public_key}
+
+
+def get_hostkeys(dojson=False):
+    key_files = glob.glob(current_app.config['HIDDIFY_CONFIG_PATH'] + "/other/ssh/host_key/*_key.pub")
+    host_keys = []
+    for file_name in key_files:
+        with open(file_name, "r") as f:
+            host_key = f.read().strip()
+            host_key = host_key.split()
+            if len(host_key) > 2:
+                host_key = host_key[:2]  # strip the hostname part
+            host_key = " ".join(host_key)
+            host_keys.append(host_key)
+    if dojson:
+        return json.dumps(host_keys)
+    return host_keys
+
+
+def get_ssh_client_version(user):
+    return 'SSH-2.0-OpenSSH_7.4p1'
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/init_db.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/init_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     execute(f'update proxy set transport="WS" where transport = "ws"')
     execute(f'update admin_user set mode="agent" where mode = "slave"')
     execute(f'update admin_user set mode="super_admin" where id=1')
     execute(f'DELETE from proxy where transport = "h1"')
 
     add_column(Domain.grpc)
     add_column(ParentDomain.alias)
+    add_column(User.ed25519_private_key)
+    add_column(User.ed25519_public_key)
     add_column(User.start_date)
     add_column(User.package_days)
     add_column(User.telegram_id)
     add_column(Child.unique_id)
     add_column(Domain.alias)
     add_column(Domain.sub_link_only)
     add_column(Domain.child_id)
@@ -104,19 +106,42 @@
         db.session.commit()
         set_hconfig(ConfigEnum.db_version, db_version, commit=False)
 
     db.session.commit()
     return BoolConfig.query.all()
 
 
+def _v44():
+    import ed25519
+    for u in User.query.all():
+
+        privkey = ed25519.Ed25519PrivateKey.generate()
+        pubkey = privkey.public_key()
+        priv_bytes = privkey.private_bytes(
+            encoding=serialization.Encoding.PEM,
+            format=serialization.PrivateFormat.OpenSSH,
+            encryption_algorithm=serialization.NoEncryption(),
+        )
+        pub_bytes = pubkey.public_bytes(
+            encoding=serialization.Encoding.OpenSSH,
+            format=serialization.PublicFormat.OpenSSH,
+        )
+        u.ed25519_private_key = priv_bytes.decode()
+        u.ed25519_public_key = pub_bytes.decode()
+    db.session.add(Proxy(l3='ssh', transport='ssh', cdn='direct', proto='ssh', enable=True, name="SSH"))
+    add_config_if_not_exist(ConfigEnum.ssh_server_redis_url, "unix:///opt/hiddify-config/other/redis/run.sock?db=1")
+    add_config_if_not_exist(ConfigEnum.ssh_server_port, random.randint(5000, 20000))
+    add_config_if_not_exist(ConfigEnum.ssh_server_enable, False)
 # def _v43():
 #     if not (Domain.query.filter(Domain.domain==hconfig(ConfigEnum.domain_fronting_domain)).first()):
 #         db.session.add(Domain(domain=hconfig(ConfigEnum.domain_fronting_domain),servernames=hconfig(ConfigEnum.domain_fronting_domain),mode=DomainType.cdn))
 
 # v7.0.0
+
+
 def _v42():
 
     for k in [ConfigEnum.telegram_fakedomain, ConfigEnum.ssfaketls_fakedomain, ConfigEnum.shadowtls_fakedomain]:
         if not hconfig(k):
             rnd_domains = get_random_domains(1)
             add_config_if_not_exist(k, rnd_domains[0])
 
@@ -362,15 +387,16 @@
         # "h1 direct vmess",
         "faketls direct ss",
         "WS direct v2ray",
         "shadowtls direct ss",
         "restls1_2 direct ss",
         "restls1_3 direct ss",
         "tcp direct ssr",
-        "WS CDN v2ray"]
+        "WS CDN v2ray"
+    ]
     )
 
 
 def make_proxy_rows(cfgs):
     for l3 in ["tls_h2", "tls", "http", "kcp", "reality"]:
         for c in cfgs:
             transport, cdn, proto = c.split(" ")
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/usage.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/usage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from sqlalchemy.orm import Load
-from hiddifypanel import xray_api, singbox_api
+from hiddifypanel.drivers import user_driver
 from sqlalchemy import func
 from flask_babelex import gettext as __
 from flask_babelex import lazy_gettext as _
 import urllib
 from hiddifypanel.models import *
 from hiddifypanel.panel.database import db
 import datetime
@@ -11,46 +11,35 @@
 from flask import flash as flask_flash
 to_gig_d = 1024**3
 
 # from hiddifypanel.panel import hiddify_api #hiddify
 
 
 def update_local_usage():
-
-    res = {}
-    have_change = False
-    for user in User.query.all():
-        d = xray_api.get_usage(user.uuid, reset=True)
-        sd = singbox_api.get_usage(user.uuid, reset=True)
-        res[user] = {'usage': (d or 0)+(sd or 0), 'ips': ''}
-
-    return add_users_usage(res, 0)
+    res = user_driver.get_users_usage(reset=True)
+    return add_users_usage(res, child_id=0)
 
     # return {"status": 'success', "comments":res}
 
 
 def add_users_usage_uuid(uuids_bytes, child_id):
     users = User.query.filter(User.uuid.in_(keys(uuids_bytes)))
     dbusers_bytes = {u: uuids_bytes.get(u.uuid, 0) for u in users}
     add_users_usage(dbusers_bytes, child_id)
 
 
-def is_already_valid(uuid):
-    xray_api.get_xray_client().add_client(t, f'{uuid}', f'{uuid}@hiddify.com', protocol=protocol, flow='xtls-rprx-vision', alter_id=0, cipher='chacha20_poly1305')
-
-
 def add_users_usage(dbusers_bytes, child_id):
     print(dbusers_bytes)
     if not hconfig(ConfigEnum.is_parent) and hconfig(ConfigEnum.parent_panel):
         from hiddifypanel.panel import hiddify_api
         hiddify_api.add_user_usage_to_parent(dbusers_bytes)
 
     res = {}
     have_change = False
-    before_enabled_users = xray_api.get_enabled_users()
+    before_enabled_users = user_driver.get_enabled_users()
     daily_usage = {}
     today = datetime.date.today()
     for adm in AdminUser.query.all():
         daily_usage[adm.id] = DailyUsage.query.filter(DailyUsage.date == today, DailyUsage.admin_id == adm.id, DailyUsage.child_id == child_id).first()
         if not daily_usage[adm.id]:
             daily_usage[adm.id] = DailyUsage(admin_id=adm.id, child_id=child_id)
             db.session.add(daily_usage[adm.id])
@@ -69,15 +58,15 @@
         detail.current_usage_GB = detail.current_usage_GB or 0
         if not user.last_reset_time or user_should_reset(user):
             user.last_reset_time = datetime.date.today()
             user.current_usage_GB = 0
             detail.current_usage_GB = 0
 
         if before_enabled_users[user.uuid] == 0 and user.is_active:
-            xray_api.add_client(user.uuid)
+            user_driver.add_client(user)
             send_bot_message(user)
             have_change = True
         if type(usage_bytes) != int or usage_bytes == 0:
             res[user.uuid] = "No usage"
         else:
             daily_usage.get(user.added_by, daily_usage[1]).usage += usage_bytes
             in_gig = (usage_bytes)/to_gig_d
@@ -87,15 +76,15 @@
             user.last_online = datetime.datetime.now()
             detail.last_online = datetime.datetime.now()
 
             if user.start_date == None:
                 user.start_date = datetime.date.today()
 
         if before_enabled_users[user.uuid] == 1 and not is_user_active(user):
-            xray_api.remove_client(user.uuid)
+            user_driver.remove_client(user)
             have_change = True
             res[user.uuid] = f"{res[user.uuid]} !OUT of USAGE! Client Removed"
 
     db.session.commit()
     if have_change:
         hiddify.quick_apply_users()
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/__init__.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/__init__.py`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/link_maker.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/link_maker.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
             "grpc-service-name": proxy["grpc_service_name"]
         }
     if proxy['l3'] == ProxyL3.reality:
         base["reality-opts"] = {
             "public-key": proxy['reality_pbk'],
             "short-id": proxy['reality_short_id'],
         }
-        if proxy['proto'] != 'grpc':
+        if proxy["transport"] != 'grpc':
             base["network"] = 'tcp'
 
     return base
 
 
 def get_clash_config_names(meta_or_normal, domains):
     allphttp = [p for p in request.args.get("phttp", "").split(',') if p]
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/all_configs.txt` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/all_configs.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/clash_config copy.yml` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/clash_config copy.yml`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/clash_config.yml` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/clash_config.yml`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/clash_proxies copy.yml` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/clash_proxies copy.yml`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/clash_proxies.yml` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/clash_proxies.yml`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/all-configs.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/all-configs.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,97 +1,110 @@
 {{_("user.home.tool.all-configs")}}
 
 <div class="col">
-<table id="all-links" class="table table-bordered table-striped dt-responsive nowrap" style="width:100%">
-  <thead>
-    <tr>
-      <th>{{_('user.home.allconfig.name')}}</th>
-      <th>{{_('user.home.allconfig.type')}}</th>
-      <th>{{_('Domain')}}</th>
-      <th>{{_('user.home.allconfig.protocol')}}</th>
-      <th>{{_('user.home.allconfig.transport')}}</th>
-      <th>{{_('user.home.allconfig.security')}}</th>
+  <table id="all-links" class="table table-bordered table-striped dt-responsive nowrap" style="width:100%">
+    <thead>
+      <tr>
+        <th>{{_('user.home.allconfig.name')}}</th>
+        <th>{{_('user.home.allconfig.type')}}</th>
+        <th>{{_('Domain')}}</th>
+        <th>{{_('user.home.allconfig.protocol')}}</th>
+        <th>{{_('user.home.allconfig.transport')}}</th>
+        <th>{{_('user.home.allconfig.security')}}</th>
 
-    </tr>
-  </thead>
-  <tbody>
-    <tr>
-      <td>
-        <div class="btn-group">
-          <a href="clashmeta://install-config?url=https://{{domain}}/{{hconfigs[ConfigEnum.proxy_path]}}/{{user.uuid}}/clash/meta/all.yml&name=mnormal_{{db_domain.alias or db_domain.domain}}-{{asn}}-{{mode}}&asn={{asn}}&mode={{mode}}"
-            class="btn btn-light orig-link"> {{_('user.home.allconfig.hiddify-configs')}}</a>
-        </div>
-      </td>
-      <td><span class="badge badge-danger">{{_('all')}}</span></td>
-      <td><span class="badge ">{{_('all')}}</span></td>
-      <td><span class="badge badge-info">{{_('all')}}</span></td>
-      <td><span class="badge badge-warning">{{_('all')}}</span></td>
-      <td><span class="badge badge-success">{{_('all')}}</span></td>
-    </tr>
-    <tr>
-      <td>
-        <div class="btn-group">
-          <a href="clash://install-config?url=https://{{domain}}/{{hconfigs[ConfigEnum.proxy_path]}}/{{user.uuid}}/clash/all.yml&name=new_normal_{{db_domain.alias or db_domain.domain}}-{{asn}}-{{mode}}&asn={{asn}}&mode={{mode}}"
-            class="btn btn-light orig-link"> {{_('user.home.allconfig.clash-configs')}}</a>
-        </div>
-      </td>
-      <td><span class="badge badge-danger">{{_('all')}}</span></td>
-      <td><span class="badge ">{{_('all')}}</span></td>
-      <td><span class="badge badge-info">{{_('user.home.allconfigs.expect_vless')}}</span></td>
-      <td><span class="badge badge-warning">{{_('all')}}</span></td>
-      <td><span class="badge badge-success">{{_('all')}}</span></td>
-    </tr>
-    <tr>
-      <td>
-        <div class="btn-group">
-          <a href="https://{{domain}}/{{hconfigs[ConfigEnum.proxy_path]}}/{{user.uuid}}/all.txt?name={{db_domain.alias or db_domain.domain}}-{{asn}}&asn={{asn}}&mode={{mode}}"
-            class="btn btn-light orig-link"> {{_('user.home.allconfig.link-configs')}}</a>
-        </div>
-      </td>
-      <td><span class="badge badge-danger">{{_('all')}}</span></td>
-      <td><span class="badge ">{{_('all')}}</span></td>
-      <td><span class="badge badge-info">{{_('all')}}</span></td>
-      <td><span class="badge badge-warning">{{_('all')}}</span></td>
-      <td><span class="badge badge-success">{{_('all')}}</span></td>
-    </tr>
-    <tr>
-      <td>
-        <div class="btn-group">
-          <a href="https://{{domain}}/{{hconfigs[ConfigEnum.proxy_path]}}/{{user.uuid}}/all.txt?name=new_link_{{db_domain.alias or db_domain.domain}}-{{asn}}-{{mode}}&asn={{asn}}&mode={{mode}}&base64=True"
-            class="btn btn-light orig-link"> {{_('user.home.allconfig.link-configs')}} b64</a>
-        </div>
-      </td>
-      <td><span class="badge badge-danger">{{_('all')}}</span></td>
-      <td><span class="badge ">{{_('all')}}</span></td>
-      <td><span class="badge badge-info">{{_('all')}}</span></td>
-      <td><span class="badge badge-warning">{{_('all')}}</span></td>
-      <td><span class="badge badge-success">{{_('all')}}</span></td>
-    </tr>
+      </tr>
+    </thead>
+    <tbody>
+      <tr>
+        <td>
+          <div class="btn-group">
+            <a href="clashmeta://install-config?url=https://{{domain}}/{{hconfigs[ConfigEnum.proxy_path]}}/{{user.uuid}}/clash/meta/all.yml&name=mnormal_{{db_domain.alias or db_domain.domain}}-{{asn}}-{{mode}}&asn={{asn}}&mode={{mode}}"
+              class="btn btn-light orig-link"> {{_('user.home.allconfig.hiddify-configs')}}</a>
+          </div>
+        </td>
+        <td><span class="badge badge-danger">{{_('all')}}</span></td>
+        <td><span class="badge ">{{_('all')}}</span></td>
+        <td><span class="badge badge-info">{{_('all')}}</span></td>
+        <td><span class="badge badge-warning">{{_('all')}}</span></td>
+        <td><span class="badge badge-success">{{_('all')}}</span></td>
+      </tr>
+      <tr>
+        <td>
+          <div class="btn-group">
+            <a href="clash://install-config?url=https://{{domain}}/{{hconfigs[ConfigEnum.proxy_path]}}/{{user.uuid}}/clash/all.yml&name=new_normal_{{db_domain.alias or db_domain.domain}}-{{asn}}-{{mode}}&asn={{asn}}&mode={{mode}}"
+              class="btn btn-light orig-link"> {{_('user.home.allconfig.clash-configs')}}</a>
+          </div>
+        </td>
+        <td><span class="badge badge-danger">{{_('all')}}</span></td>
+        <td><span class="badge ">{{_('all')}}</span></td>
+        <td><span class="badge badge-info">{{_('user.home.allconfigs.expect_vless')}}</span></td>
+        <td><span class="badge badge-warning">{{_('all')}}</span></td>
+        <td><span class="badge badge-success">{{_('all')}}</span></td>
+      </tr>
+      <tr>
+        <td>
+          <div class="btn-group">
+            <a href="https://{{domain}}/{{hconfigs[ConfigEnum.proxy_path]}}/{{user.uuid}}/all.txt?name={{db_domain.alias or db_domain.domain}}-{{asn}}&asn={{asn}}&mode={{mode}}"
+              class="btn btn-light orig-link"> {{_('user.home.allconfig.link-configs')}}</a>
+          </div>
+        </td>
+        <td><span class="badge badge-danger">{{_('all')}}</span></td>
+        <td><span class="badge ">{{_('all')}}</span></td>
+        <td><span class="badge badge-info">{{_('all')}}</span></td>
+        <td><span class="badge badge-warning">{{_('all')}}</span></td>
+        <td><span class="badge badge-success">{{_('all')}}</span></td>
+      </tr>
 
-%for d in domains
-%for t in (['http','tls'] if hconfig(ConfigEnum.http_proxy_enable,d.child_id) else ['tls'])
-%for port in hconfig(ConfigEnum.http_ports if t=='http' else ConfigEnum.tls_ports,d.child_id).split(',')
-%set phttp=port if t=='http' else None
-%set ptls=port if t=='tls' else None
-% for type in link_maker.all_proxies(d.child_id)
-% set pinfo=link_maker.make_proxy(type,d,phttp=phttp,ptls=ptls)
-% if 'msg' not in  pinfo
-    <tr>
-      <td>
-        <div class="btn-group"><a href='{{link_maker.to_link(pinfo)}}'
-            class="btn btn-light orig-link">{{pinfo["name"].replace("_", " ")}}</a></div>
-      </td>
-      <td><span class="badge badge-danger"> {% if d.has_auto_ip  %}Auto {%endif%}{{pinfo["mode"]}}</span></td>
-      <td><span class="badge ltr">{{d.domain}}</span></td>
-      <td><span class="badge badge-info">{{pinfo["proto"]}}</span></td>
-      <td><span class="badge badge-warning">{{pinfo['transport']}}</span></td>
-      <td><span class="badge badge-success">{{pinfo['l3']}}</span></td>
-    </tr>
-    
-  %endif
-  % endfor
-  % endfor
-  % endfor
-  % endfor
-  </tbody>
-</table>
+      <tr>
+        <td>
+          <div class="btn-group">
+            <a href="https://{{domain}}/{{hconfigs[ConfigEnum.proxy_path]}}/{{user.uuid}}/singbox.json?name={{db_domain.alias or db_domain.domain}}-{{asn}}&asn={{asn}}&mode={{mode}}"
+              class="btn btn-light orig-link"> {{_('singbox: ssh')}}</a>
+          </div>
+        </td>
+        <td><span class="badge badge-danger">{{_('ssh')}}</span></td>
+        <td><span class="badge ">{{_('ssh')}}</span></td>
+        <td><span class="badge badge-info">{{_('ssh')}}</span></td>
+        <td><span class="badge badge-warning">{{_('ssh')}}</span></td>
+        <td><span class="badge badge-success">{{_('ssh')}}</span></td>
+      </tr>
+      <tr>
+        <td>
+          <div class="btn-group">
+            <a href="https://{{domain}}/{{hconfigs[ConfigEnum.proxy_path]}}/{{user.uuid}}/all.txt?name=new_link_{{db_domain.alias or db_domain.domain}}-{{asn}}-{{mode}}&asn={{asn}}&mode={{mode}}&base64=True"
+              class="btn btn-light orig-link"> {{_('user.home.allconfig.link-configs')}} b64</a>
+          </div>
+        </td>
+        <td><span class="badge badge-danger">{{_('all')}}</span></td>
+        <td><span class="badge ">{{_('all')}}</span></td>
+        <td><span class="badge badge-info">{{_('all')}}</span></td>
+        <td><span class="badge badge-warning">{{_('all')}}</span></td>
+        <td><span class="badge badge-success">{{_('all')}}</span></td>
+      </tr>
+
+      %for d in domains
+      %for t in (['http','tls'] if hconfig(ConfigEnum.http_proxy_enable,d.child_id) else ['tls'])
+      %for port in hconfig(ConfigEnum.http_ports if t=='http' else ConfigEnum.tls_ports,d.child_id).split(',')
+      %set phttp=port if t=='http' else None
+      %set ptls=port if t=='tls' else None
+      % for type in link_maker.all_proxies(d.child_id)
+      % set pinfo=link_maker.make_proxy(type,d,phttp=phttp,ptls=ptls)
+      % if 'msg' not in pinfo
+      <tr>
+        <td>
+          <div class="btn-group"><a href='{{link_maker.to_link(pinfo)}}' class="btn btn-light orig-link">{{pinfo["name"].replace("_", " ")}}</a></div>
+        </td>
+        <td><span class="badge badge-danger"> {% if d.has_auto_ip %}Auto {%endif%}{{pinfo["mode"]}}</span></td>
+        <td><span class="badge ltr">{{d.domain}}</span></td>
+        <td><span class="badge badge-info">{{pinfo["proto"]}}</span></td>
+        <td><span class="badge badge-warning">{{pinfo['transport']}}</span></td>
+        <td><span class="badge badge-success">{{pinfo['l3']}}</span></td>
+      </tr>
+
+      %endif
+      % endfor
+      % endfor
+      % endfor
+      % endfor
+    </tbody>
+  </table>
 </div>
```

#### html2text {}

```diff
@@ -5,11 +5,12 @@
 ('user.home.allconfig.hiddify- {{_('all')}}                   {{_('all')}} {{_('all')}}                            {{_('all')}}                        {{_('all')}}
 configs')}}
 {{_                                                                        {{_
 ('user.home.allconfig.clash-   {{_('all')}}                   {{_('all')}} ('user.home.allconfigs.expect_vless')}} {{_('all')}}                        {{_('all')}}
 configs')}}
 {{_('user.home.allconfig.link- {{_('all')}}                   {{_('all')}} {{_('all')}}                            {{_('all')}}                        {{_('all')}}
 configs')}}
+{{_('singbox:_ssh')}}          {{_('ssh')}}                   {{_('ssh')}} {{_('ssh')}}                            {{_('ssh')}}                        {{_('ssh')}}
 {{_('user.home.allconfig.link- {{_('all')}}                   {{_('all')}} {{_('all')}}                            {{_('all')}}                        {{_('all')}}
 configs')}}_b64
 {{pinfo["name"].replace("_",_" {% if d.has_auto_ip %}Auto     {{d.domain}} {{pinfo["proto"]}}                      {{pinfo['transport']}}              {{pinfo['l3']}}
 ")}}                           {%endif%}{{pinfo["mode"]}}
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/all-configs_old.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/all-configs_old.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/android.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/android.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/base2.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/base2.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/clash-links copy.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/clash-links copy.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/clash-links.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/clash-links.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/index copy.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/index copy.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/index_old.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/index_old.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/ios copy.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/ios copy.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/ios.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/ios.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/multi.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/multi.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/speedtest.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/speedtest.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/telegram.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/telegram.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/usage.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/usage.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/templates/home/windows.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/templates/home/windows.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/panel/user/user.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/panel/user/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,26 +67,27 @@
         c = get_common_data(g.user_uuid, mode)
 
         hash_rnd = random.randint(0, 1000000)  # hash(f'{c}')
         if request.method == 'HEAD':
             resp = Response("")
         else:
             resp = Response(render_template('clash_config.yml', typ=typ, meta_or_normal=meta_or_normal, **c, hash=hash_rnd))
-        resp.mimetype = "text/plain"
-        resp.headers['Subscription-Userinfo'] = f"upload=0;download={c['usage_current_b']};total={c['usage_limit_b']};expire={c['expire_s']}"
-        resp.headers['profile-web-page-url'] = request.base_url.split("clash")[0].replace("http://", "https://")
-        if hconfig(ConfigEnum.branding_site):
-            resp.headers['support-url'] = hconfig(ConfigEnum.branding_site)
-        resp.headers['profile-update-interval'] = 1
-
-        profile_title = f'{c["db_domain"].alias or c["db_domain"].domain} {c["user"].name}'
-        if c['has_auto_cdn']:
-            profile_title += f" {c['asn']}"
-        resp.headers['profile-title'] = 'base64:'+do_base_64(profile_title)
-        return resp
+
+        return add_headers(resp, c)
+
+    @route('/singbox.json', methods=["GET", "HEAD"])
+    def singbox(self):
+        mode = "new"  # request.args.get("mode")
+        c = get_common_data(g.user_uuid, mode)
+        # response.content_type = 'text/plain';
+        if request.method == 'HEAD':
+            resp = ""
+        else:
+            resp = render_template('singbox_config.json', **c, host_keys=hiddify.get_hostkeys(True), ssh_client_version=hiddify.get_ssh_client_version(user), base64=False)
+        return add_headers(resp, c)
 
     @route('/all.txt', methods=["GET", "HEAD"])
     def all_configs(self):
         mode = "new"  # request.args.get("mode")
         base64 = request.args.get("base64", "").lower() == "true"
         c = get_common_data(g.user_uuid, mode)
         # response.content_type = 'text/plain';
@@ -98,28 +99,15 @@
         res = ""
         for line in resp.split("\n"):
             if "vmess://" in line:
                 line = "vmess://"+do_base_64(line.replace("vmess://", ""))
             res += line+"\n"
         if base64:
             res = do_base_64(res)
-        resp = Response(res)
-        resp.mimetype = "text/plain"
-        resp.headers['Subscription-Userinfo'] = f"upload=0;download={c['usage_current_b']};total={c['usage_limit_b']};expire={c['expire_s']}"
-        resp.headers['profile-web-page-url'] = request.base_url.split("all.txt")[0].replace("http://", "https://")
-        if hconfig(ConfigEnum.branding_site):
-            resp.headers['support-url'] = hconfig(ConfigEnum.branding_site)
-        resp.headers['profile-update-interval'] = 1
-        # resp.headers['content-disposition']=f'attachment; filename="{c["db_domain"].alias or c["db_domain"].domain} {c["user"].name}"'
-        profile_title = f'{c["db_domain"].alias or c["db_domain"].domain} {c["user"].name}'
-        if c['has_auto_cdn']:
-            profile_title += f" {c['asn']}"
-        resp.headers['profile-title'] = 'base64:'+do_base_64(profile_title)
-
-        return resp
+        return add_headers(res, c)
 
     @route('/manifest.webmanifest')
     def create_pwa_manifest(self):
 
         domain = urlparse(request.base_url).hostname
         name = (domain if g.is_admin else g.user.name)
         return jsonify({
@@ -255,7 +243,25 @@
         "telegram_enable": hconfig(ConfigEnum.telegram_enable) and any([d for d in domains if d.mode in [DomainType.direct, DomainType.relay, DomainType.old_xtls_direct]]),
         "ip": user_ip,
         "ip_debug": clean_ip.get_real_user_ip_debug(user_ip),
         "asn": clean_ip.get_asn_short_name(user_ip),
         "country": clean_ip.get_country(user_ip),
         'has_auto_cdn': has_auto_cdn
     }
+
+
+def add_headers(res, c):
+    resp = Response(res)
+    resp.mimetype = "text/plain"
+    resp.headers['Subscription-Userinfo'] = f"upload=0;download={c['usage_current_b']};total={c['usage_limit_b']};expire={c['expire_s']}"
+    resp.headers['profile-web-page-url'] = request.base_url.rsplit('/', 1)[0].replace("http://", "https://")+"/"
+
+    if hconfig(ConfigEnum.branding_site):
+        resp.headers['support-url'] = hconfig(ConfigEnum.branding_site)
+    resp.headers['profile-update-interval'] = 1
+    # resp.headers['content-disposition']=f'attachment; filename="{c["db_domain"].alias or c["db_domain"].domain} {c["user"].name}"'
+    profile_title = f'{c["db_domain"].alias or c["db_domain"].domain} {c["user"].name}'
+    if c['has_auto_cdn']:
+        profile_title += f" {c['asn']}"
+    resp.headers['profile-title'] = 'base64:'+do_base_64(profile_title)
+
+    return resp
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/singbox_api.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/drivers/singbox_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 import xtlsapi
 from hiddifypanel.models import *
+from .abstract_driver import DriverABS
 
 
-def get_singbox_client():
-    if hconfig(ConfigEnum.is_parent):
-        return
-    return xtlsapi.SingboxClient('127.0.0.1', 10086)
-
-
-def get_enabled_users():
-    if hconfig(ConfigEnum.is_parent):
-        return
-
-
-def get_inbound_tags():
-    if hconfig(ConfigEnum.is_parent):
-        return
-    try:
-        xray_client = get_singbox_client()
-        inbounds = [inb.name.split(">>>")[1] for inb in xray_client.stats_query('inbound')]
-        print(f"Success in get inbound tags {inbounds}")
-    except Exception as e:
-        print(f"error in get inbound tags {e}")
-        inbounds = []
-    return list(set(inbounds))
-
-
-def add_client(uuid):
-    if hconfig(ConfigEnum.is_parent):
-        return
-    raise NotImplementedError()
-
-
-def remove_client(uuid):
-    if hconfig(ConfigEnum.is_parent):
-        return
-    raise NotImplementedError()
-
-
-def get_usage(uuid, reset=False):
-    if hconfig(ConfigEnum.is_parent):
-        return
-    xray_client = get_singbox_client()
-    d = xray_client.get_client_download_traffic(f'{uuid}@hiddify.com', reset=reset)
-    u = xray_client.get_client_upload_traffic(f'{uuid}@hiddify.com', reset=reset)
-    print(f"Success {uuid} d={d} u={u}")
-    res = None
-    if d is None:
-        res = u
-    elif u is None:
-        res = d
-    else:
-        res = d + u
-    return res
+class SingboxApi(DriverABS):
+    def get_singbox_client(self):
+        if hconfig(ConfigEnum.is_parent):
+            return
+        return xtlsapi.SingboxClient('127.0.0.1', 10086)
+
+    def get_enabled_users(self):
+        if hconfig(ConfigEnum.is_parent):
+            return
+
+    def get_inbound_tags():
+        if hconfig(ConfigEnum.is_parent):
+            return
+        try:
+            xray_client = self.get_singbox_client()
+            inbounds = [inb.name.split(">>>")[1] for inb in xray_client.stats_query('inbound')]
+            print(f"Success in get inbound tags {inbounds}")
+        except Exception as e:
+            print(f"error in get inbound tags {e}")
+            inbounds = []
+        return list(set(inbounds))
+
+    def add_client(user):
+        if hconfig(ConfigEnum.is_parent):
+            return
+        # raise NotImplementedError()
+
+    def remove_client(user):
+        if hconfig(ConfigEnum.is_parent):
+            return
+        # raise NotImplementedError()
+
+    def get_usage(uuid, reset=False):
+        if hconfig(ConfigEnum.is_parent):
+            return
+        xray_client = self.get_singbox_client()
+        d = xray_client.get_client_download_traffic(f'{uuid}@hiddify.com', reset=reset)
+        u = xray_client.get_client_upload_traffic(f'{uuid}@hiddify.com', reset=reset)
+        print(f"Success {uuid} d={d} u={u}")
+        res = None
+        if d is None:
+            res = u
+        elif u is None:
+            res = d
+        else:
+            res = d + u
+        return res
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/a.txt` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/a.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/css/adminlte.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/adminlte.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/css/adminlte.fa.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/adminlte.fa.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/css/adminlte.rtl.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/adminlte.rtl.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/css/bootstrap.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/css/bootstrap4-rtl.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/bootstrap4-rtl.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/css/bootstrap5.rtl.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/bootstrap5.rtl.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/css/custom.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/css/font-awesome.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/css/lte.old` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/css/lte.old`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Black.eot` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Black.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Black.ttf` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Black.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Black.woff` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Black.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Black.woff2` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Black.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Bold.eot` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Bold.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Bold.ttf` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Bold.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Bold.woff` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Bold.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Bold.woff2` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Bold.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Light.eot` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Light.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Light.ttf` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Light.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Light.woff` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Light.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Light.woff2` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Light.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Medium.eot` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Medium.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Medium.ttf` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Medium.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Medium.woff` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Medium.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Medium.woff2` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Medium.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Thin.eot` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Thin.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Thin.ttf` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Thin.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Thin.woff` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Thin.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir-Thin.woff2` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir-Thin.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir.eot` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir.ttf` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir.woff` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/fonts/Vazir.woff2` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/fonts/Vazir.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/WhiteLogo.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/WhiteLogo.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/favicon.ico` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/hiddify-dark.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/hiddify-dark.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/hiddify.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/hiddify.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/no_back_hiddify.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/no_back_hiddify.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/pwa-icon.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/pwa-icon.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/splash/ipad_splash.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/ipad_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/splash/ipadpro1_splash.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/ipadpro1_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/splash/ipadpro2_splash.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/ipadpro2_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/splash/ipadpro3_splash.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/ipadpro3_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/splash/iphone5_splash.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/iphone5_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/splash/iphone6_splash.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/iphone6_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/splash/iphoneplus_splash.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/iphoneplus_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/splash/iphonex_splash.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/iphonex_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/splash/iphonexr_splash.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/iphonexr_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/images/splash/iphonexsmax_splash.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/images/splash/iphonexsmax_splash.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/js/adminlte.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/adminlte.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/js/bootbox.all.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/bootbox.all.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/js/bootbox.all.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/bootbox.all.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/js/bootstrap.bundle.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/js/bootstrap.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/js/custom-rtl.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/custom-rtl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/js/custom.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/custom.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/js/demo.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/demo.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/js/jquery-3.6.1.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/jquery-3.6.1.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/js/js.cookie.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/js.cookie.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/js/moment.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/moment.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/js/popper.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/js/pwa.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/pwa.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/js/qrcode.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/js/qrcode.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/css/bootstrap.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/css/bootstrap.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/js/bootstrap.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap/js/bootstrap.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap-slider/bootstrap-slider.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap-slider/bootstrap-slider.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap-slider/slider.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap-slider/slider.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap4-editable/css/bootstrap-editable.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap4-editable/css/bootstrap-editable.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap4-editable/img/loading.gif` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap4-editable/img/loading.gif`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/bootstrap4-editable/js/bootstrap-editable.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/chart.js/Chart.bundle.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/chart.js/Chart.bundle.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/chart.js/Chart.bundle.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/chart.js/Chart.bundle.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/chart.js/Chart.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/chart.js/Chart.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/chart.js/Chart.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/chart.js/Chart.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/chartjs-old/Chart.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/chartjs-old/Chart.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/chartjs-old/Chart.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/chartjs-old/Chart.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/ckeditor.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/ckeditor.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ar.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ar.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ast.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ast.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/bg.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/bg.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/cs.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/cs.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/da.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/da.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/de.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/de.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/el.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/el.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/en-au.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/en-au.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/eo.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/eo.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/es.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/es.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/et.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/et.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/eu.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/eu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/fi.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/fi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/fr.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/fr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/gl.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/gl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/gu.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/gu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/hr.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/hr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/hu.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/hu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/it.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/it.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ja.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ja.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/km.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/km.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/kn.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/kn.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ko.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ko.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ku.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ku.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/nb.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/nb.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ne.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ne.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/nl.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/nl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/oc.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/oc.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/pl.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/pl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/pt-br.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/pt-br.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/pt.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/pt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ro.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ro.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ru.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ru.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/si.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/si.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/sk.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/sk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/sq.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/sq.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/sv.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/sv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/tr.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/tr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/tt.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/tt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/ug.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/ug.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/uk.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/uk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/zh-cn.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/zh-cn.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ckeditor/translations/zh.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ckeditor/translations/zh.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/bootstrap-colorpicker.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/img/alpha-horizontal.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/img/alpha-horizontal.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/img/alpha.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/img/alpha.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/img/hue-horizontal.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/img/hue-horizontal.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/img/hue.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/img/hue.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/colorpicker/img/saturation.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/colorpicker/img/saturation.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/dataTables.bootstrap4.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/AutoFill/Readme.txt` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/AutoFill/Readme.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/filler.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/AutoFill/images/filler.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/AutoFill/js/dataTables.autoFill.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/License.txt` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/License.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/Readme.md` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/Readme.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/insert.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/images/insert.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColReorder/js/dataTables.colReorder.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/License.txt` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/License.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/Readme.md` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/Readme.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colVis.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colvis.jqueryui.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/css/dataTables.colvis.jqueryui.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/ColVis/js/dataTables.colVis.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/License.txt` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/License.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/Readme.md` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/Readme.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/css/dataTables.fixedColumns.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedColumns/js/dataTables.fixedColumns.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/Readme.txt` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/Readme.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/FixedHeader/js/dataTables.fixedHeader.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/KeyTable/Readme.txt` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/KeyTable/Readme.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/KeyTable/js/dataTables.keyTable.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/License.txt` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/License.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.scss` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/dataTables.responsive.scss`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/responsive.bootstrap4.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/css/responsive.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/dataTables.responsive.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/responsive.bootstrap4.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Responsive/js/responsive.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/Readme.txt` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/Readme.txt`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/css/dataTables.scroller.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/loading-background.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/images/loading-background.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/Scroller/js/dataTables.scroller.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/Readme.md` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/Readme.md`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/css/dataTables.tableTools.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection_hover.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/collection_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy_hover.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/copy_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv_hover.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/csv_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf_hover.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/pdf_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print_hover.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/print_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls_hover.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/images/xls_hover.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/js/dataTables.tableTools.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls.swf` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls.swf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls_pdf.swf` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/extensions/TableTools/swf/copy_csv_xls_pdf.swf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/jquery.dataTables.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/jquery.dataTables.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/jquery.dataTables.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datatables/jquery.dataTables_themeroller.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datatables/jquery.dataTables_themeroller.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/bootstrap-datepicker.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/datepicker3.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/datepicker3.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ar.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ar.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.az.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.az.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.bg.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.bg.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ca.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ca.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cs.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cs.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cy.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.cy.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.da.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.da.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.de.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.de.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.el.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.el.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.es.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.es.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.et.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.et.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fa.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fa.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fi.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fr.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.fr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.gl.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.gl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.he.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.he.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hr.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hu.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.hu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.id.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.id.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.is.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.is.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.it.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.it.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ja.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ja.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ka.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ka.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kk.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kr.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.kr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lt.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lv.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.lv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.mk.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.mk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ms.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ms.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nb.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nb.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl-BE.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl-BE.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.nl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.no.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.no.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pl.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt-BR.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt-BR.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.pt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ro.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ro.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs-latin.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs-latin.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.rs.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ru.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ru.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sk.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sl.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sq.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sq.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sv.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sw.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.sw.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.th.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.th.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.tr.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.tr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ua.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.ua.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.vi.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.vi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-CN.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-CN.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-TW.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/datepicker/locales/bootstrap-datepicker.zh-TW.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/daterangepicker/daterangepicker-bs3.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/daterangepicker/daterangepicker-bs3.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/daterangepicker/daterangepicker.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/daterangepicker/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/daterangepicker/moment.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/daterangepicker/moment.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/daterangepicker/moment.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/daterangepicker/moment.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/fastclick/fastclick.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fastclick/fastclick.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/fastclick/fastclick.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fastclick/fastclick.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/excanvas.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/excanvas.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/excanvas.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/excanvas.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.colorhelpers.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.colorhelpers.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.colorhelpers.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.colorhelpers.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.canvas.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.canvas.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.canvas.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.canvas.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.categories.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.categories.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.categories.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.categories.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.crosshair.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.errorbars.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.fillbetween.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.image.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.image.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.image.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.image.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.navigate.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.navigate.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.navigate.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.navigate.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.pie.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.pie.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.pie.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.pie.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.resize.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.resize.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.resize.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.resize.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.selection.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.selection.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.selection.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.selection.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.stack.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.stack.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.stack.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.stack.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.symbol.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.symbol.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.symbol.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.symbol.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.threshold.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.threshold.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.threshold.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.threshold.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.time.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.time.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/flot/jquery.flot.time.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/flot/jquery.flot.time.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css.map` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/css/font-awesome.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/fonts/FontAwesome.otf` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.eot` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.svg` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.ttf` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff2` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/fullcalendar/fullcalendar.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fullcalendar/fullcalendar.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/fullcalendar/fullcalendar.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fullcalendar/fullcalendar.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fullcalendar/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/fullcalendar/fullcalendar.print.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/fullcalendar/fullcalendar.print.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/all.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/_all.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/_all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/aero.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/aero.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/aero.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/aero.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/aero@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/aero@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/blue.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/blue.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/blue.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/blue.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/blue@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/blue@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/flat.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/flat.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/flat.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/flat.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/flat@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/flat@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/green.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/green.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/green.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/green.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/green@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/green@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/grey.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/grey.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/grey.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/grey.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/grey@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/grey@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/orange.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/orange.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/orange.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/orange.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/orange@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/orange@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/pink.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/pink.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/pink.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/pink.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/pink@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/pink@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/purple.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/purple.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/purple.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/purple.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/purple@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/purple@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/red.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/red.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/red.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/red.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/red@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/red@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/yellow.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/yellow.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/yellow.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/yellow.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/flat/yellow@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/flat/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/futurico/futurico.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/futurico/futurico.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/futurico/futurico.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/futurico/futurico.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/futurico/futurico@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/futurico/futurico@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/icheck.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/icheck.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/icheck.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/icheck.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/_all.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/_all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/aero.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/aero.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/blue.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/blue.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/green.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/green.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/grey.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/grey.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/line.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/line.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/line.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/line.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/line@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/line@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/orange.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/orange.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/pink.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/pink.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/purple.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/purple.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/red.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/red.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/line/yellow.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/line/yellow.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/_all.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/_all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/aero.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/aero.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/aero.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/aero.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/aero@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/aero@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/blue.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/blue.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/blue.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/blue.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/blue@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/blue@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/green.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/green.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/green.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/green.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/green@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/green@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/grey.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/grey.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/grey.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/grey.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/grey@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/grey@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/minimal.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/minimal.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/minimal.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/minimal.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/minimal@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/minimal@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/orange.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/orange.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/orange.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/orange.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/orange@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/orange@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/pink.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/pink.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/pink.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/pink.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/pink@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/pink@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/purple.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/purple.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/purple.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/purple.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/purple@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/purple@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/red.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/red.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/red.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/red.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/red@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/red@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/yellow.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/yellow.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/yellow.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/yellow.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/minimal/yellow@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/minimal/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/polaris/polaris.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/polaris/polaris.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/polaris/polaris.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/polaris/polaris.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/polaris/polaris@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/polaris/polaris@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/_all.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/_all.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/aero.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/aero.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/aero.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/aero.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/aero@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/aero@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/blue.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/blue.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/blue.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/blue.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/blue@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/blue@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/green.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/green.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/green.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/green.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/green@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/green@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/grey.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/grey.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/grey.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/grey.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/grey@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/grey@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/orange.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/orange.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/orange.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/orange.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/orange@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/orange@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/pink.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/pink.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/pink.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/pink.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/pink@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/pink@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/purple.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/purple.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/purple.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/purple.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/purple@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/purple@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/red.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/red.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/red.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/red.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/red@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/red@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/square.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/square.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/square.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/square.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/square@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/square@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/yellow.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/yellow.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/yellow.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/yellow.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/iCheck/square/yellow@2x.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/iCheck/square/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/jquery.inputmask.date.extensions.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/jquery.inputmask.date.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/jquery.inputmask.extensions.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/jquery.inputmask.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/jquery.inputmask.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/jquery.inputmask.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/jquery.inputmask.numeric.extensions.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/jquery.inputmask.numeric.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/jquery.inputmask.phone.extensions.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/jquery.inputmask.phone.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/jquery.inputmask.regex.extensions.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/jquery.inputmask.regex.extensions.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/phone-codes/phone-be.json` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/phone-codes/phone-be.json`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/input-mask/phone-codes/phone-codes.json` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/input-mask/phone-codes/phone-codes.json`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ionslider/img/sprite-skin-nice.png` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ionslider/img/sprite-skin-nice.png`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinFlat.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinFlat.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinNice.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/ionslider/ion.rangeSlider.skinNice.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/jQueryUI/jquery-ui.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jQueryUI/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/jQueryUI/jquery-ui.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jQueryUI/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/core.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/core.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/jquery.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/jquery.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/jquery.min.map` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/jquery.min.map`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/jquery.slim.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/jquery.slim.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/jquery.slim.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/jquery/jquery.slim.min.map` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jquery/jquery.slim.min.map`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-usa-en.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-usa-en.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-world-mill-en.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/jvectormap/jquery-jvectormap-world-mill-en.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/knob/jquery.knob.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/knob/jquery.knob.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/morris/morris.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/morris/morris.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/morris/morris.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/morris/morris.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/pace/pace.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/pace/pace.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/pace/pace.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/pace/pace.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/pace/pace.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/pace/pace.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/pace/pace.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/pace/pace.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/esm/popper-utils.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/esm/popper-utils.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/esm/popper-utils.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/esm/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/esm/popper.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/esm/popper.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/esm/popper.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/esm/popper.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/popper-utils.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/popper-utils.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/popper-utils.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/popper.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/popper.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/popper.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/popper.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/umd/popper-utils.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/umd/popper-utils.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/umd/popper-utils.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/umd/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/umd/popper.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/umd/popper.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/popper/umd/popper.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/popper/umd/popper.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/az.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/az.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/bg.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/ca.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/cs.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/da.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/da.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/de.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/de.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/en.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/en.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/es.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/es.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/et.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/et.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/eu.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/fa.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/fi.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/fr.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/gl.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/he.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/he.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/hi.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/hr.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/hu.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/id.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/id.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/is.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/is.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/it.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/it.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/ko.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/lt.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/lv.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/mk.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/nb.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/nl.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/pl.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/pt-BR.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/pt.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/ro.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/ru.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/sk.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/sr.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/sv.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/th.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/th.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/tr.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/uk.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/vi.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/zh-CN.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/i18n/zh-TW.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/select2.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/select2.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/select2.full.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/select2.full.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/select2.full.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/select2.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/select2.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/select2.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/select2.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/select2/select2.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/select2/select2.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/slimScroll/jquery.slimscroll.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/sparkline/jquery.sparkline.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/sparkline/jquery.sparkline.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/sparkline/jquery.sparkline.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/sparkline/jquery.sparkline.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.css` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.css`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.js` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/plugins/timepicker/bootstrap-timepicker.min.js`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-brands-400.ttf` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-brands-400.woff2` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-regular-400.ttf` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-regular-400.woff2` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-solid-900.ttf` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-solid-900.woff2` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-v4compatibility.ttf` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/static/webfonts/fa-v4compatibility.woff2` & `hiddifypanel-8.0.0.dev0/hiddifypanel/static/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/templates/500.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/templates/500.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/templates/admin-layout.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/templates/admin-layout.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/templates/admin.ht.old` & `hiddifypanel-8.0.0.dev0/hiddifypanel/templates/admin.ht.old`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/templates/donation.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/templates/donation.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/templates/flaskadmin-layout.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/templates/flaskadmin-layout.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/templates/hiddify-flask-admin/list.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/templates/hiddify-flask-admin/list.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/templates/lte-master.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/templates/lte-master.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/templates/macros.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/templates/macros.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/templates/master.html` & `hiddifypanel-8.0.0.dev0/hiddifypanel/templates/master.html`

 * *Files identical despite different names*

### Comparing `hiddifypanel-7.1.9/hiddifypanel/translations/en/LC_MESSAGES/messages.mo` & `hiddifypanel-8.0.0.dev0/hiddifypanel/translations/en/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  HiddifyPanel\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-30 16:43+0200\n"
-"PO-Revision-Date: 2023-07-30 09:30-0500\n"
+"POT-Creation-Date: 2023-08-03 10:13+0200\n"
+"PO-Revision-Date: 2023-07-30 09:43-0500\n"
 "Last-Translator: hidden u\n"
 "Language: en_US\n"
 "Language-Team: English (USA)\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -1463,14 +1463,38 @@
 msgstr ""
 "Please use a well known domain in your data center. for example, If you are "
 "in Azure data center, microsoft-update.com Is a good example"
 
 msgid "config.ssfaketls_fakedomain.label"
 msgstr "🌍 SS FakeTLS FakeDomain"
 
+msgid "config.ssh.description"
+msgstr "config.ssh.description"
+
+msgid "config.ssh.label"
+msgstr "config.ssh.label"
+
+msgid "config.ssh_server_enable.description"
+msgstr "config.ssh_server_enable.description"
+
+msgid "config.ssh_server_enable.label"
+msgstr "config.ssh_server_enable.label"
+
+msgid "config.ssh_server_ports.description"
+msgstr "config.ssh_server_ports.description"
+
+msgid "config.ssh_server_ports.label"
+msgstr "config.ssh_server_ports.label"
+
+msgid "config.ssh_server_redis_url.description"
+msgstr "config.ssh_server_redis_url.description"
+
+msgid "config.ssh_server_redis_url.label"
+msgstr "config.ssh_server_redis_url.label"
+
 msgid "config.ssr.description"
 msgstr ""
 "ShadowsocksR is a fork of the original Shadowsocks project, claimed to be "
 "superior in terms of security and stability."
 
 msgid "config.ssr.label"
 msgstr "SSR"
@@ -1805,14 +1829,20 @@
 msgid ""
 "selected domain for REALITY is not in the same ASN. To better use of the "
 "protocol, it is better to find a domain in the same ASN."
 msgstr ""
 "Selected Domain for REALITY is not in the same ASN. To better use of the "
 "Protocol, it is better to find a Domain in the same ASN"
 
+msgid "singbox: ssh"
+msgstr "singbox: ssh"
+
+msgid "ssh"
+msgstr "ssh"
+
 msgid "sub_link_only"
 msgstr "📳 Only for Subscription Link (can be Direct, Relay, or CDN)"
 
 msgid "telegram"
 msgstr "Telegram"
 
 msgid "test"
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/translations/en/LC_MESSAGES/messages.po` & `hiddifypanel-8.0.0.dev0/hiddifypanel/translations/en/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,96 +1,96 @@
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: HiddifyPanel\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-30 16:43+0200\n"
-"PO-Revision-Date: 2023-07-30 09:30-0500\n"
+"POT-Creation-Date: 2023-08-03 10:13+0200\n"
+"PO-Revision-Date: 2023-07-30 09:43-0500\n"
 "Last-Translator: hidden u\n"
 "Language-Team: English (USA)\n"
 "Language: en_US\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "Generated-By: Babel 2.12.1\n"
 
 # | msgid "This Domain does not exist in the Panel !"
-#: hiddifypanel/models/domain.py:134 hiddifypanel/panel/user/user.py:177
+#: hiddifypanel/models/domain.py:134 hiddifypanel/panel/user/user.py:165
 msgid "This domain does not exist in the panel!"
 msgstr "This Domain does not exist in the Panel !"
 
 # | msgid "Error In Auto CDN IP! It Can Not Be Find, Please Contact Admin"
 #: hiddifypanel/panel/clean_ip.py:103
 msgid "Error! auto cdn ip can not be find, please contact admin."
 msgstr "Error In Auto CDN IP! It Can Not Be Find, Please Contact Admin"
 
-#: hiddifypanel/panel/hiddify.py:76
+#: hiddifypanel/panel/hiddify.py:78
 #, fuzzy
 msgid "Access Denied"
 msgstr "Access Denied"
 
 # | msgid "Apply Configs"
-#: hiddifypanel/panel/hiddify.py:221
+#: hiddifypanel/panel/hiddify.py:223
 msgid "admin.config.apply_configs"
 msgstr "Apply Configs"
 
 # | msgid ""
 # | "Configs have been changed successfully. Click %(link)s to apply the "
 # | "configs. It may take 2 minutes to apply"
-#: hiddifypanel/panel/hiddify.py:222
+#: hiddifypanel/panel/hiddify.py:224
 msgid "config.validation-success"
 msgstr ""
 "Configs have been changed successfully. Click %(link)s to apply the configs."
 " It may take 2 minutes to apply"
 
 # | msgid " ✅ Configs have been changed successfully"
-#: hiddifypanel/panel/hiddify.py:224
+#: hiddifypanel/panel/hiddify.py:226
 msgid "config.validation-success-no-reset"
 msgstr " ✅ Configs have been changed successfully"
 
 # | msgid ""
 # | "Domain can not be resolved! There is a problem in your domain. Please "
 # | "check your Domain configurations."
 #: hiddifypanel/panel/admin/ChildAdmin.py:106
 #: hiddifypanel/panel/admin/DomainAdmin.py:154
 #: hiddifypanel/panel/admin/DomainAdmin.py:176
 #: hiddifypanel/panel/admin/DomainAdmin.py:179
 #: hiddifypanel/panel/admin/QuickSetup.py:126
 #: hiddifypanel/panel/commercial/ParentDomainAdmin.py:107
-#: hiddifypanel/panel/hiddify.py:343
+#: hiddifypanel/panel/hiddify.py:345
 msgid "Domain can not be resolved! there is a problem in your domain"
 msgstr ""
 "Domain can not be resolved! There is a problem in your domain. Please check "
 "your Domain configurations."
 
 # | msgid "Last Day"
-#: hiddifypanel/panel/hiddify.py:371
+#: hiddifypanel/panel/hiddify.py:373
 msgid "0 - Last day"
 msgstr "Last Day"
 
 # | msgid ""
 # | "Selected Domain for REALITY is not in the same ASN. To better use of the
 # "
 # | "Protocol, it is better to find a Domain in the same ASN"
-#: hiddifypanel/panel/hiddify.py:652
+#: hiddifypanel/panel/hiddify.py:654
 msgid ""
 "selected domain for REALITY is not in the same ASN. To better use of the "
 "protocol, it is better to find a domain in the same ASN."
 msgstr ""
 "Selected Domain for REALITY is not in the same ASN. To better use of the "
 "Protocol, it is better to find a Domain in the same ASN"
 
 # | msgid "User Activated"
-#: hiddifypanel/panel/usage.py:113
+#: hiddifypanel/panel/usage.py:102
 msgid "User activated!"
 msgstr "User Activated"
 
 # | msgid "Package Ended"
-#: hiddifypanel/panel/usage.py:113
+#: hiddifypanel/panel/usage.py:102
 msgid "Package ended!"
 msgstr "Package Ended"
 
 # | msgid ""
 # | "⚠️ Your Domains Changed. please do not forget to copy Admin links, "
 # | "otherwise you can not access to the panel anymore"
 #: hiddifypanel/panel/admin/Actions.py:108
@@ -2734,19 +2734,19 @@
 #: hiddifypanel/panel/user/templates/home/all-configs.html:40
 #: hiddifypanel/panel/user/templates/home/all-configs.html:41
 #: hiddifypanel/panel/user/templates/home/all-configs.html:50
 #: hiddifypanel/panel/user/templates/home/all-configs.html:51
 #: hiddifypanel/panel/user/templates/home/all-configs.html:52
 #: hiddifypanel/panel/user/templates/home/all-configs.html:53
 #: hiddifypanel/panel/user/templates/home/all-configs.html:54
-#: hiddifypanel/panel/user/templates/home/all-configs.html:63
-#: hiddifypanel/panel/user/templates/home/all-configs.html:64
-#: hiddifypanel/panel/user/templates/home/all-configs.html:65
-#: hiddifypanel/panel/user/templates/home/all-configs.html:66
-#: hiddifypanel/panel/user/templates/home/all-configs.html:67
+#: hiddifypanel/panel/user/templates/home/all-configs.html:77
+#: hiddifypanel/panel/user/templates/home/all-configs.html:78
+#: hiddifypanel/panel/user/templates/home/all-configs.html:79
+#: hiddifypanel/panel/user/templates/home/all-configs.html:80
+#: hiddifypanel/panel/user/templates/home/all-configs.html:81
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:22
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:23
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:24
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:25
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:34
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:36
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:37
@@ -2767,21 +2767,35 @@
 #: hiddifypanel/panel/user/templates/home/all-configs.html:39
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:35
 msgid "user.home.allconfigs.expect_vless"
 msgstr "Except VLess"
 
 # | msgid "Subscription Link"
 #: hiddifypanel/panel/user/templates/home/all-configs.html:47
-#: hiddifypanel/panel/user/templates/home/all-configs.html:60
+#: hiddifypanel/panel/user/templates/home/all-configs.html:74
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:43
 #: hiddifypanel/panel/user/templates/home/android.html:43
 #: hiddifypanel/panel/user/templates/home/ios.html:29
 msgid "user.home.allconfig.link-configs"
 msgstr "Subscription Link"
 
+#: hiddifypanel/panel/user/templates/home/all-configs.html:61
+#, fuzzy
+msgid "singbox: ssh"
+msgstr "singbox: ssh"
+
+#: hiddifypanel/panel/user/templates/home/all-configs.html:64
+#: hiddifypanel/panel/user/templates/home/all-configs.html:65
+#: hiddifypanel/panel/user/templates/home/all-configs.html:66
+#: hiddifypanel/panel/user/templates/home/all-configs.html:67
+#: hiddifypanel/panel/user/templates/home/all-configs.html:68
+#, fuzzy
+msgid "ssh"
+msgstr "ssh"
+
 # | msgid ""
 # | "📍 Please select one of the following applications:\n"
 # | "<br />\n"
 # | "<br />"
 #: hiddifypanel/panel/user/templates/home/android.html:2
 #: hiddifypanel/panel/user/templates/home/ios.html:3
 #: hiddifypanel/panel/user/templates/home/windows.html:46
@@ -3782,14 +3796,44 @@
 "<li>📝Python Developer</li>\n"
 "<li>📝Kotlin Developer</li>\n"
 "<li>🖥Content Providers</li>\n"
 "</ul>\n"
 "\n"
 "Please contact us at <a href=\"mailto:info@hiddify.com\">info@hiddify.com</a> if you can help us."
 
+#: hiddifypanel/templates/fake.html:1
+#, fuzzy
+msgid "config.ssh_server_redis_url.label"
+msgstr "config.ssh_server_redis_url.label"
+
+#: hiddifypanel/templates/fake.html:1
+#, fuzzy
+msgid "config.ssh_server_redis_url.description"
+msgstr "config.ssh_server_redis_url.description"
+
+#: hiddifypanel/templates/fake.html:1
+#, fuzzy
+msgid "config.ssh_server_ports.label"
+msgstr "config.ssh_server_ports.label"
+
+#: hiddifypanel/templates/fake.html:1
+#, fuzzy
+msgid "config.ssh_server_ports.description"
+msgstr "config.ssh_server_ports.description"
+
+#: hiddifypanel/templates/fake.html:1
+#, fuzzy
+msgid "config.ssh_server_enable.label"
+msgstr "config.ssh_server_enable.label"
+
+#: hiddifypanel/templates/fake.html:1
+#, fuzzy
+msgid "config.ssh_server_enable.description"
+msgstr "config.ssh_server_enable.description"
+
 # | msgid "🎛️ Core"
 #: hiddifypanel/templates/fake.html:1
 msgid "config.core_type.label"
 msgstr "🎛️ Core"
 
 # | msgid ""
 # | "☢️ XRay : Is a Complete Core\n"
@@ -3816,14 +3860,24 @@
 msgstr ""
 "✳️ Default 1.1.1.1 <br>\n"
 "🚧 Block Malware 1.1.1.2 <br>\n"
 "🔞 Block Porn 1.1.1.3\n"
 
 #: hiddifypanel/templates/fake.html:2
 #, fuzzy
+msgid "config.ssh.label"
+msgstr "config.ssh.label"
+
+#: hiddifypanel/templates/fake.html:2
+#, fuzzy
+msgid "config.ssh.description"
+msgstr "config.ssh.description"
+
+#: hiddifypanel/templates/fake.html:2
+#, fuzzy
 msgid "config.hidden.label"
 msgstr "config.hidden.label"
 
 #: hiddifypanel/templates/fake.html:2
 #, fuzzy
 msgid "config.hidden.description"
 msgstr "config.hidden.description"
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/translations/fa/LC_MESSAGES/messages.mo` & `hiddifypanel-8.0.0.dev0/hiddifypanel/translations/fa/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  HiddifyPanel\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-30 16:43+0200\n"
-"PO-Revision-Date: 2023-07-30 09:30-0500\n"
+"POT-Creation-Date: 2023-08-03 10:13+0200\n"
+"PO-Revision-Date: 2023-07-30 09:43-0500\n"
 "Last-Translator: hidden u\n"
 "Language: fa\n"
 "Language-Team: Persian\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/translations/fa/LC_MESSAGES/messages.po` & `hiddifypanel-8.0.0.dev0/hiddifypanel/translations/fa/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,96 +1,96 @@
 #
 msgid ""
 msgstr ""
 "Project-Id-Version:  HiddifyPanel\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-30 16:43+0200\n"
-"PO-Revision-Date: 2023-07-30 09:30-0500\n"
+"POT-Creation-Date: 2023-08-03 10:13+0200\n"
+"PO-Revision-Date: 2023-07-30 09:43-0500\n"
 "Last-Translator: hidden u\n"
 "Language: fa\n"
 "Language-Team: Persian\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 # | msgid "This Domain does not exist in the Panel !"
-#: hiddifypanel/models/domain.py:134 hiddifypanel/panel/user/user.py:177
+#: hiddifypanel/models/domain.py:134 hiddifypanel/panel/user/user.py:165
 msgid "This domain does not exist in the panel!"
 msgstr "این دامنه در پنل وجود ندارد!"
 
 # | msgid ""
 # | "Error In Auto CDN IP! It Can Not Be Find, Please Contact Admin"
 #: hiddifypanel/panel/clean_ip.py:103
 msgid "Error! auto cdn ip can not be find, please contact admin."
 msgstr "خطا! آی پی اتوماتیک نتوانست پیدا شود. لطفا با مدیر تماس بگیرید"
 
-#: hiddifypanel/panel/hiddify.py:76
+#: hiddifypanel/panel/hiddify.py:78
 msgid "Access Denied"
 msgstr "دسترسی غیر مجاز"
 
 # | msgid "Apply Configs"
-#: hiddifypanel/panel/hiddify.py:221
+#: hiddifypanel/panel/hiddify.py:223
 msgid "admin.config.apply_configs"
 msgstr "اعمال تنظیمات"
 
 # | msgid ""
 # | "Configs have been changed successfully. Click %(link)s to apply the
 # configs."
 # | " It may take 2 minutes to apply"
-#: hiddifypanel/panel/hiddify.py:222
+#: hiddifypanel/panel/hiddify.py:224
 msgid "config.validation-success"
 msgstr ""
 "تنظیمات با موفقیت ذخیره شدند. لطفا بر روی این لینک: %(link)s کلیک کنید تا"
 " بر روی سیستم اعمال شوند. این کار ممکن است 2 دقیقه طول بکشد"
 
 # | msgid " ✅ Configs have been changed successfully"
-#: hiddifypanel/panel/hiddify.py:224
+#: hiddifypanel/panel/hiddify.py:226
 msgid "config.validation-success-no-reset"
 msgstr " ✅ تنظیمات با موفقیت تغییر کرد"
 
 # | msgid ""
 # | "Domain can not be resolved! There is a problem in your domain. Please
 # check "
 # | "your Domain configurations."
 #: hiddifypanel/panel/admin/ChildAdmin.py:106
 #: hiddifypanel/panel/admin/DomainAdmin.py:154
 #: hiddifypanel/panel/admin/DomainAdmin.py:176
 #: hiddifypanel/panel/admin/DomainAdmin.py:179
 #: hiddifypanel/panel/admin/QuickSetup.py:126
 #: hiddifypanel/panel/commercial/ParentDomainAdmin.py:107
-#: hiddifypanel/panel/hiddify.py:343
+#: hiddifypanel/panel/hiddify.py:345
 msgid "Domain can not be resolved! there is a problem in your domain"
 msgstr "دامنه قابل دسترسی نیست! در دامنه شما مشکلی وجود دارد."
 
 # | msgid "Last Day"
-#: hiddifypanel/panel/hiddify.py:371
+#: hiddifypanel/panel/hiddify.py:373
 msgid "0 - Last day"
 msgstr "آخرین روز"
 
 # | msgid ""
 # | "Selected Domain for REALITY is not in the same ASN. To better use of the
 # "
 # | "Protocol, it is better to find a Domain in the same ASN"
-#: hiddifypanel/panel/hiddify.py:652
+#: hiddifypanel/panel/hiddify.py:654
 msgid ""
 "selected domain for REALITY is not in the same ASN. To better use of the "
 "protocol, it is better to find a domain in the same ASN."
 msgstr ""
 "دامنه انتخاب شده برای REALITY در همان ASN نیست. برای استفاده بهتر از این "
 "پروتکل، بهتر است یک دامنه در همان ASN پیدا کنید."
 
 # | msgid "User Activated"
-#: hiddifypanel/panel/usage.py:113
+#: hiddifypanel/panel/usage.py:102
 msgid "User activated!"
 msgstr "یوزر شما فعال شد"
 
 # | msgid "Package Ended"
-#: hiddifypanel/panel/usage.py:113
+#: hiddifypanel/panel/usage.py:102
 msgid "Package ended!"
 msgstr "پکیج شما به پایان رسید"
 
 # | msgid ""
 # | "⚠️ Your Domains Changed. please do not forget to copy Admin links,
 # otherwise"
 # | " you can not access to the panel anymore"
@@ -2803,19 +2803,19 @@
 #: hiddifypanel/panel/user/templates/home/all-configs.html:40
 #: hiddifypanel/panel/user/templates/home/all-configs.html:41
 #: hiddifypanel/panel/user/templates/home/all-configs.html:50
 #: hiddifypanel/panel/user/templates/home/all-configs.html:51
 #: hiddifypanel/panel/user/templates/home/all-configs.html:52
 #: hiddifypanel/panel/user/templates/home/all-configs.html:53
 #: hiddifypanel/panel/user/templates/home/all-configs.html:54
-#: hiddifypanel/panel/user/templates/home/all-configs.html:63
-#: hiddifypanel/panel/user/templates/home/all-configs.html:64
-#: hiddifypanel/panel/user/templates/home/all-configs.html:65
-#: hiddifypanel/panel/user/templates/home/all-configs.html:66
-#: hiddifypanel/panel/user/templates/home/all-configs.html:67
+#: hiddifypanel/panel/user/templates/home/all-configs.html:77
+#: hiddifypanel/panel/user/templates/home/all-configs.html:78
+#: hiddifypanel/panel/user/templates/home/all-configs.html:79
+#: hiddifypanel/panel/user/templates/home/all-configs.html:80
+#: hiddifypanel/panel/user/templates/home/all-configs.html:81
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:22
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:23
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:24
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:25
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:34
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:36
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:37
@@ -2836,21 +2836,33 @@
 #: hiddifypanel/panel/user/templates/home/all-configs.html:39
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:35
 msgid "user.home.allconfigs.expect_vless"
 msgstr "به جز VLESS"
 
 # | msgid "Subscription Link"
 #: hiddifypanel/panel/user/templates/home/all-configs.html:47
-#: hiddifypanel/panel/user/templates/home/all-configs.html:60
+#: hiddifypanel/panel/user/templates/home/all-configs.html:74
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:43
 #: hiddifypanel/panel/user/templates/home/android.html:43
 #: hiddifypanel/panel/user/templates/home/ios.html:29
 msgid "user.home.allconfig.link-configs"
 msgstr "لینک برای Subscription"
 
+#: hiddifypanel/panel/user/templates/home/all-configs.html:61
+msgid "singbox: ssh"
+msgstr ""
+
+#: hiddifypanel/panel/user/templates/home/all-configs.html:64
+#: hiddifypanel/panel/user/templates/home/all-configs.html:65
+#: hiddifypanel/panel/user/templates/home/all-configs.html:66
+#: hiddifypanel/panel/user/templates/home/all-configs.html:67
+#: hiddifypanel/panel/user/templates/home/all-configs.html:68
+msgid "ssh"
+msgstr ""
+
 # | msgid ""
 # | "📍 Please select one of the following applications:\n"
 # | "<br />\n"
 # | "<br />"
 #: hiddifypanel/panel/user/templates/home/android.html:2
 #: hiddifypanel/panel/user/templates/home/ios.html:3
 #: hiddifypanel/panel/user/templates/home/windows.html:46
@@ -3936,14 +3948,38 @@
 "<li>🖥 اگر توانایی تولید یا ارائه محتوا هستید، با ما تماس بگیرید</li>\n"
 "</ul>\n"
 "\n"
 "اگر در زمینه‌های ذکر شده و یا هر زمینه دیگری می‌توانید به ما کمک کنید، "
 "لطفاً با آدرس <a href=\"mailto:info@hiddify.com\">info@hiddify.com</a> با"
 " ما تماس بگیرید."
 
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_redis_url.label"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_redis_url.description"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_ports.label"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_ports.description"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_enable.label"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_enable.description"
+msgstr ""
+
 # | msgid "🎛️ Core"
 #: hiddifypanel/templates/fake.html:1
 msgid "config.core_type.label"
 msgstr "🎛️ هسته"
 
 # | msgid ""
 # | "☢️ XRay : Is a Complete Core\n"
@@ -3969,14 +4005,22 @@
 msgid "config.dns_server.description"
 msgstr ""
 "✳️ پیش فرض 1.1.1.1 <br>\n"
 "🚧 مسدود کردن بدافزار 1.1.1.2 <br>\n"
 "🔞 مسدود کردن پورن 1.1.1.3"
 
 #: hiddifypanel/templates/fake.html:2
+msgid "config.ssh.label"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:2
+msgid "config.ssh.description"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:2
 msgid "config.hidden.label"
 msgstr ""
 
 #: hiddifypanel/templates/fake.html:2
 msgid "config.hidden.description"
 msgstr ""
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/translations/pt/LC_MESSAGES/messages.mo` & `hiddifypanel-8.0.0.dev0/hiddifypanel/translations/pt/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  HiddifyPT\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-30 16:43+0200\n"
-"PO-Revision-Date: 2023-07-30 09:30-0500\n"
+"POT-Creation-Date: 2023-08-03 10:13+0200\n"
+"PO-Revision-Date: 2023-07-30 09:43-0500\n"
 "Last-Translator: lymanrudni\n"
 "Language: pt\n"
 "Language-Team: Portuguese\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/translations/pt/LC_MESSAGES/messages.po` & `hiddifypanel-8.0.0.dev0/hiddifypanel/translations/pt/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,107 +1,107 @@
 #
 msgid ""
 msgstr ""
 "Project-Id-Version:  HiddifyPT\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-30 16:43+0200\n"
-"PO-Revision-Date: 2023-07-30 09:30-0500\n"
+"POT-Creation-Date: 2023-08-03 10:13+0200\n"
+"PO-Revision-Date: 2023-07-30 09:43-0500\n"
 "Last-Translator: lymanrudni\n"
 "Language: pt\n"
 "Language-Team: Portuguese\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 # | msgid "This Domain does not exist in the Panel !"
-#: hiddifypanel/models/domain.py:134 hiddifypanel/panel/user/user.py:177
+#: hiddifypanel/models/domain.py:134 hiddifypanel/panel/user/user.py:165
 msgid "This domain does not exist in the panel!"
 msgstr "Este Domínio não existe no Painel!"
 
 # | msgid ""
 # | "Error In Auto CDN IP! It Can Not Be Find, Please Contact Admin"
 #: hiddifypanel/panel/clean_ip.py:103
 #, fuzzy
 msgid "Error! auto cdn ip can not be find, please contact admin."
 msgstr ""
 "Erro no Auto CDN IP! Não pode ser encontrado, entre em contato com o "
 "administrador"
 
-#: hiddifypanel/panel/hiddify.py:76
+#: hiddifypanel/panel/hiddify.py:78
 msgid "Access Denied"
 msgstr "Acesso negado"
 
 # | msgid "Apply Configs"
-#: hiddifypanel/panel/hiddify.py:221
+#: hiddifypanel/panel/hiddify.py:223
 #, fuzzy
 msgid "admin.config.apply_configs"
 msgstr "Aplicar configurações"
 
 # | msgid ""
 # | "Configs have been changed successfully. Click %(link)s to apply the
 # configs."
 # | " It may take 2 minutes to apply"
-#: hiddifypanel/panel/hiddify.py:222
+#: hiddifypanel/panel/hiddify.py:224
 #, fuzzy
 msgid "config.validation-success"
 msgstr ""
 "As configurações foram alteradas com sucesso. Clique em %(link)s para "
 "aplicar as configurações. Pode levar 2 minutos para aplicar"
 
 # | msgid " ✅ Configs have been changed successfully"
-#: hiddifypanel/panel/hiddify.py:224
+#: hiddifypanel/panel/hiddify.py:226
 #, fuzzy
 msgid "config.validation-success-no-reset"
 msgstr "✅ As configurações foram alteradas com sucesso"
 
 # | msgid ""
 # | "Domain can not be resolved! There is a problem in your domain. Please
 # check "
 # | "your Domain configurations."
 #: hiddifypanel/panel/admin/ChildAdmin.py:106
 #: hiddifypanel/panel/admin/DomainAdmin.py:154
 #: hiddifypanel/panel/admin/DomainAdmin.py:176
 #: hiddifypanel/panel/admin/DomainAdmin.py:179
 #: hiddifypanel/panel/admin/QuickSetup.py:126
 #: hiddifypanel/panel/commercial/ParentDomainAdmin.py:107
-#: hiddifypanel/panel/hiddify.py:343
+#: hiddifypanel/panel/hiddify.py:345
 #, fuzzy
 msgid "Domain can not be resolved! there is a problem in your domain"
 msgstr ""
 "O domínio não pode ser resolvido! Há um problema em seu domínio. "
 "Verifique as configurações do seu Domínio."
 
 # | msgid "Last Day"
-#: hiddifypanel/panel/hiddify.py:371
+#: hiddifypanel/panel/hiddify.py:373
 #, fuzzy
 msgid "0 - Last day"
 msgstr "Último dia"
 
 # | msgid ""
 # | "Selected Domain for REALITY is not in the same ASN. To better use of the
 # "
 # | "Protocol, it is better to find a Domain in the same ASN"
-#: hiddifypanel/panel/hiddify.py:652
+#: hiddifypanel/panel/hiddify.py:654
 msgid ""
 "selected domain for REALITY is not in the same ASN. To better use of the "
 "protocol, it is better to find a domain in the same ASN."
 msgstr ""
 "O domínio selecionado para REALITY não está no mesmo ASN.\n"
 "Para melhor aproveitamento do Protocolo, é melhor encontrar um Domínio "
 "com o mesmo ASN"
 
 # | msgid "User Activated"
-#: hiddifypanel/panel/usage.py:113
+#: hiddifypanel/panel/usage.py:102
 msgid "User activated!"
 msgstr "Usuário ativado"
 
 # | msgid "Package Ended"
-#: hiddifypanel/panel/usage.py:113
+#: hiddifypanel/panel/usage.py:102
 msgid "Package ended!"
 msgstr "Package encerrado"
 
 # | msgid ""
 # | "⚠️ Your Domains Changed. please do not forget to copy Admin links,
 # otherwise"
 # | " you can not access to the panel anymore"
@@ -3094,19 +3094,19 @@
 #: hiddifypanel/panel/user/templates/home/all-configs.html:40
 #: hiddifypanel/panel/user/templates/home/all-configs.html:41
 #: hiddifypanel/panel/user/templates/home/all-configs.html:50
 #: hiddifypanel/panel/user/templates/home/all-configs.html:51
 #: hiddifypanel/panel/user/templates/home/all-configs.html:52
 #: hiddifypanel/panel/user/templates/home/all-configs.html:53
 #: hiddifypanel/panel/user/templates/home/all-configs.html:54
-#: hiddifypanel/panel/user/templates/home/all-configs.html:63
-#: hiddifypanel/panel/user/templates/home/all-configs.html:64
-#: hiddifypanel/panel/user/templates/home/all-configs.html:65
-#: hiddifypanel/panel/user/templates/home/all-configs.html:66
-#: hiddifypanel/panel/user/templates/home/all-configs.html:67
+#: hiddifypanel/panel/user/templates/home/all-configs.html:77
+#: hiddifypanel/panel/user/templates/home/all-configs.html:78
+#: hiddifypanel/panel/user/templates/home/all-configs.html:79
+#: hiddifypanel/panel/user/templates/home/all-configs.html:80
+#: hiddifypanel/panel/user/templates/home/all-configs.html:81
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:22
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:23
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:24
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:25
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:34
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:36
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:37
@@ -3130,22 +3130,34 @@
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:35
 #, fuzzy
 msgid "user.home.allconfigs.expect_vless"
 msgstr "Exceto VMenos"
 
 # | msgid "Subscription Link"
 #: hiddifypanel/panel/user/templates/home/all-configs.html:47
-#: hiddifypanel/panel/user/templates/home/all-configs.html:60
+#: hiddifypanel/panel/user/templates/home/all-configs.html:74
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:43
 #: hiddifypanel/panel/user/templates/home/android.html:43
 #: hiddifypanel/panel/user/templates/home/ios.html:29
 #, fuzzy
 msgid "user.home.allconfig.link-configs"
 msgstr "Link de assinatura"
 
+#: hiddifypanel/panel/user/templates/home/all-configs.html:61
+msgid "singbox: ssh"
+msgstr ""
+
+#: hiddifypanel/panel/user/templates/home/all-configs.html:64
+#: hiddifypanel/panel/user/templates/home/all-configs.html:65
+#: hiddifypanel/panel/user/templates/home/all-configs.html:66
+#: hiddifypanel/panel/user/templates/home/all-configs.html:67
+#: hiddifypanel/panel/user/templates/home/all-configs.html:68
+msgid "ssh"
+msgstr ""
+
 # | msgid ""
 # | "📍 Please select one of the following applications:\n"
 # | "<br />\n"
 # | "<br />"
 #: hiddifypanel/panel/user/templates/home/android.html:2
 #: hiddifypanel/panel/user/templates/home/ios.html:3
 #: hiddifypanel/panel/user/templates/home/windows.html:46
@@ -4298,14 +4310,38 @@
 "<li>🖥Provedores de conteúdo</li>\n"
 "</ul>\n"
 "\n"
 "Entre em contato conosco em <a "
 "href=\"mailto:hiddify@gmail.com\">hiddify@gmail.com</a> se puder nos "
 "ajudar."
 
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_redis_url.label"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_redis_url.description"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_ports.label"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_ports.description"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_enable.label"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_enable.description"
+msgstr ""
+
 # | msgid "🎛️ Core"
 #: hiddifypanel/templates/fake.html:1
 #, fuzzy
 msgid "config.core_type.label"
 msgstr "🎛️ Núcleo"
 
 # | msgid ""
@@ -4333,14 +4369,22 @@
 msgid "config.dns_server.description"
 msgstr ""
 "✳️ Padrão 1.1.1.1 <br>\n"
 "🚧 Bloquear Malware 1.1.1.2 <br>\n"
 "🔞 Bloquear pornografia 1.1.1.3"
 
 #: hiddifypanel/templates/fake.html:2
+msgid "config.ssh.label"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:2
+msgid "config.ssh.description"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:2
 msgid "config.hidden.label"
 msgstr "config.hidden.label"
 
 #: hiddifypanel/templates/fake.html:2
 msgid "config.hidden.description"
 msgstr "config.hidden.description"
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/translations/zh/LC_MESSAGES/messages.mo` & `hiddifypanel-8.0.0.dev0/hiddifypanel/translations/zh/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  HiddifyPanel\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-30 16:43+0200\n"
-"PO-Revision-Date: 2023-07-30 09:30-0500\n"
+"POT-Creation-Date: 2023-08-03 10:13+0200\n"
+"PO-Revision-Date: 2023-07-30 09:43-0500\n"
 "Last-Translator: hidden u\n"
 "Language: zh\n"
 "Language-Team: Chinese\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/translations/zh/LC_MESSAGES/messages.po` & `hiddifypanel-8.0.0.dev0/hiddifypanel/translations/zh/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,98 +1,98 @@
 #
 msgid ""
 msgstr ""
 "Project-Id-Version:  HiddifyPanel\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-30 16:43+0200\n"
-"PO-Revision-Date: 2023-07-30 09:30-0500\n"
+"POT-Creation-Date: 2023-08-03 10:13+0200\n"
+"PO-Revision-Date: 2023-07-30 09:43-0500\n"
 "Last-Translator: hidden u\n"
 "Language: zh\n"
 "Language-Team: Chinese\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 # | msgid "This Domain does not exist in the Panel !"
-#: hiddifypanel/models/domain.py:134 hiddifypanel/panel/user/user.py:177
+#: hiddifypanel/models/domain.py:134 hiddifypanel/panel/user/user.py:165
 #, fuzzy
 msgid "This domain does not exist in the panel!"
 msgstr "该域名在面板中不存在！"
 
 # | msgid ""
 # | "Error In Auto CDN IP! It Can Not Be Find, Please Contact Admin"
 #: hiddifypanel/panel/clean_ip.py:103
 #, fuzzy
 msgid "Error! auto cdn ip can not be find, please contact admin."
 msgstr "自动 CDN IP 错误！找不到，请联系管理员。"
 
-#: hiddifypanel/panel/hiddify.py:76
+#: hiddifypanel/panel/hiddify.py:78
 msgid "Access Denied"
 msgstr ""
 
 # | msgid "Apply Configs"
-#: hiddifypanel/panel/hiddify.py:221
+#: hiddifypanel/panel/hiddify.py:223
 msgid "admin.config.apply_configs"
 msgstr "应用配置"
 
 # | msgid ""
 # | "Configs have been changed successfully. Click %(link)s to apply the
 # configs."
 # | " It may take 2 minutes to apply"
-#: hiddifypanel/panel/hiddify.py:222
+#: hiddifypanel/panel/hiddify.py:224
 msgid "config.validation-success"
 msgstr "配置已成功更改。单击 %(link)s 以应用配置。申请可能需要 2 分钟。"
 
 # | msgid " ✅ Configs have been changed successfully"
-#: hiddifypanel/panel/hiddify.py:224
+#: hiddifypanel/panel/hiddify.py:226
 #, fuzzy
 msgid "config.validation-success-no-reset"
 msgstr "配置已成功更改。"
 
 # | msgid ""
 # | "Domain can not be resolved! There is a problem in your domain. Please
 # check "
 # | "your Domain configurations."
 #: hiddifypanel/panel/admin/ChildAdmin.py:106
 #: hiddifypanel/panel/admin/DomainAdmin.py:154
 #: hiddifypanel/panel/admin/DomainAdmin.py:176
 #: hiddifypanel/panel/admin/DomainAdmin.py:179
 #: hiddifypanel/panel/admin/QuickSetup.py:126
 #: hiddifypanel/panel/commercial/ParentDomainAdmin.py:107
-#: hiddifypanel/panel/hiddify.py:343
+#: hiddifypanel/panel/hiddify.py:345
 msgid "Domain can not be resolved! there is a problem in your domain"
 msgstr "域名无法解析！你的域有问题"
 
 # | msgid "Last Day"
-#: hiddifypanel/panel/hiddify.py:371
+#: hiddifypanel/panel/hiddify.py:373
 #, fuzzy
 msgid "0 - Last day"
 msgstr "0 - 最后一天"
 
 # | msgid ""
 # | "Selected Domain for REALITY is not in the same ASN. To better use of the
 # "
 # | "Protocol, it is better to find a Domain in the same ASN"
-#: hiddifypanel/panel/hiddify.py:652
+#: hiddifypanel/panel/hiddify.py:654
 #, fuzzy
 msgid ""
 "selected domain for REALITY is not in the same ASN. To better use of the "
 "protocol, it is better to find a domain in the same ASN."
 msgstr "为 REALITY 选择的域不在同一个 ASN 中。为了更好地使用该协议，最好在同一 ASN 中找到一个域。"
 
 # | msgid "User Activated"
-#: hiddifypanel/panel/usage.py:113
+#: hiddifypanel/panel/usage.py:102
 #, fuzzy
 msgid "User activated!"
 msgstr "用户激活！"
 
 # | msgid "Package Ended"
-#: hiddifypanel/panel/usage.py:113
+#: hiddifypanel/panel/usage.py:102
 #, fuzzy
 msgid "Package ended!"
 msgstr "套餐结束！"
 
 # | msgid ""
 # | "⚠️ Your Domains Changed. please do not forget to copy Admin links,
 # otherwise"
@@ -2743,19 +2743,19 @@
 #: hiddifypanel/panel/user/templates/home/all-configs.html:40
 #: hiddifypanel/panel/user/templates/home/all-configs.html:41
 #: hiddifypanel/panel/user/templates/home/all-configs.html:50
 #: hiddifypanel/panel/user/templates/home/all-configs.html:51
 #: hiddifypanel/panel/user/templates/home/all-configs.html:52
 #: hiddifypanel/panel/user/templates/home/all-configs.html:53
 #: hiddifypanel/panel/user/templates/home/all-configs.html:54
-#: hiddifypanel/panel/user/templates/home/all-configs.html:63
-#: hiddifypanel/panel/user/templates/home/all-configs.html:64
-#: hiddifypanel/panel/user/templates/home/all-configs.html:65
-#: hiddifypanel/panel/user/templates/home/all-configs.html:66
-#: hiddifypanel/panel/user/templates/home/all-configs.html:67
+#: hiddifypanel/panel/user/templates/home/all-configs.html:77
+#: hiddifypanel/panel/user/templates/home/all-configs.html:78
+#: hiddifypanel/panel/user/templates/home/all-configs.html:79
+#: hiddifypanel/panel/user/templates/home/all-configs.html:80
+#: hiddifypanel/panel/user/templates/home/all-configs.html:81
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:22
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:23
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:24
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:25
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:34
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:36
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:37
@@ -2776,21 +2776,33 @@
 #: hiddifypanel/panel/user/templates/home/all-configs.html:39
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:35
 msgid "user.home.allconfigs.expect_vless"
 msgstr "除了 vless"
 
 # | msgid "Subscription Link"
 #: hiddifypanel/panel/user/templates/home/all-configs.html:47
-#: hiddifypanel/panel/user/templates/home/all-configs.html:60
+#: hiddifypanel/panel/user/templates/home/all-configs.html:74
 #: hiddifypanel/panel/user/templates/home/all-configs_old.html:43
 #: hiddifypanel/panel/user/templates/home/android.html:43
 #: hiddifypanel/panel/user/templates/home/ios.html:29
 msgid "user.home.allconfig.link-configs"
 msgstr "订阅链接"
 
+#: hiddifypanel/panel/user/templates/home/all-configs.html:61
+msgid "singbox: ssh"
+msgstr ""
+
+#: hiddifypanel/panel/user/templates/home/all-configs.html:64
+#: hiddifypanel/panel/user/templates/home/all-configs.html:65
+#: hiddifypanel/panel/user/templates/home/all-configs.html:66
+#: hiddifypanel/panel/user/templates/home/all-configs.html:67
+#: hiddifypanel/panel/user/templates/home/all-configs.html:68
+msgid "ssh"
+msgstr ""
+
 # | msgid ""
 # | "📍 Please select one of the following applications:\n"
 # | "<br />\n"
 # | "<br />"
 #: hiddifypanel/panel/user/templates/home/android.html:2
 #: hiddifypanel/panel/user/templates/home/ios.html:3
 #: hiddifypanel/panel/user/templates/home/windows.html:46
@@ -3796,14 +3808,38 @@
 "<li>Python 开发人员</li>\n"
 "<li>Kotlin 开发人员</li>\n"
 "<li>内容提供商</li>\n"
 "\n"
 "如果您能帮助我们，请通过 <a href=\"mailto:hiddify@gmail.com\">hiddify@gmail.com</a> "
 "联系我们。"
 
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_redis_url.label"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_redis_url.description"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_ports.label"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_ports.description"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_enable.label"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:1
+msgid "config.ssh_server_enable.description"
+msgstr ""
+
 # | msgid "🎛️ Core"
 #: hiddifypanel/templates/fake.html:1
 msgid "config.core_type.label"
 msgstr "🎛️ Core"
 
 # | msgid ""
 # | "☢️ XRay : Is a Complete Core\n"
@@ -3832,14 +3868,22 @@
 msgid "config.dns_server.description"
 msgstr ""
 "默认 1.1.1.1 <br>\n"
 "阻止恶意软件 1.1.1.2 <br>\n"
 "阻止色情 1.1.1.3"
 
 #: hiddifypanel/templates/fake.html:2
+msgid "config.ssh.label"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:2
+msgid "config.ssh.description"
+msgstr ""
+
+#: hiddifypanel/templates/fake.html:2
 msgid "config.hidden.label"
 msgstr ""
 
 #: hiddifypanel/templates/fake.html:2
 msgid "config.hidden.description"
 msgstr ""
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel/xray_api.py` & `hiddifypanel-8.0.0.dev0/hiddifypanel/drivers/xray_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,113 @@
 import xtlsapi
 from hiddifypanel.models import *
+from .abstract_driver import DriverABS
 
 
-def get_xray_client():
-    if hconfig(ConfigEnum.is_parent):
-        return
-    return xtlsapi.XrayClient('127.0.0.1', 10085)
-
-
-def get_enabled_users():
-    if hconfig(ConfigEnum.is_parent):
-        return
-    xray_client = get_xray_client()
-    users = User.query.all()
-    t = "xtls"
-    protocol = "vless"
-    enabled = {}
-    for u in users:
-        uuid = u.uuid
-        try:
-            xray_client.add_client(t, f'{uuid}', f'{uuid}@hiddify.com', protocol=protocol, flow='xtls-rprx-vision', alter_id=0, cipher='chacha20_poly1305')
-            xray_client.remove_client(t, f'{uuid}@hiddify.com')
-            enabled[uuid] = 0
-        except xtlsapi.exceptions.EmailAlreadyExists as e:
-            enabled[uuid] = 1
-        except Exception as e:
-            print(f"error {e}")
-            enabled[uuid] = e
-    return enabled
-
-
-def get_inbound_tags():
-    if hconfig(ConfigEnum.is_parent):
-        return
-    try:
-        xray_client = get_xray_client()
-        inbounds = [inb.name.split(">>>")[1] for inb in xray_client.stats_query('inbound')]
-        print(f"Success in get inbound tags {inbounds}")
-    except Exception as e:
-        print(f"error in get inbound tags {e}")
-        inbounds = []
-    return list(set(inbounds))
-
-
-def add_client(uuid):
-    if hconfig(ConfigEnum.is_parent):
-        return
-    xray_client = get_xray_client()
-    tags = get_inbound_tags()
-    proto_map = {
-        'vless': 'vless',
-        'realityin': 'vless',
-        'xtls': 'vless',
-                'quic': 'vless',
-                'trojan': 'trojan',
-                'vmess': 'vmess',
-                'ss': 'shadowsocks',
-                'v2ray': 'shadowsocks',
-                'kcp': 'vless',
-                'dispatcher': 'trojan',
-    }
-
-    def proto(t):
-        res = '', ''
-        for p, protocol in proto_map.items():
-            if p in t:
-                res = p, protocol
-                break
-        return res
-    for t in tags:
-        try:
-            p, protocol = proto(t)
-            if not p:
-                continue
-            if protocol == "vless" and p != "xtls" and p != "realityin":
-                xray_client.add_client(t, f'{uuid}', f'{uuid}@hiddify.com', protocol=protocol, flow='\0',)
-            else:
+class XrayApi(DriverABS):
+    def get_xray_client(self):
+        if hconfig(ConfigEnum.is_parent):
+            return
+        return xtlsapi.XrayClient('127.0.0.1', 10085)
+
+    def get_enabled_users(self):
+        if hconfig(ConfigEnum.is_parent):
+            return
+        xray_client = self.get_xray_client()
+        users = User.query.all()
+        t = "xtls"
+        protocol = "vless"
+        enabled = {}
+        for u in users:
+            uuid = u.uuid
+            try:
                 xray_client.add_client(t, f'{uuid}', f'{uuid}@hiddify.com', protocol=protocol, flow='xtls-rprx-vision', alter_id=0, cipher='chacha20_poly1305')
-            print(f"Success add  {uuid} {t}")
-        except Exception as e:
-            print(f"error in add  {uuid} {t} {e}")
-            pass
-
-
-def remove_client(uuid):
-    if hconfig(ConfigEnum.is_parent):
-        return
-    xray_client = get_xray_client()
-    tags = get_inbound_tags()
-
-    for t in tags:
+                xray_client.remove_client(t, f'{uuid}@hiddify.com')
+                enabled[uuid] = 0
+            except xtlsapi.exceptions.EmailAlreadyExists as e:
+                enabled[uuid] = 1
+            except Exception as e:
+                print(f"error {e}")
+                enabled[uuid] = e
+        return enabled
+
+    def get_inbound_tags(self):
+        if hconfig(ConfigEnum.is_parent):
+            return
         try:
-            xray_client.remove_client(t, f'{uuid}@hiddify.com')
-            print(f"Success remove  {uuid} {t}")
+            xray_client = self.get_xray_client()
+            inbounds = [inb.name.split(">>>")[1] for inb in xray_client.stats_query('inbound')]
+            print(f"Success in get inbound tags {inbounds}")
         except Exception as e:
-            print(f"error in remove  {uuid} {t} {e}")
-            pass
-
-
-def get_usage(uuid, reset=False):
-    if hconfig(ConfigEnum.is_parent):
-        return
-    xray_client = get_xray_client()
-    d = xray_client.get_client_download_traffic(f'{uuid}@hiddify.com', reset=reset)
-    u = xray_client.get_client_upload_traffic(f'{uuid}@hiddify.com', reset=reset)
-    print(f"Success {uuid} d={d} u={u}")
-    res = None
-    if d is None:
-        res = u
-    elif u is None:
-        res = d
-    else:
-        res = d + u
-    return res
+            print(f"error in get inbound tags {e}")
+            inbounds = []
+        return list(set(inbounds))
+
+    def add_client(self, user):
+        if hconfig(ConfigEnum.is_parent):
+            return
+        uuid = user.uuid
+        xray_client = self.get_xray_client()
+        tags = self.get_inbound_tags()
+        proto_map = {
+            'vless': 'vless',
+            'realityin': 'vless',
+            'xtls': 'vless',
+                    'quic': 'vless',
+                    'trojan': 'trojan',
+                    'vmess': 'vmess',
+                    'ss': 'shadowsocks',
+                    'v2ray': 'shadowsocks',
+                    'kcp': 'vless',
+                    'dispatcher': 'trojan',
+        }
+
+        def proto(t):
+            res = '', ''
+            for p, protocol in proto_map.items():
+                if p in t:
+                    res = p, protocol
+                    break
+            return res
+        for t in tags:
+            try:
+                p, protocol = proto(t)
+                if not p:
+                    continue
+                if protocol == "vless" and p != "xtls" and p != "realityin":
+                    xray_client.add_client(t, f'{uuid}', f'{uuid}@hiddify.com', protocol=protocol, flow='\0',)
+                else:
+                    xray_client.add_client(t, f'{uuid}', f'{uuid}@hiddify.com', protocol=protocol, flow='xtls-rprx-vision', alter_id=0, cipher='chacha20_poly1305')
+                print(f"Success add  {uuid} {t}")
+            except Exception as e:
+                print(f"error in add  {uuid} {t} {e}")
+                pass
+
+    def remove_client(self, uuid):
+        if hconfig(ConfigEnum.is_parent):
+            return
+        xray_client = self.get_xray_client()
+        tags = self.get_inbound_tags()
+
+        for t in tags:
+            try:
+                xray_client.remove_client(t, f'{uuid}@hiddify.com')
+                print(f"Success remove  {uuid} {t}")
+            except Exception as e:
+                print(f"error in remove  {uuid} {t} {e}")
+                pass
+
+    def get_usage(self, uuid, reset=False):
+        if hconfig(ConfigEnum.is_parent):
+            return
+        xray_client = self.get_xray_client()
+        d = xray_client.get_client_download_traffic(f'{uuid}@hiddify.com', reset=reset)
+        u = xray_client.get_client_upload_traffic(f'{uuid}@hiddify.com', reset=reset)
+        print(f"Success {uuid} d={d} u={u}")
+        res = None
+        if d is None:
+            res = u
+        elif u is None:
+            res = d
+        else:
+            res = d + u
+        return res
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel.egg-info/PKG-INFO` & `hiddifypanel-8.0.0.dev0/hiddifypanel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiddifypanel
-Version: 7.1.9
+Version: 8.0.0.dev0
 Summary: hiddifypanel multi proxy panel
 Home-page: https://github.com/hiddify/hiddify-config/
 Author: hiddify
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel.egg-info/SOURCES.txt` & `hiddifypanel-8.0.0.dev0/hiddifypanel.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,26 @@
 setup.py
 hiddifypanel/Events.py
 hiddifypanel/VERSION
 hiddifypanel/VERSION.py
 hiddifypanel/__init__.py
 hiddifypanel/__main__.py
 hiddifypanel/base.py
-hiddifypanel/singbox_api.py
-hiddifypanel/xray_api.py
+hiddifypanel/cache.py
 hiddifypanel.egg-info/PKG-INFO
 hiddifypanel.egg-info/SOURCES.txt
 hiddifypanel.egg-info/dependency_links.txt
 hiddifypanel.egg-info/entry_points.txt
 hiddifypanel.egg-info/requires.txt
 hiddifypanel.egg-info/top_level.txt
+hiddifypanel/drivers/abstract_driver.py
+hiddifypanel/drivers/singbox_api.py
+hiddifypanel/drivers/ssh_liberty_bridge_api.py
+hiddifypanel/drivers/user_driver.py
+hiddifypanel/drivers/xray_api.py
 hiddifypanel/models/__init__.py
 hiddifypanel/models/admin.py
 hiddifypanel/models/child.py
 hiddifypanel/models/config.py
 hiddifypanel/models/config_enum.py
 hiddifypanel/models/domain.py
 hiddifypanel/models/parent_domain.py
@@ -93,14 +97,15 @@
 hiddifypanel/panel/user/user.py
 hiddifypanel/panel/user/templates/all_configs copy.txt
 hiddifypanel/panel/user/templates/all_configs.txt
 hiddifypanel/panel/user/templates/clash_config copy.yml
 hiddifypanel/panel/user/templates/clash_config.yml
 hiddifypanel/panel/user/templates/clash_proxies copy.yml
 hiddifypanel/panel/user/templates/clash_proxies.yml
+hiddifypanel/panel/user/templates/singbox_config.json
 hiddifypanel/panel/user/templates/home/all-configs.html
 hiddifypanel/panel/user/templates/home/all-configs_old.html
 hiddifypanel/panel/user/templates/home/android.html
 hiddifypanel/panel/user/templates/home/base2.html
 hiddifypanel/panel/user/templates/home/clash-links copy.html
 hiddifypanel/panel/user/templates/home/clash-links.html
 hiddifypanel/panel/user/templates/home/doh.html
```

### Comparing `hiddifypanel-7.1.9/hiddifypanel.egg-info/requires.txt` & `hiddifypanel-8.0.0.dev0/hiddifypanel.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 lastversion
 psutil
 h2
 ping3
 ansi2html
 netifaces
 markupsafe
+redis
+python-redis-cache
 
 [test]
 flask-debugtoolbar
 flask-shell-ipython
 ipdb
 pytest-flask
 python-dotenv
```

### Comparing `hiddifypanel-7.1.9/setup.py` & `hiddifypanel-8.0.0.dev0/setup.py`

 * *Files identical despite different names*

