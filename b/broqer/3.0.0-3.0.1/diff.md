# Comparing `tmp/broqer-3.0.0.tar.gz` & `tmp/broqer-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "broqer-3.0.0.tar", last modified: Thu Sep 29 15:06:07 2022, max compression
+gzip compressed data, was "broqer-3.0.1.tar", last modified: Thu Aug  3 14:34:13 2023, max compression
```

## Comparing `broqer-3.0.0.tar` & `broqer-3.0.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 15:06:07.226326 broqer-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 15:06:07.218326 broqer-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 15:06:07.222326 broqer-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-09-29 15:05:27.000000 broqer-3.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-09-29 15:05:27.000000 broqer-3.0.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-09-29 15:05:27.000000 broqer-3.0.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 15:06:07.222326 broqer-3.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-09-29 15:05:27.000000 broqer-3.0.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-09-29 15:05:27.000000 broqer-3.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     3524 2022-09-29 15:05:27.000000 broqer-3.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-29 15:05:27.000000 broqer-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10767 2022-09-29 15:06:07.226326 broqer-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9916 2022-09-29 15:05:27.000000 broqer-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 15:06:07.222326 broqer-3.0.0/broqer/
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-29 15:06:07.000000 broqer-3.0.0/broqer/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4652 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/coro_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/disposable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/error_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 15:06:07.222326 broqer-3.0.0/broqer/op/
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/op/bitwise.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/op/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     4638 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/op/combine_latest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5065 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/op/filter_.py
--rw-r--r--   0 runner    (1001) docker     (121)     3849 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/op/map_.py
--rw-r--r--   0 runner    (1001) docker     (121)     6089 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/op/map_async.py
--rw-r--r--   0 runner    (1001) docker     (121)     4307 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/op/py_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2344 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/op/throttle.py
--rw-r--r--   0 runner    (1001) docker     (121)     3835 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6032 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/operator_overloading.py
--rw-r--r--   0 runner    (1001) docker     (121)    10796 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 15:06:07.222326 broqer-3.0.0/broqer/publishers/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/publishers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/publishers/poll.py
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 15:06:07.222326 broqer-3.0.0/broqer/subscribers/
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/subscribers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2117 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/subscribers/on_emit_future.py
--rw-r--r--   0 runner    (1001) docker     (121)     3512 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/subscribers/sink.py
--rw-r--r--   0 runner    (1001) docker     (121)     4394 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/subscribers/sink_async.py
--rw-r--r--   0 runner    (1001) docker     (121)     1783 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/subscribers/trace.py
--rw-r--r--   0 runner    (1001) docker     (121)     2396 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/timer.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-09-29 15:05:27.000000 broqer-3.0.0/broqer/value.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 15:06:07.222326 broqer-3.0.0/broqer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10767 2022-09-29 15:06:07.000000 broqer-3.0.0/broqer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-09-29 15:06:07.000000 broqer-3.0.0/broqer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-29 15:06:07.000000 broqer-3.0.0/broqer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-29 15:06:00.000000 broqer-3.0.0/broqer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-29 15:06:07.000000 broqer-3.0.0/broqer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 15:06:07.226326 broqer-3.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)   164101 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/example1.svg
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/hub.rst
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8301 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 15:06:07.226326 broqer-3.0.0/docs/operators/
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/accumulate.rst
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/cache.rst
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/catch_exception.rst
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/combine_latest.rst
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/debounce.rst
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/delay.rst
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/filter.rst
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/map.rst
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/map_async.rst
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/map_threaded.rst
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/merge.rst
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/partition.rst
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/reduce.rst
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/replace.rst
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/sample.rst
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/sliding_window.rst
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/switch.rst
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators/throttle.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/operators.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/overview.gnumeric
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/publishers.rst
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/subjects.rst
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-29 15:05:27.000000 broqer-3.0.0/docs/subscribers.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 15:06:07.226326 broqer-3.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-09-29 15:05:27.000000 broqer-3.0.0/examples/await.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-09-29 15:05:27.000000 broqer-3.0.0/examples/from_polling.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-09-29 15:05:27.000000 broqer-3.0.0/examples/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-09-29 15:05:27.000000 broqer-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-09-29 15:05:27.000000 broqer-3.0.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-09-29 15:06:07.230326 broqer-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-09-29 15:05:27.000000 broqer-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 15:06:07.226326 broqer-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12329 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/eventloop.py
--rw-r--r--   0 runner    (1001) docker     (121)     3675 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/helper_multi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/helper_single.py
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/test_core_disposable.py
--rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/test_core_publisher.py
--rw-r--r--   0 runner    (1001) docker     (121)    11426 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/test_core_publisher_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     6290 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/test_coro_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/test_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2073 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/test_op_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/test_op_combine_latest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2924 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/test_op_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/test_op_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/test_op_on_emit_future.py
--rw-r--r--   0 runner    (1001) docker     (121)     4209 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/test_op_sink.py
--rw-r--r--   0 runner    (1001) docker     (121)     3387 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/test_op_throttle.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-09-29 15:05:27.000000 broqer-3.0.0/tests/test_publishers_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:34:13.789576 broqer-3.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:34:13.773576 broqer-3.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:34:13.777576 broqer-3.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-03 14:33:26.000000 broqer-3.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-03 14:33:26.000000 broqer-3.0.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-03 14:33:26.000000 broqer-3.0.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:34:13.777576 broqer-3.0.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-03 14:33:26.000000 broqer-3.0.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-03 14:33:26.000000 broqer-3.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-03 14:33:26.000000 broqer-3.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-03 14:33:26.000000 broqer-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-08-03 14:34:13.789576 broqer-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-08-03 14:33:26.000000 broqer-3.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:34:13.777576 broqer-3.0.1/broqer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 14:34:13.000000 broqer-3.0.1/broqer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/coro_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/disposable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/error_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:34:13.781576 broqer-3.0.1/broqer/op/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/op/bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/op/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/op/combine_latest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/op/filter_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/op/map_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/op/map_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/op/py_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/op/throttle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/operator_overloading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:34:13.781576 broqer-3.0.1/broqer/publishers/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/publishers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/publishers/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:34:13.781576 broqer-3.0.1/broqer/subscribers/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/subscribers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/subscribers/on_emit_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/subscribers/sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/subscribers/sink_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/subscribers/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-03 14:33:26.000000 broqer-3.0.1/broqer/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:34:13.777576 broqer-3.0.1/broqer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-08-03 14:34:13.000000 broqer-3.0.1/broqer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-03 14:34:13.000000 broqer-3.0.1/broqer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:34:13.000000 broqer-3.0.1/broqer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:34:06.000000 broqer-3.0.1/broqer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 14:34:13.000000 broqer-3.0.1/broqer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:34:13.781576 broqer-3.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   164101 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/example1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/hub.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:34:13.785576 broqer-3.0.1/docs/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/accumulate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/catch_exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/combine_latest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/debounce.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/delay.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/filter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/map.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/map_async.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/map_threaded.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/merge.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/partition.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/reduce.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/replace.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/sample.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/sliding_window.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/switch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators/throttle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/operators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/overview.gnumeric
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/publishers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/subjects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-03 14:33:26.000000 broqer-3.0.1/docs/subscribers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:34:13.785576 broqer-3.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-03 14:33:26.000000 broqer-3.0.1/examples/await.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-03 14:33:26.000000 broqer-3.0.1/examples/from_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-03 14:33:26.000000 broqer-3.0.1/examples/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-03 14:33:26.000000 broqer-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-03 14:33:26.000000 broqer-3.0.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-03 14:34:13.789576 broqer-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-03 14:33:26.000000 broqer-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:34:13.789576 broqer-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/helper_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/helper_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/test_core_disposable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/test_core_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/test_core_publisher_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/test_coro_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/test_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/test_op_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/test_op_combine_latest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/test_op_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/test_op_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/test_op_on_emit_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/test_op_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/test_op_throttle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-03 14:33:26.000000 broqer-3.0.1/tests/test_publishers_poll.py
```

### Comparing `broqer-3.0.0/.github/workflows/build.yml` & `broqer-3.0.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/.github/workflows/deploy.yml` & `broqer-3.0.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/.vscode/launch.json` & `broqer-3.0.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/CHANGELOG.md` & `broqer-3.0.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+## 3.0.1
+
+* merge #43: wheel dependency updated
+* fixing #43: fixed wrong reference of internal module
+
 ## 3.0.0
 
-* fixed typo ("orginator" fixed to "origintator")
+* fixed typo ("orginator" fixed to "originator")
 * add log output for default error_handler
 * add `dependent_subscribe` function for `Values`
 * remove `OperatorFactory` logic from operators
 * remove `Concat` operator
 * add `CoroQueue` to be used in `MapAsync` and `SinkAsync`
 
 ## 2.4.0
```

### Comparing `broqer-3.0.0/CONTRIBUTING.rst` & `broqer-3.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/LICENSE` & `broqer-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/PKG-INFO` & `broqer-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broqer
-Version: 3.0.0
+Version: 3.0.1
 Summary: Carefully crafted library to operate with continuous streams of data in a reactive style with publish/subscribe and broker functionality.
 Home-page: https://github.com/semiversus/python-broqer
 Author: Günther Jena
 Author-email: guenther@jena.at
 License: MIT license
 Keywords: broker publisher subscriber reactive frp observable
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `broqer-3.0.0/README.rst` & `broqer-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/__init__.py` & `broqer-3.0.1/broqer/__init__.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/coro_queue.py` & `broqer-3.0.1/broqer/coro_queue.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/disposable.py` & `broqer-3.0.1/broqer/disposable.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/error_handler.py` & `broqer-3.0.1/broqer/error_handler.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/op/__init__.py` & `broqer-3.0.1/broqer/op/__init__.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/op/bitwise.py` & `broqer-3.0.1/broqer/op/bitwise.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/op/cache.py` & `broqer-3.0.1/broqer/op/cache.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/op/combine_latest.py` & `broqer-3.0.1/broqer/op/combine_latest.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/op/filter_.py` & `broqer-3.0.1/broqer/op/filter_.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/op/map_.py` & `broqer-3.0.1/broqer/op/map_.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/op/map_async.py` & `broqer-3.0.1/broqer/op/map_async.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/op/py_operators.py` & `broqer-3.0.1/broqer/op/py_operators.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/op/throttle.py` & `broqer-3.0.1/broqer/op/throttle.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/operator.py` & `broqer-3.0.1/broqer/operator.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/operator_overloading.py` & `broqer-3.0.1/broqer/operator_overloading.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ This module enables the operator overloading of publishers """
 import math
 import operator
 from typing import Any as Any_
 
 # pylint: disable=cyclic-import
 import broqer
-from broqer import Publisher
+from broqer import Publisher, op
 from broqer.operator import Operator
 
 
 class MapConstant(Operator):
     """ MapConstant TODO Docstring """
     def __init__(self, publisher: Publisher, value, operation) -> None:
         Operator.__init__(self)
@@ -121,15 +121,15 @@
     for method in (
             '__lt__', '__le__', '__eq__', '__ne__', '__ge__', '__gt__',
             '__add__', '__and__', '__lshift__', '__mod__', '__mul__',
             '__pow__', '__rshift__', '__sub__', '__xor__', '__concat__',
             '__getitem__', '__floordiv__', '__truediv__'):
         def _op(operand_left, operand_right, operation=method):
             if isinstance(operand_right, Publisher):
-                return broqer.op.CombineLatest(operand_left, operand_right,
+                return op.CombineLatest(operand_left, operand_right,
                                                map_=getattr(operator,
                                                             operation))
             return MapConstant(operand_left, operand_right,
                                getattr(operator, operation))
 
         setattr(Publisher, method, _op)
```

### Comparing `broqer-3.0.0/broqer/publisher.py` & `broqer-3.0.1/broqer/publisher.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/publishers/poll.py` & `broqer-3.0.1/broqer/publishers/poll.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/subscriber.py` & `broqer-3.0.1/broqer/subscriber.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/subscribers/__init__.py` & `broqer-3.0.1/broqer/subscribers/__init__.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/subscribers/on_emit_future.py` & `broqer-3.0.1/broqer/subscribers/on_emit_future.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/subscribers/sink.py` & `broqer-3.0.1/broqer/subscribers/sink.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/subscribers/sink_async.py` & `broqer-3.0.1/broqer/subscribers/sink_async.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/subscribers/trace.py` & `broqer-3.0.1/broqer/subscribers/trace.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/timer.py` & `broqer-3.0.1/broqer/timer.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer/value.py` & `broqer-3.0.1/broqer/value.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/broqer.egg-info/PKG-INFO` & `broqer-3.0.1/broqer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broqer
-Version: 3.0.0
+Version: 3.0.1
 Summary: Carefully crafted library to operate with continuous streams of data in a reactive style with publish/subscribe and broker functionality.
 Home-page: https://github.com/semiversus/python-broqer
 Author: Günther Jena
 Author-email: guenther@jena.at
 License: MIT license
 Keywords: broker publisher subscriber reactive frp observable
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `broqer-3.0.0/broqer.egg-info/SOURCES.txt` & `broqer-3.0.1/broqer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/docs/Makefile` & `broqer-3.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/docs/conf.py` & `broqer-3.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/docs/example1.svg` & `broqer-3.0.1/docs/example1.svg`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/docs/introduction.rst` & `broqer-3.0.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/docs/logo.svg` & `broqer-3.0.1/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/docs/operators.rst` & `broqer-3.0.1/docs/operators.rst`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/docs/overview.gnumeric` & `broqer-3.0.1/docs/overview.gnumeric`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/setup.py` & `broqer-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/eventloop.py` & `broqer-3.0.1/tests/eventloop.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/helper_multi.py` & `broqer-3.0.1/tests/helper_multi.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/helper_single.py` & `broqer-3.0.1/tests/helper_single.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/test_core_disposable.py` & `broqer-3.0.1/tests/test_core_disposable.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/test_core_publisher.py` & `broqer-3.0.1/tests/test_core_publisher.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/test_core_publisher_operators.py` & `broqer-3.0.1/tests/test_core_publisher_operators.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/test_coro_queue.py` & `broqer-3.0.1/tests/test_coro_queue.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/test_error_handler.py` & `broqer-3.0.1/tests/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/test_op_bitwise.py` & `broqer-3.0.1/tests/test_op_bitwise.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/test_op_combine_latest.py` & `broqer-3.0.1/tests/test_op_combine_latest.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/test_op_filter.py` & `broqer-3.0.1/tests/test_op_filter.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/test_op_map.py` & `broqer-3.0.1/tests/test_op_map.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/test_op_on_emit_future.py` & `broqer-3.0.1/tests/test_op_on_emit_future.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/test_op_sink.py` & `broqer-3.0.1/tests/test_op_sink.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/test_op_throttle.py` & `broqer-3.0.1/tests/test_op_throttle.py`

 * *Files identical despite different names*

### Comparing `broqer-3.0.0/tests/test_publishers_poll.py` & `broqer-3.0.1/tests/test_publishers_poll.py`

 * *Files identical despite different names*

