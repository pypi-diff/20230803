# Comparing `tmp/nonebot_plugin_bind-0.1.4.tar.gz` & `tmp/nonebot_plugin_bind-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bind-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_bind-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_bind-0.1.4.tar` & `nonebot_plugin_bind-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     5928 2023-08-01 10:13:17.266547 nonebot_plugin_bind-0.1.4/nonebot_plugin_bind/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 09:12:10.853222 nonebot_plugin_bind-0.1.4/nonebot_plugin_bind/_types.py
--rw-r--r--   0        0        0     5414 2023-08-01 09:26:34.170289 nonebot_plugin_bind-0.1.4/nonebot_plugin_bind/user_sql.py
--rw-r--r--   0        0        0     1078 2023-08-01 07:01:38.000000 nonebot_plugin_bind-0.1.4/nonebot_plugin_bind/utils.py
--rw-r--r--   0        0        0      522 2023-08-01 09:34:12.103709 nonebot_plugin_bind-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3018 2023-08-01 10:20:30.698992 nonebot_plugin_bind-0.1.4/README.md
--rw-r--r--   0        0        0     3660 1970-01-01 00:00:00.000000 nonebot_plugin_bind-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    13463 2023-08-03 14:47:47.991862 nonebot_plugin_bind-0.1.5/nonebot_plugin_bind/__init__.py
+-rw-r--r--   0        0        0      425 2023-08-03 14:16:23.980829 nonebot_plugin_bind-0.1.5/nonebot_plugin_bind/_types.py
+-rw-r--r--   0        0        0      293 2023-08-03 15:29:55.129796 nonebot_plugin_bind-0.1.5/nonebot_plugin_bind/config.py
+-rw-r--r--   0        0        0     4923 2023-08-03 14:34:27.375520 nonebot_plugin_bind-0.1.5/nonebot_plugin_bind/group_sql.py
+-rw-r--r--   0        0        0     2348 2023-08-02 14:26:30.241522 nonebot_plugin_bind-0.1.5/nonebot_plugin_bind/migrations/57ff5da24acb_init_db.py
+-rw-r--r--   0        0        0     4646 2023-08-03 03:49:03.293793 nonebot_plugin_bind-0.1.5/nonebot_plugin_bind/user_sql.py
+-rw-r--r--   0        0        0     5451 2023-08-03 15:35:30.890545 nonebot_plugin_bind-0.1.5/nonebot_plugin_bind/utils.py
+-rw-r--r--   0        0        0      696 2023-08-03 14:36:02.184893 nonebot_plugin_bind-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5072 2023-08-03 15:52:05.494985 nonebot_plugin_bind-0.1.5/README.md
+-rw-r--r--   0        0        0     5707 1970-01-01 00:00:00.000000 nonebot_plugin_bind-0.1.5/PKG-INFO
```

