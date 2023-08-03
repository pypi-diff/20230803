# Comparing `tmp/kestrel-lang-1.7.3.tar.gz` & `tmp/kestrel-lang-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kestrel-lang-1.7.3.tar", last modified: Thu Jul 27 01:47:34 2023, max compression
+gzip compressed data, was "kestrel-lang-1.7.4.tar", last modified: Thu Aug  3 18:46:30 2023, max compression
```

## Comparing `kestrel-lang-1.7.3.tar` & `kestrel-lang-1.7.4.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.922964 kestrel-lang-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-07-27 01:47:34.922964 kestrel-lang-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/bin/kestrel
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/bin/stix-shifter-diag
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-27 01:47:34.926964 kestrel-lang-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.910963 kestrel-lang-1.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/src/kestrel/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/src/kestrel/absinterface/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/absinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/absinterface/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/src/kestrel/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/analytics/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/analytics/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/src/kestrel/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/prefetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/src/kestrel/datasource/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/datasource/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/datasource/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/datasource/retstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/src/kestrel/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/semantics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/semantics/completor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/semantics/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/semantics/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/src/kestrel/symboltable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/symboltable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/symboltable/symtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/symboltable/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.918964 kestrel-lang-1.7.3/src/kestrel/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/syntax/ecgpattern.lark
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/syntax/ecgpattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/syntax/kestrel.lark
--rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/syntax/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/syntax/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/syntax/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.918964 kestrel-lang-1.7.3/src/kestrel_analytics_docker/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_analytics_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_analytics_docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_analytics_docker/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.918964 kestrel-lang-1.7.3/src/kestrel_analytics_python/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_analytics_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_analytics_python/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_analytics_python/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.918964 kestrel-lang-1.7.3/src/kestrel_datasource_stixbundle/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixbundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixbundle/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.918964 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.918964 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/transmitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.918964 kestrel-lang-1.7.3/src/kestrel_lang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-07-27 01:47:34.000000 kestrel-lang-1.7.3/src/kestrel_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-27 01:47:34.000000 kestrel-lang-1.7.3/src/kestrel_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 01:47:34.000000 kestrel-lang-1.7.3/src/kestrel_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-27 01:47:34.000000 kestrel-lang-1.7.3/src/kestrel_lang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 01:47:34.000000 kestrel-lang-1.7.3/src/kestrel_lang.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.922964 kestrel-lang-1.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_disp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_find.py
--rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_python_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_records.py
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_stixshifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_stixshifter_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_stixshifter_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_timestamped.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.811784 kestrel-lang-1.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-08-03 18:46:30.811784 kestrel-lang-1.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.795784 kestrel-lang-1.7.4/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/bin/kestrel
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/bin/stix-shifter-diag
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-03 18:46:30.811784 kestrel-lang-1.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.795784 kestrel-lang-1.7.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.795784 kestrel-lang-1.7.4/src/kestrel/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.795784 kestrel-lang-1.7.4/src/kestrel/absinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/absinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/absinterface/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.799784 kestrel-lang-1.7.4/src/kestrel/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/analytics/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/analytics/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.799784 kestrel-lang-1.7.4/src/kestrel/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/codegen/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/codegen/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/codegen/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/codegen/prefetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/codegen/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/codegen/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/codegen/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.799784 kestrel-lang-1.7.4/src/kestrel/datasource/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/datasource/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/datasource/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/datasource/retstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.799784 kestrel-lang-1.7.4/src/kestrel/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/semantics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/semantics/completor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/semantics/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/semantics/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.799784 kestrel-lang-1.7.4/src/kestrel/symboltable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/symboltable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/symboltable/symtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/symboltable/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.803784 kestrel-lang-1.7.4/src/kestrel/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/syntax/ecgpattern.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/syntax/ecgpattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/syntax/kestrel.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/syntax/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/syntax/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/syntax/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.803784 kestrel-lang-1.7.4/src/kestrel_analytics_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_analytics_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_analytics_docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_analytics_docker/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.803784 kestrel-lang-1.7.4/src/kestrel_analytics_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_analytics_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_analytics_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_analytics_python/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.803784 kestrel-lang-1.7.4/src/kestrel_datasource_stixbundle/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_datasource_stixbundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_datasource_stixbundle/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.803784 kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.807784 kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/worker/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/worker/transmitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.807784 kestrel-lang-1.7.4/src/kestrel_lang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-08-03 18:46:30.000000 kestrel-lang-1.7.4/src/kestrel_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-08-03 18:46:30.000000 kestrel-lang-1.7.4/src/kestrel_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 18:46:30.000000 kestrel-lang-1.7.4/src/kestrel_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-03 18:46:30.000000 kestrel-lang-1.7.4/src/kestrel_lang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-03 18:46:30.000000 kestrel-lang-1.7.4/src/kestrel_lang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:46:30.811784 kestrel-lang-1.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_command_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_command_disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_command_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_command_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_command_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_command_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_command_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_command_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_command_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_command_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_python_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_stixshifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_stixshifter_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_stixshifter_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-08-03 18:46:09.000000 kestrel-lang-1.7.4/tests/test_timestamped.py
```

### Comparing `kestrel-lang-1.7.3/AUTHORS.rst` & `kestrel-lang-1.7.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/LICENSE.md` & `kestrel-lang-1.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/PKG-INFO` & `kestrel-lang-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.7.3
+Version: 1.7.4
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
```

### Comparing `kestrel-lang-1.7.3/README.rst` & `kestrel-lang-1.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/setup.cfg` & `kestrel-lang-1.7.4/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kestrel-lang
-version = 1.7.3
+version = 1.7.4
 description = Kestrel Threat Hunting Language
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 keywords = 
 	domain specific language
 	cyber threat hunting
 	extended detection and response
@@ -34,16 +34,16 @@
 	lxml>=4.9.3
 	lark>=1.1.5
 	pandas>=2.0.0
 	pyarrow>=5.0.0
 	docker>=5.0.0
 	requests>=2.31.0
 	nest-asyncio>=1.5.6
-	stix-shifter==5.3.1
-	stix-shifter-utils==5.3.1
+	stix-shifter==6.0.3
+	stix-shifter-utils==6.0.3
 	firepit>=2.3.25
 tests_require = 
 	pytest
 
 [options.packages.find]
 where = src
```

### Comparing `kestrel-lang-1.7.3/src/kestrel/__main__.py` & `kestrel-lang-1.7.4/src/kestrel/__main__.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/absinterface/manager.py` & `kestrel-lang-1.7.4/src/kestrel/absinterface/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/analytics/interface.py` & `kestrel-lang-1.7.4/src/kestrel/analytics/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/analytics/manager.py` & `kestrel-lang-1.7.4/src/kestrel/analytics/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/codegen/commands.py` & `kestrel-lang-1.7.4/src/kestrel/codegen/commands.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/codegen/data.py` & `kestrel-lang-1.7.4/src/kestrel/codegen/data.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/codegen/display.py` & `kestrel-lang-1.7.4/src/kestrel/codegen/display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/codegen/prefetch.py` & `kestrel-lang-1.7.4/src/kestrel/codegen/prefetch.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/codegen/queries.py` & `kestrel-lang-1.7.4/src/kestrel/codegen/queries.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/codegen/relations.py` & `kestrel-lang-1.7.4/src/kestrel/codegen/relations.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/codegen/summary.py` & `kestrel-lang-1.7.4/src/kestrel/codegen/summary.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/config.py` & `kestrel-lang-1.7.4/src/kestrel/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/config.yaml` & `kestrel-lang-1.7.4/src/kestrel/config.yaml`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/datasource/interface.py` & `kestrel-lang-1.7.4/src/kestrel/datasource/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/datasource/manager.py` & `kestrel-lang-1.7.4/src/kestrel/datasource/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/datasource/retstruct.py` & `kestrel-lang-1.7.4/src/kestrel/datasource/retstruct.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/exceptions.py` & `kestrel-lang-1.7.4/src/kestrel/exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/semantics/completor.py` & `kestrel-lang-1.7.4/src/kestrel/semantics/completor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/semantics/processor.py` & `kestrel-lang-1.7.4/src/kestrel/semantics/processor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/semantics/reference.py` & `kestrel-lang-1.7.4/src/kestrel/semantics/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/session.py` & `kestrel-lang-1.7.4/src/kestrel/session.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/symboltable/variable.py` & `kestrel-lang-1.7.4/src/kestrel/symboltable/variable.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/syntax/ecgpattern.py` & `kestrel-lang-1.7.4/src/kestrel/syntax/ecgpattern.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/syntax/kestrel.lark` & `kestrel-lang-1.7.4/src/kestrel/syntax/kestrel.lark`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,17 @@
                   | info
                   | save
 
 //
 // All commands
 //
 
-find: "FIND"i ENTITY_TYPE RELATION (REVERSED)? VARIABLE where_clause? limit_clause? timespan?
+find: "FIND"i ENTITY_TYPE RELATION (REVERSED)? VARIABLE where_clause? timespan? limit_clause?
 
-get: "GET"i ENTITY_TYPE ("FROM"i datasource)? where_clause limit_clause? timespan?
+get: "GET"i ENTITY_TYPE ("FROM"i datasource)? where_clause timespan? limit_clause?
 
 group: "GROUP"i VARIABLE BY grp_spec ("WITH"i agg_list)?
 
 join: "JOIN"i VARIABLE "," VARIABLE (BY ATTRIBUTE "," ATTRIBUTE)?
 
 load: "LOAD"i stdpath ("AS"i ENTITY_TYPE)?
 
@@ -143,16 +143,16 @@
 //
 
 grp_spec: grp_expr ("," grp_expr)*
 
 grp_expr: ATTRIBUTE
         | bin_func
 
-bin_func: "BIN"i "(" ATTRIBUTE "," INT timeunit? ")"
 // No other scalar funcs are supported yet
+bin_func: "BIN"i "(" ATTRIBUTE "," INT timeunit? ")"
 
 agg_list: agg ("," agg)*
 
 agg: funcname "(" ATTRIBUTE ")" ("AS"i alias)?
 
 ?funcname: (MIN|MAX|SUM|AVG|COUNT|NUNIQUE)
 MIN: "MIN"i
```

### Comparing `kestrel-lang-1.7.3/src/kestrel/syntax/parser.py` & `kestrel-lang-1.7.4/src/kestrel/syntax/parser.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/syntax/reference.py` & `kestrel-lang-1.7.4/src/kestrel/syntax/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/syntax/utils.py` & `kestrel-lang-1.7.4/src/kestrel/syntax/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel/utils.py` & `kestrel-lang-1.7.4/src/kestrel/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel_analytics_docker/config.py` & `kestrel-lang-1.7.4/src/kestrel_analytics_docker/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel_analytics_docker/interface.py` & `kestrel-lang-1.7.4/src/kestrel_analytics_docker/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel_analytics_python/config.py` & `kestrel-lang-1.7.4/src/kestrel_analytics_python/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel_analytics_python/interface.py` & `kestrel-lang-1.7.4/src/kestrel_analytics_python/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel_datasource_stixbundle/interface.py` & `kestrel-lang-1.7.4/src/kestrel_datasource_stixbundle/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/config.py` & `kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/connector.py` & `kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/connector.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 STIX_SHIFTER_HOMEPAGE = "https://github.com/opencybersecurityalliance/stix-shifter"
 
 
 def get_package_name(connector_name):
     return "stix-shifter-modules-" + connector_name.replace("_", "-")
 
 
-def verify_package_origin(connector_name, stixshifter_version):
+def verify_package_origin(connector_name, stixshifter_version, requests_verify=True):
     _logger.debug("go to PyPI to verify package genuineness from STIX-shifter project")
     package_name = get_package_name(connector_name)
 
     try:
-        pypi_response = requests.get(f"https://pypi.org/project/{package_name}")
+        pypi_response = requests.get(
+            f"https://pypi.org/project/{package_name}", verify=requests_verify
+        )
         pypi_etree = html.fromstring(pypi_response.content)
     except:
         raise DataSourceError(
             f'STIX-shifter connector for "{connector_name}" is not installed '
             f'and Kestrel guessed Python package name "{package_name}" but failed to locate it at PyPI',
             "please verify the connector name and manually install the connector package using "
             f"`pip install {package_name}=={stixshifter_version}`",
@@ -54,21 +56,21 @@
             "please find the correct STIX-shifter connector Python package to install. "
             "And report to Kestrel developers about this malicious package",
         )
 
     _logger.info(f'"{package_name}" verified as a STIX-shifter package.')
 
 
-def install_package(connector_name):
+def install_package(connector_name, requests_verify=True):
     package_name = get_package_name(connector_name)
     _logger.debug(f"guess the connector package name: {package_name}")
 
     stixshifter_version = version("stix_shifter")
 
-    verify_package_origin(connector_name, stixshifter_version)
+    verify_package_origin(connector_name, stixshifter_version, requests_verify)
 
     package_w_ver = package_name + "==" + stixshifter_version
 
     _logger.info(f'install Python package "{package_w_ver}".')
     try:
         subprocess.check_call([sys.executable, "-m", "pip", "install", package_w_ver])
     except:
@@ -83,15 +85,15 @@
             f'STIX-shifter connector for "{connector_name}" is not installed '
             f'and Kestrel failed to install the possible Python package "{package_name}"',
             "please manually install the corresponding STIX-shifter connector Python package using "
             f"`pip install {package_name}=={stixshifter_version}`",
         )
 
 
-def ensure_version_consistency(connector_name):
+def ensure_version_consistency(connector_name, requests_verify=True):
     """Check if the installed connector package has the same version as
     stix-shifter If the version is different, uninstall connector
     package and the install the same version as stix-shifter
 
     """
     stixshifter_version = version("stix_shifter")
     package_name = get_package_name(connector_name)
@@ -106,21 +108,21 @@
     _logger.info(f'uninstalling Python package "{package_w_ver}".')
     try:
         subprocess.check_call(
             [sys.executable, "-m", "pip", "uninstall", "--yes", package_w_ver]
         )
     except:
         _logger.info(f"failed to uninstall package {package_w_ver}")
-    install_package(connector_name)
+    install_package(connector_name, requests_verify)
 
 
-def check_module_availability(connector_name):
+def check_module_availability(connector_name, requests_verify=True):
     try:
         importlib.import_module(
             "stix_shifter_modules." + connector_name + ".entry_point"
         )
 
-        ensure_version_consistency(connector_name)
+        ensure_version_consistency(connector_name, requests_verify)
 
     except:
         _logger.info(f'miss STIX-shifter connector "{connector_name}"')
-        install_package(connector_name)
+        install_package(connector_name, requests_verify)
```

### Comparing `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/diagnosis.py` & `kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/diagnosis.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,28 +80,34 @@
     def diagnose_translate_query(self, stix_pattern, quiet=False):
         if not quiet:
             print()
             print()
             print()
             print("## Diagnose: stix-shifter query translation")
 
+        if not quiet:
+            print()
+            print("#### Input: STIX pattern")
+            print(stix_pattern)
+
         dsl = translate_query(
             self.connector_name,
             {},
             stix_pattern,
             self.connection_dict,
         )
 
+        if "queries" not in dsl:
+            raise Exception(str(dsl))
+
         if not quiet:
             print()
-            print("#### Input pattern")
-            print(stix_pattern)
-            print()
-            print("#### Output data source native query")
-            print(json.dumps(dsl, indent=4))
+            print(f"#### Output: {len(dsl['queries'])} data source native queries")
+            for query in dsl["queries"]:
+                print(query)
 
         return dsl
 
     def diagnose_run_query_and_retrieval_result(self, stix_patterns, max_batch_cnt):
         print()
         print()
         print()
```

### Comparing `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/interface.py` & `kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,20 +88,24 @@
 
         $ export STIXSHIFTER_HOST101_CONNECTOR=elastic_ecs
         $ export STIXSHIFTER_HOST101_CONNECTION='{"host":"elastic.securitylog.company.com", "port":9200, "indices":"host101"}'
         $ export STIXSHIFTER_HOST101_CONFIG='{"auth":{"id":"VuaCfGcBCdbkQm-e5aOx", "api_key":"ui2lp2axTNmsyakw9tvNnw"}}'
 
 #. any in-session edit through the ``CONFIG`` command.
 
-Once you added data source profiles into ``stixshifter.yaml``, you can test the data source with command:
+After added data source profiles into ``stixshifter.yaml``, you can test the data source:
 
 .. code-block:: console
 
     $ stix-shifter-diag data_source_name
 
+where ``data_source_name`` is any profile named in the ``stixshifter.yaml`` config file, usually used in ``FROM stixshifter://data_source_name`` in the ``GET`` command.
+
+The diagnosis utility will check config, test query translation, try connect to the data source to execute a small and a large query, and retrieve data back. Details of all steps will be printed for diagnosis purpose.
+
 If you launch Kestrel in debug mode, STIX-shifter debug mode is still not
 enabled by default. To record debug level logs of STIX-shifter, create
 environment variable ``KESTREL_STIXSHIFTER_DEBUG`` with any value.
 
 .. _STIX-shifter: https://github.com/opencybersecurityalliance/stix-shifter
 .. _elastic_ecs config: https://github.com/opencybersecurityalliance/stix-shifter/blob/develop/stix_shifter_modules/elastic_ecs/configuration/lang_en.json
 .. _stix_shifter_modules/lang_en.json: https://github.com/opencybersecurityalliance/stix-shifter/blob/develop/stix_shifter_modules/lang_en.json
```

### Comparing `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/multiproc.py` & `kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/multiproc.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/query.py` & `kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/query.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/translator.py` & `kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/worker/translator.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/transmitter.py` & `kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/worker/transmitter.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/utils.py` & `kestrel-lang-1.7.4/src/kestrel_datasource_stixshifter/worker/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/src/kestrel_lang.egg-info/PKG-INFO` & `kestrel-lang-1.7.4/src/kestrel_lang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.7.3
+Version: 1.7.4
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
```

### Comparing `kestrel-lang-1.7.3/src/kestrel_lang.egg-info/SOURCES.txt` & `kestrel-lang-1.7.4/src/kestrel_lang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_cli.py` & `kestrel-lang-1.7.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_command_assign.py` & `kestrel-lang-1.7.4/tests/test_command_assign.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_command_disp.py` & `kestrel-lang-1.7.4/tests/test_command_disp.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_command_find.py` & `kestrel-lang-1.7.4/tests/test_command_find.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_command_get.py` & `kestrel-lang-1.7.4/tests/test_command_get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -201,16 +201,16 @@
 def test_get_single_stixshifter_stix_bundle_limit(set_no_prefetch_kestrel_config, set_stixshifter_stix_bundles):
     with Session() as s:
         # default data source schema is stixshifter
         stmt = """
                var = GET process
                      FROM HOST2
                      WHERE [ipv4-addr:value = '127.0.0.1']
-                     LIMIT 4
                      START 2019-01-01T00:00:00Z STOP 2023-01-01T00:00:00Z
+                     LIMIT 4
                """
 
         s.execute(stmt)
         v = s.get_variable("var")
         assert len(v) == 4
         for i in range(len(v)):
             assert v[i]["type"] == "process"
@@ -260,16 +260,16 @@
 def test_get_multiple_stixshifter_stix_bundles_limit(set_no_prefetch_kestrel_config, set_stixshifter_stix_bundles):
     with Session() as s:
         # default data source schema is stixshifter
         stmt = """
                var = GET process
                      FROM HOST1,HOST2
                      WHERE ipv4-addr:value = '127.0.0.1'
-                     LIMIT 10
                      START 2019-01-01T00:00:00Z STOP 2023-01-01T00:00:00Z
+                     LIMIT 10
                """
 
         s.execute(stmt)
         v = s.get_variable("var")
 
         # The extended graph [ipv4-addr:value = '127.0.0.1'] is recognized and
         # merged to prefetch query, resultsing in limited (32) processes. If
@@ -299,16 +299,16 @@
 def test_get_multiple_stixshifter_stix_bundles_limit_1(set_no_prefetch_kestrel_config, set_stixshifter_stix_bundles):
     with Session() as s:
         # default data source schema is stixshifter
         stmt = """
                var = GET process
                      FROM HOST1,HOST2
                      WHERE ipv4-addr:value = '127.0.0.1'
-                     LIMIT 15
                      START 2019-01-01T00:00:00Z STOP 2023-01-01T00:00:00Z
+                     LIMIT 15
                """
 
         s.execute(stmt)
         v = s.get_variable("var")
 
         # The extended graph [ipv4-addr:value = '127.0.0.1'] is recognized and
         # merged to prefetch query, resultsing in limited (32) processes. If
@@ -338,16 +338,16 @@
 def test_get_multiple_stixshifter_stix_bundles_limit_2(set_no_prefetch_kestrel_config, set_stixshifter_stix_bundles):
     with Session() as s:
         # default data source schema is stixshifter
         stmt = """
                var = GET process
                      FROM HOST1,HOST2
                      WHERE ipv4-addr:value = '127.0.0.1'
-                     LIMIT 50
                      START 2019-01-01T00:00:00Z STOP 2023-01-01T00:00:00Z
+                     LIMIT 50
                """
 
         s.execute(stmt)
         v = s.get_variable("var")
 
         # The extended graph [ipv4-addr:value = '127.0.0.1'] is recognized and
         # merged to prefetch query, resultsing in limited (32) processes. If
```

### Comparing `kestrel-lang-1.7.3/tests/test_command_group.py` & `kestrel-lang-1.7.4/tests/test_command_group.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_command_internal.py` & `kestrel-lang-1.7.4/tests/test_command_internal.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_command_join.py` & `kestrel-lang-1.7.4/tests/test_command_join.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_command_load.py` & `kestrel-lang-1.7.4/tests/test_command_load.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_command_merge.py` & `kestrel-lang-1.7.4/tests/test_command_merge.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_command_new.py` & `kestrel-lang-1.7.4/tests/test_command_new.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_command_save.py` & `kestrel-lang-1.7.4/tests/test_command_save.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_completion.py` & `kestrel-lang-1.7.4/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_display.py` & `kestrel-lang-1.7.4/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_exceptions.py` & `kestrel-lang-1.7.4/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_expressions.py` & `kestrel-lang-1.7.4/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_parser.py` & `kestrel-lang-1.7.4/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_python_analytics.py` & `kestrel-lang-1.7.4/tests/test_python_analytics.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_records.py` & `kestrel-lang-1.7.4/tests/test_records.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_session.py` & `kestrel-lang-1.7.4/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_stixshifter.py` & `kestrel-lang-1.7.4/tests/test_stixshifter.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_stixshifter_diagnosis.py` & `kestrel-lang-1.7.4/tests/test_stixshifter_diagnosis.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import pytest
 import subprocess
 
 from kestrel_datasource_stixshifter.diagnosis import Diagnosis
-from .utils import stixshifter_profile_lab101
+from .utils import stixshifter_profile_lab101, stixshifter_profile_ecs
 
 
 def test_diagnosis(stixshifter_profile_lab101):
-    pattern = " ".join([
-        "[ipv4-addr:value LIKE '%']",
-        "START t'2000-01-01T00:00:00.000Z' STOP t'3000-01-01T00:00:00.000Z'",
-    ])
+    pattern = " ".join(
+        [
+            "[ipv4-addr:value != '255.255.255.255']",
+            "START t'2000-01-01T00:00:00.000Z' STOP t'3000-01-01T00:00:00.000Z'",
+        ]
+    )
     diag = Diagnosis("lab101")
     diag.diagnose_config()
     diag.diagnose_ping()
     assert pattern == diag.diagnose_translate_query(pattern)["queries"][0]
     res = diag.diagnose_run_query_and_retrieval_result([pattern], 1)
     assert len(res) == 1 and res[0] == 533
 
 
 def test_cli(stixshifter_profile_lab101):
-
     expected_output = """
 ## Diagnose: config verification
 
 #### Kestrel specific config
 retrieval batch size: 2000
 cool down after transmission: 0
 enable fast translation: False
@@ -42,48 +43,104 @@
 {
     "auth": {
         "username": null,
         "password": null
     }
 }
 
-## Diagnose: stix-shifter to data source connection (network, auth)
+## Diagnose: stix-shifter query translation
 
-#### Results from stixshifter transmission.ping()
-{
-    "success": true
-}
+#### Input: STIX pattern
+[ipv4-addr:value != '255.255.255.255'] START t'2000-01-01T00:00:00.000Z' STOP t'3000-01-01T00:00:00.000Z'
 
-## Diagnose: stix-shifter query translation
+#### Output: 1 data source native queries
+[ipv4-addr:value != '255.255.255.255'] START t'2000-01-01T00:00:00.000Z' STOP t'3000-01-01T00:00:00.000Z'
 
-#### Input pattern
-[ipv4-addr:value LIKE '%'] START t'2000-01-01T00:00:00.000Z' STOP t'3000-01-01T00:00:00.000Z'
+## Diagnose: stix-shifter to data source connection (network, auth)
 
-#### Output data source native query
+#### Results from stixshifter transmission.ping()
 {
-    "queries": [
-        "[ipv4-addr:value LIKE '%'] START t'2000-01-01T00:00:00.000Z' STOP t'3000-01-01T00:00:00.000Z'"
-    ]
+    "success": true
 }
 
 ## Diagnose: stix-shifter query execution: <=1 batch(s)
 
 #### data retrieval results:
 one batch retrieved: 533 entries
 
 ## Diagnose: stix-shifter query execution: <=5 batch(s)
 
 #### data retrieval results:
 one batch retrieved: 533 entries
 """
 
-    result = subprocess.run(args = ["stix-shifter-diag", "lab101"], 
-                            universal_newlines = True,
-                            stdout = subprocess.PIPE
-                           )
+    result = subprocess.run(
+        args=["stix-shifter-diag", "lab101"],
+        universal_newlines=True,
+        stdout=subprocess.PIPE,
+    )
+
+    result_lines = result.stdout.splitlines()
+    result_lines = [x for x in result_lines if x]
+    expected_lines = expected_output.splitlines()
+    expected_lines = [x for x in expected_lines if x]
+    for x, y in zip(result_lines, expected_lines):
+        assert x == y
+
+
+def test_cli_ecs(stixshifter_profile_ecs):
+    expected_output = """
+## Diagnose: config verification
+
+#### Kestrel specific config
+retrieval batch size: 2000
+cool down after transmission: 0
+enable fast translation: False
+
+#### Config to be passed to stix-shifter
+connector name: elastic_ecs
+connection object [ref: https://github.com/opencybersecurityalliance/stix-shifter/blob/develop/OVERVIEW.md#connection]:
+{
+    "host": "elastic.securitylog.company.com",
+    "port": 9200,
+    "selfSignedCert": false,
+    "indices": "host101",
+    "options": {
+        "result_limit": 4000,
+        "timeout": 60
+    }
+}
+configuration object [ref: https://github.com/opencybersecurityalliance/stix-shifter/blob/develop/OVERVIEW.md#configuration]:
+{
+    "auth": {
+        "id": "********",
+        "api_key": "********"
+    }
+}
+
+## Diagnose: stix-shifter query translation
+
+#### Input: STIX pattern
+[x-oca-asset:device_id = '123456'] START t'2000-01-01T00:00:00.000Z' STOP t'3000-01-01T00:00:00.000Z'
+
+#### Output: 1 data source native queries
+(host.id : "123456" OR observer.serial_number : "123456") AND (@timestamp:["2000-01-01T00:00:00.000Z" TO "3000-01-01T00:00:00.000Z"])
+"""
+
+    result = subprocess.run(
+        args=[
+            "stix-shifter-diag",
+            "-p",
+            "[x-oca-asset:device_id = '123456'] START t'2000-01-01T00:00:00.000Z' STOP t'3000-01-01T00:00:00.000Z'",
+            "-t",
+            "ecs",
+        ],
+        universal_newlines=True,
+        stdout=subprocess.PIPE,
+    )
 
     result_lines = result.stdout.splitlines()
     result_lines = [x for x in result_lines if x]
     expected_lines = expected_output.splitlines()
     expected_lines = [x for x in expected_lines if x]
-    for x,y in zip(result_lines, expected_lines):
+    for x, y in zip(result_lines, expected_lines):
         assert x == y
```

### Comparing `kestrel-lang-1.7.3/tests/test_stixshifter_translator.py` & `kestrel-lang-1.7.4/tests/test_stixshifter_translator.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.3/tests/test_timestamped.py` & `kestrel-lang-1.7.4/tests/test_timestamped.py`

 * *Files identical despite different names*

