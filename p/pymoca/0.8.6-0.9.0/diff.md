# Comparing `tmp/pymoca-0.8.6.tar.gz` & `tmp/pymoca-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymoca-0.8.6.tar", last modified: Fri Jun 18 15:44:12 2021, max compression
+gzip compressed data, was "pymoca-0.9.0.tar", last modified: Tue Oct  5 09:14:52 2021, max compression
```

## Comparing `pymoca-0.8.6.tar` & `pymoca-0.9.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:12.436522 pymoca-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2021-06-18 15:44:02.000000 pymoca-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-06-18 15:44:02.000000 pymoca-0.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1677 2021-06-18 15:44:12.436522 pymoca-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2021-06-18 15:44:02.000000 pymoca-0.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:12.432522 pymoca-0.8.6/doc/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-18 15:44:02.000000 pymoca-0.8.6/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     7192 2021-06-18 15:44:02.000000 pymoca-0.8.6/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     6710 2021-06-18 15:44:02.000000 pymoca-0.8.6/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:12.432522 pymoca-0.8.6/doc/source/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-06-18 15:44:02.000000 pymoca-0.8.6/doc/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)      944 2021-06-18 15:44:02.000000 pymoca-0.8.6/doc/source/pymoca.generated.rst
--rw-r--r--   0 runner    (1001) docker     (121)      899 2021-06-18 15:44:02.000000 pymoca-0.8.6/doc/source/pymoca.rst
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-06-18 15:44:02.000000 pymoca-0.8.6/doc/source/setup.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:12.432522 pymoca-0.8.6/java/
--rw-r--r--   0 runner    (1001) docker     (121)  2046402 2021-06-18 15:44:02.000000 pymoca-0.8.6/java/antlr-4.7-complete.jar
--rw-r--r--   0 runner    (1001) docker     (121)      863 2021-06-18 15:44:12.440523 pymoca-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4254 2021-06-18 15:44:02.000000 pymoca-0.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:12.428522 pymoca-0.8.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:12.440523 pymoca-0.8.6/src/pymoca/
--rw-r--r--   0 runner    (1001) docker     (121)    16518 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/Modelica.g4
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-06-18 15:44:12.440523 pymoca-0.8.6/src/pymoca/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    26896 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/ast.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:12.436522 pymoca-0.8.6/src/pymoca/backends/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:12.436522 pymoca-0.8.6/src/pymoca/backends/casadi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/casadi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1295 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/casadi/_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     3086 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/casadi/alias_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)    19331 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/casadi/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    42073 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/casadi/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)    58216 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/casadi/model.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/casadi/mtensor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:12.436522 pymoca-0.8.6/src/pymoca/backends/sympy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/sympy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7394 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/sympy/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5792 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/sympy/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:12.436522 pymoca-0.8.6/src/pymoca/backends/xml/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      980 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/xml/analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     4431 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/xml/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7847 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/xml/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    14170 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/xml/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     5236 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/backends/xml/sim_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:12.436522 pymoca-0.8.6/src/pymoca/generated/
--rw-r--r--   0 runner    (1001) docker     (121)    31200 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/generated/ModelicaLexer.py
--rw-r--r--   0 runner    (1001) docker     (121)    37807 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/generated/ModelicaListener.py
--rw-r--r--   0 runner    (1001) docker     (121)   303432 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/generated/ModelicaParser.py
--rw-r--r--   0 runner    (1001) docker     (121)    22260 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/generated/ModelicaVisitor.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32609 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    47054 2021-06-18 15:44:02.000000 pymoca-0.8.6/src/pymoca/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 15:44:12.436522 pymoca-0.8.6/src/pymoca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1677 2021-06-18 15:44:12.000000 pymoca-0.8.6/src/pymoca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2021-06-18 15:44:12.000000 pymoca-0.8.6/src/pymoca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-18 15:44:12.000000 pymoca-0.8.6/src/pymoca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      257 2021-06-18 15:44:12.000000 pymoca-0.8.6/src/pymoca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-18 15:44:12.000000 pymoca-0.8.6/src/pymoca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2021-06-18 15:44:02.000000 pymoca-0.8.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:52.662485 pymoca-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1512 2021-10-05 09:14:43.000000 pymoca-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-10-05 09:14:43.000000 pymoca-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1664 2021-10-05 09:14:52.662485 pymoca-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2021-10-05 09:14:43.000000 pymoca-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:52.658485 pymoca-0.9.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-05 09:14:43.000000 pymoca-0.9.0/doc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     7192 2021-10-05 09:14:43.000000 pymoca-0.9.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     6710 2021-10-05 09:14:43.000000 pymoca-0.9.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:52.658485 pymoca-0.9.0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2021-10-05 09:14:43.000000 pymoca-0.9.0/doc/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      944 2021-10-05 09:14:43.000000 pymoca-0.9.0/doc/source/pymoca.generated.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2021-10-05 09:14:43.000000 pymoca-0.9.0/doc/source/pymoca.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2021-10-05 09:14:43.000000 pymoca-0.9.0/doc/source/setup.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:52.658485 pymoca-0.9.0/java/
+-rw-r--r--   0 runner    (1001) docker     (121)  2046402 2021-10-05 09:14:43.000000 pymoca-0.9.0/java/antlr-4.7-complete.jar
+-rw-r--r--   0 runner    (1001) docker     (121)      863 2021-10-05 09:14:52.666485 pymoca-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4254 2021-10-05 09:14:43.000000 pymoca-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:52.654485 pymoca-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:52.666485 pymoca-0.9.0/src/pymoca/
+-rw-r--r--   0 runner    (1001) docker     (121)    16518 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/Modelica.g4
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-10-05 09:14:52.666485 pymoca-0.9.0/src/pymoca/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26896 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/ast.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:52.662485 pymoca-0.9.0/src/pymoca/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:52.662485 pymoca-0.9.0/src/pymoca/backends/casadi/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/casadi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1295 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/casadi/_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3086 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/casadi/alias_relation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19331 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/casadi/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42073 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/casadi/generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    58216 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/casadi/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/casadi/mtensor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:52.662485 pymoca-0.9.0/src/pymoca/backends/sympy/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/sympy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7394 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/sympy/generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5792 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/sympy/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:52.662485 pymoca-0.9.0/src/pymoca/backends/xml/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/xml/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4431 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/xml/generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7847 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/xml/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14170 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/xml/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5236 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/backends/xml/sim_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:52.662485 pymoca-0.9.0/src/pymoca/generated/
+-rw-r--r--   0 runner    (1001) docker     (121)    31200 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/generated/ModelicaLexer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37807 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/generated/ModelicaListener.py
+-rw-r--r--   0 runner    (1001) docker     (121)   303432 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/generated/ModelicaParser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22260 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/generated/ModelicaVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32609 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47054 2021-10-05 09:14:43.000000 pymoca-0.9.0/src/pymoca/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 09:14:52.662485 pymoca-0.9.0/src/pymoca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1664 2021-10-05 09:14:52.000000 pymoca-0.9.0/src/pymoca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1346 2021-10-05 09:14:52.000000 pymoca-0.9.0/src/pymoca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-05 09:14:52.000000 pymoca-0.9.0/src/pymoca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2021-10-05 09:14:52.000000 pymoca-0.9.0/src/pymoca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-05 09:14:52.000000 pymoca-0.9.0/src/pymoca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    68611 2021-10-05 09:14:43.000000 pymoca-0.9.0/versioneer.py
```

### Comparing `pymoca-0.8.6/LICENSE` & `pymoca-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/PKG-INFO` & `pymoca-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: pymoca
-Version: 0.8.6
+Version: 0.9.0
 Summary: A python/modelica based simulation environment.
 Home-page: https://github.com/pymoca/pymoca
 Author: James Goppert
 Author-email: james.goppert@gmail.com
 Maintainer: James Goppert
 Maintainer-email: james.goppert@gmail.com
 License: BSD
 Download-URL: https://github.com/pymoca/pymoca
-Description: Pymoca contains a Python based compiler for the modelica language
-        and enables interacting with Modelica easily in Python.
-        
-        
 Platform: Windows
 Platform: Linux
 Platform: Solaris
 Platform: Mac OS-X
 Platform: Unix
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -39,7 +35,14 @@
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Python: >=3.5
 Provides-Extra: casadi
 Provides-Extra: lxml
 Provides-Extra: sympy
 Provides-Extra: examples
 Provides-Extra: all
+License-File: LICENSE
+
+Pymoca contains a Python based compiler for the modelica language
+and enables interacting with Modelica easily in Python.
+
+
+
```

### Comparing `pymoca-0.8.6/README.md` & `pymoca-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/doc/Makefile` & `pymoca-0.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/doc/make.bat` & `pymoca-0.9.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/doc/source/pymoca.generated.rst` & `pymoca-0.9.0/doc/source/pymoca.generated.rst`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/doc/source/pymoca.rst` & `pymoca-0.9.0/doc/source/pymoca.rst`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/java/antlr-4.7-complete.jar` & `pymoca-0.9.0/java/antlr-4.7-complete.jar`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/setup.cfg` & `pymoca-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/setup.py` & `pymoca-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/Modelica.g4` & `pymoca-0.9.0/src/pymoca/Modelica.g4`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/ast.py` & `pymoca-0.9.0/src/pymoca/ast.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/backends/casadi/_options.py` & `pymoca-0.9.0/src/pymoca/backends/casadi/_options.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/backends/casadi/alias_relation.py` & `pymoca-0.9.0/src/pymoca/backends/casadi/alias_relation.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/backends/casadi/api.py` & `pymoca-0.9.0/src/pymoca/backends/casadi/api.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/backends/casadi/generator.py` & `pymoca-0.9.0/src/pymoca/backends/casadi/generator.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/backends/casadi/model.py` & `pymoca-0.9.0/src/pymoca/backends/casadi/model.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/backends/casadi/mtensor.py` & `pymoca-0.9.0/src/pymoca/backends/casadi/mtensor.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/backends/sympy/generator.py` & `pymoca-0.9.0/src/pymoca/backends/sympy/generator.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/backends/sympy/runtime.py` & `pymoca-0.9.0/src/pymoca/backends/sympy/runtime.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/backends/xml/analysis.py` & `pymoca-0.9.0/src/pymoca/backends/xml/analysis.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/backends/xml/generator.py` & `pymoca-0.9.0/src/pymoca/backends/xml/generator.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/backends/xml/model.py` & `pymoca-0.9.0/src/pymoca/backends/xml/model.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/backends/xml/parser.py` & `pymoca-0.9.0/src/pymoca/backends/xml/parser.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/backends/xml/sim_scipy.py` & `pymoca-0.9.0/src/pymoca/backends/xml/sim_scipy.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/generated/ModelicaLexer.py` & `pymoca-0.9.0/src/pymoca/generated/ModelicaLexer.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/generated/ModelicaListener.py` & `pymoca-0.9.0/src/pymoca/generated/ModelicaListener.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/generated/ModelicaParser.py` & `pymoca-0.9.0/src/pymoca/generated/ModelicaParser.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/generated/ModelicaVisitor.py` & `pymoca-0.9.0/src/pymoca/generated/ModelicaVisitor.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/parser.py` & `pymoca-0.9.0/src/pymoca/parser.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca/tree.py` & `pymoca-0.9.0/src/pymoca/tree.py`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/src/pymoca.egg-info/PKG-INFO` & `pymoca-0.9.0/src/pymoca.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: pymoca
-Version: 0.8.6
+Version: 0.9.0
 Summary: A python/modelica based simulation environment.
 Home-page: https://github.com/pymoca/pymoca
 Author: James Goppert
 Author-email: james.goppert@gmail.com
 Maintainer: James Goppert
 Maintainer-email: james.goppert@gmail.com
 License: BSD
 Download-URL: https://github.com/pymoca/pymoca
-Description: Pymoca contains a Python based compiler for the modelica language
-        and enables interacting with Modelica easily in Python.
-        
-        
 Platform: Windows
 Platform: Linux
 Platform: Solaris
 Platform: Mac OS-X
 Platform: Unix
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -39,7 +35,14 @@
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Python: >=3.5
 Provides-Extra: casadi
 Provides-Extra: lxml
 Provides-Extra: sympy
 Provides-Extra: examples
 Provides-Extra: all
+License-File: LICENSE
+
+Pymoca contains a Python based compiler for the modelica language
+and enables interacting with Modelica easily in Python.
+
+
+
```

### Comparing `pymoca-0.8.6/src/pymoca.egg-info/SOURCES.txt` & `pymoca-0.9.0/src/pymoca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymoca-0.8.6/versioneer.py` & `pymoca-0.9.0/versioneer.py`

 * *Files identical despite different names*

