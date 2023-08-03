# Comparing `tmp/FuncsForSPO-6.3.0.tar.gz` & `tmp/FuncsForSPO-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-6.3.0.tar", last modified: Mon Jul 31 12:53:04 2023, max compression
+gzip compressed data, was "FuncsForSPO-6.3.1.tar", last modified: Thu Aug  3 16:00:48 2023, max compression
```

## Comparing `FuncsForSPO-6.3.0.tar` & `FuncsForSPO-6.3.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.430457 FuncsForSPO-6.3.0/
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:03.858463 FuncsForSPO-6.3.0/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:03.933522 FuncsForSPO-6.3.0/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.3.0/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.3.0/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:03.946044 FuncsForSPO-6.3.0/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.3.0/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:03.958043 FuncsForSPO-6.3.0/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.3.0/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:03.982107 FuncsForSPO-6.3.0/FuncsForSPO/fgpt/
--rw-rw-rw-   0        0        0     2127 2023-07-08 15:03:37.000000 FuncsForSPO-6.3.0/FuncsForSPO/fgpt/__fgpt.py
--rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.3.0/FuncsForSPO/fgpt/__init__.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.3.0/FuncsForSPO/fgpt/base.py
--rw-rw-rw-   0        0        0    14957 2023-07-08 15:04:45.000000 FuncsForSPO-6.3.0/FuncsForSPO/fgpt/fgpt.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:03.989436 FuncsForSPO-6.3.0/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.3.0/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.012457 FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/__translator.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/base.py
--rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.024956 FuncsForSPO-6.3.0/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.3.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.032239 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.105939 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0    13836 2023-07-21 12:08:34.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     3602 2023-07-20 21:51:33.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
--rw-rw-rw-   0        0        0     2024 2023-07-21 11:40:46.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
--rw-rw-rw-   0        0        0     1173 2023-07-21 11:45:44.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
--rw-rw-rw-   0        0        0      616 2023-06-29 19:53:08.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.124682 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.142408 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.151045 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.185177 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/base.py
--rw-rw-rw-   0        0        0    10234 2023-07-31 12:52:24.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.203973 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.224274 FuncsForSPO-6.3.0/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.238057 FuncsForSPO-6.3.0/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    56235 2023-07-18 20:57:07.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.254740 FuncsForSPO-6.3.0/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.3.0/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.269942 FuncsForSPO-6.3.0/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    38845 2023-07-04 20:15:36.000000 FuncsForSPO-6.3.0/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.288144 FuncsForSPO-6.3.0/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.3.0/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.300831 FuncsForSPO-6.3.0/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.3.0/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.3.0/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.306859 FuncsForSPO-6.3.0/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.3.0/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:53:03.922815 FuncsForSPO-6.3.0/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8023 2023-07-31 12:53:03.000000 FuncsForSPO-6.3.0/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2127 2023-07-31 12:53:03.000000 FuncsForSPO-6.3.0/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 12:53:03.000000 FuncsForSPO-6.3.0/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-07-31 12:53:03.000000 FuncsForSPO-6.3.0/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      475 2023-07-31 12:53:03.000000 FuncsForSPO-6.3.0/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.3.0/LICENSE
--rw-rw-rw-   0        0        0     8023 2023-07-31 12:53:04.426752 FuncsForSPO-6.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-31 12:53:04.430457 FuncsForSPO-6.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2663 2023-07-31 12:52:49.000000 FuncsForSPO-6.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:48.050781 FuncsForSPO-6.3.1/
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.051778 FuncsForSPO-6.3.1/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.148677 FuncsForSPO-6.3.1/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.3.1/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.3.1/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.175743 FuncsForSPO-6.3.1/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.1/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.3.1/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.194912 FuncsForSPO-6.3.1/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.1/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.3.1/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.238637 FuncsForSPO-6.3.1/FuncsForSPO/fgpt/
+-rw-rw-rw-   0        0        0     2127 2023-07-08 15:03:37.000000 FuncsForSPO-6.3.1/FuncsForSPO/fgpt/__fgpt.py
+-rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.3.1/FuncsForSPO/fgpt/__init__.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.3.1/FuncsForSPO/fgpt/base.py
+-rw-rw-rw-   0        0        0    14957 2023-07-08 15:04:45.000000 FuncsForSPO-6.3.1/FuncsForSPO/fgpt/fgpt.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.247150 FuncsForSPO-6.3.1/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.3.1/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.286341 FuncsForSPO-6.3.1/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.3.1/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.3.1/FuncsForSPO/flanguage/translator/__translator.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.3.1/FuncsForSPO/flanguage/translator/base.py
+-rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.3.1/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.306113 FuncsForSPO-6.3.1/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.1/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.3.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.322497 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.522848 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0    13836 2023-07-21 12:08:34.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     3602 2023-07-20 21:51:33.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+-rw-rw-rw-   0        0        0     2024 2023-07-21 11:40:46.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+-rw-rw-rw-   0        0        0     1173 2023-07-21 11:45:44.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
+-rw-rw-rw-   0        0        0      616 2023-06-29 19:53:08.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.564189 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.586456 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.590995 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.650393 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/focr/base.py
+-rw-rw-rw-   0        0        0    10234 2023-07-31 12:52:24.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.672773 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.732062 FuncsForSPO-6.3.1/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.783584 FuncsForSPO-6.3.1/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    56235 2023-07-18 20:57:07.000000 FuncsForSPO-6.3.1/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.818030 FuncsForSPO-6.3.1/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.1/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.3.1/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.837576 FuncsForSPO-6.3.1/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.1/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    38845 2023-07-04 20:15:36.000000 FuncsForSPO-6.3.1/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.871372 FuncsForSPO-6.3.1/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.1/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.3.1/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.897383 FuncsForSPO-6.3.1/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.3.1/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.3.1/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.909242 FuncsForSPO-6.3.1/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.3.1/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:00:47.133724 FuncsForSPO-6.3.1/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8023 2023-08-03 16:00:46.000000 FuncsForSPO-6.3.1/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2127 2023-08-03 16:00:46.000000 FuncsForSPO-6.3.1/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 16:00:46.000000 FuncsForSPO-6.3.1/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-08-03 16:00:46.000000 FuncsForSPO-6.3.1/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      475 2023-08-03 16:00:46.000000 FuncsForSPO-6.3.1/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.3.1/LICENSE
+-rw-rw-rw-   0        0        0     8023 2023-08-03 16:00:48.045878 FuncsForSPO-6.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 16:00:48.050781 FuncsForSPO-6.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2716 2023-08-03 16:00:35.000000 FuncsForSPO-6.3.1/setup.py
```

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/femails/femails.py` & `FuncsForSPO-6.3.1/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fgpt/__fgpt.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fgpt/__fgpt.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fgpt/base.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fgpt/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fgpt/fgpt.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fgpt/fgpt.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/__translator.py` & `FuncsForSPO-6.3.1/FuncsForSPO/flanguage/translator/__translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/base.py` & `FuncsForSPO-6.3.1/FuncsForSPO/flanguage/translator/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-6.3.1/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/__ocr_online_v2.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/focr/__ocr_online_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/base.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/focr/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/pdfutils/pdfutils.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-6.3.1/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO/utils/utils.py` & `FuncsForSPO-6.3.1/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-6.3.1/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.3.0
+Version: 6.3.1
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.3.0/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-6.3.1/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/LICENSE` & `FuncsForSPO-6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/PKG-INFO` & `FuncsForSPO-6.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.3.0
+Version: 6.3.1
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.3.0/README.md` & `FuncsForSPO-6.3.1/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.3.0/setup.py` & `FuncsForSPO-6.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '6.3.0'
+version = '6.3.1'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
@@ -61,11 +61,13 @@
             'pypdf',
             'pywin32',
             'gdown',
             'pytesseract',
             'pymupdf',
             'PyPDF2',
             'sqlalchemy',
-            'rich==12.6.0',
-            'pyinstaller==5.6.2',
+            # 'rich==12.6.0',
+            # 'pyinstaller==5.6.2',
+            'rich',
+            'pyinstaller',
         ],
         )
```

