# Comparing `tmp/rucio-webui-32.0.0rc1.tar.gz` & `tmp/rucio-webui-32.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-webui-32.0.0rc1.tar", last modified: Wed Jul 26 15:14:54 2023, max compression
+gzip compressed data, was "rucio-webui-32.0.0rc2.tar", last modified: Thu Aug  3 15:23:09 2023, max compression
```

## Comparing `rucio-webui-32.0.0rc1.tar` & `rucio-webui-32.0.0rc2.tar`

### file list

```diff
@@ -1,267 +1,267 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.462484 rucio-webui-32.0.0rc1/
--rwxr-xr-x   0 root         (0) root         (0)     4383 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      484 2023-07-26 15:14:48.000000 rucio-webui-32.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      841 2023-07-26 15:14:54.462484 rucio-webui-32.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1982 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.381481 rucio-webui-32.0.0rc1/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.385481 rucio-webui-32.0.0rc1/lib/rucio/
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      714 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/alembicrevision.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-07-26 15:02:05.000000 rucio-webui-32.0.0rc1/lib/rucio/vcsversion.py
--rw-r--r--   0 root         (0) root         (0)     1573 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.386481 rucio-webui-32.0.0rc1/lib/rucio/web/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.386481 rucio-webui-32.0.0rc1/lib/rucio/web/ui/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.387481 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6202 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/bp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.388481 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/common/
--rwxr-xr-x   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.389481 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/common/saml/
--rw-r--r--   0 root         (0) root         (0)      990 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/common/saml/advanced_settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.389481 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/common/saml/certs/
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/common/saml/certs/README
--rw-r--r--   0 root         (0) root         (0)      656 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/common/saml/settings.json
--rw-r--r--   0 root         (0) root         (0)    27924 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/common/utils.py
--rw-r--r--   0 root         (0) root         (0)      917 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.403482 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/
--rw-r--r--   0 root         (0) root         (0)     3705 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/account.html
--rw-r--r--   0 root         (0) root         (0)     1292 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/account_rse_usage.html
--rw-r--r--   0 root         (0) root         (0)     1825 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/account_usage.html
--rw-r--r--   0 root         (0) root         (0)     1234 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/account_usage_history.html
--rw-r--r--   0 root         (0) root         (0)      857 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/accounting.html
--rw-r--r--   0 root         (0) root         (0)      996 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/accounts.html
--rw-r--r--   0 root         (0) root         (0)     4233 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/add_rse.html
--rw-r--r--   0 root         (0) root         (0)     4109 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/approve_rules.html
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/atlas_index.html
--rw-r--r--   0 root         (0) root         (0)     2880 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/backlog_mon.html
--rw-r--r--   0 root         (0) root         (0)     1207 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/bad_replicas.html
--rw-r--r--   0 root         (0) root         (0)     1678 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html
--rw-r--r--   0 root         (0) root         (0)     8979 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/base.html
--rw-r--r--   0 root         (0) root         (0)     2652 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/cond.html
--rw-r--r--   0 root         (0) root         (0)     2678 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/dbrelease.html
--rw-r--r--   0 root         (0) root         (0)     2628 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/did.html
--rw-r--r--   0 root         (0) root         (0)     4970 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/dumps.html
--rw-r--r--   0 root         (0) root         (0)     1230 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/heartbeats.html
--rw-r--r--   0 root         (0) root         (0)      585 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/index.html
--rw-r--r--   0 root         (0) root         (0)     1789 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/infrastructure.html
--rw-r--r--   0 root         (0) root         (0)     3499 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/lifetime_exception.html
--rw-r--r--   0 root         (0) root         (0)     1270 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html
--rw-r--r--   0 root         (0) root         (0)     6608 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/list_rules.html
--rw-r--r--   0 root         (0) root         (0)     4440 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/login.html
--rw-r--r--   0 root         (0) root         (0)     1276 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/no_certificate.html
--rw-r--r--   0 root         (0) root         (0)      803 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/problem.html
--rw-r--r--   0 root         (0) root         (0)    16321 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/request_rule.html
--rw-r--r--   0 root         (0) root         (0)     4124 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rse.html
--rw-r--r--   0 root         (0) root         (0)     2380 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rse_account_usage.html
--rw-r--r--   0 root         (0) root         (0)     7277 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rse_add_protocol.html
--rw-r--r--   0 root         (0) root         (0)     1547 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rse_locks.html
--rw-r--r--   0 root         (0) root         (0)     1363 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rse_usage.html
--rw-r--r--   0 root         (0) root         (0)     1796 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rses.html
--rw-r--r--   0 root         (0) root         (0)     1919 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rule.html
--rw-r--r--   0 root         (0) root         (0)     2079 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rules.html
--rw-r--r--   0 root         (0) root         (0)     2164 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/search.html
--rw-r--r--   0 root         (0) root         (0)     5125 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/select_login_method.html
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/subscription.html
--rw-r--r--   0 root         (0) root         (0)      956 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/subscriptionrules.html
--rw-r--r--   0 root         (0) root         (0)     1562 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/subscriptions.html
--rw-r--r--   0 root         (0) root         (0)     5327 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/subscriptions_editor.html
--rw-r--r--   0 root         (0) root         (0)     3024 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/suspicious_replicas.html
--rw-r--r--   0 root         (0) root         (0)      741 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.406482 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/
--rwxr-xr-x   0 root         (0) root         (0)   135652 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/RucioUI.png
--rw-r--r--   0 root         (0) root         (0)      686 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/details_close.png
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/details_open.png
--rw-r--r--   0 root         (0) root         (0)    84798 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/error.jpg
--rw-r--r--   0 root         (0) root         (0)    10510 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.407482 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/fonts/
--rwxr-xr-x   0 root         (0) root         (0)     3400 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/fonts/login_icons.eot
--rwxr-xr-x   0 root         (0) root         (0)     9218 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/fonts/login_icons.svg
--rwxr-xr-x   0 root         (0) root         (0)     3236 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/fonts/login_icons.ttf
--rwxr-xr-x   0 root         (0) root         (0)     3312 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/fonts/login_icons.woff
--rw-r--r--   0 root         (0) root         (0)      753 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/get_info.png
--rw-r--r--   0 root         (0) root         (0)    56517 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/logo.png
--rw-r--r--   0 root         (0) root         (0)    19563 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/rucio_logo.png
--rw-r--r--   0 root         (0) root         (0)    32246 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/spinner.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.432483 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/
--rw-r--r--   0 root         (0) root         (0)     6764 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/account.js
--rw-r--r--   0 root         (0) root         (0)     8084 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/account_rse_usage.js
--rw-r--r--   0 root         (0) root         (0)    12181 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/account_usage.js
--rw-r--r--   0 root         (0) root         (0)     7667 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/account_usage_history.js
--rw-r--r--   0 root         (0) root         (0)     4998 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/accounting.js
--rw-r--r--   0 root         (0) root         (0)     1352 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/accounts.js
--rw-r--r--   0 root         (0) root         (0)     2468 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/add_rse.js
--rw-r--r--   0 root         (0) root         (0)    12226 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/approve_rules.js
--rw-r--r--   0 root         (0) root         (0)     2229 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/atlas_index.js
--rw-r--r--   0 root         (0) root         (0)    15169 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/backlog_mon.js
--rw-r--r--   0 root         (0) root         (0)     1054 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/bad_replicas.js
--rw-r--r--   0 root         (0) root         (0)    11540 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/bad_replicas_summary.js
--rw-r--r--   0 root         (0) root         (0)     7366 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/base.js
--rw-r--r--   0 root         (0) root         (0)      538 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen-sprite.png
--rw-r--r--   0 root         (0) root         (0)      738 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen-sprite@2x.png
--rw-r--r--   0 root         (0) root         (0)    13270 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen.css
--rw-r--r--   0 root         (0) root         (0)    44811 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen.jquery.js
--rw-r--r--   0 root         (0) root         (0)    28401 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen.jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    11061 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen.min.css
--rw-r--r--   0 root         (0) root         (0)    45100 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen.proto.js
--rw-r--r--   0 root         (0) root         (0)    28757 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen.proto.min.js
--rw-r--r--   0 root         (0) root         (0)     5641 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/cond.js
--rw-r--r--   0 root         (0) root         (0)     5758 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/dbrelease.js
--rw-r--r--   0 root         (0) root         (0)    43648 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/did.js
--rw-r--r--   0 root         (0) root         (0)     1396 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/filesize.min.js
--rw-r--r--   0 root         (0) root         (0)    19507 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/foundation-icons.css
--rw-r--r--   0 root         (0) root         (0)    54568 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/foundation-icons.eot
--rw-r--r--   0 root         (0) root         (0)   150251 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/foundation-icons.svg
--rw-r--r--   0 root         (0) root         (0)    56976 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/foundation-icons.ttf
--rw-r--r--   0 root         (0) root         (0)    32020 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/foundation-icons.woff
--rw-r--r--   0 root         (0) root         (0)     1359 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/heartbeats.js
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring.css
--rw-r--r--   0 root         (0) root         (0)    12386 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_account_details.js
--rw-r--r--   0 root         (0) root         (0)     3525 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_accounts.js
--rw-r--r--   0 root         (0) root         (0)     5294 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js
--rw-r--r--   0 root         (0) root         (0)     3795 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_apiclasses.js
--rw-r--r--   0 root         (0) root         (0)     3555 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_index.js
--rw-r--r--   0 root         (0) root         (0)     3043 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_resources.js
--rw-r--r--   0 root         (0) root         (0)     8872 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js
--rw-r--r--   0 root         (0) root         (0)     3055 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_scriptids.js
--rw-r--r--   0 root         (0) root         (0)    10028 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_utils.js
--rw-r--r--   0 root         (0) root         (0)      454 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/index.js
--rw-r--r--   0 root         (0) root         (0)    23108 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/jquery.multiple.select.js
--rw-r--r--   0 root         (0) root         (0)    20021 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/jquery.multiple.select2.js
--rw-r--r--   0 root         (0) root         (0)     4151 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/jquery.quicksearch.js
--rw-r--r--   0 root         (0) root         (0)     6966 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/jquery.storageapi.min.js
--rw-r--r--   0 root         (0) root         (0)    11881 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/lifetime_exception.js
--rw-r--r--   0 root         (0) root         (0)     4060 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/list_lifetime_exceptions.js
--rw-r--r--   0 root         (0) root         (0)    13472 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/list_rules.js
--rw-r--r--   0 root         (0) root         (0)      324 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/login.js
--rw-r--r--   0 root         (0) root         (0)     4279 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/multiple-select.css
--rw-r--r--   0 root         (0) root         (0)     3342 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/multiple-select.png
--rw-r--r--   0 root         (0) root         (0)     2233 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/multiple-select2.css
--rw-r--r--   0 root         (0) root         (0)    54419 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/request_rule.js
--rw-r--r--   0 root         (0) root         (0)     7089 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rse.js
--rw-r--r--   0 root         (0) root         (0)    23373 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rse_account_usage.js
--rw-r--r--   0 root         (0) root         (0)     7076 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rse_add_protocol.js
--rw-r--r--   0 root         (0) root         (0)     6559 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rse_locks.js
--rw-r--r--   0 root         (0) root         (0)    10905 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rse_usage.js
--rw-r--r--   0 root         (0) root         (0)     1632 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rses.js
--rw-r--r--   0 root         (0) root         (0)     2598 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rucio.css
--rw-r--r--   0 root         (0) root         (0)    63519 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rucio.js
--rw-r--r--   0 root         (0) root         (0)    23335 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rule.js
--rw-r--r--   0 root         (0) root         (0)     1341 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rules.js
--rw-r--r--   0 root         (0) root         (0)     6323 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/search.js
--rw-r--r--   0 root         (0) root         (0)     2197 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/select_login_method.css
--rw-r--r--   0 root         (0) root         (0)     7637 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/subscription.js
--rw-r--r--   0 root         (0) root         (0)     3071 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/subscriptionrules.js
--rw-r--r--   0 root         (0) root         (0)     4946 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/subscriptions.js
--rw-r--r--   0 root         (0) root         (0)    13983 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/subscriptions_editor.js
--rw-r--r--   0 root         (0) root         (0)     9784 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/suspicious_replicas.js
--rw-r--r--   0 root         (0) root         (0)      540 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/switch.png
--rw-r--r--   0 root         (0) root         (0)      599 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/version.js
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-26 15:02:05.000000 rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/webui_version
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.462484 rucio-webui-32.0.0rc1/lib/rucio_webui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8831 2023-07-26 15:14:54.000000 rucio-webui-32.0.0rc1/lib/rucio_webui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    16384 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/pylintrc
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5083 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      206 2023-07-26 15:14:54.463484 rucio-webui-32.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2153 2023-07-26 15:14:48.000000 rucio-webui-32.0.0rc1/setup.py
--rw-r--r--   0 root         (0) root         (0)     4749 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/setuputil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:54.461484 rucio-webui-32.0.0rc1/tests/
--rw-r--r--   0 root         (0) root         (0)     3708 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_abacus_account.py
--rw-r--r--   0 root         (0) root         (0)    10771 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_abacus_collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3255 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_abacus_rse.py
--rw-r--r--   0 root         (0) root         (0)    15997 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_account.py
--rw-r--r--   0 root         (0) root         (0)     9834 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_account_limits.py
--rw-r--r--   0 root         (0) root         (0)    20192 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_api_external_representation.py
--rw-r--r--   0 root         (0) root         (0)    13376 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_archive.py
--rw-r--r--   0 root         (0) root         (0)     4120 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_auditor.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_auditor_hdfs.py
--rw-r--r--   0 root         (0) root         (0)     4225 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_auditor_srmdumps.py
--rw-r--r--   0 root         (0) root         (0)    15239 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_automatix.py
--rw-r--r--   0 root         (0) root         (0)    23339 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_bad_replica.py
--rw-r--r--   0 root         (0) root         (0)    12468 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_bb8.py
--rw-r--r--   0 root         (0) root         (0)     4707 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_belleii.py
--rwxr-xr-x   0 root         (0) root         (0)   107211 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_bin_rucio.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     8248 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_clients.py
--rw-r--r--   0 root         (0) root         (0)     1889 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_common_types.py
--rw-r--r--   0 root         (0) root         (0)     6966 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    85465 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_conveyor.py
--rw-r--r--   0 root         (0) root         (0)    22228 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_conveyor_submitter.py
--rw-r--r--   0 root         (0) root         (0)     6971 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     7703 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_credential.py
--rw-r--r--   0 root         (0) root         (0)     7361 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_curl.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_daemons.py
--rw-r--r--   0 root         (0) root         (0)    28205 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_dataset_replicas.py
--rw-r--r--   0 root         (0) root         (0)     2759 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    55592 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_did.py
--rw-r--r--   0 root         (0) root         (0)    29541 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_did_meta_plugins.py
--rw-r--r--   0 root         (0) root         (0)     4209 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_didtype.py
--rw-r--r--   0 root         (0) root         (0)    35378 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7203 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_dumper.py
--rw-r--r--   0 root         (0) root         (0)    16658 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_dumper_consistency.py
--rw-r--r--   0 root         (0) root         (0)    10907 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_dumper_data_model.py
--rw-r--r--   0 root         (0) root         (0)     3158 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_dumper_path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    38325 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     7977 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    10138 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_hermes.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_identity.py
--rw-r--r--   0 root         (0) root         (0)    18578 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_impl_upload_download.py
--rw-r--r--   0 root         (0) root         (0)    57799 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     5281 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_judge_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    22299 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_judge_evaluator.py
--rw-r--r--   0 root         (0) root         (0)    11070 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_judge_injector.py
--rw-r--r--   0 root         (0) root         (0)    20482 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_judge_repairer.py
--rw-r--r--   0 root         (0) root         (0)    12205 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_lifetime.py
--rw-r--r--   0 root         (0) root         (0)     5879 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     6270 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     1790 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_meta_did.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_module_import.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_monitor.py
--rw-r--r--   0 root         (0) root         (0)    54354 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     2911 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_naming_convention.py
--rw-r--r--   0 root         (0) root         (0)    11606 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_oauthmanager.py
--rw-r--r--   0 root         (0) root         (0)   107576 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_oidc.py
--rw-r--r--   0 root         (0) root         (0)     4529 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     4147 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_pfns.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_ping.py
--rw-r--r--   0 root         (0) root         (0)     7607 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2765 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_qos.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    27057 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_reaper.py
--rw-r--r--   0 root         (0) root         (0)     6464 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)    62407 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_replica.py
--rw-r--r--   0 root         (0) root         (0)    32236 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_replica_recoverer.py
--rw-r--r--   0 root         (0) root         (0)    22852 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_replica_sorting.py
--rw-r--r--   0 root         (0) root         (0)    13879 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)    13074 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_root_proxy.py
--rw-r--r--   0 root         (0) root         (0)    75437 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rse.py
--rw-r--r--   0 root         (0) root         (0)    13230 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)     8966 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rse_lfn2path.py
--rw-r--r--   0 root         (0) root         (0)     4300 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 root         (0) root         (0)     3845 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rse_protocol_gfal2_impl.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rse_protocol_posix.py
--rw-r--r--   0 root         (0) root         (0)     3713 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rse_protocol_rclone.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rse_protocol_rsync.py
--rw-r--r--   0 root         (0) root         (0)     4002 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rse_protocol_srm.py
--rw-r--r--   0 root         (0) root         (0)     4678 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rse_protocol_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 root         (0) root         (0)     3803 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 root         (0) root         (0)     7770 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rse_selector.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)    90900 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)    13873 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_schema_cms.py
--rw-r--r--   0 root         (0) root         (0)     7510 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_scope.py
--rw-r--r--   0 root         (0) root         (0)    48744 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)     2771 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_temporary_did.py
--rw-r--r--   0 root         (0) root         (0)    55640 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_throttler.py
--rw-r--r--   0 root         (0) root         (0)     5045 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_tpc.py
--rw-r--r--   0 root         (0) root         (0)     3204 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_trace.py
--rw-r--r--   0 root         (0) root         (0)    19610 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_transfer.py
--rw-r--r--   0 root         (0) root         (0)     8478 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_undertaker.py
--rw-r--r--   0 root         (0) root         (0)    15673 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     6375 2023-07-26 12:29:16.000000 rucio-webui-32.0.0rc1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:09.072995 rucio-webui-32.0.0rc2/
+-rwxr-xr-x   0 root         (0) root         (0)     4383 2023-08-03 09:00:33.000000 rucio-webui-32.0.0rc2/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      484 2023-08-03 15:23:02.000000 rucio-webui-32.0.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      841 2023-08-03 15:23:09.072995 rucio-webui-32.0.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:08.996994 rucio-webui-32.0.0rc2/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:09.001994 rucio-webui-32.0.0rc2/lib/rucio/
+-rw-r--r--   0 root         (0) root         (0)      684 2023-08-03 09:00:33.000000 rucio-webui-32.0.0rc2/lib/rucio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      714 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/lib/rucio/alembicrevision.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-08-03 14:15:48.000000 rucio-webui-32.0.0rc2/lib/rucio/vcsversion.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/lib/rucio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:09.001994 rucio-webui-32.0.0rc2/lib/rucio/web/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:09.002994 rucio-webui-32.0.0rc2/lib/rucio/web/ui/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:09.002994 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6202 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/bp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:09.003994 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/common/
+-rwxr-xr-x   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:09.004994 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/common/saml/
+-rw-r--r--   0 root         (0) root         (0)      990 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/common/saml/advanced_settings.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:09.004994 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/common/saml/certs/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/common/saml/certs/README
+-rw-r--r--   0 root         (0) root         (0)      656 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/common/saml/settings.json
+-rw-r--r--   0 root         (0) root         (0)    27924 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/common/utils.py
+-rw-r--r--   0 root         (0) root         (0)      917 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:09.017994 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/account.html
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/account_rse_usage.html
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/account_usage.html
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/account_usage_history.html
+-rw-r--r--   0 root         (0) root         (0)      857 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/accounting.html
+-rw-r--r--   0 root         (0) root         (0)      996 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/accounts.html
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/add_rse.html
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/approve_rules.html
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/atlas_index.html
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/backlog_mon.html
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/bad_replicas.html
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html
+-rw-r--r--   0 root         (0) root         (0)     8979 2023-08-03 09:00:33.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)     2652 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/cond.html
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/dbrelease.html
+-rw-r--r--   0 root         (0) root         (0)     2628 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/did.html
+-rw-r--r--   0 root         (0) root         (0)     4970 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/dumps.html
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/heartbeats.html
+-rw-r--r--   0 root         (0) root         (0)      585 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/index.html
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/infrastructure.html
+-rw-r--r--   0 root         (0) root         (0)     3499 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/lifetime_exception.html
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html
+-rw-r--r--   0 root         (0) root         (0)     6608 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/list_rules.html
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/login.html
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/no_certificate.html
+-rw-r--r--   0 root         (0) root         (0)      803 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/problem.html
+-rw-r--r--   0 root         (0) root         (0)    16321 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/request_rule.html
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rse.html
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rse_account_usage.html
+-rw-r--r--   0 root         (0) root         (0)     7277 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rse_add_protocol.html
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rse_locks.html
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rse_usage.html
+-rw-r--r--   0 root         (0) root         (0)     1796 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rses.html
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rule.html
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rules.html
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/search.html
+-rw-r--r--   0 root         (0) root         (0)     5125 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/select_login_method.html
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/subscription.html
+-rw-r--r--   0 root         (0) root         (0)      956 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/subscriptionrules.html
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/subscriptions.html
+-rw-r--r--   0 root         (0) root         (0)     5327 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/subscriptions_editor.html
+-rw-r--r--   0 root         (0) root         (0)     3024 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/suspicious_replicas.html
+-rw-r--r--   0 root         (0) root         (0)      741 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:09.020995 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/
+-rwxr-xr-x   0 root         (0) root         (0)   135652 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/RucioUI.png
+-rw-r--r--   0 root         (0) root         (0)      686 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/details_close.png
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/details_open.png
+-rw-r--r--   0 root         (0) root         (0)    84798 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/error.jpg
+-rw-r--r--   0 root         (0) root         (0)    10510 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:09.021994 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/fonts/
+-rwxr-xr-x   0 root         (0) root         (0)     3400 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.eot
+-rwxr-xr-x   0 root         (0) root         (0)     9218 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.svg
+-rwxr-xr-x   0 root         (0) root         (0)     3236 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.ttf
+-rwxr-xr-x   0 root         (0) root         (0)     3312 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.woff
+-rw-r--r--   0 root         (0) root         (0)      753 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/get_info.png
+-rw-r--r--   0 root         (0) root         (0)    56517 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/logo.png
+-rw-r--r--   0 root         (0) root         (0)    19563 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/rucio_logo.png
+-rw-r--r--   0 root         (0) root         (0)    32246 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/spinner.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:09.044995 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/
+-rw-r--r--   0 root         (0) root         (0)     6764 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/account.js
+-rw-r--r--   0 root         (0) root         (0)     8084 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/account_rse_usage.js
+-rw-r--r--   0 root         (0) root         (0)    12181 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/account_usage.js
+-rw-r--r--   0 root         (0) root         (0)     7667 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/account_usage_history.js
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/accounting.js
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/accounts.js
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/add_rse.js
+-rw-r--r--   0 root         (0) root         (0)    12226 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/approve_rules.js
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/atlas_index.js
+-rw-r--r--   0 root         (0) root         (0)    15169 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/backlog_mon.js
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/bad_replicas.js
+-rw-r--r--   0 root         (0) root         (0)    11540 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/bad_replicas_summary.js
+-rw-r--r--   0 root         (0) root         (0)     7366 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/base.js
+-rw-r--r--   0 root         (0) root         (0)      538 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen-sprite.png
+-rw-r--r--   0 root         (0) root         (0)      738 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen-sprite@2x.png
+-rw-r--r--   0 root         (0) root         (0)    13270 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen.css
+-rw-r--r--   0 root         (0) root         (0)    44811 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen.jquery.js
+-rw-r--r--   0 root         (0) root         (0)    28401 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen.jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    11061 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen.min.css
+-rw-r--r--   0 root         (0) root         (0)    45100 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen.proto.js
+-rw-r--r--   0 root         (0) root         (0)    28757 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen.proto.min.js
+-rw-r--r--   0 root         (0) root         (0)     5641 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/cond.js
+-rw-r--r--   0 root         (0) root         (0)     5758 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/dbrelease.js
+-rw-r--r--   0 root         (0) root         (0)    43648 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/did.js
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/filesize.min.js
+-rw-r--r--   0 root         (0) root         (0)    19507 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/foundation-icons.css
+-rw-r--r--   0 root         (0) root         (0)    54568 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/foundation-icons.eot
+-rw-r--r--   0 root         (0) root         (0)   150251 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/foundation-icons.svg
+-rw-r--r--   0 root         (0) root         (0)    56976 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/foundation-icons.ttf
+-rw-r--r--   0 root         (0) root         (0)    32020 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/foundation-icons.woff
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/heartbeats.js
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring.css
+-rw-r--r--   0 root         (0) root         (0)    12386 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_account_details.js
+-rw-r--r--   0 root         (0) root         (0)     3525 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_accounts.js
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js
+-rw-r--r--   0 root         (0) root         (0)     3795 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_apiclasses.js
+-rw-r--r--   0 root         (0) root         (0)     3555 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_index.js
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_resources.js
+-rw-r--r--   0 root         (0) root         (0)     8872 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js
+-rw-r--r--   0 root         (0) root         (0)     3055 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_scriptids.js
+-rw-r--r--   0 root         (0) root         (0)    10028 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_utils.js
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/index.js
+-rw-r--r--   0 root         (0) root         (0)    23108 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/jquery.multiple.select.js
+-rw-r--r--   0 root         (0) root         (0)    20021 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/jquery.multiple.select2.js
+-rw-r--r--   0 root         (0) root         (0)     4151 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/jquery.quicksearch.js
+-rw-r--r--   0 root         (0) root         (0)     6966 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/jquery.storageapi.min.js
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/lifetime_exception.js
+-rw-r--r--   0 root         (0) root         (0)     4060 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/list_lifetime_exceptions.js
+-rw-r--r--   0 root         (0) root         (0)    13472 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/list_rules.js
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/login.js
+-rw-r--r--   0 root         (0) root         (0)     4279 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/multiple-select.css
+-rw-r--r--   0 root         (0) root         (0)     3342 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/multiple-select.png
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/multiple-select2.css
+-rw-r--r--   0 root         (0) root         (0)    54419 2023-08-03 09:00:33.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/request_rule.js
+-rw-r--r--   0 root         (0) root         (0)     7089 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rse.js
+-rw-r--r--   0 root         (0) root         (0)    23373 2023-08-03 09:00:33.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rse_account_usage.js
+-rw-r--r--   0 root         (0) root         (0)     7076 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rse_add_protocol.js
+-rw-r--r--   0 root         (0) root         (0)     6559 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rse_locks.js
+-rw-r--r--   0 root         (0) root         (0)    10905 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rse_usage.js
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rses.js
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rucio.css
+-rw-r--r--   0 root         (0) root         (0)    63519 2023-08-03 09:00:33.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rucio.js
+-rw-r--r--   0 root         (0) root         (0)    23335 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rule.js
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rules.js
+-rw-r--r--   0 root         (0) root         (0)     6323 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/search.js
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/select_login_method.css
+-rw-r--r--   0 root         (0) root         (0)     7637 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/subscription.js
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/subscriptionrules.js
+-rw-r--r--   0 root         (0) root         (0)     4946 2023-08-03 09:00:33.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/subscriptions.js
+-rw-r--r--   0 root         (0) root         (0)    13983 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/subscriptions_editor.js
+-rw-r--r--   0 root         (0) root         (0)     9784 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/suspicious_replicas.js
+-rw-r--r--   0 root         (0) root         (0)      540 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/switch.png
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/version.js
+-rw-r--r--   0 root         (0) root         (0)        9 2023-08-03 14:15:48.000000 rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/webui_version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:09.072995 rucio-webui-32.0.0rc2/lib/rucio_webui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8831 2023-08-03 15:23:08.000000 rucio-webui-32.0.0rc2/lib/rucio_webui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    16384 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/pylintrc
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-27 12:40:37.000000 rucio-webui-32.0.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5083 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2023-08-03 15:23:09.073995 rucio-webui-32.0.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-08-03 15:23:02.000000 rucio-webui-32.0.0rc2/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4749 2023-08-03 09:00:33.000000 rucio-webui-32.0.0rc2/setuputil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:09.072995 rucio-webui-32.0.0rc2/tests/
+-rw-r--r--   0 root         (0) root         (0)     3708 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_abacus_account.py
+-rw-r--r--   0 root         (0) root         (0)    10771 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_abacus_collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3255 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_abacus_rse.py
+-rw-r--r--   0 root         (0) root         (0)    15997 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_account.py
+-rw-r--r--   0 root         (0) root         (0)     9834 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_account_limits.py
+-rw-r--r--   0 root         (0) root         (0)    20192 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_api_external_representation.py
+-rw-r--r--   0 root         (0) root         (0)    13376 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4120 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_auditor.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_auditor_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 root         (0) root         (0)    15239 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_automatix.py
+-rw-r--r--   0 root         (0) root         (0)    23339 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_bad_replica.py
+-rw-r--r--   0 root         (0) root         (0)    12468 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_bb8.py
+-rw-r--r--   0 root         (0) root         (0)     4707 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_belleii.py
+-rwxr-xr-x   0 root         (0) root         (0)   107211 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_bin_rucio.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     8248 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_common_types.py
+-rw-r--r--   0 root         (0) root         (0)     6966 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    84744 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_conveyor.py
+-rw-r--r--   0 root         (0) root         (0)    22228 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_conveyor_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     6971 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     7703 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7361 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_curl.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_daemons.py
+-rw-r--r--   0 root         (0) root         (0)    28205 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_dataset_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    55592 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_did.py
+-rw-r--r--   0 root         (0) root         (0)    29541 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_did_meta_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     4209 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_didtype.py
+-rw-r--r--   0 root         (0) root         (0)    35378 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7203 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_dumper.py
+-rw-r--r--   0 root         (0) root         (0)    16658 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_dumper_consistency.py
+-rw-r--r--   0 root         (0) root         (0)    10907 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_dumper_data_model.py
+-rw-r--r--   0 root         (0) root         (0)     3158 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    38325 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     7977 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    10138 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_hermes.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)    18578 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_impl_upload_download.py
+-rw-r--r--   0 root         (0) root         (0)    57799 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     5281 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_judge_cleaner.py
+-rw-r--r--   0 root         (0) root         (0)    22299 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_judge_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11070 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_judge_injector.py
+-rw-r--r--   0 root         (0) root         (0)    20482 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_judge_repairer.py
+-rw-r--r--   0 root         (0) root         (0)    12205 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_lifetime.py
+-rw-r--r--   0 root         (0) root         (0)     5879 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     6270 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_meta_did.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_module_import.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    54354 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)    11606 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_oauthmanager.py
+-rw-r--r--   0 root         (0) root         (0)   107576 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     4529 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4147 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_pfns.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_ping.py
+-rw-r--r--   0 root         (0) root         (0)     7607 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_qos.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    27057 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_reaper.py
+-rw-r--r--   0 root         (0) root         (0)     6464 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    62407 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_replica.py
+-rw-r--r--   0 root         (0) root         (0)    32236 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_replica_recoverer.py
+-rw-r--r--   0 root         (0) root         (0)    22852 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_replica_sorting.py
+-rw-r--r--   0 root         (0) root         (0)    13879 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)    13074 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_root_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    75437 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rse.py
+-rw-r--r--   0 root         (0) root         (0)    13230 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)     8966 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rse_lfn2path.py
+-rw-r--r--   0 root         (0) root         (0)     4300 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rse_protocol_gfal2_impl.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rse_protocol_rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rse_protocol_rsync.py
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 root         (0) root         (0)     4678 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rse_protocol_ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 root         (0) root         (0)     7770 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)    90900 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)    13873 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_schema_cms.py
+-rw-r--r--   0 root         (0) root         (0)     7510 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_scope.py
+-rw-r--r--   0 root         (0) root         (0)    48744 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     2771 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_temporary_did.py
+-rw-r--r--   0 root         (0) root         (0)    55640 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_throttler.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_tpc.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)    19610 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     8478 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_undertaker.py
+-rw-r--r--   0 root         (0) root         (0)    15673 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     6375 2023-08-03 09:00:39.000000 rucio-webui-32.0.0rc2/tests/test_utils.py
```

### Comparing `rucio-webui-32.0.0rc1/AUTHORS.rst` & `rucio-webui-32.0.0rc2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/LICENSE` & `rucio-webui-32.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/PKG-INFO` & `rucio-webui-32.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio-webui
-Version: 32.0.0rc1
+Version: 32.0.0rc2
 Summary: Rucio WebUI Package
 Home-page: https://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rucio-webui-32.0.0rc1/README.rst` & `rucio-webui-32.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/__init__.py` & `rucio-webui-32.0.0rc2/lib/rucio/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/alembicrevision.py` & `rucio-webui-32.0.0rc2/lib/rucio/alembicrevision.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-ALEMBIC_REVISION = '295289b5a800'  # the current alembic head revision
+ALEMBIC_REVISION = '27e3a68927fb'  # the current alembic head revision
```

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/version.py` & `rucio-webui-32.0.0rc2/lib/rucio/version.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/__init__.py` & `rucio-webui-32.0.0rc2/lib/rucio/web/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/__init__.py` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/__init__.py` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/bp.py` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/bp.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/common/__init__.py` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/common/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/common/saml/advanced_settings.json` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/common/saml/advanced_settings.json`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/common/saml/settings.json` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/common/saml/settings.json`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/common/utils.py` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/common/utils.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/main.py` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/main.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/account.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/account.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/account_rse_usage.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/account_rse_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/account_usage.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/account_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/account_usage_history.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/account_usage_history.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/accounting.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/accounting.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/accounts.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/accounts.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/add_rse.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/add_rse.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/approve_rules.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/approve_rules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/atlas_index.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/atlas_index.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/backlog_mon.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/backlog_mon.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/bad_replicas.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/bad_replicas.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/base.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/base.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/cond.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/cond.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/dbrelease.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/dbrelease.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/did.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/did.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/dumps.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/dumps.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/heartbeats.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/heartbeats.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/index.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/index.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/infrastructure.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/infrastructure.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/lifetime_exception.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/lifetime_exception.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/list_rules.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/list_rules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/login.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/login.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/no_certificate.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/no_certificate.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/problem.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/problem.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/request_rule.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/request_rule.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rse.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rse.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rse_account_usage.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rse_account_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rse_add_protocol.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rse_add_protocol.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rse_locks.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rse_locks.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rse_usage.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rse_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rses.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rses.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rule.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rule.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/rules.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/rules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/search.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/search.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/select_login_method.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/select_login_method.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/subscription.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/subscription.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/subscriptionrules.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/subscriptionrules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/subscriptions.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/subscriptions.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/subscriptions_editor.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/subscriptions_editor.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/flask/templates/suspicious_replicas.html` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/flask/templates/suspicious_replicas.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/main.py` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/main.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/RucioUI.png` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/RucioUI.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/details_close.png` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/details_close.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/details_open.png` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/details_open.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/error.jpg` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/error.jpg`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/favicon.ico` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/favicon.ico`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/fonts/login_icons.eot` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.eot`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/fonts/login_icons.svg` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.svg`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/fonts/login_icons.ttf` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.ttf`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/fonts/login_icons.woff` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/fonts/login_icons.woff`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/get_info.png` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/get_info.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/logo.png` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/logo.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/rucio_logo.png` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/rucio_logo.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/media/spinner.gif` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/media/spinner.gif`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/account.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/account.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/account_rse_usage.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/account_rse_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/account_usage.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/account_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/account_usage_history.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/account_usage_history.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/accounting.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/accounting.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/accounts.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/accounts.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/add_rse.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/add_rse.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/approve_rules.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/approve_rules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/atlas_index.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/atlas_index.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/backlog_mon.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/backlog_mon.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/bad_replicas.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/bad_replicas.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/bad_replicas_summary.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/bad_replicas_summary.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/base.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/base.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen-sprite.png` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen-sprite@2x.png` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen.css` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen.jquery.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen.jquery.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen.jquery.min.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen.min.css` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen.min.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen.proto.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen.proto.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/chosen.proto.min.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/chosen.proto.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/cond.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/cond.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/dbrelease.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/dbrelease.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/did.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/did.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/filesize.min.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/filesize.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/foundation-icons.css` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/foundation-icons.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/foundation-icons.eot` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/foundation-icons.eot`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/foundation-icons.svg` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/foundation-icons.svg`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/foundation-icons.ttf` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/foundation-icons.ttf`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/foundation-icons.woff` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/foundation-icons.woff`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/heartbeats.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/heartbeats.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring.css` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_account_details.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_account_details.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_accounts.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_accounts.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_apiclasses.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_apiclasses.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_index.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_index.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_resources.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_resources.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_scriptids.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_scriptids.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/http_monitoring_utils.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/http_monitoring_utils.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/jquery.multiple.select.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/jquery.multiple.select.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/jquery.multiple.select2.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/jquery.multiple.select2.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/jquery.quicksearch.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/jquery.quicksearch.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/jquery.storageapi.min.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/jquery.storageapi.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/lifetime_exception.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/lifetime_exception.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/list_lifetime_exceptions.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/list_lifetime_exceptions.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/list_rules.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/list_rules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/multiple-select.css` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/multiple-select.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/multiple-select.png` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/multiple-select.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/multiple-select2.css` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/multiple-select2.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/request_rule.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/request_rule.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rse.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rse.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rse_account_usage.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rse_account_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rse_add_protocol.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rse_add_protocol.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rse_locks.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rse_locks.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rse_usage.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rse_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rses.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rses.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rucio.css` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rucio.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rucio.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rucio.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rule.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rule.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/rules.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/rules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/search.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/search.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/select_login_method.css` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/select_login_method.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/subscription.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/subscription.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/subscriptionrules.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/subscriptionrules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/subscriptions.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/subscriptions.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/subscriptions_editor.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/subscriptions_editor.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/suspicious_replicas.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/suspicious_replicas.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/switch.png` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/switch.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio/web/ui/static/version.js` & `rucio-webui-32.0.0rc2/lib/rucio/web/ui/static/version.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/lib/rucio_webui.egg-info/SOURCES.txt` & `rucio-webui-32.0.0rc2/lib/rucio_webui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/pylintrc` & `rucio-webui-32.0.0rc2/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/requirements.txt` & `rucio-webui-32.0.0rc2/requirements.txt`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/setup.py` & `rucio-webui-32.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/setuputil.py` & `rucio-webui-32.0.0rc2/setuputil.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_abacus_account.py` & `rucio-webui-32.0.0rc2/tests/test_abacus_account.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_abacus_collection_replica.py` & `rucio-webui-32.0.0rc2/tests/test_abacus_collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_abacus_rse.py` & `rucio-webui-32.0.0rc2/tests/test_abacus_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_account.py` & `rucio-webui-32.0.0rc2/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_account_limits.py` & `rucio-webui-32.0.0rc2/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_api_external_representation.py` & `rucio-webui-32.0.0rc2/tests/test_api_external_representation.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_archive.py` & `rucio-webui-32.0.0rc2/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_auditor.py` & `rucio-webui-32.0.0rc2/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_auditor_hdfs.py` & `rucio-webui-32.0.0rc2/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_auditor_srmdumps.py` & `rucio-webui-32.0.0rc2/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_authentication.py` & `rucio-webui-32.0.0rc2/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_automatix.py` & `rucio-webui-32.0.0rc2/tests/test_automatix.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_bad_replica.py` & `rucio-webui-32.0.0rc2/tests/test_bad_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_bb8.py` & `rucio-webui-32.0.0rc2/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_belleii.py` & `rucio-webui-32.0.0rc2/tests/test_belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_bin_rucio.py` & `rucio-webui-32.0.0rc2/tests/test_bin_rucio.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_boolean.py` & `rucio-webui-32.0.0rc2/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_clients.py` & `rucio-webui-32.0.0rc2/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_common_types.py` & `rucio-webui-32.0.0rc2/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_config.py` & `rucio-webui-32.0.0rc2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_conveyor.py` & `rucio-webui-32.0.0rc2/tests/test_conveyor.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,39 +50,39 @@
 from rucio.transfertool.fts3 import FTS3Transfertool
 from tests.ruciopytest import NoParallelGroups
 
 MAX_POLL_WAIT_SECONDS = 60
 TEST_FTS_HOST = 'https://fts:8446'
 
 
-def __wait_for_replica_transfer(dst_rse_id, scope, name, state=ReplicaState.AVAILABLE, max_wait_seconds=MAX_POLL_WAIT_SECONDS):
+def __wait_for_replica_transfer(dst_rse_id, scope, name, max_wait_seconds=MAX_POLL_WAIT_SECONDS, transfertool=None):
     """
     Wait for the replica to become AVAILABLE on the given RSE as a result of a pending transfer
     """
     replica = {}
     for _ in range(max_wait_seconds):
-        poller(once=True, older_than=0, partition_wait_time=0)
+        poller(once=True, older_than=0, partition_wait_time=0, transfertool=transfertool)
         finisher(once=True, partition_wait_time=0)
         replica = replica_core.get_replica(rse_id=dst_rse_id, scope=scope, name=name)
-        if replica['state'] == state:
+        if replica['state'] != ReplicaState.COPYING:
             break
         time.sleep(1)
     return replica
 
 
-def __wait_for_request_state(dst_rse_id, scope, name, state, max_wait_seconds=MAX_POLL_WAIT_SECONDS, run_poller=True):
+def __wait_for_state_transition(dst_rse_id, scope, name, max_wait_seconds=MAX_POLL_WAIT_SECONDS, run_poller=True, transfertool=None):
     """
     Wait for the request state to be updated to the given expected state as a result of a pending transfer
     """
     request = {}
     for _ in range(max_wait_seconds):
         if run_poller:
-            poller(once=True, older_than=0, partition_wait_time=0)
+            poller(once=True, older_than=0, partition_wait_time=0, transfertool=transfertool)
         request = request_core.get_request_by_did(rse_id=dst_rse_id, scope=scope, name=name)
-        if request['state'] == state:
+        if request['state'] != RequestState.SUBMITTED:
             break
         time.sleep(1)
     return request
 
 
 def __wait_for_fts_state(request, expected_state, max_wait_seconds=MAX_POLL_WAIT_SECONDS):
     job_state = ''
@@ -252,15 +252,15 @@
     # Register a did which doesn't exist. It will trigger an non-recoverable error during the FTS transfer.
     did = did_factory.random_file_did()
     replica_client.add_replicas(rse=src_rse, files=[{'scope': did['scope'].external, 'name': did['name'], 'bytes': 1, 'adler32': 'aaaaaaaa'}])
 
     rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
     submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=2, partition_wait_time=0, transfertype='single', filter_transfertool=None)
 
-    request = __wait_for_request_state(dst_rse_id=dst_rse_id, state=RequestState.FAILED, **did)
+    request = __wait_for_state_transition(dst_rse_id=dst_rse_id, **did)
     assert 'Unused hop in multi-hop' in request['err_msg']
     assert request['state'] == RequestState.FAILED
     request = request_core.get_request_by_did(rse_id=jump_rse_id, **did)
     assert request['state'] == RequestState.FAILED
     assert request['attributes']['source_replica_expression'] == src_rse
 
     # Each hop is a separate transfer, which will be handled by the poller and marked as failed
@@ -314,15 +314,15 @@
         ]
     )
     replica_client.add_replicas(rse=src_rse, files=[{'scope': did['scope'].external, 'name': did['name'], 'bytes': 1, 'adler32': 'aaaaaaaa'}])
 
     rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
     submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=2, partition_wait_time=0, transfertype='single', filter_transfertool=None)
 
-    request = __wait_for_request_state(dst_rse_id=dst_rse_id, state=RequestState.FAILED, **did)
+    request = __wait_for_state_transition(dst_rse_id=dst_rse_id, **did)
     assert request['state'] == RequestState.FAILED
     request = request_core.get_request_by_did(rse_id=jump_rse_id, **did)
     assert request['state'] == RequestState.FAILED
 
     # Each hop is a separate transfer, which will be handled by the poller and marked as failed
     assert metrics_mock.get_sample_value('rucio_daemons_conveyor_poller_update_request_state_total', labels={'updated': 'True'}) >= 2
 
@@ -370,15 +370,15 @@
 
     # After submission, the source rse is the one which will fail
     request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
     assert request['source_rse'] == src_rse2
     assert request['source_rse_id'] == src_rse2_id
 
     # The source_rse must be updated to the correct one
-    request = __wait_for_request_state(dst_rse_id=dst_rse_id, state=RequestState.DONE, **did)
+    request = __wait_for_state_transition(dst_rse_id=dst_rse_id, **did)
     assert request['source_rse'] == src_rse1
     assert request['source_rse_id'] == src_rse1_id
 
     replica = __wait_for_replica_transfer(dst_rse_id=dst_rse_id, **did)
     assert replica['state'] == ReplicaState.AVAILABLE
 
     # Both entries in source table must be removed after completion
@@ -388,15 +388,15 @@
     # Only one request was handled; doesn't matter that it's multisource
     assert metrics_mock.get_sample_value('rucio_daemons_conveyor_finisher_handle_requests_total') >= 1
     assert metrics_mock.get_sample_value('rucio_daemons_conveyor_poller_update_request_state_total', labels={'updated': 'True'}) >= 1
     assert metrics_mock.get_sample_value(
         'rucio_core_request_get_next_requests_total',
         labels={
             'request_type': 'TRANSFER.STAGEIN.STAGEOUT',
-            'state': 'DONE.FAILED.LOST.SUBMITTING.SUBMISSION_FAILED.NO_SOURCES.ONLY_TAPE_SOURCES.MISMATCH_SCHEME'}
+            'state': 'DONE.FAILED.LOST.SUBMISSION_FAILED.NO_SOURCES.ONLY_TAPE_SOURCES.MISMATCH_SCHEME'}
     )
 
 
 @skip_rse_tests_with_accounts
 @pytest.mark.dirty(reason="leaves files in XRD containers")
 @pytest.mark.noparallel(groups=[NoParallelGroups.XRD, NoParallelGroups.SUBMITTER, NoParallelGroups.RECEIVER])
 def test_multisource_receiver(vo, did_factory, replica_client, root_account, metrics_mock, message_mock):
@@ -494,17 +494,17 @@
         # Register a did which doesn't exist. It will trigger a failure error during the FTS transfer.
         did = did_factory.random_file_did()
         replica_client.add_replicas(rse=src_rse, files=[{'scope': did['scope'].external, 'name': did['name'], 'bytes': 1, 'adler32': 'aaaaaaaa'}])
 
         rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
         submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=2, partition_wait_time=0, transfertype='single', filter_transfertool=None)
 
-        request = __wait_for_request_state(dst_rse_id=jump_rse_id, state=RequestState.FAILED, run_poller=False, **did)
+        request = __wait_for_state_transition(dst_rse_id=jump_rse_id, run_poller=False, **did)
         assert request['state'] == RequestState.FAILED
-        request = __wait_for_request_state(dst_rse_id=dst_rse_id, state=RequestState.FAILED, run_poller=False, **did)
+        request = __wait_for_state_transition(dst_rse_id=dst_rse_id, run_poller=False, **did)
         assert request['state'] == RequestState.FAILED
         assert 'Unused hop in multi-hop' in request['err_msg']
 
         assert metrics_mock.get_sample_value('rucio_daemons_conveyor_receiver_update_request_state_total', labels={'updated': 'True'}) >= 1
 
         # Finisher will handle transfers of the same multihop one hop at a time
         finisher(once=True, partition_wait_time=0)
@@ -546,17 +546,17 @@
         all_rses = [src_rse_id, jump_rse_id, dst_rse_id]
 
         did = did_factory.upload_test_file(src_rse)
         rule_priority = 5
         rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=3600, locked=False, subscription_id=None, priority=rule_priority)
         submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=2, partition_wait_time=0, transfertype='single', filter_transfertool=None)
 
-        request = __wait_for_request_state(dst_rse_id=jump_rse_id, state=RequestState.DONE, run_poller=False, **did)
+        request = __wait_for_state_transition(dst_rse_id=jump_rse_id, run_poller=False, **did)
         assert request['state'] == RequestState.DONE
-        request = __wait_for_request_state(dst_rse_id=dst_rse_id, state=RequestState.DONE, run_poller=False, **did)
+        request = __wait_for_state_transition(dst_rse_id=dst_rse_id, run_poller=False, **did)
         assert request['state'] == RequestState.DONE
 
         fts_response = FTS3Transfertool(external_host=TEST_FTS_HOST).bulk_query({request['external_id']: {request['id']: request}})
         assert fts_response[request['external_id']][request['id']].job_response['priority'] == rule_priority
 
         # Two hops; both handled by receiver
         assert metrics_mock.get_sample_value('rucio_daemons_conveyor_receiver_update_request_state_total', labels={'updated': 'True'}) >= 2
@@ -711,17 +711,17 @@
     assert metrics_mock.get_sample_value(gauge_name, labels={'activity': 'all_activities', 'rse': dst_rse1, 'limit_attr': 'residual_capacity'}) == 0
     assert metrics_mock.get_sample_value(gauge_name, labels={'activity': 'all_activities', 'rse': dst_rse1, 'limit_attr': 'max_transfers'}) == 1
     assert metrics_mock.get_sample_value(gauge_name, labels={'activity': 'all_activities', 'rse': dst_rse1, 'limit_attr': 'active'}) == 1
     assert metrics_mock.get_sample_value(gauge_name, labels={'activity': 'all_activities', 'rse': dst_rse1, 'limit_attr': 'waiting'}) == 1
     request = request_core.get_request_by_did(rse_id=dst_rse_id1, **waiting_did)
     assert request['state'] == RequestState.WAITING
 
-    request = __wait_for_request_state(dst_rse_id=dst_rse_id1, state=RequestState.DONE, **queued_did)
+    request = __wait_for_state_transition(dst_rse_id=dst_rse_id1, **queued_did)
     assert request['state'] == RequestState.DONE
-    request = __wait_for_request_state(dst_rse_id=dst_rse_id2, state=RequestState.DONE, **did1)
+    request = __wait_for_state_transition(dst_rse_id=dst_rse_id2, **did1)
     assert request['state'] == RequestState.DONE
 
     # Now that the submitted transfers are finished, the WAITING one can be queued
     throttler(once=True, partition_wait_time=0)
     request = request_core.get_request_by_did(rse_id=dst_rse_id1, **waiting_did)
     assert request['state'] == RequestState.QUEUED
 
@@ -797,17 +797,16 @@
                                            'requested_at': datetime.utcnow()}])
     stager(once=True, rses=[{'id': rse_id} for rse_id in all_rses])
 
     replica = __wait_for_replica_transfer(dst_rse_id=dst_rse_id, max_wait_seconds=2 * MAX_POLL_WAIT_SECONDS, **did)
     assert replica['state'] == ReplicaState.AVAILABLE
 
 
-@skip_rse_tests_with_accounts
 @pytest.mark.noparallel(groups=[NoParallelGroups.SUBMITTER, NoParallelGroups.FINISHER])
-def test_transfer_to_mas_existing_replica(rse_factory, did_factory, root_account):
+def test_transfer_to_mas_existing_replica(rse_factory, did_factory, root_account, jdoe_account):
     """
     Test qos: transfer from tape to disk
     Assert rse maximum_pin_lifetime is passed to transfer tool in the transfer request
     Test rule and lock state transitions
     """
     src_rse, src_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default', rse_type=RSEType.TAPE)
     dst_rse, dst_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default', rse_type=RSEType.DISK)
@@ -827,28 +826,26 @@
     assert request['request_type'] == RequestType.TRANSFER
 
     submitter(once=True, rses=[{'id': dst_rse_id}], partition_wait_time=0, transfertools=['mock'], transfertype='single', filter_transfertool=None)
 
     assert lock_core.get_replica_locks_for_rule_id(rule_id=rule1_id)[0]['state'] == LockState.REPLICATING
     assert rule_core.get_rule(rule1_id)['state'] == RuleState.REPLICATING
 
-    # mock a successful transfer
-    request = request_core.get_request(request_id=request['id'])
-    request_core.set_request_state(request_id=request['id'], state=RequestState.DONE, external_id=request['external_id'])
-    finisher(once=True, partition_wait_time=0)
+    replica = __wait_for_replica_transfer(dst_rse_id=dst_rse_id, transfertool='mock', **did)
+    assert replica['state'] == ReplicaState.AVAILABLE
 
     assert rule_core.get_rule(rule1_id)['state'] == RuleState.OK
 
     # assert all replicas available
     for rse_id in all_rses:
         assert replica_core.get_replica(rse_id=rse_id, **did)['state'] == ReplicaState.AVAILABLE
 
     # now test a second rule, different account
-    set_local_account_limit(InternalAccount('jdoe'), dst_rse_id, bytes_=-1)
-    rule2_id = rule_core.add_rule(dids=[did], account=InternalAccount('jdoe'), copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=-1, locked=False, subscription_id=None, source_replica_expression=dst_rse)[0]
+    set_local_account_limit(jdoe_account, dst_rse_id, bytes_=-1)
+    rule2_id = rule_core.add_rule(dids=[did], account=jdoe_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=-1, locked=False, subscription_id=None, source_replica_expression=dst_rse)[0]
     request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
 
     assert request['request_type'] == RequestType.STAGEIN
 
     stager(once=True, rses=[{'id': dst_rse_id}])
 
     assert request['attributes']['lifetime'] == str(maximum_pin_lifetime)
@@ -862,17 +859,16 @@
 
     assert lock_core.get_replica_locks_for_rule_id(rule_id=rule1_id)[0]['state'] == LockState.OK
     assert rule_core.get_rule(rule1_id)['state'] == RuleState.OK
     assert lock_core.get_replica_locks_for_rule_id(rule_id=rule2_id)[0]['state'] == LockState.OK
     assert rule_core.get_rule(rule2_id)['state'] == RuleState.OK
 
 
-@skip_rse_tests_with_accounts
 @pytest.mark.noparallel(groups=[NoParallelGroups.SUBMITTER, NoParallelGroups.POLLER, NoParallelGroups.FINISHER])
-def test_failed_transfers_to_mas_existing_replica(rse_factory, did_factory, root_account):
+def test_failed_transfers_to_mas_existing_replica(rse_factory, did_factory, root_account, jdoe_account):
     """
     Test qos: transfer from tape to disk
     Assert rse maximum_pin_lifetime is passed to transfer tool in the transfer request
     Test rule and lock state transitions
     """
     src_rse, src_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default', rse_type=RSEType.TAPE)
     dst_rse, dst_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default', rse_type=RSEType.DISK)
@@ -901,16 +897,16 @@
     finisher(once=True, partition_wait_time=0)
     lock_core.failed_transfer(scope=did['scope'], name=did['name'], rse_id=dst_rse_id)
 
     assert rule_core.get_rule(rule1_id)['state'] == RuleState.STUCK
     assert lock_core.get_replica_locks_for_rule_id(rule_id=rule1_id)[0]['state'] == LockState.STUCK
 
     # now test a second rule, different account
-    set_local_account_limit(InternalAccount('jdoe'), dst_rse_id, bytes_=-1)
-    rule2_id = rule_core.add_rule(dids=[did], account=InternalAccount('jdoe'), copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=-1, locked=False, subscription_id=None, source_replica_expression=dst_rse)[0]
+    set_local_account_limit(jdoe_account, dst_rse_id, bytes_=-1)
+    rule2_id = rule_core.add_rule(dids=[did], account=jdoe_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=-1, locked=False, subscription_id=None, source_replica_expression=dst_rse)[0]
     request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
 
     # since the first rule is STUCK assert a transfer not stagein
     assert request['request_type'] == RequestType.TRANSFER
 
     submitter(once=True, rses=[{'id': dst_rse_id}], partition_wait_time=0, transfertools=['mock'], transfertype='single', filter_transfertool=None)
 
@@ -954,15 +950,15 @@
 
     # Fake that the transfer is submitted and lost
     submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=2, partition_wait_time=0, transfertype='single', filter_transfertool=None)
     request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
     __update_request(request['id'], external_id='some-fake-random-id')
 
     # The request must be marked lost
-    request = __wait_for_request_state(dst_rse_id=dst_rse_id, state=RequestState.LOST, **did)
+    request = __wait_for_state_transition(dst_rse_id=dst_rse_id, **did)
     assert request['state'] == RequestState.LOST
 
     # Set update time far in the past to bypass protections (not resubmitting too fast).
     # Run finisher and submitter, the request must be resubmitted and transferred correctly
     __update_request(request['id'], updated_at=datetime.utcnow() - timedelta(days=1))
     finisher(once=True, partition_wait_time=0)
     # The source ranking must not be updated for submission failures and lost transfers
@@ -1112,18 +1108,18 @@
     Ensure that overwrite is not set for transfers towards TAPE RSEs
     """
     rse1_id, rse2_id, rse3_id, did1, did2 = overwrite_on_tape_topology(did1_corrupted=False, did2_corrupted=True)
     all_rses = [rse1_id, rse2_id, rse3_id]
 
     submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=10, partition_wait_time=0, transfertype='single', filter_transfertool=None)
 
-    request = __wait_for_request_state(dst_rse_id=rse3_id, state=RequestState.FAILED, **did1)
+    request = __wait_for_state_transition(dst_rse_id=rse3_id, **did1)
     assert request['state'] == RequestState.FAILED
     assert 'Destination file exists and overwrite is not enabled' in request['err_msg']
-    request = __wait_for_request_state(dst_rse_id=rse3_id, state=RequestState.FAILED, **did2)
+    request = __wait_for_state_transition(dst_rse_id=rse3_id, **did2)
     assert request['state'] == RequestState.FAILED
     assert 'Destination file exists and overwrite is not enabled' in request['err_msg']
 
 
 @skip_rse_tests_with_accounts
 @pytest.mark.dirty(reason="leaves files in XRD containers")
 @pytest.mark.noparallel(groups=[NoParallelGroups.SUBMITTER, NoParallelGroups.POLLER])
@@ -1151,27 +1147,27 @@
     all_rses = [rse1_id, rse2_id, rse3_id]
 
     submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=10, partition_wait_time=0, transfertype='single', filter_transfertool=None)
 
     fts_schema_version = FTS3Transfertool(external_host=TEST_FTS_HOST).version()['schema']['major']
     if fts_schema_version >= 8:
         # Newer fts version will honor the overwrite_hop
-        request = __wait_for_request_state(dst_rse_id=rse2_id, state=RequestState.DONE, **did1)
+        request = __wait_for_state_transition(dst_rse_id=rse2_id, **did1)
         assert request['state'] == RequestState.DONE
-        request = __wait_for_request_state(dst_rse_id=rse3_id, state=RequestState.FAILED, **did1)
+        request = __wait_for_state_transition(dst_rse_id=rse3_id, **did1)
         assert request['state'] == RequestState.FAILED
         assert 'Destination file exists and overwrite is not enabled' in request['err_msg']
     else:
         # FTS only recently introduced the overwrite_hops parameter. It will be ignored on old
         # fts versions and the first hop will fail with the  file exists error
         # TODO: remove this else after FTS 3.12 release and after updating rucio/fts container with the new release
-        request = __wait_for_request_state(dst_rse_id=rse2_id, state=RequestState.FAILED, **did1)
+        request = __wait_for_state_transition(dst_rse_id=rse2_id, **did1)
         assert request['state'] == RequestState.FAILED
         assert 'Destination file exists and overwrite is not enabled' in request['err_msg']
-        request = __wait_for_request_state(dst_rse_id=rse3_id, state=RequestState.FAILED, **did1)
+        request = __wait_for_state_transition(dst_rse_id=rse3_id, **did1)
         assert request['state'] == RequestState.FAILED
         assert 'Unused hop in multi-hop' in request['err_msg']
 
 
 @skip_rse_tests_with_accounts
 @pytest.mark.dirty(reason="leaves files in XRD containers")
 @pytest.mark.noparallel(groups=[NoParallelGroups.SUBMITTER, NoParallelGroups.POLLER])
@@ -1200,17 +1196,17 @@
                         # As we don't really have tape RSEs in our tests, file_on_tape is always false
                         file['file_metadata']['dst_file']['file_on_tape'] = True
             return job_params
 
     with patch('rucio.daemons.conveyor.poller.FTS3Transfertool', _FTSWrapper):
         submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=10, partition_wait_time=0, transfertype='single', filter_transfertool=None)
 
-        request = __wait_for_request_state(dst_rse_id=rse3_id, state=RequestState.DONE, **did1)
+        request = __wait_for_state_transition(dst_rse_id=rse3_id, **did1)
         assert request['state'] == RequestState.DONE
-        request = __wait_for_request_state(dst_rse_id=rse3_id, state=RequestState.DONE, **did2)
+        request = __wait_for_state_transition(dst_rse_id=rse3_id, **did2)
         assert request['state'] == RequestState.DONE
 
 
 @skip_rse_tests_with_accounts
 @pytest.mark.dirty(reason="leaves files in XRD containers; leaves pending fts transfers in archiving state")
 @pytest.mark.noparallel(groups=[NoParallelGroups.SUBMITTER, NoParallelGroups.POLLER, NoParallelGroups.FINISHER])
 @pytest.mark.parametrize("core_config_mock", [{"table_content": [
@@ -1241,33 +1237,33 @@
                         # As we don't really have tape RSEs in our tests, file_on_tape is always false
                         file['file_metadata']['dst_file']['file_on_tape'] = True
             return job_params
 
     with patch('rucio.daemons.conveyor.poller.FTS3Transfertool', _FTSWrapper):
         submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=10, partition_wait_time=0, transfertype='single', filter_transfertool=None)
         # Both transfers must be marked as failed because the file size is incorrect
-        request = __wait_for_request_state(dst_rse_id=rse3_id, state=RequestState.FAILED, **did1)
+        request = __wait_for_state_transition(dst_rse_id=rse3_id, **did1)
         assert request['state'] == RequestState.FAILED
-        request = __wait_for_request_state(dst_rse_id=rse3_id, state=RequestState.FAILED, **did2)
+        request = __wait_for_state_transition(dst_rse_id=rse3_id, **did2)
         assert request['state'] == RequestState.FAILED
 
         # Re-submit the failed requests. They must fail again, because overwrite_corrupted_files is False
         # 2 runs: for multihop, finisher works one hop at a time
         finisher(once=True, partition_wait_time=0)
         finisher(once=True, partition_wait_time=0)
         request = request_core.get_request_by_did(rse_id=rse3_id, **did1)
         assert request['state'] == RequestState.QUEUED
         request = request_core.get_request_by_did(rse_id=rse3_id, **did2)
         assert request['state'] == RequestState.QUEUED
         submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=10, partition_wait_time=0, transfertype='single', filter_transfertool=None)
         # Set overwrite to True before running the poller or finisher
         core_config.set('transfers', 'overwrite_corrupted_files', True)
-        request = __wait_for_request_state(dst_rse_id=rse3_id, state=RequestState.FAILED, **did1)
+        request = __wait_for_state_transition(dst_rse_id=rse3_id, **did1)
         assert request['state'] == RequestState.FAILED
-        request = __wait_for_request_state(dst_rse_id=rse3_id, state=RequestState.FAILED, **did2)
+        request = __wait_for_state_transition(dst_rse_id=rse3_id, **did2)
         assert request['state'] == RequestState.FAILED
 
         # Re-submit one more time. Now the destination file must be overwritten
         finisher(once=True, partition_wait_time=0)
         finisher(once=True, partition_wait_time=0)
         request = request_core.get_request_by_did(rse_id=rse3_id, **did1)
         assert request['state'] == RequestState.QUEUED
@@ -1394,15 +1390,15 @@
             # Simulate using the mock gfal plugin a transfer failure
             file['sources'] = [set_query_parameters(s_url, {'errno': 2}) for s_url in file['sources']]
 
     # Submit the first time, but force a failure to verify that retries are correctly handled
     with patch('rucio.core.transfer.TRANSFERTOOL_CLASSES_BY_NAME', new={'fts3': _FTSWrapper}):
         submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=10, partition_wait_time=0, transfertype='single', filter_transfertool=None)
 
-    request = __wait_for_request_state(dst_rse_id=rse2_id, state=RequestState.FAILED, **did)
+    request = __wait_for_state_transition(dst_rse_id=rse2_id, **did)
     assert request['state'] == RequestState.FAILED
 
     # Re-submit the transfer without simulating a failure. Everything should go as normal starting now.
     for _ in range(4):
         # for multihop, finisher works one hop at a time. 4 is the maximum number of hops in this test graph
         finisher(once=True, partition_wait_time=0)
     submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=10, partition_wait_time=0, transfertype='single', filter_transfertool=None)
@@ -1486,24 +1482,24 @@
             file['sources'] = [set_query_parameters(s_url, {'checksum': replica['adler32']}) for s_url in file['sources']]
             file['destinations'] = [set_query_parameters(d_url, {'checksum': 'randomString2'}) for d_url in file['destinations']]
 
     with patch('rucio.core.transfer.TRANSFERTOOL_CLASSES_BY_NAME', new={'fts3': _FTSWrapper}):
         submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=2, partition_wait_time=0, transfertype='single', filter_transfertool=None)
 
     # Checksum verification disabled on this rse, so the transfer must use source validation and succeed
-    request = __wait_for_request_state(dst_rse_id=dst_rse1_id, state=RequestState.DONE, **did)
+    request = __wait_for_state_transition(dst_rse_id=dst_rse1_id, **did)
     assert request['state'] == RequestState.DONE
 
     # No common supported checksum between the source and destination rse. It will verify the destination rse checksum and fail
-    request = __wait_for_request_state(dst_rse_id=dst_rse2_id, state=RequestState.FAILED, **did)
+    request = __wait_for_state_transition(dst_rse_id=dst_rse2_id, **did)
     assert request['state'] == RequestState.FAILED
     assert 'User and destination checksums do not match' in request['err_msg']
 
     # Common checksum exists between the two. It must use "both" validation strategy and fail
-    request = __wait_for_request_state(dst_rse_id=dst_rse3_id, state=RequestState.FAILED, **did)
+    request = __wait_for_state_transition(dst_rse_id=dst_rse3_id, **did)
     assert 'Source and destination checksums do not match' in request['err_msg']
     assert request['state'] == RequestState.FAILED
 
 
 @pytest.mark.noparallel(groups=[NoParallelGroups.PREPARER])
 @pytest.mark.parametrize("file_config_mock", [{
     "overrides": [('conveyor', 'use_preparer', 'true')]
```

### Comparing `rucio-webui-32.0.0rc1/tests/test_conveyor_submitter.py` & `rucio-webui-32.0.0rc2/tests/test_conveyor_submitter.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_counter.py` & `rucio-webui-32.0.0rc2/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_credential.py` & `rucio-webui-32.0.0rc2/tests/test_credential.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_curl.py` & `rucio-webui-32.0.0rc2/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_daemons.py` & `rucio-webui-32.0.0rc2/tests/test_daemons.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_dataset_replicas.py` & `rucio-webui-32.0.0rc2/tests/test_dataset_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_db.py` & `rucio-webui-32.0.0rc2/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_did.py` & `rucio-webui-32.0.0rc2/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_did_meta_plugins.py` & `rucio-webui-32.0.0rc2/tests/test_did_meta_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_didtype.py` & `rucio-webui-32.0.0rc2/tests/test_didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_download.py` & `rucio-webui-32.0.0rc2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_dumper.py` & `rucio-webui-32.0.0rc2/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_dumper_consistency.py` & `rucio-webui-32.0.0rc2/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_dumper_data_model.py` & `rucio-webui-32.0.0rc2/tests/test_dumper_data_model.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_dumper_path_parsing.py` & `rucio-webui-32.0.0rc2/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_filter_engine.py` & `rucio-webui-32.0.0rc2/tests/test_filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_heartbeat.py` & `rucio-webui-32.0.0rc2/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_hermes.py` & `rucio-webui-32.0.0rc2/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_identity.py` & `rucio-webui-32.0.0rc2/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_impl_upload_download.py` & `rucio-webui-32.0.0rc2/tests/test_impl_upload_download.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_import_export.py` & `rucio-webui-32.0.0rc2/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_judge_cleaner.py` & `rucio-webui-32.0.0rc2/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_judge_evaluator.py` & `rucio-webui-32.0.0rc2/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_judge_injector.py` & `rucio-webui-32.0.0rc2/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_judge_repairer.py` & `rucio-webui-32.0.0rc2/tests/test_judge_repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_lifetime.py` & `rucio-webui-32.0.0rc2/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_message.py` & `rucio-webui-32.0.0rc2/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_meta.py` & `rucio-webui-32.0.0rc2/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_meta_did.py` & `rucio-webui-32.0.0rc2/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_module_import.py` & `rucio-webui-32.0.0rc2/tests/test_module_import.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_monitor.py` & `rucio-webui-32.0.0rc2/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_multi_vo.py` & `rucio-webui-32.0.0rc2/tests/test_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_naming_convention.py` & `rucio-webui-32.0.0rc2/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_oauthmanager.py` & `rucio-webui-32.0.0rc2/tests/test_oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_oidc.py` & `rucio-webui-32.0.0rc2/tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_permission.py` & `rucio-webui-32.0.0rc2/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_pfns.py` & `rucio-webui-32.0.0rc2/tests/test_pfns.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_ping.py` & `rucio-webui-32.0.0rc2/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_preparer.py` & `rucio-webui-32.0.0rc2/tests/test_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_qos.py` & `rucio-webui-32.0.0rc2/tests/test_qos.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_quarantined_replica.py` & `rucio-webui-32.0.0rc2/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_reaper.py` & `rucio-webui-32.0.0rc2/tests/test_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_redirect.py` & `rucio-webui-32.0.0rc2/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_replica.py` & `rucio-webui-32.0.0rc2/tests/test_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_replica_recoverer.py` & `rucio-webui-32.0.0rc2/tests/test_replica_recoverer.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_replica_sorting.py` & `rucio-webui-32.0.0rc2/tests/test_replica_sorting.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_request.py` & `rucio-webui-32.0.0rc2/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_root_proxy.py` & `rucio-webui-32.0.0rc2/tests/test_root_proxy.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rse.py` & `rucio-webui-32.0.0rc2/tests/test_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rse_expression_parser.py` & `rucio-webui-32.0.0rc2/tests/test_rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rse_lfn2path.py` & `rucio-webui-32.0.0rc2/tests/test_rse_lfn2path.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rse_protocol_gfal2.py` & `rucio-webui-32.0.0rc2/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rse_protocol_gfal2_impl.py` & `rucio-webui-32.0.0rc2/tests/test_rse_protocol_gfal2_impl.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rse_protocol_posix.py` & `rucio-webui-32.0.0rc2/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rse_protocol_rclone.py` & `rucio-webui-32.0.0rc2/tests/test_rse_protocol_rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rse_protocol_rsync.py` & `rucio-webui-32.0.0rc2/tests/test_rse_protocol_rsync.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rse_protocol_srm.py` & `rucio-webui-32.0.0rc2/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rse_protocol_ssh.py` & `rucio-webui-32.0.0rc2/tests/test_rse_protocol_ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rse_protocol_webdav.py` & `rucio-webui-32.0.0rc2/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rse_protocol_xrootd.py` & `rucio-webui-32.0.0rc2/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rse_selector.py` & `rucio-webui-32.0.0rc2/tests/test_rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rucio_server.py` & `rucio-webui-32.0.0rc2/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_rule.py` & `rucio-webui-32.0.0rc2/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_schema_cms.py` & `rucio-webui-32.0.0rc2/tests/test_schema_cms.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_scope.py` & `rucio-webui-32.0.0rc2/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_subscription.py` & `rucio-webui-32.0.0rc2/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_temporary_did.py` & `rucio-webui-32.0.0rc2/tests/test_temporary_did.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_throttler.py` & `rucio-webui-32.0.0rc2/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_tpc.py` & `rucio-webui-32.0.0rc2/tests/test_tpc.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_trace.py` & `rucio-webui-32.0.0rc2/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_transfer.py` & `rucio-webui-32.0.0rc2/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_undertaker.py` & `rucio-webui-32.0.0rc2/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_upload.py` & `rucio-webui-32.0.0rc2/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-32.0.0rc1/tests/test_utils.py` & `rucio-webui-32.0.0rc2/tests/test_utils.py`

 * *Files identical despite different names*

