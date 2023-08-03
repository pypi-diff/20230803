# Comparing `tmp/rucio-32.0.0rc1.tar.gz` & `tmp/rucio-32.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-32.0.0rc1.tar", last modified: Wed Jul 26 15:17:24 2023, max compression
+gzip compressed data, was "rucio-32.0.0rc2.tar", last modified: Thu Aug  3 15:22:55 2023, max compression
```

## Comparing `rucio-32.0.0rc1.tar` & `rucio-32.0.0rc2.tar`

### file list

```diff
@@ -1,635 +1,636 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.703677 rucio-32.0.0rc1/
--rwxr-xr-x   0 root         (0) root         (0)     4383 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      934 2023-07-26 15:17:17.000000 rucio-32.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-26 15:17:24.703677 rucio-32.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1982 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.524669 rucio-32.0.0rc1/bin/
--rwxr-xr-x   0 root         (0) root         (0)   128576 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio
--rwxr-xr-x   0 root         (0) root         (0)     2844 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-abacus-account
--rwxr-xr-x   0 root         (0) root         (0)     1847 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-abacus-collection-replica
--rwxr-xr-x   0 root         (0) root         (0)     2591 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-abacus-rse
--rwxr-xr-x   0 root         (0) root         (0)   133738 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-admin
--rwxr-xr-x   0 root         (0) root         (0)     3209 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-atropos
--rwxr-xr-x   0 root         (0) root         (0)     5873 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-auditor
--rwxr-xr-x   0 root         (0) root         (0)     2033 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-automatix
--rwxr-xr-x   0 root         (0) root         (0)     3127 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-bb8
--rwxr-xr-x   0 root         (0) root         (0)     6124 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-c3po
--rwxr-xr-x   0 root         (0) root         (0)     5087 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-cache-client
--rwxr-xr-x   0 root         (0) root         (0)     1386 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-cache-consumer
--rwxr-xr-x   0 root         (0) root         (0)     2370 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-conveyor-finisher
--rwxr-xr-x   0 root         (0) root         (0)     2863 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-conveyor-poller
--rwxr-xr-x   0 root         (0) root         (0)     1783 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-conveyor-preparer
--rwxr-xr-x   0 root         (0) root         (0)     1706 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-conveyor-receiver
--rwxr-xr-x   0 root         (0) root         (0)     3409 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-conveyor-stager
--rwxr-xr-x   0 root         (0) root         (0)     6774 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-conveyor-submitter
--rwxr-xr-x   0 root         (0) root         (0)     3883 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-conveyor-throttler
--rwxr-xr-x   0 root         (0) root         (0)     2570 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-dark-reaper
--rwxr-xr-x   0 root         (0) root         (0)     6493 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-dumper
--rwxr-xr-x   0 root         (0) root         (0)     1438 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-follower
--rwxr-xr-x   0 root         (0) root         (0)     2011 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-hermes
--rwxr-xr-x   0 root         (0) root         (0)     4673 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-judge-cleaner
--rwxr-xr-x   0 root         (0) root         (0)     7494 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-judge-evaluator
--rwxr-xr-x   0 root         (0) root         (0)     1695 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-judge-injector
--rwxr-xr-x   0 root         (0) root         (0)     1699 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-judge-repairer
--rwxr-xr-x   0 root         (0) root         (0)     1806 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-kronos
--rwxr-xr-x   0 root         (0) root         (0)     2510 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-light-reaper
--rwxr-xr-x   0 root         (0) root         (0)     2284 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-minos
--rwxr-xr-x   0 root         (0) root         (0)     2021 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-minos-temporary-expiration
--rwxr-xr-x   0 root         (0) root         (0)     5649 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-necromancer
--rwxr-xr-x   0 root         (0) root         (0)     2812 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-oauth-manager
--rwxr-xr-x   0 root         (0) root         (0)     4094 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-reaper
--rwxr-xr-x   0 root         (0) root         (0)    19015 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-replica-recoverer
--rwxr-xr-x   0 root         (0) root         (0)     3944 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-storage-consistency-actions
--rwxr-xr-x   0 root         (0) root         (0)     3388 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-transmogrifier
--rwxr-xr-x   0 root         (0) root         (0)     2744 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/bin/rucio-undertaker
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.527669 rucio-32.0.0rc1/etc/
--rw-r--r--   0 root         (0) root         (0)     1764 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/etc/alembic.ini.template
--rw-r--r--   0 root         (0) root         (0)     1922 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/etc/alembic_offline.ini.template
--rw-r--r--   0 root         (0) root         (0)       96 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/etc/globus-config.yml.template
--rw-r--r--   0 root         (0) root         (0)      807 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/etc/ldap.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.529669 rucio-32.0.0rc1/etc/mail_templates/
--rw-r--r--   0 root         (0) root         (0)     1210 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/etc/mail_templates/rule_approval_request.tmpl
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/etc/mail_templates/rule_approved_admin.tmpl
--rw-r--r--   0 root         (0) root         (0)      499 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/etc/mail_templates/rule_approved_user.tmpl
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/etc/mail_templates/rule_denied_admin.tmpl
--rw-r--r--   0 root         (0) root         (0)      493 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/etc/mail_templates/rule_denied_user.tmpl
--rw-r--r--   0 root         (0) root         (0)      546 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/etc/mail_templates/rule_ok_notification.tmpl
--rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/etc/rse-accounts.cfg.template
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/etc/rucio.cfg.atlas.client.template
--rw-r--r--   0 root         (0) root         (0)     8534 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/etc/rucio.cfg.template
--rw-r--r--   0 root         (0) root         (0)     7477 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/etc/rucio_multi_vo.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.500667 rucio-32.0.0rc1/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.530669 rucio-32.0.0rc1/lib/rucio/
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      714 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/alembicrevision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.538669 rucio-32.0.0rc1/lib/rucio/api/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9316 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/account.py
--rw-r--r--   0 root         (0) root         (0)    11419 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/account_limit.py
--rw-r--r--   0 root         (0) root         (0)    12914 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/authentication.py
--rw-r--r--   0 root         (0) root         (0)     8678 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/config.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/credential.py
--rw-r--r--   0 root         (0) root         (0)    28229 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/did.py
--rw-r--r--   0 root         (0) root         (0)     3055 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/dirac.py
--rw-r--r--   0 root         (0) root         (0)     2129 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/exporter.py
--rw-r--r--   0 root         (0) root         (0)     2675 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/heartbeat.py
--rw-r--r--   0 root         (0) root         (0)     6853 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/identity.py
--rw-r--r--   0 root         (0) root         (0)     1755 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/importer.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/lifetime_exception.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/lock.py
--rw-r--r--   0 root         (0) root         (0)     3070 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/meta.py
--rw-r--r--   0 root         (0) root         (0)     2689 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/permission.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    21882 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/replica.py
--rw-r--r--   0 root         (0) root         (0)     9627 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/request.py
--rw-r--r--   0 root         (0) root         (0)    23605 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/rse.py
--rw-r--r--   0 root         (0) root         (0)    15962 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/rule.py
--rw-r--r--   0 root         (0) root         (0)     3027 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/scope.py
--rw-r--r--   0 root         (0) root         (0)    10561 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/temporary_did.py
--rw-r--r--   0 root         (0) root         (0)     4583 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/api/vo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.546670 rucio-32.0.0rc1/lib/rucio/client/
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16412 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/accountclient.py
--rw-r--r--   0 root         (0) root         (0)     6020 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/accountlimitclient.py
--rw-r--r--   0 root         (0) root         (0)    47219 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/baseclient.py
--rw-r--r--   0 root         (0) root         (0)     3072 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/client.py
--rw-r--r--   0 root         (0) root         (0)     4460 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/configclient.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/credentialclient.py
--rw-r--r--   0 root         (0) root         (0)    28223 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/didclient.py
--rw-r--r--   0 root         (0) root         (0)     1991 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/diracclient.py
--rw-r--r--   0 root         (0) root         (0)    86127 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/downloadclient.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/exportclient.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/fileclient.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/importclient.py
--rw-r--r--   0 root         (0) root         (0)     2881 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/lifetimeclient.py
--rw-r--r--   0 root         (0) root         (0)     3973 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/lockclient.py
--rw-r--r--   0 root         (0) root         (0)     4722 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/metaclient.py
--rw-r--r--   0 root         (0) root         (0)     1414 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/pingclient.py
--rw-r--r--   0 root         (0) root         (0)    19343 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/replicaclient.py
--rw-r--r--   0 root         (0) root         (0)     4256 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/requestclient.py
--rw-r--r--   0 root         (0) root         (0)    27183 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/rseclient.py
--rw-r--r--   0 root         (0) root         (0)    12741 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/ruleclient.py
--rw-r--r--   0 root         (0) root         (0)     3206 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/scopeclient.py
--rw-r--r--   0 root         (0) root         (0)     7980 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/subscriptionclient.py
--rw-r--r--   0 root         (0) root         (0)     2701 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/touchclient.py
--rw-r--r--   0 root         (0) root         (0)    45907 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/client/uploadclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.551670 rucio-32.0.0rc1/lib/rucio/common/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/cache.py
--rw-r--r--   0 root         (0) root         (0)    24286 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/config.py
--rw-r--r--   0 root         (0) root         (0)     3314 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/constants.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/constraints.py
--rwxr-xr-x   0 root         (0) root         (0)     6323 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/didtype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.553670 rucio-32.0.0rc1/lib/rucio/common/dumper/
--rw-r--r--   0 root         (0) root         (0)     9183 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/dumper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16097 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/dumper/consistency.py
--rw-r--r--   0 root         (0) root         (0)     9913 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/dumper/data_models.py
--rw-r--r--   0 root         (0) root         (0)     1947 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/dumper/path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    32369 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/exception.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/extra.py
--rw-r--r--   0 root         (0) root         (0)    15070 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/logging.py
--rw-r--r--   0 root         (0) root         (0)    45324 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/pcache.py
--rw-r--r--   0 root         (0) root         (0)     3037 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.556670 rucio-32.0.0rc1/lib/rucio/common/schema/
--rw-r--r--   0 root         (0) root         (0)     5176 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15628 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/schema/atlas.py
--rw-r--r--   0 root         (0) root         (0)    15445 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/schema/belleii.py
--rw-r--r--   0 root         (0) root         (0)    18575 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/schema/cms.py
--rw-r--r--   0 root         (0) root         (0)    15026 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/schema/domatpc.py
--rw-r--r--   0 root         (0) root         (0)    15965 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/schema/escape.py
--rw-r--r--   0 root         (0) root         (0)    16280 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/schema/generic.py
--rw-r--r--   0 root         (0) root         (0)    15507 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/schema/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)    15316 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/schema/icecube.py
--rw-r--r--   0 root         (0) root         (0)    15924 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/schema/lsst.py
--rw-r--r--   0 root         (0) root         (0)     5438 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/stomp_utils.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     4929 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)     3281 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/types.py
--rw-r--r--   0 root         (0) root         (0)    69433 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.571671 rucio-32.0.0rc1/lib/rucio/core/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13710 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/account.py
--rw-r--r--   0 root         (0) root         (0)     6317 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/account_counter.py
--rw-r--r--   0 root         (0) root         (0)    14302 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/account_limit.py
--rw-r--r--   0 root         (0) root         (0)    19593 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/authentication.py
--rw-r--r--   0 root         (0) root         (0)    13304 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/config.py
--rw-r--r--   0 root         (0) root         (0)     8160 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/credential.py
--rw-r--r--   0 root         (0) root         (0)   125139 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/did.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.573671 rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/
--rw-r--r--   0 root         (0) root         (0)    11757 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17627 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/did_column_meta.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py
--rw-r--r--   0 root         (0) root         (0)    29130 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     9283 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/json_meta.py
--rw-r--r--   0 root         (0) root         (0)     7514 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/mongo_meta.py
--rw-r--r--   0 root         (0) root         (0)    13774 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/postgres_meta.py
--rw-r--r--   0 root         (0) root         (0)     9021 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/dirac.py
--rw-r--r--   0 root         (0) root         (0)     5457 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/distance.py
--rw-r--r--   0 root         (0) root         (0)     1803 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/exporter.py
--rw-r--r--   0 root         (0) root         (0)    10364 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    11149 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/identity.py
--rw-r--r--   0 root         (0) root         (0)    13821 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/importer.py
--rw-r--r--   0 root         (0) root         (0)    15257 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/lifetime_exception.py
--rw-r--r--   0 root         (0) root         (0)    22831 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/lock.py
--rw-r--r--   0 root         (0) root         (0)     9728 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/message.py
--rw-r--r--   0 root         (0) root         (0)     7717 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/meta.py
--rw-r--r--   0 root         (0) root         (0)    15825 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/monitor.py
--rw-r--r--   0 root         (0) root         (0)     5447 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/naming_convention.py
--rw-r--r--   0 root         (0) root         (0)     4914 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/nongrid_trace.py
--rw-r--r--   0 root         (0) root         (0)    65207 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/oidc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.575671 rucio-32.0.0rc1/lib/rucio/core/permission/
--rw-r--r--   0 root         (0) root         (0)     3933 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/permission/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54916 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/permission/atlas.py
--rw-r--r--   0 root         (0) root         (0)    46931 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/permission/belleii.py
--rw-r--r--   0 root         (0) root         (0)    46779 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/permission/cms.py
--rw-r--r--   0 root         (0) root         (0)    43126 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/permission/escape.py
--rw-r--r--   0 root         (0) root         (0)    45329 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/permission/generic.py
--rw-r--r--   0 root         (0) root         (0)    45875 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/permission/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     7784 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)   176322 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/replica.py
--rw-r--r--   0 root         (0) root         (0)    15444 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/replica_sorter.py
--rw-r--r--   0 root         (0) root         (0)    88422 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/request.py
--rw-r--r--   0 root         (0) root         (0)    66189 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/rse.py
--rw-r--r--   0 root         (0) root         (0)     5534 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/rse_counter.py
--rw-r--r--   0 root         (0) root         (0)    15401 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)    13958 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/rse_selector.py
--rw-r--r--   0 root         (0) root         (0)   185141 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/rule.py
--rw-r--r--   0 root         (0) root         (0)    92264 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/rule_grouping.py
--rw-r--r--   0 root         (0) root         (0)     5388 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/scope.py
--rw-r--r--   0 root         (0) root         (0)    15508 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/subscription.py
--rw-r--r--   0 root         (0) root         (0)     7467 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/temporary_did.py
--rw-r--r--   0 root         (0) root         (0)    17546 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/topology.py
--rw-r--r--   0 root         (0) root         (0)    13131 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/trace.py
--rw-r--r--   0 root         (0) root         (0)    50925 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/transfer.py
--rw-r--r--   0 root         (0) root         (0)     5531 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/vo.py
--rw-r--r--   0 root         (0) root         (0)     5035 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/core/volatile_replica.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.576671 rucio-32.0.0rc1/lib/rucio/daemons/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.577671 rucio-32.0.0rc1/lib/rucio/daemons/abacus/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/abacus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3760 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/abacus/account.py
--rw-r--r--   0 root         (0) root         (0)     3880 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/abacus/collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3620 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/abacus/rse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.578671 rucio-32.0.0rc1/lib/rucio/daemons/atropos/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/atropos/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10583 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/atropos/atropos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.579671 rucio-32.0.0rc1/lib/rucio/daemons/auditor/
--rw-r--r--   0 root         (0) root         (0)    10105 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/auditor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2920 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/auditor/hdfs.py
--rw-r--r--   0 root         (0) root         (0)     8687 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/auditor/srmdumps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.579671 rucio-32.0.0rc1/lib/rucio/daemons/automatix/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/automatix/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9938 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/automatix/automatix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.580671 rucio-32.0.0rc1/lib/rucio/daemons/badreplicas/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/badreplicas/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15688 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/badreplicas/minos.py
--rw-r--r--   0 root         (0) root         (0)     8552 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py
--rw-r--r--   0 root         (0) root         (0)     9824 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/badreplicas/necromancer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.582671 rucio-32.0.0rc1/lib/rucio/daemons/bb8/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/bb8/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13095 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/bb8/bb8.py
--rw-r--r--   0 root         (0) root         (0)    26621 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/bb8/common.py
--rw-r--r--   0 root         (0) root         (0)     6668 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/bb8/nuclei_background_rebalance.py
--rw-r--r--   0 root         (0) root         (0)     6546 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/bb8/t2_background_rebalance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.582671 rucio-32.0.0rc1/lib/rucio/daemons/c3po/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.584671 rucio-32.0.0rc1/lib/rucio/daemons/c3po/algorithms/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/algorithms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4595 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/algorithms/simple.py
--rw-r--r--   0 root         (0) root         (0)     4675 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/algorithms/t2_free_space.py
--rw-r--r--   0 root         (0) root         (0)     4798 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py
--rw-r--r--   0 root         (0) root         (0)    12175 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py
--rw-r--r--   0 root         (0) root         (0)    15033 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/c3po.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.587672 rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3301 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/agis.py
--rw-r--r--   0 root         (0) root         (0)     2134 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/free_space.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/jedi_did.py
--rw-r--r--   0 root         (0) root         (0)     1370 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/mock_did.py
--rw-r--r--   0 root         (0) root         (0)     2100 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/network_metrics.py
--rw-r--r--   0 root         (0) root         (0)     3858 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/workload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.589672 rucio-32.0.0rc1/lib/rucio/daemons/c3po/utils/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1418 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/utils/dataset_cache.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/utils/expiring_list.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/utils/popularity.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/c3po/utils/timeseries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.589672 rucio-32.0.0rc1/lib/rucio/daemons/cache/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6744 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/cache/consumer.py
--rw-r--r--   0 root         (0) root         (0)    14372 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.592672 rucio-32.0.0rc1/lib/rucio/daemons/conveyor/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/conveyor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25377 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/conveyor/common.py
--rw-r--r--   0 root         (0) root         (0)    23798 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/conveyor/finisher.py
--rw-r--r--   0 root         (0) root         (0)    14004 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/conveyor/poller.py
--rw-r--r--   0 root         (0) root         (0)     7341 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/conveyor/preparer.py
--rw-r--r--   0 root         (0) root         (0)     7576 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/conveyor/receiver.py
--rw-r--r--   0 root         (0) root         (0)     3851 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/conveyor/stager.py
--rw-r--r--   0 root         (0) root         (0)    14987 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/conveyor/submitter.py
--rw-r--r--   0 root         (0) root         (0)    20340 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/conveyor/throttler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.593672 rucio-32.0.0rc1/lib/rucio/daemons/follower/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/follower/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3379 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/follower/follower.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.594672 rucio-32.0.0rc1/lib/rucio/daemons/hermes/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/hermes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26010 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/hermes/hermes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.595672 rucio-32.0.0rc1/lib/rucio/daemons/judge/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/judge/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5649 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/judge/cleaner.py
--rw-r--r--   0 root         (0) root         (0)     6945 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/judge/evaluator.py
--rw-r--r--   0 root         (0) root         (0)     6304 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/judge/injector.py
--rw-r--r--   0 root         (0) root         (0)     5216 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/judge/repairer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.596672 rucio-32.0.0rc1/lib/rucio/daemons/oauthmanager/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/oauthmanager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8735 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/oauthmanager/oauthmanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.597672 rucio-32.0.0rc1/lib/rucio/daemons/reaper/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/reaper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11410 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/reaper/dark_reaper.py
--rw-r--r--   0 root         (0) root         (0)    11869 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/reaper/light_reaper.py
--rw-r--r--   0 root         (0) root         (0)    35938 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/reaper/reaper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.598672 rucio-32.0.0rc1/lib/rucio/daemons/replicarecoverer/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/replicarecoverer/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    27730 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.598672 rucio-32.0.0rc1/lib/rucio/daemons/storage/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.599672 rucio-32.0.0rc1/lib/rucio/daemons/storage/consistency/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/storage/consistency/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29595 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/storage/consistency/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.600672 rucio-32.0.0rc1/lib/rucio/daemons/tracer/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/tracer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23772 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/tracer/kronos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.600672 rucio-32.0.0rc1/lib/rucio/daemons/transmogrifier/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/transmogrifier/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30552 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/transmogrifier/transmogrifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.601672 rucio-32.0.0rc1/lib/rucio/daemons/undertaker/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/undertaker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5080 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/daemons/undertaker/undertaker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.601672 rucio-32.0.0rc1/lib/rucio/db/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.604672 rucio-32.0.0rc1/lib/rucio/db/sqla/
--rw-r--r--   0 root         (0) root         (0)     2154 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3806 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.604672 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3569 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.645674 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/
--rw-r--r--   0 root         (0) root         (0)     3364 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py
--rw-r--r--   0 root         (0) root         (0)     1847 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py
--rw-r--r--   0 root         (0) root         (0)     2690 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     5322 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py
--rw-r--r--   0 root         (0) root         (0)     3684 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py
--rw-r--r--   0 root         (0) root         (0)     1574 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     1339 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py
--rw-r--r--   0 root         (0) root         (0)     8518 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py
--rw-r--r--   0 root         (0) root         (0)     3327 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     3806 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py
--rw-r--r--   0 root         (0) root         (0)     1572 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py
--rw-r--r--   0 root         (0) root         (0)     1716 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py
--rw-r--r--   0 root         (0) root         (0)     4386 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1561 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     2298 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py
--rw-r--r--   0 root         (0) root         (0)     1721 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py
--rw-r--r--   0 root         (0) root         (0)     1812 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py
--rw-r--r--   0 root         (0) root         (0)     2911 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py
--rw-r--r--   0 root         (0) root         (0)     1580 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py
--rw-r--r--   0 root         (0) root         (0)     1793 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py
--rw-r--r--   0 root         (0) root         (0)     1333 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py
--rw-r--r--   0 root         (0) root         (0)     3277 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py
--rw-r--r--   0 root         (0) root         (0)     2044 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py
--rw-r--r--   0 root         (0) root         (0)     3906 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     4022 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     2867 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py
--rw-r--r--   0 root         (0) root         (0)     7553 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py
--rw-r--r--   0 root         (0) root         (0)     2422 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py
--rw-r--r--   0 root         (0) root         (0)     3666 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py
--rw-r--r--   0 root         (0) root         (0)     2711 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py
--rw-r--r--   0 root         (0) root         (0)     1474 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py
--rw-r--r--   0 root         (0) root         (0)     2801 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py
--rw-r--r--   0 root         (0) root         (0)     2474 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py
--rw-r--r--   0 root         (0) root         (0)     1717 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py
--rw-r--r--   0 root         (0) root         (0)     2034 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py
--rw-r--r--   0 root         (0) root         (0)     1297 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py
--rw-r--r--   0 root         (0) root         (0)     2807 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py
--rw-r--r--   0 root         (0) root         (0)     1624 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     1552 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py
--rw-r--r--   0 root         (0) root         (0)     1855 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py
--rw-r--r--   0 root         (0) root         (0)     2387 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     6151 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py
--rw-r--r--   0 root         (0) root         (0)     2316 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py
--rw-r--r--   0 root         (0) root         (0)     1690 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py
--rw-r--r--   0 root         (0) root         (0)     1995 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1585 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py
--rw-r--r--   0 root         (0) root         (0)     1387 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py
--rw-r--r--   0 root         (0) root         (0)     5073 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py
--rw-r--r--   0 root         (0) root         (0)     3592 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py
--rw-r--r--   0 root         (0) root         (0)     1921 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py
--rw-r--r--   0 root         (0) root         (0)     1914 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py
--rw-r--r--   0 root         (0) root         (0)     2171 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py
--rw-r--r--   0 root         (0) root         (0)     3168 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1775 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py
--rw-r--r--   0 root         (0) root         (0)     5062 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py
--rw-r--r--   0 root         (0) root         (0)     1962 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py
--rw-r--r--   0 root         (0) root         (0)     3714 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py
--rw-r--r--   0 root         (0) root         (0)     3167 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py
--rw-r--r--   0 root         (0) root         (0)     1755 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py
--rw-r--r--   0 root         (0) root         (0)     5862 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py
--rw-r--r--   0 root         (0) root         (0)     2619 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     2219 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py
--rw-r--r--   0 root         (0) root         (0)     2223 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py
--rw-r--r--   0 root         (0) root         (0)     2800 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     1907 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1572 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py
--rw-r--r--   0 root         (0) root         (0)     5433 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py
--rw-r--r--   0 root         (0) root         (0)     1375 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py
--rw-r--r--   0 root         (0) root         (0)     7442 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py
--rw-r--r--   0 root         (0) root         (0)     3754 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py
--rw-r--r--   0 root         (0) root         (0)     2145 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py
--rw-r--r--   0 root         (0) root         (0)     1556 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py
--rw-r--r--   0 root         (0) root         (0)     2858 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py
--rw-r--r--   0 root         (0) root         (0)     1771 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     9635 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py
--rw-r--r--   0 root         (0) root         (0)     4791 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1619 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py
--rw-r--r--   0 root         (0) root         (0)     5313 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py
--rw-r--r--   0 root         (0) root         (0)      921 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py
--rw-r--r--   0 root         (0) root         (0)     2971 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py
--rw-r--r--   0 root         (0) root         (0)     1974 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py
--rw-r--r--   0 root         (0) root         (0)     1134 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py
--rw-r--r--   0 root         (0) root         (0)     1920 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py
--rw-r--r--   0 root         (0) root         (0)   113401 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/models.py
--rw-r--r--   0 root         (0) root         (0)     1678 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/sautils.py
--rw-r--r--   0 root         (0) root         (0)    16986 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/session.py
--rw-r--r--   0 root         (0) root         (0)     6112 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/types.py
--rw-r--r--   0 root         (0) root         (0)    21450 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/db/sqla/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.646674 rucio-32.0.0rc1/lib/rucio/rse/
--rw-r--r--   0 root         (0) root         (0)     3327 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.651675 rucio-32.0.0rc1/lib/rucio/rse/protocols/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4627 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/cache.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/dummy.py
--rw-r--r--   0 root         (0) root         (0)    29035 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/gfal.py
--rw-r--r--   0 root         (0) root         (0)     9704 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/globus.py
--rw-r--r--   0 root         (0) root         (0)     3433 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/gsiftp.py
--rw-r--r--   0 root         (0) root         (0)     2999 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/http_cache.py
--rw-r--r--   0 root         (0) root         (0)     4519 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/mock.py
--rw-r--r--   0 root         (0) root         (0)     7248 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/ngarc.py
--rw-r--r--   0 root         (0) root         (0)    10418 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/posix.py
--rw-r--r--   0 root         (0) root         (0)    22818 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/protocol.py
--rw-r--r--   0 root         (0) root         (0)    15276 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/rclone.py
--rw-r--r--   0 root         (0) root         (0)     5554 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/rfio.py
--rw-r--r--   0 root         (0) root         (0)    14671 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/srm.py
--rw-r--r--   0 root         (0) root         (0)    17487 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/ssh.py
--rw-r--r--   0 root         (0) root         (0)     8151 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/storm.py
--rw-r--r--   0 root         (0) root         (0)    22219 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/webdav.py
--rw-r--r--   0 root         (0) root         (0)    12489 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/protocols/xrootd.py
--rw-r--r--   0 root         (0) root         (0)    36928 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/rse/rsemanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.652675 rucio-32.0.0rc1/lib/rucio/tests/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7831 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     5068 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/tests/common_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.654675 rucio-32.0.0rc1/lib/rucio/transfertool/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/transfertool/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68172 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/transfertool/fts3.py
--rw-r--r--   0 root         (0) root         (0)     8109 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/transfertool/globus.py
--rw-r--r--   0 root         (0) root         (0)     8435 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/transfertool/globus_library.py
--rw-r--r--   0 root         (0) root         (0)     1790 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/transfertool/mock.py
--rw-r--r--   0 root         (0) root         (0)     7521 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/transfertool/transfertool.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-07-26 15:02:05.000000 rucio-32.0.0rc1/lib/rucio/vcsversion.py
--rw-r--r--   0 root         (0) root         (0)     1573 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.655675 rucio-32.0.0rc1/lib/rucio/web/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.655675 rucio-32.0.0rc1/lib/rucio/web/rest/
--rwxr-xr-x   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.656675 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/authenticated_bp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.667675 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7826 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/accountlimits.py
--rw-r--r--   0 root         (0) root         (0)    37031 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/accounts.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/archives.py
--rw-r--r--   0 root         (0) root         (0)    61202 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/auth.py
--rw-r--r--   0 root         (0) root         (0)    14540 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/common.py
--rw-r--r--   0 root         (0) root         (0)    10156 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/config.py
--rw-r--r--   0 root         (0) root         (0)     7747 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/credentials.py
--rw-r--r--   0 root         (0) root         (0)    77158 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/dids.py
--rw-r--r--   0 root         (0) root         (0)     4483 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/dirac.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/export.py
--rw-r--r--   0 root         (0) root         (0)     4650 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     7924 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/identities.py
--rw-r--r--   0 root         (0) root         (0)     5281 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/import.py
--rw-r--r--   0 root         (0) root         (0)    12043 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13020 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/locks.py
--rw-r--r--   0 root         (0) root         (0)     2467 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/main.py
--rw-r--r--   0 root         (0) root         (0)     7182 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/meta.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/metrics.py
--rw-r--r--   0 root         (0) root         (0)     3154 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py
--rw-r--r--   0 root         (0) root         (0)     3084 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/ping.py
--rw-r--r--   0 root         (0) root         (0)    13360 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/redirect.py
--rw-r--r--   0 root         (0) root         (0)    72691 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/replicas.py
--rw-r--r--   0 root         (0) root         (0)    35134 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/requests.py
--rw-r--r--   0 root         (0) root         (0)    81935 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/rses.py
--rw-r--r--   0 root         (0) root         (0)    31808 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/rules.py
--rw-r--r--   0 root         (0) root         (0)     5098 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/scopes.py
--rw-r--r--   0 root         (0) root         (0)    24180 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/subscriptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.668676 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/templates/
--rw-r--r--   0 root         (0) root         (0)     2254 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html
--rw-r--r--   0 root         (0) root         (0)     2139 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html
--rw-r--r--   0 root         (0) root         (0)     4087 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/tmp_dids.py
--rw-r--r--   0 root         (0) root         (0)     3236 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/traces.py
--rw-r--r--   0 root         (0) root         (0)     9184 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/vos.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/main.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/lib/rucio/web/rest/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.703677 rucio-32.0.0rc1/lib/rucio.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25183 2023-07-26 15:17:24.000000 rucio-32.0.0rc1/lib/rucio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    16384 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/pylintrc
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5083 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      206 2023-07-26 15:17:24.704677 rucio-32.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2956 2023-07-26 15:17:17.000000 rucio-32.0.0rc1/setup.py
--rw-r--r--   0 root         (0) root         (0)     4749 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/setuputil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.701677 rucio-32.0.0rc1/tests/
--rw-r--r--   0 root         (0) root         (0)     3708 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_abacus_account.py
--rw-r--r--   0 root         (0) root         (0)    10771 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_abacus_collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3255 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_abacus_rse.py
--rw-r--r--   0 root         (0) root         (0)    15997 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_account.py
--rw-r--r--   0 root         (0) root         (0)     9834 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_account_limits.py
--rw-r--r--   0 root         (0) root         (0)    20192 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_api_external_representation.py
--rw-r--r--   0 root         (0) root         (0)    13376 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_archive.py
--rw-r--r--   0 root         (0) root         (0)     4120 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_auditor.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_auditor_hdfs.py
--rw-r--r--   0 root         (0) root         (0)     4225 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_auditor_srmdumps.py
--rw-r--r--   0 root         (0) root         (0)    15239 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_automatix.py
--rw-r--r--   0 root         (0) root         (0)    23339 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_bad_replica.py
--rw-r--r--   0 root         (0) root         (0)    12468 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_bb8.py
--rw-r--r--   0 root         (0) root         (0)     4707 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_belleii.py
--rwxr-xr-x   0 root         (0) root         (0)   107211 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_bin_rucio.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     8248 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_clients.py
--rw-r--r--   0 root         (0) root         (0)     1889 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_common_types.py
--rw-r--r--   0 root         (0) root         (0)     6966 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    85465 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_conveyor.py
--rw-r--r--   0 root         (0) root         (0)    22228 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_conveyor_submitter.py
--rw-r--r--   0 root         (0) root         (0)     6971 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     7703 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_credential.py
--rw-r--r--   0 root         (0) root         (0)     7361 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_curl.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_daemons.py
--rw-r--r--   0 root         (0) root         (0)    28205 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_dataset_replicas.py
--rw-r--r--   0 root         (0) root         (0)     2759 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    55592 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_did.py
--rw-r--r--   0 root         (0) root         (0)    29541 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_did_meta_plugins.py
--rw-r--r--   0 root         (0) root         (0)     4209 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_didtype.py
--rw-r--r--   0 root         (0) root         (0)    35378 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7203 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_dumper.py
--rw-r--r--   0 root         (0) root         (0)    16658 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_dumper_consistency.py
--rw-r--r--   0 root         (0) root         (0)    10907 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_dumper_data_model.py
--rw-r--r--   0 root         (0) root         (0)     3158 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_dumper_path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    38325 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     7977 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    10138 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_hermes.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_identity.py
--rw-r--r--   0 root         (0) root         (0)    18578 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_impl_upload_download.py
--rw-r--r--   0 root         (0) root         (0)    57799 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     5281 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_judge_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    22299 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_judge_evaluator.py
--rw-r--r--   0 root         (0) root         (0)    11070 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_judge_injector.py
--rw-r--r--   0 root         (0) root         (0)    20482 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_judge_repairer.py
--rw-r--r--   0 root         (0) root         (0)    12205 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_lifetime.py
--rw-r--r--   0 root         (0) root         (0)     5879 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     6270 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     1790 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_meta_did.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_module_import.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_monitor.py
--rw-r--r--   0 root         (0) root         (0)    54354 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     2911 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_naming_convention.py
--rw-r--r--   0 root         (0) root         (0)    11606 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_oauthmanager.py
--rw-r--r--   0 root         (0) root         (0)   107576 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_oidc.py
--rw-r--r--   0 root         (0) root         (0)     4529 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     4147 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_pfns.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_ping.py
--rw-r--r--   0 root         (0) root         (0)     7607 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2765 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_qos.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    27057 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_reaper.py
--rw-r--r--   0 root         (0) root         (0)     6464 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)    62407 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_replica.py
--rw-r--r--   0 root         (0) root         (0)    32236 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_replica_recoverer.py
--rw-r--r--   0 root         (0) root         (0)    22852 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_replica_sorting.py
--rw-r--r--   0 root         (0) root         (0)    13879 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)    13074 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_root_proxy.py
--rw-r--r--   0 root         (0) root         (0)    75437 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rse.py
--rw-r--r--   0 root         (0) root         (0)    13230 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)     8966 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rse_lfn2path.py
--rw-r--r--   0 root         (0) root         (0)     4300 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 root         (0) root         (0)     3845 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rse_protocol_gfal2_impl.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rse_protocol_posix.py
--rw-r--r--   0 root         (0) root         (0)     3713 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rse_protocol_rclone.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rse_protocol_rsync.py
--rw-r--r--   0 root         (0) root         (0)     4002 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rse_protocol_srm.py
--rw-r--r--   0 root         (0) root         (0)     4678 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rse_protocol_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 root         (0) root         (0)     3803 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 root         (0) root         (0)     7770 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rse_selector.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)    90900 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)    13873 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_schema_cms.py
--rw-r--r--   0 root         (0) root         (0)     7510 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_scope.py
--rw-r--r--   0 root         (0) root         (0)    48744 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)     2771 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_temporary_did.py
--rw-r--r--   0 root         (0) root         (0)    55640 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_throttler.py
--rw-r--r--   0 root         (0) root         (0)     5045 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_tpc.py
--rw-r--r--   0 root         (0) root         (0)     3204 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_trace.py
--rw-r--r--   0 root         (0) root         (0)    19610 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_transfer.py
--rw-r--r--   0 root         (0) root         (0)     8478 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_undertaker.py
--rw-r--r--   0 root         (0) root         (0)    15673 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     6375 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:17:24.702677 rucio-32.0.0rc1/tools/
--rwxr-xr-x   0 root         (0) root         (0)     1284 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tools/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     6123 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tools/merge_rucio_configs.py
--rwxr-xr-x   0 root         (0) root         (0)     1374 2023-07-26 12:29:16.000000 rucio-32.0.0rc1/tools/reset_database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.218883 rucio-32.0.0rc2/
+-rwxr-xr-x   0 root         (0) root         (0)     4383 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      934 2023-08-03 15:22:48.000000 rucio-32.0.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-08-03 15:22:55.218883 rucio-32.0.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.077882 rucio-32.0.0rc2/bin/
+-rwxr-xr-x   0 root         (0) root         (0)   128576 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/bin/rucio
+-rwxr-xr-x   0 root         (0) root         (0)     2844 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-abacus-account
+-rwxr-xr-x   0 root         (0) root         (0)     1847 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-abacus-collection-replica
+-rwxr-xr-x   0 root         (0) root         (0)     2591 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-abacus-rse
+-rwxr-xr-x   0 root         (0) root         (0)   133738 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/bin/rucio-admin
+-rwxr-xr-x   0 root         (0) root         (0)     3209 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-atropos
+-rwxr-xr-x   0 root         (0) root         (0)     5873 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/bin/rucio-auditor
+-rwxr-xr-x   0 root         (0) root         (0)     2033 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-automatix
+-rwxr-xr-x   0 root         (0) root         (0)     3127 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-bb8
+-rwxr-xr-x   0 root         (0) root         (0)     6124 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-c3po
+-rwxr-xr-x   0 root         (0) root         (0)     5087 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/bin/rucio-cache-client
+-rwxr-xr-x   0 root         (0) root         (0)     1386 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-cache-consumer
+-rwxr-xr-x   0 root         (0) root         (0)     2370 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-conveyor-finisher
+-rwxr-xr-x   0 root         (0) root         (0)     2863 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-conveyor-poller
+-rwxr-xr-x   0 root         (0) root         (0)     1783 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/bin/rucio-conveyor-preparer
+-rwxr-xr-x   0 root         (0) root         (0)     1706 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/bin/rucio-conveyor-receiver
+-rwxr-xr-x   0 root         (0) root         (0)     3409 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-conveyor-stager
+-rwxr-xr-x   0 root         (0) root         (0)     6774 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/bin/rucio-conveyor-submitter
+-rwxr-xr-x   0 root         (0) root         (0)     3883 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-conveyor-throttler
+-rwxr-xr-x   0 root         (0) root         (0)     2570 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-dark-reaper
+-rwxr-xr-x   0 root         (0) root         (0)     6493 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/bin/rucio-dumper
+-rwxr-xr-x   0 root         (0) root         (0)     1438 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-follower
+-rwxr-xr-x   0 root         (0) root         (0)     2011 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/bin/rucio-hermes
+-rwxr-xr-x   0 root         (0) root         (0)     4673 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-judge-cleaner
+-rwxr-xr-x   0 root         (0) root         (0)     7494 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-judge-evaluator
+-rwxr-xr-x   0 root         (0) root         (0)     1695 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-judge-injector
+-rwxr-xr-x   0 root         (0) root         (0)     1699 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-judge-repairer
+-rwxr-xr-x   0 root         (0) root         (0)     1806 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-kronos
+-rwxr-xr-x   0 root         (0) root         (0)     2510 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-light-reaper
+-rwxr-xr-x   0 root         (0) root         (0)     2284 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-minos
+-rwxr-xr-x   0 root         (0) root         (0)     2021 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-minos-temporary-expiration
+-rwxr-xr-x   0 root         (0) root         (0)     5649 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-necromancer
+-rwxr-xr-x   0 root         (0) root         (0)     2812 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-oauth-manager
+-rwxr-xr-x   0 root         (0) root         (0)     4094 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-reaper
+-rwxr-xr-x   0 root         (0) root         (0)    19015 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/bin/rucio-replica-recoverer
+-rwxr-xr-x   0 root         (0) root         (0)     3944 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-storage-consistency-actions
+-rwxr-xr-x   0 root         (0) root         (0)     3388 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-transmogrifier
+-rwxr-xr-x   0 root         (0) root         (0)     2744 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/bin/rucio-undertaker
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.080882 rucio-32.0.0rc2/etc/
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/etc/alembic.ini.template
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/etc/alembic_offline.ini.template
+-rw-r--r--   0 root         (0) root         (0)       96 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/etc/globus-config.yml.template
+-rw-r--r--   0 root         (0) root         (0)      807 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/etc/ldap.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.081882 rucio-32.0.0rc2/etc/mail_templates/
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/etc/mail_templates/rule_approval_request.tmpl
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/etc/mail_templates/rule_approved_admin.tmpl
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/etc/mail_templates/rule_approved_user.tmpl
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/etc/mail_templates/rule_denied_admin.tmpl
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/etc/mail_templates/rule_denied_user.tmpl
+-rw-r--r--   0 root         (0) root         (0)      546 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/etc/mail_templates/rule_ok_notification.tmpl
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/etc/rse-accounts.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/etc/rucio.cfg.atlas.client.template
+-rw-r--r--   0 root         (0) root         (0)     8534 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/etc/rucio.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     7477 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/etc/rucio_multi_vo.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.055881 rucio-32.0.0rc2/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.083882 rucio-32.0.0rc2/lib/rucio/
+-rw-r--r--   0 root         (0) root         (0)      684 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      714 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/alembicrevision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.090882 rucio-32.0.0rc2/lib/rucio/api/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9316 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/api/account.py
+-rw-r--r--   0 root         (0) root         (0)    11419 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/api/account_limit.py
+-rw-r--r--   0 root         (0) root         (0)    12914 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/api/authentication.py
+-rw-r--r--   0 root         (0) root         (0)     8678 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/api/config.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/api/credential.py
+-rw-r--r--   0 root         (0) root         (0)    28229 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/api/did.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/api/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/api/exporter.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/api/heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)     6853 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/api/identity.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/api/importer.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/api/lifetime_exception.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/api/lock.py
+-rw-r--r--   0 root         (0) root         (0)     3070 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/api/meta.py
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/api/permission.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/api/quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    21882 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/api/replica.py
+-rw-r--r--   0 root         (0) root         (0)     9627 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/api/request.py
+-rw-r--r--   0 root         (0) root         (0)    23605 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/api/rse.py
+-rw-r--r--   0 root         (0) root         (0)    15962 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/api/rule.py
+-rw-r--r--   0 root         (0) root         (0)     3027 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/api/scope.py
+-rw-r--r--   0 root         (0) root         (0)    10561 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/api/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/api/temporary_did.py
+-rw-r--r--   0 root         (0) root         (0)     4583 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/api/vo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.098882 rucio-32.0.0rc2/lib/rucio/client/
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16412 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/accountclient.py
+-rw-r--r--   0 root         (0) root         (0)     6020 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/accountlimitclient.py
+-rw-r--r--   0 root         (0) root         (0)    47219 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/baseclient.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     4460 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/client/configclient.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/client/credentialclient.py
+-rw-r--r--   0 root         (0) root         (0)    28223 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/didclient.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/diracclient.py
+-rw-r--r--   0 root         (0) root         (0)    86127 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/downloadclient.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/client/exportclient.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/fileclient.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/client/importclient.py
+-rw-r--r--   0 root         (0) root         (0)     2881 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/lifetimeclient.py
+-rw-r--r--   0 root         (0) root         (0)     3973 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/lockclient.py
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/metaclient.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/pingclient.py
+-rw-r--r--   0 root         (0) root         (0)    19343 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/replicaclient.py
+-rw-r--r--   0 root         (0) root         (0)     4256 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/requestclient.py
+-rw-r--r--   0 root         (0) root         (0)    27183 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/rseclient.py
+-rw-r--r--   0 root         (0) root         (0)    12741 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/ruleclient.py
+-rw-r--r--   0 root         (0) root         (0)     3206 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/scopeclient.py
+-rw-r--r--   0 root         (0) root         (0)     7980 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/subscriptionclient.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/touchclient.py
+-rw-r--r--   0 root         (0) root         (0)    45907 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/client/uploadclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.103882 rucio-32.0.0rc2/lib/rucio/common/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/common/cache.py
+-rw-r--r--   0 root         (0) root         (0)    24286 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/common/config.py
+-rw-r--r--   0 root         (0) root         (0)     3314 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/common/constants.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/common/constraints.py
+-rwxr-xr-x   0 root         (0) root         (0)     6323 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/common/didtype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.104882 rucio-32.0.0rc2/lib/rucio/common/dumper/
+-rw-r--r--   0 root         (0) root         (0)     9183 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/common/dumper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16097 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/common/dumper/consistency.py
+-rw-r--r--   0 root         (0) root         (0)     9913 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/common/dumper/data_models.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/common/dumper/path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    32369 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/common/exception.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/common/extra.py
+-rw-r--r--   0 root         (0) root         (0)    15070 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/common/logging.py
+-rw-r--r--   0 root         (0) root         (0)    45324 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/common/pcache.py
+-rw-r--r--   0 root         (0) root         (0)     3037 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/common/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.107882 rucio-32.0.0rc2/lib/rucio/common/schema/
+-rw-r--r--   0 root         (0) root         (0)     5176 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/common/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15628 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/common/schema/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    15445 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/common/schema/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    18575 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/common/schema/cms.py
+-rw-r--r--   0 root         (0) root         (0)    15026 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/common/schema/domatpc.py
+-rw-r--r--   0 root         (0) root         (0)    15965 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/common/schema/escape.py
+-rw-r--r--   0 root         (0) root         (0)    16280 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/common/schema/generic.py
+-rw-r--r--   0 root         (0) root         (0)    15507 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/common/schema/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)    15316 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/common/schema/icecube.py
+-rw-r--r--   0 root         (0) root         (0)    15924 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/common/schema/lsst.py
+-rw-r--r--   0 root         (0) root         (0)     5438 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/common/stomp_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/common/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     4929 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/common/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)     3281 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/common/types.py
+-rw-r--r--   0 root         (0) root         (0)    69433 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.121882 rucio-32.0.0rc2/lib/rucio/core/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13710 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/account.py
+-rw-r--r--   0 root         (0) root         (0)     6317 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/account_counter.py
+-rw-r--r--   0 root         (0) root         (0)    14302 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/core/account_limit.py
+-rw-r--r--   0 root         (0) root         (0)    19593 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/authentication.py
+-rw-r--r--   0 root         (0) root         (0)    13304 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/config.py
+-rw-r--r--   0 root         (0) root         (0)     8160 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/credential.py
+-rw-r--r--   0 root         (0) root         (0)   125163 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/did.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.123882 rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/
+-rw-r--r--   0 root         (0) root         (0)    11757 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17627 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/did_column_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py
+-rw-r--r--   0 root         (0) root         (0)    29130 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     9283 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/json_meta.py
+-rw-r--r--   0 root         (0) root         (0)     7514 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/mongo_meta.py
+-rw-r--r--   0 root         (0) root         (0)    13774 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/postgres_meta.py
+-rw-r--r--   0 root         (0) root         (0)     9021 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     5457 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/distance.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/core/exporter.py
+-rw-r--r--   0 root         (0) root         (0)    10364 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    11149 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/identity.py
+-rw-r--r--   0 root         (0) root         (0)    13821 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/importer.py
+-rw-r--r--   0 root         (0) root         (0)    15257 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/lifetime_exception.py
+-rw-r--r--   0 root         (0) root         (0)    22831 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/lock.py
+-rw-r--r--   0 root         (0) root         (0)     9728 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/message.py
+-rw-r--r--   0 root         (0) root         (0)     7717 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/core/meta.py
+-rw-r--r--   0 root         (0) root         (0)    15825 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     5447 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)     4914 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/nongrid_trace.py
+-rw-r--r--   0 root         (0) root         (0)    65207 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/oidc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.129882 rucio-32.0.0rc2/lib/rucio/core/permission/
+-rw-r--r--   0 root         (0) root         (0)     3933 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/permission/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54916 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/permission/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    46931 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/permission/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    46779 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/permission/cms.py
+-rw-r--r--   0 root         (0) root         (0)    43126 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/permission/escape.py
+-rw-r--r--   0 root         (0) root         (0)    45329 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/permission/generic.py
+-rw-r--r--   0 root         (0) root         (0)    45875 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/permission/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     7784 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)   176598 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/replica.py
+-rw-r--r--   0 root         (0) root         (0)    15444 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/replica_sorter.py
+-rw-r--r--   0 root         (0) root         (0)    88746 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/request.py
+-rw-r--r--   0 root         (0) root         (0)    66189 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/rse.py
+-rw-r--r--   0 root         (0) root         (0)     5534 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/rse_counter.py
+-rw-r--r--   0 root         (0) root         (0)    15401 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)    13958 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/core/rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)   185141 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/rule.py
+-rw-r--r--   0 root         (0) root         (0)    92264 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/rule_grouping.py
+-rw-r--r--   0 root         (0) root         (0)     5388 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/scope.py
+-rw-r--r--   0 root         (0) root         (0)    15508 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/temporary_did.py
+-rw-r--r--   0 root         (0) root         (0)    17546 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/topology.py
+-rw-r--r--   0 root         (0) root         (0)    13131 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/trace.py
+-rw-r--r--   0 root         (0) root         (0)    50925 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/transfer.py
+-rw-r--r--   0 root         (0) root         (0)     5531 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/vo.py
+-rw-r--r--   0 root         (0) root         (0)     5035 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/core/volatile_replica.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.130882 rucio-32.0.0rc2/lib/rucio/daemons/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.131882 rucio-32.0.0rc2/lib/rucio/daemons/abacus/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/abacus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3760 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/abacus/account.py
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/abacus/collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/abacus/rse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.132882 rucio-32.0.0rc2/lib/rucio/daemons/atropos/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/atropos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10583 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/atropos/atropos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.132882 rucio-32.0.0rc2/lib/rucio/daemons/auditor/
+-rw-r--r--   0 root         (0) root         (0)    10105 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/auditor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2920 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/auditor/hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     8687 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/auditor/srmdumps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.133882 rucio-32.0.0rc2/lib/rucio/daemons/automatix/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/automatix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9938 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/automatix/automatix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.134882 rucio-32.0.0rc2/lib/rucio/daemons/badreplicas/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/badreplicas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15688 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/badreplicas/minos.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py
+-rw-r--r--   0 root         (0) root         (0)     9777 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/badreplicas/necromancer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.136882 rucio-32.0.0rc2/lib/rucio/daemons/bb8/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/bb8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13095 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/bb8/bb8.py
+-rw-r--r--   0 root         (0) root         (0)    26621 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/bb8/common.py
+-rw-r--r--   0 root         (0) root         (0)     6668 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/bb8/nuclei_background_rebalance.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/bb8/t2_background_rebalance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.136882 rucio-32.0.0rc2/lib/rucio/daemons/c3po/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.138882 rucio-32.0.0rc2/lib/rucio/daemons/c3po/algorithms/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/algorithms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4595 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/algorithms/simple.py
+-rw-r--r--   0 root         (0) root         (0)     4675 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/algorithms/t2_free_space.py
+-rw-r--r--   0 root         (0) root         (0)     4798 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py
+-rw-r--r--   0 root         (0) root         (0)    12175 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py
+-rw-r--r--   0 root         (0) root         (0)    15033 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/c3po.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.140882 rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3301 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/agis.py
+-rw-r--r--   0 root         (0) root         (0)     2134 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/free_space.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/jedi_did.py
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/mock_did.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/network_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3858 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/workload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.141882 rucio-32.0.0rc2/lib/rucio/daemons/c3po/utils/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/utils/dataset_cache.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/utils/expiring_list.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/utils/popularity.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/c3po/utils/timeseries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.142882 rucio-32.0.0rc2/lib/rucio/daemons/cache/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6744 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/cache/consumer.py
+-rw-r--r--   0 root         (0) root         (0)    14971 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.145882 rucio-32.0.0rc2/lib/rucio/daemons/conveyor/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/conveyor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25377 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/conveyor/common.py
+-rw-r--r--   0 root         (0) root         (0)    23461 2023-08-03 14:15:29.000000 rucio-32.0.0rc2/lib/rucio/daemons/conveyor/finisher.py
+-rw-r--r--   0 root         (0) root         (0)    14782 2023-08-03 14:15:29.000000 rucio-32.0.0rc2/lib/rucio/daemons/conveyor/poller.py
+-rw-r--r--   0 root         (0) root         (0)     7457 2023-08-03 14:15:29.000000 rucio-32.0.0rc2/lib/rucio/daemons/conveyor/preparer.py
+-rw-r--r--   0 root         (0) root         (0)     7576 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/conveyor/receiver.py
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/conveyor/stager.py
+-rw-r--r--   0 root         (0) root         (0)    15103 2023-08-03 14:15:29.000000 rucio-32.0.0rc2/lib/rucio/daemons/conveyor/submitter.py
+-rw-r--r--   0 root         (0) root         (0)    20340 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/conveyor/throttler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.145882 rucio-32.0.0rc2/lib/rucio/daemons/follower/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/follower/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3379 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/follower/follower.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.146882 rucio-32.0.0rc2/lib/rucio/daemons/hermes/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/hermes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26010 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/hermes/hermes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.148882 rucio-32.0.0rc2/lib/rucio/daemons/judge/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/judge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5649 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/judge/cleaner.py
+-rw-r--r--   0 root         (0) root         (0)     6945 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/judge/evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     6304 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/judge/injector.py
+-rw-r--r--   0 root         (0) root         (0)     5216 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/judge/repairer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.148882 rucio-32.0.0rc2/lib/rucio/daemons/oauthmanager/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/oauthmanager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8735 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/oauthmanager/oauthmanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.149882 rucio-32.0.0rc2/lib/rucio/daemons/reaper/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/reaper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11410 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/reaper/dark_reaper.py
+-rw-r--r--   0 root         (0) root         (0)    11869 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/reaper/light_reaper.py
+-rw-r--r--   0 root         (0) root         (0)    35938 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/reaper/reaper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.150882 rucio-32.0.0rc2/lib/rucio/daemons/replicarecoverer/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/replicarecoverer/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    27730 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.150882 rucio-32.0.0rc2/lib/rucio/daemons/storage/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.151882 rucio-32.0.0rc2/lib/rucio/daemons/storage/consistency/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/storage/consistency/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29595 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/storage/consistency/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.152882 rucio-32.0.0rc2/lib/rucio/daemons/tracer/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/tracer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23772 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/tracer/kronos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.152882 rucio-32.0.0rc2/lib/rucio/daemons/transmogrifier/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/transmogrifier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30552 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/transmogrifier/transmogrifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.153882 rucio-32.0.0rc2/lib/rucio/daemons/undertaker/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/daemons/undertaker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5080 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/daemons/undertaker/undertaker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.153882 rucio-32.0.0rc2/lib/rucio/db/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.155882 rucio-32.0.0rc2/lib/rucio/db/sqla/
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3806 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.156882 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3569 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.182882 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/
+-rw-r--r--   0 root         (0) root         (0)     3364 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py
+-rw-r--r--   0 root         (0) root         (0)     3684 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py
+-rw-r--r--   0 root         (0) root         (0)     8518 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py
+-rw-r--r--   0 root         (0) root         (0)     3327 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     3806 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1561 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py
+-rw-r--r--   0 root         (0) root         (0)     1580 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py
+-rw-r--r--   0 root         (0) root         (0)     3906 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     4022 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)     7553 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2422 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py
+-rw-r--r--   0 root         (0) root         (0)     3666 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py
+-rw-r--r--   0 root         (0) root         (0)     2801 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     6151 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py
+-rw-r--r--   0 root         (0) root         (0)     5073 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py
+-rw-r--r--   0 root         (0) root         (0)     3592 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3168 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py
+-rw-r--r--   0 root         (0) root         (0)     5062 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py
+-rw-r--r--   0 root         (0) root         (0)     1962 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py
+-rw-r--r--   0 root         (0) root         (0)     3714 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py
+-rw-r--r--   0 root         (0) root         (0)     3167 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py
+-rw-r--r--   0 root         (0) root         (0)     5862 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     5433 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py
+-rw-r--r--   0 root         (0) root         (0)     1375 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py
+-rw-r--r--   0 root         (0) root         (0)     7442 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py
+-rw-r--r--   0 root         (0) root         (0)     3754 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py
+-rw-r--r--   0 root         (0) root         (0)     2858 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     9635 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py
+-rw-r--r--   0 root         (0) root         (0)     4791 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1619 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py
+-rw-r--r--   0 root         (0) root         (0)     5313 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py
+-rw-r--r--   0 root         (0) root         (0)      921 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py
+-rw-r--r--   0 root         (0) root         (0)   113277 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/models.py
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/sautils.py
+-rw-r--r--   0 root         (0) root         (0)    16986 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/session.py
+-rw-r--r--   0 root         (0) root         (0)     6112 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/types.py
+-rw-r--r--   0 root         (0) root         (0)    21450 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/db/sqla/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.183883 rucio-32.0.0rc2/lib/rucio/rse/
+-rw-r--r--   0 root         (0) root         (0)     3327 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/rse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.186883 rucio-32.0.0rc2/lib/rucio/rse/protocols/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4627 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/dummy.py
+-rw-r--r--   0 root         (0) root         (0)    29035 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/gfal.py
+-rw-r--r--   0 root         (0) root         (0)     9704 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/globus.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/gsiftp.py
+-rw-r--r--   0 root         (0) root         (0)     2999 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/http_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4519 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7248 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/ngarc.py
+-rw-r--r--   0 root         (0) root         (0)    10418 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/posix.py
+-rw-r--r--   0 root         (0) root         (0)    22818 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/protocol.py
+-rw-r--r--   0 root         (0) root         (0)    15276 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/rclone.py
+-rw-r--r--   0 root         (0) root         (0)     5554 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/rfio.py
+-rw-r--r--   0 root         (0) root         (0)    14671 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/srm.py
+-rw-r--r--   0 root         (0) root         (0)    17487 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     8151 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/storm.py
+-rw-r--r--   0 root         (0) root         (0)    22219 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/webdav.py
+-rw-r--r--   0 root         (0) root         (0)    12489 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/rse/protocols/xrootd.py
+-rw-r--r--   0 root         (0) root         (0)    36928 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/rse/rsemanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.187883 rucio-32.0.0rc2/lib/rucio/tests/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7831 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     5068 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/tests/common_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.188882 rucio-32.0.0rc2/lib/rucio/transfertool/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/transfertool/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68172 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/transfertool/fts3.py
+-rw-r--r--   0 root         (0) root         (0)     8109 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/transfertool/globus.py
+-rw-r--r--   0 root         (0) root         (0)     8435 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/transfertool/globus_library.py
+-rw-r--r--   0 root         (0) root         (0)     2956 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/transfertool/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7584 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/transfertool/transfertool.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-08-03 14:15:48.000000 rucio-32.0.0rc2/lib/rucio/vcsversion.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.188882 rucio-32.0.0rc2/lib/rucio/web/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/web/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.189883 rucio-32.0.0rc2/lib/rucio/web/rest/
+-rwxr-xr-x   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/web/rest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.189883 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/authenticated_bp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.196883 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7826 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/accountlimits.py
+-rw-r--r--   0 root         (0) root         (0)    37031 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/accounts.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/archives.py
+-rw-r--r--   0 root         (0) root         (0)    61286 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/auth.py
+-rw-r--r--   0 root         (0) root         (0)    14540 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/common.py
+-rw-r--r--   0 root         (0) root         (0)    10156 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/config.py
+-rw-r--r--   0 root         (0) root         (0)     7747 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/credentials.py
+-rw-r--r--   0 root         (0) root         (0)    77158 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/dids.py
+-rw-r--r--   0 root         (0) root         (0)     4483 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/export.py
+-rw-r--r--   0 root         (0) root         (0)     4650 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     7924 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/identities.py
+-rw-r--r--   0 root         (0) root         (0)     5281 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/import.py
+-rw-r--r--   0 root         (0) root         (0)    12043 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13020 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/locks.py
+-rw-r--r--   0 root         (0) root         (0)     2467 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/main.py
+-rw-r--r--   0 root         (0) root         (0)     7182 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/meta.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3154 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/ping.py
+-rw-r--r--   0 root         (0) root         (0)    13360 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/redirect.py
+-rw-r--r--   0 root         (0) root         (0)    72691 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/replicas.py
+-rw-r--r--   0 root         (0) root         (0)    35134 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/requests.py
+-rw-r--r--   0 root         (0) root         (0)    81935 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/rses.py
+-rw-r--r--   0 root         (0) root         (0)    31808 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/rules.py
+-rw-r--r--   0 root         (0) root         (0)     5098 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/scopes.py
+-rw-r--r--   0 root         (0) root         (0)    24180 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.196883 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/templates/
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html
+-rw-r--r--   0 root         (0) root         (0)     4087 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/tmp_dids.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/traces.py
+-rw-r--r--   0 root         (0) root         (0)     9184 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/vos.py
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/lib/rucio/web/rest/main.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/lib/rucio/web/rest/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.218883 rucio-32.0.0rc2/lib/rucio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25279 2023-08-03 15:22:55.000000 rucio-32.0.0rc2/lib/rucio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    16384 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/pylintrc
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5083 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2023-08-03 15:22:55.219883 rucio-32.0.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2956 2023-08-03 15:22:48.000000 rucio-32.0.0rc2/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4749 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/setuputil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.217883 rucio-32.0.0rc2/tests/
+-rw-r--r--   0 root         (0) root         (0)     3708 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_abacus_account.py
+-rw-r--r--   0 root         (0) root         (0)    10771 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_abacus_collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3255 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_abacus_rse.py
+-rw-r--r--   0 root         (0) root         (0)    15997 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_account.py
+-rw-r--r--   0 root         (0) root         (0)     9834 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_account_limits.py
+-rw-r--r--   0 root         (0) root         (0)    20192 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_api_external_representation.py
+-rw-r--r--   0 root         (0) root         (0)    13376 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4120 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_auditor.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_auditor_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 root         (0) root         (0)    15239 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_automatix.py
+-rw-r--r--   0 root         (0) root         (0)    23339 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_bad_replica.py
+-rw-r--r--   0 root         (0) root         (0)    12468 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_bb8.py
+-rw-r--r--   0 root         (0) root         (0)     4707 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_belleii.py
+-rwxr-xr-x   0 root         (0) root         (0)   107211 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_bin_rucio.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     8248 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_common_types.py
+-rw-r--r--   0 root         (0) root         (0)     6966 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    84744 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_conveyor.py
+-rw-r--r--   0 root         (0) root         (0)    22228 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_conveyor_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     6971 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     7703 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7361 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_curl.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_daemons.py
+-rw-r--r--   0 root         (0) root         (0)    28205 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_dataset_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    55592 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_did.py
+-rw-r--r--   0 root         (0) root         (0)    29541 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_did_meta_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     4209 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_didtype.py
+-rw-r--r--   0 root         (0) root         (0)    35378 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7203 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_dumper.py
+-rw-r--r--   0 root         (0) root         (0)    16658 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_dumper_consistency.py
+-rw-r--r--   0 root         (0) root         (0)    10907 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_dumper_data_model.py
+-rw-r--r--   0 root         (0) root         (0)     3158 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    38325 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     7977 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    10138 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_hermes.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)    18578 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_impl_upload_download.py
+-rw-r--r--   0 root         (0) root         (0)    57799 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     5281 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_judge_cleaner.py
+-rw-r--r--   0 root         (0) root         (0)    22299 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_judge_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11070 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_judge_injector.py
+-rw-r--r--   0 root         (0) root         (0)    20482 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_judge_repairer.py
+-rw-r--r--   0 root         (0) root         (0)    12205 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_lifetime.py
+-rw-r--r--   0 root         (0) root         (0)     5879 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     6270 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_meta_did.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_module_import.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    54354 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)    11606 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_oauthmanager.py
+-rw-r--r--   0 root         (0) root         (0)   107576 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     4529 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4147 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_pfns.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_ping.py
+-rw-r--r--   0 root         (0) root         (0)     7607 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_qos.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    27057 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_reaper.py
+-rw-r--r--   0 root         (0) root         (0)     6464 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    62407 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_replica.py
+-rw-r--r--   0 root         (0) root         (0)    32236 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_replica_recoverer.py
+-rw-r--r--   0 root         (0) root         (0)    22852 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_replica_sorting.py
+-rw-r--r--   0 root         (0) root         (0)    13879 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)    13074 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_root_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    75437 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rse.py
+-rw-r--r--   0 root         (0) root         (0)    13230 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)     8966 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rse_lfn2path.py
+-rw-r--r--   0 root         (0) root         (0)     4300 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rse_protocol_gfal2_impl.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rse_protocol_rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rse_protocol_rsync.py
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 root         (0) root         (0)     4678 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rse_protocol_ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 root         (0) root         (0)     7770 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)    90900 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)    13873 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_schema_cms.py
+-rw-r--r--   0 root         (0) root         (0)     7510 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_scope.py
+-rw-r--r--   0 root         (0) root         (0)    48744 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     2771 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_temporary_did.py
+-rw-r--r--   0 root         (0) root         (0)    55640 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_throttler.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_tpc.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)    19610 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     8478 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_undertaker.py
+-rw-r--r--   0 root         (0) root         (0)    15673 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     6375 2023-08-03 09:00:39.000000 rucio-32.0.0rc2/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:22:55.218883 rucio-32.0.0rc2/tools/
+-rwxr-xr-x   0 root         (0) root         (0)     1284 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/tools/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-08-03 09:00:33.000000 rucio-32.0.0rc2/tools/merge_rucio_configs.py
+-rwxr-xr-x   0 root         (0) root         (0)     1374 2023-07-27 12:40:37.000000 rucio-32.0.0rc2/tools/reset_database.py
```

### Comparing `rucio-32.0.0rc1/AUTHORS.rst` & `rucio-32.0.0rc2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/LICENSE` & `rucio-32.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/MANIFEST.in` & `rucio-32.0.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/PKG-INFO` & `rucio-32.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio
-Version: 32.0.0rc1
+Version: 32.0.0rc2
 Summary: Rucio Package
 Home-page: https://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rucio-32.0.0rc1/README.rst` & `rucio-32.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio` & `rucio-32.0.0rc2/bin/rucio`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-abacus-account` & `rucio-32.0.0rc2/bin/rucio-abacus-account`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-abacus-collection-replica` & `rucio-32.0.0rc2/bin/rucio-abacus-collection-replica`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-abacus-rse` & `rucio-32.0.0rc2/bin/rucio-abacus-rse`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-admin` & `rucio-32.0.0rc2/bin/rucio-admin`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-atropos` & `rucio-32.0.0rc2/bin/rucio-atropos`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-auditor` & `rucio-32.0.0rc2/bin/rucio-auditor`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-automatix` & `rucio-32.0.0rc2/bin/rucio-automatix`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-bb8` & `rucio-32.0.0rc2/bin/rucio-bb8`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-c3po` & `rucio-32.0.0rc2/bin/rucio-c3po`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-cache-client` & `rucio-32.0.0rc2/bin/rucio-cache-client`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-cache-consumer` & `rucio-32.0.0rc2/bin/rucio-cache-consumer`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-conveyor-finisher` & `rucio-32.0.0rc2/bin/rucio-conveyor-finisher`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-conveyor-poller` & `rucio-32.0.0rc2/bin/rucio-conveyor-poller`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-conveyor-preparer` & `rucio-32.0.0rc2/bin/rucio-conveyor-preparer`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-conveyor-receiver` & `rucio-32.0.0rc2/bin/rucio-conveyor-receiver`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-conveyor-stager` & `rucio-32.0.0rc2/bin/rucio-conveyor-stager`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-conveyor-submitter` & `rucio-32.0.0rc2/bin/rucio-conveyor-submitter`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-conveyor-throttler` & `rucio-32.0.0rc2/bin/rucio-conveyor-throttler`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-dark-reaper` & `rucio-32.0.0rc2/bin/rucio-dark-reaper`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-dumper` & `rucio-32.0.0rc2/bin/rucio-dumper`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-follower` & `rucio-32.0.0rc2/bin/rucio-follower`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-hermes` & `rucio-32.0.0rc2/bin/rucio-hermes`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-judge-cleaner` & `rucio-32.0.0rc2/bin/rucio-judge-cleaner`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-judge-evaluator` & `rucio-32.0.0rc2/bin/rucio-judge-evaluator`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-judge-injector` & `rucio-32.0.0rc2/bin/rucio-judge-injector`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-judge-repairer` & `rucio-32.0.0rc2/bin/rucio-judge-repairer`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-kronos` & `rucio-32.0.0rc2/bin/rucio-kronos`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-light-reaper` & `rucio-32.0.0rc2/bin/rucio-light-reaper`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-minos` & `rucio-32.0.0rc2/bin/rucio-minos`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-minos-temporary-expiration` & `rucio-32.0.0rc2/bin/rucio-minos-temporary-expiration`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-necromancer` & `rucio-32.0.0rc2/bin/rucio-necromancer`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-oauth-manager` & `rucio-32.0.0rc2/bin/rucio-oauth-manager`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-reaper` & `rucio-32.0.0rc2/bin/rucio-reaper`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-replica-recoverer` & `rucio-32.0.0rc2/bin/rucio-replica-recoverer`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-storage-consistency-actions` & `rucio-32.0.0rc2/bin/rucio-storage-consistency-actions`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-transmogrifier` & `rucio-32.0.0rc2/bin/rucio-transmogrifier`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/bin/rucio-undertaker` & `rucio-32.0.0rc2/bin/rucio-undertaker`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/etc/alembic.ini.template` & `rucio-32.0.0rc2/etc/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/etc/alembic_offline.ini.template` & `rucio-32.0.0rc2/etc/alembic_offline.ini.template`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/etc/ldap.cfg.template` & `rucio-32.0.0rc2/etc/ldap.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/etc/mail_templates/rule_approval_request.tmpl` & `rucio-32.0.0rc2/etc/mail_templates/rule_approval_request.tmpl`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/etc/mail_templates/rule_ok_notification.tmpl` & `rucio-32.0.0rc2/etc/mail_templates/rule_ok_notification.tmpl`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/etc/rse-accounts.cfg.template` & `rucio-32.0.0rc2/etc/rse-accounts.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/etc/rucio.cfg.atlas.client.template` & `rucio-32.0.0rc2/etc/rucio.cfg.atlas.client.template`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/etc/rucio.cfg.template` & `rucio-32.0.0rc2/etc/rucio.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/etc/rucio_multi_vo.cfg.template` & `rucio-32.0.0rc2/etc/rucio_multi_vo.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/__init__.py` & `rucio-32.0.0rc2/lib/rucio/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/alembicrevision.py` & `rucio-32.0.0rc2/lib/rucio/alembicrevision.py`

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

### Comparing `rucio-32.0.0rc1/lib/rucio/api/__init__.py` & `rucio-32.0.0rc2/lib/rucio/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/account.py` & `rucio-32.0.0rc2/lib/rucio/api/account.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/account_limit.py` & `rucio-32.0.0rc2/lib/rucio/api/account_limit.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/authentication.py` & `rucio-32.0.0rc2/lib/rucio/api/authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/config.py` & `rucio-32.0.0rc2/lib/rucio/api/config.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/credential.py` & `rucio-32.0.0rc2/lib/rucio/api/credential.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/did.py` & `rucio-32.0.0rc2/lib/rucio/api/did.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/dirac.py` & `rucio-32.0.0rc2/lib/rucio/api/dirac.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/exporter.py` & `rucio-32.0.0rc2/lib/rucio/api/exporter.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/heartbeat.py` & `rucio-32.0.0rc2/lib/rucio/api/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/identity.py` & `rucio-32.0.0rc2/lib/rucio/api/identity.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/importer.py` & `rucio-32.0.0rc2/lib/rucio/api/importer.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/lifetime_exception.py` & `rucio-32.0.0rc2/lib/rucio/api/lifetime_exception.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/lock.py` & `rucio-32.0.0rc2/lib/rucio/api/lock.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/meta.py` & `rucio-32.0.0rc2/lib/rucio/api/meta.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/permission.py` & `rucio-32.0.0rc2/lib/rucio/api/permission.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/quarantined_replica.py` & `rucio-32.0.0rc2/lib/rucio/api/quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/replica.py` & `rucio-32.0.0rc2/lib/rucio/api/replica.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/request.py` & `rucio-32.0.0rc2/lib/rucio/api/request.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/rse.py` & `rucio-32.0.0rc2/lib/rucio/api/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/rule.py` & `rucio-32.0.0rc2/lib/rucio/api/rule.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/scope.py` & `rucio-32.0.0rc2/lib/rucio/api/scope.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/subscription.py` & `rucio-32.0.0rc2/lib/rucio/api/subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/temporary_did.py` & `rucio-32.0.0rc2/lib/rucio/api/temporary_did.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/api/vo.py` & `rucio-32.0.0rc2/lib/rucio/api/vo.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/__init__.py` & `rucio-32.0.0rc2/lib/rucio/client/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/accountclient.py` & `rucio-32.0.0rc2/lib/rucio/client/accountclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/accountlimitclient.py` & `rucio-32.0.0rc2/lib/rucio/client/accountlimitclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/baseclient.py` & `rucio-32.0.0rc2/lib/rucio/client/baseclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/client.py` & `rucio-32.0.0rc2/lib/rucio/client/client.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/configclient.py` & `rucio-32.0.0rc2/lib/rucio/client/configclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/credentialclient.py` & `rucio-32.0.0rc2/lib/rucio/client/credentialclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/didclient.py` & `rucio-32.0.0rc2/lib/rucio/client/didclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/diracclient.py` & `rucio-32.0.0rc2/lib/rucio/client/diracclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/downloadclient.py` & `rucio-32.0.0rc2/lib/rucio/client/downloadclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/exportclient.py` & `rucio-32.0.0rc2/lib/rucio/client/exportclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/fileclient.py` & `rucio-32.0.0rc2/lib/rucio/client/fileclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/importclient.py` & `rucio-32.0.0rc2/lib/rucio/client/importclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/lifetimeclient.py` & `rucio-32.0.0rc2/lib/rucio/client/lifetimeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/lockclient.py` & `rucio-32.0.0rc2/lib/rucio/client/lockclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/metaclient.py` & `rucio-32.0.0rc2/lib/rucio/client/metaclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/pingclient.py` & `rucio-32.0.0rc2/lib/rucio/client/pingclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/replicaclient.py` & `rucio-32.0.0rc2/lib/rucio/client/replicaclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/requestclient.py` & `rucio-32.0.0rc2/lib/rucio/client/requestclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/rseclient.py` & `rucio-32.0.0rc2/lib/rucio/client/rseclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/ruleclient.py` & `rucio-32.0.0rc2/lib/rucio/client/ruleclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/scopeclient.py` & `rucio-32.0.0rc2/lib/rucio/client/scopeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/subscriptionclient.py` & `rucio-32.0.0rc2/lib/rucio/client/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/touchclient.py` & `rucio-32.0.0rc2/lib/rucio/client/touchclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/client/uploadclient.py` & `rucio-32.0.0rc2/lib/rucio/client/uploadclient.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/__init__.py` & `rucio-32.0.0rc2/lib/rucio/common/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/cache.py` & `rucio-32.0.0rc2/lib/rucio/common/cache.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/config.py` & `rucio-32.0.0rc2/lib/rucio/common/config.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/constants.py` & `rucio-32.0.0rc2/lib/rucio/common/constants.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/constraints.py` & `rucio-32.0.0rc2/lib/rucio/common/constraints.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/didtype.py` & `rucio-32.0.0rc2/lib/rucio/common/didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/dumper/__init__.py` & `rucio-32.0.0rc2/lib/rucio/common/dumper/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/dumper/consistency.py` & `rucio-32.0.0rc2/lib/rucio/common/dumper/consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/dumper/data_models.py` & `rucio-32.0.0rc2/lib/rucio/common/dumper/data_models.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/dumper/path_parsing.py` & `rucio-32.0.0rc2/lib/rucio/common/dumper/path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/exception.py` & `rucio-32.0.0rc2/lib/rucio/common/exception.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/extra.py` & `rucio-32.0.0rc2/lib/rucio/common/extra.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/logging.py` & `rucio-32.0.0rc2/lib/rucio/common/logging.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/pcache.py` & `rucio-32.0.0rc2/lib/rucio/common/pcache.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/policy.py` & `rucio-32.0.0rc2/lib/rucio/common/policy.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/schema/__init__.py` & `rucio-32.0.0rc2/lib/rucio/common/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/schema/atlas.py` & `rucio-32.0.0rc2/lib/rucio/common/schema/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/schema/belleii.py` & `rucio-32.0.0rc2/lib/rucio/common/schema/belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/schema/cms.py` & `rucio-32.0.0rc2/lib/rucio/common/schema/cms.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/schema/domatpc.py` & `rucio-32.0.0rc2/lib/rucio/common/schema/domatpc.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/schema/escape.py` & `rucio-32.0.0rc2/lib/rucio/common/schema/escape.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/schema/generic.py` & `rucio-32.0.0rc2/lib/rucio/common/schema/generic.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/schema/generic_multi_vo.py` & `rucio-32.0.0rc2/lib/rucio/common/schema/generic_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/schema/icecube.py` & `rucio-32.0.0rc2/lib/rucio/common/schema/icecube.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/schema/lsst.py` & `rucio-32.0.0rc2/lib/rucio/common/schema/lsst.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/stomp_utils.py` & `rucio-32.0.0rc2/lib/rucio/common/stomp_utils.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/stopwatch.py` & `rucio-32.0.0rc2/lib/rucio/common/stopwatch.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/test_rucio_server.py` & `rucio-32.0.0rc2/lib/rucio/common/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/types.py` & `rucio-32.0.0rc2/lib/rucio/common/types.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/common/utils.py` & `rucio-32.0.0rc2/lib/rucio/common/utils.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/__init__.py` & `rucio-32.0.0rc2/lib/rucio/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/account.py` & `rucio-32.0.0rc2/lib/rucio/core/account.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/account_counter.py` & `rucio-32.0.0rc2/lib/rucio/core/account_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/account_limit.py` & `rucio-32.0.0rc2/lib/rucio/core/account_limit.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/authentication.py` & `rucio-32.0.0rc2/lib/rucio/core/authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/config.py` & `rucio-32.0.0rc2/lib/rucio/core/config.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/credential.py` & `rucio-32.0.0rc2/lib/rucio/core/credential.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/did.py` & `rucio-32.0.0rc2/lib/rucio/core/did.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,16 @@
             raise exception.DataIdentifierNotFound("Data identifier '%s:%s' not found" % (attachment['scope'], attachment['name']))
         first_iteration = False
 
     # Remove all duplicated dictionnaries from the list
     # (convert the list of dictionaries into a list of tuple, then to a set of tuple
     # to remove duplicates, then back to a list of unique dictionaries)
     parent_dids = [dict(tup) for tup in set(tuple(dictionary.items()) for dictionary in parent_dids)]
-    session.execute(insert(models.UpdatedDID), parent_dids)
+    if parent_dids:
+        session.execute(insert(models.UpdatedDID), parent_dids)
 
 
 def __add_files_to_archive(parent_did, files_temp_table, files, account, ignore_duplicate=False, *, session: "Session"):
     """
     Add files to archive.
 
     :param parent_did: the DataIdentifier object of the parent did
```

### Comparing `rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/__init__.py` & `rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/did_column_meta.py` & `rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/did_column_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py` & `rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/filter_engine.py` & `rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/json_meta.py` & `rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/json_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/mongo_meta.py` & `rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/mongo_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/did_meta_plugins/postgres_meta.py` & `rucio-32.0.0rc2/lib/rucio/core/did_meta_plugins/postgres_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/dirac.py` & `rucio-32.0.0rc2/lib/rucio/core/dirac.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/distance.py` & `rucio-32.0.0rc2/lib/rucio/core/distance.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/exporter.py` & `rucio-32.0.0rc2/lib/rucio/core/exporter.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/heartbeat.py` & `rucio-32.0.0rc2/lib/rucio/core/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/identity.py` & `rucio-32.0.0rc2/lib/rucio/core/identity.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/importer.py` & `rucio-32.0.0rc2/lib/rucio/core/importer.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/lifetime_exception.py` & `rucio-32.0.0rc2/lib/rucio/core/lifetime_exception.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/lock.py` & `rucio-32.0.0rc2/lib/rucio/core/lock.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/message.py` & `rucio-32.0.0rc2/lib/rucio/core/message.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/meta.py` & `rucio-32.0.0rc2/lib/rucio/core/meta.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/monitor.py` & `rucio-32.0.0rc2/lib/rucio/core/monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/naming_convention.py` & `rucio-32.0.0rc2/lib/rucio/core/naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/nongrid_trace.py` & `rucio-32.0.0rc2/lib/rucio/core/nongrid_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/oidc.py` & `rucio-32.0.0rc2/lib/rucio/core/oidc.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/permission/__init__.py` & `rucio-32.0.0rc2/lib/rucio/core/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/permission/atlas.py` & `rucio-32.0.0rc2/lib/rucio/core/permission/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/permission/belleii.py` & `rucio-32.0.0rc2/lib/rucio/core/permission/belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/permission/cms.py` & `rucio-32.0.0rc2/lib/rucio/core/permission/cms.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/permission/escape.py` & `rucio-32.0.0rc2/lib/rucio/core/permission/escape.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/permission/generic.py` & `rucio-32.0.0rc2/lib/rucio/core/permission/generic.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/permission/generic_multi_vo.py` & `rucio-32.0.0rc2/lib/rucio/core/permission/generic_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/quarantined_replica.py` & `rucio-32.0.0rc2/lib/rucio/core/quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/replica.py` & `rucio-32.0.0rc2/lib/rucio/core/replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,14 +517,15 @@
     Get the replica backlog by RSE.
 
     :param session:            The database session in use.
 
     :returns: a list of dictionary {'rse_id': cnt_bad_replicas}.
     """
     query = session.query(func.count(models.RSEFileAssociation.rse_id), models.RSEFileAssociation.rse_id). \
+        with_hint(models.RSEFileAssociation, 'INDEX(DIDS DIDS_PK) USE_NL(DIDS) INDEX_RS_ASC(REPLICAS ("REPLICAS"."STATE"))', 'oracle'). \
         filter(models.RSEFileAssociation.state == ReplicaState.BAD)
 
     query = query.join(models.DataIdentifier,
                        and_(models.DataIdentifier.scope == models.RSEFileAssociation.scope,
                             models.DataIdentifier.name == models.RSEFileAssociation.name)).\
         filter(models.DataIdentifier.availability != DIDAvailability.LOST).\
         group_by(models.RSEFileAssociation.rse_id)
@@ -547,14 +548,15 @@
 
     :returns: a list of dictionary {'scope' scope, 'name': name, 'rse_id': rse_id, 'rse': rse}.
     """
     schema_dot = '%s.' % DEFAULT_SCHEMA_NAME if DEFAULT_SCHEMA_NAME else ''
     query = session.query(models.RSEFileAssociation.scope,
                           models.RSEFileAssociation.name,
                           models.RSEFileAssociation.rse_id). \
+        with_hint(models.RSEFileAssociation, 'INDEX(DIDS DIDS_PK) USE_NL(DIDS) INDEX_RS_ASC(REPLICAS ("REPLICAS"."STATE"))', 'oracle'). \
         filter(models.RSEFileAssociation.state == ReplicaState.BAD)
 
     query = filter_thread_work(session=session, query=query, total_threads=total_threads, thread_id=thread, hash_variable='%sreplicas.name' % (schema_dot))
     query = query.join(models.DataIdentifier,
                        and_(models.DataIdentifier.scope == models.RSEFileAssociation.scope,
                             models.DataIdentifier.name == models.RSEFileAssociation.name)).\
         filter(models.DataIdentifier.availability != DIDAvailability.LOST)
```

### Comparing `rucio-32.0.0rc1/lib/rucio/core/replica_sorter.py` & `rucio-32.0.0rc2/lib/rucio/core/replica_sorter.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/request.py` & `rucio-32.0.0rc2/lib/rucio/core/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -434,15 +434,15 @@
     )
 
     if processed_by:
         sub_requests = sub_requests.where(
             or_(
                 models.Request.last_processed_by.is_(null()),
                 models.Request.last_processed_by != processed_by,
-                models.Request.last_processed_at > datetime.datetime.utcnow() - datetime.timedelta(seconds=processed_at_delay)
+                models.Request.last_processed_at < datetime.datetime.utcnow() - datetime.timedelta(seconds=processed_at_delay)
             )
         )
 
     if not ignore_availability:
         sub_requests = sub_requests.where(models.RSE.availability_write == true())
 
     if isinstance(older_than, datetime.datetime):
@@ -556,25 +556,29 @@
             replica_rse.name = replica_rse_name
             source = RequestSource(rse_data=replica_rse, file_path=file_path,
                                    ranking=source_ranking, distance=distance, url=source_url)
             request.sources.append(source)
             if source_rse_id == replica_rse_id:
                 request.requested_source = source
 
-    if processed_by and requests_by_id:
-        now = datetime.datetime.utcnow()
-        updates = [
-            {
-                models.Request.id.name: request_id,
-                models.Request.last_processed_by.name: processed_by,
-                models.Request.last_processed_at.name: now,
-            }
-            for request_id in requests_by_id
-        ]
-        session.execute(update(models.Request), updates)
+    if processed_by:
+        for chunk in chunks(requests_by_id, 100):
+            stmt = update(
+                models.Request
+            ).where(
+                models.Request.id.in_(chunk)
+            ).execution_options(
+                synchronize_session=False
+            ).values(
+                {
+                    models.Request.last_processed_by: processed_by,
+                    models.Request.last_processed_at: datetime.datetime.now(),
+                }
+            )
+            session.execute(stmt)
 
     return requests_by_id
 
 
 @read_session
 def fetch_paths(request_id, *, session: "Session"):
     """
@@ -682,15 +686,15 @@
             asc(models.Request.updated_at)
         )
         if processed_by:
             query = query.where(
                 or_(
                     models.Request.last_processed_by.is_(null()),
                     models.Request.last_processed_by != processed_by,
-                    models.Request.last_processed_at > datetime.datetime.utcnow() - datetime.timedelta(seconds=processed_at_delay)
+                    models.Request.last_processed_at < datetime.datetime.utcnow() - datetime.timedelta(seconds=processed_at_delay)
                 )
             )
         if transfertool:
             query = query.with_hint(
                 models.Request, "INDEX(REQUESTS REQUESTS_TYP_STA_TRA_ACT_IDX)", 'oracle'
             ).where(
                 models.Request.transfertool == transfertool
@@ -744,25 +748,30 @@
                     res_dict['source_rse'] = get_rse_name(rse_id=src_id, session=session) if src_id is not None else None
 
                     result.append(res_dict)
             else:
                 for res in query_result:
                     result.append({'request_id': res.id, 'external_host': res.external_host, 'external_id': res.external_id})
 
-            if processed_by:
-                now = datetime.datetime.utcnow()
-                updates = [
-                    {
-                        models.Request.id.name: res_dict['request_id'],
-                        models.Request.last_processed_by.name: processed_by,
-                        models.Request.last_processed_at.name: now,
-                    }
-                    for res_dict in result
-                ]
-                session.execute(update(models.Request), updates)
+            request_ids = {r['request_id'] for r in result}
+            if processed_by and request_ids:
+                for chunk in chunks(request_ids, 100):
+                    stmt = update(
+                        models.Request
+                    ).where(
+                        models.Request.id.in_(chunk)
+                    ).execution_options(
+                        synchronize_session=False
+                    ).values(
+                        {
+                            models.Request.last_processed_by: processed_by,
+                            models.Request.last_processed_at: datetime.datetime.now(),
+                        }
+                    )
+                    session.execute(stmt)
 
     return result
 
 
 @transactional_session
 def update_request(
         request_id: str,
```

### Comparing `rucio-32.0.0rc1/lib/rucio/core/rse.py` & `rucio-32.0.0rc2/lib/rucio/core/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/rse_counter.py` & `rucio-32.0.0rc2/lib/rucio/core/rse_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/rse_expression_parser.py` & `rucio-32.0.0rc2/lib/rucio/core/rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/rse_selector.py` & `rucio-32.0.0rc2/lib/rucio/core/rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/rule.py` & `rucio-32.0.0rc2/lib/rucio/core/rule.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/rule_grouping.py` & `rucio-32.0.0rc2/lib/rucio/core/rule_grouping.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/scope.py` & `rucio-32.0.0rc2/lib/rucio/core/scope.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/subscription.py` & `rucio-32.0.0rc2/lib/rucio/core/subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/temporary_did.py` & `rucio-32.0.0rc2/lib/rucio/core/temporary_did.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/topology.py` & `rucio-32.0.0rc2/lib/rucio/core/topology.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/trace.py` & `rucio-32.0.0rc2/lib/rucio/core/trace.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/transfer.py` & `rucio-32.0.0rc2/lib/rucio/core/transfer.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/vo.py` & `rucio-32.0.0rc2/lib/rucio/core/vo.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/core/volatile_replica.py` & `rucio-32.0.0rc2/lib/rucio/core/volatile_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/abacus/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/abacus/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/abacus/account.py` & `rucio-32.0.0rc2/lib/rucio/daemons/abacus/account.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/abacus/collection_replica.py` & `rucio-32.0.0rc2/lib/rucio/daemons/abacus/collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/abacus/rse.py` & `rucio-32.0.0rc2/lib/rucio/daemons/abacus/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/atropos/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/atropos/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/atropos/atropos.py` & `rucio-32.0.0rc2/lib/rucio/daemons/atropos/atropos.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/auditor/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/auditor/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/auditor/hdfs.py` & `rucio-32.0.0rc2/lib/rucio/daemons/auditor/hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/auditor/srmdumps.py` & `rucio-32.0.0rc2/lib/rucio/daemons/auditor/srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/automatix/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/automatix/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/automatix/automatix.py` & `rucio-32.0.0rc2/lib/rucio/daemons/automatix/automatix.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/badreplicas/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/badreplicas/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/badreplicas/minos.py` & `rucio-32.0.0rc2/lib/rucio/daemons/badreplicas/minos.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py` & `rucio-32.0.0rc2/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/badreplicas/necromancer.py` & `rucio-32.0.0rc2/lib/rucio/daemons/badreplicas/necromancer.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,14 @@
             bulk=bulk,
         ),
     )
 
 
 def run_once(heartbeat_handler: "HeartbeatHandler", bulk: int, **_kwargs) -> bool:
     worker_number, total_workers, logger = heartbeat_handler.live()
-    logger(logging.INFO, 'Graceful stop done')
     must_sleep = True
 
     # Check if there is a Judge Evaluator backlog
     max_evaluator_backlog_count = config_get_int('necromancer', 'max_evaluator_backlog_count', default=0, raise_exception=False)
     max_evaluator_backlog_duration = config_get_int('necromancer', 'max_evaluator_backlog_duration', default=0, raise_exception=False)
     backlog_refresh_time = config_get_int('necromancer', 'backlog_refresh_time', default=60, raise_exception=False)
     if max_evaluator_backlog_count or max_evaluator_backlog_duration:
```

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/bb8/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/bb8/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/bb8/bb8.py` & `rucio-32.0.0rc2/lib/rucio/daemons/bb8/bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/bb8/common.py` & `rucio-32.0.0rc2/lib/rucio/daemons/bb8/common.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/bb8/nuclei_background_rebalance.py` & `rucio-32.0.0rc2/lib/rucio/daemons/bb8/nuclei_background_rebalance.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/bb8/t2_background_rebalance.py` & `rucio-32.0.0rc2/lib/rucio/daemons/bb8/t2_background_rebalance.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/algorithms/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/algorithms/simple.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/algorithms/simple.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/algorithms/t2_free_space.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/algorithms/t2_free_space.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/c3po.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/c3po.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/agis.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/agis.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/free_space.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/free_space.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/jedi_did.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/jedi_did.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/mock_did.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/mock_did.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/network_metrics.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/network_metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/collectors/workload.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/collectors/workload.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/utils/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/utils/dataset_cache.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/utils/dataset_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/utils/expiring_list.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/utils/expiring_list.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/utils/popularity.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/utils/popularity.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/c3po/utils/timeseries.py` & `rucio-32.0.0rc2/lib/rucio/daemons/c3po/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/cache/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/cache/consumer.py` & `rucio-32.0.0rc2/lib/rucio/daemons/cache/consumer.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/common.py` & `rucio-32.0.0rc2/lib/rucio/daemons/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import functools
 import logging
 import os
 import queue
 import socket
 import threading
 import time
-from collections.abc import Callable, Generator, Iterator
+from collections.abc import Callable, Generator, Iterator, Sequence
 from typing import Any, Generic, Optional, TypeVar, Union
 
 from rucio.common.logging import formatted_logger
 from rucio.common.utils import PriorityQueue
 from rucio.core import heartbeat as heartbeat_core
 from rucio.core.monitor import MetricManager
 
@@ -105,16 +105,16 @@
 
         return self.last_heart_beat['assign_thread'], self.last_heart_beat['nr_threads'], self.logger
 
 
 def _activity_looper(
         once: bool,
         sleep_time: int,
-        activities: Optional[list[str]],
-        logger,
+        activities: Optional[Sequence[str]],
+        heartbeat_handler: HeartbeatHandler,
 ) -> Generator[tuple[str, float], tuple[float, bool], None]:
     """
     Generator which loops (either once, or indefinitely) over all activities while ensuring that `sleep_time`
     passes between handling twice the same activity.
 
     Returns an activity and how much time the calling context must sleep before handling that activity
     and expects to get in return the time when the activity started to be executed and whether next
@@ -136,14 +136,15 @@
 
         if once:
             time_to_sleep = 0
             activity_next_exe_time.pop()
         else:
             time_to_sleep = desired_exe_time - time.time()
 
+        logger = heartbeat_handler.logger
         if time_to_sleep > 0:
             if activity:
                 logger(logging.DEBUG, 'Switching to activity %s and sleeping %s seconds', activity, time_to_sleep)
             else:
                 logger(logging.DEBUG, 'Sleeping %s seconds', time_to_sleep)
         else:
             if activity:
@@ -165,15 +166,15 @@
 
 def db_workqueue(
         once: bool,
         graceful_stop: threading.Event,
         executable: str,
         partition_wait_time: int,
         sleep_time: int,
-        activities: Optional[list[str]] = None,
+        activities: Optional[Sequence[str]] = None,
 ):
     """
     Used to wrap a function for interacting with the database as a work queue: i.e. to select
     a set of rows and perform some work on those rows while ensuring that two instances running in parallel don't
     work on the same set of rows. The last condition is ensured by using heartbeats to keep track of currently
     active workers.
 
@@ -194,15 +195,15 @@
                 logger = heartbeat_handler.logger
                 logger(logging.INFO, 'started')
 
                 if partition_wait_time:
                     graceful_stop.wait(partition_wait_time)
                     _, _, logger = heartbeat_handler.live(force_renew=True)
 
-                activity_loop = _activity_looper(once=once, sleep_time=sleep_time, activities=activities, logger=logger)
+                activity_loop = _activity_looper(once=once, sleep_time=sleep_time, activities=activities, heartbeat_handler=heartbeat_handler)
                 activity, time_to_sleep = next(activity_loop, (None, None))
                 while time_to_sleep is not None:
                     if graceful_stop.is_set():
                         break
 
                     if time_to_sleep > 0:
                         graceful_stop.wait(time_to_sleep)
@@ -272,23 +273,24 @@
 
 
 class ProducerConsumerDaemon(Generic[T]):
     """
     Daemon which connects N producers with M consumers via a queue.
     """
 
-    def __init__(self, producers, consumers, graceful_stop):
+    def __init__(self, producers, consumers, graceful_stop, logger=logging.log):
         self.producers = producers
         self.consumers = consumers
 
         self.queue = queue.Queue()
         self.lock = threading.Lock()
         self.graceful_stop = graceful_stop
         self.active_producers = 0
         self.producers_done_event = threading.Event()
+        self.logger = logger
 
     def _produce(
             self,
             it: Callable[[], Iterator[T]],
             wait_for_consumers: bool = False
     ):
         """
@@ -304,18 +306,20 @@
             while not self.graceful_stop.is_set():
                 if self.queue.qsize() > len(self.consumers):
                     self.graceful_stop.wait(1)
                     continue
 
                 try:
                     product = next(i)
+                    self.queue.put(product)
                 except StopIteration:
                     break
-
-                self.queue.put(product)
+                except Exception as e:
+                    METRICS.counter('exceptions.{exception}').labels(exception=e.__class__.__name__).inc()
+                    self.logger(logging.CRITICAL, "Exception", exc_info=True)
         finally:
             with self.lock:
                 self.active_producers -= 1
                 if not self.active_producers > 0:
                     self.producers_done_event.set()
 
             if wait_for_consumers:
@@ -335,14 +339,17 @@
                 product = self.queue.get_nowait()
             except queue.Empty:
                 self.producers_done_event.wait(1)
                 continue
 
             try:
                 fnc(product)
+            except Exception as e:
+                METRICS.counter('exceptions.{exception}').labels(exception=e.__class__.__name__).inc()
+                self.logger(logging.CRITICAL, "Exception", exc_info=True)
             finally:
                 self.queue.task_done()
 
     def run(self):
 
         producer_threads = []
         for i, producer in enumerate(self.producers):
```

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/conveyor/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/conveyor/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/conveyor/common.py` & `rucio-32.0.0rc2/lib/rucio/daemons/conveyor/common.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/conveyor/finisher.py` & `rucio-32.0.0rc2/lib/rucio/daemons/conveyor/finisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 
 """
 Conveyor finisher is a daemon to update replicas and rules based on requests.
 """
 
 import datetime
+import functools
 import logging
 import os
 import re
 import threading
 from types import FrameType
 from typing import TYPE_CHECKING, Optional
 from urllib.parse import urlparse
@@ -49,45 +50,54 @@
     from rucio.daemons.common import HeartbeatHandler
 
 GRACEFUL_STOP = threading.Event()
 
 REGION = make_region_memcached(expiration_time=900)
 METRICS = MetricManager(module=__name__)
 DAEMON_NAME = 'conveyor-finisher'
+FAILED_DURING_SUBMISSION_DELAY = datetime.timedelta(minutes=120)
 
 
 def _fetch_requests(
         db_bulk,
+        set_last_processed_by: bool,
         heartbeat_handler,
-        activity
+        activity,
 ):
     worker_number, total_workers, logger = heartbeat_handler.live()
 
     logger(logging.DEBUG, 'Working on activity %s', activity)
 
-    reqs = request_core.get_and_mark_next(
+    get_requests_fnc = functools.partial(
+        request_core.get_and_mark_next,
         request_type=[RequestType.TRANSFER, RequestType.STAGEIN, RequestType.STAGEOUT],
+        processed_by=heartbeat_handler.short_executable if set_last_processed_by else None,
+        limit=db_bulk,
+        total_workers=total_workers,
+        worker_number=worker_number,
+        mode_all=True,
+        include_dependent=False,
+        hash_variable='rule_id',
+    )
+    reqs = get_requests_fnc(
         state=[
             RequestState.DONE,
             RequestState.FAILED,
             RequestState.LOST,
-            RequestState.SUBMITTING,
             RequestState.SUBMISSION_FAILED,
             RequestState.NO_SOURCES,
             RequestState.ONLY_TAPE_SOURCES,
             RequestState.MISMATCH_SCHEME
         ],
-        processed_by=heartbeat_handler.short_executable,
-        limit=db_bulk,
-        older_than=datetime.datetime.utcnow(),
-        total_workers=total_workers,
-        worker_number=worker_number,
-        mode_all=True,
-        include_dependent=False,
-        hash_variable='rule_id',
+    )
+    reqs.extend(
+        get_requests_fnc(
+            state=[RequestState.SUBMITTING],
+            older_than=datetime.datetime.utcnow() - FAILED_DURING_SUBMISSION_DELAY
+        )
     )
 
     must_sleep = False
     if len(reqs) < db_bulk / 2:
         logger(logging.INFO, "Only %s transfers, which is less than half of the bulk %s", len(reqs), db_bulk)
         must_sleep = True
     return must_sleep, reqs
@@ -159,14 +169,15 @@
         sleep_time=sleep_time,
         activities=activities,
     )
     def _db_producer(*, activity: str, heartbeat_handler: "HeartbeatHandler"):
         return _fetch_requests(
             db_bulk=db_bulk,
             activity=activity,
+            set_last_processed_by=not once,
             heartbeat_handler=heartbeat_handler,
         )
 
     def _consumer(reqs):
         return _handle_requests(
             reqs=reqs,
             bulk=bulk,
@@ -194,33 +205,22 @@
     Starts up the conveyer threads.
     """
     setup_logging(process_name=DAEMON_NAME)
 
     if rucio.db.sqla.util.is_old_db():
         raise DatabaseException('Database was not updated, daemon won\'t start')
 
-    if once:
-        logging.log(logging.INFO, 'executing one finisher iteration only')
-        finisher(once=once, activities=activities, bulk=bulk, db_bulk=db_bulk)
-
-    else:
-
-        logging.log(logging.INFO, 'starting finisher threads')
-        threads = [threading.Thread(target=finisher, kwargs={'sleep_time': sleep_time,
-                                                             'activities': activities,
-                                                             'db_bulk': db_bulk,
-                                                             'bulk': bulk}) for _ in range(0, total_threads)]
-
-        [thread.start() for thread in threads]
-
-        logging.log(logging.INFO, 'waiting for interrupts')
-
-        # Interruptible joins require a timeout.
-        while threads:
-            threads = [thread.join(timeout=3.14) for thread in threads if thread and thread.is_alive()]
+    finisher(
+        once=once,
+        activities=activities,
+        bulk=bulk,
+        db_bulk=db_bulk,
+        sleep_time=sleep_time,
+        total_threads=total_threads
+    )
 
 
 def _finish_requests(reqs, suspicious_patterns, retry_protocol_mismatches, logger=logging.log):
     """
     Used by finisher to handle terminated requests,
 
     :param reqs:                         List of requests.
@@ -286,15 +286,15 @@
                         replica['error_message'] = req['err_msg'] if req['err_msg'] else request_core.get_transfer_error(req['state'])
                         replicas[req['request_type']][req['rule_id']].append(replica)
                 except RequestNotFound:
                     logger(logging.WARNING, 'Cannot find request %s anymore', req['request_id'])
 
             # All other failures
             elif req['state'] in failed_during_submission or req['state'] in failed_no_submission_attempts:
-                if req['state'] in failed_during_submission and req['updated_at'] > (datetime.datetime.utcnow() - datetime.timedelta(minutes=120)):
+                if req['state'] in failed_during_submission and req['updated_at'] > (datetime.datetime.utcnow() - FAILED_DURING_SUBMISSION_DELAY):
                     # To prevent race conditions
                     continue
                 try:
                     if request_core.should_retry_request(req, retry_protocol_mismatches):
                         new_req = request_core.requeue_and_archive(req, source_ranking_update=False, retry_protocol_mismatches=retry_protocol_mismatches, logger=logger)
                         logger(logging.WARNING, 'REQUEUED SUBMITTING DID %s:%s REQUEST %s AS %s TRY %s' % (req['scope'],
                                                                                                            req['name'],
```

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/conveyor/poller.py` & `rucio-32.0.0rc2/lib/rucio/daemons/conveyor/poller.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import json
 import logging
 import re
 import threading
 import time
 from itertools import groupby
 from types import FrameType
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Mapping, Optional, Sequence
 
 from requests.exceptions import RequestException
 from sqlalchemy.exc import DatabaseError
 
 import rucio.db.sqla.util
 from rucio.common.config import config_get, config_get_bool
 from rucio.common.exception import DatabaseException, TransferToolTimeout, TransferToolWrongAnswer
@@ -40,14 +40,15 @@
 from rucio.common.utils import dict_chunks
 from rucio.core import transfer as transfer_core, request as request_core
 from rucio.core.monitor import MetricManager
 from rucio.daemons.common import db_workqueue, ProducerConsumerDaemon
 from rucio.db.sqla.constants import RequestState, RequestType
 from rucio.transfertool.fts3 import FTS3Transfertool
 from rucio.transfertool.globus import GlobusTransferTool
+from rucio.transfertool.mock import MockTransfertool
 
 if TYPE_CHECKING:
     from rucio.daemons.common import HeartbeatHandler
 
 GRACEFUL_STOP = threading.Event()
 METRICS = MetricManager(module=__name__)
 DAEMON_NAME = 'conveyor-poller'
@@ -56,38 +57,39 @@
 FILTER_TRANSFERTOOL = config_get('conveyor', 'filter_transfertool', False, None)  # NOTE: TRANSFERTOOL to filter requests on
 
 
 def _fetch_requests(
         db_bulk,
         older_than,
         activity_shares,
+        transfertool,
+        filter_transfertool,
         activity,
         heartbeat_handler
 ):
     worker_number, total_workers, logger = heartbeat_handler.live()
 
-    logger(logging.DEBUG, 'Start to poll transfers older than %i seconds for activity %s using transfer tool: %s' % (older_than, activity, FILTER_TRANSFERTOOL))
+    logger(logging.DEBUG, 'Start to poll transfers older than %i seconds for activity %s using transfer tool: %s' % (older_than, activity, filter_transfertool))
     transfs = request_core.get_and_mark_next(
         request_type=[RequestType.TRANSFER, RequestType.STAGEIN, RequestType.STAGEOUT],
         state=[RequestState.SUBMITTED],
-        processed_by=heartbeat_handler.short_executable,
         limit=db_bulk,
         older_than=datetime.datetime.utcnow() - datetime.timedelta(seconds=older_than) if older_than else None,
         total_workers=total_workers,
         worker_number=worker_number,
         mode_all=True,
         hash_variable='id',
         activity=activity,
         activity_shares=activity_shares,
-        transfertool=FILTER_TRANSFERTOOL,
+        transfertool=filter_transfertool,
     )
 
-    if TRANSFER_TOOL and not FILTER_TRANSFERTOOL:
+    if transfertool and not filter_transfertool:
         # only keep transfers which don't have any transfertool set, or have one equal to TRANSFER_TOOL
-        transfs_tmp = [t for t in transfs if not t['transfertool'] or t['transfertool'] == TRANSFER_TOOL]
+        transfs_tmp = [t for t in transfs if not t['transfertool'] or t['transfertool'] == transfertool]
         if len(transfs_tmp) != len(transfs):
             logger(logging.INFO, 'Skipping %i transfers because of missmatched transfertool', len(transfs) - len(transfs_tmp))
         transfs = transfs_tmp
 
     if transfs:
         logger(logging.DEBUG, 'Polling %i transfers for activity %s' % (len(transfs), activity))
 
@@ -100,14 +102,15 @@
 
 
 def _handle_requests(
         transfs,
         fts_bulk,
         multi_vo,
         timeout,
+        transfertool,
         oidc_account: Optional[str],
         *,
         logger=logging.log,
 ):
     transfs.sort(key=lambda t: (t['external_host'] or '',
                                 t['scope'].vo if multi_vo else '',
                                 t['external_id'] or '',
@@ -116,39 +119,43 @@
                                                                                    t['scope'].vo if multi_vo else None)):
         transfers_by_eid = {}
         for external_id, xfers in groupby(transfers_for_host, key=lambda t: t['external_id']):
             transfers_by_eid[external_id] = {t['request_id']: t for t in xfers}
 
         for chunk in dict_chunks(transfers_by_eid, fts_bulk):
             try:
-                if TRANSFER_TOOL == 'globus':
-                    transfertool_obj = GlobusTransferTool(external_host=None)
+                if transfertool == 'mock':
+                    transfertool_obj = MockTransfertool(external_host=MockTransfertool.external_name)
+                elif transfertool == 'globus':
+                    transfertool_obj = GlobusTransferTool(external_host=GlobusTransferTool.external_name)
                 else:
                     account = None
                     if oidc_account:
                         if vo:
                             account = InternalAccount(oidc_account, vo=vo)
                         else:
                             account = InternalAccount(oidc_account)
                     transfertool_obj = FTS3Transfertool(external_host=external_host, vo=vo, oidc_account=account)
                 poll_transfers(transfertool_obj=transfertool_obj, transfers_by_eid=chunk, timeout=timeout, logger=logger)
             except Exception:
                 logger(logging.ERROR, 'Exception', exc_info=True)
 
 
 def poller(
-        once=False,
-        activities=None,
-        sleep_time=60,
-        fts_bulk=100,
-        db_bulk=1000,
-        older_than=60,
-        activity_shares=None,
-        partition_wait_time=10,
-        total_threads=1
+        once: bool = False,
+        activities: Optional[Sequence[str]] = None,
+        sleep_time: int = 60,
+        fts_bulk: int = 100,
+        db_bulk: int = 1000,
+        older_than: int = 60,
+        activity_shares: Optional[Mapping[str, float]] = None,
+        partition_wait_time: int = 10,
+        transfertool: Optional[str] = TRANSFER_TOOL,
+        filter_transfertool: Optional[str] = FILTER_TRANSFERTOOL,
+        total_threads: int = 1,
 ):
     """
     Main loop to check the status of a transfer primitive with a transfertool.
     """
 
     timeout = config_get('conveyor', 'poll_timeout', default=None, raise_exception=False)
     if timeout:
@@ -156,46 +163,48 @@
 
     multi_vo = config_get_bool('common', 'multi_vo', False, None)
     oidc_account = config_get('conveyor', 'poller_oidc_account', False, None)
 
     executable = DAEMON_NAME
 
     if activities:
-        activities.sort()
+        activities = sorted(activities)
         executable += '--activities ' + str(activities)
     if activity_shares:
-        activities.sort()
-        executable += '--activity_shares' + str(activity_shares)
-    if FILTER_TRANSFERTOOL:
-        executable += ' --filter-transfertool ' + FILTER_TRANSFERTOOL
+        executable += '--activity_shares' + str(sorted(activity_shares))
+    if filter_transfertool:
+        executable += ' --filter-transfertool ' + filter_transfertool
 
     @db_workqueue(
         once=once,
         graceful_stop=GRACEFUL_STOP,
         executable=executable,
         partition_wait_time=partition_wait_time,
         sleep_time=sleep_time,
         activities=activities,
     )
     def _db_producer(*, activity: str, heartbeat_handler: "HeartbeatHandler"):
         return _fetch_requests(
             db_bulk=db_bulk,
             older_than=older_than,
             activity_shares=activity_shares,
+            transfertool=transfertool,
+            filter_transfertool=filter_transfertool,
             activity=activity,
             heartbeat_handler=heartbeat_handler,
         )
 
     def _consumer(transfs):
         return _handle_requests(
             transfs=transfs,
             fts_bulk=fts_bulk,
             multi_vo=multi_vo,
             timeout=timeout,
             oidc_account=oidc_account,
+            transfertool=transfertool,
         )
 
     ProducerConsumerDaemon(
         producers=[_db_producer],
         consumers=[_consumer for _ in range(total_threads)],
         graceful_stop=GRACEFUL_STOP,
     ).run()
@@ -212,52 +221,53 @@
 def run(
         once=False,
         sleep_time=60,
         activities=None,
         fts_bulk=100,
         db_bulk=1000,
         older_than=60,
-        activity_shares=None,
+        activity_shares: Optional[str] = None,
         total_threads=1
 ):
     """
     Starts up the conveyer threads.
     """
     setup_logging(process_name=DAEMON_NAME)
 
     if rucio.db.sqla.util.is_old_db():
         raise DatabaseException('Database was not updated, daemon won\'t start')
 
+    parsed_activity_shares = None
     if activity_shares:
 
         try:
-            activity_shares = json.loads(activity_shares)
+            parsed_activity_shares = {str(activity): float(share) for activity, share in json.loads(activity_shares).items()}
         except Exception:
             logging.critical('activity share is not a valid JSON dictionary')
             return
 
         try:
-            if round(sum(activity_shares.values()), 2) != 1:
-                logging.critical('activity shares do not sum up to 1, got %s - aborting' % round(sum(activity_shares.values()), 2))
+            if round(sum(parsed_activity_shares.values()), 2) != 1:
+                logging.critical('activity shares do not sum up to 1, got %s - aborting' % round(sum(parsed_activity_shares.values()), 2))
                 return
         except Exception:
             logging.critical('activity shares are not numbers? - aborting')
             return
 
-        activity_shares.update((share, int(percentage * db_bulk)) for share, percentage in activity_shares.items())
-        logging.info('activity shares enabled: %s' % activity_shares)
+        parsed_activity_shares.update((share, int(percentage * db_bulk)) for share, percentage in parsed_activity_shares.items())
+        logging.info('activity shares enabled: %s' % parsed_activity_shares)
 
     poller(
         once=once,
         fts_bulk=fts_bulk,
         db_bulk=db_bulk,
         older_than=older_than,
         sleep_time=sleep_time,
         activities=activities,
-        activity_shares=activity_shares,
+        activity_shares=parsed_activity_shares,
         total_threads=total_threads,
     )
 
 
 def poll_transfers(transfertool_obj, transfers_by_eid, timeout=None, logger=logging.log):
     """
     Poll a list of transfers from an FTS server
```

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/conveyor/preparer.py` & `rucio-32.0.0rc2/lib/rucio/daemons/conveyor/preparer.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,15 @@
         sleep_time=sleep_time)
     def _db_producer(*, activity: str, heartbeat_handler: "HeartbeatHandler"):
         return _fetch_requests(
             bulk=bulk,
             ignore_availability=ignore_availability,
             cached_topology=cached_topology,
             heartbeat_handler=heartbeat_handler,
+            set_last_processed_by=not once,
         )
 
     def _consumer(batch):
         return _handle_requests(
             batch,
             transfertools=transfertools,
             bulk=bulk,
@@ -118,23 +119,24 @@
 
 
 def _fetch_requests(
         bulk: int,
         ignore_availability: bool,
         cached_topology,
         heartbeat_handler: "HeartbeatHandler",
+        set_last_processed_by: bool,
         *,
         session: "Optional[Session]" = None,
 ):
     worker_number, total_workers, logger = heartbeat_handler.live()
     topology = cached_topology.get() if cached_topology else Topology(ignore_availability=ignore_availability)
     topology.configure_multihop(logger=logger, session=session)
     requests_with_sources = list_and_mark_transfer_requests_and_source_replicas(
         rse_collection=topology,
-        processed_by=heartbeat_handler.short_executable,
+        processed_by=heartbeat_handler.short_executable if set_last_processed_by else None,
         total_workers=total_workers,
         worker_number=worker_number,
         limit=bulk,
         request_state=RequestState.PREPARING,
         request_type=[RequestType.TRANSFER, RequestType.STAGEIN],
         ignore_availability=ignore_availability,
         session=session,
```

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/conveyor/receiver.py` & `rucio-32.0.0rc2/lib/rucio/daemons/conveyor/receiver.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/conveyor/stager.py` & `rucio-32.0.0rc2/lib/rucio/daemons/conveyor/stager.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/conveyor/submitter.py` & `rucio-32.0.0rc2/lib/rucio/daemons/conveyor/submitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         activity: str,
         rse_ids: Optional[list[str]],
         request_type: list[RequestType],
         ignore_availability: bool,
         filter_transfertool: Optional[str],
         metrics: MetricManager,
         cached_topology,
+        set_last_processed_by: bool,
         heartbeat_handler: "HeartbeatHandler",
 ):
     """
     Fetches requests to be handled from the database
     """
     worker_number, total_workers, logger = heartbeat_handler.live()
 
@@ -78,15 +79,15 @@
         # if multihop is configured, we want all possible source rses. To allow multi-hopping between transfertools
         if not topology.multihop_enabled:
             required_source_rse_attrs = TRANSFERTOOL_CLASSES_BY_NAME[filter_transfertool].required_rse_attrs
 
     # retrieve (from the database) the transfer requests with their possible source replicas
     requests_with_sources = list_and_mark_transfer_requests_and_source_replicas(
         rse_collection=topology,
-        processed_by=heartbeat_handler.short_executable,
+        processed_by=heartbeat_handler.short_executable if set_last_processed_by else None,
         total_workers=total_workers,
         worker_number=worker_number,
         partition_hash_var=partition_hash_var,
         limit=bulk,
         activity=activity,
         older_than=None,
         rses=rse_ids,
@@ -268,14 +269,15 @@
             ignore_availability=ignore_availability,
             partition_hash_var=partition_hash_var,
             rse_ids=rse_ids,
             request_type=request_type,
             metrics=metrics,
             activity=activity,
             cached_topology=cached_topology,
+            set_last_processed_by=not once,
             heartbeat_handler=heartbeat_handler,
         )
 
     def _consumer(batch):
         return _handle_requests(
             batch,
             transfertools=transfertools,
```

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/conveyor/throttler.py` & `rucio-32.0.0rc2/lib/rucio/daemons/conveyor/throttler.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/follower/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/follower/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/follower/follower.py` & `rucio-32.0.0rc2/lib/rucio/daemons/follower/follower.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/hermes/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/hermes/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/hermes/hermes.py` & `rucio-32.0.0rc2/lib/rucio/daemons/hermes/hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/judge/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/judge/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/judge/cleaner.py` & `rucio-32.0.0rc2/lib/rucio/daemons/judge/cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/judge/evaluator.py` & `rucio-32.0.0rc2/lib/rucio/daemons/judge/evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/judge/injector.py` & `rucio-32.0.0rc2/lib/rucio/daemons/judge/injector.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/judge/repairer.py` & `rucio-32.0.0rc2/lib/rucio/daemons/judge/repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/oauthmanager/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/oauthmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/oauthmanager/oauthmanager.py` & `rucio-32.0.0rc2/lib/rucio/daemons/oauthmanager/oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/reaper/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/reaper/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/reaper/dark_reaper.py` & `rucio-32.0.0rc2/lib/rucio/daemons/reaper/dark_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/reaper/light_reaper.py` & `rucio-32.0.0rc2/lib/rucio/daemons/reaper/light_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/reaper/reaper.py` & `rucio-32.0.0rc2/lib/rucio/daemons/reaper/reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/replicarecoverer/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/replicarecoverer/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py` & `rucio-32.0.0rc2/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/storage/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/storage/consistency/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/storage/consistency/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/storage/consistency/actions.py` & `rucio-32.0.0rc2/lib/rucio/daemons/storage/consistency/actions.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/tracer/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/tracer/kronos.py` & `rucio-32.0.0rc2/lib/rucio/daemons/tracer/kronos.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/transmogrifier/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/transmogrifier/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/transmogrifier/transmogrifier.py` & `rucio-32.0.0rc2/lib/rucio/daemons/transmogrifier/transmogrifier.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/undertaker/__init__.py` & `rucio-32.0.0rc2/lib/rucio/daemons/undertaker/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/daemons/undertaker/undertaker.py` & `rucio-32.0.0rc2/lib/rucio/daemons/undertaker/undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/__init__.py` & `rucio-32.0.0rc2/lib/rucio/db/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/__init__.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/constants.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/constants.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/__init__.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/env.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/env.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/models.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -948,18 +948,16 @@
     tombstone: Mapped[Optional[datetime]] = mapped_column(DateTime)
     _table_args = (PrimaryKeyConstraint('scope', 'name', 'rse_id', name='REPLICAS_PK'),
                    ForeignKeyConstraint(['scope', 'name'], ['dids.scope', 'dids.name'], name='REPLICAS_LFN_FK'),
                    ForeignKeyConstraint(['rse_id'], ['rses.id'], name='REPLICAS_RSE_ID_FK'),
                    CheckConstraint('STATE IS NOT NULL', name='REPLICAS_STATE_NN'),
                    CheckConstraint('bytes IS NOT NULL', name='REPLICAS_SIZE_NN'),
                    CheckConstraint('lock_cnt IS NOT NULL', name='REPLICAS_LOCK_CNT_NN'),
-                   Index('REPLICAS_TOMBSTONE_IDX', 'tombstone'),
                    Index('REPLICAS_PATH_IDX', 'path', mysql_length=get_schema_value('NAME_LENGTH')),
                    Index('REPLICAS_STATE_IDX', 'state'),
-                   Index('REPLICAS_RSE_ID_IDX', 'rse_id'),
                    Index('REPLICAS_RSE_ID_TOMBSTONE_IDX', 'rse_id', 'tombstone'))
 
 
 class CollectionReplica(BASE, ModelBase):
     """Represents replicas for datasets/collections"""
     __tablename__ = 'collection_replicas'
     scope: Mapped[InternalScope] = mapped_column(InternalScopeString(get_schema_value('SCOPE_LENGTH')))
```

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/sautils.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/sautils.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/session.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/session.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/types.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/types.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/db/sqla/util.py` & `rucio-32.0.0rc2/lib/rucio/db/sqla/util.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/__init__.py` & `rucio-32.0.0rc2/lib/rucio/rse/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/__init__.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/cache.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/cache.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/dummy.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/dummy.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/gfal.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/gfal.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/globus.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/globus.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/gsiftp.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/gsiftp.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/http_cache.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/http_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/mock.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/mock.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/ngarc.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/ngarc.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/posix.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/posix.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/protocol.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/protocol.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/rclone.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/rfio.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/rfio.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/srm.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/srm.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/ssh.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/storm.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/storm.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/webdav.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/protocols/xrootd.py` & `rucio-32.0.0rc2/lib/rucio/rse/protocols/xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/rse/rsemanager.py` & `rucio-32.0.0rc2/lib/rucio/rse/rsemanager.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/tests/__init__.py` & `rucio-32.0.0rc2/lib/rucio/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/tests/common.py` & `rucio-32.0.0rc2/lib/rucio/tests/common.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/tests/common_server.py` & `rucio-32.0.0rc2/lib/rucio/tests/common_server.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/transfertool/__init__.py` & `rucio-32.0.0rc2/lib/rucio/transfertool/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/transfertool/fts3.py` & `rucio-32.0.0rc2/lib/rucio/transfertool/fts3.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/transfertool/globus.py` & `rucio-32.0.0rc2/lib/rucio/transfertool/globus.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/transfertool/globus_library.py` & `rucio-32.0.0rc2/lib/rucio/transfertool/globus_library.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/transfertool/mock.py` & `rucio-32.0.0rc2/lib/rucio/transfertool/mock.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,42 +12,73 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import itertools
 import logging
 import uuid
+from typing import TYPE_CHECKING, Any, Optional, Sequence
 
-from rucio.transfertool.transfertool import Transfertool, TransferToolBuilder
+from rucio.db.sqla.constants import RequestState
+from rucio.transfertool.transfertool import Transfertool, TransferToolBuilder, TransferStatusReport
+
+if TYPE_CHECKING:
+    from rucio.db.sqla.session import Session
+
+
+class MockTransferStatusReport(TransferStatusReport):
+
+    supported_db_fields = [
+        'state',
+        'external_id'
+    ]
+
+    def __init__(self, request_id: str, external_id: str):
+        super().__init__(request_id)
+        self.state = RequestState.DONE
+        self.external_id = external_id
+
+    def initialize(self, session: "Session", logger=logging.log):
+        pass
+
+    def get_monitor_msg_fields(self, session: "Session", logger=logging.log):
+        return {}
 
 
 class MockTransfertool(Transfertool):
     """
     Mock implementation of a Rucio transfertool
 
     This is not actually used anywhere at the moment
     """
 
     external_name = 'mock'
     required_rse_attrs = ()
 
-    def __init__(self, external_host, logger=logging.log):
+    def __init__(self, external_host: str, logger=logging.log):
         super(MockTransfertool, self).__init__(external_host, logger)
 
     @classmethod
     def submission_builder_for_path(cls, transfer_path, logger=logging.log):
         return transfer_path, TransferToolBuilder(cls, external_host='Mock Transfertool')
 
     def group_into_submit_jobs(self, transfers):
         return [{'transfers': list(itertools.chain.from_iterable(transfers)), 'job_params': {}}]
 
     def submit(self, files, job_params, timeout=None):
         return str(uuid.uuid1())
 
-    def query(self, transfer_ids, details=False, timeout=None):
+    def bulk_query(self, requests_by_eid: dict[str, dict[str, dict[str, Any]]], timeout: Optional[float] = None):
+        response = {}
+        for transfer_id, requests in requests_by_eid.items():
+            for request_id in requests:
+                response.setdefault(transfer_id, {})[request_id] = MockTransferStatusReport(request_id, transfer_id)
+        return response
+
+    def query(self, transfer_ids: Sequence[str], details: bool = False, timeout: Optional[float] = None):
         return [{'status': 'ok'}]
 
-    def cancel(self, transfer_ids, timeout=None):
+    def cancel(self, transfer_ids: Sequence[str], timeout: Optional[float] = None):
         return True
 
-    def update_priority(self, transfer_id, priority, timeout=None):
+    def update_priority(self, transfer_id: str, priority: int, timeout: Optional[float] = None):
         return True
```

### Comparing `rucio-32.0.0rc1/lib/rucio/transfertool/transfertool.py` & `rucio-32.0.0rc2/lib/rucio/transfertool/transfertool.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         :param external_host:   The external host where the transfertool API is running
         """
 
         self.external_host = external_host
         self.logger = logger
 
     def __str__(self):
-        return self.external_host
+        return self.external_host if self.external_host is not None else self.__class__.__name__
 
     @classmethod
     def can_perform_transfer(cls, source_rse: "RseData", dest_rse: "RseData"):
         """
         Return True if this transfertool is able to perform a transfer between the given source and destination rses
         """
         if (
```

### Comparing `rucio-32.0.0rc1/lib/rucio/version.py` & `rucio-32.0.0rc2/lib/rucio/version.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/__init__.py` & `rucio-32.0.0rc2/lib/rucio/web/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/__init__.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/__init__.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/authenticated_bp.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/authenticated_bp.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/__init__.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/accountlimits.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/accountlimits.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/accounts.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/accounts.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/archives.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/archives.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/auth.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1607,14 +1607,15 @@
 
     user_pass_view = UserPass.as_view('user_pass')
     bp.add_url_rule('/userpass', view_func=user_pass_view, methods=['get', 'options'])
     gss_view = GSS.as_view('gss')
     bp.add_url_rule('/gss', view_func=gss_view, methods=['get', 'options'])
     x509_view = x509.as_view('x509')
     bp.add_url_rule('/x509', view_func=x509_view, methods=['get', 'options'])
+    bp.add_url_rule('/x509/webui', view_func=x509_view, methods=['get', 'options'])
     bp.add_url_rule('/x509_proxy', view_func=x509_view, methods=['get', 'options'])
     ssh_view = SSH.as_view('ssh')
     bp.add_url_rule('/ssh', view_func=ssh_view, methods=['get', 'options'])
     ssh_challenge_token_view = SSHChallengeToken.as_view('ssh_challenge_token')
     bp.add_url_rule('/ssh_challenge_token', view_func=ssh_challenge_token_view, methods=['get', 'options'])
     saml_view = SAML.as_view('saml')
     bp.add_url_rule('/saml', view_func=saml_view, methods=['get', 'post', 'options'])
```

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/common.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/common.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/config.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/config.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/credentials.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/credentials.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/dids.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/dids.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/dirac.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/dirac.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/export.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/export.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/heartbeats.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/identities.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/identities.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/import.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/import.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/locks.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/locks.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/main.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/main.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/meta.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/meta.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/metrics.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/ping.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/ping.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/redirect.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/replicas.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/requests.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/requests.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/rses.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/rses.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/rules.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/rules.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/scopes.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/scopes.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/subscriptions.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/subscriptions.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/tmp_dids.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/tmp_dids.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/traces.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/traces.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/flaskapi/v1/vos.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/flaskapi/v1/vos.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/main.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/main.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio/web/rest/metrics.py` & `rucio-32.0.0rc2/lib/rucio/web/rest/metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/lib/rucio.egg-info/SOURCES.txt` & `rucio-32.0.0rc2/lib/rucio.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -311,14 +311,15 @@
 lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py
 lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py
 lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py
 lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py
 lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py
 lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py
 lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py
+lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py
 lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py
 lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py
 lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py
 lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py
 lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py
 lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py
 lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py
```

### Comparing `rucio-32.0.0rc1/pylintrc` & `rucio-32.0.0rc2/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/requirements.txt` & `rucio-32.0.0rc2/requirements.txt`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/setup.py` & `rucio-32.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/setuputil.py` & `rucio-32.0.0rc2/setuputil.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_abacus_account.py` & `rucio-32.0.0rc2/tests/test_abacus_account.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_abacus_collection_replica.py` & `rucio-32.0.0rc2/tests/test_abacus_collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_abacus_rse.py` & `rucio-32.0.0rc2/tests/test_abacus_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_account.py` & `rucio-32.0.0rc2/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_account_limits.py` & `rucio-32.0.0rc2/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_api_external_representation.py` & `rucio-32.0.0rc2/tests/test_api_external_representation.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_archive.py` & `rucio-32.0.0rc2/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_auditor.py` & `rucio-32.0.0rc2/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_auditor_hdfs.py` & `rucio-32.0.0rc2/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_auditor_srmdumps.py` & `rucio-32.0.0rc2/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_authentication.py` & `rucio-32.0.0rc2/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_automatix.py` & `rucio-32.0.0rc2/tests/test_automatix.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_bad_replica.py` & `rucio-32.0.0rc2/tests/test_bad_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_bb8.py` & `rucio-32.0.0rc2/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_belleii.py` & `rucio-32.0.0rc2/tests/test_belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_bin_rucio.py` & `rucio-32.0.0rc2/tests/test_bin_rucio.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_boolean.py` & `rucio-32.0.0rc2/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_clients.py` & `rucio-32.0.0rc2/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_common_types.py` & `rucio-32.0.0rc2/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_config.py` & `rucio-32.0.0rc2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_conveyor.py` & `rucio-32.0.0rc2/tests/test_conveyor.py`

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

### Comparing `rucio-32.0.0rc1/tests/test_conveyor_submitter.py` & `rucio-32.0.0rc2/tests/test_conveyor_submitter.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_counter.py` & `rucio-32.0.0rc2/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_credential.py` & `rucio-32.0.0rc2/tests/test_credential.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_curl.py` & `rucio-32.0.0rc2/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_daemons.py` & `rucio-32.0.0rc2/tests/test_daemons.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_dataset_replicas.py` & `rucio-32.0.0rc2/tests/test_dataset_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_db.py` & `rucio-32.0.0rc2/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_did.py` & `rucio-32.0.0rc2/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_did_meta_plugins.py` & `rucio-32.0.0rc2/tests/test_did_meta_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_didtype.py` & `rucio-32.0.0rc2/tests/test_didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_download.py` & `rucio-32.0.0rc2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_dumper.py` & `rucio-32.0.0rc2/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_dumper_consistency.py` & `rucio-32.0.0rc2/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_dumper_data_model.py` & `rucio-32.0.0rc2/tests/test_dumper_data_model.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_dumper_path_parsing.py` & `rucio-32.0.0rc2/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_filter_engine.py` & `rucio-32.0.0rc2/tests/test_filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_heartbeat.py` & `rucio-32.0.0rc2/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_hermes.py` & `rucio-32.0.0rc2/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_identity.py` & `rucio-32.0.0rc2/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_impl_upload_download.py` & `rucio-32.0.0rc2/tests/test_impl_upload_download.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_import_export.py` & `rucio-32.0.0rc2/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_judge_cleaner.py` & `rucio-32.0.0rc2/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_judge_evaluator.py` & `rucio-32.0.0rc2/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_judge_injector.py` & `rucio-32.0.0rc2/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_judge_repairer.py` & `rucio-32.0.0rc2/tests/test_judge_repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_lifetime.py` & `rucio-32.0.0rc2/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_message.py` & `rucio-32.0.0rc2/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_meta.py` & `rucio-32.0.0rc2/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_meta_did.py` & `rucio-32.0.0rc2/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_module_import.py` & `rucio-32.0.0rc2/tests/test_module_import.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_monitor.py` & `rucio-32.0.0rc2/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_multi_vo.py` & `rucio-32.0.0rc2/tests/test_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_naming_convention.py` & `rucio-32.0.0rc2/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_oauthmanager.py` & `rucio-32.0.0rc2/tests/test_oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_oidc.py` & `rucio-32.0.0rc2/tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_permission.py` & `rucio-32.0.0rc2/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_pfns.py` & `rucio-32.0.0rc2/tests/test_pfns.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_ping.py` & `rucio-32.0.0rc2/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_preparer.py` & `rucio-32.0.0rc2/tests/test_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_qos.py` & `rucio-32.0.0rc2/tests/test_qos.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_quarantined_replica.py` & `rucio-32.0.0rc2/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_reaper.py` & `rucio-32.0.0rc2/tests/test_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_redirect.py` & `rucio-32.0.0rc2/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_replica.py` & `rucio-32.0.0rc2/tests/test_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_replica_recoverer.py` & `rucio-32.0.0rc2/tests/test_replica_recoverer.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_replica_sorting.py` & `rucio-32.0.0rc2/tests/test_replica_sorting.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_request.py` & `rucio-32.0.0rc2/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_root_proxy.py` & `rucio-32.0.0rc2/tests/test_root_proxy.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rse.py` & `rucio-32.0.0rc2/tests/test_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rse_expression_parser.py` & `rucio-32.0.0rc2/tests/test_rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rse_lfn2path.py` & `rucio-32.0.0rc2/tests/test_rse_lfn2path.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rse_protocol_gfal2.py` & `rucio-32.0.0rc2/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rse_protocol_gfal2_impl.py` & `rucio-32.0.0rc2/tests/test_rse_protocol_gfal2_impl.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rse_protocol_posix.py` & `rucio-32.0.0rc2/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rse_protocol_rclone.py` & `rucio-32.0.0rc2/tests/test_rse_protocol_rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rse_protocol_rsync.py` & `rucio-32.0.0rc2/tests/test_rse_protocol_rsync.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rse_protocol_srm.py` & `rucio-32.0.0rc2/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rse_protocol_ssh.py` & `rucio-32.0.0rc2/tests/test_rse_protocol_ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rse_protocol_webdav.py` & `rucio-32.0.0rc2/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rse_protocol_xrootd.py` & `rucio-32.0.0rc2/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rse_selector.py` & `rucio-32.0.0rc2/tests/test_rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rucio_server.py` & `rucio-32.0.0rc2/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_rule.py` & `rucio-32.0.0rc2/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_schema_cms.py` & `rucio-32.0.0rc2/tests/test_schema_cms.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_scope.py` & `rucio-32.0.0rc2/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_subscription.py` & `rucio-32.0.0rc2/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_temporary_did.py` & `rucio-32.0.0rc2/tests/test_temporary_did.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_throttler.py` & `rucio-32.0.0rc2/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_tpc.py` & `rucio-32.0.0rc2/tests/test_tpc.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_trace.py` & `rucio-32.0.0rc2/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_transfer.py` & `rucio-32.0.0rc2/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_undertaker.py` & `rucio-32.0.0rc2/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_upload.py` & `rucio-32.0.0rc2/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tests/test_utils.py` & `rucio-32.0.0rc2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tools/bootstrap.py` & `rucio-32.0.0rc2/tools/bootstrap.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tools/merge_rucio_configs.py` & `rucio-32.0.0rc2/tools/merge_rucio_configs.py`

 * *Files identical despite different names*

### Comparing `rucio-32.0.0rc1/tools/reset_database.py` & `rucio-32.0.0rc2/tools/reset_database.py`

 * *Files identical despite different names*

