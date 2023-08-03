# Comparing `tmp/flumine-2.4.1.tar.gz` & `tmp/flumine-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flumine-2.4.1.tar", last modified: Tue Jul 25 07:29:30 2023, max compression
+gzip compressed data, was "dist/flumine-2.4.2.tar", last modified: Thu Aug  3 08:40:53 2023, max compression
```

## Comparing `flumine-2.4.1.tar` & `flumine-2.4.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-25 07:29:30.000000 flumine-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-25 07:29:04.000000 flumine-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17065 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/baseflumine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/clients/baseclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/clients/betconnectclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/clients/betfairclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/clients/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/clients/simulatedclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/controls/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/controls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/controls/clientcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/controls/loggingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/controls/tradingcontrols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/execution/baseexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/execution/betfairexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/execution/simulatedexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/execution/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/flumine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/markets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/markets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/markets/blotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/markets/market.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/markets/markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14302 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/markets/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/order/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/order/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/order/orderpackage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/order/ordertype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/order/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/order/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/order/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/patching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24869 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/simulation/simulatedorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/simulation/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/strategy/runnercontext.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/strategy/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/streams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/basestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/datastream.py
--rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/historicalstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/marketstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/orderstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/simulatedorderstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/sportsdatastream.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 07:29:30.000000 flumine-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-25 07:29:04.000000 flumine-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24925 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_baseflumine.py
--rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_blotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_clientcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    19619 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    63899 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_flumine.py
--rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_fluminesimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_loggingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    21248 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_orderpackage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_ordertype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_runnercontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_simulated_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    61695 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_simulatedorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    40617 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_tradingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:53.000000 flumine-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-08-03 08:40:53.000000 flumine-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-08-03 08:40:33.000000 flumine-2.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/baseflumine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/clients/baseclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/clients/betconnectclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/clients/betfairclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/clients/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/clients/simulatedclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/controls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/controls/clientcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/controls/loggingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/controls/tradingcontrols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/execution/baseexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/execution/betfairexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/execution/simulatedexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/execution/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/flumine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine/markets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/markets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/markets/blotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/markets/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/markets/markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14302 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/markets/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine/order/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/order/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/order/orderpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/order/ordertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/order/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/order/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/order/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/patching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24869 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/simulation/simulatedorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/simulation/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/strategy/runnercontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/strategy/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/streams/basestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/streams/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/streams/historicalstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/streams/marketstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/streams/orderstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/streams/simulatedorderstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/streams/sportsdatastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/streams/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-08-03 08:40:33.000000 flumine-2.4.2/flumine/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 08:40:53.000000 flumine-2.4.2/flumine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:40:53.000000 flumine-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-03 08:40:33.000000 flumine-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:53.000000 flumine-2.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25004 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_baseflumine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_blotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_clientcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19619 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63899 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_flumine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_fluminesimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_loggingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21248 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_orderpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_ordertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_runnercontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_simulated_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61695 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_simulatedorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40617 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_tradingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-08-03 08:40:33.000000 flumine-2.4.2/tests/test_worker.py
```

### Comparing `flumine-2.4.1/PKG-INFO` & `flumine-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flumine
-Version: 2.4.1
+Version: 2.4.2
 Summary: Betting trading framework
 Home-page: https://github.com/betcode-org/flumine
 Author: Liam Pauling
 Author-email: a@unknown.com
 License: MIT
 Description: <p align="center">
           <a href="https://github.com/betcode-org">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flumine Version: 2.4.1 Summary: Betting trading
+Metadata-Version: 2.1 Name: flumine Version: 2.4.2 Summary: Betting trading
 framework Home-page: https://github.com/betcode-org/flumine Author: Liam
 Pauling Author-email: a@unknown.com License: MIT Description:
                           [docs/images/logo-full.png]
 # flÅ«mine ![Build Status](https://github.com/betcode-org/flumine/actions/
 workflows/test.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/
 github/liampauling/flumine/badge.svg?branch=master)](https://coveralls.io/
 github/liampauling/flumine?branch=master) [![PyPI version](https://
```

### Comparing `flumine-2.4.1/README.md` & `flumine-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/__init__.py` & `flumine-2.4.2/flumine/__init__.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/baseflumine.py` & `flumine-2.4.2/flumine/baseflumine.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,24 +218,23 @@
     def _process_raw_data(self, event: events.RawDataEvent) -> None:
         stream_id, clk, publish_time, data = event.event
         for datum in data:
             if "id" in datum:
                 market_id = datum["id"]
                 market = self.markets.markets.get(market_id)
                 if market is None:
-                    self._add_market(market_id, None)
+                    market = self._add_market(market_id, None)
                 elif market.closed:
                     self.markets.add_market(market_id, market)
 
-                if (
-                    "marketDefinition" in datum
-                    and datum["marketDefinition"]["status"] == "CLOSED"
-                ):
-                    datum["_stream_id"] = stream_id
-                    self.handler_queue.put(events.CloseMarketEvent(datum))
+                if "marketDefinition" in datum:
+                    market.update_market_catalogue = True
+                    if datum["marketDefinition"]["status"] == "CLOSED":
+                        datum["_stream_id"] = stream_id
+                        self.handler_queue.put(events.CloseMarketEvent(datum))
 
             for strategy in self.strategies:
                 if stream_id in strategy.stream_ids:
                     utils.call_process_raw_data(strategy, clk, publish_time, datum)
 
     def _process_market_catalogues(self, event: events.MarketCatalogueEvent) -> None:
         for market_catalogue in event.event:
```

### Comparing `flumine-2.4.1/flumine/clients/baseclient.py` & `flumine-2.4.2/flumine/clients/baseclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/clients/betconnectclient.py` & `flumine-2.4.2/flumine/clients/betconnectclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/clients/betfairclient.py` & `flumine-2.4.2/flumine/clients/betfairclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/clients/clients.py` & `flumine-2.4.2/flumine/clients/clients.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/clients/simulatedclient.py` & `flumine-2.4.2/flumine/clients/simulatedclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/config.py` & `flumine-2.4.2/flumine/config.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/controls/__init__.py` & `flumine-2.4.2/flumine/controls/__init__.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/controls/clientcontrols.py` & `flumine-2.4.2/flumine/controls/clientcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/controls/loggingcontrols.py` & `flumine-2.4.2/flumine/controls/loggingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/controls/tradingcontrols.py` & `flumine-2.4.2/flumine/controls/tradingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/events/events.py` & `flumine-2.4.2/flumine/events/events.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/exceptions.py` & `flumine-2.4.2/flumine/exceptions.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/execution/baseexecution.py` & `flumine-2.4.2/flumine/execution/baseexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/execution/betfairexecution.py` & `flumine-2.4.2/flumine/execution/betfairexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/execution/simulatedexecution.py` & `flumine-2.4.2/flumine/execution/simulatedexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/execution/transaction.py` & `flumine-2.4.2/flumine/execution/transaction.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/flumine.py` & `flumine-2.4.2/flumine/flumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/markets/blotter.py` & `flumine-2.4.2/flumine/markets/blotter.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/markets/market.py` & `flumine-2.4.2/flumine/markets/market.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/markets/markets.py` & `flumine-2.4.2/flumine/markets/markets.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/markets/middleware.py` & `flumine-2.4.2/flumine/markets/middleware.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/order/order.py` & `flumine-2.4.2/flumine/order/order.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/order/orderpackage.py` & `flumine-2.4.2/flumine/order/orderpackage.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/order/ordertype.py` & `flumine-2.4.2/flumine/order/ordertype.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/order/process.py` & `flumine-2.4.2/flumine/order/process.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/order/responses.py` & `flumine-2.4.2/flumine/order/responses.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/order/trade.py` & `flumine-2.4.2/flumine/order/trade.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/patching.py` & `flumine-2.4.2/flumine/patching.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/simulation/simulatedorder.py` & `flumine-2.4.2/flumine/simulation/simulatedorder.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/simulation/simulation.py` & `flumine-2.4.2/flumine/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/simulation/utils.py` & `flumine-2.4.2/flumine/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/strategy/runnercontext.py` & `flumine-2.4.2/flumine/strategy/runnercontext.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/strategy/strategy.py` & `flumine-2.4.2/flumine/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/streams/basestream.py` & `flumine-2.4.2/flumine/streams/basestream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/streams/datastream.py` & `flumine-2.4.2/flumine/streams/datastream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/streams/historicalstream.py` & `flumine-2.4.2/flumine/streams/historicalstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/streams/marketstream.py` & `flumine-2.4.2/flumine/streams/marketstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/streams/orderstream.py` & `flumine-2.4.2/flumine/streams/orderstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/streams/simulatedorderstream.py` & `flumine-2.4.2/flumine/streams/simulatedorderstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/streams/sportsdatastream.py` & `flumine-2.4.2/flumine/streams/sportsdatastream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/streams/streams.py` & `flumine-2.4.2/flumine/streams/streams.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/utils.py` & `flumine-2.4.2/flumine/utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine/worker.py` & `flumine-2.4.2/flumine/worker.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/flumine.egg-info/PKG-INFO` & `flumine-2.4.2/flumine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flumine
-Version: 2.4.1
+Version: 2.4.2
 Summary: Betting trading framework
 Home-page: https://github.com/betcode-org/flumine
 Author: Liam Pauling
 Author-email: a@unknown.com
 License: MIT
 Description: <p align="center">
           <a href="https://github.com/betcode-org">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flumine Version: 2.4.1 Summary: Betting trading
+Metadata-Version: 2.1 Name: flumine Version: 2.4.2 Summary: Betting trading
 framework Home-page: https://github.com/betcode-org/flumine Author: Liam
 Pauling Author-email: a@unknown.com License: MIT Description:
                           [docs/images/logo-full.png]
 # flÅ«mine ![Build Status](https://github.com/betcode-org/flumine/actions/
 workflows/test.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/
 github/liampauling/flumine/badge.svg?branch=master)](https://coveralls.io/
 github/liampauling/flumine?branch=master) [![PyPI version](https://
```

### Comparing `flumine-2.4.1/flumine.egg-info/SOURCES.txt` & `flumine-2.4.2/flumine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/setup.py` & `flumine-2.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_baseflumine.py` & `flumine-2.4.2/tests/test_baseflumine.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,14 +248,15 @@
             12345,
             [{"id": "1.23", "marketDefinition": {"status": "CLOSED"}}],
         )
         self.base_flumine._process_raw_data(mock_event)
         mock__add_market.assert_called_with("1.23", None)
         mock_queue.put.assert_called_with(mock_events.CloseMarketEvent())
         self.assertEqual(mock_event.event[3][0]["_stream_id"], mock_event.event[0])
+        self.assertTrue(mock__add_market.return_value.update_market_catalogue)
 
     @mock.patch("flumine.baseflumine.BaseFlumine._add_market")
     def test__process_raw_data_no_id(self, mock__add_market):
         mock_event = mock.Mock()
         mock_event.event = (12, "AAA", 12345, [{"mid": "1.23"}])
         self.base_flumine._process_raw_data(mock_event)
         mock__add_market.assert_not_called()
```

### Comparing `flumine-2.4.1/tests/test_blotter.py` & `flumine-2.4.2/tests/test_blotter.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_clientcontrols.py` & `flumine-2.4.2/tests/test_clientcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_clients.py` & `flumine-2.4.2/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_config.py` & `flumine-2.4.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_events.py` & `flumine-2.4.2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_execution.py` & `flumine-2.4.2/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_flumine.py` & `flumine-2.4.2/tests/test_flumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_fluminesimulation.py` & `flumine-2.4.2/tests/test_fluminesimulation.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_integration.py` & `flumine-2.4.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_loggingcontrols.py` & `flumine-2.4.2/tests/test_loggingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_markets.py` & `flumine-2.4.2/tests/test_markets.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_middleware.py` & `flumine-2.4.2/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_order.py` & `flumine-2.4.2/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_orderpackage.py` & `flumine-2.4.2/tests/test_orderpackage.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_ordertype.py` & `flumine-2.4.2/tests/test_ordertype.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_process.py` & `flumine-2.4.2/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_responses.py` & `flumine-2.4.2/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_runnercontext.py` & `flumine-2.4.2/tests/test_runnercontext.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_simulated_utils.py` & `flumine-2.4.2/tests/test_simulated_utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_simulatedorder.py` & `flumine-2.4.2/tests/test_simulatedorder.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_strategy.py` & `flumine-2.4.2/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_streams.py` & `flumine-2.4.2/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_trade.py` & `flumine-2.4.2/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_tradingcontrols.py` & `flumine-2.4.2/tests/test_tradingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_transaction.py` & `flumine-2.4.2/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_utils.py` & `flumine-2.4.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.1/tests/test_worker.py` & `flumine-2.4.2/tests/test_worker.py`

 * *Files identical despite different names*

