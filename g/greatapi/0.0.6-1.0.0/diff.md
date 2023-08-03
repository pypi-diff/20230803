# Comparing `tmp/greatapi-0.0.6.tar.gz` & `tmp/greatapi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greatapi-0.0.6.tar", last modified: Wed Aug  2 17:00:08 2023, max compression
+gzip compressed data, was "greatapi-1.0.0.tar", last modified: Thu Aug  3 01:42:05 2023, max compression
```

## Comparing `greatapi-0.0.6.tar` & `greatapi-1.0.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.978250 greatapi-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 16:59:59.000000 greatapi-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-08-02 17:00:08.978250 greatapi-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-08-02 16:59:59.000000 greatapi-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.970250 greatapi-0.0.6/greatapi/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.970250 greatapi-0.0.6/greatapi/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.970250 greatapi-0.0.6/greatapi/admin/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/static/greatapi_readme.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/static/main.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/static/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.970250 greatapi-0.0.6/greatapi/admin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.970250 greatapi-0.0.6/greatapi/admin/templates/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/authentication/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/admin/templates/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/account.html
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/add_item.html
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/delete_user.html
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/group.html
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/history.html
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/items.html
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/visualization.html
--rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/navbar.html
--rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/sidebar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/commands/createsuperuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/commands/runserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/commands/startapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/commands/startproject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/conf/app_template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/app_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/app_template/__init__.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/app_template/models.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/app_template/repository.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/app_template/router.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/app_template/schemas.py-tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/conf/project_template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/project_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/project_template/main.py-tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/conf/project_template/project_name/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/project_template/project_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/project_template/project_name/__init__.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/project_template/project_name/settings.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/core/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/core/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/auth/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/auth/jwt_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/auth/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/auth/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/core/history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/history/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/history/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/history/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/core/test_auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/test_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/test_auth/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/core/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/users/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/users/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/users/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.978250 greatapi-0.0.6/greatapi/db/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/db/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/db/admin/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/db/admin/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/db/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.978250 greatapi-0.0.6/greatapi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/utils/cbv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/utils/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/utils/inferring_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/utils/management.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/utils/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.970250 greatapi-0.0.6/greatapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-08-02 17:00:08.000000 greatapi-0.0.6/greatapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-02 17:00:08.000000 greatapi-0.0.6/greatapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:00:08.000000 greatapi-0.0.6/greatapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 17:00:08.000000 greatapi-0.0.6/greatapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-02 17:00:08.000000 greatapi-0.0.6/greatapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 17:00:08.000000 greatapi-0.0.6/greatapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-02 17:00:08.978250 greatapi-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 16:59:59.000000 greatapi-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.320770 greatapi-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 01:41:51.000000 greatapi-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-08-03 01:42:05.320770 greatapi-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-08-03 01:41:51.000000 greatapi-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.308770 greatapi-1.0.0/greatapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.308770 greatapi-1.0.0/greatapi/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.312770 greatapi-1.0.0/greatapi/admin/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/static/greatapi_readme.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/static/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/static/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.312770 greatapi-1.0.0/greatapi/admin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.312770 greatapi-1.0.0/greatapi/admin/templates/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/authentication/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.312770 greatapi-1.0.0/greatapi/admin/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/dashboard/account.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/dashboard/add_item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/dashboard/delete_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/dashboard/group.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/dashboard/history.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/dashboard/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/dashboard/items.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/dashboard/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/dashboard/visualization.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/admin/templates/sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.312770 greatapi-1.0.0/greatapi/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/commands/createsuperuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/commands/runserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/commands/startapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/commands/startproject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.312770 greatapi-1.0.0/greatapi/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.316770 greatapi-1.0.0/greatapi/conf/app_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/conf/app_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/conf/app_template/__init__.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/conf/app_template/models.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/conf/app_template/repository.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/conf/app_template/router.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/conf/app_template/schemas.py-tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.316770 greatapi-1.0.0/greatapi/conf/project_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/conf/project_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/conf/project_template/main.py-tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.316770 greatapi-1.0.0/greatapi/conf/project_template/project_name/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/conf/project_template/project_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/conf/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/conf/project_template/project_name/settings.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.316770 greatapi-1.0.0/greatapi/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.316770 greatapi-1.0.0/greatapi/core/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/auth/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/auth/jwt_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/auth/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/auth/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.316770 greatapi-1.0.0/greatapi/core/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/history/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/history/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/history/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.316770 greatapi-1.0.0/greatapi/core/test_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/test_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/test_auth/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.320770 greatapi-1.0.0/greatapi/core/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/users/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/users/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/core/users/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.320770 greatapi-1.0.0/greatapi/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.320770 greatapi-1.0.0/greatapi/db/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/db/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/db/admin/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/db/admin/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/db/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.320770 greatapi-1.0.0/greatapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/utils/cbv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/utils/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/utils/inferring_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/utils/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-03 01:41:51.000000 greatapi-1.0.0/greatapi/utils/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:05.308770 greatapi-1.0.0/greatapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-08-03 01:42:05.000000 greatapi-1.0.0/greatapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-03 01:42:05.000000 greatapi-1.0.0/greatapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:42:05.000000 greatapi-1.0.0/greatapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-03 01:42:05.000000 greatapi-1.0.0/greatapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-03 01:42:05.000000 greatapi-1.0.0/greatapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 01:42:05.000000 greatapi-1.0.0/greatapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-03 01:42:05.324770 greatapi-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-03 01:41:51.000000 greatapi-1.0.0/setup.py
```

### Comparing `greatapi-0.0.6/LICENSE` & `greatapi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/PKG-INFO` & `greatapi-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greatapi
-Version: 0.0.6
+Version: 1.0.0
 Summary: GreatAPI framework, Full stack FastAPI framework.
 Home-page: https://github.com/sahajrajmalla/greatapi
 Author: Sahaj Raj Malla
 Author-email: mallasahajraj@gmail.com
 License: MIT
 Description: # GreatAPI - Full-stack FastAPI Framework
         
@@ -114,15 +114,15 @@
         After running the server, let's create a superuser to manage the administration of your project. Execute the following command:
         
         ```bash
         greatapi createsuperuser
         
         ```
         
-        Follow the prompts to create the superuser account.
+        Follow the prompts to create the superuser account and again run the server.
         
         
         
         The server will start, and you can access your application at http://localhost:8000/. Additionally, GreatAPI provides a beautifully designed built-in Admin Panel accessible at http://localhost:8000/admin.
         
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `greatapi-0.0.6/README.md` & `greatapi-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,12 +106,12 @@
 After running the server, let's create a superuser to manage the administration of your project. Execute the following command:
 
 ```bash
 greatapi createsuperuser
 
 ```
 
-Follow the prompts to create the superuser account.
+Follow the prompts to create the superuser account and again run the server.
 
 
 
 The server will start, and you can access your application at http://localhost:8000/. Additionally, GreatAPI provides a beautifully designed built-in Admin Panel accessible at http://localhost:8000/admin.
```

### Comparing `greatapi-0.0.6/greatapi/admin/sites.py` & `greatapi-1.0.0/greatapi/admin/sites.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/static/favicon.ico` & `greatapi-1.0.0/greatapi/admin/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/static/greatapi_readme.svg` & `greatapi-1.0.0/greatapi/admin/static/greatapi_readme.svg`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/static/logo.svg` & `greatapi-1.0.0/greatapi/admin/static/logo.svg`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/static/main.js` & `greatapi-1.0.0/greatapi/admin/static/main.js`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/templates/authentication/login.html` & `greatapi-1.0.0/greatapi/admin/templates/authentication/login.html`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/templates/base.html` & `greatapi-1.0.0/greatapi/admin/templates/base.html`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/templates/dashboard/account.html` & `greatapi-1.0.0/greatapi/admin/templates/dashboard/account.html`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/templates/dashboard/add_item.html` & `greatapi-1.0.0/greatapi/admin/templates/dashboard/add_item.html`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/templates/dashboard/delete_user.html` & `greatapi-1.0.0/greatapi/admin/templates/dashboard/delete_user.html`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/templates/dashboard/group.html` & `greatapi-1.0.0/greatapi/admin/templates/dashboard/group.html`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/templates/dashboard/history.html` & `greatapi-1.0.0/greatapi/admin/templates/dashboard/history.html`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/templates/dashboard/index.html` & `greatapi-1.0.0/greatapi/admin/templates/dashboard/index.html`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/templates/dashboard/items.html` & `greatapi-1.0.0/greatapi/admin/templates/dashboard/items.html`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/templates/dashboard/settings.html` & `greatapi-1.0.0/greatapi/admin/templates/dashboard/settings.html`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/templates/dashboard/visualization.html` & `greatapi-1.0.0/greatapi/admin/templates/dashboard/visualization.html`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/templates/navbar.html` & `greatapi-1.0.0/greatapi/admin/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/admin/templates/sidebar.html` & `greatapi-1.0.0/greatapi/admin/templates/sidebar.html`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/commands/__init__.py` & `greatapi-1.0.0/greatapi/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/commands/createsuperuser.py` & `greatapi-1.0.0/greatapi/commands/createsuperuser.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/conf/project_template/main.py-tpl` & `greatapi-1.0.0/greatapi/conf/project_template/main.py-tpl`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/core/auth/jwt_token.py` & `greatapi-1.0.0/greatapi/core/auth/jwt_token.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/core/auth/sites.py` & `greatapi-1.0.0/greatapi/core/auth/sites.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/core/history/repository.py` & `greatapi-1.0.0/greatapi/core/history/repository.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/core/history/schemas.py` & `greatapi-1.0.0/greatapi/core/history/schemas.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/core/history/sites.py` & `greatapi-1.0.0/greatapi/core/history/sites.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/core/test_auth/sites.py` & `greatapi-1.0.0/greatapi/core/test_auth/sites.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/core/users/query.py` & `greatapi-1.0.0/greatapi/core/users/query.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/core/users/sites.py` & `greatapi-1.0.0/greatapi/core/users/sites.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/db/admin/default.py` & `greatapi-1.0.0/greatapi/db/admin/default.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/db/admin/user.py` & `greatapi-1.0.0/greatapi/db/admin/user.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/db/database.py` & `greatapi-1.0.0/greatapi/db/database.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/utils/cbv.py` & `greatapi-1.0.0/greatapi/utils/cbv.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/utils/component.py` & `greatapi-1.0.0/greatapi/utils/component.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/utils/inferring_router.py` & `greatapi-1.0.0/greatapi/utils/inferring_router.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/utils/management.py` & `greatapi-1.0.0/greatapi/utils/management.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi/utils/urls.py` & `greatapi-1.0.0/greatapi/utils/urls.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/greatapi.egg-info/PKG-INFO` & `greatapi-1.0.0/greatapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greatapi
-Version: 0.0.6
+Version: 1.0.0
 Summary: GreatAPI framework, Full stack FastAPI framework.
 Home-page: https://github.com/sahajrajmalla/greatapi
 Author: Sahaj Raj Malla
 Author-email: mallasahajraj@gmail.com
 License: MIT
 Description: # GreatAPI - Full-stack FastAPI Framework
         
@@ -114,15 +114,15 @@
         After running the server, let's create a superuser to manage the administration of your project. Execute the following command:
         
         ```bash
         greatapi createsuperuser
         
         ```
         
-        Follow the prompts to create the superuser account.
+        Follow the prompts to create the superuser account and again run the server.
         
         
         
         The server will start, and you can access your application at http://localhost:8000/. Additionally, GreatAPI provides a beautifully designed built-in Admin Panel accessible at http://localhost:8000/admin.
         
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `greatapi-0.0.6/greatapi.egg-info/SOURCES.txt` & `greatapi-1.0.0/greatapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.6/setup.cfg` & `greatapi-1.0.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = greatapi
-version = 0.0.6
+version = 1.0.0
 description = GreatAPI framework, Full stack FastAPI framework.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sahajrajmalla/greatapi
 author = Sahaj Raj Malla
 author_email = mallasahajraj@gmail.com
 license = MIT
```

