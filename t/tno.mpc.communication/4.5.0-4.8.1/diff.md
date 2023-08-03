# Comparing `tmp/tno.mpc.communication-4.5.0.tar.gz` & `tmp/tno.mpc.communication-4.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tno.mpc.communication-4.5.0.tar", last modified: Mon May  8 14:04:43 2023, max compression
+gzip compressed data, was "tno.mpc.communication-4.8.1.tar", last modified: Thu Aug  3 09:49:22 2023, max compression
```

## Comparing `tno.mpc.communication-4.5.0.tar` & `tno.mpc.communication-4.8.1.tar`

### file list

```diff
@@ -1,63 +1,71 @@
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-08 14:04:43.447090 tno.mpc.communication-4.5.0/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      641 2023-05-08 08:50:39.000000 tno.mpc.communication-4.5.0/CITATION.cff
--rw-r--r--   0 thomas    (1000) thomas    (1000)    11401 2023-05-08 09:06:41.000000 tno.mpc.communication-4.5.0/LICENSE
--rw-r--r--   0 thomas    (1000) thomas    (1000)    16250 2023-05-08 14:04:43.447090 tno.mpc.communication-4.5.0/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)    15156 2023-05-08 09:35:32.000000 tno.mpc.communication-4.5.0/README.md
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1803 2023-05-08 09:02:49.000000 tno.mpc.communication-4.5.0/pyproject.toml
--rw-r--r--   0 thomas    (1000) thomas    (1000)       38 2023-05-08 14:04:43.447090 tno.mpc.communication-4.5.0/setup.cfg
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-08 14:04:43.417090 tno.mpc.communication-4.5.0/src/
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-08 14:04:43.417090 tno.mpc.communication-4.5.0/src/tno/
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-08 14:04:43.417090 tno.mpc.communication-4.5.0/src/tno/mpc/
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-08 14:04:43.427090 tno.mpc.communication-4.5.0/src/tno/mpc/communication/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1070 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      385 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/exceptions.py
--rwxr-xr-x   0 thomas    (1000) thomas    (1000)     1342 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/functions.py
--rwxr-xr-x   0 thomas    (1000) thomas    (1000)    15980 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/httphandlers.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    19918 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/pool.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/py.typed
--rw-r--r--   0 thomas    (1000) thomas    (1000)    21434 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/serialization.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-08 14:04:43.427090 tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      325 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1022 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/_register.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1147 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/bitarray.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1467 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/gmpy.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      910 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/int.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1813 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/numpy.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5727 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/pandas.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      984 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/tuple.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-08 14:04:43.437090 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1435 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      878 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/conftest.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7225 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/pool_fixtures_http.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    26310 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/test_packing.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2340 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/test_packing_gmpy.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2423 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/test_pool_creation.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    12505 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/test_pool_http_2p.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    12307 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/test_pool_http_3p.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1843 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/test_pool_https_3p.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-08 14:04:43.447090 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      102 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/README.md
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7985 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/ca-combined.crt
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3999 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/ca-intermediate.crt
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1704 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/ca-intermediate.pem
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3986 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/ca-root.crt
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1704 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/ca-root.pem
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3588 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_0.crt
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1704 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_0.pem
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3588 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_1.crt
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1704 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_1.pem
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3588 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_2.crt
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1704 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_2.pem
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3588 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_3.crt
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1704 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_3.pem
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3588 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_4.crt
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1708 2023-05-08 08:49:03.000000 tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_4.pem
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-08 14:04:43.427090 tno.mpc.communication-4.5.0/src/tno.mpc.communication.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)    16250 2023-05-08 14:04:43.000000 tno.mpc.communication-4.5.0/src/tno.mpc.communication.egg-info/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2348 2023-05-08 14:04:43.000000 tno.mpc.communication-4.5.0/src/tno.mpc.communication.egg-info/SOURCES.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-05-08 14:04:43.000000 tno.mpc.communication-4.5.0/src/tno.mpc.communication.egg-info/dependency_links.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)      372 2023-05-08 14:04:43.000000 tno.mpc.communication-4.5.0/src/tno.mpc.communication.egg-info/requires.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        4 2023-05-08 14:04:43.000000 tno.mpc.communication-4.5.0/src/tno.mpc.communication.egg-info/top_level.txt
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-08 14:04:43.447090 tno.mpc.communication-4.5.0/stubs/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      773 2023-05-08 09:09:55.000000 tno.mpc.communication-4.5.0/stubs/gmpy2.pyi
--rw-r--r--   0 thomas    (1000) thomas    (1000)       35 2023-05-08 09:09:55.000000 tno.mpc.communication-4.5.0/stubs/pyarrow.pyi
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.517544 tno.mpc.communication-4.8.1/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      680 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/CITATION.cff
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    11401 2023-05-08 14:06:58.000000 tno.mpc.communication-4.8.1/LICENSE
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    19026 2023-08-03 09:49:22.517544 tno.mpc.communication-4.8.1/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    17928 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/README.md
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       91 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/entry_points.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1836 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/pyproject.toml
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       38 2023-08-03 09:49:22.517544 tno.mpc.communication-4.8.1/setup.cfg
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.497544 tno.mpc.communication-4.8.1/src/
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.497544 tno.mpc.communication-4.8.1/src/pytest_tno/
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.497544 tno.mpc.communication-4.8.1/src/pytest_tno/tno/
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.497544 tno.mpc.communication-4.8.1/src/pytest_tno/tno/mpc/
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.507544 tno.mpc.communication-4.8.1/src/pytest_tno/tno/mpc/communication/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      319 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/pytest_tno/tno/mpc/communication/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/pytest_tno/tno/mpc/communication/py.typed
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     9910 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/pytest_tno/tno/mpc/communication/pytest_pool_fixtures.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.507544 tno.mpc.communication-4.8.1/src/pytest_tno/tno/mpc/communication/test/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1333 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/pytest_tno/tno/mpc/communication/test/test_fixtures.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.497544 tno.mpc.communication-4.8.1/src/tno/
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.497544 tno.mpc.communication-4.8.1/src/tno/mpc/
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.507544 tno.mpc.communication-4.8.1/src/tno/mpc/communication/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      943 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      385 2023-08-01 13:01:08.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/exceptions.py
+-rwxr-xr-x   0 thomas    (1000) thomas    (1000)     1342 2023-08-01 13:01:08.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/functions.py
+-rwxr-xr-x   0 thomas    (1000) thomas    (1000)    16106 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/httphandlers.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    20566 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/pool.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-08-01 13:01:08.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/py.typed
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    21428 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/serialization.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.507544 tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      325 2023-08-01 13:01:08.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1022 2023-08-01 13:01:08.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/_register.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1147 2023-08-01 13:01:08.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/bitarray.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1467 2023-08-01 13:01:08.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/gmpy.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      910 2023-08-01 13:01:08.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/int.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1813 2023-08-01 13:01:08.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/numpy.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5741 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/pandas.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      984 2023-08-01 13:01:08.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/tuple.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.517544 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1435 2023-08-01 13:01:08.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1049 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/conftest.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7733 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/pool_fixtures_http.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    31948 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/test_packing.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2340 2023-08-01 13:01:08.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/test_packing_gmpy.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2422 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/test_pool_creation.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    13301 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/test_pool_http_2p.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    12384 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/test_pool_http_3p.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5373 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/test_pool_https_2p.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.517544 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      102 2023-08-01 13:20:14.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/README.md
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7985 2023-08-01 13:20:14.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/ca-combined.crt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3999 2023-08-01 13:20:14.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/ca-intermediate.crt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1704 2023-08-01 13:20:14.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/ca-intermediate.pem
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3986 2023-08-01 13:20:14.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/ca-root.crt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1704 2023-08-01 13:20:14.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/ca-root.pem
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7985 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/ca-untrusted.crt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3588 2023-08-01 13:20:14.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/party_0.crt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1704 2023-08-01 13:20:14.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/party_0.pem
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3588 2023-08-01 13:20:14.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/party_1.crt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1704 2023-08-01 13:20:14.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/party_1.pem
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3588 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/party_untrusted.crt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1704 2023-08-03 09:49:17.000000 tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/party_untrusted.pem
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.507544 tno.mpc.communication-4.8.1/src/tno.mpc.communication.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    19026 2023-08-03 09:49:22.000000 tno.mpc.communication-4.8.1/src/tno.mpc.communication.egg-info/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2494 2023-08-03 09:49:22.000000 tno.mpc.communication-4.8.1/src/tno.mpc.communication.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-08-03 09:49:22.000000 tno.mpc.communication-4.8.1/src/tno.mpc.communication.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       91 2023-08-03 09:49:22.000000 tno.mpc.communication-4.8.1/src/tno.mpc.communication.egg-info/entry_points.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      337 2023-08-03 09:49:22.000000 tno.mpc.communication-4.8.1/src/tno.mpc.communication.egg-info/requires.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       15 2023-08-03 09:49:22.000000 tno.mpc.communication-4.8.1/src/tno.mpc.communication.egg-info/top_level.txt
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 09:49:22.517544 tno.mpc.communication-4.8.1/stubs/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      773 2023-05-08 14:06:58.000000 tno.mpc.communication-4.8.1/stubs/gmpy2.pyi
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       35 2023-05-08 14:06:58.000000 tno.mpc.communication-4.8.1/stubs/pyarrow.pyi
```

### Comparing `tno.mpc.communication-4.5.0/LICENSE` & `tno.mpc.communication-4.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/PKG-INFO` & `tno.mpc.communication-4.8.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,49 @@
-Metadata-Version: 2.1
-Name: tno.mpc.communication
-Version: 4.5.0
-Summary: MPC Communication module
-Author-email: TNO MPC Lab <mpclab@tno.nl>
-Maintainer-email: TNO MPC Lab <mpclab@tno.nl>
-License: Apache License, Version 2.0
-Project-URL: Homepage, https://mpc.tno.nl/
-Project-URL: Documentation, https://docs.mpc.tno.nl/communication/4.5.0
-Project-URL: Source, https://github.com/TNO-MPC/communication
-Keywords: TNO,MPC,multi-party computation,communication
-Platform: any
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: Typing :: Typed
-Classifier: Topic :: Security :: Cryptography
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: bitarray
-Provides-Extra: gmpy
-Provides-Extra: gmpy2
-Provides-Extra: numpy
-Provides-Extra: pandas
-Provides-Extra: tls
-Provides-Extra: tests
-License-File: LICENSE
+# TNO PET Lab - secure Multi-Party Computation (MPC) - Communication
 
-# TNO MPC Lab - Communication
-
-The TNO MPC lab consists of generic software components, procedures, and
+The TNO PET Lab consists of generic software components, procedures, and
 functionalities developed and maintained on a regular basis to facilitate and
-aid in the development of MPC solutions. The lab is a cross-project initiative
-allowing us to integrate and reuse previously developed MPC functionalities to
+aid in the development of PET solutions. The lab is a cross-project initiative
+allowing us to integrate and reuse previously developed PET functionalities to
 boost the development of new protocols and solutions.
 
 The package tno.mpc.communication is part of the TNO Python Toolbox.
 
 _Limitations in (end-)use: the content of this repository may solely be used for
 applications that comply with international export control laws._  
 _This implementation of cryptographic software has not been audited. Use at your
 own risk._
 
 ## Documentation
 
 Documentation of the tno.mpc.communication package can be found
-[here](https://docs.mpc.tno.nl/communication/4.5.0).
+[here](https://docs.pet.tno.nl/mpc/communication/4.8.1).
 
 ## Install
 
 Easily install the tno.mpc.communication package using pip:
 
 ```console
 $ python -m pip install tno.mpc.communication
 ```
 
-If you wish to run the tests you can use:
+Note: The package specifies several optional dependency groups:
 
-```console
-$ python -m pip install 'tno.mpc.communication[tests]'
-```
+- `gmpy`: Adds support for sending various `gmpy2` types
+- `tests`: Includes all optional libraries required to run the full test suite
+- `tls`: Required if SSL is needed
+- `bitarray`: Adds support for sending `bitarray` types
+- `numpy`: Adds support for sending `numpy` types
+- `pandas`: Adds support for sending `pandas` types
+
+See [sending, receiving messages](#sending-receiving-messages) for more
+information on the supported third party types. Optional dependencies can be
+installed by specifying their names in brackets after the package name, e.g.
+when using `pip install`, use `pip install tno.mpc.communication[extra1,extra2]`
+to install the groups `extra1` and `extra2`.
 
 ## Usage
 
 The communication module uses `async` functions for sending and receiving. If
 you are familiar with the async module, you can skip to the `Pools` section.
 
 ### Async explanation
@@ -435,7 +413,60 @@
 >>> python bob.py
 2022-07-07 09:36:16,915 - tno.mpc.communication.httphandlers - INFO - Serving on 127.0.0.1:61002
 2022-07-07 09:36:20,223 - tno.mpc.communication.httphandlers - INFO - Received message from 127.0.0.1:61001
 Hello Bob! This is Alice speaking.
 2022-07-07 09:36:20,232 - tno.mpc.communication.httphandlers - INFO - HTTPServer: Shutting down server task
 2022-07-07 09:36:20,256 - tno.mpc.communication.httphandlers - INFO - Server 127.0.0.1:61002 shutdown
 ```
+
+## Test fixtures
+
+The `tno.mpc.communication` package exports several pytest fixtures as pytest
+plugins to facilitate the user in testing with pool objects. The fixtures take
+care of all configuration and clean-up of the pool objects so that you don't
+have to worry about that.
+
+Usage:
+
+```py
+# test_my_module.py
+import pytest
+from typing import Callable
+from tno.mpc.communication import Pool
+
+def test_with_two_pools(http_pool_duo: tuple[Pool, Pool]) -> None:
+    sender, receiver = http_pool_duo
+    # ... your code
+
+def test_with_three_pools(http_pool_trio: tuple[Pool, Pool, Pool]) -> None:
+    alice, bob, charlie = http_pool_trio
+    # ... your code
+
+@pytest.mark.parameterize("n_players", (2, 3, 4))
+def test_with_variable_pools(
+    n_players: int,
+    http_pool_group_factory: Callable[[int], tuple[Pool, ...]],
+) -> None:
+    pools = http_pool_group_factory(n_players)
+    # ... your code
+```
+
+### Fixture scope
+
+The scope of the fixtures can be set dynamically through the
+`--fixture-pool-scope`
+[option to pytest](https://docs.pytest.org/en/7.1.x/reference/reference.html#configuration-options).
+_Note that this will also change the scope of the global `event_loop` fixture
+that is provided by `pytest-asyncio`._ By default, in line with
+`pytest_asyncio`, the scope of all our fixtures is `"function"`. We advise to
+configure a larger scope (e.g. `"session"`, `"package"` or `"module"`) when
+possible to reduce test set-up and teardown time.
+
+Our fixtures pass `True` to the `port_reuse` argument of `aiohttp.web.TCPSite`.
+Their
+[documentation](https://docs.aiohttp.org/en/stable/web_reference.html?highlight=reuse_port#aiohttp.web.TCPSite)
+states that this option is not supported on Windows (outside of WSL). If you
+experience any issues, please disable the plugin by adding
+`-p no:pytest_tno.tno.mpc.communication.pytest_pool_fixtures` to your pytest
+configuration. Note that without `port_reuse` the tests may crash, as the test
+may try to bind to ports which may not have been freed by the operating system.
+For more reliable testing, run the tests on a WSL / Linux platform.
```

### Comparing `tno.mpc.communication-4.5.0/README.md` & `tno.mpc.communication-4.8.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,80 @@
-# TNO MPC Lab - Communication
+Metadata-Version: 2.1
+Name: tno.mpc.communication
+Version: 4.8.1
+Summary: MPC Communication module
+Author-email: TNO PET Lab <petlab@tno.nl>
+Maintainer-email: TNO PET Lab <petlab@tno.nl>
+License: Apache License, Version 2.0
+Project-URL: Homepage, https://pet.tno.nl/
+Project-URL: Documentation, https://docs.pet.tno.nl/mpc/communication/4.8.1
+Project-URL: Source, https://github.com/TNO-MPC/communication
+Keywords: TNO,MPC,multi-party computation,communication
+Platform: any
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: Typing :: Typed
+Classifier: Topic :: Security :: Cryptography
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: gmpy
+Provides-Extra: gmpy2
+Provides-Extra: bitarray
+Provides-Extra: numpy
+Provides-Extra: pandas
+Provides-Extra: tls
+Provides-Extra: tests
+License-File: LICENSE
 
-The TNO MPC lab consists of generic software components, procedures, and
+# TNO PET Lab - secure Multi-Party Computation (MPC) - Communication
+
+The TNO PET Lab consists of generic software components, procedures, and
 functionalities developed and maintained on a regular basis to facilitate and
-aid in the development of MPC solutions. The lab is a cross-project initiative
-allowing us to integrate and reuse previously developed MPC functionalities to
+aid in the development of PET solutions. The lab is a cross-project initiative
+allowing us to integrate and reuse previously developed PET functionalities to
 boost the development of new protocols and solutions.
 
 The package tno.mpc.communication is part of the TNO Python Toolbox.
 
 _Limitations in (end-)use: the content of this repository may solely be used for
 applications that comply with international export control laws._  
 _This implementation of cryptographic software has not been audited. Use at your
 own risk._
 
 ## Documentation
 
 Documentation of the tno.mpc.communication package can be found
-[here](https://docs.mpc.tno.nl/communication/4.5.0).
+[here](https://docs.pet.tno.nl/mpc/communication/4.8.1).
 
 ## Install
 
 Easily install the tno.mpc.communication package using pip:
 
 ```console
 $ python -m pip install tno.mpc.communication
 ```
 
-If you wish to run the tests you can use:
+Note: The package specifies several optional dependency groups:
 
-```console
-$ python -m pip install 'tno.mpc.communication[tests]'
-```
+- `gmpy`: Adds support for sending various `gmpy2` types
+- `tests`: Includes all optional libraries required to run the full test suite
+- `tls`: Required if SSL is needed
+- `bitarray`: Adds support for sending `bitarray` types
+- `numpy`: Adds support for sending `numpy` types
+- `pandas`: Adds support for sending `pandas` types
+
+See [sending, receiving messages](#sending-receiving-messages) for more
+information on the supported third party types. Optional dependencies can be
+installed by specifying their names in brackets after the package name, e.g.
+when using `pip install`, use `pip install tno.mpc.communication[extra1,extra2]`
+to install the groups `extra1` and `extra2`.
 
 ## Usage
 
 The communication module uses `async` functions for sending and receiving. If
 you are familiar with the async module, you can skip to the `Pools` section.
 
 ### Async explanation
@@ -404,7 +444,60 @@
 >>> python bob.py
 2022-07-07 09:36:16,915 - tno.mpc.communication.httphandlers - INFO - Serving on 127.0.0.1:61002
 2022-07-07 09:36:20,223 - tno.mpc.communication.httphandlers - INFO - Received message from 127.0.0.1:61001
 Hello Bob! This is Alice speaking.
 2022-07-07 09:36:20,232 - tno.mpc.communication.httphandlers - INFO - HTTPServer: Shutting down server task
 2022-07-07 09:36:20,256 - tno.mpc.communication.httphandlers - INFO - Server 127.0.0.1:61002 shutdown
 ```
+
+## Test fixtures
+
+The `tno.mpc.communication` package exports several pytest fixtures as pytest
+plugins to facilitate the user in testing with pool objects. The fixtures take
+care of all configuration and clean-up of the pool objects so that you don't
+have to worry about that.
+
+Usage:
+
+```py
+# test_my_module.py
+import pytest
+from typing import Callable
+from tno.mpc.communication import Pool
+
+def test_with_two_pools(http_pool_duo: tuple[Pool, Pool]) -> None:
+    sender, receiver = http_pool_duo
+    # ... your code
+
+def test_with_three_pools(http_pool_trio: tuple[Pool, Pool, Pool]) -> None:
+    alice, bob, charlie = http_pool_trio
+    # ... your code
+
+@pytest.mark.parameterize("n_players", (2, 3, 4))
+def test_with_variable_pools(
+    n_players: int,
+    http_pool_group_factory: Callable[[int], tuple[Pool, ...]],
+) -> None:
+    pools = http_pool_group_factory(n_players)
+    # ... your code
+```
+
+### Fixture scope
+
+The scope of the fixtures can be set dynamically through the
+`--fixture-pool-scope`
+[option to pytest](https://docs.pytest.org/en/7.1.x/reference/reference.html#configuration-options).
+_Note that this will also change the scope of the global `event_loop` fixture
+that is provided by `pytest-asyncio`._ By default, in line with
+`pytest_asyncio`, the scope of all our fixtures is `"function"`. We advise to
+configure a larger scope (e.g. `"session"`, `"package"` or `"module"`) when
+possible to reduce test set-up and teardown time.
+
+Our fixtures pass `True` to the `port_reuse` argument of `aiohttp.web.TCPSite`.
+Their
+[documentation](https://docs.aiohttp.org/en/stable/web_reference.html?highlight=reuse_port#aiohttp.web.TCPSite)
+states that this option is not supported on Windows (outside of WSL). If you
+experience any issues, please disable the plugin by adding
+`-p no:pytest_tno.tno.mpc.communication.pytest_pool_fixtures` to your pytest
+configuration. Note that without `port_reuse` the tests may crash, as the test
+may try to bind to ports which may not have been freed by the operating system.
+For more reliable testing, run the tests on a WSL / Linux platform.
```

### Comparing `tno.mpc.communication-4.5.0/pyproject.toml` & `tno.mpc.communication-4.8.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tno.mpc.communication"
 description = "MPC Communication module"
 readme = "README.md"
-authors = [{name = "TNO MPC Lab", email = "mpclab@tno.nl"}]
-maintainers = [{name = "TNO MPC Lab", email = "mpclab@tno.nl"}]
+authors = [{name = "TNO PET Lab", email = "petlab@tno.nl"}]
+maintainers = [{name = "TNO PET Lab", email = "petlab@tno.nl"}]
 keywords = [
     "TNO",
     "MPC",
     "multi-party computation",
     "communication",
 ]
 license = {text = "Apache License, Version 2.0"}
@@ -21,34 +21,33 @@
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "Typing :: Typed",
     "Topic :: Security :: Cryptography",
 ]
-urls = {Homepage = "https://mpc.tno.nl/", Documentation = "https://docs.mpc.tno.nl/communication/4.5.0", Source = "https://github.com/TNO-MPC/communication"}
-dynamic = ["version"]
-requires-python = ">=3.7"
+urls = {Homepage = "https://pet.tno.nl/", Documentation = "https://docs.pet.tno.nl/mpc/communication/4.8.1", Source = "https://github.com/TNO-MPC/communication"}
+dynamic = ["entry-points", "version"]
+requires-python = ">=3.8"
 dependencies = [
     "aiohttp",
     "mypy_extensions",
     "ormsgpack>=1.1.0",
-    "typing_extensions~=4.0; python_version<'3.8'",
 ]
 
 [project.optional-dependencies]
-bitarray = [
-    "bitarray",
-]
 gmpy = [
     "tno.mpc.encryption_schemes.utils[gmpy]",
 ]
 gmpy2 = [
     "tno.mpc.encryption_schemes.utils[gmpy]",
 ]
+bitarray = [
+    "bitarray",
+]
 numpy = [
     "numpy",
 ]
 pandas = [
     "pandas",
     "pyarrow",
 ]
@@ -56,20 +55,22 @@
     "pyOpenSSL",
 ]
 tests = [
     "tno.mpc.communication[bitarray,gmpy,numpy,pandas,tls]",
     "pandas-stubs",
     "pytest",
     "pytest-asyncio",
+    "pytest-timeout",
     "typeguard",
 ]
 
 [tool.setuptools]
 platforms = ["any"]
 
 [tool.setuptools.dynamic]
+entry-points = {file = "entry_points.txt"}
 version = {attr = "tno.mpc.communication.__version__"}
 
 [tool.setuptools.package-data]
 "*" = ["py.typed"]
 "tno.mpc.communication" = ["test/tls_certs/*"]
```

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/__init__.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,21 +10,12 @@
 from tno.mpc.communication.exceptions import RepetitionError as RepetitionError
 from tno.mpc.communication.pool import Pool as Pool
 from tno.mpc.communication.serialization import Serialization as Serialization
 from tno.mpc.communication.serialization import (
     SupportsSerialization as SupportsSerialization,
 )
 
-__version__ = "4.5.0"
+__version__ = "4.8.1"
 
 
 # Register all default (de)serializers
 Serialization.clear_serialization_logic(reload_defaults=True)
-
-
-def init_pool() -> Pool:
-    """
-    Initializes a new Pool object.
-
-    :return: new Pool object.
-    """
-    return Pool()
```

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/functions.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/functions.py`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/httphandlers.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/httphandlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 
 from __future__ import annotations
 
 import asyncio
 import functools
 import logging
 import ssl
-import sys
 from asyncio import Future, Transport
-from typing import Any, Awaitable, Callable, cast, overload
+from typing import Any, Awaitable, Callable, Protocol, cast, overload
 
-from aiohttp import ClientSession, ClientTimeout, web
+from aiohttp import (
+    ClientConnectorCertificateError,
+    ClientConnectorSSLError,
+    ClientSession,
+    ClientSSLError,
+    ClientTimeout,
+    web,
+)
 
 from .functions import init
 from .serialization import DEFAULT_PACK_OPTION, Serialization
 
-if sys.version_info >= (3, 8):
-    from typing import Protocol
-else:
-    from typing_extensions import Protocol
-
-
 logger = init(__name__, logger_level=logging.INFO)
 
 
 class AbstractPool(Protocol):
     """
     Protocol that mimics tno.mpc.communication.Pool.
 
@@ -126,16 +126,16 @@
             return msg_prefix + str(msg_id)
         return msg_id
 
     async def shutdown(self) -> None:
         """
         Shutdown HTTP Client. Closes open HTTP session.
         """
-        if self.session and not self.session.closed:
-            await self.session.close()
+        if (session := self.session) and not session.closed:
+            await session.close()
             logger.info(
                 f"Client {self.addr}:{self.port} shutdown\nTotal bytes sent: {self.total_bytes_sent}\nTotal messages sent: {self.msg_send_counter}"
             )
 
     async def send(
         self,
         message: Any,
@@ -177,16 +177,16 @@
         self,
         data: bytes,
         retry_delay: int = 1,
         timeout: ClientTimeout = ClientTimeout(total=300),
         num_retries: int = -1,
     ) -> None:
         """
-        Sends a POST request to containing this data to this client.
-        If sending of message fails and retry_delay > 0 then retry after retry_delay seconds
+        Sends a POST request containing the provided data to this client.
+        If sending of message fails and retry_delay > 0 then retry after retry_delay seconds.
 
         :param data: the data to send
         :param retry_delay: number of seconds to wait before retrying after failure
         :param timeout: timeout for the connection
         :param num_retries: number of retries that are allowed for sending the message (-1 for unbounded retries)
         """
         try:
@@ -202,14 +202,20 @@
                 assert resp.status == 200, "Did not receive status OK (200)"
 
                 response_message = await resp.text()
 
                 self.total_bytes_sent += len(data)
 
                 logger.debug(f"Response: {response_message}")
+        except (
+            ClientConnectorCertificateError,
+            ClientConnectorSSLError,
+            ClientSSLError,
+        ):
+            raise
         except Exception:
             logger.exception("Message not received.")
             if retry_delay and num_retries != 0:
                 logger.debug(
                     f"Connection failed. Retrying ({num_retries} attempts remaining), url: {self.addr}:{self.port}, data:"
                     f" {data[0:min(100,len(data))]!r}..."
                 )
@@ -233,20 +239,20 @@
         :return: the received message
         """
         if msg_id is None:
             msg_id = self.msg_recv_counter
         msg_id = HTTPClient._prefix_msg_id(msg_id, self.msg_prefix)
         self.msg_recv_counter += 1
 
-        data = self.buffer.pop(msg_id, None)
-        if data is None:
-            fut: Future[dict[str, Any]]
-            fut = self.buffer[msg_id] = Future()
-            return fut
-        return data
+        if (data := self.buffer.pop(msg_id, None)) is not None:
+            return data
+
+        fut: Future[dict[str, Any]]
+        fut = self.buffer[msg_id] = Future()
+        return fut
 
     async def _create_client_session(self, cookies: dict[str, str]) -> None:
         """
         Create an aiohttp ClientSession for use with this HTTPClient. This method should only be
         called once during construction.
 
         :param cookies: Cookies for this ClientSession
@@ -310,20 +316,20 @@
             self.run_server(get_handler, post_handler)
         )
 
     async def shutdown(self) -> None:
         """
         Shutdown HTTP Server.
         """
+        if (task := self.server_task) and not task.cancelled():
+            logger.info("HTTPServer: Shutting down server task")
+            task.cancel()
         if self.site:
             logger.debug("HTTPServer: Shutting down site")
             await self.site.stop()
-        if self.server_task and not self.server_task.cancelled():
-            logger.info("HTTPServer: Shutting down server task")
-            self.server_task.cancel()
         logger.info(
             f"Server {self.addr}:{self.port} shutdown\nTotal bytes received: {self.total_bytes_recv}\nTotal messages received: {self.msg_recv_counter}"
         )
 
     async def _post_handler(self, request: web.Request) -> web.Response:
         """
         Handles an incoming HTTP POST request and writes every JSON POST request to socket.
```

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/pool.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 import asyncio
 import functools
 import logging
 import socket
 import ssl
 import warnings
 from asyncio import Future
-from typing import Any, Iterable, cast
+from pathlib import Path
+from typing import Any, Iterable, Union, cast
 
 from aiohttp import ClientTimeout
 
 from .functions import init
 from .httphandlers import HTTPClient, HTTPServer
 from .serialization import DEFAULT_PACK_OPTION, Serialization
 
@@ -25,17 +26,17 @@
 class Pool:
     """
     Facilitates a communication pool that enables communication between us (server) and others (clients).
     """
 
     def __init__(
         self,
-        key: str | None = None,
-        cert: str | None = None,
-        ca_cert: str | None = None,
+        key: Path | str | None = None,
+        cert: Path | str | None = None,
+        ca_cert: Path | str | None = None,
         timeout: ClientTimeout = ClientTimeout(total=300),
         max_retries: int = -1,
     ):
         """
         Initialises a pool.
 
         The key and certificate paths are provided as arguments to ssl.SSLContext.load_cert_chain.
@@ -99,15 +100,15 @@
         )
 
     def add_http_client(
         self,
         name: str,
         addr: str,
         port: int | None = None,
-        cert: str | None = None,
+        cert: Path | str | None = None,
         **cert_kwargs: Any,
     ) -> None:
         r"""
         Add an HTTP Client to the pool. addr can be either an IP address or a
         hostname.
 
         :param name: name of the client
@@ -118,15 +119,14 @@
         :raise ImportError: required dependencies for client identification through certificates
             are missing
         """
         ssl_ctx = self.create_ssl_context(self.key, self.cert, self.ca_cert)
         port = self.get_port(ssl_ctx) if port is None else port
         client = HTTPClient(self, addr, port, ssl_ctx)
         self.pool_handlers[name] = client
-        self.handlers_lookup[f"{socket.gethostbyname(addr)}:{port}"] = client
         if cert:
             try:
                 import OpenSSL.crypto  # pylint: disable=import-outside-toplevel
             except ImportError as exc:
                 raise ImportError(
                     "Could not import the required dependencies for client identification through "
                     "ssl/tls. Please install tno.mpc.communication[tls]."
@@ -141,17 +141,17 @@
                 f"{client_cert.get_issuer().CN}:{client_cert.get_serial_number()}"
             ] = client
         else:
             self.handlers_lookup[f"{socket.gethostbyname(addr)}:{port}"] = client
 
     @staticmethod
     def create_ssl_context(
-        key: str | None,
-        cert: str | None,
-        ca_cert: str | None = None,
+        key: Path | str | None,
+        cert: Path | str | None,
+        ca_cert: Path | str | None = None,
         server: bool = False,
     ) -> ssl.SSLContext | None:
         """
         Create an SSL context.
 
         The key and certificate paths are provided as arguments to ssl.SSLContext.load_cert_chain.
         The ca_cert is provided as argument to ssl.SSLContext.load_verify_locations. Please refer
@@ -163,14 +163,17 @@
         :param ca_cert: path to the certificate authority (CA) certificate to use in the ssl context
         :param server: boolean stating whether we need a server context or not (client)
         :return: an SSL context or None
         """
         if ca_cert is None:
             return None
 
+        key = cast(Union[Path, str], key)
+        cert = cast(Union[Path, str], cert)
+
         if server:
             purpose = ssl.Purpose.CLIENT_AUTH
         else:
             purpose = ssl.Purpose.SERVER_AUTH
 
         ctx = ssl.create_default_context(purpose=purpose)
         ctx.load_cert_chain(certfile=cast(str, cert), keyfile=cast(str, key))
@@ -192,15 +195,15 @@
         if ssl_ctx is None:
             return 80
         return 443
 
     def _preprocess_broadcast(
         self,
         msg_id: str,
-        handler_names: list[str] | None = None,
+        handler_names: Iterable[str] | None = None,
         timeout: ClientTimeout | None = None,
         max_retries: int | None = None,
     ) -> tuple[ClientTimeout, int, list[HTTPClient], bool, int, str]:
         """
         Preprocessing for the broadcast method
 
         :param msg_id: a string identifying the message to send
@@ -247,15 +250,15 @@
 
         return timeout, max_retries, handlers, use_pickle, option, msg_id
 
     def async_broadcast(
         self,
         message: Any,
         msg_id: str,
-        handler_names: list[str] | None = None,
+        handler_names: Iterable[str] | None = None,
         timeout: ClientTimeout | None = None,
         max_retries: int | None = None,
     ) -> None:
         """
         Send a message to multiple other parties asynchronously.
         Serializes the message and schedules the sending of the message and returns immediately after that.
         There is no assurance of feedback about the message being delivered.
@@ -289,15 +292,15 @@
                 handler._send(data, timeout=timeout, num_retries=max_retries)
             )
 
     async def broadcast(
         self,
         message: Any,
         msg_id: str,
-        handler_names: list[str] | None = None,
+        handler_names: Iterable[str] | None = None,
         timeout: ClientTimeout | None = None,
         max_retries: int | None = None,
     ) -> None:
         """
         Send a message to multiple other parties synchronously
 
         :param message: the message to send
@@ -424,48 +427,61 @@
             for handler in handler_names
         )
 
     async def recv_all(
         self,
         handler_names: Iterable[str] | None = None,
         msg_id: str | None = None,
+        timeout: float | None = None,
     ) -> tuple[tuple[str, Any]]:
         """
         Method that receives one message for each party in an asynchronous fashion.
 
-        :param handler_names: List of pool handler names to receive a message from. If None, will receive one message
-             from all parties.
+        :param handler_names: List of pool handler names to receive a message from. If None, will
+            receive one message from all parties.
         :param msg_id: an optional string identifying the message to collect
-        :return: Tuple of tuples containing first the party name and second the corresponding message.
+        :param timeout: maximum time in seconds to wait for the message to be received. Waits
+            indefinitely if None.
+        :raise TimeoutError: message was not received before timeout
+        :return: Tuple of tuples containing first the party name and second the corresponding
+            message.
         """
         if handler_names is None:
             handler_names = self.pool_handlers.keys()
 
         async def result_tuple(handler: str) -> tuple[str, Any]:
             """
             Receive a message from the given handler, using the outer scope msg_id.
 
             :param handler: Pool handler name to receive a message from.
             :return: Tuple containing first the party name and second the received message.
             """
-            return handler, await self.recv(handler, msg_id)
+            return handler, await self.recv(handler, msg_id, timeout=timeout)
 
         return await asyncio.gather(*(result_tuple(handler_name) for handler_name in handler_names))  # type: ignore[no-any-return]
 
-    async def recv(self, handler_name: str, msg_id: str | None = None) -> Any:
+    async def recv(
+        self,
+        handler_name: str,
+        msg_id: str | None = None,
+        timeout: float | None = None,
+    ) -> Any:
         """
         Receive a message asynchronously from a peer. Ensures result.
 
         :param handler_name: the name of the pool handler to receive a message from
         :param msg_id: an optional string identifying the message to collect
+        :param timeout: maximum time in seconds to wait for the message to be received. Waits
+            indefinitely if None.
+        :raise TimeoutError: message was not received before timeout
         :return: the message from peer.
         """
         result = self.arecv(handler_name, msg_id)
         if asyncio.isfuture(result):
-            await result
+            await asyncio.wait_for(result, timeout=timeout)
             return result.result()
         return result
 
     def update_msg_prefix(self, msg_prefix: str | None) -> None:
         """
         Updates the message prefix that is used for all clients in the pool.
         This message prefix is used for both sending and receiving of messages.
@@ -479,18 +495,18 @@
         """
         Gracefully shutdown all connections/listeners in the pool.
         """
         total_bytes_sent = 0
         msg_send_counter = 0
         total_bytes_recv = 0
         msg_recv_counter = 0
-        if self.http_server is not None:
-            await self.http_server.shutdown()
-            msg_recv_counter = self.http_server.msg_recv_counter
-            total_bytes_recv = self.http_server.total_bytes_recv
+        if (server := self.http_server) is not None:
+            await server.shutdown()
+            msg_recv_counter = server.msg_recv_counter
+            total_bytes_recv = server.total_bytes_recv
         for handler in self.pool_handlers.values():
             await handler.shutdown()
             total_bytes_sent += handler.total_bytes_sent
             msg_send_counter += handler.msg_send_counter
         self.pool_handlers = {}
         self.handlers_lookup = {}
         logger.info(
```

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/serialization.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 This module contains the serialization logic used in sending and receiving arbitrary objects.
 """
 
 from __future__ import annotations
 
 import inspect
 import pickle
-import sys
 from functools import partial
-from typing import Any, Callable, TypeVar, Union
+from typing import (
+    Any,
+    Callable,
+    Collection,
+    Container,
+    Iterable,
+    Protocol,
+    TypeVar,
+    Union,
+)
 
 import ormsgpack
 from mypy_extensions import Arg, KwArg
 
 from tno.mpc.communication import serializer_plugins
 from tno.mpc.communication.exceptions import AnnotationError, RepetitionError
 from tno.mpc.communication.functions import init
 
-if sys.version_info >= (3, 8):
-    from typing import Protocol
-else:
-    from typing_extensions import Protocol
-
-
 logger = init(__name__)
 
 SerializerFunction = Union[
     Callable[[Arg(Any, "self"), KwArg(Any)], Any],
     Callable[[Arg(Any, "obj"), KwArg(Any)], Any],
     Callable[[Arg(Any, "self"), Arg(bool, "use_pickle"), KwArg(Any)], Any],
     Callable[[Arg(Any, "obj"), Arg(bool, "use_pickle"), KwArg(Any)], Any],
@@ -36,17 +38,18 @@
     Callable[[Arg(Any, "obj"), Arg(bool, "use_pickle"), KwArg(Any)], Any],
 ]
 DorSFunction = TypeVar(
     "DorSFunction", bound=Union[SerializerFunction, DeserializerFunction]
 )
 
 DEFAULT_PACK_OPTION = (
-    ormsgpack.OPT_SERIALIZE_NUMPY
-    | ormsgpack.OPT_PASSTHROUGH_BIG_INT
+    ormsgpack.OPT_PASSTHROUGH_BIG_INT
     | ormsgpack.OPT_PASSTHROUGH_TUPLE
+    | ormsgpack.OPT_PASSTHROUGH_DATACLASS
+    | ormsgpack.OPT_SERIALIZE_NUMPY
 )
 
 
 class SupportsSerialization(Protocol):
     """
     Type placeholder for classes supporting custom serialization.
     """
@@ -149,15 +152,15 @@
             check_annotations=check_annotations,
             overwrite=overwrite,
         )
 
     @staticmethod
     def _register_serializer(
         serializer: SerializerFunction,
-        types: tuple[str, ...],
+        types: Collection[str],
         check_annotations: bool = True,
         overwrite: bool = False,
     ) -> None:
         """
         Register a serializer function.
 
         :param serializer: Serializer function.
@@ -186,15 +189,15 @@
         Serialization._register(
             SERIALIZER_FUNCS, serializer, types, overwrite=overwrite
         )
 
     @staticmethod
     def _register_deserializer(
         deserializer: DeserializerFunction,
-        types: tuple[str, ...],
+        types: Collection[str],
         check_annotations: bool = True,
         overwrite: bool = False,
     ) -> None:
         """
         Register a deserializer function.
 
         :param deserializer: Deserializer function.
@@ -226,15 +229,15 @@
             DESERIALIZER_FUNCS, deserializer, types, overwrite=overwrite
         )
 
     @staticmethod
     def _register(
         target_dict: dict[str, DorSFunction],
         d_or_s_function: DorSFunction,
-        types: tuple[str, ...],
+        types: Iterable[str],
         overwrite: bool,
     ) -> None:
         """
         In-place add (de)serializer to a target dictionary for multiple keys.
 
         :param target_dict: Target dictionary.
         :param d_or_s_function: (De)serializer to register in the target dictionary
@@ -497,15 +500,15 @@
             "bound to any other parameter, i.e. a '**kwargs' parameter. This is required in the "
             "function definition. These keyword arguments should also be forwarded to the next "
             "(de)serialization call."
         )
 
 
 def _validate_provided_return_annotation(
-    signature: inspect.Signature, types: tuple[str, ...]
+    signature: inspect.Signature, types: Container[str]
 ) -> None:
     """
     Validate that the signature agrees with the provided types.
 
     :param signature: Signature to validate.
     :param types: Types that are supposedly consistent with the signature.
     :raise AnnotationError: Types and signature do not agree.
```

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/_register.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/_register.py`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/bitarray.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/bitarray.py`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/gmpy.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/gmpy.py`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/int.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/int.py`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/numpy.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/numpy.py`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/pandas.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from __future__ import annotations
 
 import datetime
 import io
 import sys
 import warnings
-from typing import Any, Callable, Hashable
+from typing import Any, Callable, Dict, cast
 
 from tno.mpc.communication.functions import redirect_importerror_to_optionalimporterror
 from tno.mpc.communication.serialization import Serialization
 
 with redirect_importerror_to_optionalimporterror():
     import numpy as np
     import pandas as pd
@@ -35,15 +35,15 @@
     str,
 )
 TEMP_COLUMN_NAME = "TNO_MPC_COMMUNICATION_TEMPNAME"
 
 
 def pandas_serialize_dataframe(  # pylint: disable=missing-raises-doc
     obj: DataFrame, use_pickle: bool, **kwargs: Any
-) -> bytes | dict[Hashable, Any]:
+) -> bytes | dict[str, Any]:
     r"""
     Function for serializing pandas dataframes
 
     Attempt to use parquet for smaller serialized dataframe, but fallback to dictionaries
     otherwise.
 
     :param obj: pandas object to serialize
@@ -85,19 +85,19 @@
                 "type <str>. This might be resolved by using "
                 "'df.columns = df.columns.astype(str)'. Falling back to serialization via "
                 "dictionary."
             )
         else:
             raise exc
     # Fall-back to dictionary serialization
-    return obj.to_dict()
+    return cast(Dict[str, Any], obj.to_dict(orient="split"))
 
 
 def pandas_deserialize_dataframe(
-    obj: bytes | dict[Hashable, Any], use_pickle: bool, **_kwargs: Any
+    obj: bytes | dict[str, Any], use_pickle: bool, **_kwargs: Any
 ) -> DataFrame:
     r"""
     Function for deserializing pandas dataframe
 
     :param obj: pandas dataframe to deserialize
     :param use_pickle: set to True to enable serialization fallback to pickle
     :param \**_kwargs: optional extra keyword arguments
@@ -111,25 +111,23 @@
         except ImportError as exc:
             raise ImportError(
                 "The pandas object was serialized to parquet, but the required dependencies for "
                 "deserializing this format are missing. Please install "
                 "tno.mpc.communication[pandas]."
             ) from exc
     else:  # Dataframe is serialized as dictionary
-        dataframe = pd.DataFrame(obj)
+        dataframe = pd.DataFrame(**obj)
     return dataframe.applymap(
         lambda x: Serialization.deserialize(x, use_pickle=use_pickle)
         if isinstance(x, dict) and "type" in x and "data" in x
         else x
     )
 
 
-def pandas_serialize_series(
-    obj: Series[Any], **_kwargs: Any
-) -> bytes | dict[Hashable, Any]:
+def pandas_serialize_series(obj: Series[Any], **_kwargs: Any) -> bytes | dict[str, Any]:
     r"""
     Function for serializing pandas series
 
     :param obj: pandas series to serialize
     :param \**_kwargs: optional extra keyword arguments
     :return: serialized series
     """
@@ -137,15 +135,15 @@
         return pandas_serialize_dataframe(
             pd.DataFrame(obj, columns=[TEMP_COLUMN_NAME]), **_kwargs
         )
     return pandas_serialize_dataframe(pd.DataFrame(obj), **_kwargs)
 
 
 def pandas_deserialize_series(
-    obj: bytes | dict[Hashable, Any], **kwargs: Any
+    obj: bytes | dict[str, Any], **kwargs: Any
 ) -> Series:  # type: ignore[type-arg]
     r"""
     Function for deserializing pandas series
 
     :param obj: pandas series to deserialize
     :param \**kwargs: optional extra keyword arguments
     :return: deserialized series
```

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/serializer_plugins/tuple.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/serializer_plugins/tuple.py`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/__init__.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/__init__.py`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/pool_fixtures_http.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/pool_fixtures_http.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 Module used to generate pool fixtures to use in unit tests.
 """
 
+from __future__ import annotations
+
 import asyncio
+import warnings
 from asyncio import AbstractEventLoop
 from pathlib import Path
-from typing import Any, AsyncGenerator, Generator, Tuple
+from typing import Any, AsyncGenerator, Generator
 
 import pytest
 import pytest_asyncio
-from _pytest.fixtures import FixtureRequest
 
 from tno.mpc.communication import Pool
 
 
 @pytest_asyncio.fixture(scope="module")
 def event_loop(  # pylint: disable=unused-argument
-    request: FixtureRequest,
+    request: pytest.FixtureRequest,
 ) -> Generator[AbstractEventLoop, None, None]:
     """
     Create an instance of the default event loop for each test case. This overrides the event_loop method from
     pytest-asyncio with a scope.
 
     :param request: A fixture request.
     :return: A new event loop
@@ -40,15 +42,15 @@
         pass
 
 
 @pytest.mark.asyncio
 async def pool_http_local_base(
     id_: int,
     lport: int,
-    *args: Tuple[str, int],
+    *args: tuple[str, int],
     tls: bool = False,
     certs_as_identifier: bool = False,
 ) -> AsyncGenerator[Pool, None]:
     r"""
     Generates an async generator which yields a test pool
 
     :param id_: the identifier of the listening client
@@ -82,15 +84,15 @@
     yield pool
     await pool.shutdown()
 
 
 @pytest.mark.asyncio
 async def generate_http_test_pools(
     clients: int, *args: Any, **kwargs: Any
-) -> AsyncGenerator[Tuple[Pool, ...], None]:
+) -> AsyncGenerator[tuple[Pool, ...], None]:
     r"""
     Generates an async generator which yields n test pools which are all connected with each other.
     Connections:
     Client 0: port 4444 + 10 * n
     Client 1: port 4445 + 10 * n
     Client i: port 4444 + 10 * n + i
 
@@ -100,14 +102,22 @@
     await finish(pools)
 
     :param clients: number of clients (n)
     :param \*args: additional positional arguments provided to pool_http_local_base
     :param \**kwargs: additional keyword arguments provided to pool_http_local_base
     :return: a collection of communication pools
     """
+    warnings.warn(
+        "As of tno.mpc.communication 4.8.0, all fixtures in tno.mpc.communication.test are "
+        "deprecated in favor of the new pytest plugin fixtures. Most notably, http_pool_duo and "
+        "http_pool_trio replace fixture_pool_http_2p and fixture_pool_http_3p respectively. "
+        "Groups of HTTP pools of arbitrary size can be generated through http_pool_group_factory. "
+        "Please refer to the README for usage instructions.",
+        DeprecationWarning,
+    )
     pools = []
     base_port = 4444 + clients * 10
     for client in range(clients):
         pools.append(
             pool_http_local_base(
                 client,
                 base_port + client,
@@ -121,114 +131,114 @@
         obj.append(await pool.asend(None))
     yield tuple(obj)
     await asyncio.gather(*[finish(pool) for pool in pools])
 
 
 # HTTP
 @pytest_asyncio.fixture(name="pool_http_2p", scope="module")
-async def fixture_pool_http_2p() -> AsyncGenerator[Tuple[Pool, ...], None]:
+async def fixture_pool_http_2p() -> AsyncGenerator[tuple[Pool, ...], None]:
     """
     Creates a collection of 2 communication pools
 
     :return: a collection of communication pools
     """
     pools = generate_http_test_pools(2)
     yield await pools.asend(None)
     await finish(pools)
 
 
 @pytest_asyncio.fixture(name="pool_http_3p", scope="module")
-async def fixture_pool_http_3p() -> AsyncGenerator[Tuple[Pool, ...], None]:
+async def fixture_pool_http_3p() -> AsyncGenerator[tuple[Pool, ...], None]:
     """
     Creates a collection of 3 communication pools
 
     :return: a collection of communication pools
     """
     pools = generate_http_test_pools(3)
     yield await pools.asend(None)
     await finish(pools)
 
 
 @pytest_asyncio.fixture(name="pool_http_4p", scope="module")
-async def fixture_pool_http_4p() -> AsyncGenerator[Tuple[Pool, ...], None]:
+async def fixture_pool_http_4p() -> AsyncGenerator[tuple[Pool, ...], None]:
     """
     Creates a collection of 4 communication pools
 
     :return: a collection of communication pools
     """
     pools = generate_http_test_pools(4)
     yield await pools.asend(None)
     await finish(pools)
 
 
 @pytest_asyncio.fixture(name="pool_http_5p", scope="module")
-async def fixture_pool_http_5p() -> AsyncGenerator[Tuple[Pool, ...], None]:
+async def fixture_pool_http_5p() -> AsyncGenerator[tuple[Pool, ...], None]:
     """
     Creates a collection of 5 communication pools
 
     :return: a collection of communication pools
     """
     pools = generate_http_test_pools(5)
     yield await pools.asend(None)
     await finish(pools)
 
 
 # HTTPS
 @pytest_asyncio.fixture(name="pool_https_2p", scope="function")
-async def fixture_pool_https_2p() -> AsyncGenerator[Tuple[Pool, ...], None]:
+async def fixture_pool_https_2p() -> AsyncGenerator[tuple[Pool, ...], None]:
     """
     Creates a collection of 2 communication pools using SSL/TLS
 
     :return: a collection of communication pools
     """
     pools = generate_http_test_pools(2, tls=True)
     yield await pools.asend(None)
     await finish(pools)
 
 
 @pytest_asyncio.fixture(name="pool_https_3p", scope="function")
-async def fixture_pool_https_3p() -> AsyncGenerator[Tuple[Pool, ...], None]:
+async def fixture_pool_https_3p() -> AsyncGenerator[tuple[Pool, ...], None]:
     """
     Creates a collection of 3 communication pools using SSL/TLS
 
     :return: a collection of communication pools
     """
     pools = generate_http_test_pools(3, tls=True)
     yield await pools.asend(None)
     await finish(pools)
 
 
 @pytest_asyncio.fixture(name="pool_https_3p_certs_as_id", scope="function")
-async def fixture_pool_https_3p_certs_as_id() -> AsyncGenerator[Tuple[Pool, ...], None]:
+async def fixture_pool_https_3p_certs_as_id() -> AsyncGenerator[tuple[Pool, ...], None]:
     """
     Creates a collection of 3 communication pools using SSL/TLS
 
     Clients are identified by their certificate
 
     :return: a collection of communication pools
     """
     pools = generate_http_test_pools(3, tls=True, certs_as_identifier=True)
     yield await pools.asend(None)
     await finish(pools)
 
 
 @pytest_asyncio.fixture(name="pool_https_4p", scope="function")
-async def fixture_pool_https_4p() -> AsyncGenerator[Tuple[Pool, ...], None]:
+async def fixture_pool_https_4p() -> AsyncGenerator[tuple[Pool, ...], None]:
     """
     Creates a collection of 4 communication pools using SSL/TLS
 
     :return: a collection of communication pools
     """
     pools = generate_http_test_pools(4, tls=True)
     yield await pools.asend(None)
     await finish(pools)
 
 
 @pytest_asyncio.fixture(name="pool_https_5p", scope="function")
-async def fixture_pool_https_5p() -> AsyncGenerator[Tuple[Pool, ...], None]:
+async def fixture_pool_https_5p() -> AsyncGenerator[tuple[Pool, ...], None]:
     """
     Creates a collection of 5 communication pools using SSL/TLS
 
     :return: a collection of communication pools
     """
     pools = generate_http_test_pools(5, tls=True)
     yield await pools.asend(None)
```

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/test_packing.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/test_packing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 This module tests packing and unpacking of objects
 (serialization/deserialization)
 """
 
+from __future__ import annotations
+
 import copy
+from dataclasses import asdict, dataclass
 from datetime import datetime
 from decimal import Decimal
-from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Union, cast
+from typing import Any, Callable, TypeVar, cast
 
 import bitarray
 import numpy as np
 import numpy.typing as npt
 import ormsgpack
 import pandas as pd
 import pytest
@@ -18,26 +21,27 @@
 from tno.mpc.communication import (
     AnnotationError,
     RepetitionError,
     Serialization,
     SupportsSerialization,
 )
 from tno.mpc.communication.httphandlers import HTTPClient
+from tno.mpc.communication.serialization import DEFAULT_PACK_OPTION
 
 TypePlaceholder = TypeVar("TypePlaceholder")
 
 
 def pack_unpack_test(
     obj: TypePlaceholder,
     comparator: Callable[[TypePlaceholder, TypePlaceholder], bool] = lambda a, b: a
     == b,
     expect: bool = True,
     use_pickle: bool = False,
-    serial_option: Optional[int] = None,
-    deserial_option: Optional[int] = None,
+    serial_option: int | None = DEFAULT_PACK_OPTION,
+    deserial_option: int | None = None,
     **kwargs: Any,
 ) -> None:
     r"""
     Tests packing and unpacking of an object
 
     :param obj: the object to pack/unpack
     :param comparator: function comparing two objects, returning True
@@ -112,15 +116,15 @@
 
 
 def test_int_serialization_fail() -> None:
     """
     Tests packing and unpacking of Python ints
     """
     with pytest.raises(TypeError):
-        pack_unpack_test(2**2048, serial_options=None)
+        pack_unpack_test(2**2048, serial_option=None)
 
 
 def test_float_serialization() -> None:
     """
     Tests packing and unpacking of floats
     """
     pack_unpack_test(1.0)
@@ -160,15 +164,15 @@
     pack_unpack_test(bitarray.bitarray("10101110"))
 
 
 def test_empty_list() -> None:
     """
     Tests packing and unpacking of empty lists
     """
-    list_: List[None] = []
+    list_: list[None] = []
     pack_unpack_test(list_)
 
 
 def test_list_serialization_same_type() -> None:
     """
     Tests packing and unpacking of lists with objects of same type
     """
@@ -257,15 +261,15 @@
     )
 
 
 def test_empty_dict() -> None:
     """
     Tests packing and unpacking of empty dictionary
     """
-    dict_: Dict[Any, Any] = {}
+    dict_: dict[Any, Any] = {}
     pack_unpack_test(dict_)
 
 
 def test_monstrous_collection_serialization() -> None:
     """
     Tests packing and unpacking of a complex collection
     """
@@ -335,24 +339,24 @@
         Serialization.register_class(ClassNoLogic)  # type: ignore[arg-type]
 
 
 def test_empty_series_serialization() -> None:
     """
     Tests packing and unpacking of an empty pandas series
     """
-    dataframe = pd.Series(dtype=object)
-    pack_unpack_test(dataframe, lambda df1, df2: df1.equals(df2))
+    series: pd.Series[Any] = pd.Series(dtype=object)
+    pack_unpack_test(series, lambda df1, df2: df1.equals(df2))
 
 
 def test_series_serialization() -> None:
     """
     Tests packing and unpacking of a pandas series
     """
-    dataframe = pd.Series([1, 2, 3], index=["a", "b", "c"])
-    pack_unpack_test(dataframe, lambda df1, df2: df1.equals(df2))
+    series: pd.Series[Any] = pd.Series([1, 2, 3], index=["a", "b", "c"])
+    pack_unpack_test(series, lambda df1, df2: df1.equals(df2))
 
 
 def test_empty_dataframe_serialization() -> None:
     """
     Tests packing and unpacking of an empty pandas dataframe
     """
     dataframe = pd.DataFrame()
@@ -494,15 +498,15 @@
 
         :param \**_kwargs: optional extra keyword arguments
         :return: serialized object
         """
         return self.value
 
     @staticmethod
-    def deserialize(value: int, **_kwargs: Any) -> "ClassWrongSignature":  # type: ignore[override]  # pylint: disable=arguments-renamed
+    def deserialize(value: int, **_kwargs: Any) -> ClassWrongSignature:  # type: ignore[override]  # pylint: disable=arguments-renamed
         r"""
         Deserialization method
 
         :param \**_kwargs: optional extra keyword arguments
         :param value: object to deserialize
         :return: deserializes object
         """
@@ -557,25 +561,25 @@
         """
         Initialization of class
 
         :param value: value attribute of class
         """
         self.value = value
 
-    def serialize(self, **_kwargs: Any) -> Dict[str, int]:
+    def serialize(self, **_kwargs: Any) -> dict[str, int]:
         r"""
         Serialization method
 
         :param \**_kwargs: optional extra keyword arguments
         :return: serialized object
         """
         return {"value": self.value}
 
     @staticmethod
-    def deserialize(obj: Any, **_kwargs: Any) -> "ClassMismatchType":
+    def deserialize(obj: Any, **_kwargs: Any) -> ClassMismatchType:
         r"""
         Deserialization method
 
         :param obj: object to deserialize
         :param \**_kwargs: optional extra keyword arguments
         :return: deserializes object
         """
@@ -591,25 +595,25 @@
         """
         Initialization of class
 
         :param value: value attribute of class
         """
         self.value = value
 
-    def serialize(self, **_kwargs: Any) -> Dict[str, int]:
+    def serialize(self, **_kwargs: Any) -> dict[str, int]:
         r"""
         Serialization method
 
         :param \**_kwargs: optional extra keyword arguments
         :return: serialized object
         """
         return {"value": self.value}
 
     @staticmethod
-    def deserialize(obj: Dict[str, int], **_kwargs: Any) -> "ClassCorrect":
+    def deserialize(obj: dict[str, int], **_kwargs: Any) -> ClassCorrect:
         r"""
         Deserialization method
 
         :param obj: object to deserialize
         :param \**_kwargs: optional extra keyword arguments
         :return: deserializes object
         """
@@ -625,25 +629,25 @@
         """
         Initialization of class
 
         :param value: value attribute of class
         """
         self.value = value
 
-    def serialize(self, **_kwargs: "Any") -> "dict":  # type: ignore[type-arg]
+    def serialize(self, **_kwargs: Any) -> dict:  # type: ignore[type-arg]
         r"""
         Serialization method
 
         :param \**_kwargs: optional extra keyword arguments
         :return: serialized object
         """
         return {"value": self.value}
 
     @staticmethod
-    def deserialize(obj: "dict", **_kwargs: "Any") -> "ClassCorrect2":  # type: ignore[type-arg]
+    def deserialize(obj: dict, **_kwargs: Any) -> ClassCorrect2:  # type: ignore[type-arg]
         r"""
         Deserialization method
 
         :param obj: object to deserialize
         :param \**_kwargs: optional extra keyword arguments
         :return: deserializes object
         """
@@ -651,25 +655,25 @@
 
 
 class ClassCorrect3:
     """
     Class that implements serialization logic correctly
     """
 
-    def __init__(self, values: List[int], name: str) -> None:
+    def __init__(self, values: list[int], name: str) -> None:
         """
         Initialization of class
 
         :param values: list of values; values attribute of class
         :param name: name attribute of class
         """
         self.values = values
         self.name = name
 
-    def serialize(self, **_kwargs: "Any") -> Union[bytes, Dict[str, bytes]]:
+    def serialize(self, **_kwargs: Any) -> bytes | dict[str, bytes]:
         r"""
         Serialization method
 
         :param \**_kwargs: optional extra keyword arguments
         :return: serialized object
         """
         return Serialization.serialize(
@@ -677,17 +681,15 @@
                 "values": self.values,
                 "name": self.name,
             },
             use_pickle=True,
         )
 
     @staticmethod
-    def deserialize(
-        obj: Union[bytes, Dict[str, bytes]], **_kwargs: "Any"
-    ) -> "ClassCorrect3":
+    def deserialize(obj: bytes | dict[str, bytes], **_kwargs: Any) -> ClassCorrect3:
         r"""
         Deserialization method
 
         :param obj: object to deserialize
         :param \**_kwargs: optional extra keyword arguments
         :return: deserializes object
         """
@@ -696,131 +698,194 @@
 
 
 class ClassNoKwargs:
     """
     Class that implements correct serialization logic but doesn't use optional keyword arguments.
     """
 
-    def __init__(self, values: List[int], name: str) -> None:
+    def __init__(self, values: list[int], name: str) -> None:
         """
         Initialization of class
 
         :param values: list of values; values attribute of class
         :param name: name attribute of class
         """
         self.values = values
         self.name = name
 
-    def serialize(self) -> Dict[str, Any]:
+    def serialize(self) -> dict[str, Any]:
         """
         Serialization method
 
         :return: serialized object
         """
         return {
             "values": self.values,
             "name": self.name,
         }
 
     @staticmethod
-    def deserialize(obj: Dict[str, Any]) -> "ClassNoKwargs":
+    def deserialize(obj: dict[str, Any]) -> ClassNoKwargs:
         """
         Deserialization method
 
         :param obj: object to deserialize
         :return: deserializes object
         """
         return ClassNoKwargs(obj["values"], obj["name"])
 
 
 class ClassCorrectKwargs(SupportsSerialization):
     """
     Class that implements correct serialization logic making use of additional keyword arguments.
     """
 
-    origin: List[Union[str, HTTPClient]] = []
-    destination: List[Union[str, HTTPClient]] = []
+    origin: list[str | HTTPClient] = []
+    destination: list[str | HTTPClient] = []
 
     def __init__(
-        self, values: List[int], name: str
+        self, values: list[int], name: str
     ):  # pylint: disable=super-init-not-called
         self.values = values
         self.name = name
 
     def serialize(  # type: ignore[override]  # pylint: disable=arguments-differ
-        self, *, destination: Union[str, HTTPClient], **kwargs: Any
-    ) -> Dict[str, Any]:
+        self, *, destination: str | HTTPClient, **_kwargs: Any
+    ) -> dict[str, Any]:
         r"""
         Serialization method
 
         :param destination: Receiver of the message.
-        :param \**kwargs: optional extra keyword arguments
+        :param \**_kwargs: optional extra keyword arguments
         :return: serialized object
         """
         self.destination.append(destination)
         return {
             "values": self.values,
             "name": self.name,
         }
 
     @staticmethod
     def deserialize(  # type: ignore[override]  # pylint: disable=arguments-differ
-        obj: Dict[str, Any],
+        obj: dict[str, Any],
         *,
-        origin: Union[str, HTTPClient],
-        **kwargs: Any,
-    ) -> "ClassCorrectKwargs":
+        origin: str | HTTPClient,
+        **_kwargs: Any,
+    ) -> ClassCorrectKwargs:
         r"""
         Deserialization method
 
         :param obj: object to deserialize
         :param origin: Sender of the message.
-        :param \**kwargs: optional extra keyword arguments
+        :param \**_kwargs: optional extra keyword arguments
         :return: deserializes object
         """
         ClassCorrectKwargs.origin.append(origin)
         return ClassCorrectKwargs(obj["values"], obj["name"])
 
 
 class ClassCorrectKwargs2:
     """
     Class that implements correct serialization logic making use of additional keyword arguments.
     """
 
-    def __init__(self, values: List[int], other: ClassCorrectKwargs):
+    def __init__(self, values: list[int], other: ClassCorrectKwargs):
         self.values = values
         self.other = other
 
-    def serialize(self, **_kwargs: Any) -> Dict[str, Any]:
+    def serialize(self, **_kwargs: Any) -> dict[str, Any]:
         r"""
         Serialization method
 
         :param \**_kwargs: optional extra keyword arguments
         :return: serialized object
         """
         return {
             "values": self.values,
             "other": self.other,
         }
 
     @staticmethod
-    def deserialize(obj: Dict[str, Any], **_kwargs: Any) -> "ClassCorrectKwargs2":
+    def deserialize(obj: dict[str, Any], **_kwargs: Any) -> ClassCorrectKwargs2:
         r"""
         Deserialization method
 
         :param obj: object to deserialize
         :param \**_kwargs: optional extra keyword arguments
-        :return: deserializes object
+        :return: deserialized object
         """
         return ClassCorrectKwargs2(obj["values"], obj["other"])
 
 
+class NestedClassCorrect(SupportsSerialization):
+    """
+    Class that implements serialization logic correctly
+    """
+
+    def __init__(self, value: int) -> None:
+        """
+        Initialization of class
+
+        :param value: value attribute of class
+        """
+        self.instance = ClassCorrect(value)
+
+    def serialize(self, **_kwargs: Any) -> dict[str, ClassCorrect]:
+        r"""
+        Serialization method
+
+        :param \**_kwargs: optional extra keyword arguments
+        :return: serialized object
+        """
+        return {"instance": self.instance}
+
+    @staticmethod
+    def deserialize(obj: dict[str, ClassCorrect], **_kwargs: Any) -> NestedClassCorrect:
+        r"""
+        Deserialization method
+
+        :param obj: object to deserialize
+        :param \**_kwargs: optional extra keyword arguments
+        :return: deserializes object
+        """
+        return NestedClassCorrect(obj["instance"].value)
+
+
+@dataclass
+class MyDataClass:
+    """
+    Dataclass with custom serialization logic
+    """
+
+    attribute: int
+
+    def serialize(self, **_kwargs: Any) -> dict[str, int]:
+        r"""
+        Serialization method
+
+        :param \**_kwargs: optional extra keyword arguments
+        :return: serialized object
+        """
+        return asdict(self)
+
+    @staticmethod
+    def deserialize(obj: dict[str, int], **_kwargs: Any) -> MyDataClass:
+        r"""
+        Deserialization method
+
+        :param obj: object to deserialize
+        :param \**_kwargs: optional extra keyword arguments
+        :return: deserialized object
+        """
+        return MyDataClass(**obj)
+
+
 @pytest.mark.parametrize("correct_class", (ClassCorrect, ClassCorrect2))
 def test_custom_serialization_correct(
-    correct_class: Type[Union[ClassCorrect, ClassCorrect2]]
+    correct_class: type[ClassCorrect | ClassCorrect2],
 ) -> None:
     """
     Tests correctly implemented serialization logic
 
     :param correct_class: a correctly implemented serialization class
     """
     Serialization.clear_serialization_logic()
@@ -833,16 +898,16 @@
     "correct_class, correct_class_2",
     (
         (ClassCorrect2, ClassCorrect3),
         (ClassCorrect, ClassCorrect3),
     ),
 )
 def test_custom_serialization_correct2(
-    correct_class: Type[Union[ClassCorrect, ClassCorrect2]],
-    correct_class_2: Type[ClassCorrect3],
+    correct_class: type[ClassCorrect | ClassCorrect2],
+    correct_class_2: type[ClassCorrect3],
 ) -> None:
     """
     Tests correctly implemented serialization logic
 
     :param correct_class: a correctly implemented serialization class
     :param correct_class_2: a correctly implemented serialization class
     """
@@ -897,14 +962,25 @@
     )
     assert ClassCorrectKwargs.origin == ["origin2"]
     assert ClassCorrectKwargs.destination == ["destination2"]
     ClassCorrectKwargs.origin = []
     ClassCorrectKwargs.destination = []
 
 
+def test_dataclass_serialization() -> None:
+    """
+    Tests packing and unpacking of dataclasses with custom serialization logic
+    """
+    Serialization.clear_serialization_logic()
+    Serialization.register_class(MyDataClass)
+    my_dataclass = MyDataClass(1)
+
+    pack_unpack_test(my_dataclass)
+
+
 def test_ndarray_custom_logic_elements_serialization() -> None:
     """
     Tests packing and unpacking of a numpy array with custom-serialized elements
     """
     Serialization.clear_serialization_logic()
     array_: npt.NDArray[np.int_] = np.array([ClassCorrect(1)])
 
@@ -931,7 +1007,124 @@
     Serialization.register_class(ClassCorrect)
     pack_unpack_test(
         array_,
         compare,
         serial_option=ormsgpack.OPT_SERIALIZE_NUMPY,
         use_pickle=False,
     )
+
+
+def test_series_custom_logic_elements_serialization() -> None:
+    """
+    Tests packing and unpacking of a pandas series with custom-serialized elements
+    """
+    Serialization.clear_serialization_logic()
+    Serialization.register_class(ClassCorrect)
+    series = pd.Series([ClassCorrect(1)])
+
+    def compare(series1: pd.Series[Any], series2: pd.Series[Any]) -> bool:
+        """
+        Check two pandas series that contain a single ClassCorrect element for equality
+
+        :param series1: first series
+        :param series2: second series
+        :return: True if the ClassCorrect elements have the same value
+        """
+
+        return (
+            cast(ClassCorrect, series1[0]).value == cast(ClassCorrect, series2[0]).value
+        )
+
+    pack_unpack_test(
+        series,
+        compare,
+        use_pickle=False,
+    )
+
+
+def test_dataframe_custom_logic_elements_serialization() -> None:
+    """
+    Tests packing and unpacking of a pandas dataframe with custom-serialized elements
+    """
+    Serialization.clear_serialization_logic()
+    Serialization.register_class(ClassCorrect)
+    dataframe = pd.DataFrame({"col1": [ClassCorrect(1)]})
+
+    def compare(df1: pd.DataFrame, df2: pd.DataFrame) -> bool:
+        """
+        Check two pandas dataframes that contain a single ClassCorrect element for equality
+
+        :param df1: first dataframe
+        :param df2: second dataframe
+        :return: True if the ClassCorrect elements have the same value
+        """
+
+        return (
+            cast(ClassCorrect, df1.iloc[0, 0]).value
+            == cast(ClassCorrect, df2.iloc[0, 0]).value
+        )
+
+    pack_unpack_test(
+        dataframe,
+        compare,
+        use_pickle=False,
+    )
+
+
+def test_series_nested_custom_logic_elements_serialization() -> None:
+    """
+    Tests packing and unpacking of a pandas series with nested custom-serialized elements
+    """
+    Serialization.clear_serialization_logic()
+    Serialization.register_class(ClassCorrect)
+    Serialization.register_class(NestedClassCorrect)
+    series = pd.Series([NestedClassCorrect(1)])
+
+    def compare(series1: pd.Series[Any], series2: pd.Series[Any]) -> bool:
+        """
+        Check two pandas series that contain a single NestedClassCorrect element for equality
+
+        :param series1: first series
+        :param series2: second series
+        :return: True if the NestedClassCorrect elements have the same value
+        """
+
+        return (
+            cast(NestedClassCorrect, series1[0]).instance.value
+            == cast(NestedClassCorrect, series2[0]).instance.value
+        )
+
+    pack_unpack_test(
+        series,
+        compare,
+        use_pickle=False,
+    )
+
+
+def test_dataframe_nested_custom_logic_elements_serialization() -> None:
+    """
+    Tests packing and unpacking of a pandas dataframe with nested custom-serialized elements
+    """
+    Serialization.clear_serialization_logic()
+    Serialization.register_class(ClassCorrect)
+    Serialization.register_class(NestedClassCorrect)
+    dataframe = pd.DataFrame({"col1": [NestedClassCorrect(1)]})
+
+    def compare(df1: pd.DataFrame, df2: pd.DataFrame) -> bool:
+        """
+        Check two pandas dataframes that contain a single NestedClassCorrect element for equality
+
+        :param df1: first dataframe
+        :param df2: second dataframe
+        :return: True if the NestedClassCorrect elements have the same value
+        """
+
+        return (
+            cast(NestedClassCorrect, df1.iloc[0, 0]).instance.value
+            == cast(NestedClassCorrect, df2.iloc[0, 0]).instance.value
+        )
+
+    pack_unpack_test(
+        dataframe,
+        compare,
+        use_pickle=False,
+    )
```

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/test_packing_gmpy.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/test_packing_gmpy.py`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/test_pool_creation.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/test_pool_creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 @pytest.mark.parametrize(
     "http_addr, http_port",
     [
         (
             f"{randint(0, 255)}.{randint(0, 255)}.{randint(0, 255)}.{randint(0, 255)}",
             randint(0, 255),
         )
-        for _ in range(100)
+        for _ in range(10)
     ],
 )
 def test_http_client_equality(http_addr: str, http_port: int) -> None:
     """
     Tests whether equality works properly for http clients
 
     :param http_addr: IP address of the HTTP client.
```

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/test_pool_http_3p.py` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/test_pool_http_3p.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 """
 This module tests the communication between three communication pools.
 """
+from __future__ import annotations
+
 import asyncio
-from typing import Any, List, Optional, Tuple
+from typing import Any, Iterable, Sequence
 
 import pytest
+from aiohttp import ClientTimeout
 
 from tno.mpc.communication import Pool
-from tno.mpc.communication.test import (  # pylint: disable=unused-import
-    event_loop,
-    fixture_pool_http_3p,
-)
 
 
-@pytest.mark.asyncio
 async def send_message(
-    pools: Tuple[Pool, ...],
+    pools: Sequence[Pool],
     sender: int,
     receiver: int,
     message: Any,
-    msg_id: Optional[str] = None,
+    msg_id: str | None = None,
 ) -> None:
     """
     Send a message
 
     :param pools: the communication pools to use
     :param sender: the id of the sending party
     :param receiver: the id of the receiving party
     :param message: the message to send
     :param msg_id: the message id to use
     """
-    await pools[sender].send(f"local{receiver}", message, msg_id)
+    await pools[sender].send(
+        f"local{receiver}",
+        message,
+        msg_id,
+        timeout=ClientTimeout(total=2),
+        max_retries=2,
+    )
 
 
-@pytest.mark.asyncio
 async def broadcast_message(
-    pools: Tuple[Pool, ...],
+    pools: Sequence[Pool],
     sender: int,
-    receivers: List[int],
+    receivers: Iterable[int],
     message: Any,
     msg_id: str,
 ) -> None:
     """
     Send a message
 
     :param pools: the communication pools to use
@@ -51,42 +54,40 @@
     :param msg_id: the message id to use
     """
     await pools[sender].broadcast(
         message, msg_id, [f"local{receiver}" for receiver in receivers]
     )
 
 
-@pytest.mark.asyncio
 async def assert_recv_message(
-    pools: Tuple[Pool, ...],
+    pools: Sequence[Pool],
     sender: int,
     receiver: int,
     message: Any,
-    msg_id: Optional[str] = None,
+    msg_id: str | None = None,
 ) -> None:
     """
     Receives a message and validates whether it is in line with the expected message
 
     :param pools: the communication pools to use
     :param sender: the id of the sending party
     :param receiver: the id of the receiving party
     :param message: the expected message
     :param msg_id: the message id of the expected message
     """
     res = await pools[receiver].recv(f"local{sender}", msg_id)
     assert res == message
 
 
-@pytest.mark.asyncio
 async def assert_send_recv_all_message(
-    pools: Tuple[Pool, ...],
+    pools: Sequence[Pool],
     receiver: int,
-    senders: List[int],
+    senders: Iterable[int],
     message: Any,
-    msg_id: Optional[str] = None,
+    msg_id: str | None = None,
 ) -> None:
     """
     Sends a message to one party from each other party and validate whether it is received correctly.
 
     :param pools: the communication pools to use
     :param receiver: the id of the receiving party
     :param senders: the ids of the sending parties.
@@ -103,40 +104,38 @@
     received_from = []
     for sender, received_message in res:
         assert received_message == message
         received_from.append(int(sender[5:]))
     assert sorted(received_from) == sorted(senders)
 
 
-@pytest.mark.asyncio
 async def assert_send_message(
-    pools: Tuple[Pool, ...],
+    pools: Sequence[Pool],
     sender: int,
     receiver: int,
     message: Any,
-    msg_id: Optional[str] = None,
+    msg_id: str | None = None,
 ) -> None:
     """
     Sends a message and validates whether it is received correctly
 
     :param pools: the communication pools to use
     :param sender: the id of the sending party
     :param receiver: the id of the receiving party
     :param message: the message
     :param msg_id: the message id to use
     """
     await send_message(pools, sender, receiver, message, msg_id)
     await assert_recv_message(pools, sender, receiver, message, msg_id)
 
 
-@pytest.mark.asyncio
 async def assert_broadcast_message(
-    pools: Tuple[Pool, ...],
+    pools: Sequence[Pool],
     sender: int,
-    receivers: List[int],
+    receivers: Iterable[int],
     message: Any,
     msg_id: str,
 ) -> None:
     """
     Send a message
 
     :param pools: the communication pools to use
@@ -151,217 +150,219 @@
             assert_recv_message(pools, sender, receiver, message, msg_id)
             for receiver in receivers
         )
     )
 
 
 @pytest.mark.asyncio
-async def test_http_3p_server(pool_http_3p: Tuple[Pool, Pool, Pool]) -> None:
+async def test_http_3p_server(http_pool_trio: tuple[Pool, Pool, Pool]) -> None:
     """
     Tests sending and receiving of multiple messages between three communication pools
 
-    :param pool_http_3p: collection of three communication pools
+    :param http_pool_trio: collection of three communication pools
     """
     await asyncio.gather(
         *(
-            assert_send_message(pool_http_3p, 0, 1, "Hello1!"),
-            assert_send_message(pool_http_3p, 0, 2, "Hello2!"),
-            assert_send_message(pool_http_3p, 1, 0, "Hello3!"),
-            assert_send_message(pool_http_3p, 1, 2, "Hello4!"),
-            assert_send_message(pool_http_3p, 2, 0, "Hello5!"),
-            assert_send_message(pool_http_3p, 2, 1, "Hello6!"),
+            assert_send_message(http_pool_trio, 0, 1, "Hello1!"),
+            assert_send_message(http_pool_trio, 0, 2, "Hello2!"),
+            assert_send_message(http_pool_trio, 1, 0, "Hello3!"),
+            assert_send_message(http_pool_trio, 1, 2, "Hello4!"),
+            assert_send_message(http_pool_trio, 2, 0, "Hello5!"),
+            assert_send_message(http_pool_trio, 2, 1, "Hello6!"),
         )
     )
 
 
 @pytest.mark.asyncio
-async def test_http_3p_server_broadcast(pool_http_3p: Tuple[Pool, Pool, Pool]) -> None:
+async def test_http_3p_server_broadcast(
+    http_pool_trio: tuple[Pool, Pool, Pool]
+) -> None:
     """
     Tests sending and receiving of multiple broadcast messages between three communication pools
 
-    :param pool_http_3p: collection of three communication pools
+    :param http_pool_trio: collection of three communication pools
     """
     await asyncio.gather(
         *(
-            assert_broadcast_message(pool_http_3p, 0, [1, 2], "Hello1!", "id1"),
-            assert_broadcast_message(pool_http_3p, 1, [0, 2], "Hello2!", "id2"),
-            assert_broadcast_message(pool_http_3p, 2, [0, 1], "Hello3!", "id3"),
-            assert_broadcast_message(pool_http_3p, 0, [1], "Hello1!", "id4"),
-            assert_broadcast_message(pool_http_3p, 1, [2], "Hello2!", "id5"),
-            assert_broadcast_message(pool_http_3p, 2, [0], "Hello3!", "id6"),
+            assert_broadcast_message(http_pool_trio, 0, [1, 2], "Hello1!", "id1"),
+            assert_broadcast_message(http_pool_trio, 1, [0, 2], "Hello2!", "id2"),
+            assert_broadcast_message(http_pool_trio, 2, [0, 1], "Hello3!", "id3"),
+            assert_broadcast_message(http_pool_trio, 0, [1], "Hello1!", "id4"),
+            assert_broadcast_message(http_pool_trio, 1, [2], "Hello2!", "id5"),
+            assert_broadcast_message(http_pool_trio, 2, [0], "Hello3!", "id6"),
         )
     )
 
 
 @pytest.mark.asyncio
-async def test_http_3p_server_2(pool_http_3p: Tuple[Pool, Pool, Pool]) -> None:
+async def test_http_3p_server_2(http_pool_trio: tuple[Pool, Pool, Pool]) -> None:
     """
     Tests sending and receiving of multiple messages between three communication pools
 
-    :param pool_http_3p: collection of three communication pools
+    :param http_pool_trio: collection of three communication pools
     """
     await asyncio.gather(
         *(
-            assert_send_message(pool_http_3p, 0, 1, "Hello1!"),
-            assert_send_message(pool_http_3p, 0, 1, "Hello2!"),
-            assert_send_message(pool_http_3p, 0, 1, "Hello1!"),
+            assert_send_message(http_pool_trio, 0, 1, "Hello1!"),
+            assert_send_message(http_pool_trio, 0, 1, "Hello2!"),
+            assert_send_message(http_pool_trio, 0, 1, "Hello1!"),
         )
     )
 
 
 @pytest.mark.asyncio
 async def test_http_3p_server_broadcast_2(
-    pool_http_3p: Tuple[Pool, Pool, Pool]
+    http_pool_trio: tuple[Pool, Pool, Pool]
 ) -> None:
     """
     Tests sending and receiving of multiple broadcast messages between three communication pools
 
-    :param pool_http_3p: collection of three communication pools
+    :param http_pool_trio: collection of three communication pools
     """
     await asyncio.gather(
         *(
-            assert_broadcast_message(pool_http_3p, 0, [1, 2], "Hello1!", "id1"),
-            assert_broadcast_message(pool_http_3p, 0, [1, 2], "Hello2!", "id2"),
-            assert_broadcast_message(pool_http_3p, 0, [1, 2], "Hello3!", "id3"),
-            assert_broadcast_message(pool_http_3p, 0, [1], "Hello1!", "id4"),
-            assert_broadcast_message(pool_http_3p, 0, [2], "Hello2!", "id5"),
+            assert_broadcast_message(http_pool_trio, 0, [1, 2], "Hello1!", "id1"),
+            assert_broadcast_message(http_pool_trio, 0, [1, 2], "Hello2!", "id2"),
+            assert_broadcast_message(http_pool_trio, 0, [1, 2], "Hello3!", "id3"),
+            assert_broadcast_message(http_pool_trio, 0, [1], "Hello1!", "id4"),
+            assert_broadcast_message(http_pool_trio, 0, [2], "Hello2!", "id5"),
         )
     )
 
 
 @pytest.mark.asyncio
-async def test_http_3p_server_3(pool_http_3p: Tuple[Pool, Pool, Pool]) -> None:
+async def test_http_3p_server_3(http_pool_trio: tuple[Pool, Pool, Pool]) -> None:
     """
     Tests sending and receiving of multiple messages between three communication pools
 
-    :param pool_http_3p: collection of three communication pools
+    :param http_pool_trio: collection of three communication pools
     """
     await asyncio.gather(
         *(
-            assert_send_message(pool_http_3p, 0, 1, "Hello1!"),
-            assert_send_message(pool_http_3p, 0, 2, "Hello2!"),
-            assert_send_message(pool_http_3p, 1, 0, "Hello3!"),
-            assert_send_message(pool_http_3p, 1, 2, "Hello4!"),
-            assert_send_message(pool_http_3p, 2, 0, "Hello5!"),
-            assert_send_message(pool_http_3p, 2, 1, "Hello6!"),
-            assert_send_message(pool_http_3p, 0, 1, "Hello7!"),
-            assert_send_message(pool_http_3p, 0, 2, "Hello8!"),
-            assert_send_message(pool_http_3p, 1, 0, "Hello9!"),
-            assert_send_message(pool_http_3p, 1, 2, "Hello10!"),
-            assert_send_message(pool_http_3p, 2, 0, "Hello11!"),
-            assert_send_message(pool_http_3p, 2, 1, "Hello12!"),
+            assert_send_message(http_pool_trio, 0, 1, "Hello1!"),
+            assert_send_message(http_pool_trio, 0, 2, "Hello2!"),
+            assert_send_message(http_pool_trio, 1, 0, "Hello3!"),
+            assert_send_message(http_pool_trio, 1, 2, "Hello4!"),
+            assert_send_message(http_pool_trio, 2, 0, "Hello5!"),
+            assert_send_message(http_pool_trio, 2, 1, "Hello6!"),
+            assert_send_message(http_pool_trio, 0, 1, "Hello7!"),
+            assert_send_message(http_pool_trio, 0, 2, "Hello8!"),
+            assert_send_message(http_pool_trio, 1, 0, "Hello9!"),
+            assert_send_message(http_pool_trio, 1, 2, "Hello10!"),
+            assert_send_message(http_pool_trio, 2, 0, "Hello11!"),
+            assert_send_message(http_pool_trio, 2, 1, "Hello12!"),
         )
     )
 
 
 @pytest.mark.asyncio
-async def test_http_3p_server_msg_id(pool_http_3p: Tuple[Pool, Pool, Pool]) -> None:
+async def test_http_3p_server_msg_id(http_pool_trio: tuple[Pool, Pool, Pool]) -> None:
     """
     Tests sending and receiving of multiple messages between three communication pools with a message id
 
-    :param pool_http_3p: collection of three communication pools
+    :param http_pool_trio: collection of three communication pools
     """
     await asyncio.gather(
         *(
-            assert_send_message(pool_http_3p, 0, 1, "Hello1!", "Msg ID 1"),
-            assert_send_message(pool_http_3p, 0, 1, "Hello2!", "Msg ID 2"),
+            assert_send_message(http_pool_trio, 0, 1, "Hello1!", "Msg ID 1"),
+            assert_send_message(http_pool_trio, 0, 1, "Hello2!", "Msg ID 2"),
         )
     )
 
 
 @pytest.mark.asyncio
 async def test_http_3p_server_mixed_receive(
-    pool_http_3p: Tuple[Pool, Pool, Pool]
+    http_pool_trio: tuple[Pool, Pool, Pool]
 ) -> None:
     """
     Tests sending and receiving of multiple messages of varying types between three communication pools
 
-    :param pool_http_3p: collection of three communication pools
+    :param http_pool_trio: collection of three communication pools
     """
     await asyncio.gather(
         *(
-            send_message(pool_http_3p, 0, 1, "Hello1!"),
-            send_message(pool_http_3p, 2, 1, b"Hello2!"),
-            send_message(pool_http_3p, 0, 1, b"Hello3!"),
-            send_message(pool_http_3p, 2, 1, "Hello4!"),
-            assert_recv_message(pool_http_3p, 2, 1, b"Hello2!"),
-            assert_recv_message(pool_http_3p, 2, 1, "Hello4!"),
-            assert_recv_message(pool_http_3p, 0, 1, "Hello1!"),
-            assert_recv_message(pool_http_3p, 0, 1, b"Hello3!"),
+            send_message(http_pool_trio, 0, 1, "Hello1!"),
+            send_message(http_pool_trio, 2, 1, b"Hello2!"),
+            send_message(http_pool_trio, 0, 1, b"Hello3!"),
+            send_message(http_pool_trio, 2, 1, "Hello4!"),
+            assert_recv_message(http_pool_trio, 2, 1, b"Hello2!"),
+            assert_recv_message(http_pool_trio, 2, 1, "Hello4!"),
+            assert_recv_message(http_pool_trio, 0, 1, "Hello1!"),
+            assert_recv_message(http_pool_trio, 0, 1, b"Hello3!"),
         )
     )
 
 
 @pytest.mark.asyncio
 async def test_http_3p_server_recv_all_mixed(
-    pool_http_3p: Tuple[Pool, Pool, Pool]
+    http_pool_trio: tuple[Pool, Pool, Pool]
 ) -> None:
     """
     Test receiving of a message from each other party using the recv_all method.
 
-    :param pool_http_3p: collection of three communication pools
+    :param http_pool_trio: collection of three communication pools
     """
     await asyncio.gather(
         *(
-            assert_send_recv_all_message(pool_http_3p, 0, [1, 2], "Hello1!", "id1"),
-            assert_send_recv_all_message(pool_http_3p, 0, [1, 2], b"Hello2!", "id2"),
-            assert_send_recv_all_message(pool_http_3p, 0, [1, 2], b"Hello3!", "id3"),
-            assert_send_recv_all_message(pool_http_3p, 0, [1], "Hello1!", "id4"),
-            assert_send_recv_all_message(pool_http_3p, 0, [2], b"Hello2!", "id5"),
+            assert_send_recv_all_message(http_pool_trio, 0, [1, 2], "Hello1!", "id1"),
+            assert_send_recv_all_message(http_pool_trio, 0, [1, 2], b"Hello2!", "id2"),
+            assert_send_recv_all_message(http_pool_trio, 0, [1, 2], b"Hello3!", "id3"),
+            assert_send_recv_all_message(http_pool_trio, 0, [1], "Hello1!", "id4"),
+            assert_send_recv_all_message(http_pool_trio, 0, [2], b"Hello2!", "id5"),
         )
     )
 
 
 @pytest.mark.asyncio
 async def test_http_3p_server_mixed_broadcast(
-    pool_http_3p: Tuple[Pool, Pool, Pool]
+    http_pool_trio: tuple[Pool, Pool, Pool]
 ) -> None:
     """
     Tests sending and receiving of multiple broadcast messages of various types between three communication pools
 
-    :param pool_http_3p: collection of three communication pools
+    :param http_pool_trio: collection of three communication pools
     """
     await asyncio.gather(
         *(
-            assert_broadcast_message(pool_http_3p, 0, [1, 2], "Hello1!", "id1"),
-            assert_broadcast_message(pool_http_3p, 0, [1, 2], b"Hello2!", "id2"),
-            assert_broadcast_message(pool_http_3p, 0, [1, 2], b"Hello3!", "id3"),
-            assert_broadcast_message(pool_http_3p, 0, [1], "Hello1!", "id4"),
-            assert_broadcast_message(pool_http_3p, 0, [2], b"Hello2!", "id5"),
+            assert_broadcast_message(http_pool_trio, 0, [1, 2], "Hello1!", "id1"),
+            assert_broadcast_message(http_pool_trio, 0, [1, 2], b"Hello2!", "id2"),
+            assert_broadcast_message(http_pool_trio, 0, [1, 2], b"Hello3!", "id3"),
+            assert_broadcast_message(http_pool_trio, 0, [1], "Hello1!", "id4"),
+            assert_broadcast_message(http_pool_trio, 0, [2], b"Hello2!", "id5"),
         )
     )
 
 
 @pytest.mark.asyncio
 async def test_broadcast_msg_id_string_prefix(
-    pool_http_3p: Tuple[Pool, Pool, Pool]
+    http_pool_trio: tuple[Pool, Pool, Pool]
 ) -> None:
     """
     Tests asynchronous sending and receiving of a string with a prefixed custom message id between
     three communication pools
 
-    :param pool_http_3p: collection of three communication pools
+    :param http_pool_trio: collection of three communication pools
     """
-    pool_http_3p[0].update_msg_prefix("prefix")
-    pool_http_3p[1].update_msg_prefix("prefix")
-    pool_http_3p[2].update_msg_prefix("prefix")
+    http_pool_trio[0].update_msg_prefix("prefix")
+    http_pool_trio[1].update_msg_prefix("prefix")
+    http_pool_trio[2].update_msg_prefix("prefix")
 
-    await assert_broadcast_message(pool_http_3p, 0, [1, 2], "Hello1!", "id1")
+    await assert_broadcast_message(http_pool_trio, 0, [1, 2], "Hello1!", "id1")
 
 
 @pytest.mark.asyncio
 async def test_broadcast_msg_id_string_prefix_deviation(
-    pool_http_3p: Tuple[Pool, Pool, Pool]
+    http_pool_trio: tuple[Pool, Pool, Pool]
 ) -> None:
     """
     Tests asynchronous sending and receiving of a string with a prefixed custom message id between
     three communication pools
 
-    :param pool_http_3p: collection of three communication pools
+    :param http_pool_trio: collection of three communication pools
     """
-    pool_http_3p[0].update_msg_prefix("prefix")
-    pool_http_3p[1].update_msg_prefix("prefix")
-    pool_http_3p[2].update_msg_prefix("prefix")
-    list(pool_http_3p[0].pool_handlers.values())[0].msg_prefix = "something different"
+    http_pool_trio[0].update_msg_prefix("prefix")
+    http_pool_trio[1].update_msg_prefix("prefix")
+    http_pool_trio[2].update_msg_prefix("prefix")
+    list(http_pool_trio[0].pool_handlers.values())[0].msg_prefix = "something different"
 
     with pytest.raises(ValueError):
-        await assert_broadcast_message(pool_http_3p, 0, [1, 2], "Hello1!", "id1")
+        await assert_broadcast_message(http_pool_trio, 0, [1, 2], "Hello1!", "id1")
```

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/ca-combined.crt` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/ca-combined.crt`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/ca-intermediate.crt` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/ca-intermediate.crt`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/ca-intermediate.pem` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/ca-intermediate.pem`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/ca-root.crt` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/ca-root.crt`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/ca-root.pem` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/ca-root.pem`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_0.crt` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/party_0.crt`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_0.pem` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/party_0.pem`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_1.crt` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/party_1.crt`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_1.pem` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/party_1.pem`

 * *Files identical despite different names*

### Comparing `tno.mpc.communication-4.5.0/src/tno/mpc/communication/test/tls_certs/party_2.crt` & `tno.mpc.communication-4.8.1/src/tno/mpc/communication/test/tls_certs/party_untrusted.crt`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 Certificate:
     Data:
         Version: 1 (0x0)
-        Serial Number: 4 (0x4)
+        Serial Number: 2 (0x2)
         Signature Algorithm: sha256WithRSAEncryption
         Issuer: CN=ca-intermediate
         Validity
-            Not Before: Mar 27 18:01:32 2023 GMT
-            Not After : Aug 12 18:01:32 2050 GMT
-        Subject: CN=party_2
+            Not Before: Jul 18 07:39:58 2023 GMT
+            Not After : Dec  3 07:39:58 2050 GMT
+        Subject: CN=party_0
         Subject Public Key Info:
             Public Key Algorithm: rsaEncryption
                 RSA Public-Key: (2048 bit)
                 Modulus:
-                    00:b8:80:e0:b1:f6:79:b7:03:1d:a8:d5:35:36:fd:
-                    9e:f1:3e:93:65:0b:0e:bf:47:0c:08:fa:bd:22:fd:
-                    e5:42:ce:06:da:84:b0:ce:6d:e2:fa:9e:95:c9:ee:
-                    7a:c9:1f:80:d2:23:7c:c0:80:71:47:0f:c9:62:54:
-                    58:6e:13:e0:09:cf:24:97:d8:30:8b:73:29:05:5c:
-                    b0:f5:21:94:e1:44:e0:4e:d0:3b:1f:7e:d5:3f:fb:
-                    13:c3:c1:ce:84:86:ad:15:a3:82:9f:32:95:16:44:
-                    d1:5b:74:da:8d:7b:e7:3a:d9:25:4b:d7:de:cb:e5:
-                    da:83:dd:a5:55:64:75:bf:ee:52:b6:a8:c7:56:50:
-                    5f:76:24:95:a1:d5:70:3a:c1:6c:04:6e:ca:84:1b:
-                    14:42:1d:01:09:46:7c:c5:0d:fe:eb:31:ea:94:20:
-                    d4:ab:ef:be:2f:1d:53:78:f8:e9:5c:86:30:d8:f6:
-                    dc:61:3c:7b:58:96:5d:59:68:dc:dc:18:c4:e1:4e:
-                    c6:4c:c6:91:3d:1c:5e:6f:6f:b9:18:cc:77:66:bc:
-                    b3:b6:de:f0:12:84:7b:33:b0:f5:98:fa:a2:26:25:
-                    83:69:63:40:75:1b:eb:56:6a:57:45:89:43:4b:86:
-                    80:b3:a3:67:2b:e5:cc:f1:c3:bb:15:b5:e8:cc:97:
-                    92:bd
+                    00:c3:7d:05:11:88:25:48:a5:36:9f:e1:f8:68:10:
+                    59:3e:6b:45:b0:0a:a0:9f:8b:0f:7e:34:3c:c9:84:
+                    c3:d6:f6:9a:fb:b6:99:25:6c:e8:22:84:c8:44:30:
+                    04:49:37:87:2f:29:06:2b:23:67:f4:c1:28:de:dd:
+                    e4:16:69:91:9d:09:58:09:49:fb:dc:cc:4f:a1:51:
+                    fb:70:4f:3d:3f:4f:97:0d:b6:d4:ed:e0:39:5f:72:
+                    95:56:c8:ea:b3:09:ab:5c:15:5c:bd:4f:06:0e:e4:
+                    16:d6:0d:b3:bd:86:74:5a:32:70:d4:5f:44:ff:15:
+                    47:11:23:57:0b:22:e1:ec:90:50:57:de:e5:c1:4a:
+                    18:58:21:ba:46:c1:ba:11:e6:e2:73:ab:72:5e:a1:
+                    83:b4:64:75:58:1a:db:4c:f8:e1:fa:ef:15:bd:b1:
+                    7a:f6:84:a3:1d:35:ec:20:47:1a:f0:42:9d:62:00:
+                    0f:d3:8e:27:27:76:59:21:61:47:22:c7:9f:72:d6:
+                    9c:ed:87:fa:be:22:c4:6d:6c:33:f9:24:35:ea:b3:
+                    2f:f8:91:9c:3a:34:92:23:41:60:2d:71:d3:ff:fa:
+                    ef:2e:b5:a6:11:ff:75:35:10:50:30:4f:fb:77:05:
+                    c7:bd:b7:e3:21:aa:17:f1:70:0b:35:dc:2c:a5:3b:
+                    89:13
                 Exponent: 65537 (0x10001)
     Signature Algorithm: sha256WithRSAEncryption
-         08:6c:82:57:0e:fb:54:c3:b9:1c:ef:4e:80:cf:dd:7a:98:01:
-         cc:ce:11:2f:70:3d:5a:9d:4e:8a:7f:40:62:5a:38:e2:a2:37:
-         dd:0c:50:73:97:71:9e:76:8d:a0:9f:82:38:5a:bf:e5:47:cc:
-         75:5b:ba:3a:d7:51:3c:d9:ef:ae:6c:32:c3:e1:90:3b:7c:fa:
-         53:65:b4:f0:c5:dd:ba:aa:43:98:92:40:ad:fb:3b:13:69:3c:
-         d7:06:c8:e7:b8:59:27:4b:42:cf:b1:af:a9:c8:e2:d6:a7:d6:
-         52:ca:68:d2:f0:72:97:3e:f0:c0:ed:60:da:f7:0e:c5:cc:ee:
-         59:39:26:ee:86:74:81:41:e3:40:dc:42:1d:e6:12:ab:5e:52:
-         04:cb:7c:eb:e7:9a:d1:f5:f8:71:80:9a:d6:8d:ee:0d:c9:99:
-         92:b0:e4:56:c5:7c:7f:0f:cc:76:50:de:56:59:3d:a3:e2:36:
-         d8:43:d3:87:1a:36:b0:34:f5:06:73:c7:05:65:c0:56:8c:a4:
-         0b:c2:0f:c5:18:51:f5:82:4a:43:62:a7:30:3d:93:61:f8:3a:
-         9c:89:f0:63:4f:e4:7a:85:f8:ec:9b:0e:b4:c4:9f:78:82:a4:
-         86:0a:86:bb:a9:cc:63:8c:f4:5d:b3:2c:d0:3a:6b:6e:ff:d6:
-         03:e4:de:1c
+         d9:61:56:b8:0f:67:96:28:d7:0e:72:36:b8:b5:b4:af:56:ac:
+         3a:5e:77:d6:f4:ce:d0:a4:d3:09:e7:ab:5b:ec:78:d6:c2:41:
+         47:60:73:67:b6:70:dc:dc:4d:6e:b7:2b:f3:69:2a:a4:d4:69:
+         e4:8e:d5:6a:62:d7:9e:f2:e3:fd:ce:78:e2:a0:49:f4:66:87:
+         8e:ed:24:f3:72:f5:44:4d:62:c3:64:95:ee:61:c2:d2:e8:a9:
+         dd:1f:84:ad:e2:be:e6:51:72:1c:b8:c3:ea:cf:60:30:65:b2:
+         68:de:b5:ba:81:1d:f6:4c:f9:35:2d:56:a0:01:42:a0:ed:8f:
+         23:5c:87:cc:2b:18:f6:98:00:b7:14:ad:9c:fc:54:b8:4c:b6:
+         ae:7d:b8:cf:6c:72:ff:84:2d:bf:cc:5e:97:1c:d2:1b:7b:26:
+         27:00:99:3b:56:b4:33:70:a8:a4:15:c6:ed:9b:96:2e:20:f5:
+         de:65:9b:88:68:4f:1a:ff:42:e5:8e:2e:09:af:6d:df:5e:0c:
+         04:54:7e:d1:75:8e:f8:2f:4e:a4:c4:26:e7:e8:b1:4e:08:24:
+         49:65:3b:bd:b9:36:a9:f2:28:45:68:42:e9:d8:e3:29:0c:91:
+         cd:a2:ee:5c:9f:f4:3e:3d:83:2b:8d:bb:e8:0e:57:c6:33:6b:
+         4c:f4:82:b2
 -----BEGIN CERTIFICATE-----
-MIICojCCAYoCAQQwDQYJKoZIhvcNAQELBQAwGjEYMBYGA1UEAwwPY2EtaW50ZXJt
-ZWRpYXRlMCAXDTIzMDMyNzE4MDEzMloYDzIwNTAwODEyMTgwMTMyWjASMRAwDgYD
-VQQDDAdwYXJ0eV8yMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAuIDg
-sfZ5twMdqNU1Nv2e8T6TZQsOv0cMCPq9Iv3lQs4G2oSwzm3i+p6Vye56yR+A0iN8
-wIBxRw/JYlRYbhPgCc8kl9gwi3MpBVyw9SGU4UTgTtA7H37VP/sTw8HOhIatFaOC
-nzKVFkTRW3TajXvnOtklS9fey+Xag92lVWR1v+5StqjHVlBfdiSVodVwOsFsBG7K
-hBsUQh0BCUZ8xQ3+6zHqlCDUq+++Lx1TePjpXIYw2PbcYTx7WJZdWWjc3BjE4U7G
-TMaRPRxeb2+5GMx3Zryztt7wEoR7M7D1mPqiJiWDaWNAdRvrVmpXRYlDS4aAs6Nn
-K+XM8cO7FbXozJeSvQIDAQABMA0GCSqGSIb3DQEBCwUAA4IBAQAIbIJXDvtUw7kc
-706Az916mAHMzhEvcD1anU6Kf0BiWjjiojfdDFBzl3Gedo2gn4I4Wr/lR8x1W7o6
-11E82e+ubDLD4ZA7fPpTZbTwxd26qkOYkkCt+zsTaTzXBsjnuFknS0LPsa+pyOLW
-p9ZSymjS8HKXPvDA7WDa9w7FzO5ZOSbuhnSBQeNA3EId5hKrXlIEy3zr55rR9fhx
-gJrWje4NyZmSsORWxXx/D8x2UN5WWT2j4jbYQ9OHGjawNPUGc8cFZcBWjKQLwg/F
-GFH1gkpDYqcwPZNh+DqcifBjT+R6hfjsmw60xJ94gqSGCoa7qcxjjPRdsyzQOmtu
-/9YD5N4c
+MIICojCCAYoCAQIwDQYJKoZIhvcNAQELBQAwGjEYMBYGA1UEAwwPY2EtaW50ZXJt
+ZWRpYXRlMCAXDTIzMDcxODA3Mzk1OFoYDzIwNTAxMjAzMDczOTU4WjASMRAwDgYD
+VQQDDAdwYXJ0eV8wMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAw30F
+EYglSKU2n+H4aBBZPmtFsAqgn4sPfjQ8yYTD1vaa+7aZJWzoIoTIRDAESTeHLykG
+KyNn9MEo3t3kFmmRnQlYCUn73MxPoVH7cE89P0+XDbbU7eA5X3KVVsjqswmrXBVc
+vU8GDuQW1g2zvYZ0WjJw1F9E/xVHESNXCyLh7JBQV97lwUoYWCG6RsG6Eebic6ty
+XqGDtGR1WBrbTPjh+u8VvbF69oSjHTXsIEca8EKdYgAP044nJ3ZZIWFHIsefctac
+7Yf6viLEbWwz+SQ16rMv+JGcOjSSI0FgLXHT//rvLrWmEf91NRBQME/7dwXHvbfj
+IaoX8XALNdwspTuJEwIDAQABMA0GCSqGSIb3DQEBCwUAA4IBAQDZYVa4D2eWKNcO
+cja4tbSvVqw6XnfW9M7QpNMJ56tb7HjWwkFHYHNntnDc3E1utyvzaSqk1GnkjtVq
+Ytee8uP9znjioEn0ZoeO7STzcvVETWLDZJXuYcLS6KndH4St4r7mUXIcuMPqz2Aw
+ZbJo3rW6gR32TPk1LVagAUKg7Y8jXIfMKxj2mAC3FK2c/FS4TLaufbjPbHL/hC2/
+zF6XHNIbeyYnAJk7VrQzcKikFcbtm5YuIPXeZZuIaE8a/0Llji4Jr23fXgwEVH7R
+dY74L06kxCbn6LFOCCRJZTu9uTap8ihFaELp2OMpDJHNou5cn/Q+PYMrjbvoDlfG
+M2tM9IKy
 -----END CERTIFICATE-----
```

### Comparing `tno.mpc.communication-4.5.0/src/tno.mpc.communication.egg-info/PKG-INFO` & `tno.mpc.communication-4.8.1/src/tno.mpc.communication.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,80 @@
 Metadata-Version: 2.1
 Name: tno.mpc.communication
-Version: 4.5.0
+Version: 4.8.1
 Summary: MPC Communication module
-Author-email: TNO MPC Lab <mpclab@tno.nl>
-Maintainer-email: TNO MPC Lab <mpclab@tno.nl>
+Author-email: TNO PET Lab <petlab@tno.nl>
+Maintainer-email: TNO PET Lab <petlab@tno.nl>
 License: Apache License, Version 2.0
-Project-URL: Homepage, https://mpc.tno.nl/
-Project-URL: Documentation, https://docs.mpc.tno.nl/communication/4.5.0
+Project-URL: Homepage, https://pet.tno.nl/
+Project-URL: Documentation, https://docs.pet.tno.nl/mpc/communication/4.8.1
 Project-URL: Source, https://github.com/TNO-MPC/communication
 Keywords: TNO,MPC,multi-party computation,communication
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Typing :: Typed
 Classifier: Topic :: Security :: Cryptography
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: bitarray
 Provides-Extra: gmpy
 Provides-Extra: gmpy2
+Provides-Extra: bitarray
 Provides-Extra: numpy
 Provides-Extra: pandas
 Provides-Extra: tls
 Provides-Extra: tests
 License-File: LICENSE
 
-# TNO MPC Lab - Communication
+# TNO PET Lab - secure Multi-Party Computation (MPC) - Communication
 
-The TNO MPC lab consists of generic software components, procedures, and
+The TNO PET Lab consists of generic software components, procedures, and
 functionalities developed and maintained on a regular basis to facilitate and
-aid in the development of MPC solutions. The lab is a cross-project initiative
-allowing us to integrate and reuse previously developed MPC functionalities to
+aid in the development of PET solutions. The lab is a cross-project initiative
+allowing us to integrate and reuse previously developed PET functionalities to
 boost the development of new protocols and solutions.
 
 The package tno.mpc.communication is part of the TNO Python Toolbox.
 
 _Limitations in (end-)use: the content of this repository may solely be used for
 applications that comply with international export control laws._  
 _This implementation of cryptographic software has not been audited. Use at your
 own risk._
 
 ## Documentation
 
 Documentation of the tno.mpc.communication package can be found
-[here](https://docs.mpc.tno.nl/communication/4.5.0).
+[here](https://docs.pet.tno.nl/mpc/communication/4.8.1).
 
 ## Install
 
 Easily install the tno.mpc.communication package using pip:
 
 ```console
 $ python -m pip install tno.mpc.communication
 ```
 
-If you wish to run the tests you can use:
+Note: The package specifies several optional dependency groups:
 
-```console
-$ python -m pip install 'tno.mpc.communication[tests]'
-```
+- `gmpy`: Adds support for sending various `gmpy2` types
+- `tests`: Includes all optional libraries required to run the full test suite
+- `tls`: Required if SSL is needed
+- `bitarray`: Adds support for sending `bitarray` types
+- `numpy`: Adds support for sending `numpy` types
+- `pandas`: Adds support for sending `pandas` types
+
+See [sending, receiving messages](#sending-receiving-messages) for more
+information on the supported third party types. Optional dependencies can be
+installed by specifying their names in brackets after the package name, e.g.
+when using `pip install`, use `pip install tno.mpc.communication[extra1,extra2]`
+to install the groups `extra1` and `extra2`.
 
 ## Usage
 
 The communication module uses `async` functions for sending and receiving. If
 you are familiar with the async module, you can skip to the `Pools` section.
 
 ### Async explanation
@@ -435,7 +444,60 @@
 >>> python bob.py
 2022-07-07 09:36:16,915 - tno.mpc.communication.httphandlers - INFO - Serving on 127.0.0.1:61002
 2022-07-07 09:36:20,223 - tno.mpc.communication.httphandlers - INFO - Received message from 127.0.0.1:61001
 Hello Bob! This is Alice speaking.
 2022-07-07 09:36:20,232 - tno.mpc.communication.httphandlers - INFO - HTTPServer: Shutting down server task
 2022-07-07 09:36:20,256 - tno.mpc.communication.httphandlers - INFO - Server 127.0.0.1:61002 shutdown
 ```
+
+## Test fixtures
+
+The `tno.mpc.communication` package exports several pytest fixtures as pytest
+plugins to facilitate the user in testing with pool objects. The fixtures take
+care of all configuration and clean-up of the pool objects so that you don't
+have to worry about that.
+
+Usage:
+
+```py
+# test_my_module.py
+import pytest
+from typing import Callable
+from tno.mpc.communication import Pool
+
+def test_with_two_pools(http_pool_duo: tuple[Pool, Pool]) -> None:
+    sender, receiver = http_pool_duo
+    # ... your code
+
+def test_with_three_pools(http_pool_trio: tuple[Pool, Pool, Pool]) -> None:
+    alice, bob, charlie = http_pool_trio
+    # ... your code
+
+@pytest.mark.parameterize("n_players", (2, 3, 4))
+def test_with_variable_pools(
+    n_players: int,
+    http_pool_group_factory: Callable[[int], tuple[Pool, ...]],
+) -> None:
+    pools = http_pool_group_factory(n_players)
+    # ... your code
+```
+
+### Fixture scope
+
+The scope of the fixtures can be set dynamically through the
+`--fixture-pool-scope`
+[option to pytest](https://docs.pytest.org/en/7.1.x/reference/reference.html#configuration-options).
+_Note that this will also change the scope of the global `event_loop` fixture
+that is provided by `pytest-asyncio`._ By default, in line with
+`pytest_asyncio`, the scope of all our fixtures is `"function"`. We advise to
+configure a larger scope (e.g. `"session"`, `"package"` or `"module"`) when
+possible to reduce test set-up and teardown time.
+
+Our fixtures pass `True` to the `port_reuse` argument of `aiohttp.web.TCPSite`.
+Their
+[documentation](https://docs.aiohttp.org/en/stable/web_reference.html?highlight=reuse_port#aiohttp.web.TCPSite)
+states that this option is not supported on Windows (outside of WSL). If you
+experience any issues, please disable the plugin by adding
+`-p no:pytest_tno.tno.mpc.communication.pytest_pool_fixtures` to your pytest
+configuration. Note that without `port_reuse` the tests may crash, as the test
+may try to bind to ports which may not have been freed by the operating system.
+For more reliable testing, run the tests on a WSL / Linux platform.
```

### Comparing `tno.mpc.communication-4.5.0/src/tno.mpc.communication.egg-info/SOURCES.txt` & `tno.mpc.communication-4.8.1/src/tno.mpc.communication.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 CITATION.cff
 LICENSE
 README.md
+entry_points.txt
 pyproject.toml
+src/pytest_tno/tno/mpc/communication/__init__.py
+src/pytest_tno/tno/mpc/communication/py.typed
+src/pytest_tno/tno/mpc/communication/pytest_pool_fixtures.py
+src/pytest_tno/tno/mpc/communication/test/test_fixtures.py
 src/tno.mpc.communication.egg-info/PKG-INFO
 src/tno.mpc.communication.egg-info/SOURCES.txt
 src/tno.mpc.communication.egg-info/dependency_links.txt
+src/tno.mpc.communication.egg-info/entry_points.txt
 src/tno.mpc.communication.egg-info/requires.txt
 src/tno.mpc.communication.egg-info/top_level.txt
 src/tno/mpc/communication/__init__.py
 src/tno/mpc/communication/exceptions.py
 src/tno/mpc/communication/functions.py
 src/tno/mpc/communication/httphandlers.py
 src/tno/mpc/communication/pool.py
@@ -26,26 +32,23 @@
 src/tno/mpc/communication/test/conftest.py
 src/tno/mpc/communication/test/pool_fixtures_http.py
 src/tno/mpc/communication/test/test_packing.py
 src/tno/mpc/communication/test/test_packing_gmpy.py
 src/tno/mpc/communication/test/test_pool_creation.py
 src/tno/mpc/communication/test/test_pool_http_2p.py
 src/tno/mpc/communication/test/test_pool_http_3p.py
-src/tno/mpc/communication/test/test_pool_https_3p.py
+src/tno/mpc/communication/test/test_pool_https_2p.py
 src/tno/mpc/communication/test/tls_certs/README.md
 src/tno/mpc/communication/test/tls_certs/ca-combined.crt
 src/tno/mpc/communication/test/tls_certs/ca-intermediate.crt
 src/tno/mpc/communication/test/tls_certs/ca-intermediate.pem
 src/tno/mpc/communication/test/tls_certs/ca-root.crt
 src/tno/mpc/communication/test/tls_certs/ca-root.pem
+src/tno/mpc/communication/test/tls_certs/ca-untrusted.crt
 src/tno/mpc/communication/test/tls_certs/party_0.crt
 src/tno/mpc/communication/test/tls_certs/party_0.pem
 src/tno/mpc/communication/test/tls_certs/party_1.crt
 src/tno/mpc/communication/test/tls_certs/party_1.pem
-src/tno/mpc/communication/test/tls_certs/party_2.crt
-src/tno/mpc/communication/test/tls_certs/party_2.pem
-src/tno/mpc/communication/test/tls_certs/party_3.crt
-src/tno/mpc/communication/test/tls_certs/party_3.pem
-src/tno/mpc/communication/test/tls_certs/party_4.crt
-src/tno/mpc/communication/test/tls_certs/party_4.pem
+src/tno/mpc/communication/test/tls_certs/party_untrusted.crt
+src/tno/mpc/communication/test/tls_certs/party_untrusted.pem
 stubs/gmpy2.pyi
 stubs/pyarrow.pyi
```

### Comparing `tno.mpc.communication-4.5.0/stubs/gmpy2.pyi` & `tno.mpc.communication-4.8.1/stubs/gmpy2.pyi`

 * *Files identical despite different names*

