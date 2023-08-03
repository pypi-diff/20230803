# Comparing `tmp/coconut-develop-3.0.3.post0.dev4.tar.gz` & `tmp/coconut-develop-3.0.3.post0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coconut-develop-3.0.3.post0.dev4.tar", last modified: Wed Aug  2 00:09:55 2023, max compression
+gzip compressed data, was "dist/coconut-develop-3.0.3.post0.dev5.tar", last modified: Thu Aug  3 10:08:05 2023, max compression
```

## Comparing `coconut-develop-3.0.3.post0.dev4.tar` & `coconut-develop-3.0.3.post0.dev5.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.068654 coconut-develop-3.0.3.post0.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)   202781 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/DOCS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/FAQ.md
--rw-r--r--   0 runner    (1001) docker     (123)    65131 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/HELP.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-08-02 00:09:55.068654 coconut-develop-3.0.3.post0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.056654 coconut-develop-3.0.3.post0.dev4/__coconut__/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/__coconut__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60331 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/__coconut__/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/__coconut__/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.056654 coconut-develop-3.0.3.post0.dev4/_coconut/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/_coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/_coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/_coconut/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.060654 coconut-develop-3.0.3.post0.dev4/coconut/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/__coconut__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/__coconut__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/_pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/api.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.060654 coconut-develop-3.0.3.post0.dev4/coconut/command/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/command/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    46967 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/command/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/command/command.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/command/mypy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.060654 coconut-develop-3.0.3.post0.dev4/coconut/command/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/command/resources/zcoconut.pth
--rw-r--r--   0 runner    (1001) docker     (123)    24763 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/command/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/command/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.064654 coconut-develop-3.0.3.post0.dev4/coconut/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   206759 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    93531 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/compiler/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)    36566 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/compiler/header.py
--rw-r--r--   0 runner    (1001) docker     (123)    58872 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/compiler/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.064654 coconut-develop-3.0.3.post0.dev4/coconut/compiler/templates/
--rw-r--r--   0 runner    (1001) docker     (123)   102541 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/compiler/templates/header.py_template
--rw-r--r--   0 runner    (1001) docker     (123)    56501 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/compiler/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    38170 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/convenience.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/highlighter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.064654 coconut-develop-3.0.3.post0.dev4/coconut/icoconut/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/icoconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/icoconut/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.064654 coconut-develop-3.0.3.post0.dev4/coconut/icoconut/coconut/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-02 00:09:54.000000 coconut-develop-3.0.3.post0.dev4/coconut/icoconut/coconut/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.064654 coconut-develop-3.0.3.post0.dev4/coconut/icoconut/coconut_py/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/icoconut/coconut_py/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.064654 coconut-develop-3.0.3.post0.dev4/coconut/icoconut/coconut_py2/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/icoconut/coconut_py2/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.064654 coconut-develop-3.0.3.post0.dev4/coconut/icoconut/coconut_py3/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/icoconut/coconut_py3/kernel.json
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/icoconut/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/icoconut/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/root.py
--rw-r--r--   0 runner    (1001) docker     (123)    21746 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.064654 coconut-develop-3.0.3.post0.dev4/coconut/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/constants_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    32751 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.064654 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.056654 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.064654 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/agnostic/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/agnostic/__init__.coco
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/agnostic/main.coco
--rw-r--r--   0 runner    (1001) docker     (123)    64209 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/agnostic/primary.coco
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/agnostic/specific.coco
--rw-r--r--   0 runner    (1001) docker     (123)    42170 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/agnostic/suite.coco
--rw-r--r--   0 runner    (1001) docker     (123)    15411 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/agnostic/tutorial.coco
--rw-r--r--   0 runner    (1001) docker     (123)    46342 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/agnostic/util.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.064654 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/non_strict/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.068654 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_2/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_2/py2_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.068654 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_3/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_3/py3_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.068654 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_35/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_35/py35_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.068654 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_36/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_36/py36_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.068654 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_38/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_38/py38_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.068654 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_sys/
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/extras.coco
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/importable.coco
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/runnable.coco
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/tests/src/runner.coco
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/coconut/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.068654 coconut-develop-3.0.3.post0.dev4/coconut_develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-02 00:09:55.000000 coconut-develop-3.0.3.post0.dev4/coconut_develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-02 00:09:55.068654 coconut-develop-3.0.3.post0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:09:55.068654 coconut-develop-3.0.3.post0.dev4/xontrib/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-01 21:53:33.000000 coconut-develop-3.0.3.post0.dev4/xontrib/coconut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)   202781 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/DOCS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-03 10:08:03.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut/kernel.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut_py3/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut_py3/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut_py/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut_py2/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/icoconut/coconut_py2/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/__coconut__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/__coconut__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21746 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47581 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/resources/zcoconut.pth
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24763 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/command.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/command/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)    93531 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   206822 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57558 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58872 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   102541 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/templates/header.py_template
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36566 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/compiler/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/convenience.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/api.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    32695 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/constants_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    24083 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/extras.coco
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/importable.coco
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/runnable.coco
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/runner.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/main.coco
+-rw-r--r--   0 runner    (1001) docker     (123)    42170 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/suite.coco
+-rw-r--r--   0 runner    (1001) docker     (123)    46342 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/util.coco
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/__init__.coco
+-rw-r--r--   0 runner    (1001) docker     (123)    15411 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/tutorial.coco
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/specific.coco
+-rw-r--r--   0 runner    (1001) docker     (123)    64209 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/primary.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_3/py3_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_sys/
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/non_strict/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_38/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_38/py38_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_35/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_35/py35_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_2/py2_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_36/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_36/py36_test.coco
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/_pyparsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38295 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/coconut/convenience.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut_develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/coconut_develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/__coconut__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/__coconut__/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60331 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/__coconut__/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/__coconut__/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/xontrib/coconut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/FAQ.md
+-rw-r--r--   0 runner    (1001) docker     (123)    65131 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/HELP.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:08:05.000000 coconut-develop-3.0.3.post0.dev5/_coconut/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/_coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/_coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-03 08:29:10.000000 coconut-develop-3.0.3.post0.dev5/_coconut/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `coconut-develop-3.0.3.post0.dev4/CONTRIBUTING.md` & `coconut-develop-3.0.3.post0.dev5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/DOCS.md` & `coconut-develop-3.0.3.post0.dev5/DOCS.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/FAQ.md` & `coconut-develop-3.0.3.post0.dev5/FAQ.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/HELP.md` & `coconut-develop-3.0.3.post0.dev5/HELP.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/LICENSE.txt` & `coconut-develop-3.0.3.post0.dev5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/PKG-INFO` & `coconut-develop-3.0.3.post0.dev5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,100 @@
 Metadata-Version: 2.1
 Name: coconut-develop
-Version: 3.0.3.post0.dev4
+Version: 3.0.3.post0.dev5
 Summary: Simple, elegant, Pythonic functional programming.
 Home-page: http://coconut-lang.org
 Author: Evan Hubinger
 Author-email: evanjhub@gmail.com
 License: Apache 2.0
+Description: |logo| Coconut
+        ==============
+        
+        ..
+            <insert toctree here>
+        
+        .. |logo| image:: https://github.com/evhub/coconut/raw/gh-pages/favicon-32x32.png
+        
+        .. image:: https://opencollective.com/coconut/backers/badge.svg
+            :alt: Backers on Open Collective
+            :target: #backers
+        .. image:: https://opencollective.com/coconut/sponsors/badge.svg
+            :alt: Sponsors on Open Collective
+            :target: #sponsors
+        .. image:: https://badges.gitter.im/evhub/coconut.svg
+            :alt: Join the chat at https://gitter.im/evhub/coconut
+            :target: https://gitter.im/evhub/coconut?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+        
+        Coconut (`coconut-lang.org`__) is a variant of Python_ that **adds on top of Python syntax** new features for simple, elegant, Pythonic **functional programming**.
+        
+        __ Coconut_
+        .. _Coconut: http://coconut-lang.org/
+        
+        Coconut is developed on GitHub_ and hosted on PyPI_. Installing Coconut is as easy as opening a command prompt and entering::
+        
+            pip install coconut
+        
+        To help you get started, check out these links for more information about Coconut:
+        
+        - Tutorial_: If you're new to Coconut, a good place to start is Coconut's **tutorial**.
+        - Documentation_: If you're looking for info about a specific feature, check out Coconut's **documentation**.
+        - `Online Interpreter`_: If you want to try Coconut in your browser, check out Coconut's **online interpreter**.
+        - FAQ_: If you have general questions about Coconut—like who Coconut is built for and whether or not you should use it—Coconut's frequently asked questions are often the best place to start.
+        - `Create a New Issue <https://github.com/evhub/coconut/issues/new>`_: If you're having a problem with Coconut, creating a new issue detailing the problem will allow it to be addressed as soon as possible.
+        - Gitter_: For any questions, concerns, or comments about anything Coconut-related, ask around at Coconut's Gitter, a GitHub-integrated chat room for Coconut developers.
+        - Releases_: Want to know what's been added in recent Coconut versions? Check out the release log for all the new features and fixes.
+        
+        .. _Python: https://www.python.org/
+        .. _PyPI: https://pypi.python.org/pypi/coconut
+        .. _Tutorial: http://coconut.readthedocs.io/en/latest/HELP.html
+        .. _Documentation: http://coconut.readthedocs.io/en/latest/DOCS.html
+        .. _`Online Interpreter`: https://cs121-team-panda.github.io/coconut-interpreter
+        .. _FAQ: http://coconut.readthedocs.io/en/latest/FAQ.html
+        .. _GitHub: https://github.com/evhub/coconut
+        .. _Gitter: https://gitter.im/evhub/coconut
+        .. _Releases: https://github.com/evhub/coconut/releases
+        
+        Credits
+        +++++++
+        
+        Contributors
+        ------------
+        
+        This project exists thanks to all the people who contribute! `Become a contributor`__.
+        
+        .. image:: https://opencollective.com/coconut/contributors.svg?width=890&button=false
+            :target: https://github.com/evhub/coconut/graphs/contributors
+        
+        __ Contributor_
+        .. _Contributor: http://coconut.readthedocs.io/en/develop/CONTRIBUTING.html
+        
+        Backers
+        -------
+        
+        Thank you to all our backers! `Become a backer`__.
+        
+        .. image:: https://opencollective.com/coconut/backers.svg?width=890
+            :target: https://opencollective.com/coconut#backers
+        
+        __ Backer_
+        .. _Backer: https://opencollective.com/coconut#backer
+        
+        Sponsors
+        --------
+        
+        Support Coconut by becoming a sponsor. Your logo will show up here with a link to your website. `Become a sponsor`__.
+        
+        .. image:: https://opencollective.com/XX/sponsor/0/avatar.svg
+            :target: https://opencollective.com/coconut/sponsor/0/website
+        
+        __ Sponsor_
+        .. _Sponsor: https://opencollective.com/coconut#sponsor
+        
 Keywords: functional,programming,language,compiler,pattern,pattern-matching,algebraic,data type,data types,lambda,lambdas,lazy,evaluation,lazy list,lazy lists,tail,recursion,call,recursive,infix,function,composition,compose,partial,application,currying,curry,pipeline,pipe,unicode,operator,operators,frozenset,literal,syntax,destructuring,assignment,fold,datamaker,prepattern,iterator,none,coalesce,coalescing,statement,lru_cache,memoization,backport,typing,embed,PEP 622,overrides,islice,itertools,functools,TYPE_CHECKING,Expected,breakpoint,help,reduce,takewhile,dropwhile,tee,count,makedata,consume,parallel_map,addpattern,recursive_iterator,concurrent_map,fmap,starmap,reiterable,scan,groupsof,memoize,zip_longest,override,flatten,ident,call,safe_call,flip,const,lift,all_equal,collectby,multi_enumerate,cartesian_product,multiset,cycle,windowsof,and_then,and_then_await,py_chr,py_dict,py_hex,py_input,py_int,py_map,py_object,py_oct,py_open,py_print,py_range,py_str,py_super,py_zip,py_filter,py_reversed,py_enumerate,py_raw_input,py_xrange,py_repr,py_breakpoint,_namedtuple_of,reveal_type,reveal_locals,MatchError,__fmap__,__iter_getitem__,data,match,case,cases,where,addpattern,then,operator,type,copyclosure,λ
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Interpreters
@@ -47,91 +131,7 @@
 Provides-Extra: xonsh
 Provides-Extra: jupyter
 Provides-Extra: all
 Provides-Extra: ipython
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: dev
-License-File: LICENSE.txt
-
-|logo| Coconut
-==============
-
-..
-    <insert toctree here>
-
-.. |logo| image:: https://github.com/evhub/coconut/raw/gh-pages/favicon-32x32.png
-
-.. image:: https://opencollective.com/coconut/backers/badge.svg
-    :alt: Backers on Open Collective
-    :target: #backers
-.. image:: https://opencollective.com/coconut/sponsors/badge.svg
-    :alt: Sponsors on Open Collective
-    :target: #sponsors
-.. image:: https://badges.gitter.im/evhub/coconut.svg
-    :alt: Join the chat at https://gitter.im/evhub/coconut
-    :target: https://gitter.im/evhub/coconut?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-
-Coconut (`coconut-lang.org`__) is a variant of Python_ that **adds on top of Python syntax** new features for simple, elegant, Pythonic **functional programming**.
-
-__ Coconut_
-.. _Coconut: http://coconut-lang.org/
-
-Coconut is developed on GitHub_ and hosted on PyPI_. Installing Coconut is as easy as opening a command prompt and entering::
-
-    pip install coconut
-
-To help you get started, check out these links for more information about Coconut:
-
-- Tutorial_: If you're new to Coconut, a good place to start is Coconut's **tutorial**.
-- Documentation_: If you're looking for info about a specific feature, check out Coconut's **documentation**.
-- `Online Interpreter`_: If you want to try Coconut in your browser, check out Coconut's **online interpreter**.
-- FAQ_: If you have general questions about Coconut—like who Coconut is built for and whether or not you should use it—Coconut's frequently asked questions are often the best place to start.
-- `Create a New Issue <https://github.com/evhub/coconut/issues/new>`_: If you're having a problem with Coconut, creating a new issue detailing the problem will allow it to be addressed as soon as possible.
-- Gitter_: For any questions, concerns, or comments about anything Coconut-related, ask around at Coconut's Gitter, a GitHub-integrated chat room for Coconut developers.
-- Releases_: Want to know what's been added in recent Coconut versions? Check out the release log for all the new features and fixes.
-
-.. _Python: https://www.python.org/
-.. _PyPI: https://pypi.python.org/pypi/coconut
-.. _Tutorial: http://coconut.readthedocs.io/en/latest/HELP.html
-.. _Documentation: http://coconut.readthedocs.io/en/latest/DOCS.html
-.. _`Online Interpreter`: https://cs121-team-panda.github.io/coconut-interpreter
-.. _FAQ: http://coconut.readthedocs.io/en/latest/FAQ.html
-.. _GitHub: https://github.com/evhub/coconut
-.. _Gitter: https://gitter.im/evhub/coconut
-.. _Releases: https://github.com/evhub/coconut/releases
-
-Credits
-+++++++
-
-Contributors
-------------
-
-This project exists thanks to all the people who contribute! `Become a contributor`__.
-
-.. image:: https://opencollective.com/coconut/contributors.svg?width=890&button=false
-    :target: https://github.com/evhub/coconut/graphs/contributors
-
-__ Contributor_
-.. _Contributor: http://coconut.readthedocs.io/en/develop/CONTRIBUTING.html
-
-Backers
--------
-
-Thank you to all our backers! `Become a backer`__.
-
-.. image:: https://opencollective.com/coconut/backers.svg?width=890
-    :target: https://opencollective.com/coconut#backers
-
-__ Backer_
-.. _Backer: https://opencollective.com/coconut#backer
-
-Sponsors
---------
-
-Support Coconut by becoming a sponsor. Your logo will show up here with a link to your website. `Become a sponsor`__.
-
-.. image:: https://opencollective.com/XX/sponsor/0/avatar.svg
-    :target: https://opencollective.com/coconut/sponsor/0/website
-
-__ Sponsor_
-.. _Sponsor: https://opencollective.com/coconut#sponsor
```

### Comparing `coconut-develop-3.0.3.post0.dev4/README.rst` & `coconut-develop-3.0.3.post0.dev5/README.rst`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/__coconut__/__init__.py` & `coconut-develop-3.0.3.post0.dev5/__coconut__/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/__coconut__/__init__.pyi` & `coconut-develop-3.0.3.post0.dev5/__coconut__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/_coconut/__init__.py` & `coconut-develop-3.0.3.post0.dev5/_coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/_coconut/__init__.pyi` & `coconut-develop-3.0.3.post0.dev5/_coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/__coconut__.py` & `coconut-develop-3.0.3.post0.dev5/coconut/__coconut__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/__coconut__.pyi` & `coconut-develop-3.0.3.post0.dev5/coconut/__coconut__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/__init__.py` & `coconut-develop-3.0.3.post0.dev5/coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/__init__.pyi` & `coconut-develop-3.0.3.post0.dev5/coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/__main__.py` & `coconut-develop-3.0.3.post0.dev5/coconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/_pyparsing.py` & `coconut-develop-3.0.3.post0.dev5/coconut/_pyparsing.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/api.py` & `coconut-develop-3.0.3.post0.dev5/coconut/api.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/api.pyi` & `coconut-develop-3.0.3.post0.dev5/coconut/api.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/command/__init__.py` & `coconut-develop-3.0.3.post0.dev5/coconut/command/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/command/cli.py` & `coconut-develop-3.0.3.post0.dev5/coconut/command/cli.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/command/command.py` & `coconut-develop-3.0.3.post0.dev5/coconut/command/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from contextlib import contextmanager
 from subprocess import CalledProcessError
 
 from coconut._pyparsing import (
     unset_fast_pyparsing_reprs,
     collect_timing_info,
     print_timing_info,
+    SUPPORTS_INCREMENTAL,
 )
 
 from coconut.compiler import Compiler
 from coconut.exceptions import (
     CoconutException,
     CoconutInternalException,
 )
@@ -69,14 +70,15 @@
     jupyter_console_commands,
     default_jobs,
     create_package_retries,
     default_use_cache_dir,
     coconut_cache_dir,
     coconut_run_kwargs,
     interpreter_uses_incremental,
+    disable_incremental_for_len,
 )
 from coconut.util import (
     univ_open,
     ver_tuple_to_str,
     install_custom_kernel,
     get_clock_time,
     first_import_time,
@@ -259,14 +261,16 @@
                 logger.warn("--stack-size should generally be a multiple of 4, not {stack_size} (to support 4 KB pages)".format(stack_size=args.stack_size))
             if args.mypy is not None and args.no_line_numbers:
                 logger.warn("using --mypy running with --no-line-numbers is not recommended; mypy error messages won't include Coconut line numbers")
             if args.line_numbers and args.no_line_numbers:
                 raise CoconutException("cannot compile with both --line-numbers and --no-line-numbers")
             if args.site_install and args.site_uninstall:
                 raise CoconutException("cannot --site-install and --site-uninstall simultaneously")
+            if args.incremental and not SUPPORTS_INCREMENTAL:
+                raise CoconutException("--incremental mode requires cPyparsing (run '{python} -m pip install --upgrade cPyparsing' to fix)".format(python=sys.executable))
             for and_args in getattr(args, "and") or []:
                 if len(and_args) > 2:
                     raise CoconutException(
                         "--and accepts at most two arguments, source and dest ({n} given: {args!r})".format(
                             n=len(and_args),
                             args=and_args,
                         ),
@@ -599,21 +603,24 @@
                     else:
                         self.execute_file(destpath, argv_source_path=codepath)
 
             parse_kwargs = dict(
                 filename=os.path.basename(codepath),
             )
             if self.incremental:
-                code_dir, code_fname = os.path.split(codepath)
+                if disable_incremental_for_len is not None and len(code) > disable_incremental_for_len:
+                    logger.warn("--incremental mode is not currently supported for files as large as {codepath!r}")
+                else:
+                    code_dir, code_fname = os.path.split(codepath)
 
-                cache_dir = os.path.join(code_dir, coconut_cache_dir)
-                ensure_dir(cache_dir)
+                    cache_dir = os.path.join(code_dir, coconut_cache_dir)
+                    ensure_dir(cache_dir)
 
-                pickle_fname = code_fname + ".pickle"
-                parse_kwargs["incremental_cache_filename"] = os.path.join(cache_dir, pickle_fname)
+                    pickle_fname = code_fname + ".pickle"
+                    parse_kwargs["incremental_cache_filename"] = os.path.join(cache_dir, pickle_fname)
 
             if package is True:
                 self.submit_comp_job(codepath, callback, "parse_package", code, package_level=package_level, **parse_kwargs)
             elif package is False:
                 self.submit_comp_job(codepath, callback, "parse_file", code, **parse_kwargs)
             else:
                 raise CoconutInternalException("invalid value for package", package)
@@ -818,17 +825,18 @@
 
             if allow_show and self.display:
                 logger.print(compiled)
 
             if path is None:  # header is not included
                 if not self.mypy:
                     no_str_code = self.comp.remove_strs(compiled)
-                    result = mypy_builtin_regex.search(no_str_code)
-                    if result:
-                        logger.warn("found mypy-only built-in " + repr(result.group(0)) + "; pass --mypy to use mypy-only built-ins at the interpreter")
+                    if no_str_code is not None:
+                        result = mypy_builtin_regex.search(no_str_code)
+                        if result:
+                            logger.warn("found mypy-only built-in " + repr(result.group(0)) + "; pass --mypy to use mypy-only built-ins at the interpreter")
 
             else:  # header is included
                 compiled = rem_encoding(compiled)
 
             self.runner.run(compiled, use_eval=use_eval, path=path, all_errors_exit=path is not None)
 
             self.run_mypy(code=self.runner.was_run_code())
```

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/command/command.pyi` & `coconut-develop-3.0.3.post0.dev5/coconut/command/command.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/command/mypy.py` & `coconut-develop-3.0.3.post0.dev5/coconut/command/mypy.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/command/util.py` & `coconut-develop-3.0.3.post0.dev5/coconut/command/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/command/watch.py` & `coconut-develop-3.0.3.post0.dev5/coconut/command/watch.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/compiler/__init__.py` & `coconut-develop-3.0.3.post0.dev5/coconut/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/compiler/compiler.py` & `coconut-develop-3.0.3.post0.dev5/coconut/compiler/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -930,20 +930,22 @@
             yield
         except ParseBaseException as err:
             # don't reformat, since we might have gotten here because reformat failed
             complain(self.make_parse_err(err, include_ln=False, reformat=False, endpoint=True))
         except CoconutException as err:
             complain(err)
 
-    def remove_strs(self, inputstring, inner_environment=True):
-        """Remove strings/comments from the given input."""
-        with self.complain_on_err():
+    def remove_strs(self, inputstring, inner_environment=True, **kwargs):
+        """Remove strings/comments from the given input if possible."""
+        try:
             with (self.inner_environment() if inner_environment else noop_ctx()):
-                return self.str_proc(inputstring)
-        return inputstring
+                return self.str_proc(inputstring, **kwargs)
+        except Exception:
+            logger.log_exc()
+        return None
 
     def get_matcher(self, original, loc, check_var, name_list=None):
         """Get a Matcher object."""
         return Matcher(self, original, loc, check_var, name_list=name_list)
 
     def add_ref(self, reftype, data):
         """Add a reference and return the identifier."""
@@ -1209,15 +1211,15 @@
         with self.lock:
             self.reset(keep_state, filename)
             self.current_compiler[0] = self
             yield
 
     def streamline(self, grammar, inputstring="", force=False):
         """Streamline the given grammar for the given inputstring."""
-        if force or (streamline_grammar_for_len is not None and len(inputstring) >= streamline_grammar_for_len):
+        if force or (streamline_grammar_for_len is not None and len(inputstring) > streamline_grammar_for_len):
             start_time = get_clock_time()
             prep_grammar(grammar, streamline=True)
             logger.log_lambda(
                 lambda: "Streamlined {grammar} in {time} seconds (streamlined due to receiving input of length {length}).".format(
                     grammar=get_name(grammar),
                     time=get_clock_time() - start_time,
                     length=len(inputstring),
@@ -1257,15 +1259,15 @@
             if streamline:
                 self.streamline(parser, inputstring)
             # unpickling must happen after streamlining and must occur in the
             #  compiler so that it happens in the same process as compilation
             if incremental_cache_filename is not None:
                 incremental_enabled = enable_incremental_parsing()
                 if not incremental_enabled:
-                    raise CoconutException("--incremental mode requires cPyparsing (run '{python} -m pip install --upgrade cPyparsing' to fix)".format(python=sys.executable))
+                    raise CoconutException("incremental_cache_filename requires cPyparsing (run '{python} -m pip install --upgrade cPyparsing' to fix)".format(python=sys.executable))
                 did_load_cache = unpickle_incremental_cache(incremental_cache_filename)
                 logger.log("{Loaded} incremental cache for {filename!r} from {incremental_cache_filename!r}.".format(
                     Loaded="Loaded" if did_load_cache else "Failed to load",
                     filename=filename,
                     incremental_cache_filename=incremental_cache_filename,
                 ))
             pre_procd = None
```

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/compiler/grammar.py` & `coconut-develop-3.0.3.post0.dev5/coconut/compiler/grammar.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/compiler/header.py` & `coconut-develop-3.0.3.post0.dev5/coconut/compiler/header.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/compiler/matching.py` & `coconut-develop-3.0.3.post0.dev5/coconut/compiler/matching.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/compiler/templates/header.py_template` & `coconut-develop-3.0.3.post0.dev5/coconut/compiler/templates/header.py_template`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/compiler/util.py` & `coconut-develop-3.0.3.post0.dev5/coconut/compiler/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,16 +62,17 @@
     Empty,
     Literal,
     CaselessLiteral,
     Group,
     ParserElement,
     _trim_arity,
     _ParseResultsWithOffset,
-    line as _line,
     all_parse_elements,
+    line as _line,
+    __version__ as pyparsing_version,
 )
 
 from coconut.integrations import embed
 from coconut.util import (
     override,
     get_name,
     get_target_info,
@@ -107,14 +108,15 @@
     reserved_prefix,
     incremental_mode_cache_size,
     default_incremental_cache_size,
     repeatedly_clear_incremental_cache,
     py_vers_with_eols,
     unwrapper,
     incremental_cache_limit,
+    incremental_mode_cache_successes,
 )
 from coconut.exceptions import (
     CoconutException,
     CoconutInternalException,
     CoconutDeferredSyntaxError,
 )
 
@@ -352,34 +354,17 @@
             kwargs["ignore_one_token"] = ignore_one_token
         if not trim_arity:
             kwargs["trim_arity"] = trim_arity
         action = partial(ComputationNode, action, **kwargs)
     return add_action(item, action, make_copy)
 
 
-def should_clear_cache():
-    """Determine if we should be clearing the packrat cache."""
-    if not ParserElement._packratEnabled:
-        internal_assert(not ParserElement._incrementalEnabled)
-        return False
-    if not ParserElement._incrementalEnabled:
-        return True
-    if ParserElement._incrementalWithResets and repeatedly_clear_incremental_cache:
-        return True
-    if incremental_cache_limit is not None and len(ParserElement.packrat_cache) > incremental_cache_limit:
-        return True
-    return False
-
-
 def final_evaluate_tokens(tokens):
     """Same as evaluate_tokens but should only be used once a parse is assured."""
-    # don't clear the cache in incremental mode
-    if should_clear_cache():
-        # clear cache without resetting stats
-        ParserElement.packrat_cache.clear()
+    clear_packrat_cache()
     return evaluate_tokens(tokens)
 
 
 def final(item):
     """Collapse the computation graph upon parsing the given item."""
     # evaluate_tokens expects a computation graph, so we just call add_action directly
     return add_action(trace(item), final_evaluate_tokens)
@@ -533,14 +518,47 @@
             # this is sketchy, so errors should only be complained
             return get_func_closure(packrat_cache.get.__func__)["cache"]
         except Exception as err:
             complain(err)
             return {}
 
 
+def should_clear_cache():
+    """Determine if we should be clearing the packrat cache."""
+    if not ParserElement._packratEnabled:
+        return False
+    if SUPPORTS_INCREMENTAL:
+        if not ParserElement._incrementalEnabled:
+            return True
+        if ParserElement._incrementalWithResets and repeatedly_clear_incremental_cache:
+            return True
+        if incremental_cache_limit is not None and len(ParserElement.packrat_cache) > incremental_cache_limit:
+            # only clear the second half of the cache, since the first
+            #  half is what will help us next time we recompile
+            return "second half"
+    return False
+
+
+def clear_packrat_cache():
+    """Clear the packrat cache if applicable."""
+    clear_cache = should_clear_cache()
+    if not clear_cache:
+        return
+    if clear_cache == "second half":
+        cache_items = list(get_pyparsing_cache().items())
+        restore_items = cache_items[:len(cache_items) // 2]
+    else:
+        restore_items = ()
+    # clear cache without resetting stats
+    ParserElement.packrat_cache.clear()
+    # restore any items we want to keep
+    for lookup, value in restore_items:
+        ParserElement.packrat_cache.set(lookup, value)
+
+
 def get_cache_items_for(original):
     """Get items from the pyparsing cache filtered to only from parsing original."""
     cache = get_pyparsing_cache()
     for lookup, value in cache.items():
         got_orig = lookup[1]
         if got_orig == original:
             yield lookup, value
@@ -557,14 +575,15 @@
     return highest_loc
 
 
 def enable_incremental_parsing():
     """Enable incremental parsing mode where prefix/suffix parses are reused."""
     if not SUPPORTS_INCREMENTAL:
         return False
+    ParserElement._should_cache_incremental_success = incremental_mode_cache_successes
     if ParserElement._incrementalEnabled and not ParserElement._incrementalWithResets:  # incremental mode is already enabled
         return True
     ParserElement._incrementalEnabled = False
     try:
         ParserElement.enableIncremental(incremental_mode_cache_size, still_reset_cache=False)
     except ImportError as err:
         raise CoconutException(str(err))
@@ -575,27 +594,35 @@
 def pickle_incremental_cache(original, filename, protocol=pickle.HIGHEST_PROTOCOL):
     """Pickle the pyparsing cache for original to filename."""
     internal_assert(all_parse_elements is not None, "pickle_incremental_cache requires cPyparsing")
 
     pickleable_cache_items = []
     for lookup, value in get_cache_items_for(original):
         if incremental_mode_cache_size is not None and len(pickleable_cache_items) > incremental_mode_cache_size:
-            complain("got too large incremental cache: " + str(len(get_pyparsing_cache())) + " > " + str(incremental_mode_cache_size))
+            complain(
+                "got too large incremental cache: "
+                + str(len(get_pyparsing_cache())) + " > " + str(incremental_mode_cache_size)
+            )
             break
         if len(pickleable_cache_items) >= incremental_cache_limit:
             break
-        pickleable_lookup = (lookup[0].parse_element_index,) + lookup[1:]
-        pickleable_cache_items.append((pickleable_lookup, value))
+        loc = lookup[2]
+        # only include cache items that aren't at the start or end, since those
+        #  are the only ones that parseIncremental will reuse
+        if 0 < loc < len(original) - 1:
+            pickleable_lookup = (lookup[0].parse_element_index,) + lookup[1:]
+            pickleable_cache_items.append((pickleable_lookup, value))
 
     logger.log("Saving {num_items} incremental cache items to {filename!r}.".format(
         num_items=len(pickleable_cache_items),
         filename=filename,
     ))
     pickle_info_obj = {
         "VERSION": VERSION,
+        "pyparsing_version": pyparsing_version,
         "pickleable_cache_items": pickleable_cache_items,
     }
     with univ_open(filename, "wb") as pickle_file:
         pickle.dump(pickle_info_obj, pickle_file, protocol=protocol)
 
 
 def unpickle_incremental_cache(filename):
@@ -606,33 +633,33 @@
         return False
     try:
         with univ_open(filename, "rb") as pickle_file:
             pickle_info_obj = pickle.load(pickle_file)
     except Exception:
         logger.log_exc()
         return False
-    if pickle_info_obj["VERSION"] != VERSION:
+    if pickle_info_obj["VERSION"] != VERSION or pickle_info_obj["pyparsing_version"] != pyparsing_version:
         return False
+
     pickleable_cache_items = pickle_info_obj["pickleable_cache_items"]
     logger.log("Loaded {num_items} incremental cache items from {filename!r}.".format(
         num_items=len(pickleable_cache_items),
         filename=filename,
     ))
 
     max_cache_size = min(
         incremental_mode_cache_size or float("inf"),
         incremental_cache_limit or float("inf"),
     )
     if max_cache_size != float("inf"):
         pickleable_cache_items = pickleable_cache_items[-max_cache_size:]
 
-    packrat_cache = ParserElement.packrat_cache
     for pickleable_lookup, value in pickleable_cache_items:
         lookup = (all_parse_elements[pickleable_lookup[0]],) + pickleable_lookup[1:]
-        packrat_cache.set(lookup, value)
+        ParserElement.packrat_cache.set(lookup, value)
     return True
 
 
 # -----------------------------------------------------------------------------------------------------------------------
 # TARGETS:
 # -----------------------------------------------------------------------------------------------------------------------
 on_new_python = False
```

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/constants.py` & `coconut-develop-3.0.3.post0.dev5/coconut/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,30 +116,32 @@
 
 varchars = string.ascii_letters + string.digits + "_"
 
 use_computation_graph_env_var = "COCONUT_USE_COMPUTATION_GRAPH"
 
 # below constants are experimentally determined to maximize performance
 
-streamline_grammar_for_len = 4000
+streamline_grammar_for_len = 4096
+disable_incremental_for_len = streamline_grammar_for_len  # disables --incremental
 
 use_packrat_parser = True  # True also gives us better error messages
 packrat_cache_size = None  # only works because final() clears the cache
 
 # note that _parseIncremental produces much smaller caches
 use_incremental_if_available = True
 
 # these only apply to use_incremental_if_available, not compiler.util.enable_incremental_parsing()
 default_incremental_cache_size = None
 repeatedly_clear_incremental_cache = True
 never_clear_incremental_cache = False
 
 # this is what gets used in compiler.util.enable_incremental_parsing()
 incremental_mode_cache_size = None
-incremental_cache_limit = 524288  # clear cache when it gets this large
+incremental_cache_limit = 1048576  # clear cache when it gets this large
+incremental_mode_cache_successes = False
 
 use_left_recursion_if_available = False
 
 # -----------------------------------------------------------------------------------------------------------------------
 # COMPILER CONSTANTS:
 # -----------------------------------------------------------------------------------------------------------------------
 
@@ -957,15 +959,15 @@
         ("numpy", "py<3;cpy"),
         ("pandas", "py36"),
     ),
 }
 
 # min versions are inclusive
 min_versions = {
-    "cPyparsing": (2, 4, 7, 2, 2, 2),
+    "cPyparsing": (2, 4, 7, 2, 2, 3),
     ("pre-commit", "py3"): (3,),
     ("psutil", "py>=27"): (5,),
     "jupyter": (1, 0),
     "types-backports": (0, 1),
     ("futures", "py<3"): (3, 4),
     ("backports.functools-lru-cache", "py<3"): (1, 6),
     ("argparse", "py<27"): (1, 4),
```

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/convenience.py` & `coconut-develop-3.0.3.post0.dev5/coconut/convenience.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/convenience.pyi` & `coconut-develop-3.0.3.post0.dev5/coconut/convenience.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/exceptions.py` & `coconut-develop-3.0.3.post0.dev5/coconut/exceptions.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/highlighter.py` & `coconut-develop-3.0.3.post0.dev5/coconut/highlighter.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/icoconut/__init__.py` & `coconut-develop-3.0.3.post0.dev5/coconut/icoconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/icoconut/__main__.py` & `coconut-develop-3.0.3.post0.dev5/coconut/icoconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/icoconut/embed.py` & `coconut-develop-3.0.3.post0.dev5/coconut/icoconut/embed.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/icoconut/root.py` & `coconut-develop-3.0.3.post0.dev5/coconut/icoconut/root.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/integrations.py` & `coconut-develop-3.0.3.post0.dev5/coconut/integrations.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
                         logger.log_exc()
                         line = original_lines[-1]
                     remaining_pieces = remaining_ln_pieces.get(ln)
                     if remaining_pieces is None:
                         # we handle our own inner_environment rather than have remove_strs do it so that we can reformat
                         with self.compiler.inner_environment():
                             line_no_strs = self.compiler.remove_strs(line, inner_environment=False)
-                            if ";" in line_no_strs:
+                            if line_no_strs is not None and ";" in line_no_strs:
                                 remaining_pieces = [
                                     self.compiler.reformat(piece, ignore_errors=True)
                                     for piece in line_no_strs.split(";")
                                 ]
                             else:
                                 remaining_pieces = [line]
                     if remaining_pieces:
```

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/main.py` & `coconut-develop-3.0.3.post0.dev5/coconut/main.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/requirements.py` & `coconut-develop-3.0.3.post0.dev5/coconut/requirements.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/root.py` & `coconut-develop-3.0.3.post0.dev5/coconut/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -----------------------------------------------------------------------------------------------------------------------
 # VERSION:
 # -----------------------------------------------------------------------------------------------------------------------
 
 VERSION = "3.0.3"
 VERSION_NAME = None
 # False for release, int >= 1 for develop
-DEVELOP = 4
+DEVELOP = 5
 ALPHA = False  # for pre releases rather than post releases
 
 assert DEVELOP is False or DEVELOP >= 1, "DEVELOP must be False or an int >= 1"
 assert DEVELOP or not ALPHA, "alpha releases are only for develop"
 
 # -----------------------------------------------------------------------------------------------------------------------
 # UTILITIES:
```

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/terminal.py` & `coconut-develop-3.0.3.post0.dev5/coconut/terminal.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/__init__.py` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/__main__.py` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/constants_test.py` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/constants_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/main_test.py` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/main_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -808,14 +808,16 @@
             p.sendline("'1; 2' |> print")
             p.expect("1; 2")
             p.sendline('$ENV_VAR = "ABC"')
             p.expect("$")
             p.sendline('echo f"{$ENV_VAR}"; echo f"{$ENV_VAR}"')
             p.expect("ABC")
             p.expect("ABC")
+            p.sendline('len("""1\n3\n5""") |> print')
+            p.expect("5")
             if not PYPY or PY39:
                 if PY36:
                     p.sendline("echo 123;; 123")
                     p.expect("123;; 123")
                     p.sendline("echo abc; echo abc")
                     p.expect("abc")
                     p.expect("abc")
@@ -904,52 +906,50 @@
 
     def test_package(self):
         run(["--package"])
 
     def test_no_tco(self):
         run(["--no-tco"])
 
+    if PY35:
+        def test_no_wrap(self):
+            run(["--no-wrap"])
+
     # run fewer tests on Windows so appveyor doesn't time out
     if not WINDOWS:
         def test_keep_lines(self):
             run(["--keep-lines"])
 
         def test_strict(self):
             run(["--strict"])
 
         def test_and(self):
             run(["--and"])  # src and dest built by comp
 
-        def test_incremental(self):
-            run(["--incremental"])
-            # includes "Error" because exceptions include the whole file
-            run(["--incremental", "--force"], check_errors=False)
+        def test_run_arg(self):
+            run(use_run_arg=True)
 
-    if PY35:
-        def test_no_wrap(self):
-            run(["--no-wrap"])
+        if not PYPY and not PY26:
+            def test_jobs_zero(self):
+                run(["--jobs", "0"])
+
+        if not PYPY:
+            def test_incremental(self):
+                run(["--incremental"])
+                # includes "Error" because exceptions include the whole file
+                run(["--incremental", "--force"], check_errors=False)
 
     if get_bool_env_var("COCONUT_TEST_VERBOSE"):
         def test_verbose(self):
             run(["--jobs", "0", "--verbose"])
 
     if get_bool_env_var("COCONUT_TEST_TRACE"):
         def test_trace(self):
             run(["--jobs", "0", "--trace"], check_errors=False)
 
-    # avoids a strange, unreproducable failure on appveyor
-    if not (WINDOWS and sys.version_info[:2] == (3, 8)):
-        def test_run_arg(self):
-            run(use_run_arg=True)
-
-    # not WINDOWS is for appveyor timeout prevention
-    if not WINDOWS and not PYPY and not PY26:
-        def test_jobs_zero(self):
-            run(["--jobs", "0"])
-
 
 # more appveyor timeout prevention
 if not WINDOWS:
     @add_test_func_names
     class TestExternal(unittest.TestCase):
 
         if not PYPY or PY2:
```

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/agnostic/main.coco` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/main.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/agnostic/primary.coco` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/primary.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/agnostic/specific.coco` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/specific.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/agnostic/suite.coco` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/suite.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/agnostic/tutorial.coco` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/tutorial.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/agnostic/util.coco` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/agnostic/util.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/non_strict/non_strict_test.coco` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/non_strict/non_strict_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_3/py3_test.coco` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_3/py3_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_35/py35_test.coco` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_35/py35_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_36/py36_test.coco` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_36/py36_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/src/cocotest/target_sys/target_sys_test.coco` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/cocotest/target_sys/target_sys_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/tests/src/extras.coco` & `coconut-develop-3.0.3.post0.dev5/coconut/tests/src/extras.coco`

 * *Files 2% similar despite different names*

```diff
@@ -321,15 +321,18 @@
     assert_raises(-> parse("u''"), CoconutStyleError)
     assert_raises(-> parse("def f(x):\\\n pass"), CoconutStyleError)
     assert_raises(-> parse("abc "), CoconutStyleError, err_has="\n     ^")
     assert_raises(-> parse("abc", "file"), CoconutStyleError)
     assert_raises(-> parse("a=1;"), CoconutStyleError, err_has="\n     ^")
     assert_raises(-> parse("class derp(object)"), CoconutStyleError)
     assert_raises(-> parse("def f(a.b) = True"), CoconutStyleError, err_has="\n        ^")
-    assert_raises(-> parse("match def kwd_only_x_is_int_def_0(*, x is int = 0) = x"), CoconutStyleError, err_has="\n        ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~|")
+    assert_raises(-> parse("match def kwd_only_x_is_int_def_0(*, x is int = 0) = x"), CoconutStyleError, err_has=(
+        "\n        ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~|",
+        "\n        ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~/",
+    ))
     try:
         parse("""
 try:
     x is int is str = x
 except MatchError:
     pass
 else:
```

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut/util.py` & `coconut-develop-3.0.3.post0.dev5/coconut/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/coconut_develop.egg-info/SOURCES.txt` & `coconut-develop-3.0.3.post0.dev5/coconut_develop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/conf.py` & `coconut-develop-3.0.3.post0.dev5/conf.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/setup.py` & `coconut-develop-3.0.3.post0.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.3.post0.dev4/xontrib/coconut.py` & `coconut-develop-3.0.3.post0.dev5/xontrib/coconut.py`

 * *Files identical despite different names*

