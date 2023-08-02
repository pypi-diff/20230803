# Comparing `tmp/gnssrefl-1.4.3.tar.gz` & `tmp/gnssrefl-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-1.4.3.tar", last modified: Mon Jul 17 14:04:19 2023, max compression
+gzip compressed data, was "gnssrefl-1.4.4.tar", last modified: Wed Aug  2 22:33:25 2023, max compression
```

## Comparing `gnssrefl-1.4.3.tar` & `gnssrefl-1.4.4.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:04:19.010497 gnssrefl-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-17 14:04:19.010497 gnssrefl-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:04:18.982496 gnssrefl-1.4.3/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/gnssrefl/check_rinex_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-17 14:04:00.000000 gnssrefl-1.4.3/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:04:18.982496 gnssrefl-1.4.3/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/decipher_argt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/filesizes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16210 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gnssir.py
--rw-r--r--   0 runner    (1001) docker     (123)    13093 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gnssir_input.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33744 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gnssir_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (123)   183142 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/make_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/make_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    28009 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/nmea2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/nyquist_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/nyquist_libs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34342 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19612 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/quickLook_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16994 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/quickLook_function2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5881 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/quickPhase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/quicklib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50791 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/rinex3_snr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/smoosh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/smoosh_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    60208 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    60672 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/vwc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/vwc_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    32905 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/xnmeasnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:04:18.982496 gnssrefl-1.4.3/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-17 14:04:18.000000 gnssrefl-1.4.3/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-17 14:04:18.000000 gnssrefl-1.4.3/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:04:18.000000 gnssrefl-1.4.3/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-17 14:04:18.000000 gnssrefl-1.4.3/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 14:04:18.000000 gnssrefl-1.4.3/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 14:04:18.000000 gnssrefl-1.4.3/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:04:19.010497 gnssrefl-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:04:19.010497 gnssrefl-1.4.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-17 14:04:01.000000 gnssrefl-1.4.3/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:33:25.705357 gnssrefl-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 22:33:10.000000 gnssrefl-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 22:33:10.000000 gnssrefl-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-02 22:33:25.705357 gnssrefl-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-02 22:33:10.000000 gnssrefl-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:33:25.685356 gnssrefl-1.4.4/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:33:25.685356 gnssrefl-1.4.4/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/decipher_argt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_qld.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/filesizes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16210 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gnssir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gnssir_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35025 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gnssir_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (123)   183744 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/make_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/make_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28009 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/nmea2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/nyquist_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/nyquist_libs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34342 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19612 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/quickLook_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16994 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/quickLook_function2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5881 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/quickPhase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/quicklib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50791 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/rinex3_snr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/smoosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/smoosh_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60208 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60672 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/vwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/vwc_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32905 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/xnmeasnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:33:25.685356 gnssrefl-1.4.4/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-02 22:33:25.000000 gnssrefl-1.4.4/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-02 22:33:25.000000 gnssrefl-1.4.4/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:33:25.000000 gnssrefl-1.4.4/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-02 22:33:25.000000 gnssrefl-1.4.4/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 22:33:25.000000 gnssrefl-1.4.4/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 22:33:25.000000 gnssrefl-1.4.4/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 22:33:25.705357 gnssrefl-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:33:25.705357 gnssrefl-1.4.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-02 22:33:11.000000 gnssrefl-1.4.4/test/test_rinex2snr.py
```

### Comparing `gnssrefl-1.4.3/LICENSE` & `gnssrefl-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/PKG-INFO` & `gnssrefl-1.4.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.4.3
+Version: 1.4.4
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
 
-**github version: 1.4.3** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.4** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+
+August 2, 2023: Updated azimuth outputs for gnssir and quickLook so that the azimuth of the 
+rising or setting part of the arc is reported rather than the average average, as was done in the older versions.
 
 July 7, 2023: The newarcs option had a bug in it: the refraction correction was not being applied.
 While the refraction correction is not very important for some applications (snow, soil moisture), using it sometimes and not
 using it other times IS NOT GOOD.  You will see a bias in time series when you switched. This bug is fixed as of version 1.4.1
 I will be removing all versions (1.3.16 up to 1.4.1) from pypi that have this bug. If you were 
 using the newarcs option in the last month, you need to rerun gnssir and any 
 downstream codes (subdaily, daily_avg etc). This bug has
```

### Comparing `gnssrefl-1.4.3/README.md` & `gnssrefl-1.4.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # gnssrefl
 
-**github version: 1.4.3** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.4** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+
+August 2, 2023: Updated azimuth outputs for gnssir and quickLook so that the azimuth of the 
+rising or setting part of the arc is reported rather than the average average, as was done in the older versions.
 
 July 7, 2023: The newarcs option had a bug in it: the refraction correction was not being applied.
 While the refraction correction is not very important for some applications (snow, soil moisture), using it sometimes and not
 using it other times IS NOT GOOD.  You will see a bias in time series when you switched. This bug is fixed as of version 1.4.1
 I will be removing all versions (1.3.16 up to 1.4.1) from pypi that have this bug. If you were 
 using the newarcs option in the last month, you need to rerun gnssir and any 
 downstream codes (subdaily, daily_avg etc). This bug has
```

### Comparing `gnssrefl-1.4.3/gnssrefl/EGM96.py` & `gnssrefl-1.4.4/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/check_rinex_file.py` & `gnssrefl-1.4.4/gnssrefl/check_rinex_file.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/computemp1mp2.py` & `gnssrefl-1.4.4/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/daily_avg.py` & `gnssrefl-1.4.4/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/daily_avg_cl.py` & `gnssrefl-1.4.4/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-1.4.4/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/decipher_argt.py` & `gnssrefl-1.4.4/gnssrefl/decipher_argt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/download_ioc.py` & `gnssrefl-1.4.4/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/download_noaa.py` & `gnssrefl-1.4.4/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/download_orbits.py` & `gnssrefl-1.4.4/gnssrefl/download_orbits.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,17 +71,17 @@
 
             esa : ESA, multi-GNSS
 
             gfr : GFZ rapid, GPS, Galileo and Glonass, since May 17 2021
 
             wum : (disabled) Wuhan, multi-GNSS, not rapid
 
-            gnss2 : multi-GNSS, but uses IGN instead of CDDIS
+            gnss2 : multi-GNSS, but uses IGN instead of CDDIS. does not work
 
-            gnss3 : multi-GNSS, but uses GFZ archive instead of CDDIS
+            gnss3 : multi-GNSS, but uses GFZ archive instead of CDDIS. same as gnss-gfz
 
             ultra : ultra orbits directly from GFZ
 
             rapid : rapid orbits directly from GFZ
 
     year : integer
         full year
@@ -94,15 +94,15 @@
 
     """
 
 #   make sure environment variables exist.  set to current directory if not
     g.check_environ_variables()
 
     orbit_list = ['igs', 'igr', 'jax', 'grg', 'wum', 'gbm', 'nav', 'gps', 'gps+glo', 
-            'gnss', 'gfr', 'esa', 'gnss2', 'gnss3','ultra', 'rapid','nav-esa', 'nav-sopac','nav-cddis']
+            'gnss', 'gfr', 'esa', 'gnss2', 'gnss3','gnss-gfz','ultra', 'rapid','nav-esa', 'nav-sopac','nav-cddis']
 
 #   assign to normal variables
     pCtr = orbit
 
     if len(str(year)) != 4:
         print('Year must have four characters: ', year)
         sys.exit()
@@ -162,19 +162,20 @@
                     filename, fdir, foundit = g.getsp3file_flex(year, month, day, pCtr)
                 elif pCtr == 'gfr':
                 # rapid GFZ is available again ...
                     filename, fdir, foundit = g.rapid_gfz_orbits(year, month, day)
                 elif pCtr == 'ultra':
                     hour = 0 # for now only download hour 0 for ultra products
                     filename, fdir, foundit = g.ultra_gfz_orbits(year, month, day, hour)
-                elif pCtr == 'gnss3':
+                elif (pCtr == 'gnss3') or (pCtr == 'gnss-gfz'):
                 # use GFZ archive instead of CDDIS
                     filename, fdir, foundit = g.gbm_orbits_direct(year, month, day)
                 elif pCtr == 'gnss2':
                 # use IGN instead of CDDIS
+                    print('To my knowledge, this option no longer works')
                     filename, fdir, foundit = g.avoid_cddis(year, month, day)
                 else:
                     filename, fdir, foundit = g.getsp3file_mgex(year, month, day, pCtr)
             if foundit:
                 print('SUCCESS:', fdir+'/'+filename)
             else:
                 print(filename, ' not found')
```

### Comparing `gnssrefl-1.4.3/gnssrefl/download_psmsl.py` & `gnssrefl-1.4.4/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/download_rinex.py` & `gnssrefl-1.4.4/gnssrefl/download_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/download_teqc.py` & `gnssrefl-1.4.4/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/download_tides.py` & `gnssrefl-1.4.4/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/download_unr.py` & `gnssrefl-1.4.4/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/download_wsv.py` & `gnssrefl-1.4.4/gnssrefl/download_wsv.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     fout.write("% 1   2  3   4  5  6     7      8     9  \n")
 
 
     for i in range(0, N):
         sl = float(data[i]['value'])/100 # change to meters
         t = data[i]['timestamp']
         o=datetime.datetime.fromisoformat(t)
+        #print(o)
         ts = datetime.datetime.utctimetuple(o)
         #    print(ts.tm_year, ts.tm_mon, ts.tm_mday, ts.tm_hour, ts.tm_min, ts.tm_sec, ts.tm_yday)
         year = ts.tm_year ; mm  = ts.tm_mon ; dd =  ts.tm_mday
         hh = ts.tm_hour ; minutes = ts.tm_min ; sec = ts.tm_sec
         doy = ts.tm_yday
         # calcualte MJD
         m, f = g.mjd(year, mm, dd, hh, minutes, sec)
```

### Comparing `gnssrefl-1.4.3/gnssrefl/filesizes.py` & `gnssrefl-1.4.4/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/gnssir.py` & `gnssrefl-1.4.4/gnssrefl/gnssir.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/gnssir_cl.py` & `gnssrefl-1.4.4/gnssrefl/gnssir_cl.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         If changed here, then it overrides what you requested in the json. default is 0.
     azim2 : int, optional
         upper limit azimuth.
         If the azimuth angles are changed in the json (using 'azval' key) and not changed here, then the json overrides these.
         If changed here, then it overrides what you requested in the json. default is 360.
     nooverwrite : bool, optional
         Use to overwrite lomb scargle result files or not.
-        Default is True (do not overwrite files).
+        Default is False, i.e., it will overwrite.
     extension : string, optional
         extension for result file, useful for testing strategies. default is empty string
     compress : boolean, optional
         xz compress SNR files after use. default is False.
     screenstats : bool, optional
         whether to print stats to the screen or not. default is True.
     delTmax : int, optional
```

### Comparing `gnssrefl-1.4.3/gnssrefl/gnssir_input.py` & `gnssrefl-1.4.4/gnssrefl/gnssir_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/gnssir_v2.py` & `gnssrefl-1.4.4/gnssrefl/gnssir_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     """
 
     Computes lomb scargle periodograms for a given station, year, day of year etc.
 
     Arcs are determined differently than in the first version of the code, which
     was quadrant based. This identifies arcs and applies azimuth constraints after the fact.
 
+    2023-aug-02 trying to fix the issue with azimuth print out being different than
+    azimuth at lowest elevation angle
+
     Parameters
     ----------
     station : string
         4 character station name
     year : integer
         full year
     doy : integer
@@ -192,14 +195,16 @@
 
                     # allow more than one set of elevation angles
                     if len(ellist) > 0:
                         arclist = np.empty(shape=[0,6])
                         for ij in range(0,len(ellist),2):
                             te1 = ellist[ij]; te2 = ellist[ij+1]; newl = [te1,te2]
                             # poorly named inputs - elev, azimuth, seconds of the day, ...
+                            # te1 and te2 are the requested elevation angles I believe
+                            # satNu is the requested satellite number
                             tarclist = new_rise_set_again(thissat[:,1],thissat[:,2],thissat[:,3],te1, te2,ediff,satNu,screenstats)
                             arclist = np.append(arclist, tarclist,axis=0)
 
                     else:
                         arclist = new_rise_set_again(thissat[:,1],thissat[:,2],thissat[:,3],e1, e2,ediff,satNu,screenstats)
 
                     nr,nc = arclist.shape
@@ -214,15 +219,15 @@
                     for a in range(0,nr):
                         sind = int(arclist[a,0]) ; eind = int(arclist[a,1])
                         #if screenstats:
                         #    print('Indices for this arc', a, sind, eind)
                         # create array for the requested arc
                         d2 = np.array(thissat[sind:eind, :], dtype=float)
                         # window the data - which also removes DC 
-                        # try this ... 
+                        # this is saying that these are the min and max elev angles you should be using
                         e1 = arclist[a,4]; e2 = arclist[a,5]
                         x,y, Nvv, cf, meanTime,avgAzim,outFact1, Edot2, delT= window_new(d2, f, 
                                 satNu,ncols,pele, lsp['polyV'],e1,e2,azvalues,screenstats)
                         Nv = Nvv # number of points
                         UTCtime = meanTime
 
                         if (delT != 0):
@@ -243,14 +248,17 @@
 
                             if abs(maxF - minH) < 0.10: #  peak too close to min value
                                 tooclose = True
 
                             if abs(maxF - maxH) < 0.10: #  peak too close to max value
                                 tooclose = True
 
+                            if False:
+                                print(avgAzim, satNu, e1, e2)
+
                             if (not tooclose) & (delT < delTmax) & (maxAmp > reqAmp[ct]) & (maxAmp/Noise > PkNoise):
                             # request from a tide gauge person for Month, Day, Hour, Minute
 
                                 if lsp['mmdd']:
                                     ctime = g.nicerTime(UTCtime); ctime2 = ctime[0:2] + ' ' + ctime[3:5]
                                     fout.write(" {0:4.0f} {1:3.0f} {2:6.3f} {3:3.0f} {4:6.3f} {5:6.2f} {6:6.2f} {7:6.2f} {8:6.2f} {9:4.0f} {10:3.0f} {11:2.0f} {12:8.5f} {13:6.2f} {14:7.2f} {15:12.6f} {16:1.0f} {17:2.0f} {18:2.0f} {19:5s} \n".format(year,doy,maxF,satNu, UTCtime, avgAzim,maxAmp,eminObs,emaxObs,Nv, f,riseSet, Edot2, maxAmp/Noise, delT, MJD,irefr,month,day,ctime2)) 
                                 else:
@@ -638,14 +646,16 @@
 
 
 def window_new(snrD, f, satNu,ncols,pele,pfitV,e1,e2,azlist,screenstats):
     """
     retrieves SNR arcs for a given satellite. returns elevation angle and 
     detrended linear SNR
 
+    2023-aug02 updated to improve azimuth calculation reported
+
     Parameters
     ----------
     snrD : numpy array (multiD)
         contents of the snr file, i.e. 0 column is satellite numbers, 1 column elevation angle ...
     f : int
         frequency you want
     satNu : int
@@ -653,17 +663,17 @@
     ncols : int
         how many columns does the SNR file have
     pele : list of floats
         elevation angles for polynomial fit
     pfitV : float
         polynomial order
     e1 : float
-        min elev angle (deg)
+        requested min elev angle (deg)
     e2 : float
-        max elev angle (deg)
+        requested max elev angle (deg)
     azlist : list of floats (deg)
         non-continguous azimuth regions, corrected for negative regions
     screenstats : bool
         whether you want debugging information
 
     Returns
     -------
@@ -674,15 +684,16 @@
     Nvv :  int
         number of points in x/y array
     cf : float
         scale factor for requested frequency (used in LSP)
     meanTime : float
         UTC hour of the day (GPS time)
     avgAzim : float
-        azimuth of the arc (deg)
+        average azimuth of the arc (deg) 
+        ### this will not be entirely consistent with other metric
     outFact1: float
         kept for backwards compatibility.  set to zero
     outFact2 : float
         edot factor used in RH dot correction
     delT : float
         arc length in minutes
 
@@ -740,14 +751,15 @@
                 # arbitrary
                 Nvv = len(ele[i])
                 if Nvv > 15:
                     # get the index of the min elevation angle
                     ie = np.argmin(ele[i])
                     # find the azimuth of that first elevation angle 
                     initA = azm[i][ie]
+                    #print('initial azimuth ostensibly for min eangle',initA)
                     keeparc = check_azim_compliance(initA,azlist)
                     if keeparc :
                         x = ele[i] ; y = data[i]
                         edot = edot[i]
                         sat = sat[i] ; azm = azm[i]
                         seconds = seconds[i]
                     else:
@@ -783,15 +795,19 @@
     # average tan(elev)
             cunit = np.mean(np.tan(np.pi*x/180))
     #       return tan(e)/edot, in units of one over (radians/hour) now. used for RHdot correction
     #       so when multiplyed by RHdot - which would be meters/hours ===>>> you will get a meter correction
     
             outFact2 = cunit/(avgEdot_fit*3600)
 
-    return x,y, Nvv, cf, meanTime,avgAzim,outFact1, outFact2, delT
+    # This originally returned the average azimuth.
+    # I think you can return the initA instead of avgAzim here
+    #    return x,y, Nvv, cf, meanTime,avgAzim,outFact1, outFact2, delT
+    #print('new ', initA, ' old ', avgAzim)
+    return x,y, Nvv, cf, meanTime,initA, outFact1, outFact2, delT
 
 
 def find_mgnss_satlist(f,year,doy):
     """
     find satellite list for a given frequency and date
 
     Parameters
@@ -921,33 +937,35 @@
     elv : numpy array  of floats
         elevation angles from SNR file
     azm : numpy array  of floats
         azimuth angles from SNR file
     dates : numpy array  of floats
         seconds of the day from SNR file
     e1 : float
-        min eval
+        min elevation angle (deg)
     e2 : float
-        max eval
+        max elevation angle (deg)
     ediff : float
-        el angle difference QC
+        el angle difference required, deg, QC
     sat : int
         satellite number
+    screenstats : bool
+        whether you want info printed to the screen
 
     Returns
     -------
     tv : numpy array
         beginning and ending indices of the arc
         satellite number, arc number, elev min, elev max
 
     """
     # require arcs to be this length in elev angle
     min_deg = (e2-ediff)   - (e1 + ediff)
 
-#   time limit in seconds - taken from david
+#   time limit in seconds - taken from david purnell
     gaptlim = 5*60 # seems awfully small
     #newf = np.array(f[i, :], dtype=float)
     iarc = 0
     ddate = np.ediff1d(dates)
     delv = np.ediff1d(elv)
     bkpt = len(ddate)
     bkpt = np.append(bkpt, np.where(ddate > gaptlim)[0])
@@ -965,14 +983,16 @@
         eind = bkpt[ii] + 1
         nelv = np.array(elv[sind:eind], dtype=float)
         nazm = np.array(azm[sind:eind], dtype=float)
         nt = np.array(dates[sind:eind], dtype=float)
         #nazm = azm[sind:eind]
         minObse = min(nelv)
         maxObse = max(nelv)
+        #print('min/max obs e ', minObse, maxObse)
+        # how to get the azimuth?
 
         nogood = False
         verysmall = False
         ediff_violation = False
         if (minObse - e1) > ediff:
             nogood = True
             ediff_violation = True 
@@ -996,10 +1016,12 @@
                     print('Failed sat/arc',sat,iarc+1, sind,eind,' min/max elev: ', np.round(minObse,2), np.round(maxObse,2), add)
             else:
                 print('Keep   sat/arc',sat,iarc+1, sind,eind,' min/max elev: ', np.round(minObse,2), np.round(maxObse,2))
 
         if not nogood :
             iarc = iarc + 1
             newl = [sind, eind, int(sat), iarc,e1,e2]
+            #print('indices ',sind, eind, elv[sind], elv[eind] )
+            #print('indices ',sind, eind, elv[sind], elv[eind], azm[sind], azm[eind])
             tv = np.append(tv, [newl],axis=0)
 
     return tv
```

### Comparing `gnssrefl-1.4.3/gnssrefl/gnsssnr.f` & `gnssrefl-1.4.4/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/gnsssnrbigger.f` & `gnssrefl-1.4.4/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/gps.py` & `gnssrefl-1.4.4/gnssrefl/gps.py`

 * *Files 1% similar despite different names*

```diff
@@ -3470,15 +3470,15 @@
         snrexe = gnssSNR_version() ; warn_and_exit(snrexe,fortran)
     elif (orbtype == 'gfr'):
         f,orbdir,foundit=rapid_gfz_orbits(year,month,day)
         snrexe = gnssSNR_version() ; warn_and_exit(snrexe,fortran)
     elif (orbtype == 'rapid'):
         f,orbdir,foundit=rapid_gfz_orbits(year,month,day)
         snrexe = gnssSNR_version() ; warn_and_exit(snrexe,fortran)
-    elif (orbtype == 'gnss3'):
+    elif (orbtype == 'gnss3') or (orbtype == 'gnss-gfz'):
         f,orbdir,foundit=gbm_orbits_direct(year,month,day)
         snrexe = gnssSNR_version() ; warn_and_exit(snrexe,fortran)
     elif (orbtype == 'sp3'):
         #print('uses default IGS orbits, so only GPS ?')
         f,orbdir,foundit=getsp3file_flex(year,month,day,'igs')
         snrexe = gnssSNR_version() ; warn_and_exit(snrexe,fortran)
     elif (orbtype == 'gfz'):
@@ -5067,14 +5067,33 @@
             hatanaka_warning()
 
 
 def avoid_cddis(year,month,day):
     """
     work around for people that can't use CDDIS ftps
     this will get multi-GNSS files for GFZ from the IGN
+    hopefully
+
+    Parameters
+    ----------
+    year : int 
+        full year
+    month : int
+        month of the year
+    day : int
+        calendar day
+    Returns
+    -------
+    filename : str
+        name of the orbit file
+    fdir : str
+        where the orbit file is stored
+    foundit : bool
+        whether it was found or not
+
     """
     fdir = os.environ['ORBITS'] + '/' + str(year) + '/sp3/'
     doy,cdoy,cyyyy,cyy = ymd2doy(year,month,day)
     foundit = False; 
     wk,swk = kgpsweek(year, month, day, 0,0,0)
     cwk = '{:04d}'.format(wk); cday = str(int(swk/86400))
     # old file name for precise files
@@ -6233,21 +6252,26 @@
     foundit = False
     return_name = ''
 
     month, day, doy, cyyyy, cyy, cdoy = ymd2ch(year,month,day)
     gpsweek,sec=kgpsweek(year,month,day,0,0,0)
     cgpsweek = str(gpsweek)
 
-    gns = 'ftp://ftp.gfz-potsdam.de/pub/GNSS/products/mgex/' + cgpsweek + '/'
+    # they changed during 2245 ... 
+    if (gpsweek < 2245):
+        gns = 'ftp://ftp.gfz-potsdam.de/pub/GNSS/products/mgex/' + cgpsweek + '/'
+    else:
+        gns = 'ftp://ftp.gfz-potsdam.de/pub/GNSS/products/mgex/' + cgpsweek + '_IGS20/'
 
     fdir = os.environ['ORBITS'] + '/' + cyyyy + '/sp3'
     littlename = 'gbm' + str(gpsweek) + str(int(sec/86400)) + '.sp3'
     bigname = 'GFZ0MGXRAP_' + cyyyy + cdoy + '0000_01D_05M_ORB.SP3'
 
     bigname2 = 'GBM0MGXRAP_' + cyyyy + cdoy + '0000_01D_05M_ORB.SP3'
+    print(bigname, bigname2)
 
     # first, do you have it locally?  
     # look for compressed file
     fullname = fdir + '/' + littlename 
     if os.path.isfile(fullname):
         foundit = True
         return_name = littlename
@@ -6267,23 +6291,26 @@
             return_name = littlename
 
     # checked for the first kind of name because that is how it was stored on CDDIS.
     # now use the name as how it is stored at GFZ.  I think
     bigname = bigname2 
     if not foundit:
         url = gns + littlename + '.Z'
+        print(url)
         try:
             wget.download(url,littlename + '.Z')
             subprocess.call(['uncompress', littlename + '.Z'])
         except:
             okok = 1
+
         if os.path.isfile(littlename):
             foundit = True ; return_name = littlename
         else:
             url = gns + bigname + '.gz'
+            print(url)
             try:
                 wget.download(url,bigname + '.gz')
                 subprocess.call(['gunzip', bigname + '.gz'])
                 foundit = True ; return_name = bigname
             except:
                 okok = 1
```

### Comparing `gnssrefl-1.4.3/gnssrefl/gpssnr.f` & `gnssrefl-1.4.4/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/gpsweek.py` & `gnssrefl-1.4.4/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/gpt_1wA.pickle` & `gnssrefl-1.4.4/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/highrate.py` & `gnssrefl-1.4.4/gnssrefl/highrate.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/installexe_cl.py` & `gnssrefl-1.4.4/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/invsnr_cl.py` & `gnssrefl-1.4.4/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/invsnr_input.py` & `gnssrefl-1.4.4/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/karnak_libraries.py` & `gnssrefl-1.4.4/gnssrefl/karnak_libraries.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/kelly.py` & `gnssrefl-1.4.4/gnssrefl/kelly.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/llh2xyz.py` & `gnssrefl-1.4.4/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/make_json_input.py` & `gnssrefl-1.4.4/gnssrefl/make_json_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/make_meta.py` & `gnssrefl-1.4.4/gnssrefl/make_meta.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/nmea2snr.py` & `gnssrefl-1.4.4/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/nmea2snr_cl.py` & `gnssrefl-1.4.4/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/nyquist_cl.py` & `gnssrefl-1.4.4/gnssrefl/nyquist_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/nyquist_libs.py` & `gnssrefl-1.4.4/gnssrefl/nyquist_libs.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,21 +92,24 @@
     Parameters
     ----------
     station : str
         4 char station name
 
     allN : numpy array ?
         azimuth and nyquist answers
+    info : str
+        information for the title
 
     Returns
     -------
     pngfile : str
         name of plot file
 
     """
+    # wavelengths in meters, being lazy
     l2 = 0.24421
     l5 = 0.254828048
     l1 = 0.19029360
     #fig = Figure(figsize=(8,4),dpi=360)
     #fig,ax = fig.subplots()
     fig, ax = plt.subplots(figsize=(10,6))
     ax.plot(allN[:,0],allN[:,1],'bo',label='L1')
@@ -120,19 +123,27 @@
     ax.legend(loc="upper right")
     if ("REFL_CODE" in os.environ):
         xdir = os.environ['REFL_CODE'] + '/Files/' + station + '/'
     else:
         xdir = './'
     pngfile = xdir + station + '_nyquist.png'
     plt.show()
-
-
-    fig.savefig(pngfile, format="png")
     print('pngfile stored in: ', pngfile)
+    fig.savefig(pngfile, format="png")
 
+    txtfile = xdir + station + '_nyquist.txt'
+    print(txtfile)
+    nr,nc = allN.shape
+    N = len(allN)
+    fout = open(txtfile, 'w+')
+    fout.write('{0:s}  {1:s} \n'.format('%', station + ' ' + info ))
+    for i in range(0,N):
+        fout.write('{0:7.2f}  {1:7.2f} \n'.format(allN[i,0], allN[i,1]))
+    fout.close()
+    print('Writing txtfile to ', txtfile)
 
 def read_the_orbits(obsfile,constel):
     """
     Parameters
     ----------
     obsfile : str
         name of the orbit file to be read
```

### Comparing `gnssrefl-1.4.3/gnssrefl/phase_functions.py` & `gnssrefl-1.4.4/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/prn2gps.py` & `gnssrefl-1.4.4/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/query_unr.py` & `gnssrefl-1.4.4/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/quickLook_cl.py` & `gnssrefl-1.4.4/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/quickLook_function.py` & `gnssrefl-1.4.4/gnssrefl/quickLook_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/quickLook_function2.py` & `gnssrefl-1.4.4/gnssrefl/quickLook_function2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/quickPhase.py` & `gnssrefl-1.4.4/gnssrefl/quickPhase.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/quicklib.py` & `gnssrefl-1.4.4/gnssrefl/quicklib.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/quickplt.py` & `gnssrefl-1.4.4/gnssrefl/quickplt.py`

 * *Files 11% similar despite different names*

```diff
@@ -177,15 +177,25 @@
     if args.ylimits is not None:
         print('found y-axis limits')
         ylimits = args.ylimits
         plt.ylim((ylimits))
     if args.xlimits is not None:
         print('found x-axis limits')
         xlimits = args.xlimits
-        plt.xlim((xlimits))
+        if convert_mjd:
+            t1 = Time(xlimits[0],format='mjd')
+            t1_utc = t1.utc # change to UTC
+            tval1 =  t1_utc.datetime # change to datetime
+            t2 = Time(xlimits[1],format='mjd')
+            t2_utc = t2.utc # change to UTC
+            tval2 =  t2_utc.datetime # change to datetime
+            plt.xlim((tval1,tval2))
+
+        else:
+            plt.xlim((xlimits))
 
     if args.outfile is not None:
         plt.savefig(args.outfile,dpi=300)
 
     plt.show()
```

### Comparing `gnssrefl-1.4.3/gnssrefl/read_snr_files.py` & `gnssrefl-1.4.4/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/refl_zones.py` & `gnssrefl-1.4.4/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/refl_zones_cl.py` & `gnssrefl-1.4.4/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/refraction.py` & `gnssrefl-1.4.4/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/rh_plot.py` & `gnssrefl-1.4.4/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/rinex2snr.py` & `gnssrefl-1.4.4/gnssrefl/rinex2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/rinex2snr_cl.py` & `gnssrefl-1.4.4/gnssrefl/rinex2snr_cl.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
             gps (default) : will use GPS broadcast orbit
 
             gps+glos : will use JAXA orbits which have GPS and Glonass (usually available in 48 hours)
 
             gnss : use GFZ final orbits, which is multi-GNSS (available in 3-4 days?), but from CDDIS archive
 
-            gnss3 : GFZ orbits downloaded from GFZ instead of CDDIS, but do they include beidou?
+            gnss-gfz : GFZ orbits downloaded from GFZ instead of CDDIS, but do they include beidou?. Same as gnss3?
 
             nav : GPS broadcast, perfectly adequate for reflectometry. Same as gps.
 
             igs : IGS precise, GPS only
 
             igr : IGS rapid, GPS only
 
@@ -271,15 +271,15 @@
     if len(str(year)) != 4:
         print('Year must be four characters long. Exiting.', year)
         sys.exit()
 
     # currently allowed orbit types - shanghai removed 2020sep08
     #
     orbit_list = ['gps', 'gps+glo', 'gnss', 'nav', 'igs', 'igr', 'jax', 'gbm',
-                  'grg', 'wum', 'gfr', 'esa', 'ultra', 'rapid', 'gnss2','nav-sopac','nav-esa','nav-cddis','gnss3']
+                  'grg', 'wum', 'gfr', 'esa', 'ultra', 'rapid', 'gnss2','nav-sopac','nav-esa','nav-cddis','gnss3','gnss-gfz']
     if orb not in orbit_list:
         print('You picked an orbit type I do not recognize. Here are the ones I allow')
         print(orbit_list)
         print('Exiting')
         sys.exit()
 
     # if you choose GPS, you get the nav message
@@ -289,15 +289,15 @@
     if orb == 'rapid':
         orb = 'gfr'
 
     # if you choose GNSS, you get the GFZ sp3 file  (precise)
     # I think gbm should be changed to 'gnss3' though perhaps not here
     if orb == 'gnss':
         orb = 'gbm'
-        print('Using GBM orbit')
+        print('Using GBM orbit archived at CDDIS')
 
 
     # get orbit from IGS
     if orb == 'gnss2':
         # this code wants year month day....
         year, month, day = g.ydoy2ymd(year, doy)
         filename, fdir, foundit = g.avoid_cddis(year, month, day)
```

### Comparing `gnssrefl-1.4.3/gnssrefl/rinex3_rinex2.py` & `gnssrefl-1.4.4/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/rinex3_snr.py` & `gnssrefl-1.4.4/gnssrefl/rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/rinpy.py` & `gnssrefl-1.4.4/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-1.4.4/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/smoosh.py` & `gnssrefl-1.4.4/gnssrefl/smoosh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/smoosh_snr.py` & `gnssrefl-1.4.4/gnssrefl/smoosh_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/snow_functions.py` & `gnssrefl-1.4.4/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/snowdepth_cl.py` & `gnssrefl-1.4.4/gnssrefl/snowdepth_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/spline_functions.py` & `gnssrefl-1.4.4/gnssrefl/spline_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/subdaily.py` & `gnssrefl-1.4.4/gnssrefl/subdaily.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/subdaily_cl.py` & `gnssrefl-1.4.4/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/utils.py` & `gnssrefl-1.4.4/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/veg_multiyr.py` & `gnssrefl-1.4.4/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/vwc.py` & `gnssrefl-1.4.4/gnssrefl/vwc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/vwc_cl.py` & `gnssrefl-1.4.4/gnssrefl/vwc_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/vwc_input.py` & `gnssrefl-1.4.4/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/xnmeasnr.f` & `gnssrefl-1.4.4/gnssrefl/xnmeasnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/xyz2llh.py` & `gnssrefl-1.4.4/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/ydoy.py` & `gnssrefl-1.4.4/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl/ymd.py` & `gnssrefl-1.4.4/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-1.4.4/gnssrefl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.4.3
+Version: 1.4.4
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
 
-**github version: 1.4.3** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.4** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+
+August 2, 2023: Updated azimuth outputs for gnssir and quickLook so that the azimuth of the 
+rising or setting part of the arc is reported rather than the average average, as was done in the older versions.
 
 July 7, 2023: The newarcs option had a bug in it: the refraction correction was not being applied.
 While the refraction correction is not very important for some applications (snow, soil moisture), using it sometimes and not
 using it other times IS NOT GOOD.  You will see a bias in time series when you switched. This bug is fixed as of version 1.4.1
 I will be removing all versions (1.3.16 up to 1.4.1) from pypi that have this bug. If you were 
 using the newarcs option in the last month, you need to rerun gnssir and any 
 downstream codes (subdaily, daily_avg etc). This bug has
```

### Comparing `gnssrefl-1.4.3/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-1.4.4/gnssrefl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 gnssrefl/daily_avg.py
 gnssrefl/daily_avg_cl.py
 gnssrefl/decipher_argt.py
 gnssrefl/download_ioc.py
 gnssrefl/download_noaa.py
 gnssrefl/download_orbits.py
 gnssrefl/download_psmsl.py
+gnssrefl/download_qld.py
 gnssrefl/download_rinex.py
 gnssrefl/download_teqc.py
 gnssrefl/download_tides.py
 gnssrefl/download_unr.py
 gnssrefl/download_wsv.py
 gnssrefl/filesizes.py
 gnssrefl/gnssir.py
```

### Comparing `gnssrefl-1.4.3/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-1.4.4/gnssrefl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/pyproject.toml` & `gnssrefl-1.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.3/setup.py` & `gnssrefl-1.4.4/setup.py`

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
-    version="1.4.3",
+    version="1.4.4",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
```

### Comparing `gnssrefl-1.4.3/test/test_gps.py` & `gnssrefl-1.4.4/test/test_gps.py`

 * *Files identical despite different names*

