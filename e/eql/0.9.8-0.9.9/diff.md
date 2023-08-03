# Comparing `tmp/eql-0.9.8.tar.gz` & `tmp/eql-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eql-0.9.8.tar", last modified: Thu Jan 14 15:48:01 2021, max compression
+gzip compressed data, was "dist/eql-0.9.9.tar", last modified: Mon Feb 22 18:38:39 2021, max compression
```

## Comparing `eql-0.9.8.tar` & `eql-0.9.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 rwolf      (503) staff       (20)        0 2021-01-14 15:48:01.000000 eql-0.9.8/
--rw-r--r--   0 rwolf      (503) staff       (20)    32971 2019-07-25 23:23:40.000000 eql-0.9.8/LICENSE
--rw-r--r--   0 rwolf      (503) staff       (20)       33 2020-05-18 20:17:38.000000 eql-0.9.8/MANIFEST.in
--rw-r--r--   0 rwolf      (503) staff       (20)     1093 2021-01-14 15:48:01.000000 eql-0.9.8/PKG-INFO
--rw-r--r--   0 rwolf      (503) staff       (20)     2079 2020-05-28 21:26:43.000000 eql-0.9.8/README.md
-drwxr-xr-x   0 rwolf      (503) staff       (20)        0 2021-01-14 15:48:01.000000 eql-0.9.8/eql/
--rw-r--r--   0 rwolf      (503) staff       (20)     2455 2021-01-14 15:47:47.000000 eql-0.9.8/eql/__init__.py
--rw-r--r--   0 rwolf      (503) staff       (20)       81 2019-05-01 20:39:47.000000 eql-0.9.8/eql/__main__.py
--rw-r--r--   0 rwolf      (503) staff       (20)    41225 2021-01-14 15:47:47.000000 eql-0.9.8/eql/ast.py
--rw-r--r--   0 rwolf      (503) staff       (20)     5207 2020-01-14 01:06:28.000000 eql-0.9.8/eql/build.py
--rw-r--r--   0 rwolf      (503) staff       (20)    47729 2020-07-06 17:02:25.000000 eql-0.9.8/eql/engine.py
--rw-r--r--   0 rwolf      (503) staff       (20)     1372 2019-09-10 17:59:03.000000 eql-0.9.8/eql/errors.py
-drwxr-xr-x   0 rwolf      (503) staff       (20)        0 2021-01-14 15:48:01.000000 eql-0.9.8/eql/etc/
--rw-r--r--   0 rwolf      (503) staff       (20)      481 2019-05-01 20:39:47.000000 eql-0.9.8/eql/etc/__init__.py
--rw-r--r--   0 rwolf      (503) staff       (20)      896 2020-04-28 18:52:39.000000 eql-0.9.8/eql/etc/__init__.pyc
--rw-r--r--   0 rwolf      (503) staff       (20)     3825 2020-11-24 19:28:50.000000 eql-0.9.8/eql/etc/eql.g
--rw-r--r--   0 rwolf      (503) staff       (20)    65744 2019-11-01 21:12:24.000000 eql-0.9.8/eql/etc/test_data.json
--rw-r--r--   0 rwolf      (503) staff       (20)    13156 2020-07-06 18:54:00.000000 eql-0.9.8/eql/etc/test_folding.toml
--rw-r--r--   0 rwolf      (503) staff       (20)     3005 2020-07-06 18:54:02.000000 eql-0.9.8/eql/etc/test_optimizer.toml
--rw-r--r--   0 rwolf      (503) staff       (20)    43281 2020-07-06 18:54:00.000000 eql-0.9.8/eql/etc/test_queries.toml
--rw-r--r--   0 rwolf      (503) staff       (20)    12888 2020-07-06 18:54:00.000000 eql-0.9.8/eql/etc/test_string_functions.toml
--rw-r--r--   0 rwolf      (503) staff       (20)     1443 2019-07-26 19:15:33.000000 eql-0.9.8/eql/events.py
--rw-r--r--   0 rwolf      (503) staff       (20)    21568 2020-06-08 17:25:26.000000 eql-0.9.8/eql/functions.py
--rw-r--r--   0 rwolf      (503) staff       (20)     2669 2019-11-01 21:12:24.000000 eql-0.9.8/eql/highlighters.py
--rw-r--r--   0 rwolf      (503) staff       (20)      859 2019-07-26 19:15:33.000000 eql-0.9.8/eql/loader.py
--rw-r--r--   0 rwolf      (503) staff       (20)     4960 2020-10-13 19:50:38.000000 eql-0.9.8/eql/main.py
--rw-r--r--   0 rwolf      (503) staff       (20)     5722 2020-06-08 17:25:26.000000 eql-0.9.8/eql/optimizer.py
--rw-r--r--   0 rwolf      (503) staff       (20)    59426 2020-11-24 19:28:50.000000 eql-0.9.8/eql/parser.py
--rw-r--r--   0 rwolf      (503) staff       (20)     4665 2020-05-29 18:02:19.000000 eql-0.9.8/eql/pipes.py
--rw-r--r--   0 rwolf      (503) staff       (20)    11436 2020-05-18 20:17:38.000000 eql-0.9.8/eql/schema.py
--rw-r--r--   0 rwolf      (503) staff       (20)    27739 2020-05-18 20:17:38.000000 eql-0.9.8/eql/shell.py
--rw-r--r--   0 rwolf      (503) staff       (20)      861 2020-05-18 20:17:38.000000 eql-0.9.8/eql/signatures.py
--rw-r--r--   0 rwolf      (503) staff       (20)    10332 2019-08-02 18:32:03.000000 eql-0.9.8/eql/table.py
-drwxr-xr-x   0 rwolf      (503) staff       (20)        0 2021-01-14 15:48:01.000000 eql-0.9.8/eql/tests/
--rw-r--r--   0 rwolf      (503) staff       (20)      157 2019-07-26 19:15:33.000000 eql-0.9.8/eql/tests/__init__.py
--rw-r--r--   0 rwolf      (503) staff       (20)     3530 2020-07-06 18:58:51.000000 eql-0.9.8/eql/tests/base.py
--rw-r--r--   0 rwolf      (503) staff       (20)     6292 2020-03-11 20:44:33.000000 eql-0.9.8/eql/transpilers.py
--rw-r--r--   0 rwolf      (503) staff       (20)     4493 2020-05-18 20:17:38.000000 eql-0.9.8/eql/types.py
--rw-r--r--   0 rwolf      (503) staff       (20)    12712 2020-06-08 17:25:26.000000 eql-0.9.8/eql/utils.py
--rw-r--r--   0 rwolf      (503) staff       (20)     9061 2020-05-18 20:17:38.000000 eql-0.9.8/eql/walkers.py
-drwxr-xr-x   0 rwolf      (503) staff       (20)        0 2021-01-14 15:48:01.000000 eql-0.9.8/eql.egg-info/
--rw-r--r--   0 rwolf      (503) staff       (20)     1093 2021-01-14 15:48:01.000000 eql-0.9.8/eql.egg-info/PKG-INFO
--rw-r--r--   0 rwolf      (503) staff       (20)      794 2021-01-14 15:48:01.000000 eql-0.9.8/eql.egg-info/SOURCES.txt
--rw-r--r--   0 rwolf      (503) staff       (20)        1 2021-01-14 15:48:01.000000 eql-0.9.8/eql.egg-info/dependency_links.txt
--rw-r--r--   0 rwolf      (503) staff       (20)       90 2021-01-14 15:48:01.000000 eql-0.9.8/eql.egg-info/entry_points.txt
--rw-r--r--   0 rwolf      (503) staff       (20)        1 2020-10-13 20:17:13.000000 eql-0.9.8/eql.egg-info/not-zip-safe
--rw-r--r--   0 rwolf      (503) staff       (20)      631 2021-01-14 15:48:01.000000 eql-0.9.8/eql.egg-info/requires.txt
--rw-r--r--   0 rwolf      (503) staff       (20)        4 2021-01-14 15:48:01.000000 eql-0.9.8/eql.egg-info/top_level.txt
--rw-r--r--   0 rwolf      (503) staff       (20)      257 2021-01-14 15:48:01.000000 eql-0.9.8/setup.cfg
--rw-r--r--   0 rwolf      (503) staff       (20)     3802 2020-11-24 19:28:50.000000 eql-0.9.8/setup.py
+drwxr-xr-x   0 rwolf      (503) staff       (20)        0 2021-02-22 18:38:39.000000 eql-0.9.9/
+-rw-r--r--   0 rwolf      (503) staff       (20)    32971 2019-07-25 23:23:40.000000 eql-0.9.9/LICENSE
+-rw-r--r--   0 rwolf      (503) staff       (20)       33 2020-05-18 20:17:38.000000 eql-0.9.9/MANIFEST.in
+-rw-r--r--   0 rwolf      (503) staff       (20)     1093 2021-02-22 18:38:39.000000 eql-0.9.9/PKG-INFO
+-rw-r--r--   0 rwolf      (503) staff       (20)     2479 2021-02-10 17:00:29.000000 eql-0.9.9/README.md
+drwxr-xr-x   0 rwolf      (503) staff       (20)        0 2021-02-22 18:38:39.000000 eql-0.9.9/eql/
+-rw-r--r--   0 rwolf      (503) staff       (20)     2455 2021-02-22 18:38:30.000000 eql-0.9.9/eql/__init__.py
+-rw-r--r--   0 rwolf      (503) staff       (20)       81 2019-05-01 20:39:47.000000 eql-0.9.9/eql/__main__.py
+-rw-r--r--   0 rwolf      (503) staff       (20)    41225 2021-01-14 15:47:47.000000 eql-0.9.9/eql/ast.py
+-rw-r--r--   0 rwolf      (503) staff       (20)     5207 2020-01-14 01:06:28.000000 eql-0.9.9/eql/build.py
+-rw-r--r--   0 rwolf      (503) staff       (20)    47729 2020-07-06 17:02:25.000000 eql-0.9.9/eql/engine.py
+-rw-r--r--   0 rwolf      (503) staff       (20)     1372 2019-09-10 17:59:03.000000 eql-0.9.9/eql/errors.py
+drwxr-xr-x   0 rwolf      (503) staff       (20)        0 2021-02-22 18:38:39.000000 eql-0.9.9/eql/etc/
+-rw-r--r--   0 rwolf      (503) staff       (20)      481 2019-05-01 20:39:47.000000 eql-0.9.9/eql/etc/__init__.py
+-rw-r--r--   0 rwolf      (503) staff       (20)      896 2020-04-28 18:52:39.000000 eql-0.9.9/eql/etc/__init__.pyc
+-rw-r--r--   0 rwolf      (503) staff       (20)     4070 2021-02-22 18:38:30.000000 eql-0.9.9/eql/etc/eql.g
+-rw-r--r--   0 rwolf      (503) staff       (20)    65744 2019-11-01 21:12:24.000000 eql-0.9.9/eql/etc/test_data.json
+-rw-r--r--   0 rwolf      (503) staff       (20)    13156 2020-07-06 18:54:00.000000 eql-0.9.9/eql/etc/test_folding.toml
+-rw-r--r--   0 rwolf      (503) staff       (20)     3005 2020-07-06 18:54:02.000000 eql-0.9.9/eql/etc/test_optimizer.toml
+-rw-r--r--   0 rwolf      (503) staff       (20)    43281 2020-07-06 18:54:00.000000 eql-0.9.9/eql/etc/test_queries.toml
+-rw-r--r--   0 rwolf      (503) staff       (20)    12888 2020-07-06 18:54:00.000000 eql-0.9.9/eql/etc/test_string_functions.toml
+-rw-r--r--   0 rwolf      (503) staff       (20)     1443 2019-07-26 19:15:33.000000 eql-0.9.9/eql/events.py
+-rw-r--r--   0 rwolf      (503) staff       (20)    21568 2020-06-08 17:25:26.000000 eql-0.9.9/eql/functions.py
+-rw-r--r--   0 rwolf      (503) staff       (20)     2669 2019-11-01 21:12:24.000000 eql-0.9.9/eql/highlighters.py
+-rw-r--r--   0 rwolf      (503) staff       (20)      859 2019-07-26 19:15:33.000000 eql-0.9.9/eql/loader.py
+-rw-r--r--   0 rwolf      (503) staff       (20)     4960 2020-10-13 19:50:38.000000 eql-0.9.9/eql/main.py
+-rw-r--r--   0 rwolf      (503) staff       (20)     5722 2020-06-08 17:25:26.000000 eql-0.9.9/eql/optimizer.py
+-rw-r--r--   0 rwolf      (503) staff       (20)    60906 2021-02-22 18:38:30.000000 eql-0.9.9/eql/parser.py
+-rw-r--r--   0 rwolf      (503) staff       (20)     4665 2020-05-29 18:02:19.000000 eql-0.9.9/eql/pipes.py
+-rw-r--r--   0 rwolf      (503) staff       (20)    11436 2020-05-18 20:17:38.000000 eql-0.9.9/eql/schema.py
+-rw-r--r--   0 rwolf      (503) staff       (20)    27739 2020-05-18 20:17:38.000000 eql-0.9.9/eql/shell.py
+-rw-r--r--   0 rwolf      (503) staff       (20)      861 2020-05-18 20:17:38.000000 eql-0.9.9/eql/signatures.py
+-rw-r--r--   0 rwolf      (503) staff       (20)    10332 2019-08-02 18:32:03.000000 eql-0.9.9/eql/table.py
+drwxr-xr-x   0 rwolf      (503) staff       (20)        0 2021-02-22 18:38:39.000000 eql-0.9.9/eql/tests/
+-rw-r--r--   0 rwolf      (503) staff       (20)      157 2019-07-26 19:15:33.000000 eql-0.9.9/eql/tests/__init__.py
+-rw-r--r--   0 rwolf      (503) staff       (20)     3530 2020-07-06 18:58:51.000000 eql-0.9.9/eql/tests/base.py
+-rw-r--r--   0 rwolf      (503) staff       (20)     6292 2020-03-11 20:44:33.000000 eql-0.9.9/eql/transpilers.py
+-rw-r--r--   0 rwolf      (503) staff       (20)     4493 2020-05-18 20:17:38.000000 eql-0.9.9/eql/types.py
+-rw-r--r--   0 rwolf      (503) staff       (20)    12712 2020-06-08 17:25:26.000000 eql-0.9.9/eql/utils.py
+-rw-r--r--   0 rwolf      (503) staff       (20)     9061 2020-05-18 20:17:38.000000 eql-0.9.9/eql/walkers.py
+drwxr-xr-x   0 rwolf      (503) staff       (20)        0 2021-02-22 18:38:39.000000 eql-0.9.9/eql.egg-info/
+-rw-r--r--   0 rwolf      (503) staff       (20)     1093 2021-02-22 18:38:39.000000 eql-0.9.9/eql.egg-info/PKG-INFO
+-rw-r--r--   0 rwolf      (503) staff       (20)      794 2021-02-22 18:38:39.000000 eql-0.9.9/eql.egg-info/SOURCES.txt
+-rw-r--r--   0 rwolf      (503) staff       (20)        1 2021-02-22 18:38:39.000000 eql-0.9.9/eql.egg-info/dependency_links.txt
+-rw-r--r--   0 rwolf      (503) staff       (20)       90 2021-02-22 18:38:39.000000 eql-0.9.9/eql.egg-info/entry_points.txt
+-rw-r--r--   0 rwolf      (503) staff       (20)        1 2021-02-22 18:38:39.000000 eql-0.9.9/eql.egg-info/not-zip-safe
+-rw-r--r--   0 rwolf      (503) staff       (20)      631 2021-02-22 18:38:39.000000 eql-0.9.9/eql.egg-info/requires.txt
+-rw-r--r--   0 rwolf      (503) staff       (20)        4 2021-02-22 18:38:39.000000 eql-0.9.9/eql.egg-info/top_level.txt
+-rw-r--r--   0 rwolf      (503) staff       (20)      257 2021-02-22 18:38:39.000000 eql-0.9.9/setup.cfg
+-rw-r--r--   0 rwolf      (503) staff       (20)     3802 2021-02-22 18:38:30.000000 eql-0.9.9/setup.py
```

### Comparing `eql-0.9.8/LICENSE` & `eql-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/PKG-INFO` & `eql-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eql
-Version: 0.9.8
+Version: 0.9.9
 Summary: Event Query Language
 Home-page: https://eql.readthedocs.io
 Author: Endgame, Inc.
 Author-email: eql@endgame.com
 License: AGPLv3
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `eql-0.9.8/README.md` & `eql-0.9.9/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # Event Query Language
 [![PyPI](https://img.shields.io/pypi/v/eql.svg)](https://pypi.python.org/pypi/eql)
-[![Gitter](https://badges.gitter.im/eventquerylang/community.svg)](https://gitter.im/eventquerylang/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 [![Documentation](https://readthedocs.org/projects/eql/badge/?version=latest)](https://eql.readthedocs.io/en/latest/?badge=latest)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/eventquerylang.svg?style=social)](https://twitter.com/eventquerylang)
 
 ![What is EQL?](docs/_static/eql-whoami.jpg)
 Browse a [library of EQL analytics](https://eqllib.readthedocs.io)
 
+## Now in Elasticsearch!
+
+Since Endgame [joined forced with Elastic](https://www.elastic.co/blog/endgame-joins-forces-with-elastic), EQL is now natively integrated in Elasticsearch! See the Elasticsearch [EQL documentation](https://www.elastic.co/guide/en/elasticsearch/reference/current/eql.html) for more information. Also, please note that we have made a few changes to EQL in Elasticsearch to accomodate non-security users. Those are best summarized [here](https://www.elastic.co/guide/en/elasticsearch/reference/current/eql-syntax.html#eql-unsupported-syntax).
+
 # Getting Started
 
 The EQL module current supports Python 2.7 and 3.5+. Assuming a supported Python version is installed, run the command:
 
 ```console
 $ pip install eql
 ```
```

### Comparing `eql-0.9.8/eql/__init__.py` & `eql-0.9.9/eql/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 from .walkers import (
     ConfigurableWalker,
     DepthFirstWalker,
     RecursiveWalker,
     Walker,
 )
 
-__version__ = '0.9.8'
+__version__ = '0.9.9'
 __all__ = (
     "__version__",
     "AnalyticOutput",
     "BaseEngine",
     "BaseTranspiler",
     "ConfigurableWalker",
     "DepthFirstWalker",
```

### Comparing `eql-0.9.8/eql/ast.py` & `eql-0.9.9/eql/ast.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/build.py` & `eql-0.9.9/eql/build.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/engine.py` & `eql-0.9.9/eql/engine.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/errors.py` & `eql-0.9.9/eql/errors.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/etc/__init__.pyc` & `eql-0.9.9/eql/etc/__init__.pyc`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/etc/eql.g` & `eql-0.9.9/eql/etc/eql.g`

 * *Files 5% similar despite different names*

```diff
@@ -29,23 +29,28 @@
 // Expressions
 expressions: expr ("," expr)* [","]
 ?expr: or_expr
 ?or_expr: and_expr ("or" and_expr)*
 ?and_expr: not_expr ("and" not_expr)*
 ?not_expr.3: NOT_OP* term
 ?term: sum_expr comp_op sum_expr -> comparison
-     | sum_expr "not" "in" "(" expressions [","]? ")"  -> not_in_set
-     | sum_expr "in" "(" expressions [","]? ")" -> in_set
-     | sum_expr ILIKE (literal | "(" literal ("," literal)* ")") -> ilike
+     | sum_expr "not" IN "(" expressions [","]? ")"  -> not_in_set
+     | sum_expr IN "(" expressions [","]? ")" -> in_set
+     | sum_expr STRING_PREDICATE (literal | "(" literal ("," literal)* ")") -> string_predicate
      | sum_expr
 
 
 // Need to recover these tokens
+IN.3: "in~" | "in"
 EQUALS: "==" | "="
-ILIKE: ":"
+STRING_PREDICATE.3:  ":"
+                  |  "like~"
+                  |  "regex~"
+                  |  "like"
+                  |  "regex"
 COMP_OP: "<=" | "<" | "!=" | ">=" | ">"
 ?comp_op: EQUALS | COMP_OP
 MULT_OP:    "*" | "/" | "%"
 NOT_OP:     "not"
 
 ?sum_expr: mul_expr (SIGN mul_expr)*
 ?mul_expr: named_subquery_test (MULT_OP named_subquery_test)*
@@ -58,15 +63,15 @@
 
 // hacky approach to work around this ambiguity introduced with the colon operator
 // x : length
 // x : length( ) not allowed, now requires `:length(` form
 METHOD_START.3: ":" NAME "("
 method_name: METHOD_START
 method: method_name [expressions] ")"
-function_call: name "(" [expressions] ")"
+function_call: (INSENSITIVE_NAME | NAME) "(" [expressions] ")"
 ?atom: single_atom
      |  "(" expr ")"
 ?signed_single_atom: SIGN? single_atom
 ?single_atom: literal
             | field
             | base_field
 base_field: name | escaped_name
@@ -110,14 +115,15 @@
 UCASE_LETTER: "A".."Z"
 DIGIT: "0".."9"
 
 LETTER: UCASE_LETTER | LCASE_LETTER
 WORD: LETTER+
 
 ESCAPED_NAME: "`" /[^`\r\n]+/ "`"
+INSENSITIVE_NAME.2: ("_"|LETTER) ("_"|LETTER|DIGIT)* "~"
 NAME: ("_"|LETTER) ("_"|LETTER|DIGIT)*
 UNSIGNED_INTEGER: /[0-9]+/
 EXPONENT: /[Ee][-+]?\d+/
 DECIMAL: UNSIGNED_INTEGER? "." UNSIGNED_INTEGER+ EXPONENT?
        | UNSIGNED_INTEGER EXPONENT
 SIGN:           "+" | "-"
 DQ_STRING:        /"(\\[btnfr"'\\]|[^\r\n"\\])*"/
```

### Comparing `eql-0.9.8/eql/etc/test_data.json` & `eql-0.9.9/eql/etc/test_data.json`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/etc/test_folding.toml` & `eql-0.9.9/eql/etc/test_folding.toml`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/etc/test_optimizer.toml` & `eql-0.9.9/eql/etc/test_optimizer.toml`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/etc/test_queries.toml` & `eql-0.9.9/eql/etc/test_queries.toml`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/etc/test_string_functions.toml` & `eql-0.9.9/eql/etc/test_string_functions.toml`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/events.py` & `eql-0.9.9/eql/events.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/functions.py` & `eql-0.9.9/eql/functions.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/highlighters.py` & `eql-0.9.9/eql/highlighters.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/loader.py` & `eql-0.9.9/eql/loader.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/main.py` & `eql-0.9.9/eql/main.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/optimizer.py` & `eql-0.9.9/eql/optimizer.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/parser.py` & `eql-0.9.9/eql/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -481,16 +481,20 @@
         if text in keywords:
             raise self._error(node, "Invalid use of keyword", cls=EqlSyntaxError)
 
         return text
 
     def name(self, node):
         """Check for illegal use of keyword."""
-        text = node["NAME"].value
-        if text in keywords:
+        if isinstance(node, KvTree):
+            text = node.children[0].value
+        else:
+            text = str(node)
+
+        if text.rstrip("~") in keywords:
             raise self._error(node, "Invalid use of keyword", cls=EqlSyntaxError)
 
         return text
 
     def number(self, node):
         """Parse a number with a sign."""
         token = node.children[-1]
@@ -579,26 +583,38 @@
         #         raise self._error(node, "Reuse of variable {base}")
 
         #     # This can be overridden by the parent function that is parsing it
         #     return self._add_variable(node.base)
         field = ast.Field(base, path)
         return self._update_field_info(NodeInfo(field, source=node))
 
-    def ilike(self, node):
+    def string_predicate(self, node):
         """Callback function to walk the AST."""
+        predicate = node["STRING_PREDICATE"]
+        if predicate == ":":
+            function_name = "wildcard"
+        elif predicate in ("like", "like~"):
+            function_name = "wildcard"
+        elif predicate in ("regex", "regex~"):
+            function_name = "match"
+        else:
+            raise self._error(node, message="Invalid syntax", cls=EqlSyntaxError)
+
         if not self._elasticsearch_syntax:
-            raise self._error(node, message="Invalid syntax, try == or wildcard()", cls=EqlSyntaxError)
+            args = ", ".join(self.text[n.meta.start_pos:n.meta.end_pos] for n in node.child_trees)
+            raise self._error(node, "Invalid syntax. Try: {function_name}({args})", cls=EqlSyntaxError,
+                              function_name=function_name, args=args)
 
         children = self.visit(node.child_trees)
 
         for child in children:  # type: NodeInfo
             if not child.validate_type(TypeHint.String):
                 raise self._type_error(child, TypeHint.String)
 
-        return NodeInfo(ast.FunctionCall("wildcard", [child.node for child in children], TypeHint.Boolean))
+        return NodeInfo(ast.FunctionCall(function_name, [child.node for child in children]), TypeHint.Boolean)
 
     def comparison(self, node):
         """Callback function to walk the AST."""
         left, comp_op, right = self.visit_children(node)  # type: (NodeInfo, str, NodeInfo)
 
         op = comp_op.value
 
@@ -637,29 +653,30 @@
                     left.validate_type(TypeHint.String) and right.validate_type(TypeHint.String)):
 
                 raise self._type_error(right, left, error_message, error_node=node)
 
         eql_node = ast.Comparison(left.node, op, right.node)
 
         # there is no special comparison operator for wildcards, just look for * in the string
-        if not self._elasticsearch_syntax and isinstance(right.node, ast.String) and '*' in right.node.value:
-            func_call = ast.FunctionCall('wildcard', [left.node, right.node])
+        if not self._elasticsearch_syntax:
+            if isinstance(right.node, ast.String) and '*' in right.node.value:
+                func_call = ast.FunctionCall('wildcard', [left.node, right.node])
 
-            if op == ast.Comparison.EQ:
-                eql_node = func_call
-            elif op == ast.Comparison.NE:
-                eql_node = ~func_call
-
-        elif not self._elasticsearch_syntax and isinstance(left.node, ast.String) and '*' in left.node.value:
-            func_call = ast.FunctionCall('wildcard', [right.node, left.node])
-
-            if op == ast.Comparison.EQ:
-                eql_node = func_call
-            elif op == ast.Comparison.NE:
-                eql_node = ~func_call
+                if op == ast.Comparison.EQ:
+                    eql_node = func_call
+                elif op == ast.Comparison.NE:
+                    eql_node = ~func_call
+
+            elif isinstance(left.node, ast.String) and '*' in left.node.value:
+                func_call = ast.FunctionCall('wildcard', [right.node, left.node])
+
+                if op == ast.Comparison.EQ:
+                    eql_node = func_call
+                elif op == ast.Comparison.NE:
+                    eql_node = ~func_call
 
         return NodeInfo(eql_node, TypeHint.Boolean, nullable=left.nullable or right.nullable, source=node)
 
     def mathop(self, node):
         """Callback function to walk the AST."""
         result = self.visit(node.children[0])
         message = "Unable to {func} {actual_type}"
@@ -723,15 +740,19 @@
         """Method for converting `x not in (...)`."""
         info = self.in_set(node)
         info.node = ~info.node
         return info
 
     def in_set(self, node):
         """Callback function to walk the AST."""
-        outer, container = self.visit_children(node)  # type: (NodeInfo, list[NodeInfo])
+        if not self._elasticsearch_syntax and node.get("IN") == "in~":
+            raise self._error(node, message="Invalid syntax. Explicit case-insensitivity is not supported.",
+                              cls=EqlSyntaxError)
+
+        outer, container = self.visit(node.child_trees)  # type: (NodeInfo, list[NodeInfo])
 
         if not outer.validate_type(TypeHint.primitives()):
             # can't compare non-primitives to sets
             raise self._type_error(outer, TypeHint.primitives())
 
         # Check that everything inside the container has the same type as outside
         error_message = "Unable to compare {expected_type} to {actual_type}"
@@ -766,18 +787,32 @@
             if signature:
                 type_hint = signature.return_value
 
         return type_hint
 
     def function_call(self, node, prev_node=None, prev_arg=None):
         """Callback function to walk the AST."""
-        function_name = self.visit(node["name"] or node["method_name"])
+        if node.data == "method":
+            name_node = node["method_name"]
+            function_name = self.method_name(name_node)
+        else:
+            name_node = node.children[0]
+            function_name = self.name(name_node)
+
         args = []
         nodes = []
 
+        if function_name.endswith("~"):
+            # remove the trailing ~ and use the existing AST
+            function_name = function_name.rstrip("~")
+
+            if not self._elasticsearch_syntax:
+                raise self._error(node, "Invalid syntax. Explicit case-insensitivity is not supported",
+                                  cls=EqlSyntaxError)
+
         non_method_arguments = node["expressions"].children if node["expressions"] else []
 
         if prev_node:
             nodes.append(prev_node)
 
         if prev_arg:
             args.append(prev_arg)
@@ -836,15 +871,15 @@
             self._var_types = old_variables
 
             expr = ast.FunctionCall(function_name, [a.node for a in args], as_method=prev_node is not None)
             nullable = any(a.nullable for a in args) or signature.sometimes_null
             return NodeInfo(expr, signature.return_value, nullable=nullable, source=node)
 
         elif self._check_functions:
-            raise self._error(node["name"], "Unknown function {NAME}")
+            raise self._error(name_node, "Unknown function {function_name}", function_name=function_name)
         else:
             args = []
 
             if node["expressions"]:
                 args = self.visit(node["expressions"])
 
             func_node = ast.FunctionCall(function_name, [a.node for a in args], as_method=prev_node is not None)
```

### Comparing `eql-0.9.8/eql/pipes.py` & `eql-0.9.9/eql/pipes.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/schema.py` & `eql-0.9.9/eql/schema.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/shell.py` & `eql-0.9.9/eql/shell.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/signatures.py` & `eql-0.9.9/eql/signatures.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/table.py` & `eql-0.9.9/eql/table.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/tests/base.py` & `eql-0.9.9/eql/tests/base.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/transpilers.py` & `eql-0.9.9/eql/transpilers.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/types.py` & `eql-0.9.9/eql/types.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/utils.py` & `eql-0.9.9/eql/utils.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql/walkers.py` & `eql-0.9.9/eql/walkers.py`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql.egg-info/PKG-INFO` & `eql-0.9.9/eql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eql
-Version: 0.9.8
+Version: 0.9.9
 Summary: Event Query Language
 Home-page: https://eql.readthedocs.io
 Author: Endgame, Inc.
 Author-email: eql@endgame.com
 License: AGPLv3
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `eql-0.9.8/eql.egg-info/SOURCES.txt` & `eql-0.9.9/eql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eql-0.9.8/eql.egg-info/requires.txt` & `eql-0.9.9/eql.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-lark-parser~=0.10.1
+lark-parser~=0.11.1
 
 [:python_version < "3.4"]
 enum34
 
 [cli]
 pygments
 prompt_toolkit
```

### Comparing `eql-0.9.8/setup.py` & `eql-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools.command.test import test as TestCommand
 
 
 with io.open('eql/__init__.py', 'rt', encoding='utf8') as f:
     __version__ = re.search(r'__version__ = \'(.*?)\'', f.read()).group(1)
 
 install_requires = [
-    "lark-parser~=0.10.1",
+    "lark-parser~=0.11.1",
     "enum34; python_version<'3.4'",
 ]
 
 test_requires = [
     "mock~=1.3.0",
     "pytest~=3.8.2",
     "pytest-cov==2.4",
```

