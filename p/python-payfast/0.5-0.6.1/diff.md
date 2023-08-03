# Comparing `tmp/python-payfast-0.5.tar.gz` & `tmp/python-payfast-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-payfast-0.5.tar", last modified: Thu Jul 13 15:09:26 2023, max compression
+gzip compressed data, was "python-payfast-0.6.1.tar", last modified: Thu Aug  3 12:48:15 2023, max compression
```

## Comparing `python-payfast-0.5.tar` & `python-payfast-0.6.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.181051 python-payfast-0.5/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-06-06 20:50:53.000000 python-payfast-0.5/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       72 2023-06-12 19:59:05.000000 python-payfast-0.5/MANIFEST.in
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      790 2023-07-13 15:09:26.177051 python-payfast-0.5/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      143 2023-07-12 09:54:32.000000 python-payfast-0.5/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.173051 python-payfast-0.5/payfast/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2441 2023-07-13 15:08:36.000000 python-payfast-0.5/payfast/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.173051 python-payfast-0.5/payfast/api/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-07 11:51:53.000000 python-payfast-0.5/payfast/api/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      533 2023-06-21 18:57:35.000000 python-payfast-0.5/payfast/api/refunds.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    27368 2023-07-13 14:36:03.000000 python-payfast-0.5/payfast/api/subscriptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     8005 2023-06-21 18:48:00.000000 python-payfast-0.5/payfast/api/transactions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      566 2023-06-12 19:22:21.000000 python-payfast-0.5/payfast/apps.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6242 2023-07-13 15:00:50.000000 python-payfast-0.5/payfast/base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2614 2023-07-12 07:27:56.000000 python-payfast-0.5/payfast/callbacks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7301 2023-07-13 15:08:13.000000 python-payfast-0.5/payfast/conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1210 2023-07-10 13:24:31.000000 python-payfast-0.5/payfast/constants.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2188 2023-07-10 14:27:12.000000 python-payfast-0.5/payfast/decorators.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1908 2023-06-21 19:24:26.000000 python-payfast-0.5/payfast/exceptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    11812 2023-07-10 14:13:51.000000 python-payfast-0.5/payfast/itn.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      251 2023-06-21 18:47:03.000000 python-payfast-0.5/payfast/logging.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    15833 2023-07-13 13:57:00.000000 python-payfast-0.5/payfast/payment.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2111 2023-06-08 18:38:43.000000 python-payfast-0.5/payfast/security_checks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     3308 2023-07-13 13:57:13.000000 python-payfast-0.5/payfast/serialization.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      376 2023-06-19 18:50:19.000000 python-payfast-0.5/payfast/signals.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2761 2023-06-15 13:28:20.000000 python-payfast-0.5/payfast/signature.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.169051 python-payfast-0.5/payfast/templates/
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.173051 python-payfast-0.5/payfast/templates/payfast/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      285 2023-07-10 12:50:03.000000 python-payfast-0.5/payfast/templates/payfast/form.html
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      299 2023-06-12 20:32:31.000000 python-payfast-0.5/payfast/templates/payfast/sandbox.html
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      419 2023-07-10 12:49:49.000000 python-payfast-0.5/payfast/templates.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      544 2023-06-14 16:50:45.000000 python-payfast-0.5/payfast/timezone.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      618 2023-06-13 13:20:57.000000 python-payfast-0.5/payfast/urls.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     4071 2023-07-12 08:10:34.000000 python-payfast-0.5/payfast/utils.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1577 2023-07-12 08:09:37.000000 python-payfast-0.5/payfast/validation.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     5009 2023-07-10 13:58:41.000000 python-payfast-0.5/payfast/views.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.177051 python-payfast-0.5/python_payfast.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      790 2023-07-13 15:09:26.000000 python-payfast-0.5/python_payfast.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1215 2023-07-13 15:09:26.000000 python-payfast-0.5/python_payfast.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-07-13 15:09:26.000000 python-payfast-0.5/python_payfast.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      102 2023-07-13 15:09:26.000000 python-payfast-0.5/python_payfast.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-07-13 15:09:26.000000 python-payfast-0.5/python_payfast.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-07-13 15:09:26.181051 python-payfast-0.5/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1804 2023-06-15 12:19:47.000000 python-payfast-0.5/setup.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.177051 python-payfast-0.5/tests/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-06 18:42:13.000000 python-payfast-0.5/tests/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-07-13 15:09:26.177051 python-payfast-0.5/tests/api/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:55:21.000000 python-payfast-0.5/tests/api/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      436 2023-06-12 18:51:32.000000 python-payfast-0.5/tests/api/test_subscriptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      563 2023-06-12 18:11:31.000000 python-payfast-0.5/tests/api/test_transactions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:58.000000 python-payfast-0.5/tests/test_base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:53.000000 python-payfast-0.5/tests/test_callbacks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:58.000000 python-payfast-0.5/tests/test_conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:35.000000 python-payfast-0.5/tests/test_constants.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:02:08.000000 python-payfast-0.5/tests/test_exceptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1541 2023-07-12 09:51:05.000000 python-payfast-0.5/tests/test_itn.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      300 2023-06-12 18:51:58.000000 python-payfast-0.5/tests/test_payfast.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      431 2023-06-12 19:22:34.000000 python-payfast-0.5/tests/test_payment.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:36.000000 python-payfast-0.5/tests/test_security_checks.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:46.000000 python-payfast-0.5/tests/test_signature.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:05.000000 python-payfast-0.5/tests/test_templates.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:20.000000 python-payfast-0.5/tests/test_timezone.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:26.000000 python-payfast-0.5/tests/test_utils.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 12:48:15.155122 python-payfast-0.6.1/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-06-06 20:50:53.000000 python-payfast-0.6.1/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       72 2023-06-12 19:59:05.000000 python-payfast-0.6.1/MANIFEST.in
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      792 2023-08-03 12:48:15.155122 python-payfast-0.6.1/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      143 2023-07-12 09:54:32.000000 python-payfast-0.6.1/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 12:48:14.999120 python-payfast-0.6.1/payfast/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2443 2023-08-03 12:46:46.000000 python-payfast-0.6.1/payfast/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 12:48:15.027120 python-payfast-0.6.1/payfast/api/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-07 11:51:53.000000 python-payfast-0.6.1/payfast/api/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      533 2023-06-21 18:57:35.000000 python-payfast-0.6.1/payfast/api/refunds.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    27524 2023-08-03 12:26:57.000000 python-payfast-0.6.1/payfast/api/subscriptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     8005 2023-08-03 07:45:23.000000 python-payfast-0.6.1/payfast/api/transactions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      566 2023-06-12 19:22:21.000000 python-payfast-0.6.1/payfast/apps.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7038 2023-08-03 12:32:24.000000 python-payfast-0.6.1/payfast/base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2614 2023-07-12 07:27:56.000000 python-payfast-0.6.1/payfast/callbacks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7295 2023-08-03 12:43:54.000000 python-payfast-0.6.1/payfast/conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1210 2023-07-10 13:24:31.000000 python-payfast-0.6.1/payfast/constants.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2188 2023-07-10 14:27:12.000000 python-payfast-0.6.1/payfast/decorators.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1908 2023-08-03 11:36:37.000000 python-payfast-0.6.1/payfast/exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    11812 2023-07-10 14:13:51.000000 python-payfast-0.6.1/payfast/itn.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      251 2023-07-20 08:00:37.000000 python-payfast-0.6.1/payfast/logging.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    15833 2023-08-02 08:28:02.000000 python-payfast-0.6.1/payfast/payment.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2111 2023-06-08 18:38:43.000000 python-payfast-0.6.1/payfast/security_checks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     3308 2023-07-13 13:57:13.000000 python-payfast-0.6.1/payfast/serialization.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      376 2023-06-19 18:50:19.000000 python-payfast-0.6.1/payfast/signals.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2761 2023-06-15 13:28:20.000000 python-payfast-0.6.1/payfast/signature.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 12:48:14.991120 python-payfast-0.6.1/payfast/templates/
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 12:48:15.051120 python-payfast-0.6.1/payfast/templates/payfast/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      285 2023-07-10 12:50:03.000000 python-payfast-0.6.1/payfast/templates/payfast/form.html
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      299 2023-06-12 20:32:31.000000 python-payfast-0.6.1/payfast/templates/payfast/sandbox.html
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      419 2023-07-10 12:49:49.000000 python-payfast-0.6.1/payfast/templates.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      544 2023-06-14 16:50:45.000000 python-payfast-0.6.1/payfast/timezone.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      618 2023-06-13 13:20:57.000000 python-payfast-0.6.1/payfast/urls.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     4071 2023-07-12 08:10:34.000000 python-payfast-0.6.1/payfast/utils.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1577 2023-07-12 08:09:37.000000 python-payfast-0.6.1/payfast/validation.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     5009 2023-07-10 13:58:41.000000 python-payfast-0.6.1/payfast/views.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 12:48:15.071121 python-payfast-0.6.1/python_payfast.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      792 2023-08-03 12:48:14.000000 python-payfast-0.6.1/python_payfast.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1215 2023-08-03 12:48:14.000000 python-payfast-0.6.1/python_payfast.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-08-03 12:48:14.000000 python-payfast-0.6.1/python_payfast.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      102 2023-08-03 12:48:14.000000 python-payfast-0.6.1/python_payfast.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-08-03 12:48:14.000000 python-payfast-0.6.1/python_payfast.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-08-03 12:48:15.155122 python-payfast-0.6.1/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1804 2023-06-15 12:19:47.000000 python-payfast-0.6.1/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 12:48:15.119121 python-payfast-0.6.1/tests/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-06 18:42:13.000000 python-payfast-0.6.1/tests/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 12:48:15.131121 python-payfast-0.6.1/tests/api/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:55:21.000000 python-payfast-0.6.1/tests/api/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      436 2023-06-12 18:51:32.000000 python-payfast-0.6.1/tests/api/test_subscriptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      563 2023-06-12 18:11:31.000000 python-payfast-0.6.1/tests/api/test_transactions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:58.000000 python-payfast-0.6.1/tests/test_base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:53.000000 python-payfast-0.6.1/tests/test_callbacks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:57:58.000000 python-payfast-0.6.1/tests/test_conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:35.000000 python-payfast-0.6.1/tests/test_constants.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:02:08.000000 python-payfast-0.6.1/tests/test_exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1541 2023-07-12 09:51:05.000000 python-payfast-0.6.1/tests/test_itn.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      300 2023-06-12 18:51:58.000000 python-payfast-0.6.1/tests/test_payfast.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      431 2023-06-12 19:22:34.000000 python-payfast-0.6.1/tests/test_payment.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:36.000000 python-payfast-0.6.1/tests/test_security_checks.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 16:01:46.000000 python-payfast-0.6.1/tests/test_signature.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:58:05.000000 python-payfast-0.6.1/tests/test_templates.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:20.000000 python-payfast-0.6.1/tests/test_timezone.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-06-12 15:56:26.000000 python-payfast-0.6.1/tests/test_utils.py
```

### Comparing `python-payfast-0.5/LICENSE` & `python-payfast-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/PKG-INFO` & `python-payfast-0.6.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-payfast
-Version: 0.5
+Version: 0.6.1
 Summary: A very opinionated Python client library for the PayFast API.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `python-payfast-0.5/payfast/__init__.py` & `python-payfast-0.6.1/payfast/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from payfast.api.subscriptions import Subscriptions, Cards
 from payfast.api.transactions import Transactions, CCTransactions
 from payfast.api.refunds import Refunds
 
 
 
 
-__version__ = '0.5'
+__version__ = '0.6.1'
 __title__ = 'python-payfast'
 
 
 
 
 class PayFast:
```

### Comparing `python-payfast-0.5/payfast/api/refunds.py` & `python-payfast-0.6.1/payfast/api/refunds.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/api/subscriptions.py` & `python-payfast-0.6.1/payfast/api/subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -840,15 +840,20 @@
                 "data": {
                     "response": 4,
                     "message": "The subscription is not in a valid state."
                 }
             }
         """
         amount_cents = int(amount * 100)
+        logger.info(f'Charging card "{token}" with {amount_cents} cents.')
         uri = urljoin([self.uri, token, 'adhoc'])
+        if itn:
+            itn = 'true'
+        else:
+            itn = 'false'
         _payload = {
             'amount': amount_cents,
             'item_name': item_name,
             'item_description': item_description,
             'itn': itn,
             'm_payment_id': m_payment_id,
             'cc_cvv': cc_cvv,
```

### Comparing `python-payfast-0.5/payfast/api/transactions.py` & `python-payfast-0.6.1/payfast/api/transactions.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/apps.py` & `python-payfast-0.6.1/payfast/apps.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/base.py` & `python-payfast-0.6.1/payfast/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 from datetime import datetime
 from urllib.parse import urljoin
+import urllib.parse
 
 import requests
 
 from payfast import timezone
 from payfast.conf import settings
 from payfast.signature import make_signature
 from payfast.exceptions import PayFastAPIException, PayFastTimeout
@@ -111,57 +112,72 @@
         self,
         method,
         uri,
         payload=None,
         params=None,
         headers=None,
         raise_for_status=True,
+        urlencode=False,
         **kwargs
     ):
         if not headers:
             for_headers = payload or params
-            headers = self.get_headers(for_headers)
+            content_type = None
+            if method.lower() != 'get':
+                content_type = 'application/json'
+                if urlencode:
+                    content_type = 'application/x-www-form-urlencoded'
+            headers = self.get_headers(for_headers, content_type=content_type)
 
         if settings.DEBUG:
-            uri += '/?testing=true'
+            # NOTE: Do not use ``uri += '/?testing=true'`` (no forward slash)
+            # as that will result in a redirect which will cause the request
+            # to fail with a 405 Method Not Allowed status.
+            uri += '?testing=true'
 
         request_args = {
             'method': method,
             'url': uri,
             'headers': headers,
         }
         if payload:
-            payload = json.dumps(payload)
+            if urlencode:
+                payload = urllib.parse.urlencode(payload)
+            else:
+                payload = json.dumps(payload)
             request_args['data'] = payload
 
         elif params:
             request_args['params'] = params
 
         logger.debug(json.dumps(request_args, indent=4))
 
         req = requests.Request(**request_args)
         req = req.prepare()
-
         response = None
         try:
-            response = self.session.send(req, timeout=settings.API_TIMEOUT)
+            response = self.session.send(
+                req,
+                timeout=settings.API_TIMEOUT,
+                allow_redirects=False,
+            )
         except (
             requests.ConnectionError,
             requests.Timeout
         ):
             raise PayFastTimeout()
 
         response = self.handle_response(
             response,
             raise_for_status=raise_for_status,
         )
         return response
 
 
-    def get_headers(self, payload):
+    def get_headers(self, payload, content_type=None):
         # There's a bug on PayFast's API where they don't account
         # for microseconds which means that using datetime.isoformat()
         # will not work.
         # timestamp = timezone.now().isoformat()
         timestamp = timezone.now()
         timestamp = timestamp.strftime('%Y-%m-%dT%H:%M:%S')
         headers = {
@@ -176,14 +192,17 @@
                     **headers,
                     **payload,
                 }
             elif isinstance(payload, str):
                 for_signature['payload'] = payload
         signature = make_signature(for_signature, a12y=True)
         headers['signature'] = signature
+
+        if content_type:
+            headers['content-type'] = content_type
         return headers
 
 
 
 
 class Resource:
```

### Comparing `python-payfast-0.5/payfast/callbacks.py` & `python-payfast-0.6.1/payfast/callbacks.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/conf.py` & `python-payfast-0.6.1/payfast/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,17 +69,17 @@
 
 
 class Settings:
 
     DEBUG = config('PAYFAST_DEBUG', cast=bool, default=True)
     USE_PAYFAST_SANDBOX = DEBUG
 
-    DEFAULT_MERCHANT_ID = 10005195
-    DEFAULT_MERCHANT_KEY = 'cfd5vff7cvxpp'
-    DEFAULT_SALT_PASSPHRASE = '123456789A_bcdefgh'
+    DEFAULT_MERCHANT_ID = 10030202
+    DEFAULT_MERCHANT_KEY = '4fkhqhutgnkhj'
+    DEFAULT_SALT_PASSPHRASE = 'testing12345'
 
     PAYFAST_HOST = None
     PROCESS_URL = None
     if USE_PAYFAST_SANDBOX:
         PAYFAST_HOST = 'sandbox.payfast.co.za'
     else:
         PAYFAST_HOST = 'www.payfast.co.za'
```

### Comparing `python-payfast-0.5/payfast/constants.py` & `python-payfast-0.6.1/payfast/constants.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/decorators.py` & `python-payfast-0.6.1/payfast/decorators.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/exceptions.py` & `python-payfast-0.6.1/payfast/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/itn.py` & `python-payfast-0.6.1/payfast/itn.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/payment.py` & `python-payfast-0.6.1/payfast/payment.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/security_checks.py` & `python-payfast-0.6.1/payfast/security_checks.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/serialization.py` & `python-payfast-0.6.1/payfast/serialization.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/signature.py` & `python-payfast-0.6.1/payfast/signature.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/timezone.py` & `python-payfast-0.6.1/payfast/timezone.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/urls.py` & `python-payfast-0.6.1/payfast/urls.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/utils.py` & `python-payfast-0.6.1/payfast/utils.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/validation.py` & `python-payfast-0.6.1/payfast/validation.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/payfast/views.py` & `python-payfast-0.6.1/payfast/views.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/python_payfast.egg-info/PKG-INFO` & `python-payfast-0.6.1/python_payfast.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-payfast
-Version: 0.5
+Version: 0.6.1
 Summary: A very opinionated Python client library for the PayFast API.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `python-payfast-0.5/python_payfast.egg-info/SOURCES.txt` & `python-payfast-0.6.1/python_payfast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/setup.py` & `python-payfast-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/tests/api/test_transactions.py` & `python-payfast-0.6.1/tests/api/test_transactions.py`

 * *Files identical despite different names*

### Comparing `python-payfast-0.5/tests/test_itn.py` & `python-payfast-0.6.1/tests/test_itn.py`

 * *Files identical despite different names*

