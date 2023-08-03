# Comparing `tmp/yams-0.50.0.tar.gz` & `tmp/yams-0.50.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yams-0.50.0.tar", last modified: Wed Jul 19 08:48:09 2023, max compression
+gzip compressed data, was "yams-0.50.1.tar", last modified: Thu Aug  3 15:34:15 2023, max compression
```

## Comparing `yams-0.50.0.tar` & `yams-0.50.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.471916 yams-0.50.0/
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    17987 2023-07-17 22:32:31.000000 yams-0.50.0/COPYING
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    26527 2023-07-17 22:32:31.000000 yams-0.50.0/COPYING.LESSER
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    13724 2023-07-17 22:32:31.000000 yams-0.50.0/ChangeLog
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      469 2023-07-17 22:32:31.000000 yams-0.50.0/MANIFEST.in
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1397 2023-07-19 08:48:09.471916 yams-0.50.0/PKG-INFO
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      969 2023-07-17 22:32:31.000000 yams-0.50.0/README.rst
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1679 2023-07-19 08:36:22.000000 yams-0.50.0/__pkginfo__.py
-drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.459916 yams-0.50.0/bin/
--rwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)     3838 2023-07-17 22:32:31.000000 yams-0.50.0/bin/owl2yams
--rwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)       94 2023-07-17 22:32:31.000000 yams-0.50.0/bin/yams-check
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      360 2023-07-17 22:32:31.000000 yams-0.50.0/bin/yams-check.bat
--rwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)       94 2023-07-17 22:32:31.000000 yams-0.50.0/bin/yams-view
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      360 2023-07-17 22:32:31.000000 yams-0.50.0/bin/yams-view.bat
-drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.459916 yams-0.50.0/docs/
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      634 2023-07-17 22:32:31.000000 yams-0.50.0/docs/Makefile
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1923 2023-07-17 22:32:31.000000 yams-0.50.0/docs/conf.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      460 2023-07-17 22:32:31.000000 yams-0.50.0/docs/index.rst
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      760 2023-07-17 22:32:31.000000 yams-0.50.0/docs/make.bat
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1415 2023-07-17 22:32:31.000000 yams-0.50.0/docs/yams.rst
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)       74 2023-07-17 22:32:31.000000 yams-0.50.0/mypy.ini
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      244 2023-07-17 22:32:31.000000 yams-0.50.0/pyproject.toml
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)       38 2023-07-19 08:48:09.475916 yams-0.50.0/setup.cfg
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     2095 2023-07-17 22:32:31.000000 yams-0.50.0/setup.py
-drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.463916 yams-0.50.0/test/
-drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.463916 yams-0.50.0/test/data/
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      824 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/__init__.py
-drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.463916 yams-0.50.0/test/data/dbmodel/
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      815 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/dbmodel/__init__.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1274 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/dbmodel/blog.py
-drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.463916 yams-0.50.0/test/data/schema/
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     2470 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema/Company.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1135 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema/Dates.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     3252 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema/State.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      978 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema/__init__.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     3610 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema/schema.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)        7 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema/toignore
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1625 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema1.txt
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1489 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema2.txt
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      925 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema_post_build_callback.py
-drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.467916 yams-0.50.0/test/data2/
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      821 2023-07-17 22:32:31.000000 yams-0.50.0/test/data2/__init__.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1067 2023-07-17 22:32:31.000000 yams-0.50.0/test/data2/schema.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    13040 2023-07-17 22:32:31.000000 yams-0.50.0/test/unittest_constraints.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     6356 2023-07-17 22:32:31.000000 yams-0.50.0/test/unittest_diff.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    36195 2023-07-17 22:32:31.000000 yams-0.50.0/test/unittest_reader.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    29219 2023-07-17 22:32:31.000000 yams-0.50.0/test/unittest_schema.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     2742 2023-07-17 22:32:31.000000 yams-0.50.0/test/unittest_schema2dot.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     2313 2023-07-17 22:32:31.000000 yams-0.50.0/test/unittest_serialize.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     9932 2023-07-19 08:36:00.000000 yams-0.50.0/test/unittest_specialization.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     2497 2023-07-17 22:32:31.000000 yams-0.50.0/test/unittest_xy.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     2559 2023-07-17 22:32:31.000000 yams-0.50.0/tox.ini
-drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.467916 yams-0.50.0/yams/
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     7211 2023-07-19 08:36:00.000000 yams-0.50.0/yams/__init__.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     5163 2023-07-19 08:36:00.000000 yams-0.50.0/yams/_exceptions.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    39988 2023-07-19 08:41:42.000000 yams-0.50.0/yams/buildobjs.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    29393 2023-07-19 08:36:00.000000 yams-0.50.0/yams/constraints.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    12344 2023-07-19 08:36:00.000000 yams-0.50.0/yams/diff.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     6181 2023-07-17 22:32:31.000000 yams-0.50.0/yams/interfaces.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-17 22:32:31.000000 yams-0.50.0/yams/py.typed
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    16241 2023-07-19 08:36:00.000000 yams-0.50.0/yams/reader.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    71338 2023-07-19 08:36:00.000000 yams-0.50.0/yams/schema.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    12618 2023-07-17 22:32:31.000000 yams-0.50.0/yams/schema2dot.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1665 2023-07-19 08:36:00.000000 yams-0.50.0/yams/serialize.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     4506 2023-07-19 08:36:00.000000 yams-0.50.0/yams/tools.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     2272 2023-07-17 22:32:31.000000 yams-0.50.0/yams/types.py
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     5851 2023-07-19 08:36:00.000000 yams-0.50.0/yams/xy.py
-drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.471916 yams-0.50.0/yams.egg-info/
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1397 2023-07-19 08:48:09.000000 yams-0.50.0/yams.egg-info/PKG-INFO
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1218 2023-07-19 08:48:09.000000 yams-0.50.0/yams.egg-info/SOURCES.txt
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)        1 2023-07-19 08:48:09.000000 yams-0.50.0/yams.egg-info/dependency_links.txt
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)       49 2023-07-19 08:48:09.000000 yams-0.50.0/yams.egg-info/requires.txt
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)        5 2023-07-19 08:48:09.000000 yams-0.50.0/yams.egg-info/top_level.txt
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    21077 2023-07-17 22:32:31.000000 yams-0.50.0/yams.png
--rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     5326 2023-07-17 22:32:31.000000 yams-0.50.0/yams.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.519949 yams-0.50.1/
+-rw-rw-rw-   0 root         (0) root         (0)    17987 2023-08-03 15:33:19.000000 yams-0.50.1/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)    26527 2023-08-03 15:33:19.000000 yams-0.50.1/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)    13724 2023-08-03 15:33:19.000000 yams-0.50.1/ChangeLog
+-rw-rw-rw-   0 root         (0) root         (0)      469 2023-08-03 15:33:19.000000 yams-0.50.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-08-03 15:34:15.515949 yams-0.50.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      969 2023-08-03 15:33:19.000000 yams-0.50.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2023-08-03 15:33:19.000000 yams-0.50.1/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.219945 yams-0.50.1/bin/
+-rwxrwxrwx   0 root         (0) root         (0)     3838 2023-08-03 15:33:19.000000 yams-0.50.1/bin/owl2yams
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-08-03 15:33:19.000000 yams-0.50.1/bin/yams-check
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-08-03 15:33:19.000000 yams-0.50.1/bin/yams-check.bat
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-08-03 15:33:19.000000 yams-0.50.1/bin/yams-view
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-08-03 15:33:19.000000 yams-0.50.1/bin/yams-view.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.247945 yams-0.50.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-08-03 15:33:19.000000 yams-0.50.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1923 2023-08-03 15:33:19.000000 yams-0.50.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-08-03 15:33:19.000000 yams-0.50.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-08-03 15:33:19.000000 yams-0.50.1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-08-03 15:33:19.000000 yams-0.50.1/docs/yams.rst
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-08-03 15:33:19.000000 yams-0.50.1/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-08-03 15:33:19.000000 yams-0.50.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 15:34:15.519949 yams-0.50.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-08-03 15:33:19.000000 yams-0.50.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.315946 yams-0.50.1/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.323946 yams-0.50.1/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.331946 yams-0.50.1/test/data/dbmodel/
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/dbmodel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/dbmodel/blog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.331946 yams-0.50.1/test/data/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2470 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema/Company.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema/Dates.py
+-rw-rw-rw-   0 root         (0) root         (0)     3252 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema/State.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3610 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema/toignore
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema1.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema2.txt
+-rw-rw-rw-   0 root         (0) root         (0)      925 2023-08-03 15:33:19.000000 yams-0.50.1/test/data/schema_post_build_callback.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.335946 yams-0.50.1/test/data2/
+-rw-rw-rw-   0 root         (0) root         (0)      821 2023-08-03 15:33:19.000000 yams-0.50.1/test/data2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-08-03 15:33:19.000000 yams-0.50.1/test/data2/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    13040 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)     6356 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_diff.py
+-rw-rw-rw-   0 root         (0) root         (0)    36195 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)    29219 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2742 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_schema2dot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     9932 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_specialization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2497 2023-08-03 15:33:19.000000 yams-0.50.1/test/unittest_xy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2559 2023-08-03 15:33:19.000000 yams-0.50.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.471948 yams-0.50.1/yams/
+-rw-rw-rw-   0 root         (0) root         (0)     7211 2023-08-03 15:33:19.000000 yams-0.50.1/yams/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5163 2023-08-03 15:33:19.000000 yams-0.50.1/yams/_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    39988 2023-08-03 15:33:19.000000 yams-0.50.1/yams/buildobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)    29418 2023-08-03 15:33:19.000000 yams-0.50.1/yams/constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)    12344 2023-08-03 15:33:19.000000 yams-0.50.1/yams/diff.py
+-rw-rw-rw-   0 root         (0) root         (0)     6181 2023-08-03 15:33:19.000000 yams-0.50.1/yams/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-03 15:33:19.000000 yams-0.50.1/yams/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    16241 2023-08-03 15:33:19.000000 yams-0.50.1/yams/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)    71338 2023-08-03 15:33:19.000000 yams-0.50.1/yams/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12618 2023-08-03 15:33:19.000000 yams-0.50.1/yams/schema2dot.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2023-08-03 15:33:19.000000 yams-0.50.1/yams/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     4506 2023-08-03 15:33:19.000000 yams-0.50.1/yams/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2023-08-03 15:33:19.000000 yams-0.50.1/yams/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     5851 2023-08-03 15:33:19.000000 yams-0.50.1/yams/xy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:34:15.499949 yams-0.50.1/yams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-08-03 15:34:14.000000 yams-0.50.1/yams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-08-03 15:34:14.000000 yams-0.50.1/yams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 15:34:14.000000 yams-0.50.1/yams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-08-03 15:34:14.000000 yams-0.50.1/yams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-03 15:34:14.000000 yams-0.50.1/yams.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    21077 2023-08-03 15:33:19.000000 yams-0.50.1/yams.png
+-rw-rw-rw-   0 root         (0) root         (0)     5326 2023-08-03 15:33:19.000000 yams-0.50.1/yams.svg
```

### Comparing `yams-0.50.0/COPYING` & `yams-0.50.1/COPYING`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/COPYING.LESSER` & `yams-0.50.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/ChangeLog` & `yams-0.50.1/ChangeLog`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/PKG-INFO` & `yams-0.50.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yams
-Version: 0.50.0
+Version: 0.50.1
 Summary: entity / relation schema
 Home-page: https://forge.extranet.logilab.fr/open-source/yams
 Author: Logilab
 Author-email: devel@logilab.fr
 License: LGPL
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yams-0.50.0/README.rst` & `yams-0.50.1/README.rst`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/__pkginfo__.py` & `yams-0.50.1/__pkginfo__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # pylint: disable-msg=W0622
 
 # package name
 modname = "yams"
 
 # release version
-numversion = (0, 50, 0)
+numversion = (0, 50, 1)
 version = ".".join(str(num) for num in numversion)
 
 # license and copyright
 license = "LGPL"
 
 # short and long description
 description = "entity / relation schema"
@@ -45,14 +45,15 @@
 
 # executable
 scripts = ["bin/yams-check", "bin/yams-view"]
 
 install_requires = [
     "setuptools",
     "logilab-common >= 1.9.0",
+    "typing_extensions >=3.8.0, <5.0.0",
     "python-dateutil",
 ]
 
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `yams-0.50.0/bin/owl2yams` & `yams-0.50.1/bin/owl2yams`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/docs/Makefile` & `yams-0.50.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/docs/conf.py` & `yams-0.50.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/docs/make.bat` & `yams-0.50.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/docs/yams.rst` & `yams-0.50.1/docs/yams.rst`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/setup.py` & `yams-0.50.1/setup.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/data/__init__.py` & `yams-0.50.1/test/data/__init__.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/data/dbmodel/__init__.py` & `yams-0.50.1/test/data/dbmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/data/dbmodel/blog.py` & `yams-0.50.1/test/data/dbmodel/blog.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/data/schema/Company.py` & `yams-0.50.1/test/data/schema/Company.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/data/schema/Dates.py` & `yams-0.50.1/test/data/schema/Dates.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/data/schema/State.py` & `yams-0.50.1/test/data/schema/State.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/data/schema/__init__.py` & `yams-0.50.1/test/data/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/data/schema/schema.py` & `yams-0.50.1/test/data/schema/schema.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/data/schema1.txt` & `yams-0.50.1/test/data/schema1.txt`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/data/schema2.txt` & `yams-0.50.1/test/data/schema2.txt`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/data/schema_post_build_callback.py` & `yams-0.50.1/test/data/schema_post_build_callback.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/data2/__init__.py` & `yams-0.50.1/test/data2/__init__.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/data2/schema.py` & `yams-0.50.1/test/data2/schema.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/unittest_constraints.py` & `yams-0.50.1/test/unittest_constraints.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/unittest_diff.py` & `yams-0.50.1/test/unittest_diff.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/unittest_reader.py` & `yams-0.50.1/test/unittest_reader.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/unittest_schema.py` & `yams-0.50.1/test/unittest_schema.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/unittest_schema2dot.py` & `yams-0.50.1/test/unittest_schema2dot.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/unittest_serialize.py` & `yams-0.50.1/test/unittest_serialize.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/unittest_specialization.py` & `yams-0.50.1/test/unittest_specialization.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/test/unittest_xy.py` & `yams-0.50.1/test/unittest_xy.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/tox.ini` & `yams-0.50.1/tox.ini`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams/__init__.py` & `yams-0.50.1/yams/__init__.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams/_exceptions.py` & `yams-0.50.1/yams/_exceptions.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams/buildobjs.py` & `yams-0.50.1/yams/buildobjs.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams/constraints.py` & `yams-0.50.1/yams/constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,28 +24,28 @@
 import datetime
 from dateutil.parser import parse
 import warnings
 
 from typing import (
     Any,
     Dict,
-    Literal,
     Match,
     Tuple,
     Type,
     Union,
     Optional,
     Callable,
     Sequence,
     List,
     cast,
 )
 
 from logilab.common.deprecation import class_renamed, send_warning
 from logilab.common.date import todate, todatetime
+from typing_extensions import Literal
 
 import yams
 from yams import KEYWORD_MAP, BadSchemaDefinition
 from yams.interfaces import IConstraint, IVocabularyConstraint
 import yams.types as yams_types
 
 __docformat__: str = "restructuredtext en"
```

### Comparing `yams-0.50.0/yams/diff.py` & `yams-0.50.1/yams/diff.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams/interfaces.py` & `yams-0.50.1/yams/interfaces.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams/reader.py` & `yams-0.50.1/yams/reader.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams/schema.py` & `yams-0.50.1/yams/schema.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams/schema2dot.py` & `yams-0.50.1/yams/schema2dot.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams/serialize.py` & `yams-0.50.1/yams/serialize.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams/tools.py` & `yams-0.50.1/yams/tools.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams/types.py` & `yams-0.50.1/yams/types.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams/xy.py` & `yams-0.50.1/yams/xy.py`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams.egg-info/PKG-INFO` & `yams-0.50.1/yams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yams
-Version: 0.50.0
+Version: 0.50.1
 Summary: entity / relation schema
 Home-page: https://forge.extranet.logilab.fr/open-source/yams
 Author: Logilab
 Author-email: devel@logilab.fr
 License: LGPL
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yams-0.50.0/yams.egg-info/SOURCES.txt` & `yams-0.50.1/yams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams.png` & `yams-0.50.1/yams.png`

 * *Files identical despite different names*

### Comparing `yams-0.50.0/yams.svg` & `yams-0.50.1/yams.svg`

 * *Files identical despite different names*

