# Comparing `tmp/jaclang-0.0.3.tar.gz` & `tmp/jaclang-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaclang-0.0.3.tar", last modified: Thu Aug  3 11:45:19 2023, max compression
+gzip compressed data, was "jaclang-2.0.0.tar", last modified: Tue Jun  6 16:46:30 2023, max compression
```

## Comparing `jaclang-0.0.3.tar` & `jaclang-2.0.0.tar`

### file list

```diff
@@ -1,92 +1,10 @@
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/
--rw-r--r--   0 ninja     (1000) ninja     (1000)      213 2023-08-03 11:45:19.700051 jaclang-0.0.3/PKG-INFO
--rw-r--r--   0 ninja     (1000) ninja     (1000)      411 2023-06-14 22:26:43.000000 jaclang-0.0.3/README.md
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/
--rw-r--r--   0 ninja     (1000) ninja     (1000)      194 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/__init__.py
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/cli/
--rw-r--r--   0 ninja     (1000) ninja     (1000)      175 2023-07-10 18:30:36.000000 jaclang-0.0.3/jaclang/cli/__init__.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     1059 2023-07-07 17:22:45.000000 jaclang-0.0.3/jaclang/cli/cli.jac
--rw-r--r--   0 ninja     (1000) ninja     (1000)      386 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/cli/cmds.jac
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/cli/impl/
--rw-r--r--   0 ninja     (1000) ninja     (1000)       39 2023-08-03 11:40:55.000000 jaclang-0.0.3/jaclang/cli/impl/__init__.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     2398 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/cli/impl/cli_impl.jac
--rw-r--r--   0 ninja     (1000) ninja     (1000)      719 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/cli/impl/cmds_impl.jac
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/core/
--rw-r--r--   0 ninja     (1000) ninja     (1000)      212 2023-07-11 19:07:20.000000 jaclang-0.0.3/jaclang/core/__init__.py
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/core/impl/
--rw-r--r--   0 ninja     (1000) ninja     (1000)       39 2023-08-03 11:40:55.000000 jaclang-0.0.3/jaclang/core/impl/__init__.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     3063 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/core/impl/arch_impl.jac
--rw-r--r--   0 ninja     (1000) ninja     (1000)     2486 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/core/impl/element_impl.jac
--rw-r--r--   0 ninja     (1000) ninja     (1000)      370 2023-07-25 14:45:56.000000 jaclang-0.0.3/jaclang/core/impl/exec_ctx_impl.jac
--rw-r--r--   0 ninja     (1000) ninja     (1000)     1364 2023-07-08 21:48:59.000000 jaclang-0.0.3/jaclang/core/impl/memory_impl.jac
--rw-r--r--   0 ninja     (1000) ninja     (1000)     2786 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/core/primitives.jac
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/jac/
--rw-r--r--   0 ninja     (1000) ninja     (1000)       26 2023-06-07 20:54:41.000000 jaclang-0.0.3/jaclang/jac/__init__.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)    47429 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/jac/absyntree.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     1107 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/jac/constant.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     4645 2023-08-01 15:12:45.000000 jaclang-0.0.3/jaclang/jac/importer.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)    13803 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/jac/lexer.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)    40357 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/jac/parser.py
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/jac/passes/
--rw-r--r--   0 ninja     (1000) ninja     (1000)       69 2023-07-09 22:53:31.000000 jaclang-0.0.3/jaclang/jac/passes/__init__.py
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/jac/passes/blue/
--rw-r--r--   0 ninja     (1000) ninja     (1000)      638 2023-07-09 22:53:31.000000 jaclang-0.0.3/jaclang/jac/passes/blue/__init__.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)    97828 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/jac/passes/blue/ast_build_pass.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)    43497 2023-08-01 14:51:01.000000 jaclang-0.0.3/jaclang/jac/passes/blue/blue_pygen_pass.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     9711 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/jac/passes/blue/decl_def_match_pass.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     2669 2023-07-09 22:53:31.000000 jaclang-0.0.3/jaclang/jac/passes/blue/import_pass.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)      964 2023-07-09 22:53:31.000000 jaclang-0.0.3/jaclang/jac/passes/blue/sub_node_tab_pass.py
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/jac/passes/blue/tests/
--rw-r--r--   0 ninja     (1000) ninja     (1000)       28 2023-07-09 22:53:31.000000 jaclang-0.0.3/jaclang/jac/passes/blue/tests/__init__.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     2339 2023-07-20 23:26:09.000000 jaclang-0.0.3/jaclang/jac/passes/blue/tests/test_ast_build_pass.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     4611 2023-07-23 13:38:13.000000 jaclang-0.0.3/jaclang/jac/passes/blue/tests/test_blue_pygen_pass.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     1676 2023-07-09 22:53:31.000000 jaclang-0.0.3/jaclang/jac/passes/blue/tests/test_decl_def_match_pass.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)      576 2023-07-09 22:53:31.000000 jaclang-0.0.3/jaclang/jac/passes/blue/tests/test_import_pass.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)      842 2023-07-09 22:53:31.000000 jaclang-0.0.3/jaclang/jac/passes/blue/tests/test_sub_node_pass.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     2123 2023-07-09 23:00:15.000000 jaclang-0.0.3/jaclang/jac/passes/blue/tests/test_type_analyze_pass.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)    18256 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/jac/passes/blue/type_analyze_pass.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     5141 2023-07-23 13:38:13.000000 jaclang-0.0.3/jaclang/jac/passes/ir_pass.py
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/jac/passes/purple/
--rw-r--r--   0 ninja     (1000) ninja     (1000)      343 2023-07-10 18:30:36.000000 jaclang-0.0.3/jaclang/jac/passes/purple/__init__.py
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/jac/passes/purple/impl/
--rw-r--r--   0 ninja     (1000) ninja     (1000)       39 2023-08-03 11:40:55.000000 jaclang-0.0.3/jaclang/jac/passes/purple/impl/__init__.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     8501 2023-08-01 14:51:04.000000 jaclang-0.0.3/jaclang/jac/passes/purple/impl/purple_pygen_pass_impl.jac
--rw-r--r--   0 ninja     (1000) ninja     (1000)     1125 2023-08-01 13:58:57.000000 jaclang-0.0.3/jaclang/jac/passes/purple/purple_pygen_pass.jac
--rw-r--r--   0 ninja     (1000) ninja     (1000)     3422 2023-07-06 12:42:49.000000 jaclang-0.0.3/jaclang/jac/sym_table.py
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/jac/tests/
--rw-r--r--   0 ninja     (1000) ninja     (1000)       27 2023-06-07 20:54:41.000000 jaclang-0.0.3/jaclang/jac/tests/__init__.py
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/jac/tests/fixtures/
--rw-r--r--   0 ninja     (1000) ninja     (1000)       35 2023-06-07 20:54:41.000000 jaclang-0.0.3/jaclang/jac/tests/fixtures/__init__.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)      263 2023-06-21 21:49:24.000000 jaclang-0.0.3/jaclang/jac/tests/fixtures/activity.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     1653 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/jac/tests/fixtures/fam.jac
--rw-r--r--   0 ninja     (1000) ninja     (1000)       78 2023-06-22 15:58:17.000000 jaclang-0.0.3/jaclang/jac/tests/fixtures/hello_world.jac
--rw-r--r--   0 ninja     (1000) ninja     (1000)     1394 2023-07-28 21:06:12.000000 jaclang-0.0.3/jaclang/jac/tests/fixtures/lexer_fam.jac
--rw-r--r--   0 ninja     (1000) ninja     (1000)       85 2023-06-07 20:54:41.000000 jaclang-0.0.3/jaclang/jac/tests/fixtures/stuff.jac
--rw-r--r--   0 ninja     (1000) ninja     (1000)      743 2023-07-10 18:30:36.000000 jaclang-0.0.3/jaclang/jac/tests/test_importer.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     1950 2023-07-06 00:30:09.000000 jaclang-0.0.3/jaclang/jac/tests/test_lexer.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     1804 2023-07-04 19:46:42.000000 jaclang-0.0.3/jaclang/jac/tests/test_parser.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)      382 2023-06-25 17:49:55.000000 jaclang-0.0.3/jaclang/jac/tests/test_utils.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     1768 2023-07-10 18:30:36.000000 jaclang-0.0.3/jaclang/jac/transform.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     2188 2023-07-18 13:27:54.000000 jaclang-0.0.3/jaclang/jac/transpiler.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     3825 2023-07-23 13:38:13.000000 jaclang-0.0.3/jaclang/jac/utils.py
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/utils/
--rw-r--r--   0 ninja     (1000) ninja     (1000)       46 2023-06-07 20:54:41.000000 jaclang-0.0.3/jaclang/utils/__init__.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     1779 2023-06-24 22:52:22.000000 jaclang-0.0.3/jaclang/utils/fstring_parser.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)      239 2023-07-05 20:21:22.000000 jaclang-0.0.3/jaclang/utils/log.py
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/utils/sly/
--rw-r--r--   0 ninja     (1000) ninja     (1000)      115 2023-06-07 20:54:41.000000 jaclang-0.0.3/jaclang/utils/sly/__init__.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     1957 2023-06-07 20:54:41.000000 jaclang-0.0.3/jaclang/utils/sly/docparse.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)    16846 2023-06-22 15:58:48.000000 jaclang-0.0.3/jaclang/utils/sly/lex.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)    88197 2023-06-26 19:57:59.000000 jaclang-0.0.3/jaclang/utils/sly/yacc.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     3229 2023-07-03 18:38:12.000000 jaclang-0.0.3/jaclang/utils/test.py
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang/utils/tests/
--rw-r--r--   0 ninja     (1000) ninja     (1000)       23 2023-06-23 19:35:18.000000 jaclang-0.0.3/jaclang/utils/tests/__init__.py
--rw-r--r--   0 ninja     (1000) ninja     (1000)     1887 2023-06-23 19:49:15.000000 jaclang-0.0.3/jaclang/utils/tests/test_fstring_parser.py
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-08-03 11:45:19.700051 jaclang-0.0.3/jaclang.egg-info/
--rw-r--r--   0 ninja     (1000) ninja     (1000)      213 2023-08-03 11:45:19.000000 jaclang-0.0.3/jaclang.egg-info/PKG-INFO
--rw-r--r--   0 ninja     (1000) ninja     (1000)     2401 2023-08-03 11:45:19.000000 jaclang-0.0.3/jaclang.egg-info/SOURCES.txt
--rw-r--r--   0 ninja     (1000) ninja     (1000)        1 2023-08-03 11:45:19.000000 jaclang-0.0.3/jaclang.egg-info/dependency_links.txt
--rw-r--r--   0 ninja     (1000) ninja     (1000)       51 2023-08-03 11:45:19.000000 jaclang-0.0.3/jaclang.egg-info/entry_points.txt
--rw-r--r--   0 ninja     (1000) ninja     (1000)        8 2023-08-03 11:45:19.000000 jaclang-0.0.3/jaclang.egg-info/top_level.txt
--rw-r--r--   0 ninja     (1000) ninja     (1000)       38 2023-08-03 11:45:19.700051 jaclang-0.0.3/setup.cfg
--rw-r--r--   0 ninja     (1000) ninja     (1000)      526 2023-08-03 11:44:36.000000 jaclang-0.0.3/setup.py
+drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-06-06 16:46:30.112150 jaclang-2.0.0/
+-rw-r--r--   0 ninja     (1000) ninja     (1000)      151 2023-06-06 16:46:30.112150 jaclang-2.0.0/PKG-INFO
+-rw-r--r--   0 ninja     (1000) ninja     (1000)      376 2023-06-06 16:27:44.000000 jaclang-2.0.0/README.md
+drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-06-06 16:46:30.112150 jaclang-2.0.0/jaclang.egg-info/
+-rw-r--r--   0 ninja     (1000) ninja     (1000)      151 2023-06-06 16:46:30.000000 jaclang-2.0.0/jaclang.egg-info/PKG-INFO
+-rw-r--r--   0 ninja     (1000) ninja     (1000)      142 2023-06-06 16:46:30.000000 jaclang-2.0.0/jaclang.egg-info/SOURCES.txt
+-rw-r--r--   0 ninja     (1000) ninja     (1000)        1 2023-06-06 16:46:30.000000 jaclang-2.0.0/jaclang.egg-info/dependency_links.txt
+-rw-r--r--   0 ninja     (1000) ninja     (1000)        1 2023-06-06 16:46:30.000000 jaclang-2.0.0/jaclang.egg-info/top_level.txt
+-rw-r--r--   0 ninja     (1000) ninja     (1000)       38 2023-06-06 16:46:30.112150 jaclang-2.0.0/setup.cfg
+-rw-r--r--   0 ninja     (1000) ninja     (1000)      410 2023-06-06 16:28:24.000000 jaclang-2.0.0/setup.py
```

