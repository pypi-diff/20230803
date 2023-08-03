# Comparing `tmp/rucio-clients-32.0.0rc1.tar.gz` & `tmp/rucio-clients-32.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-clients-32.0.0rc1.tar", last modified: Wed Jul 26 15:14:47 2023, max compression
+gzip compressed data, was "rucio-clients-32.0.0rc2.tar", last modified: Thu Aug  3 15:23:02 2023, max compression
```

## Comparing `rucio-clients-32.0.0rc1.tar` & `rucio-clients-32.0.0rc2.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:47.805165 rucio-clients-32.0.0rc1/
--rwxr-xr-x   0 root         (0) root         (0)     4383 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      598 2023-07-26 15:14:41.000000 rucio-clients-32.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      936 2023-07-26 15:14:47.805165 rucio-clients-32.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1982 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:47.752163 rucio-clients-32.0.0rc1/bin/
--rwxr-xr-x   0 root         (0) root         (0)   128576 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/bin/rucio
--rwxr-xr-x   0 root         (0) root         (0)   133738 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/bin/rucio-admin
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:47.753163 rucio-clients-32.0.0rc1/etc/
--rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/etc/rse-accounts.cfg.template
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/etc/rucio.cfg.atlas.client.template
--rw-r--r--   0 root         (0) root         (0)     8534 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/etc/rucio.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:47.748163 rucio-clients-32.0.0rc1/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:47.754163 rucio-clients-32.0.0rc1/lib/rucio/
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      714 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/alembicrevision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:47.761163 rucio-clients-32.0.0rc1/lib/rucio/client/
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16412 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/accountclient.py
--rw-r--r--   0 root         (0) root         (0)     6020 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/accountlimitclient.py
--rw-r--r--   0 root         (0) root         (0)    47219 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/baseclient.py
--rw-r--r--   0 root         (0) root         (0)     3072 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/client.py
--rw-r--r--   0 root         (0) root         (0)     4460 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/configclient.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/credentialclient.py
--rw-r--r--   0 root         (0) root         (0)    28223 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/didclient.py
--rw-r--r--   0 root         (0) root         (0)     1991 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/diracclient.py
--rw-r--r--   0 root         (0) root         (0)    86127 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/downloadclient.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/exportclient.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/fileclient.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/importclient.py
--rw-r--r--   0 root         (0) root         (0)     2881 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/lifetimeclient.py
--rw-r--r--   0 root         (0) root         (0)     3973 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/lockclient.py
--rw-r--r--   0 root         (0) root         (0)     4722 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/metaclient.py
--rw-r--r--   0 root         (0) root         (0)     1414 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/pingclient.py
--rw-r--r--   0 root         (0) root         (0)    19343 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/replicaclient.py
--rw-r--r--   0 root         (0) root         (0)     4256 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/requestclient.py
--rw-r--r--   0 root         (0) root         (0)    27183 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/rseclient.py
--rw-r--r--   0 root         (0) root         (0)    12741 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/ruleclient.py
--rw-r--r--   0 root         (0) root         (0)     3206 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/scopeclient.py
--rw-r--r--   0 root         (0) root         (0)     7980 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/subscriptionclient.py
--rw-r--r--   0 root         (0) root         (0)     2701 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/touchclient.py
--rw-r--r--   0 root         (0) root         (0)    45907 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/client/uploadclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:47.766163 rucio-clients-32.0.0rc1/lib/rucio/common/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/cache.py
--rw-r--r--   0 root         (0) root         (0)    24286 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/config.py
--rw-r--r--   0 root         (0) root         (0)     3314 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/constants.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/constraints.py
--rwxr-xr-x   0 root         (0) root         (0)     6323 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/didtype.py
--rw-r--r--   0 root         (0) root         (0)    32369 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/exception.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/extra.py
--rw-r--r--   0 root         (0) root         (0)    15070 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/logging.py
--rw-r--r--   0 root         (0) root         (0)    45324 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/pcache.py
--rw-r--r--   0 root         (0) root         (0)     3037 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:47.769164 rucio-clients-32.0.0rc1/lib/rucio/common/schema/
--rw-r--r--   0 root         (0) root         (0)     5176 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15628 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/schema/atlas.py
--rw-r--r--   0 root         (0) root         (0)    15445 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/schema/belleii.py
--rw-r--r--   0 root         (0) root         (0)    18575 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/schema/cms.py
--rw-r--r--   0 root         (0) root         (0)    15026 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/schema/domatpc.py
--rw-r--r--   0 root         (0) root         (0)    15965 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/schema/escape.py
--rw-r--r--   0 root         (0) root         (0)    16280 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/schema/generic.py
--rw-r--r--   0 root         (0) root         (0)    15507 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/schema/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)    15316 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/schema/icecube.py
--rw-r--r--   0 root         (0) root         (0)    15924 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/schema/lsst.py
--rw-r--r--   0 root         (0) root         (0)     5438 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/stomp_utils.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     4929 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)     3281 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/types.py
--rw-r--r--   0 root         (0) root         (0)    69433 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:47.769164 rucio-clients-32.0.0rc1/lib/rucio/rse/
--rw-r--r--   0 root         (0) root         (0)     3327 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:47.774164 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4627 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/cache.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/dummy.py
--rw-r--r--   0 root         (0) root         (0)    29035 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/gfal.py
--rw-r--r--   0 root         (0) root         (0)     9704 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/globus.py
--rw-r--r--   0 root         (0) root         (0)     3433 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/gsiftp.py
--rw-r--r--   0 root         (0) root         (0)     2999 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/http_cache.py
--rw-r--r--   0 root         (0) root         (0)     4519 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/mock.py
--rw-r--r--   0 root         (0) root         (0)     7248 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/ngarc.py
--rw-r--r--   0 root         (0) root         (0)    10418 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/posix.py
--rw-r--r--   0 root         (0) root         (0)    22818 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/protocol.py
--rw-r--r--   0 root         (0) root         (0)    15276 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/rclone.py
--rw-r--r--   0 root         (0) root         (0)     5554 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/rfio.py
--rw-r--r--   0 root         (0) root         (0)    14671 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/srm.py
--rw-r--r--   0 root         (0) root         (0)    17487 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/ssh.py
--rw-r--r--   0 root         (0) root         (0)     8151 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/storm.py
--rw-r--r--   0 root         (0) root         (0)    22219 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/webdav.py
--rw-r--r--   0 root         (0) root         (0)    12489 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/xrootd.py
--rw-r--r--   0 root         (0) root         (0)    36928 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/rse/rsemanager.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-07-26 15:02:05.000000 rucio-clients-32.0.0rc1/lib/rucio/vcsversion.py
--rw-r--r--   0 root         (0) root         (0)     1573 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/lib/rucio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:47.805165 rucio-clients-32.0.0rc1/lib/rucio_clients.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5113 2023-07-26 15:14:47.000000 rucio-clients-32.0.0rc1/lib/rucio_clients.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    16384 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/pylintrc
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5083 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      206 2023-07-26 15:14:47.806166 rucio-clients-32.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3074 2023-07-26 15:14:41.000000 rucio-clients-32.0.0rc1/setup.py
--rw-r--r--   0 root         (0) root         (0)     4749 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/setuputil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:47.804165 rucio-clients-32.0.0rc1/tests/
--rw-r--r--   0 root         (0) root         (0)     3708 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_abacus_account.py
--rw-r--r--   0 root         (0) root         (0)    10771 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_abacus_collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3255 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_abacus_rse.py
--rw-r--r--   0 root         (0) root         (0)    15997 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_account.py
--rw-r--r--   0 root         (0) root         (0)     9834 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_account_limits.py
--rw-r--r--   0 root         (0) root         (0)    20192 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_api_external_representation.py
--rw-r--r--   0 root         (0) root         (0)    13376 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_archive.py
--rw-r--r--   0 root         (0) root         (0)     4120 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_auditor.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_auditor_hdfs.py
--rw-r--r--   0 root         (0) root         (0)     4225 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_auditor_srmdumps.py
--rw-r--r--   0 root         (0) root         (0)    15239 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_automatix.py
--rw-r--r--   0 root         (0) root         (0)    23339 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_bad_replica.py
--rw-r--r--   0 root         (0) root         (0)    12468 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_bb8.py
--rw-r--r--   0 root         (0) root         (0)     4707 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_belleii.py
--rwxr-xr-x   0 root         (0) root         (0)   107211 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_bin_rucio.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     8248 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_clients.py
--rw-r--r--   0 root         (0) root         (0)     1889 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_common_types.py
--rw-r--r--   0 root         (0) root         (0)     6966 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    85465 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_conveyor.py
--rw-r--r--   0 root         (0) root         (0)    22228 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_conveyor_submitter.py
--rw-r--r--   0 root         (0) root         (0)     6971 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     7703 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_credential.py
--rw-r--r--   0 root         (0) root         (0)     7361 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_curl.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_daemons.py
--rw-r--r--   0 root         (0) root         (0)    28205 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_dataset_replicas.py
--rw-r--r--   0 root         (0) root         (0)     2759 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    55592 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_did.py
--rw-r--r--   0 root         (0) root         (0)    29541 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_did_meta_plugins.py
--rw-r--r--   0 root         (0) root         (0)     4209 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_didtype.py
--rw-r--r--   0 root         (0) root         (0)    35378 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7203 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_dumper.py
--rw-r--r--   0 root         (0) root         (0)    16658 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_dumper_consistency.py
--rw-r--r--   0 root         (0) root         (0)    10907 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_dumper_data_model.py
--rw-r--r--   0 root         (0) root         (0)     3158 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_dumper_path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    38325 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     7977 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    10138 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_hermes.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_identity.py
--rw-r--r--   0 root         (0) root         (0)    18578 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_impl_upload_download.py
--rw-r--r--   0 root         (0) root         (0)    57799 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     5281 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_judge_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    22299 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_judge_evaluator.py
--rw-r--r--   0 root         (0) root         (0)    11070 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_judge_injector.py
--rw-r--r--   0 root         (0) root         (0)    20482 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_judge_repairer.py
--rw-r--r--   0 root         (0) root         (0)    12205 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_lifetime.py
--rw-r--r--   0 root         (0) root         (0)     5879 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     6270 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     1790 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_meta_did.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_module_import.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_monitor.py
--rw-r--r--   0 root         (0) root         (0)    54354 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     2911 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_naming_convention.py
--rw-r--r--   0 root         (0) root         (0)    11606 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_oauthmanager.py
--rw-r--r--   0 root         (0) root         (0)   107576 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_oidc.py
--rw-r--r--   0 root         (0) root         (0)     4529 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     4147 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_pfns.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_ping.py
--rw-r--r--   0 root         (0) root         (0)     7607 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2765 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_qos.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    27057 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_reaper.py
--rw-r--r--   0 root         (0) root         (0)     6464 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)    62407 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_replica.py
--rw-r--r--   0 root         (0) root         (0)    32236 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_replica_recoverer.py
--rw-r--r--   0 root         (0) root         (0)    22852 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_replica_sorting.py
--rw-r--r--   0 root         (0) root         (0)    13879 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)    13074 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_root_proxy.py
--rw-r--r--   0 root         (0) root         (0)    75437 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rse.py
--rw-r--r--   0 root         (0) root         (0)    13230 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)     8966 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rse_lfn2path.py
--rw-r--r--   0 root         (0) root         (0)     4300 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 root         (0) root         (0)     3845 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rse_protocol_gfal2_impl.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rse_protocol_posix.py
--rw-r--r--   0 root         (0) root         (0)     3713 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rse_protocol_rclone.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rse_protocol_rsync.py
--rw-r--r--   0 root         (0) root         (0)     4002 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rse_protocol_srm.py
--rw-r--r--   0 root         (0) root         (0)     4678 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rse_protocol_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 root         (0) root         (0)     3803 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 root         (0) root         (0)     7770 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rse_selector.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)    90900 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)    13873 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_schema_cms.py
--rw-r--r--   0 root         (0) root         (0)     7510 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_scope.py
--rw-r--r--   0 root         (0) root         (0)    48744 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)     2771 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_temporary_did.py
--rw-r--r--   0 root         (0) root         (0)    55640 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_throttler.py
--rw-r--r--   0 root         (0) root         (0)     5045 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_tpc.py
--rw-r--r--   0 root         (0) root         (0)     3204 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_trace.py
--rw-r--r--   0 root         (0) root         (0)    19610 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_transfer.py
--rw-r--r--   0 root         (0) root         (0)     8478 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_undertaker.py
--rw-r--r--   0 root         (0) root         (0)    15673 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     6375 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:14:47.805165 rucio-clients-32.0.0rc1/tools/
--rw-r--r--   0 root         (0) root         (0)     6123 2023-07-26 12:29:16.000000 rucio-clients-32.0.0rc1/tools/merge_rucio_configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:02.500942 rucio-clients-32.0.0rc2/
+-rwxr-xr-x   0 root         (0) root         (0)     4383 2023-08-03 09:00:33.000000 rucio-clients-32.0.0rc2/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      598 2023-08-03 15:22:56.000000 rucio-clients-32.0.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      936 2023-08-03 15:23:02.500942 rucio-clients-32.0.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:02.449941 rucio-clients-32.0.0rc2/bin/
+-rwxr-xr-x   0 root         (0) root         (0)   128576 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/bin/rucio
+-rwxr-xr-x   0 root         (0) root         (0)   133738 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/bin/rucio-admin
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:02.450941 rucio-clients-32.0.0rc2/etc/
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/etc/rse-accounts.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/etc/rucio.cfg.atlas.client.template
+-rw-r--r--   0 root         (0) root         (0)     8534 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/etc/rucio.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:02.445941 rucio-clients-32.0.0rc2/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:02.451941 rucio-clients-32.0.0rc2/lib/rucio/
+-rw-r--r--   0 root         (0) root         (0)      684 2023-08-03 09:00:33.000000 rucio-clients-32.0.0rc2/lib/rucio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      714 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/alembicrevision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:02.458941 rucio-clients-32.0.0rc2/lib/rucio/client/
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16412 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/accountclient.py
+-rw-r--r--   0 root         (0) root         (0)     6020 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/accountlimitclient.py
+-rw-r--r--   0 root         (0) root         (0)    47219 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/baseclient.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     4460 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/client/configclient.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/client/credentialclient.py
+-rw-r--r--   0 root         (0) root         (0)    28223 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/didclient.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/diracclient.py
+-rw-r--r--   0 root         (0) root         (0)    86127 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/downloadclient.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/client/exportclient.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/fileclient.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/client/importclient.py
+-rw-r--r--   0 root         (0) root         (0)     2881 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/lifetimeclient.py
+-rw-r--r--   0 root         (0) root         (0)     3973 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/lockclient.py
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/metaclient.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/pingclient.py
+-rw-r--r--   0 root         (0) root         (0)    19343 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/replicaclient.py
+-rw-r--r--   0 root         (0) root         (0)     4256 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/requestclient.py
+-rw-r--r--   0 root         (0) root         (0)    27183 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/rseclient.py
+-rw-r--r--   0 root         (0) root         (0)    12741 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/ruleclient.py
+-rw-r--r--   0 root         (0) root         (0)     3206 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/scopeclient.py
+-rw-r--r--   0 root         (0) root         (0)     7980 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/subscriptionclient.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/touchclient.py
+-rw-r--r--   0 root         (0) root         (0)    45907 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/client/uploadclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:02.463941 rucio-clients-32.0.0rc2/lib/rucio/common/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/common/cache.py
+-rw-r--r--   0 root         (0) root         (0)    24286 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/common/config.py
+-rw-r--r--   0 root         (0) root         (0)     3314 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/common/constants.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/common/constraints.py
+-rwxr-xr-x   0 root         (0) root         (0)     6323 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/common/didtype.py
+-rw-r--r--   0 root         (0) root         (0)    32369 2023-08-03 09:00:33.000000 rucio-clients-32.0.0rc2/lib/rucio/common/exception.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/common/extra.py
+-rw-r--r--   0 root         (0) root         (0)    15070 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/common/logging.py
+-rw-r--r--   0 root         (0) root         (0)    45324 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/common/pcache.py
+-rw-r--r--   0 root         (0) root         (0)     3037 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/common/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:02.466941 rucio-clients-32.0.0rc2/lib/rucio/common/schema/
+-rw-r--r--   0 root         (0) root         (0)     5176 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/common/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15628 2023-08-03 09:00:33.000000 rucio-clients-32.0.0rc2/lib/rucio/common/schema/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    15445 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/common/schema/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    18575 2023-08-03 09:00:33.000000 rucio-clients-32.0.0rc2/lib/rucio/common/schema/cms.py
+-rw-r--r--   0 root         (0) root         (0)    15026 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/common/schema/domatpc.py
+-rw-r--r--   0 root         (0) root         (0)    15965 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/common/schema/escape.py
+-rw-r--r--   0 root         (0) root         (0)    16280 2023-08-03 09:00:33.000000 rucio-clients-32.0.0rc2/lib/rucio/common/schema/generic.py
+-rw-r--r--   0 root         (0) root         (0)    15507 2023-08-03 09:00:33.000000 rucio-clients-32.0.0rc2/lib/rucio/common/schema/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)    15316 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/common/schema/icecube.py
+-rw-r--r--   0 root         (0) root         (0)    15924 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/common/schema/lsst.py
+-rw-r--r--   0 root         (0) root         (0)     5438 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/common/stomp_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/common/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     4929 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/common/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)     3281 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/common/types.py
+-rw-r--r--   0 root         (0) root         (0)    69433 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:02.466941 rucio-clients-32.0.0rc2/lib/rucio/rse/
+-rw-r--r--   0 root         (0) root         (0)     3327 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:02.472941 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4627 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/dummy.py
+-rw-r--r--   0 root         (0) root         (0)    29035 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/gfal.py
+-rw-r--r--   0 root         (0) root         (0)     9704 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/globus.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/gsiftp.py
+-rw-r--r--   0 root         (0) root         (0)     2999 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/http_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4519 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7248 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/ngarc.py
+-rw-r--r--   0 root         (0) root         (0)    10418 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/posix.py
+-rw-r--r--   0 root         (0) root         (0)    22818 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/protocol.py
+-rw-r--r--   0 root         (0) root         (0)    15276 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/rclone.py
+-rw-r--r--   0 root         (0) root         (0)     5554 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/rfio.py
+-rw-r--r--   0 root         (0) root         (0)    14671 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/srm.py
+-rw-r--r--   0 root         (0) root         (0)    17487 2023-08-03 09:00:33.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     8151 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/storm.py
+-rw-r--r--   0 root         (0) root         (0)    22219 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/webdav.py
+-rw-r--r--   0 root         (0) root         (0)    12489 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/xrootd.py
+-rw-r--r--   0 root         (0) root         (0)    36928 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/rse/rsemanager.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-08-03 14:15:48.000000 rucio-clients-32.0.0rc2/lib/rucio/vcsversion.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/lib/rucio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:02.500942 rucio-clients-32.0.0rc2/lib/rucio_clients.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5113 2023-08-03 15:23:02.000000 rucio-clients-32.0.0rc2/lib/rucio_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    16384 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/pylintrc
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-27 12:40:37.000000 rucio-clients-32.0.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5083 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2023-08-03 15:23:02.501942 rucio-clients-32.0.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-08-03 15:22:56.000000 rucio-clients-32.0.0rc2/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4749 2023-08-03 09:00:33.000000 rucio-clients-32.0.0rc2/setuputil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:02.499942 rucio-clients-32.0.0rc2/tests/
+-rw-r--r--   0 root         (0) root         (0)     3708 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_abacus_account.py
+-rw-r--r--   0 root         (0) root         (0)    10771 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_abacus_collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3255 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_abacus_rse.py
+-rw-r--r--   0 root         (0) root         (0)    15997 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_account.py
+-rw-r--r--   0 root         (0) root         (0)     9834 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_account_limits.py
+-rw-r--r--   0 root         (0) root         (0)    20192 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_api_external_representation.py
+-rw-r--r--   0 root         (0) root         (0)    13376 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4120 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_auditor.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_auditor_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 root         (0) root         (0)    15239 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_automatix.py
+-rw-r--r--   0 root         (0) root         (0)    23339 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_bad_replica.py
+-rw-r--r--   0 root         (0) root         (0)    12468 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_bb8.py
+-rw-r--r--   0 root         (0) root         (0)     4707 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_belleii.py
+-rwxr-xr-x   0 root         (0) root         (0)   107211 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_bin_rucio.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     8248 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_common_types.py
+-rw-r--r--   0 root         (0) root         (0)     6966 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    84744 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_conveyor.py
+-rw-r--r--   0 root         (0) root         (0)    22228 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_conveyor_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     6971 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     7703 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7361 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_curl.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_daemons.py
+-rw-r--r--   0 root         (0) root         (0)    28205 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_dataset_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    55592 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_did.py
+-rw-r--r--   0 root         (0) root         (0)    29541 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_did_meta_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     4209 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_didtype.py
+-rw-r--r--   0 root         (0) root         (0)    35378 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7203 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_dumper.py
+-rw-r--r--   0 root         (0) root         (0)    16658 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_dumper_consistency.py
+-rw-r--r--   0 root         (0) root         (0)    10907 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_dumper_data_model.py
+-rw-r--r--   0 root         (0) root         (0)     3158 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    38325 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     7977 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    10138 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_hermes.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)    18578 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_impl_upload_download.py
+-rw-r--r--   0 root         (0) root         (0)    57799 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     5281 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_judge_cleaner.py
+-rw-r--r--   0 root         (0) root         (0)    22299 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_judge_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11070 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_judge_injector.py
+-rw-r--r--   0 root         (0) root         (0)    20482 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_judge_repairer.py
+-rw-r--r--   0 root         (0) root         (0)    12205 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_lifetime.py
+-rw-r--r--   0 root         (0) root         (0)     5879 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     6270 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_meta_did.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_module_import.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    54354 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)    11606 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_oauthmanager.py
+-rw-r--r--   0 root         (0) root         (0)   107576 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     4529 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4147 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_pfns.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_ping.py
+-rw-r--r--   0 root         (0) root         (0)     7607 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_qos.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    27057 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_reaper.py
+-rw-r--r--   0 root         (0) root         (0)     6464 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    62407 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_replica.py
+-rw-r--r--   0 root         (0) root         (0)    32236 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_replica_recoverer.py
+-rw-r--r--   0 root         (0) root         (0)    22852 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_replica_sorting.py
+-rw-r--r--   0 root         (0) root         (0)    13879 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)    13074 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_root_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    75437 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rse.py
+-rw-r--r--   0 root         (0) root         (0)    13230 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)     8966 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rse_lfn2path.py
+-rw-r--r--   0 root         (0) root         (0)     4300 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rse_protocol_gfal2_impl.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rse_protocol_rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rse_protocol_rsync.py
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 root         (0) root         (0)     4678 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rse_protocol_ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 root         (0) root         (0)     7770 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)    90900 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)    13873 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_schema_cms.py
+-rw-r--r--   0 root         (0) root         (0)     7510 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_scope.py
+-rw-r--r--   0 root         (0) root         (0)    48744 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     2771 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_temporary_did.py
+-rw-r--r--   0 root         (0) root         (0)    55640 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_throttler.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_tpc.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)    19610 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     8478 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_undertaker.py
+-rw-r--r--   0 root         (0) root         (0)    15673 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     6375 2023-08-03 09:00:39.000000 rucio-clients-32.0.0rc2/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:23:02.499942 rucio-clients-32.0.0rc2/tools/
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-08-03 09:00:33.000000 rucio-clients-32.0.0rc2/tools/merge_rucio_configs.py
```

### Comparing `rucio-clients-32.0.0rc1/AUTHORS.rst` & `rucio-clients-32.0.0rc2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/LICENSE` & `rucio-clients-32.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/MANIFEST.in` & `rucio-clients-32.0.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/PKG-INFO` & `rucio-clients-32.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio-clients
-Version: 32.0.0rc1
+Version: 32.0.0rc2
 Summary: Rucio Client Lite Package
 Home-page: https://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rucio-clients-32.0.0rc1/README.rst` & `rucio-clients-32.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/bin/rucio` & `rucio-clients-32.0.0rc2/bin/rucio`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/bin/rucio-admin` & `rucio-clients-32.0.0rc2/bin/rucio-admin`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/etc/rse-accounts.cfg.template` & `rucio-clients-32.0.0rc2/etc/rse-accounts.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/etc/rucio.cfg.atlas.client.template` & `rucio-clients-32.0.0rc2/etc/rucio.cfg.atlas.client.template`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/etc/rucio.cfg.template` & `rucio-clients-32.0.0rc2/etc/rucio.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/__init__.py` & `rucio-clients-32.0.0rc2/lib/rucio/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/alembicrevision.py` & `rucio-clients-32.0.0rc2/lib/rucio/alembicrevision.py`

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

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/__init__.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/accountclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/accountclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/accountlimitclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/accountlimitclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/baseclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/baseclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/client.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/client.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/configclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/configclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/credentialclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/credentialclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/didclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/didclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/diracclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/diracclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/downloadclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/downloadclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/exportclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/exportclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/fileclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/fileclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/importclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/importclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/lifetimeclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/lifetimeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/lockclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/lockclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/metaclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/metaclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/pingclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/pingclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/replicaclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/replicaclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/requestclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/requestclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/rseclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/rseclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/ruleclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/ruleclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/scopeclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/scopeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/subscriptionclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/touchclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/touchclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/client/uploadclient.py` & `rucio-clients-32.0.0rc2/lib/rucio/client/uploadclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/__init__.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/cache.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/cache.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/config.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/config.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/constants.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/constants.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/constraints.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/constraints.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/didtype.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/exception.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/exception.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/extra.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/extra.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/logging.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/logging.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/pcache.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/pcache.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/policy.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/policy.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/schema/__init__.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/schema/atlas.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/schema/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/schema/belleii.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/schema/belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/schema/cms.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/schema/cms.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/schema/domatpc.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/schema/domatpc.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/schema/escape.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/schema/escape.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/schema/generic.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/schema/generic.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/schema/generic_multi_vo.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/schema/generic_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/schema/icecube.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/schema/icecube.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/schema/lsst.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/schema/lsst.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/stomp_utils.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/stomp_utils.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/stopwatch.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/stopwatch.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/test_rucio_server.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/types.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/types.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/common/utils.py` & `rucio-clients-32.0.0rc2/lib/rucio/common/utils.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/__init__.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/__init__.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/cache.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/cache.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/dummy.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/dummy.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/gfal.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/gfal.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/globus.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/globus.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/gsiftp.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/gsiftp.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/http_cache.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/http_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/mock.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/mock.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/ngarc.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/ngarc.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/posix.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/posix.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/protocol.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/protocol.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/rclone.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/rfio.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/rfio.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/srm.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/srm.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/ssh.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/storm.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/storm.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/webdav.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/protocols/xrootd.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/protocols/xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/rse/rsemanager.py` & `rucio-clients-32.0.0rc2/lib/rucio/rse/rsemanager.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio/version.py` & `rucio-clients-32.0.0rc2/lib/rucio/version.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/lib/rucio_clients.egg-info/SOURCES.txt` & `rucio-clients-32.0.0rc2/lib/rucio_clients.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/pylintrc` & `rucio-clients-32.0.0rc2/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/requirements.txt` & `rucio-clients-32.0.0rc2/requirements.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/setup.py` & `rucio-clients-32.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/setuputil.py` & `rucio-clients-32.0.0rc2/setuputil.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_abacus_account.py` & `rucio-clients-32.0.0rc2/tests/test_abacus_account.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_abacus_collection_replica.py` & `rucio-clients-32.0.0rc2/tests/test_abacus_collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_abacus_rse.py` & `rucio-clients-32.0.0rc2/tests/test_abacus_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_account.py` & `rucio-clients-32.0.0rc2/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_account_limits.py` & `rucio-clients-32.0.0rc2/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_api_external_representation.py` & `rucio-clients-32.0.0rc2/tests/test_api_external_representation.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_archive.py` & `rucio-clients-32.0.0rc2/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_auditor.py` & `rucio-clients-32.0.0rc2/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_auditor_hdfs.py` & `rucio-clients-32.0.0rc2/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_auditor_srmdumps.py` & `rucio-clients-32.0.0rc2/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_authentication.py` & `rucio-clients-32.0.0rc2/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_automatix.py` & `rucio-clients-32.0.0rc2/tests/test_automatix.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_bad_replica.py` & `rucio-clients-32.0.0rc2/tests/test_bad_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_bb8.py` & `rucio-clients-32.0.0rc2/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_belleii.py` & `rucio-clients-32.0.0rc2/tests/test_belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_bin_rucio.py` & `rucio-clients-32.0.0rc2/tests/test_bin_rucio.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_boolean.py` & `rucio-clients-32.0.0rc2/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_clients.py` & `rucio-clients-32.0.0rc2/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_common_types.py` & `rucio-clients-32.0.0rc2/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_config.py` & `rucio-clients-32.0.0rc2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_conveyor.py` & `rucio-clients-32.0.0rc2/tests/test_conveyor.py`

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

### Comparing `rucio-clients-32.0.0rc1/tests/test_conveyor_submitter.py` & `rucio-clients-32.0.0rc2/tests/test_conveyor_submitter.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_counter.py` & `rucio-clients-32.0.0rc2/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_credential.py` & `rucio-clients-32.0.0rc2/tests/test_credential.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_curl.py` & `rucio-clients-32.0.0rc2/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_daemons.py` & `rucio-clients-32.0.0rc2/tests/test_daemons.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_dataset_replicas.py` & `rucio-clients-32.0.0rc2/tests/test_dataset_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_db.py` & `rucio-clients-32.0.0rc2/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_did.py` & `rucio-clients-32.0.0rc2/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_did_meta_plugins.py` & `rucio-clients-32.0.0rc2/tests/test_did_meta_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_didtype.py` & `rucio-clients-32.0.0rc2/tests/test_didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_download.py` & `rucio-clients-32.0.0rc2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_dumper.py` & `rucio-clients-32.0.0rc2/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_dumper_consistency.py` & `rucio-clients-32.0.0rc2/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_dumper_data_model.py` & `rucio-clients-32.0.0rc2/tests/test_dumper_data_model.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_dumper_path_parsing.py` & `rucio-clients-32.0.0rc2/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_filter_engine.py` & `rucio-clients-32.0.0rc2/tests/test_filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_heartbeat.py` & `rucio-clients-32.0.0rc2/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_hermes.py` & `rucio-clients-32.0.0rc2/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_identity.py` & `rucio-clients-32.0.0rc2/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_impl_upload_download.py` & `rucio-clients-32.0.0rc2/tests/test_impl_upload_download.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_import_export.py` & `rucio-clients-32.0.0rc2/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_judge_cleaner.py` & `rucio-clients-32.0.0rc2/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_judge_evaluator.py` & `rucio-clients-32.0.0rc2/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_judge_injector.py` & `rucio-clients-32.0.0rc2/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_judge_repairer.py` & `rucio-clients-32.0.0rc2/tests/test_judge_repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_lifetime.py` & `rucio-clients-32.0.0rc2/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_message.py` & `rucio-clients-32.0.0rc2/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_meta.py` & `rucio-clients-32.0.0rc2/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_meta_did.py` & `rucio-clients-32.0.0rc2/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_module_import.py` & `rucio-clients-32.0.0rc2/tests/test_module_import.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_monitor.py` & `rucio-clients-32.0.0rc2/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_multi_vo.py` & `rucio-clients-32.0.0rc2/tests/test_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_naming_convention.py` & `rucio-clients-32.0.0rc2/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_oauthmanager.py` & `rucio-clients-32.0.0rc2/tests/test_oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_oidc.py` & `rucio-clients-32.0.0rc2/tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_permission.py` & `rucio-clients-32.0.0rc2/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_pfns.py` & `rucio-clients-32.0.0rc2/tests/test_pfns.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_ping.py` & `rucio-clients-32.0.0rc2/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_preparer.py` & `rucio-clients-32.0.0rc2/tests/test_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_qos.py` & `rucio-clients-32.0.0rc2/tests/test_qos.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_quarantined_replica.py` & `rucio-clients-32.0.0rc2/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_reaper.py` & `rucio-clients-32.0.0rc2/tests/test_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_redirect.py` & `rucio-clients-32.0.0rc2/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_replica.py` & `rucio-clients-32.0.0rc2/tests/test_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_replica_recoverer.py` & `rucio-clients-32.0.0rc2/tests/test_replica_recoverer.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_replica_sorting.py` & `rucio-clients-32.0.0rc2/tests/test_replica_sorting.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_request.py` & `rucio-clients-32.0.0rc2/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_root_proxy.py` & `rucio-clients-32.0.0rc2/tests/test_root_proxy.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rse.py` & `rucio-clients-32.0.0rc2/tests/test_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rse_expression_parser.py` & `rucio-clients-32.0.0rc2/tests/test_rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rse_lfn2path.py` & `rucio-clients-32.0.0rc2/tests/test_rse_lfn2path.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rse_protocol_gfal2.py` & `rucio-clients-32.0.0rc2/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rse_protocol_gfal2_impl.py` & `rucio-clients-32.0.0rc2/tests/test_rse_protocol_gfal2_impl.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rse_protocol_posix.py` & `rucio-clients-32.0.0rc2/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rse_protocol_rclone.py` & `rucio-clients-32.0.0rc2/tests/test_rse_protocol_rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rse_protocol_rsync.py` & `rucio-clients-32.0.0rc2/tests/test_rse_protocol_rsync.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rse_protocol_srm.py` & `rucio-clients-32.0.0rc2/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rse_protocol_ssh.py` & `rucio-clients-32.0.0rc2/tests/test_rse_protocol_ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rse_protocol_webdav.py` & `rucio-clients-32.0.0rc2/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rse_protocol_xrootd.py` & `rucio-clients-32.0.0rc2/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rse_selector.py` & `rucio-clients-32.0.0rc2/tests/test_rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rucio_server.py` & `rucio-clients-32.0.0rc2/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_rule.py` & `rucio-clients-32.0.0rc2/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_schema_cms.py` & `rucio-clients-32.0.0rc2/tests/test_schema_cms.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_scope.py` & `rucio-clients-32.0.0rc2/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_subscription.py` & `rucio-clients-32.0.0rc2/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_temporary_did.py` & `rucio-clients-32.0.0rc2/tests/test_temporary_did.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_throttler.py` & `rucio-clients-32.0.0rc2/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_tpc.py` & `rucio-clients-32.0.0rc2/tests/test_tpc.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_trace.py` & `rucio-clients-32.0.0rc2/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_transfer.py` & `rucio-clients-32.0.0rc2/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_undertaker.py` & `rucio-clients-32.0.0rc2/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_upload.py` & `rucio-clients-32.0.0rc2/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tests/test_utils.py` & `rucio-clients-32.0.0rc2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-32.0.0rc1/tools/merge_rucio_configs.py` & `rucio-clients-32.0.0rc2/tools/merge_rucio_configs.py`

 * *Files identical despite different names*

