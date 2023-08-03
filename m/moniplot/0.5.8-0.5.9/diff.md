# Comparing `tmp/moniplot-0.5.8.tar.gz` & `tmp/moniplot-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moniplot-0.5.8.tar", last modified: Tue Mar 28 11:46:43 2023, max compression
+gzip compressed data, was "moniplot-0.5.9.tar", last modified: Tue Mar 28 15:27:43 2023, max compression
```

## Comparing `moniplot-0.5.8.tar` & `moniplot-0.5.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 11:46:43.919589 moniplot-0.5.8/
--rw-r--r--   0 richardh  (1304) earth     (3300)      202 2023-03-28 10:04:14.000000 moniplot-0.5.8/.gitignore
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 11:46:43.915589 moniplot-0.5.8/.idea/
--rw-r--r--   0 richardh  (1304) earth     (3300)       47 2023-03-28 10:18:53.000000 moniplot-0.5.8/.idea/.gitignore
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 11:46:43.915589 moniplot-0.5.8/.idea/inspectionProfiles/
--rw-r--r--   0 richardh  (1304) earth     (3300)      228 2023-03-28 10:18:53.000000 moniplot-0.5.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 richardh  (1304) earth     (3300)      313 2023-03-28 10:36:32.000000 moniplot-0.5.8/.idea/misc.xml
--rw-r--r--   0 richardh  (1304) earth     (3300)      268 2023-03-28 10:18:52.000000 moniplot-0.5.8/.idea/modules.xml
--rw-r--r--   0 richardh  (1304) earth     (3300)      486 2023-03-28 10:36:32.000000 moniplot-0.5.8/.idea/moniplot.iml
--rw-r--r--   0 richardh  (1304) earth     (3300)      167 2023-03-28 10:18:53.000000 moniplot-0.5.8/.idea/vcs.xml
--rw-r--r--   0 richardh  (1304) earth     (3300)      175 2022-09-28 14:03:36.000000 moniplot-0.5.8/.readthedocs.yaml
--rw-r--r--   0 richardh  (1304) earth     (3300)      517 2022-09-20 11:28:02.000000 moniplot-0.5.8/CITATION.cff
--rw-r--r--   0 richardh  (1304) earth     (3300)      858 2022-07-06 10:22:13.000000 moniplot-0.5.8/INSTALL.md
--rw-r--r--   0 richardh  (1304) earth     (3300)    35149 2022-05-23 12:01:25.000000 moniplot-0.5.8/LICENSE
--rw-r--r--   0 richardh  (1304) earth     (3300)        0 2022-05-23 12:01:25.000000 moniplot-0.5.8/MANIFEST.in
--rw-r--r--   0 richardh  (1304) earth     (3300)     2906 2023-03-28 11:46:43.919589 moniplot-0.5.8/PKG-INFO
--rw-r--r--   0 richardh  (1304) earth     (3300)     1681 2022-10-03 12:37:31.000000 moniplot-0.5.8/README.md
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 11:46:43.915589 moniplot-0.5.8/docs/
--rw-r--r--   0 richardh  (1304) earth     (3300)      634 2022-09-28 08:51:14.000000 moniplot-0.5.8/docs/Makefile
--rw-r--r--   0 richardh  (1304) earth     (3300)     2055 2022-09-30 14:49:54.000000 moniplot-0.5.8/docs/build.rst
--rw-r--r--   0 richardh  (1304) earth     (3300)     2121 2023-02-16 13:24:55.000000 moniplot-0.5.8/docs/conf.py
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 11:46:43.919589 moniplot-0.5.8/docs/figures/
--rw-r--r--   0 richardh  (1304) earth     (3300)    61903 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_lplot-1.png
--rw-r--r--   0 richardh  (1304) earth     (3300)    59592 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_lplot-2.png
--rw-r--r--   0 richardh  (1304) earth     (3300)    61665 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_lplot-3.png
--rw-r--r--   0 richardh  (1304) earth     (3300)   172522 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_lplot-4.png
--rw-r--r--   0 richardh  (1304) earth     (3300)    45354 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_lplot-5.png
--rw-r--r--   0 richardh  (1304) earth     (3300)    65237 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_qhist-1.png
--rw-r--r--   0 richardh  (1304) earth     (3300)    38863 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_quality-1.png
--rw-r--r--   0 richardh  (1304) earth     (3300)    40640 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_quality-2.png
--rw-r--r--   0 richardh  (1304) earth     (3300)    31479 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_quality-3.png
--rw-r--r--   0 richardh  (1304) earth     (3300)   717829 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_signal-01.png
--rw-r--r--   0 richardh  (1304) earth     (3300)   752791 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_signal-02.png
--rw-r--r--   0 richardh  (1304) earth     (3300)   749139 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_signal-03.png
--rw-r--r--   0 richardh  (1304) earth     (3300)   700724 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_signal-04.png
--rw-r--r--   0 richardh  (1304) earth     (3300)   886685 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_signal-05.png
--rw-r--r--   0 richardh  (1304) earth     (3300)   675689 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_signal-06.png
--rw-r--r--   0 richardh  (1304) earth     (3300)   706166 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_signal-07.png
--rw-r--r--   0 richardh  (1304) earth     (3300)   510167 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_signal-08.png
--rw-r--r--   0 richardh  (1304) earth     (3300)   537227 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_signal-09.png
--rw-r--r--   0 richardh  (1304) earth     (3300)   628781 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_signal-10.png
--rw-r--r--   0 richardh  (1304) earth     (3300)   653521 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_signal-11.png
--rw-r--r--   0 richardh  (1304) earth     (3300)    84566 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/figures/mon_plot_draw_trend-1.png
--rw-r--r--   0 richardh  (1304) earth     (3300)      843 2022-09-29 13:27:07.000000 moniplot-0.5.8/docs/index.rst
--rw-r--r--   0 richardh  (1304) earth     (3300)      795 2022-09-28 08:51:14.000000 moniplot-0.5.8/docs/make.bat
--rw-r--r--   0 richardh  (1304) earth     (3300)       51 2022-09-28 09:12:05.000000 moniplot-0.5.8/docs/modules.rst
--rw-r--r--   0 richardh  (1304) earth     (3300)     1555 2022-09-28 09:12:05.000000 moniplot-0.5.8/docs/moniplot.lib.rst
--rw-r--r--   0 richardh  (1304) earth     (3300)      991 2023-03-28 10:04:14.000000 moniplot-0.5.8/docs/moniplot.rst
--rw-r--r--   0 richardh  (1304) earth     (3300)     3161 2022-10-17 07:24:06.000000 moniplot-0.5.8/docs/quick.rst
--rw-r--r--   0 richardh  (1304) earth     (3300)     1740 2023-02-16 14:12:22.000000 moniplot-0.5.8/pyproject.toml
--rw-r--r--   0 richardh  (1304) earth     (3300)      437 2023-03-28 11:41:43.000000 moniplot-0.5.8/requirement.txt
--rw-r--r--   0 richardh  (1304) earth     (3300)      239 2023-03-28 11:46:43.919589 moniplot-0.5.8/setup.cfg
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 11:46:43.911589 moniplot-0.5.8/src/
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 11:46:43.919589 moniplot-0.5.8/src/moniplot/
--rw-r--r--   0 richardh  (1304) earth     (3300)     1075 2023-03-28 10:04:14.000000 moniplot-0.5.8/src/moniplot/__init__.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     7463 2023-03-28 10:23:07.000000 moniplot-0.5.8/src/moniplot/biweight.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    12175 2023-03-28 10:23:07.000000 moniplot-0.5.8/src/moniplot/image_to_xarray.py
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 11:46:43.919589 moniplot-0.5.8/src/moniplot/lib/
--rw-r--r--   0 richardh  (1304) earth     (3300)        0 2022-05-23 12:01:25.000000 moniplot-0.5.8/src/moniplot/lib/__init__.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    16137 2023-03-28 10:04:14.000000 moniplot-0.5.8/src/moniplot/lib/fig_draw_image.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     3543 2023-03-28 10:04:14.000000 moniplot-0.5.8/src/moniplot/lib/fig_draw_lplot.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     3668 2023-03-28 10:04:14.000000 moniplot-0.5.8/src/moniplot/lib/fig_draw_multiplot.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     2256 2023-03-28 10:04:14.000000 moniplot-0.5.8/src/moniplot/lib/fig_draw_qhist.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     2596 2023-03-28 10:04:14.000000 moniplot-0.5.8/src/moniplot/lib/fig_draw_tracks.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    11166 2023-03-28 10:04:14.000000 moniplot-0.5.8/src/moniplot/lib/fig_draw_trend.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     3671 2023-03-28 10:04:14.000000 moniplot-0.5.8/src/moniplot/lib/fig_info.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     1215 2022-10-20 08:35:24.000000 moniplot-0.5.8/src/moniplot/lib/fig_legend.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    53699 2023-03-28 10:04:14.000000 moniplot-0.5.8/src/moniplot/mon_plot.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    15695 2023-03-28 10:04:14.000000 moniplot-0.5.8/src/moniplot/tol_colors.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     1254 2022-11-07 10:30:05.000000 moniplot-0.5.8/src/moniplot/unbiased_std.py
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 11:46:43.919589 moniplot-0.5.8/src/moniplot.egg-info/
--rw-r--r--   0 richardh  (1304) earth     (3300)     2906 2023-03-28 11:46:43.000000 moniplot-0.5.8/src/moniplot.egg-info/PKG-INFO
--rw-r--r--   0 richardh  (1304) earth     (3300)     1953 2023-03-28 11:46:43.000000 moniplot-0.5.8/src/moniplot.egg-info/SOURCES.txt
--rw-r--r--   0 richardh  (1304) earth     (3300)        1 2023-03-28 11:46:43.000000 moniplot-0.5.8/src/moniplot.egg-info/dependency_links.txt
--rw-r--r--   0 richardh  (1304) earth     (3300)      168 2023-03-28 11:46:43.000000 moniplot-0.5.8/src/moniplot.egg-info/requires.txt
--rw-r--r--   0 richardh  (1304) earth     (3300)        9 2023-03-28 11:46:43.000000 moniplot-0.5.8/src/moniplot.egg-info/top_level.txt
-drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 11:46:43.919589 moniplot-0.5.8/tests/
--rw-r--r--   0 richardh  (1304) earth     (3300)     6909 2023-03-28 11:32:52.000000 moniplot-0.5.8/tests/test_layout.py
--rw-r--r--   0 richardh  (1304) earth     (3300)     1677 2023-03-28 11:20:25.000000 moniplot-0.5.8/tests/test_lplot.py
--rw-r--r--   0 richardh  (1304) earth     (3300)    12642 2023-03-28 11:17:49.000000 moniplot-0.5.8/tests/test_mon_plot.py
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:27:43.031128 moniplot-0.5.9/
+-rw-r--r--   0 richardh  (1304) earth     (3300)      202 2023-03-28 10:04:14.000000 moniplot-0.5.9/.gitignore
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:27:43.027128 moniplot-0.5.9/.idea/
+-rw-r--r--   0 richardh  (1304) earth     (3300)       47 2023-03-28 15:17:29.000000 moniplot-0.5.9/.idea/.gitignore
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:27:43.027128 moniplot-0.5.9/.idea/inspectionProfiles/
+-rw-r--r--   0 richardh  (1304) earth     (3300)      228 2023-03-28 15:17:29.000000 moniplot-0.5.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      313 2023-03-28 15:17:29.000000 moniplot-0.5.9/.idea/misc.xml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      268 2023-03-28 15:17:29.000000 moniplot-0.5.9/.idea/modules.xml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      486 2023-03-28 15:17:29.000000 moniplot-0.5.9/.idea/moniplot.iml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      167 2023-03-28 15:17:29.000000 moniplot-0.5.9/.idea/vcs.xml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      175 2022-09-28 14:03:36.000000 moniplot-0.5.9/.readthedocs.yaml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      517 2022-09-20 11:28:02.000000 moniplot-0.5.9/CITATION.cff
+-rw-r--r--   0 richardh  (1304) earth     (3300)      858 2022-07-06 10:22:13.000000 moniplot-0.5.9/INSTALL.md
+-rw-r--r--   0 richardh  (1304) earth     (3300)    35149 2022-05-23 12:01:25.000000 moniplot-0.5.9/LICENSE
+-rw-r--r--   0 richardh  (1304) earth     (3300)        0 2022-05-23 12:01:25.000000 moniplot-0.5.9/MANIFEST.in
+-rw-r--r--   0 richardh  (1304) earth     (3300)     2906 2023-03-28 15:27:43.031128 moniplot-0.5.9/PKG-INFO
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1681 2022-10-03 12:37:31.000000 moniplot-0.5.9/README.md
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:27:43.027128 moniplot-0.5.9/docs/
+-rw-r--r--   0 richardh  (1304) earth     (3300)      634 2022-09-28 08:51:14.000000 moniplot-0.5.9/docs/Makefile
+-rw-r--r--   0 richardh  (1304) earth     (3300)     2055 2022-09-30 14:49:54.000000 moniplot-0.5.9/docs/build.rst
+-rw-r--r--   0 richardh  (1304) earth     (3300)     2121 2023-02-16 13:24:55.000000 moniplot-0.5.9/docs/conf.py
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:27:43.031128 moniplot-0.5.9/docs/figures/
+-rw-r--r--   0 richardh  (1304) earth     (3300)    61903 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_lplot-1.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)    59592 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_lplot-2.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)    61665 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_lplot-3.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)   172522 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_lplot-4.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)    45354 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_lplot-5.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)    65237 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_qhist-1.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)    38863 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_quality-1.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)    40640 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_quality-2.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)    31479 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_quality-3.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)   717829 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_signal-01.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)   752791 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_signal-02.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)   749139 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_signal-03.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)   700724 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_signal-04.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)   886685 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_signal-05.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)   675689 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_signal-06.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)   706166 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_signal-07.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)   510167 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_signal-08.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)   537227 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_signal-09.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)   628781 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_signal-10.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)   653521 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_signal-11.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)    84566 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/figures/mon_plot_draw_trend-1.png
+-rw-r--r--   0 richardh  (1304) earth     (3300)      843 2022-09-29 13:27:07.000000 moniplot-0.5.9/docs/index.rst
+-rw-r--r--   0 richardh  (1304) earth     (3300)      795 2022-09-28 08:51:14.000000 moniplot-0.5.9/docs/make.bat
+-rw-r--r--   0 richardh  (1304) earth     (3300)       51 2022-09-28 09:12:05.000000 moniplot-0.5.9/docs/modules.rst
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1555 2022-09-28 09:12:05.000000 moniplot-0.5.9/docs/moniplot.lib.rst
+-rw-r--r--   0 richardh  (1304) earth     (3300)      991 2023-03-28 10:04:14.000000 moniplot-0.5.9/docs/moniplot.rst
+-rw-r--r--   0 richardh  (1304) earth     (3300)     3161 2022-10-17 07:24:06.000000 moniplot-0.5.9/docs/quick.rst
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1591 2023-03-28 15:17:29.000000 moniplot-0.5.9/pyproject.toml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      435 2023-03-28 15:17:29.000000 moniplot-0.5.9/requirements.txt
+-rw-r--r--   0 richardh  (1304) earth     (3300)      239 2023-03-28 15:27:43.031128 moniplot-0.5.9/setup.cfg
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:27:43.023128 moniplot-0.5.9/src/
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:27:43.031128 moniplot-0.5.9/src/moniplot/
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1075 2023-03-28 10:04:14.000000 moniplot-0.5.9/src/moniplot/__init__.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     7463 2023-03-28 15:17:29.000000 moniplot-0.5.9/src/moniplot/biweight.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    12175 2023-03-28 15:17:29.000000 moniplot-0.5.9/src/moniplot/image_to_xarray.py
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:27:43.031128 moniplot-0.5.9/src/moniplot/lib/
+-rw-r--r--   0 richardh  (1304) earth     (3300)        0 2022-05-23 12:01:25.000000 moniplot-0.5.9/src/moniplot/lib/__init__.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    16137 2023-03-28 10:04:14.000000 moniplot-0.5.9/src/moniplot/lib/fig_draw_image.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     3543 2023-03-28 10:04:14.000000 moniplot-0.5.9/src/moniplot/lib/fig_draw_lplot.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     3668 2023-03-28 10:04:14.000000 moniplot-0.5.9/src/moniplot/lib/fig_draw_multiplot.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     2256 2023-03-28 10:04:14.000000 moniplot-0.5.9/src/moniplot/lib/fig_draw_qhist.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     2596 2023-03-28 10:04:14.000000 moniplot-0.5.9/src/moniplot/lib/fig_draw_tracks.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    11166 2023-03-28 10:04:14.000000 moniplot-0.5.9/src/moniplot/lib/fig_draw_trend.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     3671 2023-03-28 10:04:14.000000 moniplot-0.5.9/src/moniplot/lib/fig_info.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1215 2022-10-20 08:35:24.000000 moniplot-0.5.9/src/moniplot/lib/fig_legend.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    53699 2023-03-28 10:04:14.000000 moniplot-0.5.9/src/moniplot/mon_plot.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    15695 2023-03-28 10:04:14.000000 moniplot-0.5.9/src/moniplot/tol_colors.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1254 2022-11-07 10:30:05.000000 moniplot-0.5.9/src/moniplot/unbiased_std.py
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:27:43.031128 moniplot-0.5.9/src/moniplot.egg-info/
+-rw-r--r--   0 richardh  (1304) earth     (3300)     2906 2023-03-28 15:27:42.000000 moniplot-0.5.9/src/moniplot.egg-info/PKG-INFO
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1954 2023-03-28 15:27:43.000000 moniplot-0.5.9/src/moniplot.egg-info/SOURCES.txt
+-rw-r--r--   0 richardh  (1304) earth     (3300)        1 2023-03-28 15:27:42.000000 moniplot-0.5.9/src/moniplot.egg-info/dependency_links.txt
+-rw-r--r--   0 richardh  (1304) earth     (3300)      118 2023-03-28 15:27:42.000000 moniplot-0.5.9/src/moniplot.egg-info/requires.txt
+-rw-r--r--   0 richardh  (1304) earth     (3300)        9 2023-03-28 15:27:42.000000 moniplot-0.5.9/src/moniplot.egg-info/top_level.txt
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-03-28 15:27:43.031128 moniplot-0.5.9/tests/
+-rw-r--r--   0 richardh  (1304) earth     (3300)     6909 2023-03-28 15:17:29.000000 moniplot-0.5.9/tests/test_layout.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1677 2023-03-28 15:17:29.000000 moniplot-0.5.9/tests/test_lplot.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    12642 2023-03-28 15:17:29.000000 moniplot-0.5.9/tests/test_mon_plot.py
```

### Comparing `moniplot-0.5.8/CITATION.cff` & `moniplot-0.5.9/CITATION.cff`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/INSTALL.md` & `moniplot-0.5.9/INSTALL.md`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/LICENSE` & `moniplot-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/PKG-INFO` & `moniplot-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moniplot
-Version: 0.5.8
+Version: 0.5.9
 Summary: moniplot is a Python data visualization library for (satellite) instrument monitoring
 Author-email: Richard van Hees <R.M.van.Hees@sron.nl>, Paul Tol <P.J.J.Tol@sron.nl>
 License: GPL-3.0-only
 Project-URL: homepage, https://github.com/rmvanhees/moniplot
 Project-URL: documentation, https://moniplot.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/rmvanhees/moniplot/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `moniplot-0.5.8/README.md` & `moniplot-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/Makefile` & `moniplot-0.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/build.rst` & `moniplot-0.5.9/docs/build.rst`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/conf.py` & `moniplot-0.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_lplot-1.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_lplot-1.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_lplot-2.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_lplot-2.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_lplot-3.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_lplot-3.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_lplot-4.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_lplot-4.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_lplot-5.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_lplot-5.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_qhist-1.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_qhist-1.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_quality-1.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_quality-1.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_quality-2.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_quality-2.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_quality-3.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_quality-3.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_signal-01.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_signal-01.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_signal-02.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_signal-02.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_signal-03.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_signal-03.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_signal-04.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_signal-04.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_signal-05.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_signal-05.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_signal-06.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_signal-06.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_signal-07.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_signal-07.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_signal-08.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_signal-08.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_signal-09.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_signal-09.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_signal-10.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_signal-10.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_signal-11.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_signal-11.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/figures/mon_plot_draw_trend-1.png` & `moniplot-0.5.9/docs/figures/mon_plot_draw_trend-1.png`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/index.rst` & `moniplot-0.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/make.bat` & `moniplot-0.5.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/moniplot.lib.rst` & `moniplot-0.5.9/docs/moniplot.lib.rst`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/moniplot.rst` & `moniplot-0.5.9/docs/moniplot.rst`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/docs/quick.rst` & `moniplot-0.5.9/docs/quick.rst`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/pyproject.toml` & `moniplot-0.5.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -25,22 +25,20 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering :: Atmospheric Science",
   "Topic :: Scientific/Engineering :: Visualization"
 ]
 requires-python = ">=3.8"
 dependencies = [
-  # "cartopy>=0.21",
-  "h5py~=2.10.0; python_version=='3.9'",
-  "h5py>=3.5; python_version!='3.9'",
-  "matplotlib~=3.3.4; python_version=='3.9'",
-  "matplotlib>=3.5; python_version!='3.9'",
-  "numpy>=1.19",
-  "xarray~=0.19.0; python_version=='3.9'",
-  "xarray>=2022.3; python_version!='3.9'",
+  "importlib-resources>5.8; python_version=='3.8'",
+  "h5py>=3.7",
+  "matplotlib>=3.5",
+  # "Cartopy>0.21",
+  "numpy>=1.23",
+  "xarray>=2022.3"
 ]
 
 [project.urls]
 homepage = "https://github.com/rmvanhees/moniplot"
 documentation = "https://moniplot.readthedocs.io/en/latest/"
 # Source = "https://github.com/rmvanhees/moniplot"
 # Changelog = "https://github.com/rmvanhees/moniplot/HISTORY.rst"
```

### Comparing `moniplot-0.5.8/src/moniplot/__init__.py` & `moniplot-0.5.9/src/moniplot/__init__.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/src/moniplot/biweight.py` & `moniplot-0.5.9/src/moniplot/biweight.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/src/moniplot/image_to_xarray.py` & `moniplot-0.5.9/src/moniplot/image_to_xarray.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/src/moniplot/lib/fig_draw_image.py` & `moniplot-0.5.9/src/moniplot/lib/fig_draw_image.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/src/moniplot/lib/fig_draw_lplot.py` & `moniplot-0.5.9/src/moniplot/lib/fig_draw_lplot.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/src/moniplot/lib/fig_draw_multiplot.py` & `moniplot-0.5.9/src/moniplot/lib/fig_draw_multiplot.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/src/moniplot/lib/fig_draw_qhist.py` & `moniplot-0.5.9/src/moniplot/lib/fig_draw_qhist.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/src/moniplot/lib/fig_draw_tracks.py` & `moniplot-0.5.9/src/moniplot/lib/fig_draw_tracks.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/src/moniplot/lib/fig_draw_trend.py` & `moniplot-0.5.9/src/moniplot/lib/fig_draw_trend.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/src/moniplot/lib/fig_info.py` & `moniplot-0.5.9/src/moniplot/lib/fig_info.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/src/moniplot/lib/fig_legend.py` & `moniplot-0.5.9/src/moniplot/lib/fig_legend.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/src/moniplot/mon_plot.py` & `moniplot-0.5.9/src/moniplot/mon_plot.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/src/moniplot/tol_colors.py` & `moniplot-0.5.9/src/moniplot/tol_colors.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/src/moniplot/unbiased_std.py` & `moniplot-0.5.9/src/moniplot/unbiased_std.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/src/moniplot.egg-info/PKG-INFO` & `moniplot-0.5.9/src/moniplot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moniplot
-Version: 0.5.8
+Version: 0.5.9
 Summary: moniplot is a Python data visualization library for (satellite) instrument monitoring
 Author-email: Richard van Hees <R.M.van.Hees@sron.nl>, Paul Tol <P.J.J.Tol@sron.nl>
 License: GPL-3.0-only
 Project-URL: homepage, https://github.com/rmvanhees/moniplot
 Project-URL: documentation, https://moniplot.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/rmvanhees/moniplot/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `moniplot-0.5.8/src/moniplot.egg-info/SOURCES.txt` & `moniplot-0.5.9/src/moniplot.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .readthedocs.yaml
 CITATION.cff
 INSTALL.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-requirement.txt
+requirements.txt
 setup.cfg
 .idea/.gitignore
 .idea/misc.xml
 .idea/modules.xml
 .idea/moniplot.iml
 .idea/vcs.xml
 .idea/inspectionProfiles/profiles_settings.xml
```

### Comparing `moniplot-0.5.8/tests/test_layout.py` & `moniplot-0.5.9/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/tests/test_lplot.py` & `moniplot-0.5.9/tests/test_lplot.py`

 * *Files identical despite different names*

### Comparing `moniplot-0.5.8/tests/test_mon_plot.py` & `moniplot-0.5.9/tests/test_mon_plot.py`

 * *Files identical despite different names*

