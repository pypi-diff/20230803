# Comparing `tmp/geospacelab-0.6.5.tar.gz` & `tmp/geospacelab-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geospacelab-0.6.5.tar", last modified: Sat Jul 15 00:08:10 2023, max compression
+gzip compressed data, was "geospacelab-0.6.6.tar", last modified: Thu Aug  3 08:47:10 2023, max compression
```

## Comparing `geospacelab-0.6.5.tar` & `geospacelab-0.6.6.tar`

### file list

```diff
@@ -1,379 +1,379 @@
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.060927 geospacelab-0.6.5/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1515 2021-08-21 16:59:48.000000 geospacelab-0.6.5/LICENSE
--rw-rw-r--   0 lei       (1000) lei       (1000)      279 2023-03-01 11:24:55.000000 geospacelab-0.6.5/MANIFEST.in
--rw-rw-r--   0 lei       (1000) lei       (1000)    22727 2023-07-15 00:08:10.060927 geospacelab-0.6.5/PKG-INFO
--rw-rw-r--   0 lei       (1000) lei       (1000)    21702 2023-02-21 14:28:53.000000 geospacelab-0.6.5/README.md
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.044927 geospacelab-0.6.5/geospacelab/
--rw-rw-r--   0 lei       (1000) lei       (1000)      505 2023-07-15 00:07:34.000000 geospacelab-0.6.5/geospacelab/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.044927 geospacelab-0.6.5/geospacelab/config/
--rw-rw-r--   0 lei       (1000) lei       (1000)      638 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/config/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4726 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/config/_preferences.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.044927 geospacelab-0.6.5/geospacelab/cs/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1282 2023-03-01 11:02:12.000000 geospacelab-0.6.5/geospacelab/cs/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      723 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/cs/_aacgm.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      756 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/cs/_apex.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    17124 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/cs/_cs_base.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    18253 2022-11-07 08:45:01.000000 geospacelab-0.6.5/geospacelab/cs/_geo.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      604 2021-08-21 16:59:48.000000 geospacelab-0.6.5/geospacelab/cs/geo_utilities.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.044927 geospacelab-0.6.5/geospacelab/datahub/
--rw-rw-r--   0 lei       (1000) lei       (1000)    19560 2023-02-06 07:59:04.000000 geospacelab-0.6.5/geospacelab/datahub/__dataset_base__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    18655 2022-11-29 09:26:23.000000 geospacelab-0.6.5/geospacelab/datahub/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2825 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/__metadata_base__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    38795 2023-06-08 13:44:45.000000 geospacelab-0.6.5/geospacelab/datahub/__variable_base__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.044927 geospacelab-0.6.5/geospacelab/datahub/sources/
--rw-rw-r--   0 lei       (1000) lei       (1000)      327 2022-12-07 06:22:00.000000 geospacelab-0.6.5/geospacelab/datahub/sources/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.044927 geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/
--rw-rw-r--   0 lei       (1000) lei       (1000)      680 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.044927 geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/dmsp/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-04-05 13:39:25.000000 geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/dmsp/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2516 2023-04-05 13:50:32.000000 geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.044927 geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/omni/
--rw-rw-r--   0 lei       (1000) lei       (1000)    10896 2023-04-03 09:52:12.000000 geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/omni/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4137 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/omni/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2995 2023-07-14 23:46:55.000000 geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/omni/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7341 2023-07-15 00:06:04.000000 geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/omni/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.044927 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/
--rw-rw-r--   0 lei       (1000) lei       (1000)      557 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/
--rw-rw-r--   0 lei       (1000) lei       (1000)      583 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_fp/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_fp/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/
--rw-rw-r--   0 lei       (1000) lei       (1000)    12352 2022-12-14 12:48:43.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1994 2022-12-14 12:22:24.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1499 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4888 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/
--rw-rw-r--   0 lei       (1000) lei       (1000)    12468 2022-12-14 12:48:43.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1840 2022-12-14 12:45:25.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1856 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5445 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct16/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct16/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6544 2022-12-14 12:13:27.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/l1b/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/l1b/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/l2d/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/l2d/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/l2l/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/l2l/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2605 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/loader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/
--rw-rw-r--   0 lei       (1000) lei       (1000)      737 2022-11-24 09:06:45.000000 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/image/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-11-24 08:47:10.000000 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/image/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/image/ie/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5771 2023-05-11 10:38:52.000000 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/image/ie/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3056 2023-06-26 11:16:03.000000 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/image/ie/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2582 2022-11-24 12:20:08.000000 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/image/ie/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3704 2023-02-03 18:57:40.000000 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/image/ie/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/miracle/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:07:56.000000 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/miracle/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/miracle/abk/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:19:05.000000 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/miracle/abk/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/miracle/kev/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:18:50.000000 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/miracle/kev/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/miracle/muo/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:18:58.000000 geospacelab-0.6.5/geospacelab/datahub/sources/fmi/miracle/muo/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/
--rw-rw-r--   0 lei       (1000) lei       (1000)      496 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4095 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/hpo/
--rw-rw-r--   0 lei       (1000) lei       (1000)     6386 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/hpo/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3896 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/hpo/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1590 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/hpo/loader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/hpo/nowcast/
--rw-rw-r--   0 lei       (1000) lei       (1000)     6310 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/hpo/nowcast/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4665 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/hpo/nowcast/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2687 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/hpo/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5666 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6630 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1563 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/loader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/nowcast/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5644 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/nowcast/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7365 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/nowcast/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1563 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/nowcast/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/nowcast/variable_config.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/snf107/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5707 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/snf107/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1663 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/snf107/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/gfz/snf107/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/
--rw-rw-r--   0 lei       (1000) lei       (1000)      556 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/ampere/
--rw-rw-r--   0 lei       (1000) lei       (1000)      155 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/ampere/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/ampere/fitted/
--rw-rw-r--   0 lei       (1000) lei       (1000)     8505 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/ampere/fitted/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2709 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/ampere/fitted/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1546 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/ampere/fitted/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/ampere/grd/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-09 08:44:35.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/ampere/grd/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    11635 2023-06-09 10:16:48.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/ampere/grd/loader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/
--rw-rw-r--   0 lei       (1000) lei       (1000)      155 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5496 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/
--rw-rw-r--   0 lei       (1000) lei       (1000)     8283 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5322 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4347 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/
--rw-rw-r--   0 lei       (1000) lei       (1000)    12477 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     9531 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4686 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/
--rw-rw-r--   0 lei       (1000) lei       (1000)     2034 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/gnss/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/gnss/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/gnss/tecmap/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5966 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/gnss/tecmap/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4305 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/gnss/tecmap/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2895 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/gnss/tecmap/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1517 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/gnss/tecmap/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/
--rw-rw-r--   0 lei       (1000) lei       (1000)    15249 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    16084 2022-11-05 11:21:54.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.048927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      652 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/eiscat_hdf5_info.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    16337 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2514 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/utilities.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8330 2023-04-19 11:06:29.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/
--rw-rw-r--   0 lei       (1000) lei       (1000)    14228 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7529 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8274 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/variable_config.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8269 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/
--rw-rw-r--   0 lei       (1000) lei       (1000)     7925 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3753 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6371 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/
--rw-rw-r--   0 lei       (1000) lei       (1000)     7851 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3397 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8949 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/
--rw-rw-r--   0 lei       (1000) lei       (1000)      524 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4817 2022-11-05 11:03:22.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/
--rw-rw-r--   0 lei       (1000) lei       (1000)    10317 2022-09-08 10:10:13.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4902 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    10280 2023-04-20 12:28:27.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/
--rw-r--r--   0 lei       (1000) lei       (1000)    11542 2023-04-20 09:13:20.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3360 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6745 2023-04-19 11:05:17.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/
--rw-rw-r--   0 lei       (1000) lei       (1000)    10204 2022-09-08 10:10:14.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3229 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4054 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/variable_config.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4717 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/utilities.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/ncei/
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/ncei/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/ncei/dmsp/
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/ncei/dmsp/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/nipr/
--rw-rw-r--   0 lei       (1000) lei       (1000)      764 2023-06-01 07:10:28.000000 geospacelab-0.6.5/geospacelab/datahub/sources/nipr/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/nipr/asc/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:59:47.000000 geospacelab-0.6.5/geospacelab/datahub/sources/nipr/asc/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/nipr/asc/tro_wmi/
--rw-rw-r--   0 lei       (1000) lei       (1000)    11064 2023-06-02 07:24:23.000000 geospacelab-0.6.5/geospacelab/datahub/sources/nipr/asc/tro_wmi/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1850 2023-06-01 13:04:28.000000 geospacelab-0.6.5/geospacelab/datahub/sources/nipr/asc/tro_wmi/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8330 2023-04-19 11:06:29.000000 geospacelab-0.6.5/geospacelab/datahub/sources/nipr/asc/tro_wmi/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/noaa/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/noaa/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/noaa/swpc/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/noaa/swpc/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/noaa/swpc/goesxray/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/noaa/swpc/goesxray/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/noaa/swpc/solarwind/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/noaa/swpc/solarwind/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/superdarn/
--rw-rw-r--   0 lei       (1000) lei       (1000)      592 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/superdarn/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/superdarn/potmap/
--rw-rw-r--   0 lei       (1000) lei       (1000)     8795 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/superdarn/potmap/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5756 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/superdarn/potmap/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    10900 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/superdarn/potmap/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1551 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/superdarn/potmap/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/supermag/
--rw-rw-r--   0 lei       (1000) lei       (1000)     2019 2023-02-03 11:28:38.000000 geospacelab-0.6.5/geospacelab/datahub/sources/supermag/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/supermag/indices/
--rw-rw-r--   0 lei       (1000) lei       (1000)     6727 2023-02-06 06:54:34.000000 geospacelab-0.6.5/geospacelab/datahub/sources/supermag/indices/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7842 2023-02-06 06:47:42.000000 geospacelab-0.6.5/geospacelab/datahub/sources/supermag/indices/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1531 2023-02-06 08:02:57.000000 geospacelab-0.6.5/geospacelab/datahub/sources/supermag/indices/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3006 2023-02-03 18:57:39.000000 geospacelab-0.6.5/geospacelab/datahub/sources/supermag/indices/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/supermag/magnetometer/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/supermag/magnetometer/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    27422 2023-02-03 11:24:53.000000 geospacelab-0.6.5/geospacelab/datahub/sources/supermag/supermag_api.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/tud/
--rw-rw-r--   0 lei       (1000) lei       (1000)     2742 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/
--rw-rw-r--   0 lei       (1000) lei       (1000)      595 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/dns_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9336 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/dns_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1591 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/dns_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2436 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/dns_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3337 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/dns_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/wnd_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9389 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/wnd_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1591 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/wnd_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2890 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/wnd_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5546 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/wnd_acc/variable_config.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5469 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/tud/goce/
--rw-rw-r--   0 lei       (1000) lei       (1000)      569 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/goce/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9506 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1593 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3715 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6288 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/
--rw-rw-r--   0 lei       (1000) lei       (1000)      578 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/dns_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)    12306 2022-11-28 12:45:58.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/dns_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1621 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/dns_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4335 2022-10-10 08:45:16.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/dns_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4116 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/dns_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/wnd_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)    10348 2023-01-27 09:29:24.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/wnd_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1618 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/wnd_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2867 2023-01-15 11:57:47.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/wnd_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3346 2023-01-27 09:35:38.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/wnd_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace_fo/
--rw-rw-r--   0 lei       (1000) lei       (1000)      578 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace_fo/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.052927 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace_fo/dns_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9615 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace_fo/dns_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1739 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace_fo/dns_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2731 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace_fo/dns_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4116 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace_fo/dns_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/
--rw-rw-r--   0 lei       (1000) lei       (1000)      583 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9240 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1622 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2039 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3336 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_pod/
--rw-rw-r--   0 lei       (1000) lei       (1000)    11754 2022-10-11 09:28:21.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_pod/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1622 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_pod/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2039 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_pod/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3336 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_pod/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1648 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/ae/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5351 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/ae/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6552 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/ae/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1585 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/ae/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3704 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/ae/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/asysym/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5383 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/asysym/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6635 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/asysym/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1610 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/asysym/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3728 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/asysym/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/dst/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5337 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/dst/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6235 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/dst/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1521 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/dst/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1516 2022-02-23 05:03:33.000000 geospacelab-0.6.5/geospacelab/datahub/sources/wdc/dst/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/express/
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-21 16:59:48.000000 geospacelab-0.6.5/geospacelab/express/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4152 2022-10-18 12:32:59.000000 geospacelab-0.6.5/geospacelab/express/dmsp_dashboard.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8218 2023-01-16 12:39:08.000000 geospacelab-0.6.5/geospacelab/express/eiscat_dashboard.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7978 2022-11-11 08:30:29.000000 geospacelab-0.6.5/geospacelab/express/millstonehill_dashboard.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3937 2022-11-21 13:16:14.000000 geospacelab-0.6.5/geospacelab/express/omni_dashboard.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/future/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/future/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/future/empiricalmodels/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/future/empiricalmodels/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/future/empiricalmodels/ovationprime2010/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/future/empiricalmodels/ovationprime2010/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    39045 2023-03-01 11:22:40.000000 geospacelab-0.6.5/geospacelab/future/empiricalmodels/ovationprime2010/ovationprime.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/future/satllites/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/future/satllites/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5213 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/future/satllites/orbit_analyzer.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1151 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/future/test_sscws.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/observatory/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/observatory/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)       11 2022-09-08 09:38:55.000000 geospacelab-0.6.5/geospacelab/observatory/constants.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/observatory/earth/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/observatory/earth/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3720 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/observatory/earth/_func.py
--rw-rw-r--   0 lei       (1000) lei       (1000)       10 2022-09-08 09:37:46.000000 geospacelab-0.6.5/geospacelab/observatory/earth/constants.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1082 2022-09-08 09:57:47.000000 geospacelab-0.6.5/geospacelab/observatory/earth/geodesy.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/observatory/orbit/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-09-08 10:08:40.000000 geospacelab-0.6.5/geospacelab/observatory/orbit/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    13350 2022-11-14 20:00:31.000000 geospacelab-0.6.5/geospacelab/observatory/orbit/sc_orbit.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    23767 2023-01-27 13:25:36.000000 geospacelab-0.6.5/geospacelab/observatory/orbit/utilities.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/quantity/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-09-03 10:12:23.000000 geospacelab-0.6.5/geospacelab/quantity/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/toolbox/
--rw-rw-r--   0 lei       (1000) lei       (1000)       56 2021-07-13 05:22:19.000000 geospacelab-0.6.5/geospacelab/toolbox/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/toolbox/io/
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-21 16:59:48.000000 geospacelab-0.6.5/geospacelab/toolbox/io/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1067 2021-08-21 16:59:48.000000 geospacelab-0.6.5/geospacelab/toolbox/io/dialog.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/toolbox/unit/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-07-13 05:22:19.000000 geospacelab-0.6.5/geospacelab/toolbox/unit/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/toolbox/utilities/
--rw-rw-r--   0 lei       (1000) lei       (1000)        1 2021-07-13 05:22:19.000000 geospacelab-0.6.5/geospacelab/toolbox/utilities/__init__.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)     6067 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/toolbox/utilities/numpyarray.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1838 2022-10-10 13:43:05.000000 geospacelab-0.6.5/geospacelab/toolbox/utilities/numpymath.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)     3310 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/toolbox/utilities/pybasic.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)     2813 2021-11-29 20:45:17.000000 geospacelab-0.6.5/geospacelab/toolbox/utilities/pyclass.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)    10865 2023-02-06 11:56:22.000000 geospacelab-0.6.5/geospacelab/toolbox/utilities/pydatetime.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)     1816 2021-08-21 16:59:48.000000 geospacelab-0.6.5/geospacelab/toolbox/utilities/pylogging.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      754 2021-08-21 16:59:48.000000 geospacelab-0.6.5/geospacelab/toolbox/utilities/pyos.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/visualization/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1025 2023-02-06 14:01:52.000000 geospacelab-0.6.5/geospacelab/visualization/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/visualization/mpl/
--rw-rw-r--   0 lei       (1000) lei       (1000)    31503 2023-04-20 12:11:24.000000 geospacelab-0.6.5/geospacelab/visualization/mpl/__base__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      825 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/visualization/mpl/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      747 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/visualization/mpl/_helpers.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-30 07:16:41.000000 geospacelab-0.6.5/geospacelab/visualization/mpl/axes.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)    14484 2023-05-17 11:50:34.000000 geospacelab-0.6.5/geospacelab/visualization/mpl/axis_ticks.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7090 2023-02-09 07:50:05.000000 geospacelab-0.6.5/geospacelab/visualization/mpl/colormaps.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    16912 2023-05-09 07:55:30.000000 geospacelab-0.6.5/geospacelab/visualization/mpl/dashboards.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3335 2021-11-29 20:45:17.000000 geospacelab-0.6.5/geospacelab/visualization/mpl/figure.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/visualization/mpl/geomap/
--rw-rw-r--   0 lei       (1000) lei       (1000)     2368 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/visualization/mpl/geomap/__base__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      327 2022-08-30 10:45:18.000000 geospacelab-0.6.5/geospacelab/visualization/mpl/geomap/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2847 2022-12-14 09:15:38.000000 geospacelab-0.6.5/geospacelab/visualization/mpl/geomap/geodashboards.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    37622 2023-05-19 14:06:23.000000 geospacelab-0.6.5/geospacelab/visualization/mpl/geomap/geopanels.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    32516 2023-06-09 07:05:12.000000 geospacelab-0.6.5/geospacelab/visualization/mpl/panels.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/visualization/plotly/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-10-20 11:58:01.000000 geospacelab-0.6.5/geospacelab/visualization/plotly/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      224 2021-10-20 11:58:01.000000 geospacelab-0.6.5/geospacelab/visualization/plotly/ipanel.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.056927 geospacelab-0.6.5/geospacelab/wrapper/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-07-13 05:22:19.000000 geospacelab-0.6.5/geospacelab/wrapper/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.060927 geospacelab-0.6.5/geospacelab/wrapper/geopack/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1067 2023-03-01 10:54:57.000000 geospacelab-0.6.5/geospacelab/wrapper/geopack/LICENSE
--rw-rw-r--   0 lei       (1000) lei       (1000)    16623 2023-03-01 10:54:57.000000 geospacelab-0.6.5/geospacelab/wrapper/geopack/README.md
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-03-01 10:52:29.000000 geospacelab-0.6.5/geospacelab/wrapper/geopack/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.060927 geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-03-01 10:54:57.000000 geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/__init__.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)    48858 2023-03-01 11:38:52.000000 geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/geopack.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    40639 2023-03-01 10:54:57.000000 geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/igrf13coeffs.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)    76431 2023-03-01 10:54:57.000000 geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/t01.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    75795 2023-03-01 10:54:57.000000 geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/t04.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    14024 2023-03-01 10:54:57.000000 geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/t89.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    65292 2023-03-01 10:54:57.000000 geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/t96.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    15324 2023-03-01 10:54:57.000000 geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/test_geopack1.md
--rw-rw-r--   0 lei       (1000) lei       (1000)     6669 2023-03-01 11:22:40.000000 geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/test_geopack1.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-07-15 00:08:10.044927 geospacelab-0.6.5/geospacelab.egg-info/
--rw-rw-r--   0 lei       (1000) lei       (1000)    22727 2023-07-15 00:08:09.000000 geospacelab-0.6.5/geospacelab.egg-info/PKG-INFO
--rw-rw-r--   0 lei       (1000) lei       (1000)    14102 2023-07-15 00:08:10.000000 geospacelab-0.6.5/geospacelab.egg-info/SOURCES.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)        1 2023-07-15 00:08:09.000000 geospacelab-0.6.5/geospacelab.egg-info/dependency_links.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)      229 2023-07-15 00:08:09.000000 geospacelab-0.6.5/geospacelab.egg-info/requires.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)       23 2023-07-15 00:08:09.000000 geospacelab-0.6.5/geospacelab.egg-info/top_level.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)      148 2023-07-15 00:08:10.060927 geospacelab-0.6.5/setup.cfg
--rw-rw-r--   0 lei       (1000) lei       (1000)     3410 2023-03-01 11:42:51.000000 geospacelab-0.6.5/setup.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1515 2021-08-21 16:59:48.000000 geospacelab-0.6.6/LICENSE
+-rw-rw-r--   0 lei       (1000) lei       (1000)      279 2023-03-01 11:24:55.000000 geospacelab-0.6.6/MANIFEST.in
+-rw-rw-r--   0 lei       (1000) lei       (1000)    22727 2023-08-03 08:47:10.081039 geospacelab-0.6.6/PKG-INFO
+-rw-rw-r--   0 lei       (1000) lei       (1000)    21702 2023-02-21 14:28:53.000000 geospacelab-0.6.6/README.md
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      505 2023-08-03 08:47:01.000000 geospacelab-0.6.6/geospacelab/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/config/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      638 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/config/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4726 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/config/_preferences.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/cs/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1282 2023-03-01 11:02:12.000000 geospacelab-0.6.6/geospacelab/cs/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      723 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/cs/_aacgm.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      756 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/cs/_apex.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    17124 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/cs/_cs_base.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    18253 2022-11-07 08:45:01.000000 geospacelab-0.6.6/geospacelab/cs/_geo.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      604 2021-08-21 16:59:48.000000 geospacelab-0.6.6/geospacelab/cs/geo_utilities.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    19625 2023-08-03 07:48:27.000000 geospacelab-0.6.6/geospacelab/datahub/__dataset_base__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    18655 2022-11-29 09:26:23.000000 geospacelab-0.6.6/geospacelab/datahub/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2825 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/__metadata_base__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    38795 2023-06-08 13:44:45.000000 geospacelab-0.6.6/geospacelab/datahub/__variable_base__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      327 2022-12-07 06:22:00.000000 geospacelab-0.6.6/geospacelab/datahub/sources/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      680 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/dmsp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-04-05 13:39:25.000000 geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/dmsp/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2516 2023-04-05 13:50:32.000000 geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/omni/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10896 2023-04-03 09:52:12.000000 geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/omni/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4137 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/omni/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2995 2023-07-14 23:46:55.000000 geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/omni/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7341 2023-07-15 00:06:04.000000 geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/omni/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      557 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      583 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_fp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_fp/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    12352 2022-12-14 12:48:43.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1994 2022-12-14 12:22:24.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1499 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4888 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    12468 2022-12-14 12:48:43.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1840 2022-12-14 12:45:25.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1856 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5445 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct16/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct16/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6544 2022-12-14 12:13:27.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/l1b/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/l1b/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/l2d/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/l2d/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/l2l/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/l2l/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2605 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/loader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      737 2022-11-24 09:06:45.000000 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/image/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-11-24 08:47:10.000000 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/image/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/image/ie/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5771 2023-05-11 10:38:52.000000 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/image/ie/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3056 2023-06-26 11:16:03.000000 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/image/ie/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2582 2022-11-24 12:20:08.000000 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/image/ie/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3704 2023-02-03 18:57:40.000000 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/image/ie/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/miracle/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:07:56.000000 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/miracle/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/miracle/abk/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:19:05.000000 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/miracle/abk/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/miracle/kev/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:18:50.000000 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/miracle/kev/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/miracle/muo/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:18:58.000000 geospacelab-0.6.6/geospacelab/datahub/sources/fmi/miracle/muo/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      496 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4095 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/hpo/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6386 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/hpo/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3896 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/hpo/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1590 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/hpo/loader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/hpo/nowcast/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6310 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/hpo/nowcast/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4665 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/hpo/nowcast/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2687 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/hpo/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5666 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6630 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1563 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/loader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/nowcast/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5644 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/nowcast/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7365 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/nowcast/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1563 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/nowcast/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/nowcast/variable_config.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/snf107/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5707 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/snf107/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1663 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/snf107/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/gfz/snf107/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      556 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/ampere/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      155 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/ampere/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/ampere/fitted/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8505 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/ampere/fitted/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2709 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/ampere/fitted/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1546 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/ampere/fitted/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/ampere/grd/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-09 08:44:35.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/ampere/grd/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    11635 2023-06-09 10:16:48.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/ampere/grd/loader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      155 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5496 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8283 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5322 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4347 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    12477 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9531 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4686 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2034 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/gnss/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/gnss/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/gnss/tecmap/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5966 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/gnss/tecmap/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4305 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/gnss/tecmap/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2895 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/gnss/tecmap/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1517 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/gnss/tecmap/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    15249 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    16084 2022-11-05 11:21:54.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      652 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/eiscat_hdf5_info.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    16337 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2514 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/utilities.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8330 2023-04-19 11:06:29.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    14228 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7529 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8274 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/variable_config.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8269 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7925 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3753 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6371 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7851 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3397 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8949 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      524 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4817 2022-11-05 11:03:22.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.073039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10317 2022-09-08 10:10:13.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4902 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10280 2023-04-20 12:28:27.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/
+-rw-r--r--   0 lei       (1000) lei       (1000)    11542 2023-04-20 09:13:20.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3360 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6745 2023-04-19 11:05:17.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10204 2022-09-08 10:10:14.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3229 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4054 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/variable_config.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4717 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/utilities.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/ncei/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/ncei/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/ncei/dmsp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/ncei/dmsp/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/nipr/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      764 2023-06-01 07:10:28.000000 geospacelab-0.6.6/geospacelab/datahub/sources/nipr/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/nipr/asc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:59:47.000000 geospacelab-0.6.6/geospacelab/datahub/sources/nipr/asc/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/nipr/asc/tro_wmi/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    11064 2023-06-02 07:24:23.000000 geospacelab-0.6.6/geospacelab/datahub/sources/nipr/asc/tro_wmi/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1850 2023-06-01 13:04:28.000000 geospacelab-0.6.6/geospacelab/datahub/sources/nipr/asc/tro_wmi/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8330 2023-04-19 11:06:29.000000 geospacelab-0.6.6/geospacelab/datahub/sources/nipr/asc/tro_wmi/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/noaa/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/noaa/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/noaa/swpc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/noaa/swpc/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/noaa/swpc/goesxray/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/noaa/swpc/goesxray/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/noaa/swpc/solarwind/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/noaa/swpc/solarwind/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/superdarn/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      592 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/superdarn/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/superdarn/potmap/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8795 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/superdarn/potmap/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5756 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/superdarn/potmap/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10900 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/superdarn/potmap/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1551 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/superdarn/potmap/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/supermag/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2019 2023-02-03 11:28:38.000000 geospacelab-0.6.6/geospacelab/datahub/sources/supermag/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/supermag/indices/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6727 2023-02-06 06:54:34.000000 geospacelab-0.6.6/geospacelab/datahub/sources/supermag/indices/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7842 2023-02-06 06:47:42.000000 geospacelab-0.6.6/geospacelab/datahub/sources/supermag/indices/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1531 2023-02-06 08:02:57.000000 geospacelab-0.6.6/geospacelab/datahub/sources/supermag/indices/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3006 2023-02-03 18:57:39.000000 geospacelab-0.6.6/geospacelab/datahub/sources/supermag/indices/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/supermag/magnetometer/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/supermag/magnetometer/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    27422 2023-02-03 11:24:53.000000 geospacelab-0.6.6/geospacelab/datahub/sources/supermag/supermag_api.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/tud/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2742 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      595 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/dns_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9336 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/dns_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1591 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/dns_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2436 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/dns_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3337 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/dns_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/wnd_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9389 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/wnd_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1591 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/wnd_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2890 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/wnd_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5546 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/wnd_acc/variable_config.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5469 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/tud/goce/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      569 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/goce/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9506 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1593 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3715 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6288 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      578 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/dns_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    12306 2022-11-28 12:45:58.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/dns_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1621 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/dns_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4335 2022-10-10 08:45:16.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/dns_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4116 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/dns_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/wnd_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10436 2023-08-03 07:51:09.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/wnd_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1648 2023-08-03 07:57:12.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/wnd_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2867 2023-01-15 11:57:47.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/wnd_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3346 2023-01-27 09:35:38.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/wnd_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace_fo/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      578 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace_fo/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace_fo/dns_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9615 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace_fo/dns_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1739 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace_fo/dns_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2731 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace_fo/dns_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4116 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace_fo/dns_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      583 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9240 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1622 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2039 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3336 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_pod/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    11754 2022-10-11 09:28:21.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_pod/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1622 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_pod/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2039 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_pod/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3336 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_pod/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1648 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/ae/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5351 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/ae/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6552 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/ae/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1585 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/ae/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3704 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/ae/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.077039 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/asysym/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5383 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/asysym/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6635 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/asysym/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1610 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/asysym/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3728 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/asysym/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/dst/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5337 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/dst/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6235 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/dst/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1521 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/dst/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1516 2022-02-23 05:03:33.000000 geospacelab-0.6.6/geospacelab/datahub/sources/wdc/dst/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/express/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-21 16:59:48.000000 geospacelab-0.6.6/geospacelab/express/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4152 2022-10-18 12:32:59.000000 geospacelab-0.6.6/geospacelab/express/dmsp_dashboard.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8218 2023-01-16 12:39:08.000000 geospacelab-0.6.6/geospacelab/express/eiscat_dashboard.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7978 2022-11-11 08:30:29.000000 geospacelab-0.6.6/geospacelab/express/millstonehill_dashboard.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3937 2022-11-21 13:16:14.000000 geospacelab-0.6.6/geospacelab/express/omni_dashboard.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/future/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/future/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/future/empiricalmodels/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/future/empiricalmodels/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/future/empiricalmodels/ovationprime2010/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/future/empiricalmodels/ovationprime2010/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    39045 2023-03-01 11:22:40.000000 geospacelab-0.6.6/geospacelab/future/empiricalmodels/ovationprime2010/ovationprime.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/future/satllites/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/future/satllites/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5213 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/future/satllites/orbit_analyzer.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1151 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/future/test_sscws.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/observatory/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/observatory/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)       11 2022-09-08 09:38:55.000000 geospacelab-0.6.6/geospacelab/observatory/constants.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/observatory/earth/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/observatory/earth/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3720 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/observatory/earth/_func.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)       10 2022-09-08 09:37:46.000000 geospacelab-0.6.6/geospacelab/observatory/earth/constants.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1082 2022-09-08 09:57:47.000000 geospacelab-0.6.6/geospacelab/observatory/earth/geodesy.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/observatory/orbit/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-09-08 10:08:40.000000 geospacelab-0.6.6/geospacelab/observatory/orbit/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    13350 2022-11-14 20:00:31.000000 geospacelab-0.6.6/geospacelab/observatory/orbit/sc_orbit.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    23767 2023-01-27 13:25:36.000000 geospacelab-0.6.6/geospacelab/observatory/orbit/utilities.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/quantity/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-09-03 10:12:23.000000 geospacelab-0.6.6/geospacelab/quantity/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/toolbox/
+-rw-rw-r--   0 lei       (1000) lei       (1000)       56 2021-07-13 05:22:19.000000 geospacelab-0.6.6/geospacelab/toolbox/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/toolbox/io/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-21 16:59:48.000000 geospacelab-0.6.6/geospacelab/toolbox/io/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1067 2021-08-21 16:59:48.000000 geospacelab-0.6.6/geospacelab/toolbox/io/dialog.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/toolbox/unit/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-07-13 05:22:19.000000 geospacelab-0.6.6/geospacelab/toolbox/unit/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/toolbox/utilities/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        1 2021-07-13 05:22:19.000000 geospacelab-0.6.6/geospacelab/toolbox/utilities/__init__.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)     6067 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/toolbox/utilities/numpyarray.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1838 2022-10-10 13:43:05.000000 geospacelab-0.6.6/geospacelab/toolbox/utilities/numpymath.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)     3310 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/toolbox/utilities/pybasic.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)     2813 2021-11-29 20:45:17.000000 geospacelab-0.6.6/geospacelab/toolbox/utilities/pyclass.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)    10865 2023-02-06 11:56:22.000000 geospacelab-0.6.6/geospacelab/toolbox/utilities/pydatetime.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)     1816 2021-08-21 16:59:48.000000 geospacelab-0.6.6/geospacelab/toolbox/utilities/pylogging.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      754 2021-08-21 16:59:48.000000 geospacelab-0.6.6/geospacelab/toolbox/utilities/pyos.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/visualization/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1025 2023-02-06 14:01:52.000000 geospacelab-0.6.6/geospacelab/visualization/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/visualization/mpl/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    31503 2023-04-20 12:11:24.000000 geospacelab-0.6.6/geospacelab/visualization/mpl/__base__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      825 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/visualization/mpl/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      747 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/visualization/mpl/_helpers.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-30 07:16:41.000000 geospacelab-0.6.6/geospacelab/visualization/mpl/axes.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)    14484 2023-05-17 11:50:34.000000 geospacelab-0.6.6/geospacelab/visualization/mpl/axis_ticks.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7090 2023-02-09 07:50:05.000000 geospacelab-0.6.6/geospacelab/visualization/mpl/colormaps.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    16912 2023-05-09 07:55:30.000000 geospacelab-0.6.6/geospacelab/visualization/mpl/dashboards.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3335 2021-11-29 20:45:17.000000 geospacelab-0.6.6/geospacelab/visualization/mpl/figure.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/visualization/mpl/geomap/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2368 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/visualization/mpl/geomap/__base__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      327 2022-08-30 10:45:18.000000 geospacelab-0.6.6/geospacelab/visualization/mpl/geomap/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2847 2022-12-14 09:15:38.000000 geospacelab-0.6.6/geospacelab/visualization/mpl/geomap/geodashboards.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    37622 2023-05-19 14:06:23.000000 geospacelab-0.6.6/geospacelab/visualization/mpl/geomap/geopanels.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    32516 2023-06-09 07:05:12.000000 geospacelab-0.6.6/geospacelab/visualization/mpl/panels.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/visualization/plotly/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-10-20 11:58:01.000000 geospacelab-0.6.6/geospacelab/visualization/plotly/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      224 2021-10-20 11:58:01.000000 geospacelab-0.6.6/geospacelab/visualization/plotly/ipanel.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/wrapper/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-07-13 05:22:19.000000 geospacelab-0.6.6/geospacelab/wrapper/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/wrapper/geopack/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1067 2023-03-01 10:54:57.000000 geospacelab-0.6.6/geospacelab/wrapper/geopack/LICENSE
+-rw-rw-r--   0 lei       (1000) lei       (1000)    16623 2023-03-01 10:54:57.000000 geospacelab-0.6.6/geospacelab/wrapper/geopack/README.md
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-03-01 10:52:29.000000 geospacelab-0.6.6/geospacelab/wrapper/geopack/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.081039 geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-03-01 10:54:57.000000 geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/__init__.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)    48858 2023-03-01 11:38:52.000000 geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/geopack.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    40639 2023-03-01 10:54:57.000000 geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/igrf13coeffs.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)    76431 2023-03-01 10:54:57.000000 geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/t01.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    75795 2023-03-01 10:54:57.000000 geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/t04.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    14024 2023-03-01 10:54:57.000000 geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/t89.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    65292 2023-03-01 10:54:57.000000 geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/t96.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    15324 2023-03-01 10:54:57.000000 geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/test_geopack1.md
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6669 2023-03-01 11:22:40.000000 geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/test_geopack1.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2023-08-03 08:47:10.069039 geospacelab-0.6.6/geospacelab.egg-info/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    22727 2023-08-03 08:47:10.000000 geospacelab-0.6.6/geospacelab.egg-info/PKG-INFO
+-rw-rw-r--   0 lei       (1000) lei       (1000)    14102 2023-08-03 08:47:10.000000 geospacelab-0.6.6/geospacelab.egg-info/SOURCES.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)        1 2023-08-03 08:47:10.000000 geospacelab-0.6.6/geospacelab.egg-info/dependency_links.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)      230 2023-08-03 08:47:10.000000 geospacelab-0.6.6/geospacelab.egg-info/requires.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)       23 2023-08-03 08:47:10.000000 geospacelab-0.6.6/geospacelab.egg-info/top_level.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)      148 2023-08-03 08:47:10.085039 geospacelab-0.6.6/setup.cfg
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3411 2023-07-20 08:49:11.000000 geospacelab-0.6.6/setup.py
```

### Comparing `geospacelab-0.6.5/LICENSE` & `geospacelab-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/PKG-INFO` & `geospacelab-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geospacelab
-Version: 0.6.5
+Version: 0.6.6
 Summary: Collect, manage, and visualize geospace data.
 Home-page: https://github.com/JouleCai/geospacelab
 Author: Lei Cai
 Author-email: lei.cai@oulu.fi
 License: BSD 3-Clause License
 Keywords: Geospace,EISCAT,DMSP,Space weather,Ionosphere,Space,Magnetosphere
 Classifier: Development Status :: 4 - Beta
```

### Comparing `geospacelab-0.6.5/README.md` & `geospacelab-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/config/__init__.py` & `geospacelab-0.6.6/geospacelab/config/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/config/_preferences.py` & `geospacelab-0.6.6/geospacelab/config/_preferences.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/cs/__init__.py` & `geospacelab-0.6.6/geospacelab/cs/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/cs/_aacgm.py` & `geospacelab-0.6.6/geospacelab/cs/_aacgm.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/cs/_apex.py` & `geospacelab-0.6.6/geospacelab/cs/_apex.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/cs/_cs_base.py` & `geospacelab-0.6.6/geospacelab/cs/_cs_base.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/cs/_geo.py` & `geospacelab-0.6.6/geospacelab/cs/_geo.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/cs/geo_utilities.py` & `geospacelab-0.6.6/geospacelab/cs/geo_utilities.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/__dataset_base__.py` & `geospacelab-0.6.6/geospacelab/datahub/__dataset_base__.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,15 @@
         self.data_file_ext = kwargs.pop('data_file_ext', '*')
         self.data_search_recursive = kwargs.pop('data_search_recursive', False)
         self.time_clip = kwargs.pop('time_clip', True)
 
     def search_data_files(
             self,
             initial_file_dir=None, search_pattern='*', recursive=None,
-            direct_append=True, allow_multiple_files=False,
+            direct_append=True, allow_multiple_files=False, include_extension=True,
             **kwargs) -> list:
         """
         Search the data files by the input pattern in the file name. The search method is based on pathlib.glob.
         For a dataset inheritance, a wrapper can be added for a custom setting.
 
         :param initial_file_dir: The initial file directory for searching.
         :type initial_file_dir: str or pathlib.Path, default: DatasetModel.data_root_dir.
@@ -284,16 +284,17 @@
         """
 
         file_paths = []
         if initial_file_dir is None:
             initial_file_dir = self.data_root_dir
         if recursive is None:
             recursive = self.data_search_recursive
-        if str(self.data_file_ext):
-            search_pattern = search_pattern + '.' + self.data_file_ext
+        if include_extension:   
+            if str(self.data_file_ext):
+                search_pattern = search_pattern + '.' + self.data_file_ext
         if recursive:
             search_pattern = '**/' + search_pattern
         paths = list(initial_file_dir.glob(search_pattern))
 
         import natsort
         paths = natsort.natsorted(paths, reverse=False)
         if len(paths) == 1:
```

### Comparing `geospacelab-0.6.5/geospacelab/datahub/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/__metadata_base__.py` & `geospacelab-0.6.6/geospacelab/datahub/__metadata_base__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/__variable_base__.py` & `geospacelab-0.6.6/geospacelab/datahub/__variable_base__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/omni/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/omni/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/omni/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/omni/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/omni/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/omni/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/cdaweb/omni/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/cdaweb/omni/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/esa_eo/swarm/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/esa_eo/swarm/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/fmi/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/fmi/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/fmi/image/ie/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/fmi/image/ie/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/fmi/image/ie/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/fmi/image/ie/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/fmi/image/ie/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/fmi/image/ie/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/fmi/image/ie/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/fmi/image/ie/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/hpo/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/hpo/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/hpo/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/hpo/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/hpo/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/hpo/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/hpo/nowcast/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/hpo/nowcast/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/hpo/nowcast/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/hpo/nowcast/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/hpo/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/hpo/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/nowcast/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/nowcast/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/nowcast/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/nowcast/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/nowcast/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/nowcast/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/nowcast/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/nowcast/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/kpap/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/kpap/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/snf107/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/snf107/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/snf107/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/snf107/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/gfz/snf107/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/gfz/snf107/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/ampere/fitted/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/ampere/fitted/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/ampere/fitted/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/ampere/fitted/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/ampere/fitted/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/ampere/fitted/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/ampere/grd/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/ampere/grd/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/gnss/tecmap/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/gnss/tecmap/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/gnss/tecmap/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/gnss/tecmap/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/gnss/tecmap/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/gnss/tecmap/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/gnss/tecmap/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/gnss/tecmap/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/eiscat_hdf5_info.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/eiscat_hdf5_info.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/utilities.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/utilities.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/eiscat/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/eiscat/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/madrigal/utilities.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/madrigal/utilities.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/nipr/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/nipr/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/nipr/asc/tro_wmi/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/nipr/asc/tro_wmi/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/nipr/asc/tro_wmi/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/nipr/asc/tro_wmi/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/nipr/asc/tro_wmi/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/nipr/asc/tro_wmi/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/superdarn/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/superdarn/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/superdarn/potmap/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/superdarn/potmap/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/superdarn/potmap/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/superdarn/potmap/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/superdarn/potmap/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/superdarn/potmap/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/superdarn/potmap/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/superdarn/potmap/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/supermag/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/supermag/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/supermag/indices/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/supermag/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/supermag/indices/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/supermag/indices/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/supermag/indices/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/supermag/indices/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/supermag/indices/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/supermag/indices/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/supermag/supermag_api.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/supermag/supermag_api.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/dns_acc/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/dns_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/dns_acc/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/dns_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/dns_acc/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/dns_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/dns_acc/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/dns_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/wnd_acc/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/wnd_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/wnd_acc/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/wnd_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/wnd_acc/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/wnd_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/champ/wnd_acc/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/champ/wnd_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/goce/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/goce/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/dns_acc/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/dns_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/dns_acc/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/dns_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/dns_acc/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/dns_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/dns_acc/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/dns_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/wnd_acc/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/wnd_acc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,24 +210,26 @@
             initial_file_dir = kwargs.pop(
                 'initial_file_dir', self.data_root_dir
             )
 
             file_patterns = [
                 'G' + self.sat_id.upper(),
                 self.product.upper().replace('-', '_'),
-                this_day.strftime('%Y_%m'),
+                this_day.strftime('%Y_%m'), 
+                self.product_version + '.txt'
             ]
             # remove empty str
             file_patterns = [pattern for pattern in file_patterns if str(pattern)]
             search_pattern = '*' + '*'.join(file_patterns) + '*'
 
             done = super().search_data_files(
                 initial_file_dir=initial_file_dir,
                 search_pattern=search_pattern,
                 allow_multiple_files=False,
+                include_extension=False,
             )
             # Validate file paths
 
             if (not done and self.allow_download) or self.force_download:
                 done = self.download_data()
                 if done:
                     initial_file_dir = self.data_root_dir
```

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/wnd_acc/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_acc/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 
 
 class Downloader(DownloaderModel):
 
     def __init__(
             self, dt_fr, dt_to,
             sat_id=None,
-            product='WND-ACC',
-            version='v02',
+            product='DNS-ACC',
+            version='v01',
             force=True, direct_download=True, **kwargs
     ):
         if version == 'v01':
-            raise ValueError
+            v_str = "version_01"
         elif version == 'v02':
             v_str = "version_02"
         else:
             raise NotImplementedError
-        data_file_root_dir = prf.datahub_data_root_dir / "TUD" / "GRACE" / product.upper() / version
-        ftp_data_dir = f'{v_str}/GRACE_data'
 
+        data_file_root_dir = prf.datahub_data_root_dir / "TUD" / "SWARM" / product.upper() / version
+        ftp_data_dir = f'{v_str}/Swarm_data'
         file_name_patterns = [sat_id.upper(), product.replace('-', '_')]
         super(Downloader, self).__init__(
             dt_fr, dt_to,
             data_file_root_dir=data_file_root_dir, ftp_data_dir=ftp_data_dir, force=force,
             direct_download=direct_download, file_name_patterns=file_name_patterns, **kwargs
         )
```

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/wnd_acc/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/wnd_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace/wnd_acc/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/wnd_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace_fo/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace_fo/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace_fo/dns_acc/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace_fo/dns_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace_fo/dns_acc/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace_fo/dns_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace_fo/dns_acc/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace_fo/dns_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/grace_fo/dns_acc/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace_fo/dns_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_acc/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_acc/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_pod/downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class Downloader(DownloaderModel):
 
     def __init__(
             self, dt_fr, dt_to,
             sat_id=None,
-            product='DNS-ACC',
+            product='DNS-POD',
             version='v01',
             force=True, direct_download=True, **kwargs
     ):
         if version == 'v01':
             v_str = "version_01"
         elif version == 'v02':
             v_str = "version_02"
```

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_acc/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_acc/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_pod/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_pod/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_pod/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/grace/wnd_acc/downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,27 +14,28 @@
 
 
 class Downloader(DownloaderModel):
 
     def __init__(
             self, dt_fr, dt_to,
             sat_id=None,
-            product='DNS-POD',
-            version='v01',
+            product='WND-ACC',
+            version='v02',
             force=True, direct_download=True, **kwargs
     ):
         if version == 'v01':
-            v_str = "version_01"
-        elif version == 'v02':
+            raise ValueError
+        elif 'v02' in version:
+            version_ = 'v02'
             v_str = "version_02"
         else:
             raise NotImplementedError
+        data_file_root_dir = prf.datahub_data_root_dir / "TUD" / "GRACE" / product.upper() / version_
+        ftp_data_dir = f'{v_str}/GRACE_data'
 
-        data_file_root_dir = prf.datahub_data_root_dir / "TUD" / "SWARM" / product.upper() / version
-        ftp_data_dir = f'{v_str}/Swarm_data'
         file_name_patterns = [sat_id.upper(), product.replace('-', '_')]
         super(Downloader, self).__init__(
             dt_fr, dt_to,
             data_file_root_dir=data_file_root_dir, ftp_data_dir=ftp_data_dir, force=force,
             direct_download=direct_download, file_name_patterns=file_name_patterns, **kwargs
         )
```

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_pod/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_pod/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/tud/swarm/dns_pod/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/tud/swarm/dns_pod/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/wdc/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/wdc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/wdc/ae/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/wdc/ae/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/wdc/ae/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/wdc/ae/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/wdc/ae/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/wdc/ae/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/wdc/ae/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/wdc/ae/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/wdc/asysym/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/wdc/asysym/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/wdc/asysym/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/wdc/asysym/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/wdc/asysym/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/wdc/asysym/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/wdc/asysym/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/wdc/asysym/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/wdc/dst/__init__.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/wdc/dst/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/wdc/dst/downloader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/wdc/dst/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/wdc/dst/loader.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/wdc/dst/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/datahub/sources/wdc/dst/variable_config.py` & `geospacelab-0.6.6/geospacelab/datahub/sources/wdc/dst/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/express/dmsp_dashboard.py` & `geospacelab-0.6.6/geospacelab/express/dmsp_dashboard.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/express/eiscat_dashboard.py` & `geospacelab-0.6.6/geospacelab/express/eiscat_dashboard.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/express/millstonehill_dashboard.py` & `geospacelab-0.6.6/geospacelab/express/millstonehill_dashboard.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/express/omni_dashboard.py` & `geospacelab-0.6.6/geospacelab/express/omni_dashboard.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/future/empiricalmodels/ovationprime2010/ovationprime.py` & `geospacelab-0.6.6/geospacelab/future/empiricalmodels/ovationprime2010/ovationprime.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/future/satllites/orbit_analyzer.py` & `geospacelab-0.6.6/geospacelab/future/satllites/orbit_analyzer.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/future/test_sscws.py` & `geospacelab-0.6.6/geospacelab/future/test_sscws.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/observatory/earth/_func.py` & `geospacelab-0.6.6/geospacelab/observatory/earth/_func.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/observatory/earth/geodesy.py` & `geospacelab-0.6.6/geospacelab/observatory/earth/geodesy.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/observatory/orbit/sc_orbit.py` & `geospacelab-0.6.6/geospacelab/observatory/orbit/sc_orbit.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/observatory/orbit/utilities.py` & `geospacelab-0.6.6/geospacelab/observatory/orbit/utilities.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/toolbox/io/dialog.py` & `geospacelab-0.6.6/geospacelab/toolbox/io/dialog.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/toolbox/utilities/numpyarray.py` & `geospacelab-0.6.6/geospacelab/toolbox/utilities/numpyarray.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/toolbox/utilities/numpymath.py` & `geospacelab-0.6.6/geospacelab/toolbox/utilities/numpymath.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/toolbox/utilities/pybasic.py` & `geospacelab-0.6.6/geospacelab/toolbox/utilities/pybasic.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/toolbox/utilities/pyclass.py` & `geospacelab-0.6.6/geospacelab/toolbox/utilities/pyclass.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/toolbox/utilities/pydatetime.py` & `geospacelab-0.6.6/geospacelab/toolbox/utilities/pydatetime.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/toolbox/utilities/pylogging.py` & `geospacelab-0.6.6/geospacelab/toolbox/utilities/pylogging.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/toolbox/utilities/pyos.py` & `geospacelab-0.6.6/geospacelab/toolbox/utilities/pyos.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/visualization/__init__.py` & `geospacelab-0.6.6/geospacelab/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/visualization/mpl/__base__.py` & `geospacelab-0.6.6/geospacelab/visualization/mpl/__base__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/visualization/mpl/__init__.py` & `geospacelab-0.6.6/geospacelab/visualization/mpl/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/visualization/mpl/_helpers.py` & `geospacelab-0.6.6/geospacelab/visualization/mpl/_helpers.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/visualization/mpl/axis_ticks.py` & `geospacelab-0.6.6/geospacelab/visualization/mpl/axis_ticks.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/visualization/mpl/colormaps.py` & `geospacelab-0.6.6/geospacelab/visualization/mpl/colormaps.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/visualization/mpl/dashboards.py` & `geospacelab-0.6.6/geospacelab/visualization/mpl/dashboards.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/visualization/mpl/figure.py` & `geospacelab-0.6.6/geospacelab/visualization/mpl/figure.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/visualization/mpl/geomap/__base__.py` & `geospacelab-0.6.6/geospacelab/visualization/mpl/geomap/__base__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/visualization/mpl/geomap/geodashboards.py` & `geospacelab-0.6.6/geospacelab/visualization/mpl/geomap/geodashboards.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/visualization/mpl/geomap/geopanels.py` & `geospacelab-0.6.6/geospacelab/visualization/mpl/geomap/geopanels.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/visualization/mpl/panels.py` & `geospacelab-0.6.6/geospacelab/visualization/mpl/panels.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/wrapper/geopack/LICENSE` & `geospacelab-0.6.6/geospacelab/wrapper/geopack/LICENSE`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/wrapper/geopack/README.md` & `geospacelab-0.6.6/geospacelab/wrapper/geopack/README.md`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/geopack.py` & `geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/geopack.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/igrf13coeffs.txt` & `geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/igrf13coeffs.txt`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/t01.py` & `geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/t01.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/t04.py` & `geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/t04.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/t89.py` & `geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/t89.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/t96.py` & `geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/t96.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/test_geopack1.md` & `geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/test_geopack1.md`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab/wrapper/geopack/geopack/test_geopack1.py` & `geospacelab-0.6.6/geospacelab/wrapper/geopack/geopack/test_geopack1.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/geospacelab.egg-info/PKG-INFO` & `geospacelab-0.6.6/geospacelab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geospacelab
-Version: 0.6.5
+Version: 0.6.6
 Summary: Collect, manage, and visualize geospace data.
 Home-page: https://github.com/JouleCai/geospacelab
 Author: Lei Cai
 Author-email: lei.cai@oulu.fi
 License: BSD 3-Clause License
 Keywords: Geospace,EISCAT,DMSP,Space weather,Ionosphere,Space,Magnetosphere
 Classifier: Development Status :: 4 - Beta
```

### Comparing `geospacelab-0.6.5/geospacelab.egg-info/SOURCES.txt` & `geospacelab-0.6.6/geospacelab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geospacelab-0.6.5/setup.py` & `geospacelab-0.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
               'scipy>=1.6.0',
               'h5py>=3.2.1',
               'netcdf4>=1.5.7',
               'matplotlib>=3.5',
               'madrigalweb>=3.2',
               'aacgmv2>=2.6.2',
               'cdflib>=0.3.20',
-              'geopack>=1.0.8',
+              'geopack>=1.0.10',
               'palettable',
               'toml',
               'sscws',
               'pandas>=1.5.3',
           ],
     python_requires='>=3.7',
     # py_modules=["geospacelab"],
```

