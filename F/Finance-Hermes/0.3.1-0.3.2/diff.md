# Comparing `tmp/Finance-Hermes-0.3.1.tar.gz` & `tmp/Finance-Hermes-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Hermes-0.3.1.tar", last modified: Mon Jul 31 12:11:45 2023, max compression
+gzip compressed data, was "dist/Finance-Hermes-0.3.2.tar", last modified: Thu Aug  3 13:47:54 2023, max compression
```

## Comparing `Finance-Hermes-0.3.1.tar` & `Finance-Hermes-0.3.2.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/Finance_Hermes.egg-info/
--rw-r--r--   0 root         (0) root         (0)      233 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/Finance_Hermes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      829 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/Finance_Hermes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/Finance_Hermes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/Finance_Hermes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/Finance_Hermes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    11357 2022-11-01 07:48:09.000000 Finance-Hermes-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      358 2023-07-29 01:53:47.000000 Finance-Hermes-0.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      233 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      195 2022-11-06 15:36:04.000000 Finance-Hermes-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/hermes/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-31 12:11:22.000000 Finance-Hermes-0.3.1/hermes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/hermes/factors/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.1/hermes/factors/__init__.py
--rw-r--r--   0 root         (0) root         (0)   360795 2023-07-31 12:08:41.000000 Finance-Hermes-0.3.1/hermes/factors/base.c
--rw-r--r--   0 root         (0) root         (0)     4919 2023-07-31 12:05:26.000000 Finance-Hermes-0.3.1/hermes/factors/base.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/hermes/factors/test/
--rw-r--r--   0 root         (0) root         (0)   241941 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.1/hermes/factors/test/factor_test.c
--rw-r--r--   0 root         (0) root         (0)     2062 2023-07-29 06:11:05.000000 Finance-Hermes-0.3.1/hermes/factors/test/factor_test.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/hermes/kdutils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.1/hermes/kdutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)   271147 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.1/hermes/kdutils/base.c
--rw-r--r--   0 root         (0) root         (0)     2338 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/hermes/kdutils/base.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/hermes/kdutils/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.1/hermes/kdutils/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)   678491 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.1/hermes/kdutils/core/fixes.c
--rw-r--r--   0 root         (0) root         (0)     9714 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/hermes/kdutils/core/fixes.pyx
--rw-r--r--   0 root         (0) root         (0)   392670 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.1/hermes/kdutils/core/helper.c
--rw-r--r--   0 root         (0) root         (0)     7825 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/hermes/kdutils/core/helper.pyx
--rw-r--r--   0 root         (0) root         (0)   190192 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.1/hermes/kdutils/create_id.c
--rw-r--r--   0 root         (0) root         (0)      870 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/hermes/kdutils/create_id.pyx
--rw-r--r--   0 root         (0) root         (0)   235985 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.1/hermes/kdutils/lazy.c
--rw-r--r--   0 root         (0) root         (0)     1578 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/hermes/kdutils/lazy.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/hermes/lzador/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/hermes/lzador/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161732 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.1/hermes/lzador/calculater.c
--rw-r--r--   0 root         (0) root         (0)      657 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/hermes/lzador/calculater.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/requirements/
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/requirements/py3.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3337 2023-07-31 12:08:25.000000 Finance-Hermes-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/Finance_Hermes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      233 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/Finance_Hermes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      942 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/Finance_Hermes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/Finance_Hermes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/Finance_Hermes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/Finance_Hermes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-11-01 07:48:09.000000 Finance-Hermes-0.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      358 2023-07-29 01:53:47.000000 Finance-Hermes-0.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      233 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      195 2022-11-06 15:36:04.000000 Finance-Hermes-0.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/hermes/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-03 13:47:37.000000 Finance-Hermes-0.3.2/hermes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/hermes/factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.2/hermes/factors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   360795 2023-08-03 13:47:53.000000 Finance-Hermes-0.3.2/hermes/factors/base.c
+-rw-r--r--   0 root         (0) root         (0)     4919 2023-08-03 13:45:46.000000 Finance-Hermes-0.3.2/hermes/factors/base.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/hermes/factors/test/
+-rw-r--r--   0 root         (0) root         (0)   245684 2023-08-03 13:47:53.000000 Finance-Hermes-0.3.2/hermes/factors/test/factor_test.c
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-08-03 13:45:46.000000 Finance-Hermes-0.3.2/hermes/factors/test/factor_test.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/hermes/factors/trading/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 13:45:46.000000 Finance-Hermes-0.3.2/hermes/factors/trading/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   554944 2023-08-03 13:47:53.000000 Finance-Hermes-0.3.2/hermes/factors/trading/factor_north.c
+-rw-r--r--   0 root         (0) root         (0)    10129 2023-08-03 13:45:46.000000 Finance-Hermes-0.3.2/hermes/factors/trading/factor_north.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/hermes/kdutils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.2/hermes/kdutils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   271147 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.2/hermes/kdutils/base.c
+-rw-r--r--   0 root         (0) root         (0)     2338 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.2/hermes/kdutils/base.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/hermes/kdutils/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.2/hermes/kdutils/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   678491 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.2/hermes/kdutils/core/fixes.c
+-rw-r--r--   0 root         (0) root         (0)     9714 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.2/hermes/kdutils/core/fixes.pyx
+-rw-r--r--   0 root         (0) root         (0)   392670 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.2/hermes/kdutils/core/helper.c
+-rw-r--r--   0 root         (0) root         (0)     7825 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.2/hermes/kdutils/core/helper.pyx
+-rw-r--r--   0 root         (0) root         (0)   190192 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.2/hermes/kdutils/create_id.c
+-rw-r--r--   0 root         (0) root         (0)      870 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.2/hermes/kdutils/create_id.pyx
+-rw-r--r--   0 root         (0) root         (0)   235985 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.2/hermes/kdutils/lazy.c
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.2/hermes/kdutils/lazy.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/hermes/lzador/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.2/hermes/lzador/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161732 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.2/hermes/lzador/calculater.c
+-rw-r--r--   0 root         (0) root         (0)      657 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.2/hermes/lzador/calculater.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/requirements/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.2/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 13:47:54.000000 Finance-Hermes-0.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3384 2023-08-03 13:47:18.000000 Finance-Hermes-0.3.2/setup.py
```

### Comparing `Finance-Hermes-0.3.1/Finance_Hermes.egg-info/SOURCES.txt` & `Finance-Hermes-0.3.2/Finance_Hermes.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 Finance_Hermes.egg-info/top_level.txt
 hermes/__init__.py
 hermes/factors/__init__.py
 hermes/factors/base.c
 hermes/factors/base.pyx
 hermes/factors/test/factor_test.c
 hermes/factors/test/factor_test.pyx
+hermes/factors/trading/__init__.py
+hermes/factors/trading/factor_north.c
+hermes/factors/trading/factor_north.pyx
 hermes/kdutils/__init__.py
 hermes/kdutils/base.c
 hermes/kdutils/base.pyx
 hermes/kdutils/create_id.c
 hermes/kdutils/create_id.pyx
 hermes/kdutils/lazy.c
 hermes/kdutils/lazy.pyx
```

### Comparing `Finance-Hermes-0.3.1/LICENSE` & `Finance-Hermes-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/hermes/factors/base.c` & `Finance-Hermes-0.3.2/hermes/factors/base.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/hermes/factors/base.pyx` & `Finance-Hermes-0.3.2/hermes/factors/base.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/hermes/factors/test/factor_test.c` & `Finance-Hermes-0.3.2/hermes/factors/test/factor_test.c`

 * *Files 2% similar despite different names*

```diff
@@ -1234,15 +1234,14 @@
 
 /* Module declarations from 'hermes.factors.test.factor_test' */
 #define __Pyx_MODULE_NAME "hermes.factors.test.factor_test"
 extern int __pyx_module_is_main_hermes__factors__test__factor_test;
 int __pyx_module_is_main_hermes__factors__test__factor_test = 0;
 
 /* Implementation of 'hermes.factors.test.factor_test' */
-static const char __pyx_k_[] = "\346\265\213\350\257\225\345\233\240\345\255\220";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_nan[] = "nan";
 static const char __pyx_k_pdb[] = "pdb";
 static const char __pyx_k_str[] = "__str__";
 static const char __pyx_k_data[] = "_data";
 static const char __pyx_k_init[] = "__init__";
@@ -1259,14 +1258,15 @@
 static const char __pyx_k_data_2[] = "data";
 static const char __pyx_k_format[] = "_format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_kwargs[] = "kwargs";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_test_2[] = "__test__";
+static const char __pyx_k_window[] = "window";
 static const char __pyx_k_factor1[] = "factor1";
 static const char __pyx_k_factor2[] = "factor2";
 static const char __pyx_k_factor3[] = "factor3";
 static const char __pyx_k_factor4[] = "factor4";
 static const char __pyx_k_factors[] = "factors";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_category[] = "category";
@@ -1277,14 +1277,16 @@
 static const char __pyx_k_init_self[] = "_init_self";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_openPrice[] = "openPrice";
 static const char __pyx_k_FactorBase[] = "FactorBase";
 static const char __pyx_k_FactorTest[] = "FactorTest";
 static const char __pyx_k_closePrice[] = "closePrice";
 static const char __pyx_k_dy_q_ti_se[] = "dy_q_ti_se";
+static const char __pyx_k_max_window[] = "_max_window";
+static const char __pyx_k_Test_Factor[] = "Test Factor";
 static const char __pyx_k_data_format[] = "data_format";
 static const char __pyx_k_factor_test[] = "factor_test";
 static const char __pyx_k_marketValue[] = "marketValue";
 static const char __pyx_k_turnoverVol[] = "turnoverVol";
 static const char __pyx_k_dependencies[] = "dependencies";
 static const char __pyx_k_LongCallMixin[] = "LongCallMixin";
 static const char __pyx_k_data_format_2[] = "_data_format";
@@ -1297,24 +1299,24 @@
 static const char __pyx_k_FactorTest___init[] = "FactorTest.__init__";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_hermes_factors_base[] = "hermes.factors.base";
 static const char __pyx_k_FactorTest__init_self[] = "FactorTest._init_self";
 static const char __pyx_k_dy_q_evebitda_caldr_se[] = "dy_q_evebitda_caldr_se";
 static const char __pyx_k_hermes_factors_test_factor_test[] = "hermes.factors.test.factor_test";
 static const char __pyx_k_hermes_factors_test_factor_test_2[] = "hermes/factors/test/factor_test.pyx";
-static PyObject *__pyx_kp_s_;
 static PyObject *__pyx_n_s_FactorBase;
 static PyObject *__pyx_n_s_FactorTest;
 static PyObject *__pyx_n_s_FactorTest___init;
 static PyObject *__pyx_n_s_FactorTest__init_self;
 static PyObject *__pyx_n_s_FactorTest_test1;
 static PyObject *__pyx_n_s_FactorTest_test2;
 static PyObject *__pyx_n_s_FactorTest_test3;
 static PyObject *__pyx_n_s_LongCallMixin;
 static PyObject *__pyx_n_s_ShortCallMixin;
+static PyObject *__pyx_kp_s_Test_Factor;
 static PyObject *__pyx_n_s_category;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_closePrice;
 static PyObject *__pyx_n_s_close_se;
 static PyObject *__pyx_n_s_data;
 static PyObject *__pyx_n_s_data_2;
 static PyObject *__pyx_n_s_data_format;
@@ -1338,14 +1340,15 @@
 static PyObject *__pyx_n_s_init;
 static PyObject *__pyx_n_s_init_data;
 static PyObject *__pyx_n_s_init_self;
 static PyObject *__pyx_n_s_isinf;
 static PyObject *__pyx_n_s_kwargs;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_marketValue;
+static PyObject *__pyx_n_s_max_window;
 static PyObject *__pyx_n_s_metaclass;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_n_s_nan;
 static PyObject *__pyx_n_s_negMarketValue;
 static PyObject *__pyx_n_s_np;
@@ -1360,34 +1363,37 @@
 static PyObject *__pyx_n_s_test1;
 static PyObject *__pyx_n_s_test2;
 static PyObject *__pyx_n_s_test3;
 static PyObject *__pyx_n_s_test_2;
 static PyObject *__pyx_n_s_totalshares_se;
 static PyObject *__pyx_n_s_turnoverVol;
 static PyObject *__pyx_n_s_vwap;
+static PyObject *__pyx_n_s_window;
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data_format, PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_2_init_self(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test___defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_4test1(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies); /* proto */
+static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_4test1(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies, CYTHON_UNUSED PyObject *__pyx_v_window); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_2__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_6test2(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies); /* proto */
+static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_6test2(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies, CYTHON_UNUSED PyObject *__pyx_v_window); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_4__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_8test3(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies); /* proto */
+static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_8test3(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies, CYTHON_UNUSED PyObject *__pyx_v_window); /* proto */
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_4;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_codeobj__3;
-static PyObject *__pyx_codeobj__5;
-static PyObject *__pyx_codeobj__7;
-static PyObject *__pyx_codeobj__9;
-static PyObject *__pyx_codeobj__11;
+static PyObject *__pyx_int_10;
+static PyObject *__pyx_int_14;
+static PyObject *__pyx_tuple_;
+static PyObject *__pyx_tuple__3;
+static PyObject *__pyx_tuple__5;
+static PyObject *__pyx_tuple__7;
+static PyObject *__pyx_tuple__9;
+static PyObject *__pyx_codeobj__2;
+static PyObject *__pyx_codeobj__4;
+static PyObject *__pyx_codeobj__6;
+static PyObject *__pyx_codeobj__8;
+static PyObject *__pyx_codeobj__10;
 /* Late includes */
 
 /* "hermes/factors/test/factor_test.pyx":9
  * class FactorTest(FactorBase, LongCallMixin, ShortCallMixin):
  * 
  *     def __init__(self, data_format, **kwargs):             # <<<<<<<<<<<<<<
  *         __str__ = 'factor_test'
@@ -1479,67 +1485,76 @@
   __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "hermes/factors/test/factor_test.pyx":10
  * 
  *     def __init__(self, data_format, **kwargs):
  *         __str__ = 'factor_test'             # <<<<<<<<<<<<<<
  *         self.category = 'test'
- *         self.name = ''
+ *         self.name = 'Test Factor'
  */
   __Pyx_INCREF(__pyx_n_s_factor_test);
   __pyx_v___str__ = __pyx_n_s_factor_test;
 
   /* "hermes/factors/test/factor_test.pyx":11
  *     def __init__(self, data_format, **kwargs):
  *         __str__ = 'factor_test'
  *         self.category = 'test'             # <<<<<<<<<<<<<<
- *         self.name = ''
+ *         self.name = 'Test Factor'
  *         self._data_format = data_format
  */
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_category, __pyx_n_s_test) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
 
   /* "hermes/factors/test/factor_test.pyx":12
  *         __str__ = 'factor_test'
  *         self.category = 'test'
- *         self.name = ''             # <<<<<<<<<<<<<<
+ *         self.name = 'Test Factor'             # <<<<<<<<<<<<<<
  *         self._data_format = data_format
- *         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None
+ *         self._max_window = 10
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_name, __pyx_kp_s_) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_name, __pyx_kp_s_Test_Factor) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
 
   /* "hermes/factors/test/factor_test.pyx":13
  *         self.category = 'test'
- *         self.name = ''
+ *         self.name = 'Test Factor'
  *         self._data_format = data_format             # <<<<<<<<<<<<<<
+ *         self._max_window = 10
  *         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None
- * 
  */
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data_format_2, __pyx_v_data_format) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
 
   /* "hermes/factors/test/factor_test.pyx":14
- *         self.name = ''
+ *         self.name = 'Test Factor'
  *         self._data_format = data_format
+ *         self._max_window = 10             # <<<<<<<<<<<<<<
+ *         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None
+ * 
+ */
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_max_window, __pyx_int_10) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+
+  /* "hermes/factors/test/factor_test.pyx":15
+ *         self._data_format = data_format
+ *         self._max_window = 10
  *         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None             # <<<<<<<<<<<<<<
  * 
  *     def _init_self(self, **kwargs):
  */
-  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_end_date, __pyx_v_kwargs, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_end_date, __pyx_v_kwargs, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 15, __pyx_L1_error)
   if ((__pyx_t_2 != 0)) {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_1 = __pyx_t_4;
     __pyx_t_4 = 0;
   } else {
     __Pyx_INCREF(Py_None);
     __pyx_t_1 = Py_None;
   }
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_1) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "hermes/factors/test/factor_test.pyx":9
  * class FactorTest(FactorBase, LongCallMixin, ShortCallMixin):
  * 
  *     def __init__(self, data_format, **kwargs):             # <<<<<<<<<<<<<<
  *         __str__ = 'factor_test'
@@ -1558,15 +1573,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___str__);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/test/factor_test.pyx":16
+/* "hermes/factors/test/factor_test.pyx":17
  *         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None
  * 
  *     def _init_self(self, **kwargs):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
 
@@ -1600,26 +1615,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_init_self") < 0)) __PYX_ERR(0, 16, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_init_self") < 0)) __PYX_ERR(0, 17, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_init_self", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 16, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_init_self", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 17, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("hermes.factors.test.factor_test.FactorTest._init_self", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_2_init_self(__pyx_self, __pyx_v_self, __pyx_v_kwargs);
@@ -1638,41 +1653,44 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/test/factor_test.pyx":19
+/* "hermes/factors/test/factor_test.pyx":20
  *         pass
  * 
- *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap']):             # <<<<<<<<<<<<<<
+ *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap'], window=0):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         close_se = data['openPrice']
  */
 
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test___defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)Py_None));
   __Pyx_GIVEREF(((PyObject *)Py_None));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_None));
   __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_dependencies);
   __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_dependencies);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_dependencies);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_INCREF(((PyObject *)__pyx_int_0));
+  __Pyx_GIVEREF(((PyObject *)__pyx_int_0));
+  PyTuple_SET_ITEM(__pyx_t_1, 2, ((PyObject *)__pyx_int_0));
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None);
   __pyx_t_1 = 0;
@@ -1690,36 +1708,40 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6hermes_7factors_4test_11factor_test_10FactorTest_5test1(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6hermes_7factors_4test_11factor_test_10FactorTest_4test1[] = "FactorTest.test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap'])";
+static char __pyx_doc_6hermes_7factors_4test_11factor_test_10FactorTest_4test1[] = "FactorTest.test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap'], window=0)";
 static PyMethodDef __pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_5test1 = {"test1", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6hermes_7factors_4test_11factor_test_10FactorTest_5test1, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6hermes_7factors_4test_11factor_test_10FactorTest_4test1};
 static PyObject *__pyx_pw_6hermes_7factors_4test_11factor_test_10FactorTest_5test1(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_data = 0;
   CYTHON_UNUSED PyObject *__pyx_v_dependencies = 0;
+  CYTHON_UNUSED PyObject *__pyx_v_window = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("test1 (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_data_2,&__pyx_n_s_dependencies,0};
-    PyObject* values[3] = {0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_data_2,&__pyx_n_s_dependencies,&__pyx_n_s_window,0};
+    PyObject* values[4] = {0,0,0,0};
     __pyx_defaults *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self);
     values[1] = ((PyObject *)((PyObject *)Py_None));
     values[2] = __pyx_dynamic_args->__pyx_arg_dependencies;
+    values[3] = ((PyObject *)((PyObject *)__pyx_int_0));
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
@@ -1738,49 +1760,58 @@
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dependencies);
           if (value) { values[2] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_window);
+          if (value) { values[3] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "test1") < 0)) __PYX_ERR(0, 19, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "test1") < 0)) __PYX_ERR(0, 20, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_self = values[0];
     __pyx_v_data = values[1];
     __pyx_v_dependencies = values[2];
+    __pyx_v_window = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("test1", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 19, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("test1", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 20, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("hermes.factors.test.factor_test.FactorTest.test1", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_4test1(__pyx_self, __pyx_v_self, __pyx_v_data, __pyx_v_dependencies);
+  __pyx_r = __pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_4test1(__pyx_self, __pyx_v_self, __pyx_v_data, __pyx_v_dependencies, __pyx_v_window);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_4test1(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies) {
+static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_4test1(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies, CYTHON_UNUSED PyObject *__pyx_v_window) {
   PyObject *__pyx_v_close_se = NULL;
   PyObject *__pyx_v_dy_q_ti_se = NULL;
   PyObject *__pyx_v_totalshares_se = NULL;
   PyObject *__pyx_v_dy_q_evebitda_caldr_se = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -1792,162 +1823,162 @@
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("test1", 0);
   __Pyx_INCREF(__pyx_v_data);
 
-  /* "hermes/factors/test/factor_test.pyx":20
+  /* "hermes/factors/test/factor_test.pyx":21
  * 
- *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap']):
+ *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap'], window=0):
  *         data = self._data if data is None else data             # <<<<<<<<<<<<<<
  *         close_se = data['openPrice']
  *         dy_q_ti_se = data['closePrice']
  */
   __pyx_t_2 = (__pyx_v_data == Py_None);
   if ((__pyx_t_2 != 0)) {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
     __Pyx_INCREF(__pyx_v_data);
     __pyx_t_1 = __pyx_v_data;
   }
   __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":21
- *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap']):
+  /* "hermes/factors/test/factor_test.pyx":22
+ *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap'], window=0):
  *         data = self._data if data is None else data
  *         close_se = data['openPrice']             # <<<<<<<<<<<<<<
  *         dy_q_ti_se = data['closePrice']
  *         totalshares_se = data['vwap']
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_openPrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_openPrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_close_se = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":22
+  /* "hermes/factors/test/factor_test.pyx":23
  *         data = self._data if data is None else data
  *         close_se = data['openPrice']
  *         dy_q_ti_se = data['closePrice']             # <<<<<<<<<<<<<<
  *         totalshares_se = data['vwap']
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_closePrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_closePrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_dy_q_ti_se = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":23
+  /* "hermes/factors/test/factor_test.pyx":24
  *         close_se = data['openPrice']
  *         dy_q_ti_se = data['closePrice']
  *         totalshares_se = data['vwap']             # <<<<<<<<<<<<<<
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_vwap); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_vwap); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_totalshares_se = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":24
+  /* "hermes/factors/test/factor_test.pyx":25
  *         dy_q_ti_se = data['closePrice']
  *         totalshares_se = data['vwap']
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)             # <<<<<<<<<<<<<<
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
  */
-  __pyx_t_1 = PyNumber_Multiply(__pyx_int_4, __pyx_v_dy_q_ti_se); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Multiply(__pyx_int_4, __pyx_v_dy_q_ti_se); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_v_totalshares_se); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_v_totalshares_se); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_v_close_se, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_v_close_se, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_dy_q_evebitda_caldr_se = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":26
+  /* "hermes/factors/test/factor_test.pyx":27
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan             # <<<<<<<<<<<<<<
  *         return self._format(dy_q_evebitda_caldr_se, "test1")
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_nan); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_nan); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":25
+  /* "hermes/factors/test/factor_test.pyx":26
  *         totalshares_se = data['vwap']
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |             # <<<<<<<<<<<<<<
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
  *         return self._format(dy_q_evebitda_caldr_se, "test1")
  */
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_dy_q_evebitda_caldr_se, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_dy_q_evebitda_caldr_se, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
 
-  /* "hermes/factors/test/factor_test.pyx":26
+  /* "hermes/factors/test/factor_test.pyx":27
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan             # <<<<<<<<<<<<<<
  *         return self._format(dy_q_evebitda_caldr_se, "test1")
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_isinf); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_isinf); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_v_dy_q_evebitda_caldr_se) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_dy_q_evebitda_caldr_se);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":25
+  /* "hermes/factors/test/factor_test.pyx":26
  *         totalshares_se = data['vwap']
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |             # <<<<<<<<<<<<<<
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
  *         return self._format(dy_q_evebitda_caldr_se, "test1")
  */
-  __pyx_t_6 = PyNumber_Or(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_Or(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_dy_q_evebitda_caldr_se, __pyx_t_6, __pyx_t_3) < 0)) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_dy_q_evebitda_caldr_se, __pyx_t_6, __pyx_t_3) < 0)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":27
+  /* "hermes/factors/test/factor_test.pyx":28
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
  *         return self._format(dy_q_evebitda_caldr_se, "test1")             # <<<<<<<<<<<<<<
  * 
- *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
+ *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue'], window=10):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -1956,52 +1987,52 @@
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_dy_q_evebitda_caldr_se, __pyx_n_s_test1};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_dy_q_evebitda_caldr_se, __pyx_n_s_test1};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   {
-    __pyx_t_1 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_dy_q_evebitda_caldr_se);
     __Pyx_GIVEREF(__pyx_v_dy_q_evebitda_caldr_se);
     PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_7, __pyx_v_dy_q_evebitda_caldr_se);
     __Pyx_INCREF(__pyx_n_s_test1);
     __Pyx_GIVEREF(__pyx_n_s_test1);
     PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_7, __pyx_n_s_test1);
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/test/factor_test.pyx":19
+  /* "hermes/factors/test/factor_test.pyx":20
  *         pass
  * 
- *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap']):             # <<<<<<<<<<<<<<
+ *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap'], window=0):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         close_se = data['openPrice']
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -2018,41 +2049,44 @@
   __Pyx_XDECREF(__pyx_v_dy_q_evebitda_caldr_se);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/test/factor_test.pyx":29
+/* "hermes/factors/test/factor_test.pyx":30
  *         return self._format(dy_q_evebitda_caldr_se, "test1")
  * 
- *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):             # <<<<<<<<<<<<<<
+ *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue'], window=10):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         close_se = data['marketValue']
  */
 
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_2__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)Py_None));
   __Pyx_GIVEREF(((PyObject *)Py_None));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_None));
   __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_dependencies);
   __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_dependencies);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_dependencies);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __Pyx_INCREF(((PyObject *)__pyx_int_10));
+  __Pyx_GIVEREF(((PyObject *)__pyx_int_10));
+  PyTuple_SET_ITEM(__pyx_t_1, 2, ((PyObject *)__pyx_int_10));
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None);
   __pyx_t_1 = 0;
@@ -2070,36 +2104,40 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6hermes_7factors_4test_11factor_test_10FactorTest_7test2(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6hermes_7factors_4test_11factor_test_10FactorTest_6test2[] = "FactorTest.test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue'])";
+static char __pyx_doc_6hermes_7factors_4test_11factor_test_10FactorTest_6test2[] = "FactorTest.test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue'], window=10)";
 static PyMethodDef __pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_7test2 = {"test2", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6hermes_7factors_4test_11factor_test_10FactorTest_7test2, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6hermes_7factors_4test_11factor_test_10FactorTest_6test2};
 static PyObject *__pyx_pw_6hermes_7factors_4test_11factor_test_10FactorTest_7test2(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_data = 0;
   CYTHON_UNUSED PyObject *__pyx_v_dependencies = 0;
+  CYTHON_UNUSED PyObject *__pyx_v_window = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("test2 (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_data_2,&__pyx_n_s_dependencies,0};
-    PyObject* values[3] = {0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_data_2,&__pyx_n_s_dependencies,&__pyx_n_s_window,0};
+    PyObject* values[4] = {0,0,0,0};
     __pyx_defaults1 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self);
     values[1] = ((PyObject *)((PyObject *)Py_None));
     values[2] = __pyx_dynamic_args->__pyx_arg_dependencies;
+    values[3] = ((PyObject *)((PyObject *)__pyx_int_10));
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
@@ -2118,49 +2156,58 @@
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dependencies);
           if (value) { values[2] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_window);
+          if (value) { values[3] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "test2") < 0)) __PYX_ERR(0, 29, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "test2") < 0)) __PYX_ERR(0, 30, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_self = values[0];
     __pyx_v_data = values[1];
     __pyx_v_dependencies = values[2];
+    __pyx_v_window = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("test2", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 29, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("test2", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 30, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("hermes.factors.test.factor_test.FactorTest.test2", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_6test2(__pyx_self, __pyx_v_self, __pyx_v_data, __pyx_v_dependencies);
+  __pyx_r = __pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_6test2(__pyx_self, __pyx_v_self, __pyx_v_data, __pyx_v_dependencies, __pyx_v_window);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_6test2(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies) {
+static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_6test2(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies, CYTHON_UNUSED PyObject *__pyx_v_window) {
   PyObject *__pyx_v_close_se = NULL;
   PyObject *__pyx_v_dy_q_ti_se = NULL;
   PyObject *__pyx_v_totalshares_se = NULL;
   PyObject *__pyx_v_dy_q_evebitda_caldr_se = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -2172,162 +2219,162 @@
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("test2", 0);
   __Pyx_INCREF(__pyx_v_data);
 
-  /* "hermes/factors/test/factor_test.pyx":30
+  /* "hermes/factors/test/factor_test.pyx":31
  * 
- *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
+ *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue'], window=10):
  *         data = self._data if data is None else data             # <<<<<<<<<<<<<<
  *         close_se = data['marketValue']
  *         dy_q_ti_se = data['turnoverVol']
  */
   __pyx_t_2 = (__pyx_v_data == Py_None);
   if ((__pyx_t_2 != 0)) {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 31, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
     __Pyx_INCREF(__pyx_v_data);
     __pyx_t_1 = __pyx_v_data;
   }
   __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":31
- *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
+  /* "hermes/factors/test/factor_test.pyx":32
+ *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue'], window=10):
  *         data = self._data if data is None else data
  *         close_se = data['marketValue']             # <<<<<<<<<<<<<<
  *         dy_q_ti_se = data['turnoverVol']
  *         totalshares_se = data['negMarketValue']
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_marketValue); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_marketValue); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_close_se = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":32
+  /* "hermes/factors/test/factor_test.pyx":33
  *         data = self._data if data is None else data
  *         close_se = data['marketValue']
  *         dy_q_ti_se = data['turnoverVol']             # <<<<<<<<<<<<<<
  *         totalshares_se = data['negMarketValue']
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_turnoverVol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_turnoverVol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_dy_q_ti_se = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":33
+  /* "hermes/factors/test/factor_test.pyx":34
  *         close_se = data['marketValue']
  *         dy_q_ti_se = data['turnoverVol']
  *         totalshares_se = data['negMarketValue']             # <<<<<<<<<<<<<<
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_negMarketValue); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_negMarketValue); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_totalshares_se = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":34
+  /* "hermes/factors/test/factor_test.pyx":35
  *         dy_q_ti_se = data['turnoverVol']
  *         totalshares_se = data['negMarketValue']
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)             # <<<<<<<<<<<<<<
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
  */
-  __pyx_t_1 = PyNumber_Multiply(__pyx_int_4, __pyx_v_dy_q_ti_se); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Multiply(__pyx_int_4, __pyx_v_dy_q_ti_se); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_v_totalshares_se); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_v_totalshares_se); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_v_close_se, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_v_close_se, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_dy_q_evebitda_caldr_se = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":36
+  /* "hermes/factors/test/factor_test.pyx":37
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan             # <<<<<<<<<<<<<<
  *         return self._format(dy_q_evebitda_caldr_se, "test2")
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_nan); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_nan); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":35
+  /* "hermes/factors/test/factor_test.pyx":36
  *         totalshares_se = data['negMarketValue']
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |             # <<<<<<<<<<<<<<
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
  *         return self._format(dy_q_evebitda_caldr_se, "test2")
  */
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_dy_q_evebitda_caldr_se, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_dy_q_evebitda_caldr_se, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
 
-  /* "hermes/factors/test/factor_test.pyx":36
+  /* "hermes/factors/test/factor_test.pyx":37
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan             # <<<<<<<<<<<<<<
  *         return self._format(dy_q_evebitda_caldr_se, "test2")
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_isinf); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_isinf); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_v_dy_q_evebitda_caldr_se) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_dy_q_evebitda_caldr_se);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 36, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":35
+  /* "hermes/factors/test/factor_test.pyx":36
  *         totalshares_se = data['negMarketValue']
  *         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |             # <<<<<<<<<<<<<<
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
  *         return self._format(dy_q_evebitda_caldr_se, "test2")
  */
-  __pyx_t_6 = PyNumber_Or(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_Or(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_dy_q_evebitda_caldr_se, __pyx_t_6, __pyx_t_3) < 0)) __PYX_ERR(0, 35, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_dy_q_evebitda_caldr_se, __pyx_t_6, __pyx_t_3) < 0)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":37
+  /* "hermes/factors/test/factor_test.pyx":38
  *         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
  *                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
  *         return self._format(dy_q_evebitda_caldr_se, "test2")             # <<<<<<<<<<<<<<
  * 
- *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):
+ *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice'], window=14):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -2336,52 +2383,52 @@
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_dy_q_evebitda_caldr_se, __pyx_n_s_test2};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_dy_q_evebitda_caldr_se, __pyx_n_s_test2};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   {
-    __pyx_t_1 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_dy_q_evebitda_caldr_se);
     __Pyx_GIVEREF(__pyx_v_dy_q_evebitda_caldr_se);
     PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_7, __pyx_v_dy_q_evebitda_caldr_se);
     __Pyx_INCREF(__pyx_n_s_test2);
     __Pyx_GIVEREF(__pyx_n_s_test2);
     PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_7, __pyx_n_s_test2);
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/test/factor_test.pyx":29
+  /* "hermes/factors/test/factor_test.pyx":30
  *         return self._format(dy_q_evebitda_caldr_se, "test1")
  * 
- *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):             # <<<<<<<<<<<<<<
+ *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue'], window=10):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         close_se = data['marketValue']
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -2398,41 +2445,44 @@
   __Pyx_XDECREF(__pyx_v_dy_q_evebitda_caldr_se);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/test/factor_test.pyx":39
+/* "hermes/factors/test/factor_test.pyx":40
  *         return self._format(dy_q_evebitda_caldr_se, "test2")
  * 
- *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):             # <<<<<<<<<<<<<<
+ *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice'], window=14):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         turnoverVol = data['turnoverVol']
  */
 
 static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_4__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)Py_None));
   __Pyx_GIVEREF(((PyObject *)Py_None));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_None));
   __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self)->__pyx_arg_dependencies);
   __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self)->__pyx_arg_dependencies);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self)->__pyx_arg_dependencies);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_INCREF(((PyObject *)__pyx_int_14));
+  __Pyx_GIVEREF(((PyObject *)__pyx_int_14));
+  PyTuple_SET_ITEM(__pyx_t_1, 2, ((PyObject *)__pyx_int_14));
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None);
   __pyx_t_1 = 0;
@@ -2450,36 +2500,40 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6hermes_7factors_4test_11factor_test_10FactorTest_9test3(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6hermes_7factors_4test_11factor_test_10FactorTest_8test3[] = "FactorTest.test3(self, data=None, dependencies=['turnoverVol', 'closePrice'])";
+static char __pyx_doc_6hermes_7factors_4test_11factor_test_10FactorTest_8test3[] = "FactorTest.test3(self, data=None, dependencies=['turnoverVol', 'closePrice'], window=14)";
 static PyMethodDef __pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_9test3 = {"test3", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6hermes_7factors_4test_11factor_test_10FactorTest_9test3, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6hermes_7factors_4test_11factor_test_10FactorTest_8test3};
 static PyObject *__pyx_pw_6hermes_7factors_4test_11factor_test_10FactorTest_9test3(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_data = 0;
   CYTHON_UNUSED PyObject *__pyx_v_dependencies = 0;
+  CYTHON_UNUSED PyObject *__pyx_v_window = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("test3 (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_data_2,&__pyx_n_s_dependencies,0};
-    PyObject* values[3] = {0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_data_2,&__pyx_n_s_dependencies,&__pyx_n_s_window,0};
+    PyObject* values[4] = {0,0,0,0};
     __pyx_defaults2 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self);
     values[1] = ((PyObject *)((PyObject *)Py_None));
     values[2] = __pyx_dynamic_args->__pyx_arg_dependencies;
+    values[3] = ((PyObject *)((PyObject *)__pyx_int_14));
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
@@ -2498,49 +2552,58 @@
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dependencies);
           if (value) { values[2] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_window);
+          if (value) { values[3] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "test3") < 0)) __PYX_ERR(0, 39, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "test3") < 0)) __PYX_ERR(0, 40, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_self = values[0];
     __pyx_v_data = values[1];
     __pyx_v_dependencies = values[2];
+    __pyx_v_window = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("test3", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 39, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("test3", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 40, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("hermes.factors.test.factor_test.FactorTest.test3", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_8test3(__pyx_self, __pyx_v_self, __pyx_v_data, __pyx_v_dependencies);
+  __pyx_r = __pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_8test3(__pyx_self, __pyx_v_self, __pyx_v_data, __pyx_v_dependencies, __pyx_v_window);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_8test3(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies) {
+static PyObject *__pyx_pf_6hermes_7factors_4test_11factor_test_10FactorTest_8test3(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_dependencies, CYTHON_UNUSED PyObject *__pyx_v_window) {
   PyObject *__pyx_v_turnoverVol = NULL;
   PyObject *__pyx_v_closePrice = NULL;
   PyObject *__pyx_v_factor1 = NULL;
   PyObject *__pyx_v_factor2 = NULL;
   PyObject *__pyx_v_factors = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -2553,92 +2616,92 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("test3", 0);
   __Pyx_INCREF(__pyx_v_data);
 
-  /* "hermes/factors/test/factor_test.pyx":40
+  /* "hermes/factors/test/factor_test.pyx":41
  * 
- *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):
+ *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice'], window=14):
  *         data = self._data if data is None else data             # <<<<<<<<<<<<<<
  *         turnoverVol = data['turnoverVol']
  *         closePrice = data['closePrice']
  */
   __pyx_t_2 = (__pyx_v_data == Py_None);
   if ((__pyx_t_2 != 0)) {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 41, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
     __Pyx_INCREF(__pyx_v_data);
     __pyx_t_1 = __pyx_v_data;
   }
   __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":41
- *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):
+  /* "hermes/factors/test/factor_test.pyx":42
+ *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice'], window=14):
  *         data = self._data if data is None else data
  *         turnoverVol = data['turnoverVol']             # <<<<<<<<<<<<<<
  *         closePrice = data['closePrice']
  *         factor1 = turnoverVol * closePrice
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_turnoverVol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_turnoverVol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_turnoverVol = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":42
+  /* "hermes/factors/test/factor_test.pyx":43
  *         data = self._data if data is None else data
  *         turnoverVol = data['turnoverVol']
  *         closePrice = data['closePrice']             # <<<<<<<<<<<<<<
  *         factor1 = turnoverVol * closePrice
  *         factor2 = turnoverVol + closePrice
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_closePrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_s_closePrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_closePrice = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":43
+  /* "hermes/factors/test/factor_test.pyx":44
  *         turnoverVol = data['turnoverVol']
  *         closePrice = data['closePrice']
  *         factor1 = turnoverVol * closePrice             # <<<<<<<<<<<<<<
  *         factor2 = turnoverVol + closePrice
  *         factors = {
  */
-  __pyx_t_1 = PyNumber_Multiply(__pyx_v_turnoverVol, __pyx_v_closePrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Multiply(__pyx_v_turnoverVol, __pyx_v_closePrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_factor1 = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":44
+  /* "hermes/factors/test/factor_test.pyx":45
  *         closePrice = data['closePrice']
  *         factor1 = turnoverVol * closePrice
  *         factor2 = turnoverVol + closePrice             # <<<<<<<<<<<<<<
  *         factors = {
  *             'factor3': self._format(factor1, "factor3"),
  */
-  __pyx_t_1 = PyNumber_Add(__pyx_v_turnoverVol, __pyx_v_closePrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_v_turnoverVol, __pyx_v_closePrice); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_factor2 = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":46
+  /* "hermes/factors/test/factor_test.pyx":47
  *         factor2 = turnoverVol + closePrice
  *         factors = {
  *             'factor3': self._format(factor1, "factor3"),             # <<<<<<<<<<<<<<
  *             'factor4': self._format(factor2, "factor4")
  *         }
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -2647,55 +2710,55 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_factor1, __pyx_n_s_factor3};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_factor1, __pyx_n_s_factor3};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 46, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_INCREF(__pyx_v_factor1);
     __Pyx_GIVEREF(__pyx_v_factor1);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_factor1);
     __Pyx_INCREF(__pyx_n_s_factor3);
     __Pyx_GIVEREF(__pyx_n_s_factor3);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_n_s_factor3);
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_factor3, __pyx_t_3) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_factor3, __pyx_t_3) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":47
+  /* "hermes/factors/test/factor_test.pyx":48
  *         factors = {
  *             'factor3': self._format(factor1, "factor3"),
  *             'factor4': self._format(factor2, "factor4")             # <<<<<<<<<<<<<<
  *         }
  *         return factors
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_7 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -2704,63 +2767,63 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_v_factor2, __pyx_n_s_factor4};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_v_factor2, __pyx_n_s_factor4};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_INCREF(__pyx_v_factor2);
     __Pyx_GIVEREF(__pyx_v_factor2);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_6, __pyx_v_factor2);
     __Pyx_INCREF(__pyx_n_s_factor4);
     __Pyx_GIVEREF(__pyx_n_s_factor4);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_6, __pyx_n_s_factor4);
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_factor4, __pyx_t_3) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_factor4, __pyx_t_3) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_factors = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":49
+  /* "hermes/factors/test/factor_test.pyx":50
  *             'factor4': self._format(factor2, "factor4")
  *         }
  *         return factors             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_factors);
   __pyx_r = __pyx_v_factors;
   goto __pyx_L0;
 
-  /* "hermes/factors/test/factor_test.pyx":39
+  /* "hermes/factors/test/factor_test.pyx":40
  *         return self._format(dy_q_evebitda_caldr_se, "test2")
  * 
- *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):             # <<<<<<<<<<<<<<
+ *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice'], window=14):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         turnoverVol = data['turnoverVol']
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -2824,24 +2887,24 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_s_, __pyx_k_, sizeof(__pyx_k_), 0, 0, 1, 0},
   {&__pyx_n_s_FactorBase, __pyx_k_FactorBase, sizeof(__pyx_k_FactorBase), 0, 0, 1, 1},
   {&__pyx_n_s_FactorTest, __pyx_k_FactorTest, sizeof(__pyx_k_FactorTest), 0, 0, 1, 1},
   {&__pyx_n_s_FactorTest___init, __pyx_k_FactorTest___init, sizeof(__pyx_k_FactorTest___init), 0, 0, 1, 1},
   {&__pyx_n_s_FactorTest__init_self, __pyx_k_FactorTest__init_self, sizeof(__pyx_k_FactorTest__init_self), 0, 0, 1, 1},
   {&__pyx_n_s_FactorTest_test1, __pyx_k_FactorTest_test1, sizeof(__pyx_k_FactorTest_test1), 0, 0, 1, 1},
   {&__pyx_n_s_FactorTest_test2, __pyx_k_FactorTest_test2, sizeof(__pyx_k_FactorTest_test2), 0, 0, 1, 1},
   {&__pyx_n_s_FactorTest_test3, __pyx_k_FactorTest_test3, sizeof(__pyx_k_FactorTest_test3), 0, 0, 1, 1},
   {&__pyx_n_s_LongCallMixin, __pyx_k_LongCallMixin, sizeof(__pyx_k_LongCallMixin), 0, 0, 1, 1},
   {&__pyx_n_s_ShortCallMixin, __pyx_k_ShortCallMixin, sizeof(__pyx_k_ShortCallMixin), 0, 0, 1, 1},
+  {&__pyx_kp_s_Test_Factor, __pyx_k_Test_Factor, sizeof(__pyx_k_Test_Factor), 0, 0, 1, 0},
   {&__pyx_n_s_category, __pyx_k_category, sizeof(__pyx_k_category), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_closePrice, __pyx_k_closePrice, sizeof(__pyx_k_closePrice), 0, 0, 1, 1},
   {&__pyx_n_s_close_se, __pyx_k_close_se, sizeof(__pyx_k_close_se), 0, 0, 1, 1},
   {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
   {&__pyx_n_s_data_2, __pyx_k_data_2, sizeof(__pyx_k_data_2), 0, 0, 1, 1},
   {&__pyx_n_s_data_format, __pyx_k_data_format, sizeof(__pyx_k_data_format), 0, 0, 1, 1},
@@ -2865,14 +2928,15 @@
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
   {&__pyx_n_s_init_data, __pyx_k_init_data, sizeof(__pyx_k_init_data), 0, 0, 1, 1},
   {&__pyx_n_s_init_self, __pyx_k_init_self, sizeof(__pyx_k_init_self), 0, 0, 1, 1},
   {&__pyx_n_s_isinf, __pyx_k_isinf, sizeof(__pyx_k_isinf), 0, 0, 1, 1},
   {&__pyx_n_s_kwargs, __pyx_k_kwargs, sizeof(__pyx_k_kwargs), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_marketValue, __pyx_k_marketValue, sizeof(__pyx_k_marketValue), 0, 0, 1, 1},
+  {&__pyx_n_s_max_window, __pyx_k_max_window, sizeof(__pyx_k_max_window), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_n_s_nan, __pyx_k_nan, sizeof(__pyx_k_nan), 0, 0, 1, 1},
   {&__pyx_n_s_negMarketValue, __pyx_k_negMarketValue, sizeof(__pyx_k_negMarketValue), 0, 0, 1, 1},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
@@ -2887,14 +2951,15 @@
   {&__pyx_n_s_test1, __pyx_k_test1, sizeof(__pyx_k_test1), 0, 0, 1, 1},
   {&__pyx_n_s_test2, __pyx_k_test2, sizeof(__pyx_k_test2), 0, 0, 1, 1},
   {&__pyx_n_s_test3, __pyx_k_test3, sizeof(__pyx_k_test3), 0, 0, 1, 1},
   {&__pyx_n_s_test_2, __pyx_k_test_2, sizeof(__pyx_k_test_2), 0, 0, 1, 1},
   {&__pyx_n_s_totalshares_se, __pyx_k_totalshares_se, sizeof(__pyx_k_totalshares_se), 0, 0, 1, 1},
   {&__pyx_n_s_turnoverVol, __pyx_k_turnoverVol, sizeof(__pyx_k_turnoverVol), 0, 0, 1, 1},
   {&__pyx_n_s_vwap, __pyx_k_vwap, sizeof(__pyx_k_vwap), 0, 0, 1, 1},
+  {&__pyx_n_s_window, __pyx_k_window, sizeof(__pyx_k_window), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   return 0;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -2904,77 +2969,79 @@
   /* "hermes/factors/test/factor_test.pyx":9
  * class FactorTest(FactorBase, LongCallMixin, ShortCallMixin):
  * 
  *     def __init__(self, data_format, **kwargs):             # <<<<<<<<<<<<<<
  *         __str__ = 'factor_test'
  *         self.category = 'test'
  */
-  __pyx_tuple__2 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_data_format, __pyx_n_s_kwargs, __pyx_n_s_str); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 9, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_init, 9, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_data_format, __pyx_n_s_kwargs, __pyx_n_s_str); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_init, 9, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 9, __pyx_L1_error)
 
-  /* "hermes/factors/test/factor_test.pyx":16
+  /* "hermes/factors/test/factor_test.pyx":17
  *         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None
  * 
  *     def _init_self(self, **kwargs):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_init_self, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_init_self, 17, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 17, __pyx_L1_error)
 
-  /* "hermes/factors/test/factor_test.pyx":19
+  /* "hermes/factors/test/factor_test.pyx":20
  *         pass
  * 
- *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap']):             # <<<<<<<<<<<<<<
+ *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap'], window=0):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         close_se = data['openPrice']
  */
-  __pyx_tuple__6 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_data_2, __pyx_n_s_dependencies, __pyx_n_s_close_se, __pyx_n_s_dy_q_ti_se, __pyx_n_s_totalshares_se, __pyx_n_s_dy_q_evebitda_caldr_se); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_test1, 19, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_data_2, __pyx_n_s_dependencies, __pyx_n_s_window, __pyx_n_s_close_se, __pyx_n_s_dy_q_ti_se, __pyx_n_s_totalshares_se, __pyx_n_s_dy_q_evebitda_caldr_se); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(4, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_test1, 20, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 20, __pyx_L1_error)
 
-  /* "hermes/factors/test/factor_test.pyx":29
+  /* "hermes/factors/test/factor_test.pyx":30
  *         return self._format(dy_q_evebitda_caldr_se, "test1")
  * 
- *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):             # <<<<<<<<<<<<<<
+ *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue'], window=10):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         close_se = data['marketValue']
  */
-  __pyx_tuple__8 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_data_2, __pyx_n_s_dependencies, __pyx_n_s_close_se, __pyx_n_s_dy_q_ti_se, __pyx_n_s_totalshares_se, __pyx_n_s_dy_q_evebitda_caldr_se); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 29, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_test2, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_data_2, __pyx_n_s_dependencies, __pyx_n_s_window, __pyx_n_s_close_se, __pyx_n_s_dy_q_ti_se, __pyx_n_s_totalshares_se, __pyx_n_s_dy_q_evebitda_caldr_se); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(4, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_test2, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 30, __pyx_L1_error)
 
-  /* "hermes/factors/test/factor_test.pyx":39
+  /* "hermes/factors/test/factor_test.pyx":40
  *         return self._format(dy_q_evebitda_caldr_se, "test2")
  * 
- *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):             # <<<<<<<<<<<<<<
+ *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice'], window=14):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         turnoverVol = data['turnoverVol']
  */
-  __pyx_tuple__10 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_data_2, __pyx_n_s_dependencies, __pyx_n_s_turnoverVol, __pyx_n_s_closePrice, __pyx_n_s_factor1, __pyx_n_s_factor2, __pyx_n_s_factors); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 39, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_test3, 39, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_data_2, __pyx_n_s_dependencies, __pyx_n_s_window, __pyx_n_s_turnoverVol, __pyx_n_s_closePrice, __pyx_n_s_factor1, __pyx_n_s_factor2, __pyx_n_s_factors); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(4, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_test_factor_test_2, __pyx_n_s_test3, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_10 = PyInt_FromLong(10); if (unlikely(!__pyx_int_10)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_14 = PyInt_FromLong(14); if (unlikely(!__pyx_int_14)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -3336,110 +3403,110 @@
   /* "hermes/factors/test/factor_test.pyx":9
  * class FactorTest(FactorBase, LongCallMixin, ShortCallMixin):
  * 
  *     def __init__(self, data_format, **kwargs):             # <<<<<<<<<<<<<<
  *         __str__ = 'factor_test'
  *         self.category = 'test'
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_1__init__, 0, __pyx_n_s_FactorTest___init, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_1__init__, 0, __pyx_n_s_FactorTest___init, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_2) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":16
+  /* "hermes/factors/test/factor_test.pyx":17
  *         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None
  * 
  *     def _init_self(self, **kwargs):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_3_init_self, 0, __pyx_n_s_FactorTest__init_self, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_3_init_self, 0, __pyx_n_s_FactorTest__init_self, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init_self, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init_self, __pyx_t_2) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":19
+  /* "hermes/factors/test/factor_test.pyx":20
  *         pass
  * 
- *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap']):             # <<<<<<<<<<<<<<
+ *     def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap'], window=0):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         close_se = data['openPrice']
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_5test1, 0, __pyx_n_s_FactorTest_test1, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_5test1, 0, __pyx_n_s_FactorTest_test1, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults), 1)) __PYX_ERR(0, 19, __pyx_L1_error)
-  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults), 1)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_n_s_openPrice);
   __Pyx_GIVEREF(__pyx_n_s_openPrice);
   PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_openPrice);
   __Pyx_INCREF(__pyx_n_s_closePrice);
   __Pyx_GIVEREF(__pyx_n_s_closePrice);
   PyList_SET_ITEM(__pyx_t_5, 1, __pyx_n_s_closePrice);
   __Pyx_INCREF(__pyx_n_s_vwap);
   __Pyx_GIVEREF(__pyx_n_s_vwap);
   PyList_SET_ITEM(__pyx_t_5, 2, __pyx_n_s_vwap);
   __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_2)->__pyx_arg_dependencies = __pyx_t_5;
   __Pyx_GIVEREF(__pyx_t_5);
   __pyx_t_5 = 0;
   __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_6hermes_7factors_4test_11factor_test___defaults__);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_test1, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_test1, __pyx_t_2) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":29
+  /* "hermes/factors/test/factor_test.pyx":30
  *         return self._format(dy_q_evebitda_caldr_se, "test1")
  * 
- *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):             # <<<<<<<<<<<<<<
+ *     def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue'], window=10):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         close_se = data['marketValue']
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_7test2, 0, __pyx_n_s_FactorTest_test2, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_7test2, 0, __pyx_n_s_FactorTest_test2, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults1), 1)) __PYX_ERR(0, 29, __pyx_L1_error)
-  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 29, __pyx_L1_error)
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults1), 1)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_n_s_marketValue);
   __Pyx_GIVEREF(__pyx_n_s_marketValue);
   PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_marketValue);
   __Pyx_INCREF(__pyx_n_s_turnoverVol);
   __Pyx_GIVEREF(__pyx_n_s_turnoverVol);
   PyList_SET_ITEM(__pyx_t_5, 1, __pyx_n_s_turnoverVol);
   __Pyx_INCREF(__pyx_n_s_negMarketValue);
   __Pyx_GIVEREF(__pyx_n_s_negMarketValue);
   PyList_SET_ITEM(__pyx_t_5, 2, __pyx_n_s_negMarketValue);
   __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_t_2)->__pyx_arg_dependencies = __pyx_t_5;
   __Pyx_GIVEREF(__pyx_t_5);
   __pyx_t_5 = 0;
   __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_6hermes_7factors_4test_11factor_test_2__defaults__);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_test2, __pyx_t_2) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_test2, __pyx_t_2) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/test/factor_test.pyx":39
+  /* "hermes/factors/test/factor_test.pyx":40
  *         return self._format(dy_q_evebitda_caldr_se, "test2")
  * 
- *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):             # <<<<<<<<<<<<<<
+ *     def test3(self, data=None, dependencies=['turnoverVol', 'closePrice'], window=14):             # <<<<<<<<<<<<<<
  *         data = self._data if data is None else data
  *         turnoverVol = data['turnoverVol']
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_9test3, 0, __pyx_n_s_FactorTest_test3, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4test_11factor_test_10FactorTest_9test3, 0, __pyx_n_s_FactorTest_test3, NULL, __pyx_n_s_hermes_factors_test_factor_test, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults2), 1)) __PYX_ERR(0, 39, __pyx_L1_error)
-  __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L1_error)
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults2), 1)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_n_s_turnoverVol);
   __Pyx_GIVEREF(__pyx_n_s_turnoverVol);
   PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_turnoverVol);
   __Pyx_INCREF(__pyx_n_s_closePrice);
   __Pyx_GIVEREF(__pyx_n_s_closePrice);
   PyList_SET_ITEM(__pyx_t_5, 1, __pyx_n_s_closePrice);
   __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_t_2)->__pyx_arg_dependencies = __pyx_t_5;
   __Pyx_GIVEREF(__pyx_t_5);
   __pyx_t_5 = 0;
   __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_6hermes_7factors_4test_11factor_test_4__defaults__);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_test3, __pyx_t_2) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_test3, __pyx_t_2) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "hermes/factors/test/factor_test.pyx":7
  * 
  * 
  * class FactorTest(FactorBase, LongCallMixin, ShortCallMixin):             # <<<<<<<<<<<<<<
  *
```

### Comparing `Finance-Hermes-0.3.1/hermes/factors/test/factor_test.pyx` & `Finance-Hermes-0.3.2/hermes/factors/test/factor_test.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -5,42 +5,43 @@
 
 
 class FactorTest(FactorBase, LongCallMixin, ShortCallMixin):
 
     def __init__(self, data_format, **kwargs):
         __str__ = 'factor_test'
         self.category = 'test'
-        self.name = '测试因子'
+        self.name = 'Test Factor'
         self._data_format = data_format
+        self._max_window = 10
         self._data = self.init_data(**kwargs) if 'end_date' in kwargs else None
 
     def _init_self(self, **kwargs):
         pass
     
-    def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap']):
+    def test1(self, data=None, dependencies=['openPrice', 'closePrice', 'vwap'], window=0):
         data = self._data if data is None else data
         close_se = data['openPrice']
         dy_q_ti_se = data['closePrice']
         totalshares_se = data['vwap']
         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
         return self._format(dy_q_evebitda_caldr_se, "test1")
     
-    def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue']):
+    def test2(self, data=None, dependencies=['marketValue', 'turnoverVol', 'negMarketValue'], window=10):
         data = self._data if data is None else data
         close_se = data['marketValue']
         dy_q_ti_se = data['turnoverVol']
         totalshares_se = data['negMarketValue']
         dy_q_evebitda_caldr_se = close_se / (4 * dy_q_ti_se / totalshares_se)
         dy_q_evebitda_caldr_se[(dy_q_evebitda_caldr_se < 0) |
                                (np.isinf(dy_q_evebitda_caldr_se))] = np.nan
         return self._format(dy_q_evebitda_caldr_se, "test2")
     
-    def test3(self, data=None, dependencies=['turnoverVol', 'closePrice']):
+    def test3(self, data=None, dependencies=['turnoverVol', 'closePrice'], window=14):
         data = self._data if data is None else data
         turnoverVol = data['turnoverVol']
         closePrice = data['closePrice']
         factor1 = turnoverVol * closePrice
         factor2 = turnoverVol + closePrice
         factors = {
             'factor3': self._format(factor1, "factor3"),
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Finance-Hermes-0.3.1/hermes/kdutils/base.c` & `Finance-Hermes-0.3.2/hermes/kdutils/base.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/hermes/kdutils/base.pyx` & `Finance-Hermes-0.3.2/hermes/kdutils/base.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/hermes/kdutils/core/fixes.c` & `Finance-Hermes-0.3.2/hermes/kdutils/core/fixes.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/hermes/kdutils/core/fixes.pyx` & `Finance-Hermes-0.3.2/hermes/kdutils/core/fixes.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/hermes/kdutils/core/helper.c` & `Finance-Hermes-0.3.2/hermes/kdutils/core/helper.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/hermes/kdutils/core/helper.pyx` & `Finance-Hermes-0.3.2/hermes/kdutils/core/helper.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/hermes/kdutils/create_id.c` & `Finance-Hermes-0.3.2/hermes/kdutils/create_id.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/hermes/kdutils/create_id.pyx` & `Finance-Hermes-0.3.2/hermes/kdutils/create_id.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/hermes/kdutils/lazy.c` & `Finance-Hermes-0.3.2/hermes/kdutils/lazy.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/hermes/kdutils/lazy.pyx` & `Finance-Hermes-0.3.2/hermes/kdutils/lazy.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/hermes/lzador/calculater.c` & `Finance-Hermes-0.3.2/hermes/lzador/calculater.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/hermes/lzador/calculater.pyx` & `Finance-Hermes-0.3.2/hermes/lzador/calculater.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.1/setup.py` & `Finance-Hermes-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,16 @@
 else:
     n_cpu = 0
 
 ext_modules = [
     'hermes/kdutils/core/fixes.pyx', 'hermes/kdutils/core/helper.pyx',
     'hermes/factors/base.pyx', 'hermes/kdutils/base.pyx',
     'hermes/kdutils/create_id.pyx', 'hermes/kdutils/lazy.pyx',
-    'hermes/lzador/calculater.pyx', 'hermes/factors/test/factor_test.pyx'
+    'hermes/lzador/calculater.pyx', 'hermes/factors/test/factor_test.pyx',
+    'hermes/factors/trading/factor_north.pyx'
 ]
 
 
 def generate_extensions(ext_modules, line_trace=True):
 
     extensions = []
```

