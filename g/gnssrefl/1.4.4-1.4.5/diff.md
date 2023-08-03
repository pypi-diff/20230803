# Comparing `tmp/gnssrefl-1.4.4.tar.gz` & `tmp/gnssrefl-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-1.4.4.tar", last modified: Wed Aug  2 22:33:25 2023, max compression
+gzip compressed data, was "gnssrefl-1.4.5.tar", last modified: Thu Aug  3 17:58:36 2023, max compression
```

## Comparing `gnssrefl-1.4.4.tar` & `gnssrefl-1.4.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:33:25.705357 gnssrefl-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 22:33:10.000000 gnssrefl-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 22:33:10.000000 gnssrefl-1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-02 22:33:25.705357 gnssrefl-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-02 22:33:10.000000 gnssrefl-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:33:25.685356 gnssrefl-1.4.4/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/check_rinex_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:33:25.685356 gnssrefl-1.4.4/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/decipher_argt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_qld.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/filesizes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16210 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gnssir.py
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gnssir_input.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    35025 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gnssir_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (123)   183744 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/make_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/make_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    28009 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/nmea2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/nyquist_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/nyquist_libs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34342 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19612 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/quickLook_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16994 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/quickLook_function2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5881 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/quickPhase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/quicklib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50791 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/rinex3_snr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/smoosh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/smoosh_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    60208 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    60672 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/vwc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/vwc_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    32905 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/xnmeasnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:33:25.685356 gnssrefl-1.4.4/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-02 22:33:25.000000 gnssrefl-1.4.4/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-02 22:33:25.000000 gnssrefl-1.4.4/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:33:25.000000 gnssrefl-1.4.4/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-02 22:33:25.000000 gnssrefl-1.4.4/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 22:33:25.000000 gnssrefl-1.4.4/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 22:33:25.000000 gnssrefl-1.4.4/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 22:33:25.705357 gnssrefl-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:33:25.705357 gnssrefl-1.4.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:58:36.578696 gnssrefl-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 17:58:22.000000 gnssrefl-1.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 17:58:22.000000 gnssrefl-1.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-03 17:58:36.578696 gnssrefl-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-03 17:58:22.000000 gnssrefl-1.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:58:36.558696 gnssrefl-1.4.5/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:58:36.558696 gnssrefl-1.4.5/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/decipher_argt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/download_qld.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/filesizes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16210 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/gnssir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/gnssir_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35040 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/gnssir_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (123)   183744 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/make_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/make_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28009 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/nmea2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/nyquist_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/nyquist_libs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34342 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19612 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/quickLook_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16994 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/quickLook_function2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5881 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/quickPhase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/quicklib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50791 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/rinex3_snr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/smoosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/smoosh_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60208 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60672 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/vwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/vwc_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32905 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/xnmeasnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:58:36.558696 gnssrefl-1.4.5/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-03 17:58:36.000000 gnssrefl-1.4.5/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-03 17:58:36.000000 gnssrefl-1.4.5/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:58:36.000000 gnssrefl-1.4.5/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-03 17:58:36.000000 gnssrefl-1.4.5/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 17:58:36.000000 gnssrefl-1.4.5/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 17:58:36.000000 gnssrefl-1.4.5/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:58:36.578696 gnssrefl-1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:58:36.578696 gnssrefl-1.4.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 17:58:23.000000 gnssrefl-1.4.5/test/test_rinex2snr.py
```

### Comparing `gnssrefl-1.4.4/LICENSE` & `gnssrefl-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/PKG-INFO` & `gnssrefl-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.4.4
+Version: 1.4.5
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.4.4** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.5** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 August 2, 2023: Updated azimuth outputs for gnssir and quickLook so that the azimuth of the 
 rising or setting part of the arc is reported rather than the average average, as was done in the older versions.
 
 July 7, 2023: The newarcs option had a bug in it: the refraction correction was not being applied.
 While the refraction correction is not very important for some applications (snow, soil moisture), using it sometimes and not
 using it other times IS NOT GOOD.  You will see a bias in time series when you switched. This bug is fixed as of version 1.4.1
```

### Comparing `gnssrefl-1.4.4/README.md` & `gnssrefl-1.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # gnssrefl
 
-**github version: 1.4.4** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.5** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 August 2, 2023: Updated azimuth outputs for gnssir and quickLook so that the azimuth of the 
 rising or setting part of the arc is reported rather than the average average, as was done in the older versions.
 
 July 7, 2023: The newarcs option had a bug in it: the refraction correction was not being applied.
 While the refraction correction is not very important for some applications (snow, soil moisture), using it sometimes and not
 using it other times IS NOT GOOD.  You will see a bias in time series when you switched. This bug is fixed as of version 1.4.1
```

### Comparing `gnssrefl-1.4.4/gnssrefl/EGM96.py` & `gnssrefl-1.4.5/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/check_rinex_file.py` & `gnssrefl-1.4.5/gnssrefl/check_rinex_file.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/computemp1mp2.py` & `gnssrefl-1.4.5/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/daily_avg.py` & `gnssrefl-1.4.5/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/daily_avg_cl.py` & `gnssrefl-1.4.5/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-1.4.5/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/decipher_argt.py` & `gnssrefl-1.4.5/gnssrefl/decipher_argt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/download_ioc.py` & `gnssrefl-1.4.5/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/download_noaa.py` & `gnssrefl-1.4.5/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/download_orbits.py` & `gnssrefl-1.4.5/gnssrefl/download_orbits.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/download_psmsl.py` & `gnssrefl-1.4.5/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/download_qld.py` & `gnssrefl-1.4.5/gnssrefl/download_qld.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/download_rinex.py` & `gnssrefl-1.4.5/gnssrefl/download_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/download_teqc.py` & `gnssrefl-1.4.5/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/download_tides.py` & `gnssrefl-1.4.5/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/download_unr.py` & `gnssrefl-1.4.5/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/download_wsv.py` & `gnssrefl-1.4.5/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/filesizes.py` & `gnssrefl-1.4.5/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/gnssir.py` & `gnssrefl-1.4.5/gnssrefl/gnssir.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/gnssir_cl.py` & `gnssrefl-1.4.5/gnssrefl/gnssir_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/gnssir_input.py` & `gnssrefl-1.4.5/gnssrefl/gnssir_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/gnssir_v2.py` & `gnssrefl-1.4.5/gnssrefl/gnssir_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -696,14 +696,15 @@
         edot factor used in RH dot correction
     delT : float
         arc length in minutes
 
     """
     x=[]; y=[]; azi=[]; seconds = []; edot = [] ; sat = []
     Nvv= 0; meanTime = 0; avgAzim = 0 ; outFact2 = 0 ; delT = 0
+    initA = 0;
     cf = g.arc_scaleF(f,satNu)
     outFact1 = 0 # backwards compatability
     good = True
 
     if f in [1,101,201,301]:
         column = 7
     elif f in [2,20,102,302]:
```

### Comparing `gnssrefl-1.4.4/gnssrefl/gnsssnr.f` & `gnssrefl-1.4.5/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/gnsssnrbigger.f` & `gnssrefl-1.4.5/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/gps.py` & `gnssrefl-1.4.5/gnssrefl/gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/gpssnr.f` & `gnssrefl-1.4.5/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/gpsweek.py` & `gnssrefl-1.4.5/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/gpt_1wA.pickle` & `gnssrefl-1.4.5/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/highrate.py` & `gnssrefl-1.4.5/gnssrefl/highrate.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/installexe_cl.py` & `gnssrefl-1.4.5/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/invsnr_cl.py` & `gnssrefl-1.4.5/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/invsnr_input.py` & `gnssrefl-1.4.5/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/karnak_libraries.py` & `gnssrefl-1.4.5/gnssrefl/karnak_libraries.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/kelly.py` & `gnssrefl-1.4.5/gnssrefl/kelly.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/llh2xyz.py` & `gnssrefl-1.4.5/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/make_json_input.py` & `gnssrefl-1.4.5/gnssrefl/make_json_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/make_meta.py` & `gnssrefl-1.4.5/gnssrefl/make_meta.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/nmea2snr.py` & `gnssrefl-1.4.5/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/nmea2snr_cl.py` & `gnssrefl-1.4.5/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/nyquist_cl.py` & `gnssrefl-1.4.5/gnssrefl/nyquist_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/nyquist_libs.py` & `gnssrefl-1.4.5/gnssrefl/nyquist_libs.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/phase_functions.py` & `gnssrefl-1.4.5/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/prn2gps.py` & `gnssrefl-1.4.5/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/query_unr.py` & `gnssrefl-1.4.5/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/quickLook_cl.py` & `gnssrefl-1.4.5/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/quickLook_function.py` & `gnssrefl-1.4.5/gnssrefl/quickLook_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/quickLook_function2.py` & `gnssrefl-1.4.5/gnssrefl/quickLook_function2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/quickPhase.py` & `gnssrefl-1.4.5/gnssrefl/quickPhase.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/quicklib.py` & `gnssrefl-1.4.5/gnssrefl/quicklib.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/quickplt.py` & `gnssrefl-1.4.5/gnssrefl/quickplt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/read_snr_files.py` & `gnssrefl-1.4.5/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/refl_zones.py` & `gnssrefl-1.4.5/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/refl_zones_cl.py` & `gnssrefl-1.4.5/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/refraction.py` & `gnssrefl-1.4.5/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/rh_plot.py` & `gnssrefl-1.4.5/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/rinex2snr.py` & `gnssrefl-1.4.5/gnssrefl/rinex2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/rinex2snr_cl.py` & `gnssrefl-1.4.5/gnssrefl/rinex2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/rinex3_rinex2.py` & `gnssrefl-1.4.5/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/rinex3_snr.py` & `gnssrefl-1.4.5/gnssrefl/rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/rinpy.py` & `gnssrefl-1.4.5/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-1.4.5/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/smoosh.py` & `gnssrefl-1.4.5/gnssrefl/smoosh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/smoosh_snr.py` & `gnssrefl-1.4.5/gnssrefl/smoosh_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/snow_functions.py` & `gnssrefl-1.4.5/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/snowdepth_cl.py` & `gnssrefl-1.4.5/gnssrefl/snowdepth_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/spline_functions.py` & `gnssrefl-1.4.5/gnssrefl/spline_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/subdaily.py` & `gnssrefl-1.4.5/gnssrefl/subdaily.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/subdaily_cl.py` & `gnssrefl-1.4.5/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/utils.py` & `gnssrefl-1.4.5/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/veg_multiyr.py` & `gnssrefl-1.4.5/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/vwc.py` & `gnssrefl-1.4.5/gnssrefl/vwc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/vwc_cl.py` & `gnssrefl-1.4.5/gnssrefl/vwc_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/vwc_input.py` & `gnssrefl-1.4.5/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/xnmeasnr.f` & `gnssrefl-1.4.5/gnssrefl/xnmeasnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/xyz2llh.py` & `gnssrefl-1.4.5/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/ydoy.py` & `gnssrefl-1.4.5/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl/ymd.py` & `gnssrefl-1.4.5/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-1.4.5/gnssrefl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.4.4
+Version: 1.4.5
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.4.4** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.5** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 August 2, 2023: Updated azimuth outputs for gnssir and quickLook so that the azimuth of the 
 rising or setting part of the arc is reported rather than the average average, as was done in the older versions.
 
 July 7, 2023: The newarcs option had a bug in it: the refraction correction was not being applied.
 While the refraction correction is not very important for some applications (snow, soil moisture), using it sometimes and not
 using it other times IS NOT GOOD.  You will see a bias in time series when you switched. This bug is fixed as of version 1.4.1
```

### Comparing `gnssrefl-1.4.4/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-1.4.5/gnssrefl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-1.4.5/gnssrefl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/pyproject.toml` & `gnssrefl-1.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.4/setup.py` & `gnssrefl-1.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "progress",
     "astropy",
     "simplekml",
     "earthscope-sdk",
 ]
 setup(
     name="gnssrefl",
-    version="1.4.4",
+    version="1.4.5",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
```

### Comparing `gnssrefl-1.4.4/test/test_gps.py` & `gnssrefl-1.4.5/test/test_gps.py`

 * *Files identical despite different names*

