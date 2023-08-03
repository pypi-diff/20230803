# Comparing `tmp/ciecplib-0.7.2.tar.gz` & `tmp/ciecplib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciecplib-0.7.2.tar", last modified: Thu Apr 20 11:23:18 2023, max compression
+gzip compressed data, was "ciecplib-0.8.0.tar", last modified: Thu Aug  3 17:47:24 2023, max compression
```

## Comparing `ciecplib-0.7.2.tar` & `ciecplib-0.8.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.609881 ciecplib-0.7.2/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2020-09-17 12:57:58.000000 ciecplib-0.7.2/LICENSE
--rw-r--r--   0 duncan    (1000) duncan    (1000)       80 2022-11-14 23:16:49.000000 ciecplib-0.7.2/MANIFEST.in
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2779 2023-04-20 11:23:18.609881 ciecplib-0.7.2/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1569 2023-02-14 15:31:52.000000 ciecplib-0.7.2/README.md
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.579881 ciecplib-0.7.2/ciecplib/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1121 2023-04-20 11:20:08.000000 ciecplib-0.7.2/ciecplib/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2531 2022-11-14 23:16:49.000000 ciecplib-0.7.2/ciecplib/conftest.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4156 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/cookies.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1852 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/env.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3589 2023-04-20 11:00:56.000000 ciecplib-0.7.2/ciecplib/kerberos.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1782 2022-11-14 20:46:26.000000 ciecplib-0.7.2/ciecplib/logging.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4114 2022-11-14 20:46:26.000000 ciecplib-0.7.2/ciecplib/requests.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2536 2023-02-14 15:17:22.000000 ciecplib-0.7.2/ciecplib/sessions.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.589881 ciecplib-0.7.2/ciecplib/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      814 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3808 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tests/test_cookies.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1181 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tests/test_env.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2490 2023-04-20 09:13:39.000000 ciecplib-0.7.2/ciecplib/tests/test_kerberos.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1116 2022-11-14 20:46:26.000000 ciecplib-0.7.2/ciecplib/tests/test_requests.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2204 2022-11-14 20:46:26.000000 ciecplib-0.7.2/ciecplib/tests/test_sessions.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4991 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tests/test_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6143 2022-11-15 15:28:45.000000 ciecplib-0.7.2/ciecplib/tests/test_x509.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.599881 ciecplib-0.7.2/ciecplib/tool/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      827 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tool/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5217 2023-04-20 11:00:56.000000 ciecplib-0.7.2/ciecplib/tool/ecp_cert_info.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3610 2022-11-14 20:46:26.000000 ciecplib-0.7.2/ciecplib/tool/ecp_curl.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5883 2022-11-15 13:27:59.000000 ciecplib-0.7.2/ciecplib/tool/ecp_get_cert.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5858 2022-11-14 20:46:26.000000 ciecplib-0.7.2/ciecplib/tool/ecp_get_cookie.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.599881 ciecplib-0.7.2/ciecplib/tool/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      819 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tool/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2010 2022-11-14 23:16:49.000000 ciecplib-0.7.2/ciecplib/tool/tests/test_common.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2309 2022-11-14 23:16:49.000000 ciecplib-0.7.2/ciecplib/tool/tests/test_ecp_cert_info.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3095 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tool/tests/test_ecp_curl.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2700 2022-11-14 23:16:49.000000 ciecplib-0.7.2/ciecplib/tool/tests/test_ecp_get_cert.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2688 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tool/tests/test_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8910 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/tool/utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5119 2022-11-14 23:16:49.000000 ciecplib-0.7.2/ciecplib/ui.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6961 2022-06-13 15:22:20.000000 ciecplib-0.7.2/ciecplib/utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    13419 2022-11-15 15:28:45.000000 ciecplib-0.7.2/ciecplib/x509.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.579881 ciecplib-0.7.2/ciecplib.egg-info/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2779 2023-04-20 11:23:18.000000 ciecplib-0.7.2/ciecplib.egg-info/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1341 2023-04-20 11:23:18.000000 ciecplib-0.7.2/ciecplib.egg-info/SOURCES.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-04-20 11:23:18.000000 ciecplib-0.7.2/ciecplib.egg-info/dependency_links.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      204 2023-04-20 11:23:18.000000 ciecplib-0.7.2/ciecplib.egg-info/entry_points.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      233 2023-04-20 11:23:18.000000 ciecplib-0.7.2/ciecplib.egg-info/requires.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        9 2023-04-20 11:23:18.000000 ciecplib-0.7.2/ciecplib.egg-info/top_level.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5282 2023-04-20 11:20:08.000000 ciecplib-0.7.2/ciecplib.spec
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.609881 ciecplib-0.7.2/debian/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3118 2023-04-20 11:20:08.000000 ciecplib-0.7.2/debian/changelog
--rw-r--r--   0 duncan    (1000) duncan    (1000)       31 2020-09-17 12:57:58.000000 ciecplib-0.7.2/debian/ciecp-utils.install
--rw-r--r--   0 duncan    (1000) duncan    (1000)        2 2020-09-17 12:57:58.000000 ciecplib-0.7.2/debian/compat
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1515 2023-04-20 09:13:39.000000 ciecplib-0.7.2/debian/control
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1040 2020-09-17 12:57:58.000000 ciecplib-0.7.2/debian/copyright
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.609881 ciecplib-0.7.2/debian/patches/
--rw-r--r--   0 duncan    (1000) duncan    (1000)       26 2022-11-14 23:16:49.000000 ciecplib-0.7.2/debian/patches/series
--rw-r--r--   0 duncan    (1000) duncan    (1000)      290 2022-11-14 23:16:49.000000 ciecplib-0.7.2/debian/patches/setup.cfg-pyopenssl.patch
--rw-r--r--   0 duncan    (1000) duncan    (1000)       29 2020-09-17 12:57:58.000000 ciecplib-0.7.2/debian/python3-ciecplib.install
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)      157 2022-11-14 23:16:49.000000 ciecplib-0.7.2/debian/rules
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:23:18.609881 ciecplib-0.7.2/debian/source/
--rw-r--r--   0 duncan    (1000) duncan    (1000)       12 2020-09-17 12:57:58.000000 ciecplib-0.7.2/debian/source/format
--rw-r--r--   0 duncan    (1000) duncan    (1000)      167 2022-06-13 15:22:20.000000 ciecplib-0.7.2/debian/watch
--rw-r--r--   0 duncan    (1000) duncan    (1000)      176 2022-11-15 12:53:44.000000 ciecplib-0.7.2/pyproject.toml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1997 2023-04-20 11:23:18.609881 ciecplib-0.7.2/setup.cfg
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1997 2022-11-15 14:40:17.000000 ciecplib-0.7.2/setup.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-08-03 17:47:24.649376 ciecplib-0.8.0/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2020-09-17 12:57:58.000000 ciecplib-0.8.0/LICENSE
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       80 2023-07-19 10:32:12.000000 ciecplib-0.8.0/MANIFEST.in
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2779 2023-08-03 17:47:24.649376 ciecplib-0.8.0/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1569 2023-07-19 10:32:12.000000 ciecplib-0.8.0/README.md
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-08-03 17:47:24.627709 ciecplib-0.8.0/ciecplib/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1121 2023-08-03 17:46:25.000000 ciecplib-0.8.0/ciecplib/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2531 2023-07-19 10:32:12.000000 ciecplib-0.8.0/ciecplib/conftest.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4156 2022-06-13 15:22:20.000000 ciecplib-0.8.0/ciecplib/cookies.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1852 2022-06-13 15:22:20.000000 ciecplib-0.8.0/ciecplib/env.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3645 2023-07-19 12:23:11.000000 ciecplib-0.8.0/ciecplib/kerberos.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1782 2022-11-14 20:46:26.000000 ciecplib-0.8.0/ciecplib/logging.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4114 2022-11-14 20:46:26.000000 ciecplib-0.8.0/ciecplib/requests.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2536 2023-02-14 15:17:22.000000 ciecplib-0.8.0/ciecplib/sessions.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-08-03 17:47:24.638542 ciecplib-0.8.0/ciecplib/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      814 2022-06-13 15:22:20.000000 ciecplib-0.8.0/ciecplib/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3808 2022-06-13 15:22:20.000000 ciecplib-0.8.0/ciecplib/tests/test_cookies.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1181 2022-06-13 15:22:20.000000 ciecplib-0.8.0/ciecplib/tests/test_env.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2873 2023-07-19 12:23:11.000000 ciecplib-0.8.0/ciecplib/tests/test_kerberos.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1140 2023-08-03 17:07:59.000000 ciecplib-0.8.0/ciecplib/tests/test_requests.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2204 2022-11-14 20:46:26.000000 ciecplib-0.8.0/ciecplib/tests/test_sessions.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4991 2022-06-13 15:22:20.000000 ciecplib-0.8.0/ciecplib/tests/test_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6143 2023-07-19 10:32:12.000000 ciecplib-0.8.0/ciecplib/tests/test_x509.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-08-03 17:47:24.638542 ciecplib-0.8.0/ciecplib/tool/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      827 2022-06-13 15:22:20.000000 ciecplib-0.8.0/ciecplib/tool/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5244 2023-08-03 17:07:59.000000 ciecplib-0.8.0/ciecplib/tool/ecp_cert_info.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3610 2022-11-14 20:46:26.000000 ciecplib-0.8.0/ciecplib/tool/ecp_curl.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5883 2023-07-19 10:32:12.000000 ciecplib-0.8.0/ciecplib/tool/ecp_get_cert.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5858 2022-11-14 20:46:26.000000 ciecplib-0.8.0/ciecplib/tool/ecp_get_cookie.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-08-03 17:47:24.638542 ciecplib-0.8.0/ciecplib/tool/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      819 2022-06-13 15:22:20.000000 ciecplib-0.8.0/ciecplib/tool/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2010 2023-07-19 10:32:12.000000 ciecplib-0.8.0/ciecplib/tool/tests/test_common.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2305 2023-08-03 17:07:59.000000 ciecplib-0.8.0/ciecplib/tool/tests/test_ecp_cert_info.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3095 2022-06-13 15:22:20.000000 ciecplib-0.8.0/ciecplib/tool/tests/test_ecp_curl.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2700 2023-07-19 10:32:12.000000 ciecplib-0.8.0/ciecplib/tool/tests/test_ecp_get_cert.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2688 2022-06-13 15:22:20.000000 ciecplib-0.8.0/ciecplib/tool/tests/test_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8910 2022-06-13 15:22:20.000000 ciecplib-0.8.0/ciecplib/tool/utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5119 2023-07-19 10:32:12.000000 ciecplib-0.8.0/ciecplib/ui.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6961 2022-06-13 15:22:20.000000 ciecplib-0.8.0/ciecplib/utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    13145 2023-07-19 12:23:11.000000 ciecplib-0.8.0/ciecplib/x509.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-08-03 17:47:24.627709 ciecplib-0.8.0/ciecplib.egg-info/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2779 2023-08-03 17:47:24.000000 ciecplib-0.8.0/ciecplib.egg-info/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1341 2023-08-03 17:47:24.000000 ciecplib-0.8.0/ciecplib.egg-info/SOURCES.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-08-03 17:47:24.000000 ciecplib-0.8.0/ciecplib.egg-info/dependency_links.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      204 2023-08-03 17:47:24.000000 ciecplib-0.8.0/ciecplib.egg-info/entry_points.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      240 2023-08-03 17:47:24.000000 ciecplib-0.8.0/ciecplib.egg-info/requires.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        9 2023-08-03 17:47:24.000000 ciecplib-0.8.0/ciecplib.egg-info/top_level.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5669 2023-08-03 17:46:25.000000 ciecplib-0.8.0/ciecplib.spec
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-08-03 17:47:24.649376 ciecplib-0.8.0/debian/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3296 2023-08-03 17:46:25.000000 ciecplib-0.8.0/debian/changelog
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       31 2020-09-17 12:57:58.000000 ciecplib-0.8.0/debian/ciecp-utils.install
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        2 2020-09-17 12:57:58.000000 ciecplib-0.8.0/debian/compat
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1617 2023-07-19 12:23:11.000000 ciecplib-0.8.0/debian/control
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1040 2020-09-17 12:57:58.000000 ciecplib-0.8.0/debian/copyright
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-08-03 17:47:24.649376 ciecplib-0.8.0/debian/patches/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       26 2023-07-19 10:32:12.000000 ciecplib-0.8.0/debian/patches/series
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      290 2023-07-19 10:32:12.000000 ciecplib-0.8.0/debian/patches/setup.cfg-pyopenssl.patch
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       29 2020-09-17 12:57:58.000000 ciecplib-0.8.0/debian/python3-ciecplib.install
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)      157 2023-07-19 10:32:12.000000 ciecplib-0.8.0/debian/rules
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-08-03 17:47:24.649376 ciecplib-0.8.0/debian/source/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       12 2020-09-17 12:57:58.000000 ciecplib-0.8.0/debian/source/format
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      167 2022-06-13 15:22:20.000000 ciecplib-0.8.0/debian/watch
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      596 2023-07-19 12:23:11.000000 ciecplib-0.8.0/pyproject.toml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2005 2023-08-03 17:47:24.649376 ciecplib-0.8.0/setup.cfg
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1997 2023-07-19 10:32:12.000000 ciecplib-0.8.0/setup.py
```

### Comparing `ciecplib-0.7.2/LICENSE` & `ciecplib-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/PKG-INFO` & `ciecplib-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciecplib
-Version: 0.7.2
+Version: 0.8.0
 Summary: A python client for SAML/ECP authentication
 Home-page: https://pypi.org/project/ciecplib
 Author: Duncan Macleod
 Author-email: duncan.macleod@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/duncanmmacleod/ciecplib/issues
 Project-URL: Documentation, https://ciecplib.readthedocs.io/
```

### Comparing `ciecplib-0.7.2/README.md` & `ciecplib-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/__init__.py` & `ciecplib-0.8.0/ciecplib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 from .ui import (
     get_cert,
     get_cookie,
 )
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
 __credits__ = "Scott Koranda, Dave Dykstra"
-__version__ = "0.7.2"
+__version__ = "0.8.0"
```

### Comparing `ciecplib-0.7.2/ciecplib/conftest.py` & `ciecplib-0.8.0/ciecplib/conftest.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/cookies.py` & `ciecplib-0.8.0/ciecplib/cookies.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/env.py` & `ciecplib-0.8.0/ciecplib/env.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/logging.py` & `ciecplib-0.8.0/ciecplib/logging.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/requests.py` & `ciecplib-0.8.0/ciecplib/requests.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/sessions.py` & `ciecplib-0.8.0/ciecplib/sessions.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tests/__init__.py` & `ciecplib-0.8.0/ciecplib/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tests/test_cookies.py` & `ciecplib-0.8.0/ciecplib/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tests/test_env.py` & `ciecplib-0.8.0/ciecplib/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tests/test_requests.py` & `ciecplib-0.8.0/ciecplib/tests/test_requests.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 
 
 def test_get(requests_mock):
     requests_mock.get("https://test.example.com", content=b"HELLO")
     assert ciecplib_requests.get(
         "https://test.example.com",
         endpoint="https://test.example.com/SOAP/ECP",
+        kerberos=False,
     ).text == "HELLO"
```

### Comparing `ciecplib-0.7.2/ciecplib/tests/test_sessions.py` & `ciecplib-0.8.0/ciecplib/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tests/test_utils.py` & `ciecplib-0.8.0/ciecplib/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tests/test_x509.py` & `ciecplib-0.8.0/ciecplib/tests/test_x509.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tool/__init__.py` & `ciecplib-0.8.0/ciecplib/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tool/ecp_cert_info.py` & `ciecplib-0.8.0/ciecplib/tool/ecp_cert_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -199,16 +199,16 @@
         cert,
         path=args.file,
         display=getattr(args, "display", None),
         verbose=args.verbose,
         stream=sys.stdout,
     )
 
-    # assert --valid if given
-    if args.valid:
-        assert isvalid, (
+    # check credential validity if given
+    if args.valid and not isvalid:
+        raise ValueError(
             f"timeleft ({remaining}) is less than required ({valid})"
         )
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `ciecplib-0.7.2/ciecplib/tool/ecp_curl.py` & `ciecplib-0.8.0/ciecplib/tool/ecp_curl.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tool/ecp_get_cert.py` & `ciecplib-0.8.0/ciecplib/tool/ecp_get_cert.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tool/ecp_get_cookie.py` & `ciecplib-0.8.0/ciecplib/tool/ecp_get_cookie.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tool/tests/__init__.py` & `ciecplib-0.8.0/ciecplib/tool/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tool/tests/test_common.py` & `ciecplib-0.8.0/ciecplib/tool/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tool/tests/test_ecp_cert_info.py` & `ciecplib-0.8.0/ciecplib/tool/tests/test_ecp_cert_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     f"{ecp_cert_info.__name__}.time_left",
     mock.Mock(side_effect=(3700., 3500.)),
 )
 def test_valid():
     """Check that the --valid option for ecp-cert-info works
     """
     ecp_cert_info.main(["--valid", "1:0"])
-    with pytest.raises(AssertionError):
+    with pytest.raises(ValueError):
         ecp_cert_info.main(["--valid", "1:0"])
 
 
 @mock.patch(f"{ecp_cert_info.__name__}.load_cert")
 def test_main(load_cert, capsys, x509):
     load_cert.return_value = x509
     ecp_cert_info.main([])
```

### Comparing `ciecplib-0.7.2/ciecplib/tool/tests/test_ecp_curl.py` & `ciecplib-0.8.0/ciecplib/tool/tests/test_ecp_curl.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tool/tests/test_ecp_get_cert.py` & `ciecplib-0.8.0/ciecplib/tool/tests/test_ecp_get_cert.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tool/tests/test_utils.py` & `ciecplib-0.8.0/ciecplib/tool/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/tool/utils.py` & `ciecplib-0.8.0/ciecplib/tool/utils.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/ui.py` & `ciecplib-0.8.0/ciecplib/ui.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/utils.py` & `ciecplib-0.8.0/ciecplib/utils.py`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib/x509.py` & `ciecplib-0.8.0/ciecplib/x509.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with ciecplib.  If not, see <http://www.gnu.org/licenses/>.
 
 import calendar
 import datetime
 import shutil
-import struct
 import sys
 import tempfile
 import time
 
 from cryptography import x509 as crypto_x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric.rsa import generate_private_key
 from cryptography.hazmat.primitives.serialization import (
     Encoding,
     NoEncryption,
     PrivateFormat,
-    PublicFormat,
 )
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
 
 PROXY_CERT_INFO_EXT_OID = crypto_x509.ObjectIdentifier("1.3.6.1.5.5.7.1.14")
 
 # backport short names for cryptography < 2.5
@@ -356,23 +354,15 @@
         public_exponent=65537,
         key_size=bits,
         backend=default_backend(),
     )
     proxy_public_key = proxy_private_key.public_key()
 
     # create a serial number for the proxy
-    digest = hashes.Hash(hashes.SHA256(), backend=default_backend())
-    digest.update(proxy_public_key.public_bytes(
-        encoding=Encoding.DER,
-        format=PublicFormat.PKCS1,
-    ))
-    serial = int(
-        struct.unpack("<L", digest.finalize()[:4])[0]
-        & 0x7fffffff
-    )
+    serial = crypto_x509.random_serial_number()
 
     # generate a new subject by appending the serial number to
     # the subject of the original certificate
     proxy_subject = crypto_x509.Name(
         list(cert.subject) + [
             crypto_x509.NameAttribute(
                 crypto_x509.NameOID.COMMON_NAME,
```

### Comparing `ciecplib-0.7.2/ciecplib.egg-info/PKG-INFO` & `ciecplib-0.8.0/ciecplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciecplib
-Version: 0.7.2
+Version: 0.8.0
 Summary: A python client for SAML/ECP authentication
 Home-page: https://pypi.org/project/ciecplib
 Author: Duncan Macleod
 Author-email: duncan.macleod@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/duncanmmacleod/ciecplib/issues
 Project-URL: Documentation, https://ciecplib.readthedocs.io/
```

### Comparing `ciecplib-0.7.2/ciecplib.egg-info/SOURCES.txt` & `ciecplib-0.8.0/ciecplib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/ciecplib.spec` & `ciecplib-0.8.0/ciecplib.spec`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 %define srcname ciecplib
-%define version 0.7.2
+%define version 0.8.0
 %define release 1
 
 # -- metadata ---------------
 
 Name:      %{srcname}
 Version:   %{version}
 Release:   %{release}%{?dist}
@@ -22,15 +22,15 @@
 # -- build requirements -----
 
 # macros
 BuildRequires: python-rpm-macros
 BuildRequires: python3-rpm-macros
 
 # build
-BuildRequires: python3 >= 3.6.0
+BuildRequires: python3-devel >= 3.6.0
 BuildRequires: python%{python3_pkgversion}-setuptools >= 30.3.0
 BuildRequires: python%{python3_pkgversion}-wheel
 
 # man pages
 %if 0%{?fedora} >= 26 || 0%{?rhel} >= 8
 BuildRequires: python%{python3_pkgversion}-argparse-manpage
 %endif
@@ -42,14 +42,15 @@
 %endif
 BuildRequires: python%{python3_pkgversion}-requests
 BuildRequires: python%{python3_pkgversion}-requests-ecp
 
 # tests
 %if 0%{?fedora} >= 30 || 0%{?rhel} >= 9
 BuildRequires: python%{python3_pkgversion}-pytest >= 3.9.0
+BuildRequires: python%{python3_pkgversion}-requests-mock
 %endif
 
 # -- packages ---------------
 
 # src.rpm
 %description
 The Python client for SAML ECP authentication.
@@ -61,14 +62,18 @@
 %else
 Requires: python%{python3_pkgversion}-cryptography
 Requires: python%{python3_pkgversion}-pyOpenSSL >= 17.1.0
 %endif
 Requires: python%{python3_pkgversion}-requests
 Requires: python%{python3_pkgversion}-requests-ecp
 Conflicts: ciecp-utils < 0.4.3-1
+%if 0%{?fedora} >= 36 || 0%{?rhel} >= 8
+Recommends: python%{python3_pkgversion}-gssapi
+Recommends: python%{python3_pkgversion}-requests-gssapi
+%endif
 %{?python_provide:%python_provide python%{python3_pkgversion}-%{srcname}}
 %description -n python%{python3_pkgversion}-%{srcname}
 The Python %{python3_version} client for SAML ECP authentication.
 
 %package -n ciecp-utils
 Summary: Command line utilities for SAML ECP authentication
 Requires: python%{python3_pkgversion}-%{srcname} = %{version}-%{release}
@@ -98,15 +103,15 @@
 export PYTHONPATH="%{buildroot}%{python3_sitelib}"
 export PATH="%{buildroot}%{_bindir}:${PATH}"
 ecp-cert-info --help
 ecp-curl --help
 ecp-get-cert --help
 ecp-get-cookie --help
 %if 0%{?fedora} >= 30 || 0%{?rhel} >= 9
-%{__python3} -m pytest %{?_pytest_options}%{?!_pytest_options:--verbose -ra --pyargs requests_ecp}
+%{__python3} -m pytest --verbose -ra --pyargs ciecplib
 %endif
 
 %clean
 rm -rf $RPM_BUILD_ROOT
 
 # -- files ------------------
 
@@ -122,14 +127,20 @@
 %if 0%{?fedora} >= 26 || 0%{?rhel} >= 8
 %{_mandir}/man1/*.1*
 %endif
 
 # -- changelog --------------
 
 %changelog
+* Thu Aug 03 2023 Duncan Macleod <duncan.macleod@ligo.org> - 0.8.0-1
+- update for 0.8.0
+- add python3-devel build requirement
+- add python3-gssapi requirement
+- add python3-requests-mock build requirement for testing
+
 * Thu Apr 20 2023 Duncan Macleod <duncan.macleod@ligo.org> - 0.7.2-1
 - update for 0.7.2
 
 * Tue Nov 15 2022 Duncan Macleod <duncan.macleod@ligo.org> - 0.7.1-1
 - update for 0.7.1
 
 * Wed Nov 02 2022 Duncan Macleod <duncan.macleod@ligo.org> - 0.7.0-2
```

### Comparing `ciecplib-0.7.2/debian/changelog` & `ciecplib-0.8.0/debian/changelog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+ciecplib (0.8.0-1) unstable; urgency=low
+
+  * Update for 0.8.0
+  * Add python3-gssapi requirement
+
+ -- Duncan Macleod <duncan.macleod@ligo.org>  Thu, 03 Aug 2023 18:11:00 +0100
+
 ciecplib (0.7.2-1) unstable; urgency=low
 
   * Update for 0.7.2
 
  -- Duncan Macleod <duncan.macleod@ligo.org>  Thu, 20 Apr 2023 12:02:00 +0100
 
 ciecplib (0.7.1-1) unstable; urgency=low
```

### Comparing `ciecplib-0.7.2/debian/control` & `ciecplib-0.8.0/debian/control`

 * *Files 9% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 Homepage: https://github.com/duncanmmacleod/ciecplib
 Build-Depends:
  debhelper (>= 9),
  dh-python,
  python3-all,
  python3-argparse-manpage,
  python3-cryptography,
+ python3-gssapi,
  python3-openssl (>=17.1.0),
- python3-importlib-metadata | python3-minimal (<< 3.9.0),
+ python3-importlib-metadata | python3-minimal (>= 3.8.0),
  python3-pytest,
  python3-requests,
  python3-requests-ecp,
+ python3-requests-kerberos,
  python3-requests-mock,
  python3-setuptools (>= 30.3.0),
 
 # -- python3-ciecplib ---------------------------------------------------------
 # requires buster-backports or newer
 
 Package: python3-ciecplib
@@ -29,14 +31,17 @@
 Depends:
  ${misc:Depends},
  ${python3:Depends},
  python3-cryptography,
  python3-openssl (>=17.1.0),
  python3-requests,
  python3-requests-ecp,
+Recommends:
+ python3-gssapi,
+ python3-requests-kerberos,
 Description: Python client for SAML/ECP authentication and HTTP requests
  CIECPLib provides Python-based utilities for SAML/ECP authentication
  and HTTP requests.
  .
  This package provides the Python 3 library.
 
 # -- ciecp-utils --------------------------------------------------------------
```

### Comparing `ciecplib-0.7.2/debian/copyright` & `ciecplib-0.8.0/debian/copyright`

 * *Files identical despite different names*

### Comparing `ciecplib-0.7.2/setup.cfg` & `ciecplib-0.8.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 docs = 
 	sphinx
 	sphinx-argparse
 	sphinx-automodapi
 	sphinx_rtd_theme
 	sphinx-tabs
 kerberos = 
+	gssapi
 	requests-ecp[kerberos]
 manpages = 
 	argparse-manpage
 tests = 
 	pytest >= 3.9.0
 	pytest-cov
 	requests-mock
```

### Comparing `ciecplib-0.7.2/setup.py` & `ciecplib-0.8.0/setup.py`

 * *Files identical despite different names*

